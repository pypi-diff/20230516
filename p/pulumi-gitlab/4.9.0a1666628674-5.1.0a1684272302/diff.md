# Comparing `tmp/pulumi_gitlab-4.9.0a1666628674.tar.gz` & `tmp/pulumi_gitlab-5.1.0a1684272302.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-4.9.0a1666628674.tar", last modified: Mon Oct 24 16:29:17 2022, max compression
+gzip compressed data, was "pulumi_gitlab-5.1.0a1684272302.tar", last modified: Tue May 16 21:32:18 2023, max compression
```

## Comparing `pulumi_gitlab-4.9.0a1666628674.tar` & `pulumi_gitlab-5.1.0a1684272302.tar`

### file list

```diff
@@ -1,122 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (121)    15068 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41789 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)   690957 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    19660 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (121)    30500 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)    13955 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)    19017 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    12989 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    15428 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (121)    18697 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4050 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (121)     5799 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    13528 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    37320 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (121)    13666 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    24426 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)    30589 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (121)     6569 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (121)     8568 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6653 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    24027 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    16997 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    11124 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (121)    50120 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (121)    23419 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)    33679 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    10032 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    46605 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    12990 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (121)    21224 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    20006 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)    11204 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    14114 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    21008 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    34419 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    13356 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (121)    13496 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/managed_license.py
--rw-r--r--   0 runner    (1001) docker     (121)   143765 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20048 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    16323 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)    13430 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     9919 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)   207341 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    22325 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    21004 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    14991 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)    36176 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    18418 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    13439 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (121)    43374 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    74557 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)    23095 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (121)    14008 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)    25238 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)    19969 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (121)    15179 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    17670 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    21758 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    16195 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    21523 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    30915 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    24337 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    15306 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (121)    18963 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (121)    45107 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (121)    37739 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)    15484 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (121)    59413 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (121)    21890 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    10971 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)    20056 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (121)    32444 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    13260 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    15378 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/cluster_agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44219 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_user_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23419 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12990 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21008 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16259 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13356 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/managed_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164830 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20146 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16323 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263073 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22570 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23095 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24116 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45107 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37942 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59665 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:32:18.976014 pulumi_gitlab-5.1.0a1684272302/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-16 21:32:18.000000 pulumi_gitlab-5.1.0a1684272302/setup.py
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/PKG-INFO` & `pulumi_gitlab-5.1.0a1684272302/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 4.9.0a1666628674
+Version: 5.1.0a1684272302
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v4/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -42,15 +43,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v4
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/README.md` & `pulumi_gitlab-5.1.0a1684272302/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v4/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -31,15 +31,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v4
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/__init__.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .application import *
 from .application_settings import *
 from .branch import *
 from .branch_protection import *
 from .cluster_agent import *
 from .cluster_agent_token import *
 from .deploy_key import *
 from .deploy_key_enable import *
 from .deploy_token import *
+from .get_application import *
 from .get_branch import *
 from .get_cluster_agent import *
 from .get_cluster_agents import *
 from .get_current_user import *
 from .get_group import *
 from .get_group_hook import *
 from .get_group_hooks import *
 from .get_group_membership import *
+from .get_group_subgroups import *
 from .get_group_variable import *
 from .get_group_variables import *
+from .get_groups import *
 from .get_instance_deploy_keys import *
 from .get_instance_variable import *
 from .get_instance_variables import *
+from .get_metadata import *
 from .get_project import *
+from .get_project_branches import *
 from .get_project_hook import *
 from .get_project_hooks import *
 from .get_project_issue import *
 from .get_project_issues import *
 from .get_project_membership import *
 from .get_project_milestone import *
 from .get_project_milestones import *
@@ -42,14 +48,15 @@
 from .get_project_variables import *
 from .get_projects import *
 from .get_release_link import *
 from .get_release_links import *
 from .get_repository_file import *
 from .get_repository_tree import *
 from .get_user import *
+from .get_user_sshkeys import *
 from .get_users import *
 from .group import *
 from .group_access_token import *
 from .group_badge import *
 from .group_cluster import *
 from .group_custom_attribute import *
 from .group_hook import *
@@ -60,14 +67,15 @@
 from .group_saml_link import *
 from .group_share_group import *
 from .group_variable import *
 from .instance_cluster import *
 from .instance_variable import *
 from .label import *
 from .managed_license import *
+from .pages_domain import *
 from .personal_access_token import *
 from .pipeline_schedule import *
 from .pipeline_schedule_variable import *
 from .pipeline_trigger import *
 from .project import *
 from .project_access_token import *
 from .project_approval_rule import *
@@ -88,14 +96,16 @@
 from .project_share_group import *
 from .project_tag import *
 from .project_variable import *
 from .provider import *
 from .release_link import *
 from .repository_file import *
 from .runner import *
+from .service_custom_issue_tracker import *
+from .service_emails_on_push import *
 from .service_external_wiki import *
 from .service_github import *
 from .service_jira import *
 from .service_microsoft_teams import *
 from .service_pipelines_email import *
 from .service_slack import *
 from .system_hook import *
@@ -116,14 +126,22 @@
     config = _utilities.lazy_import('pulumi_gitlab.config')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "gitlab",
+  "mod": "index/application",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/application:Application": "Application"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/applicationSettings",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/applicationSettings:ApplicationSettings": "ApplicationSettings"
   }
  },
  {
@@ -316,14 +334,22 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/managedLicense:ManagedLicense": "ManagedLicense"
   }
  },
  {
   "pkg": "gitlab",
+  "mod": "index/pagesDomain",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/pagesDomain:PagesDomain": "PagesDomain"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/personalAccessToken",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/personalAccessToken:PersonalAccessToken": "PersonalAccessToken"
   }
  },
  {
@@ -532,14 +558,30 @@
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/runner:Runner": "Runner"
   }
  },
  {
   "pkg": "gitlab",
+  "mod": "index/serviceCustomIssueTracker",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/serviceCustomIssueTracker:ServiceCustomIssueTracker": "ServiceCustomIssueTracker"
+  }
+ },
+ {
+  "pkg": "gitlab",
+  "mod": "index/serviceEmailsOnPush",
+  "fqn": "pulumi_gitlab",
+  "classes": {
+   "gitlab:index/serviceEmailsOnPush:ServiceEmailsOnPush": "ServiceEmailsOnPush"
+  }
+ },
+ {
+  "pkg": "gitlab",
   "mod": "index/serviceExternalWiki",
   "fqn": "pulumi_gitlab",
   "classes": {
    "gitlab:index/serviceExternalWiki:ServiceExternalWiki": "ServiceExternalWiki"
   }
  },
  {
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,33 +381,40 @@
 
 @pulumi.input_type
 class ProjectContainerExpirationPolicyArgs:
     def __init__(__self__, *,
                  cadence: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  keep_n: Optional[pulumi.Input[int]] = None,
+                 name_regex: Optional[pulumi.Input[str]] = None,
                  name_regex_delete: Optional[pulumi.Input[str]] = None,
                  name_regex_keep: Optional[pulumi.Input[str]] = None,
                  next_run_at: Optional[pulumi.Input[str]] = None,
                  older_than: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] cadence: The cadence of the policy. Valid values are: `1d`, `7d`, `14d`, `1month`, `3month`.
         :param pulumi.Input[bool] enabled: If true, the policy is enabled.
         :param pulumi.Input[int] keep_n: The number of images to keep.
-        :param pulumi.Input[str] name_regex_delete: The regular expression to match image names to delete. **Note**: the upstream API has some inconsistencies with the `name_regex` field here. It's basically unusable at the moment.
+        :param pulumi.Input[str] name_regex: The regular expression to match image names to delete.
+        :param pulumi.Input[str] name_regex_delete: The regular expression to match image names to delete.
         :param pulumi.Input[str] name_regex_keep: The regular expression to match image names to keep.
         :param pulumi.Input[str] next_run_at: The next time the policy will run.
         :param pulumi.Input[str] older_than: The number of days to keep images.
         """
         if cadence is not None:
             pulumi.set(__self__, "cadence", cadence)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if keep_n is not None:
             pulumi.set(__self__, "keep_n", keep_n)
+        if name_regex is not None:
+            pulumi.set(__self__, "name_regex", name_regex)
+        if name_regex_delete is not None:
+            warnings.warn("""`name_regex_delete` has been deprecated. Use `name_regex` instead.""", DeprecationWarning)
+            pulumi.log.warn("""name_regex_delete is deprecated: `name_regex_delete` has been deprecated. Use `name_regex` instead.""")
         if name_regex_delete is not None:
             pulumi.set(__self__, "name_regex_delete", name_regex_delete)
         if name_regex_keep is not None:
             pulumi.set(__self__, "name_regex_keep", name_regex_keep)
         if next_run_at is not None:
             pulumi.set(__self__, "next_run_at", next_run_at)
         if older_than is not None:
@@ -446,18 +453,30 @@
         return pulumi.get(self, "keep_n")
 
     @keep_n.setter
     def keep_n(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "keep_n", value)
 
     @property
+    @pulumi.getter(name="nameRegex")
+    def name_regex(self) -> Optional[pulumi.Input[str]]:
+        """
+        The regular expression to match image names to delete.
+        """
+        return pulumi.get(self, "name_regex")
+
+    @name_regex.setter
+    def name_regex(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name_regex", value)
+
+    @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> Optional[pulumi.Input[str]]:
         """
-        The regular expression to match image names to delete. **Note**: the upstream API has some inconsistencies with the `name_regex` field here. It's basically unusable at the moment.
+        The regular expression to match image names to delete.
         """
         return pulumi.get(self, "name_regex_delete")
 
     @name_regex_delete.setter
     def name_regex_delete(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_regex_delete", value)
 
@@ -718,15 +737,15 @@
         """
         :param pulumi.Input[str] author_email_regex: All commit author emails must match this regex, e.g. `@my-company.com$`.
         :param pulumi.Input[str] branch_name_regex: All branch names must match this regex, e.g. `(feature|hotfix)\\/*`.
         :param pulumi.Input[bool] commit_committer_check: Users can only push commits to this repository that were committed with one of their own verified emails.
         :param pulumi.Input[str] commit_message_negative_regex: No commit message is allowed to match this regex, for example `ssh\\:\\/\\/`.
         :param pulumi.Input[str] commit_message_regex: All commit messages must match this regex, e.g. `Fixed \\d+\\..*`.
         :param pulumi.Input[bool] deny_delete_tag: Deny deleting a tag.
-        :param pulumi.Input[str] file_name_regex: All commited filenames must not match this regex, e.g. `(jar|exe)$`.
+        :param pulumi.Input[str] file_name_regex: All committed filenames must not match this regex, e.g. `(jar|exe)$`.
         :param pulumi.Input[int] max_file_size: Maximum file size (MB).
         :param pulumi.Input[bool] member_check: Restrict commits by author (email) to existing GitLab users.
         :param pulumi.Input[bool] prevent_secrets: GitLab will reject any files that are likely to contain secrets.
         :param pulumi.Input[bool] reject_unsigned_commits: Reject commit when it’s not signed through GPG.
         """
         if author_email_regex is not None:
             pulumi.set(__self__, "author_email_regex", author_email_regex)
@@ -823,15 +842,15 @@
     def deny_delete_tag(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "deny_delete_tag", value)
 
     @property
     @pulumi.getter(name="fileNameRegex")
     def file_name_regex(self) -> Optional[pulumi.Input[str]]:
         """
-        All commited filenames must not match this regex, e.g. `(jar|exe)$`.
+        All committed filenames must not match this regex, e.g. `(jar|exe)$`.
         """
         return pulumi.get(self, "file_name_regex")
 
     @file_name_regex.setter
     def file_name_regex(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "file_name_regex", value)
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/application_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                  asset_proxy_enabled: Optional[pulumi.Input[bool]] = None,
                  asset_proxy_secret_key: Optional[pulumi.Input[str]] = None,
                  asset_proxy_url: Optional[pulumi.Input[str]] = None,
                  authorized_keys_enabled: Optional[pulumi.Input[bool]] = None,
                  auto_devops_domain: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  automatic_purchased_storage_allocation: Optional[pulumi.Input[bool]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
                  check_namespace_plan: Optional[pulumi.Input[bool]] = None,
                  commit_email_hostname: Optional[pulumi.Input[str]] = None,
                  container_expiration_policies_enable_historic_entries: Optional[pulumi.Input[bool]] = None,
                  container_registry_cleanup_tags_service_max_list_size: Optional[pulumi.Input[int]] = None,
                  container_registry_delete_tags_service_timeout: Optional[pulumi.Input[int]] = None,
                  container_registry_expiration_policies_caching: Optional[pulumi.Input[bool]] = None,
                  container_registry_expiration_policies_worker_capacity: Optional[pulumi.Input[int]] = None,
@@ -111,14 +112,15 @@
                  git_two_factor_session_expiry: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_default: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_fast: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_medium: Optional[pulumi.Input[int]] = None,
                  grafana_enabled: Optional[pulumi.Input[bool]] = None,
                  grafana_url: Optional[pulumi.Input[str]] = None,
                  gravatar_enabled: Optional[pulumi.Input[bool]] = None,
+                 group_owners_can_manage_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  hashed_storage_enabled: Optional[pulumi.Input[bool]] = None,
                  help_page_hide_commercial_content: Optional[pulumi.Input[bool]] = None,
                  help_page_support_url: Optional[pulumi.Input[str]] = None,
                  help_page_text: Optional[pulumi.Input[str]] = None,
                  help_text: Optional[pulumi.Input[str]] = None,
                  hide_third_party_offers: Optional[pulumi.Input[bool]] = None,
                  home_page_url: Optional[pulumi.Input[str]] = None,
@@ -270,50 +272,51 @@
         :param pulumi.Input[bool] asset_proxy_enabled: (If enabled, requires: asset*proxy*url) Enable proxying of assets. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_secret_key: Shared secret with the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_url: URL of the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] authorized_keys_enabled: By default, we write to the authorized_keys file to support Git over SSH without additional configuration. GitLab can be optimized to authenticate SSH keys via the database file. Only disable this if you have configured your OpenSSH server to use the AuthorizedKeysCommand.
         :param pulumi.Input[str] auto_devops_domain: Specify a domain to use by default for every project’s Auto Review Apps and Auto Deploy stages.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for projects by default. It automatically builds, tests, and deploys applications based on a predefined CI/CD configuration.
         :param pulumi.Input[bool] automatic_purchased_storage_allocation: Enabling this permits automatic allocation of purchased storage in a namespace.
+        :param pulumi.Input[bool] can_create_group: Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
         :param pulumi.Input[bool] check_namespace_plan: Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         :param pulumi.Input[str] commit_email_hostname: Custom hostname (for private commit emails).
         :param pulumi.Input[bool] container_expiration_policies_enable_historic_entries: Enable cleanup policies for all projects.
         :param pulumi.Input[int] container_registry_cleanup_tags_service_max_list_size: The maximum number of tags that can be deleted in a single execution of cleanup policies.
         :param pulumi.Input[int] container_registry_delete_tags_service_timeout: The maximum time, in seconds, that the cleanup process can take to delete a batch of tags for cleanup policies.
         :param pulumi.Input[bool] container_registry_expiration_policies_caching: Caching during the execution of cleanup policies.
         :param pulumi.Input[int] container_registry_expiration_policies_worker_capacity: Number of workers for cleanup policies.
         :param pulumi.Input[int] container_registry_token_expire_delay: Container Registry token duration in minutes.
         :param pulumi.Input[bool] deactivate_dormant_users: Enable automatic deactivation of dormant users.
         :param pulumi.Input[str] default_artifacts_expire_in: Set the default expiration time for each job’s artifacts.
         :param pulumi.Input[str] default_branch_name: Instance-level custom initial branch name (introduced in GitLab 13.2).
         :param pulumi.Input[int] default_branch_protection: Determine if developers can push to the default branch. Can take: 0 (not protected, both users with the Developer role or Maintainer role can push new commits and force push), 1 (partially protected, users with the Developer role or Maintainer role can push new commits, but cannot force push) or 2 (fully protected, users with the Developer or Maintainer role cannot push new commits, but users with the Developer or Maintainer role can; no one can force push) as a parameter. Default is 2.
         :param pulumi.Input[str] default_ci_config_path: Default CI/CD configuration file and path for new projects (.gitlab-ci.yml if not set).
-        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter.
         :param pulumi.Input[int] default_project_creation: Default project creation protection. Can take: 0 (No one), 1 (Maintainers) or 2 (Developers + Maintainers).
-        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[int] default_projects_limit: Project limit per user. Default is 100000.
-        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
-        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
-        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
-        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[int] default_projects_limit: Project limit per user.
+        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
+        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         :param pulumi.Input[int] diff_max_files: Maximum files in a diff.
         :param pulumi.Input[int] diff_max_lines: Maximum lines in a diff.
         :param pulumi.Input[int] diff_max_patch_bytes: Maximum diff patch size, in bytes.
         :param pulumi.Input[bool] disable_feed_token: Disable display of RSS/Atom and calendar feed tokens (introduced in GitLab 13.7).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disabled_oauth_sign_in_sources: Disabled OAuth sign-in sources.
         :param pulumi.Input[bool] dns_rebinding_protection_enabled: Enforce DNS rebinding attack protection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Null means there is no restriction.
         :param pulumi.Input[bool] domain_denylist_enabled: (If enabled, requires: domain_denylist) Allows blocking sign-ups from emails from specific domains.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_denylists: Users with email addresses that match these domains cannot sign up. Wildcards allowed. Use separate lines for multiple entries. Ex: domain.com, *.domain.com.
-        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
-        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
-        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
-        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
-        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
+        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
+        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
+        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
+        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         :param pulumi.Input[str] eks_access_key_id: AWS IAM access key ID.
         :param pulumi.Input[str] eks_account_id: Amazon account ID.
         :param pulumi.Input[bool] eks_integration_enabled: Enable integration with Amazon EKS.
         :param pulumi.Input[str] eks_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[bool] elasticsearch_aws: Enable the use of AWS hosted Elasticsearch.
         :param pulumi.Input[str] elasticsearch_aws_access_key: AWS IAM access key.
         :param pulumi.Input[str] elasticsearch_aws_region: The AWS region the Elasticsearch domain is configured.
@@ -342,127 +345,128 @@
         :param pulumi.Input[bool] external_authorization_service_enabled: (If enabled, requires: external*authorization*service*default*label, external*authorization*service*timeout and external*authorization*service*url) Enable using an external authorization service for accessing projects.
         :param pulumi.Input[float] external_authorization_service_timeout: The timeout after which an authorization request is aborted, in seconds. When a request times out, access is denied to the user. (min: 0.001, max: 10, step: 0.001).
         :param pulumi.Input[str] external_authorization_service_url: URL to which authorization requests are directed.
         :param pulumi.Input[int] external_pipeline_validation_service_timeout: How long to wait for a response from the pipeline validation service. Assumes OK if it times out.
         :param pulumi.Input[str] external_pipeline_validation_service_token: Optional. Token to include as the X-Gitlab-Token header in requests to the URL in external*pipeline*validation*service*url.
         :param pulumi.Input[str] external_pipeline_validation_service_url: URL to use for pipeline validation requests.
         :param pulumi.Input[int] file_template_project_id: The ID of a project to load custom file templates from.
-        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         :param pulumi.Input[str] geo_node_allowed_ips: Comma-separated list of IPs and CIDRs of allowed secondary nodes. For example, 1.1.1.1, 2.2.2.0/24.
         :param pulumi.Input[int] geo_status_timeout: The amount of seconds after which a request to get a secondary node status times out.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         :param pulumi.Input[int] git_two_factor_session_expiry: Maximum duration (in minutes) of a session for Git operations when 2FA is enabled.
         :param pulumi.Input[int] gitaly_timeout_default: Default Gitaly timeout, in seconds. This timeout is not enforced for Git fetch/push operations or Sidekiq jobs. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_fast: Gitaly fast operation timeout, in seconds. Some Gitaly operations are expected to be fast. If they exceed this threshold, there may be a problem with a storage shard and ‘failing fast’ can help maintain the stability of the GitLab instance. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_medium: Medium Gitaly timeout, in seconds. This should be a value between the Fast and the Default timeout. Set to 0 to disable timeouts.
         :param pulumi.Input[bool] grafana_enabled: Enable Grafana.
         :param pulumi.Input[str] grafana_url: Grafana URL.
         :param pulumi.Input[bool] gravatar_enabled: Enable Gravatar.
+        :param pulumi.Input[bool] group_owners_can_manage_default_branch_protection: Prevent overrides of default branch protection.
         :param pulumi.Input[bool] hashed_storage_enabled: Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         :param pulumi.Input[bool] help_page_hide_commercial_content: Hide marketing-related entries from help.
         :param pulumi.Input[str] help_page_support_url: Alternate support URL for help page and help dropdown.
         :param pulumi.Input[str] help_page_text: Custom text displayed on the help page.
         :param pulumi.Input[str] help_text: GitLab server administrator information.
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
-        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails. Enabled by default.
-        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
-        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user. Disabled by default.
-        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
+        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
+        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
+        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         :param pulumi.Input[int] local_markdown_version: Increase this value when any cached Markdown should be invalidated.
         :param pulumi.Input[bool] mailgun_events_enabled: Enable Mailgun event receiver.
         :param pulumi.Input[str] mailgun_signing_key: The Mailgun HTTP webhook signing key for receiving events from webhook.
         :param pulumi.Input[bool] maintenance_mode: When instance is in maintenance mode, non-administrative users can sign in with read-only access and make read-only API requests.
         :param pulumi.Input[str] maintenance_mode_message: Message displayed when instance is in maintenance mode.
         :param pulumi.Input[int] max_artifacts_size: Maximum artifacts size in MB.
         :param pulumi.Input[int] max_attachment_size: Limit attachment size in MB.
-        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
-        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
-        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
-        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         :param pulumi.Input[int] max_pages_size: Maximum size of pages repositories in MB.
         :param pulumi.Input[int] max_personal_access_token_lifetime: Maximum allowable lifetime for access tokens in days.
         :param pulumi.Input[int] max_ssh_key_lifetime: Maximum allowable lifetime for SSH keys in days. Introduced in GitLab 14.6.
         :param pulumi.Input[int] metrics_method_call_threshold: A method call is only tracked when it takes longer than the given amount of milliseconds.
         :param pulumi.Input[bool] mirror_available: Allow repository mirroring to configured by project Maintainers. If disabled, only Administrators can configure repository mirroring.
         :param pulumi.Input[int] mirror_capacity_threshold: Minimum capacity to be available before scheduling more mirrors preemptively.
         :param pulumi.Input[int] mirror_max_capacity: Maximum number of mirrors that can be synchronizing at the same time.
         :param pulumi.Input[int] mirror_max_delay: Maximum time (in minutes) between updates that a mirror can have when scheduled to synchronize.
         :param pulumi.Input[bool] npm_package_requests_forwarding: Use npmjs.org as a default remote repository when the package is not found in the GitLab Package Registry for npm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] outbound_local_requests_whitelists: Define a list of trusted domains or IP addresses to which local requests are allowed when local requests for hooks and services are disabled.
         :param pulumi.Input[int] package_registry_cleanup_policies_worker_capacity: Number of workers assigned to the packages cleanup policies.
         :param pulumi.Input[bool] pages_domain_verification_enabled: Require users to prove ownership of custom domains. Domain verification is an essential security measure for public GitLab sites. Users are required to demonstrate they control a domain before it is enabled.
-        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
-        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password. Default is true.
+        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password.
+        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password.
         :param pulumi.Input[bool] password_lowercase_required: Indicates whether passwords require at least one lowercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_number_required: Indicates whether passwords require at least one number. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_symbol_required: Indicates whether passwords require at least one symbol character. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_uppercase_required: Indicates whether passwords require at least one uppercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[str] performance_bar_allowed_group_path: Path of the group that is allowed to toggle the performance bar.
         :param pulumi.Input[str] personal_access_token_prefix: Prefix for all generated personal access tokens.
-        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
-        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit.
+        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration.
         :param pulumi.Input[str] plantuml_url: The PlantUML instance URL for integration.
         :param pulumi.Input[float] polling_interval_multiplier: Interval multiplier used by endpoints that perform polling. Set to 0 to disable polling.
         :param pulumi.Input[bool] project_export_enabled: Enable project export.
         :param pulumi.Input[bool] prometheus_metrics_enabled: Enable Prometheus metrics.
         :param pulumi.Input[bool] protected_ci_variables: CI/CD variables are protected by default.
         :param pulumi.Input[int] push_event_activities_limit: Number of changes (branches or tags) in a single push to determine whether individual push events or bulk push events are created. Bulk push events are created if it surpasses that value.
         :param pulumi.Input[int] push_event_hooks_limit: Number of changes (branches or tags) in a single push to determine whether webhooks and services fire or not. Webhooks and services aren’t submitted if it surpasses that value.
         :param pulumi.Input[bool] pypi_package_requests_forwarding: Use pypi.org as a default remote repository when the package is not found in the GitLab Package Registry for PyPI.
         :param pulumi.Input[str] rate_limiting_response_text: When rate limiting is enabled via the throttle_* settings, send this plain text response when a rate limit is exceeded. ‘Retry later’ is sent if this is blank.
-        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. To disable throttling set to 0.
         :param pulumi.Input[bool] recaptcha_enabled: (If enabled, requires: recaptcha*private*key and recaptcha*site*key) Enable reCAPTCHA.
         :param pulumi.Input[str] recaptcha_private_key: Private key for reCAPTCHA.
         :param pulumi.Input[str] recaptcha_site_key: Site key for reCAPTCHA.
         :param pulumi.Input[int] receive_max_input_size: Maximum push size (MB).
         :param pulumi.Input[bool] repository_checks_enabled: GitLab periodically runs git fsck in all project and wiki repositories to look for silent disk corruption issues.
         :param pulumi.Input[int] repository_size_limit: Size limit per repository (MB).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repository_storages: (GitLab 13.0 and earlier) List of names of enabled storage paths, taken from gitlab.yml. New projects are created in one of these stores, chosen at random.
         :param pulumi.Input[Mapping[str, pulumi.Input[int]]] repository_storages_weighted: (GitLab 13.1 and later) Hash of names of taken from gitlab.yml to weights. New projects are created in one of these stores, chosen by a weighted random selection.
         :param pulumi.Input[bool] require_admin_approval_after_user_signup: When enabled, any user that signs up for an account using the registration form is placed under a Pending approval state and has to be explicitly approved by an administrator.
         :param pulumi.Input[bool] require_two_factor_authentication: (If enabled, requires: two*factor*grace_period) Require all users to set up Two-factor authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
-        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
-        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
-        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
+        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
+        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
+        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         :param pulumi.Input[bool] send_user_confirmation_email: Send confirmation email on sign-up.
         :param pulumi.Input[int] session_expire_delay: Session duration in minutes. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] shared_runners_enabled: (If enabled, requires: shared*runners*text and shared*runners*minutes) Enable shared runners for new projects.
         :param pulumi.Input[int] shared_runners_minutes: Set the maximum number of CI/CD minutes that a group can use on shared runners per month.
         :param pulumi.Input[str] shared_runners_text: Shared runners text.
-        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
-        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
-        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
+        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
+        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits.
         :param pulumi.Input[str] sign_in_text: Text on the login page.
-        :param pulumi.Input[bool] signup_enabled: Enable registration. Default is true.
+        :param pulumi.Input[bool] signup_enabled: Enable registration.
         :param pulumi.Input[bool] slack_app_enabled: (If enabled, requires: slack*app*id, slack*app*secret and slack*app*secret) Enable Slack app.
         :param pulumi.Input[str] slack_app_id: The app ID of the Slack-app.
         :param pulumi.Input[str] slack_app_secret: The app secret of the Slack-app.
         :param pulumi.Input[str] slack_app_signing_secret: The signing secret of the Slack-app.
         :param pulumi.Input[str] slack_app_verification_token: The verification token of the Slack-app.
-        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes.
         :param pulumi.Input[str] snowplow_app_id: The Snowplow site name / application ID. (for example, gitlab)
         :param pulumi.Input[str] snowplow_collector_hostname: The Snowplow collector hostname. (for example, snowplow.trx.gitlab.net)
         :param pulumi.Input[str] snowplow_cookie_domain: The Snowplow cookie domain. (for example, .gitlab.com)
         :param pulumi.Input[bool] snowplow_enabled: Enable snowplow tracking.
-        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
-        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
+        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects.
         :param pulumi.Input[str] sourcegraph_url: The Sourcegraph instance URL for integration.
         :param pulumi.Input[str] spam_check_api_key: API key used by GitLab for accessing the Spam Check service endpoint.
-        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint. Default is false.
+        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint.
         :param pulumi.Input[str] spam_check_endpoint_url: URL of the external Spamcheck service endpoint. Valid URI schemes are grpc or tls. Specifying tls forces communication to be encrypted.
         :param pulumi.Input[bool] suggest_pipeline_enabled: Enable pipeline suggestion banner.
         :param pulumi.Input[int] terminal_max_session_time: Maximum time for web terminal websocket connection (in seconds). Set to 0 for unlimited time.
         :param pulumi.Input[str] terms: (Required by: enforce_terms) Markdown content for the ToS.
         :param pulumi.Input[bool] throttle_authenticated_api_enabled: (If enabled, requires: throttle*authenticated*api*period*in*seconds and throttle*authenticated*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_authenticated_api_period_in_seconds: Rate limit period (in seconds).
         :param pulumi.Input[int] throttle_authenticated_api_requests_per_period: Maximum requests per period per user.
@@ -477,29 +481,29 @@
         :param pulumi.Input[int] throttle_unauthenticated_api_requests_per_period: Max requests per period per IP.
         :param pulumi.Input[bool] throttle_unauthenticated_packages_api_enabled: (If enabled, requires: throttle*unauthenticated*packages*api*period*in*seconds and throttle*unauthenticated*packages*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_period_in_seconds: Rate limit period (in seconds). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_requests_per_period: Maximum requests per period per user. View Package Registry rate limits for more details.
         :param pulumi.Input[bool] throttle_unauthenticated_web_enabled: (If enabled, requires: throttle*unauthenticated*web*period*in*seconds and throttle*unauthenticated*web*requests*per*period) Enable unauthenticated web request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_unauthenticated_web_period_in_seconds: Rate limit period in seconds.
         :param pulumi.Input[int] throttle_unauthenticated_web_requests_per_period: Max requests per period per IP.
-        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours. Default is false.
+        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours.
         :param pulumi.Input[int] two_factor_grace_period: Amount of time (in hours) that users are allowed to skip forced configuration of two-factor authentication.
         :param pulumi.Input[bool] unique_ips_limit_enabled: (If enabled, requires: unique*ips*limit*per*user and unique*ips*limit*time*window) Limit sign in from multiple IPs.
         :param pulumi.Input[int] unique_ips_limit_per_user: Maximum number of IPs per user.
         :param pulumi.Input[int] unique_ips_limit_time_window: How many seconds an IP is counted towards the limit.
         :param pulumi.Input[bool] usage_ping_enabled: Every week GitLab reports license usage back to GitLab, Inc.
         :param pulumi.Input[bool] user_deactivation_emails_enabled: Send an email to users upon account deactivation.
         :param pulumi.Input[bool] user_default_external: Newly registered users are external by default.
         :param pulumi.Input[str] user_default_internal_regex: Specify an email address regex pattern to identify default internal users.
         :param pulumi.Input[bool] user_oauth_applications: Allow users to register any application to use GitLab as an OAuth provider.
         :param pulumi.Input[bool] user_show_add_ssh_key_message: When set to false disable the You won't be able to pull or push project code via SSH warning shown to users with no uploaded SSH key.
         :param pulumi.Input[bool] version_check_enabled: Let GitLab inform you when an update is available.
         :param pulumi.Input[bool] web_ide_clientside_preview_enabled: Live Preview (allow live previews of JavaScript projects in the Web IDE using CodeSandbox Live Preview).
         :param pulumi.Input[str] whats_new_variant: What’s new variant, possible values: all*tiers, current*tier, and disabled.
-        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         if abuse_notification_email is not None:
             pulumi.set(__self__, "abuse_notification_email", abuse_notification_email)
         if admin_mode is not None:
             pulumi.set(__self__, "admin_mode", admin_mode)
         if after_sign_out_path is not None:
             pulumi.set(__self__, "after_sign_out_path", after_sign_out_path)
@@ -529,14 +533,16 @@
             pulumi.set(__self__, "authorized_keys_enabled", authorized_keys_enabled)
         if auto_devops_domain is not None:
             pulumi.set(__self__, "auto_devops_domain", auto_devops_domain)
         if auto_devops_enabled is not None:
             pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
         if automatic_purchased_storage_allocation is not None:
             pulumi.set(__self__, "automatic_purchased_storage_allocation", automatic_purchased_storage_allocation)
+        if can_create_group is not None:
+            pulumi.set(__self__, "can_create_group", can_create_group)
         if check_namespace_plan is not None:
             pulumi.set(__self__, "check_namespace_plan", check_namespace_plan)
         if commit_email_hostname is not None:
             pulumi.set(__self__, "commit_email_hostname", commit_email_hostname)
         if container_expiration_policies_enable_historic_entries is not None:
             pulumi.set(__self__, "container_expiration_policies_enable_historic_entries", container_expiration_policies_enable_historic_entries)
         if container_registry_cleanup_tags_service_max_list_size is not None:
@@ -695,14 +701,16 @@
             pulumi.set(__self__, "gitaly_timeout_medium", gitaly_timeout_medium)
         if grafana_enabled is not None:
             pulumi.set(__self__, "grafana_enabled", grafana_enabled)
         if grafana_url is not None:
             pulumi.set(__self__, "grafana_url", grafana_url)
         if gravatar_enabled is not None:
             pulumi.set(__self__, "gravatar_enabled", gravatar_enabled)
+        if group_owners_can_manage_default_branch_protection is not None:
+            pulumi.set(__self__, "group_owners_can_manage_default_branch_protection", group_owners_can_manage_default_branch_protection)
         if hashed_storage_enabled is not None:
             pulumi.set(__self__, "hashed_storage_enabled", hashed_storage_enabled)
         if help_page_hide_commercial_content is not None:
             pulumi.set(__self__, "help_page_hide_commercial_content", help_page_hide_commercial_content)
         if help_page_support_url is not None:
             pulumi.set(__self__, "help_page_support_url", help_page_support_url)
         if help_page_text is not None:
@@ -1191,14 +1199,26 @@
         return pulumi.get(self, "automatic_purchased_storage_allocation")
 
     @automatic_purchased_storage_allocation.setter
     def automatic_purchased_storage_allocation(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "automatic_purchased_storage_allocation", value)
 
     @property
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
+        """
+        return pulumi.get(self, "can_create_group")
+
+    @can_create_group.setter
+    def can_create_group(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "can_create_group", value)
+
+    @property
     @pulumi.getter(name="checkNamespacePlan")
     def check_namespace_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         """
         return pulumi.get(self, "check_namespace_plan")
 
@@ -1350,15 +1370,15 @@
     def default_ci_config_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_ci_config_path", value)
 
     @property
     @pulumi.getter(name="defaultGroupVisibility")
     def default_group_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new groups receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_group_visibility")
 
     @default_group_visibility.setter
     def default_group_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_group_visibility", value)
 
@@ -1374,87 +1394,87 @@
     def default_project_creation(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_project_creation", value)
 
     @property
     @pulumi.getter(name="defaultProjectVisibility")
     def default_project_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new projects receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_project_visibility")
 
     @default_project_visibility.setter
     def default_project_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_project_visibility", value)
 
     @property
     @pulumi.getter(name="defaultProjectsLimit")
     def default_projects_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Project limit per user. Default is 100000.
+        Project limit per user.
         """
         return pulumi.get(self, "default_projects_limit")
 
     @default_projects_limit.setter
     def default_projects_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_projects_limit", value)
 
     @property
     @pulumi.getter(name="defaultSnippetVisibility")
     def default_snippet_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new snippets receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_snippet_visibility")
 
     @default_snippet_visibility.setter
     def default_snippet_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_snippet_visibility", value)
 
     @property
     @pulumi.getter(name="delayedGroupDeletion")
     def delayed_group_deletion(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
         """
         return pulumi.get(self, "delayed_group_deletion")
 
     @delayed_group_deletion.setter
     def delayed_group_deletion(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delayed_group_deletion", value)
 
     @property
     @pulumi.getter(name="delayedProjectDeletion")
     def delayed_project_deletion(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
         """
         return pulumi.get(self, "delayed_project_deletion")
 
     @delayed_project_deletion.setter
     def delayed_project_deletion(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delayed_project_deletion", value)
 
     @property
     @pulumi.getter(name="deleteInactiveProjects")
     def delete_inactive_projects(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
+        Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
         """
         return pulumi.get(self, "delete_inactive_projects")
 
     @delete_inactive_projects.setter
     def delete_inactive_projects(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delete_inactive_projects", value)
 
     @property
     @pulumi.getter(name="deletionAdjournedPeriod")
     def deletion_adjourned_period(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         """
         return pulumi.get(self, "deletion_adjourned_period")
 
     @deletion_adjourned_period.setter
     def deletion_adjourned_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "deletion_adjourned_period", value)
 
@@ -1530,15 +1550,15 @@
     def dns_rebinding_protection_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dns_rebinding_protection_enabled", value)
 
     @property
     @pulumi.getter(name="domainAllowlists")
     def domain_allowlists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        Force people to use only corporate emails for sign-up. Null means there is no restriction.
         """
         return pulumi.get(self, "domain_allowlists")
 
     @domain_allowlists.setter
     def domain_allowlists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "domain_allowlists", value)
 
@@ -1566,63 +1586,63 @@
     def domain_denylists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "domain_denylists", value)
 
     @property
     @pulumi.getter(name="dsaKeyRestriction")
     def dsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
+        The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
         """
         return pulumi.get(self, "dsa_key_restriction")
 
     @dsa_key_restriction.setter
     def dsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="ecdsaKeyRestriction")
     def ecdsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
         """
         return pulumi.get(self, "ecdsa_key_restriction")
 
     @ecdsa_key_restriction.setter
     def ecdsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ecdsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="ecdsaSkKeyRestriction")
     def ecdsa_sk_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
         """
         return pulumi.get(self, "ecdsa_sk_key_restriction")
 
     @ecdsa_sk_key_restriction.setter
     def ecdsa_sk_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ecdsa_sk_key_restriction", value)
 
     @property
     @pulumi.getter(name="ed25519KeyRestriction")
     def ed25519_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
         """
         return pulumi.get(self, "ed25519_key_restriction")
 
     @ed25519_key_restriction.setter
     def ed25519_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ed25519_key_restriction", value)
 
     @property
     @pulumi.getter(name="ed25519SkKeyRestriction")
     def ed25519_sk_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         """
         return pulumi.get(self, "ed25519_sk_key_restriction")
 
     @ed25519_sk_key_restriction.setter
     def ed25519_sk_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ed25519_sk_key_restriction", value)
 
@@ -2058,15 +2078,15 @@
     def file_template_project_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "file_template_project_id", value)
 
     @property
     @pulumi.getter(name="firstDayOfWeek")
     def first_day_of_week(self) -> Optional[pulumi.Input[int]]:
         """
-        Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         """
         return pulumi.get(self, "first_day_of_week")
 
     @first_day_of_week.setter
     def first_day_of_week(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "first_day_of_week", value)
 
@@ -2094,15 +2114,15 @@
     def geo_status_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "geo_status_timeout", value)
 
     @property
     @pulumi.getter(name="gitRateLimitUsersAllowlists")
     def git_rate_limit_users_allowlists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         """
         return pulumi.get(self, "git_rate_limit_users_allowlists")
 
     @git_rate_limit_users_allowlists.setter
     def git_rate_limit_users_allowlists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "git_rate_limit_users_allowlists", value)
 
@@ -2187,14 +2207,26 @@
         return pulumi.get(self, "gravatar_enabled")
 
     @gravatar_enabled.setter
     def gravatar_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "gravatar_enabled", value)
 
     @property
+    @pulumi.getter(name="groupOwnersCanManageDefaultBranchProtection")
+    def group_owners_can_manage_default_branch_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Prevent overrides of default branch protection.
+        """
+        return pulumi.get(self, "group_owners_can_manage_default_branch_protection")
+
+    @group_owners_can_manage_default_branch_protection.setter
+    def group_owners_can_manage_default_branch_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "group_owners_can_manage_default_branch_protection", value)
+
+    @property
     @pulumi.getter(name="hashedStorageEnabled")
     def hashed_storage_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         """
         return pulumi.get(self, "hashed_storage_enabled")
 
@@ -2346,87 +2378,87 @@
     def import_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "import_sources", value)
 
     @property
     @pulumi.getter(name="inProductMarketingEmailsEnabled")
     def in_product_marketing_emails_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable in-product marketing emails. Enabled by default.
+        Enable in-product marketing emails.
         """
         return pulumi.get(self, "in_product_marketing_emails_enabled")
 
     @in_product_marketing_emails_enabled.setter
     def in_product_marketing_emails_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "in_product_marketing_emails_enabled", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsDeleteAfterMonths")
     def inactive_projects_delete_after_months(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_delete_after_months")
 
     @inactive_projects_delete_after_months.setter
     def inactive_projects_delete_after_months(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_delete_after_months", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsMinSizeMb")
     def inactive_projects_min_size_mb(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_min_size_mb")
 
     @inactive_projects_min_size_mb.setter
     def inactive_projects_min_size_mb(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_min_size_mb", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsSendWarningEmailAfterMonths")
     def inactive_projects_send_warning_email_after_months(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_send_warning_email_after_months")
 
     @inactive_projects_send_warning_email_after_months.setter
     def inactive_projects_send_warning_email_after_months(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_send_warning_email_after_months", value)
 
     @property
     @pulumi.getter(name="invisibleCaptchaEnabled")
     def invisible_captcha_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
+        Enable Invisible CAPTCHA spam detection during sign-up.
         """
         return pulumi.get(self, "invisible_captcha_enabled")
 
     @invisible_captcha_enabled.setter
     def invisible_captcha_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "invisible_captcha_enabled", value)
 
     @property
     @pulumi.getter(name="issuesCreateLimit")
     def issues_create_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of issue creation requests per minute per user. Disabled by default.
+        Max number of issue creation requests per minute per user.
         """
         return pulumi.get(self, "issues_create_limit")
 
     @issues_create_limit.setter
     def issues_create_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "issues_create_limit", value)
 
     @property
     @pulumi.getter(name="keepLatestArtifact")
     def keep_latest_artifact(self) -> Optional[pulumi.Input[bool]]:
         """
-        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         """
         return pulumi.get(self, "keep_latest_artifact")
 
     @keep_latest_artifact.setter
     def keep_latest_artifact(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "keep_latest_artifact", value)
 
@@ -2514,51 +2546,51 @@
     def max_attachment_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_attachment_size", value)
 
     @property
     @pulumi.getter(name="maxExportSize")
     def max_export_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
+        Maximum export size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_export_size")
 
     @max_export_size.setter
     def max_export_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_export_size", value)
 
     @property
     @pulumi.getter(name="maxImportSize")
     def max_import_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
+        Maximum import size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_import_size")
 
     @max_import_size.setter
     def max_import_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_import_size", value)
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloads")
     def max_number_of_repository_downloads(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads")
 
     @max_number_of_repository_downloads.setter
     def max_number_of_repository_downloads(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_number_of_repository_downloads", value)
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloadsWithinTimePeriod")
     def max_number_of_repository_downloads_within_time_period(self) -> Optional[pulumi.Input[int]]:
         """
-        Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads_within_time_period")
 
     @max_number_of_repository_downloads_within_time_period.setter
     def max_number_of_repository_downloads_within_time_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_number_of_repository_downloads_within_time_period", value)
 
@@ -2706,27 +2738,27 @@
     def pages_domain_verification_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pages_domain_verification_enabled", value)
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForGit")
     def password_authentication_enabled_for_git(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
+        Enable authentication for Git over HTTP(S) via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_git")
 
     @password_authentication_enabled_for_git.setter
     def password_authentication_enabled_for_git(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "password_authentication_enabled_for_git", value)
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForWeb")
     def password_authentication_enabled_for_web(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable authentication for the web interface via a GitLab account password. Default is true.
+        Enable authentication for the web interface via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_web")
 
     @password_authentication_enabled_for_web.setter
     def password_authentication_enabled_for_web(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "password_authentication_enabled_for_web", value)
 
@@ -2802,27 +2834,27 @@
     def personal_access_token_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "personal_access_token_prefix", value)
 
     @property
     @pulumi.getter(name="pipelineLimitPerProjectUserSha")
     def pipeline_limit_per_project_user_sha(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
+        Maximum number of pipeline creation requests per minute per user and commit.
         """
         return pulumi.get(self, "pipeline_limit_per_project_user_sha")
 
     @pipeline_limit_per_project_user_sha.setter
     def pipeline_limit_per_project_user_sha(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "pipeline_limit_per_project_user_sha", value)
 
     @property
     @pulumi.getter(name="plantumlEnabled")
     def plantuml_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        (If enabled, requires: plantuml_url) Enable PlantUML integration.
         """
         return pulumi.get(self, "plantuml_enabled")
 
     @plantuml_enabled.setter
     def plantuml_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "plantuml_enabled", value)
 
@@ -2934,15 +2966,15 @@
     def rate_limiting_response_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rate_limiting_response_text", value)
 
     @property
     @pulumi.getter(name="rawBlobRequestLimit")
     def raw_blob_request_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        Max number of requests per minute for each raw path. To disable throttling set to 0.
         """
         return pulumi.get(self, "raw_blob_request_limit")
 
     @raw_blob_request_limit.setter
     def raw_blob_request_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "raw_blob_request_limit", value)
 
@@ -3066,51 +3098,51 @@
     def require_two_factor_authentication(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_two_factor_authentication", value)
 
     @property
     @pulumi.getter(name="restrictedVisibilityLevels")
     def restricted_visibility_levels(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
+        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
         """
         return pulumi.get(self, "restricted_visibility_levels")
 
     @restricted_visibility_levels.setter
     def restricted_visibility_levels(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "restricted_visibility_levels", value)
 
     @property
     @pulumi.getter(name="rsaKeyRestriction")
     def rsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
+        The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
         """
         return pulumi.get(self, "rsa_key_restriction")
 
     @rsa_key_restriction.setter
     def rsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "rsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="searchRateLimit")
     def search_rate_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit")
 
     @search_rate_limit.setter
     def search_rate_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "search_rate_limit", value)
 
     @property
     @pulumi.getter(name="searchRateLimitUnauthenticated")
     def search_rate_limit_unauthenticated(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit_unauthenticated")
 
     @search_rate_limit_unauthenticated.setter
     def search_rate_limit_unauthenticated(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "search_rate_limit_unauthenticated", value)
 
@@ -3174,39 +3206,39 @@
     def shared_runners_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "shared_runners_text", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterCompressionThresholdBytes")
     def sidekiq_job_limiter_compression_threshold_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
+        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
         """
         return pulumi.get(self, "sidekiq_job_limiter_compression_threshold_bytes")
 
     @sidekiq_job_limiter_compression_threshold_bytes.setter
     def sidekiq_job_limiter_compression_threshold_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sidekiq_job_limiter_compression_threshold_bytes", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterLimitBytes")
     def sidekiq_job_limiter_limit_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
+        The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
         """
         return pulumi.get(self, "sidekiq_job_limiter_limit_bytes")
 
     @sidekiq_job_limiter_limit_bytes.setter
     def sidekiq_job_limiter_limit_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sidekiq_job_limiter_limit_bytes", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterMode")
     def sidekiq_job_limiter_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        track or compress. Sets the behavior for Sidekiq job size limits.
         """
         return pulumi.get(self, "sidekiq_job_limiter_mode")
 
     @sidekiq_job_limiter_mode.setter
     def sidekiq_job_limiter_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sidekiq_job_limiter_mode", value)
 
@@ -3222,15 +3254,15 @@
     def sign_in_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sign_in_text", value)
 
     @property
     @pulumi.getter(name="signupEnabled")
     def signup_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable registration. Default is true.
+        Enable registration.
         """
         return pulumi.get(self, "signup_enabled")
 
     @signup_enabled.setter
     def signup_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "signup_enabled", value)
 
@@ -3294,15 +3326,15 @@
     def slack_app_verification_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "slack_app_verification_token", value)
 
     @property
     @pulumi.getter(name="snippetSizeLimit")
     def snippet_size_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        Max snippet content size in bytes.
         """
         return pulumi.get(self, "snippet_size_limit")
 
     @snippet_size_limit.setter
     def snippet_size_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "snippet_size_limit", value)
 
@@ -3354,27 +3386,27 @@
     def snowplow_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "snowplow_enabled", value)
 
     @property
     @pulumi.getter(name="sourcegraphEnabled")
     def sourcegraph_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
+        Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
         """
         return pulumi.get(self, "sourcegraph_enabled")
 
     @sourcegraph_enabled.setter
     def sourcegraph_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sourcegraph_enabled", value)
 
     @property
     @pulumi.getter(name="sourcegraphPublicOnly")
     def sourcegraph_public_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        Blocks Sourcegraph from being loaded on private and internal projects.
         """
         return pulumi.get(self, "sourcegraph_public_only")
 
     @sourcegraph_public_only.setter
     def sourcegraph_public_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sourcegraph_public_only", value)
 
@@ -3402,15 +3434,15 @@
     def spam_check_api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "spam_check_api_key", value)
 
     @property
     @pulumi.getter(name="spamCheckEndpointEnabled")
     def spam_check_endpoint_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enables spam checking using external Spam Check API endpoint. Default is false.
+        Enables spam checking using external Spam Check API endpoint.
         """
         return pulumi.get(self, "spam_check_endpoint_enabled")
 
     @spam_check_endpoint_enabled.setter
     def spam_check_endpoint_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "spam_check_endpoint_enabled", value)
 
@@ -3678,15 +3710,15 @@
     def throttle_unauthenticated_web_requests_per_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "throttle_unauthenticated_web_requests_per_period", value)
 
     @property
     @pulumi.getter(name="timeTrackingLimitToHours")
     def time_tracking_limit_to_hours(self) -> Optional[pulumi.Input[bool]]:
         """
-        Limit display of time tracking units to hours. Default is false.
+        Limit display of time tracking units to hours.
         """
         return pulumi.get(self, "time_tracking_limit_to_hours")
 
     @time_tracking_limit_to_hours.setter
     def time_tracking_limit_to_hours(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "time_tracking_limit_to_hours", value)
 
@@ -3846,15 +3878,15 @@
     def whats_new_variant(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "whats_new_variant", value)
 
     @property
     @pulumi.getter(name="wikiPageMaxContentBytes")
     def wiki_page_max_content_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         return pulumi.get(self, "wiki_page_max_content_bytes")
 
     @wiki_page_max_content_bytes.setter
     def wiki_page_max_content_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "wiki_page_max_content_bytes", value)
 
@@ -3876,14 +3908,15 @@
                  asset_proxy_enabled: Optional[pulumi.Input[bool]] = None,
                  asset_proxy_secret_key: Optional[pulumi.Input[str]] = None,
                  asset_proxy_url: Optional[pulumi.Input[str]] = None,
                  authorized_keys_enabled: Optional[pulumi.Input[bool]] = None,
                  auto_devops_domain: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  automatic_purchased_storage_allocation: Optional[pulumi.Input[bool]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
                  check_namespace_plan: Optional[pulumi.Input[bool]] = None,
                  commit_email_hostname: Optional[pulumi.Input[str]] = None,
                  container_expiration_policies_enable_historic_entries: Optional[pulumi.Input[bool]] = None,
                  container_registry_cleanup_tags_service_max_list_size: Optional[pulumi.Input[int]] = None,
                  container_registry_delete_tags_service_timeout: Optional[pulumi.Input[int]] = None,
                  container_registry_expiration_policies_caching: Optional[pulumi.Input[bool]] = None,
                  container_registry_expiration_policies_worker_capacity: Optional[pulumi.Input[int]] = None,
@@ -3959,14 +3992,15 @@
                  git_two_factor_session_expiry: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_default: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_fast: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_medium: Optional[pulumi.Input[int]] = None,
                  grafana_enabled: Optional[pulumi.Input[bool]] = None,
                  grafana_url: Optional[pulumi.Input[str]] = None,
                  gravatar_enabled: Optional[pulumi.Input[bool]] = None,
+                 group_owners_can_manage_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  hashed_storage_enabled: Optional[pulumi.Input[bool]] = None,
                  help_page_hide_commercial_content: Optional[pulumi.Input[bool]] = None,
                  help_page_support_url: Optional[pulumi.Input[str]] = None,
                  help_page_text: Optional[pulumi.Input[str]] = None,
                  help_text: Optional[pulumi.Input[str]] = None,
                  hide_third_party_offers: Optional[pulumi.Input[bool]] = None,
                  home_page_url: Optional[pulumi.Input[str]] = None,
@@ -4118,50 +4152,51 @@
         :param pulumi.Input[bool] asset_proxy_enabled: (If enabled, requires: asset*proxy*url) Enable proxying of assets. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_secret_key: Shared secret with the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_url: URL of the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] authorized_keys_enabled: By default, we write to the authorized_keys file to support Git over SSH without additional configuration. GitLab can be optimized to authenticate SSH keys via the database file. Only disable this if you have configured your OpenSSH server to use the AuthorizedKeysCommand.
         :param pulumi.Input[str] auto_devops_domain: Specify a domain to use by default for every project’s Auto Review Apps and Auto Deploy stages.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for projects by default. It automatically builds, tests, and deploys applications based on a predefined CI/CD configuration.
         :param pulumi.Input[bool] automatic_purchased_storage_allocation: Enabling this permits automatic allocation of purchased storage in a namespace.
+        :param pulumi.Input[bool] can_create_group: Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
         :param pulumi.Input[bool] check_namespace_plan: Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         :param pulumi.Input[str] commit_email_hostname: Custom hostname (for private commit emails).
         :param pulumi.Input[bool] container_expiration_policies_enable_historic_entries: Enable cleanup policies for all projects.
         :param pulumi.Input[int] container_registry_cleanup_tags_service_max_list_size: The maximum number of tags that can be deleted in a single execution of cleanup policies.
         :param pulumi.Input[int] container_registry_delete_tags_service_timeout: The maximum time, in seconds, that the cleanup process can take to delete a batch of tags for cleanup policies.
         :param pulumi.Input[bool] container_registry_expiration_policies_caching: Caching during the execution of cleanup policies.
         :param pulumi.Input[int] container_registry_expiration_policies_worker_capacity: Number of workers for cleanup policies.
         :param pulumi.Input[int] container_registry_token_expire_delay: Container Registry token duration in minutes.
         :param pulumi.Input[bool] deactivate_dormant_users: Enable automatic deactivation of dormant users.
         :param pulumi.Input[str] default_artifacts_expire_in: Set the default expiration time for each job’s artifacts.
         :param pulumi.Input[str] default_branch_name: Instance-level custom initial branch name (introduced in GitLab 13.2).
         :param pulumi.Input[int] default_branch_protection: Determine if developers can push to the default branch. Can take: 0 (not protected, both users with the Developer role or Maintainer role can push new commits and force push), 1 (partially protected, users with the Developer role or Maintainer role can push new commits, but cannot force push) or 2 (fully protected, users with the Developer or Maintainer role cannot push new commits, but users with the Developer or Maintainer role can; no one can force push) as a parameter. Default is 2.
         :param pulumi.Input[str] default_ci_config_path: Default CI/CD configuration file and path for new projects (.gitlab-ci.yml if not set).
-        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter.
         :param pulumi.Input[int] default_project_creation: Default project creation protection. Can take: 0 (No one), 1 (Maintainers) or 2 (Developers + Maintainers).
-        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[int] default_projects_limit: Project limit per user. Default is 100000.
-        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
-        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
-        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
-        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[int] default_projects_limit: Project limit per user.
+        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
+        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         :param pulumi.Input[int] diff_max_files: Maximum files in a diff.
         :param pulumi.Input[int] diff_max_lines: Maximum lines in a diff.
         :param pulumi.Input[int] diff_max_patch_bytes: Maximum diff patch size, in bytes.
         :param pulumi.Input[bool] disable_feed_token: Disable display of RSS/Atom and calendar feed tokens (introduced in GitLab 13.7).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disabled_oauth_sign_in_sources: Disabled OAuth sign-in sources.
         :param pulumi.Input[bool] dns_rebinding_protection_enabled: Enforce DNS rebinding attack protection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Null means there is no restriction.
         :param pulumi.Input[bool] domain_denylist_enabled: (If enabled, requires: domain_denylist) Allows blocking sign-ups from emails from specific domains.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_denylists: Users with email addresses that match these domains cannot sign up. Wildcards allowed. Use separate lines for multiple entries. Ex: domain.com, *.domain.com.
-        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
-        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
-        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
-        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
-        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
+        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
+        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
+        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
+        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         :param pulumi.Input[str] eks_access_key_id: AWS IAM access key ID.
         :param pulumi.Input[str] eks_account_id: Amazon account ID.
         :param pulumi.Input[bool] eks_integration_enabled: Enable integration with Amazon EKS.
         :param pulumi.Input[str] eks_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[bool] elasticsearch_aws: Enable the use of AWS hosted Elasticsearch.
         :param pulumi.Input[str] elasticsearch_aws_access_key: AWS IAM access key.
         :param pulumi.Input[str] elasticsearch_aws_region: The AWS region the Elasticsearch domain is configured.
@@ -4190,127 +4225,128 @@
         :param pulumi.Input[bool] external_authorization_service_enabled: (If enabled, requires: external*authorization*service*default*label, external*authorization*service*timeout and external*authorization*service*url) Enable using an external authorization service for accessing projects.
         :param pulumi.Input[float] external_authorization_service_timeout: The timeout after which an authorization request is aborted, in seconds. When a request times out, access is denied to the user. (min: 0.001, max: 10, step: 0.001).
         :param pulumi.Input[str] external_authorization_service_url: URL to which authorization requests are directed.
         :param pulumi.Input[int] external_pipeline_validation_service_timeout: How long to wait for a response from the pipeline validation service. Assumes OK if it times out.
         :param pulumi.Input[str] external_pipeline_validation_service_token: Optional. Token to include as the X-Gitlab-Token header in requests to the URL in external*pipeline*validation*service*url.
         :param pulumi.Input[str] external_pipeline_validation_service_url: URL to use for pipeline validation requests.
         :param pulumi.Input[int] file_template_project_id: The ID of a project to load custom file templates from.
-        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         :param pulumi.Input[str] geo_node_allowed_ips: Comma-separated list of IPs and CIDRs of allowed secondary nodes. For example, 1.1.1.1, 2.2.2.0/24.
         :param pulumi.Input[int] geo_status_timeout: The amount of seconds after which a request to get a secondary node status times out.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         :param pulumi.Input[int] git_two_factor_session_expiry: Maximum duration (in minutes) of a session for Git operations when 2FA is enabled.
         :param pulumi.Input[int] gitaly_timeout_default: Default Gitaly timeout, in seconds. This timeout is not enforced for Git fetch/push operations or Sidekiq jobs. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_fast: Gitaly fast operation timeout, in seconds. Some Gitaly operations are expected to be fast. If they exceed this threshold, there may be a problem with a storage shard and ‘failing fast’ can help maintain the stability of the GitLab instance. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_medium: Medium Gitaly timeout, in seconds. This should be a value between the Fast and the Default timeout. Set to 0 to disable timeouts.
         :param pulumi.Input[bool] grafana_enabled: Enable Grafana.
         :param pulumi.Input[str] grafana_url: Grafana URL.
         :param pulumi.Input[bool] gravatar_enabled: Enable Gravatar.
+        :param pulumi.Input[bool] group_owners_can_manage_default_branch_protection: Prevent overrides of default branch protection.
         :param pulumi.Input[bool] hashed_storage_enabled: Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         :param pulumi.Input[bool] help_page_hide_commercial_content: Hide marketing-related entries from help.
         :param pulumi.Input[str] help_page_support_url: Alternate support URL for help page and help dropdown.
         :param pulumi.Input[str] help_page_text: Custom text displayed on the help page.
         :param pulumi.Input[str] help_text: GitLab server administrator information.
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
-        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails. Enabled by default.
-        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
-        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user. Disabled by default.
-        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
+        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
+        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
+        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         :param pulumi.Input[int] local_markdown_version: Increase this value when any cached Markdown should be invalidated.
         :param pulumi.Input[bool] mailgun_events_enabled: Enable Mailgun event receiver.
         :param pulumi.Input[str] mailgun_signing_key: The Mailgun HTTP webhook signing key for receiving events from webhook.
         :param pulumi.Input[bool] maintenance_mode: When instance is in maintenance mode, non-administrative users can sign in with read-only access and make read-only API requests.
         :param pulumi.Input[str] maintenance_mode_message: Message displayed when instance is in maintenance mode.
         :param pulumi.Input[int] max_artifacts_size: Maximum artifacts size in MB.
         :param pulumi.Input[int] max_attachment_size: Limit attachment size in MB.
-        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
-        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
-        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
-        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         :param pulumi.Input[int] max_pages_size: Maximum size of pages repositories in MB.
         :param pulumi.Input[int] max_personal_access_token_lifetime: Maximum allowable lifetime for access tokens in days.
         :param pulumi.Input[int] max_ssh_key_lifetime: Maximum allowable lifetime for SSH keys in days. Introduced in GitLab 14.6.
         :param pulumi.Input[int] metrics_method_call_threshold: A method call is only tracked when it takes longer than the given amount of milliseconds.
         :param pulumi.Input[bool] mirror_available: Allow repository mirroring to configured by project Maintainers. If disabled, only Administrators can configure repository mirroring.
         :param pulumi.Input[int] mirror_capacity_threshold: Minimum capacity to be available before scheduling more mirrors preemptively.
         :param pulumi.Input[int] mirror_max_capacity: Maximum number of mirrors that can be synchronizing at the same time.
         :param pulumi.Input[int] mirror_max_delay: Maximum time (in minutes) between updates that a mirror can have when scheduled to synchronize.
         :param pulumi.Input[bool] npm_package_requests_forwarding: Use npmjs.org as a default remote repository when the package is not found in the GitLab Package Registry for npm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] outbound_local_requests_whitelists: Define a list of trusted domains or IP addresses to which local requests are allowed when local requests for hooks and services are disabled.
         :param pulumi.Input[int] package_registry_cleanup_policies_worker_capacity: Number of workers assigned to the packages cleanup policies.
         :param pulumi.Input[bool] pages_domain_verification_enabled: Require users to prove ownership of custom domains. Domain verification is an essential security measure for public GitLab sites. Users are required to demonstrate they control a domain before it is enabled.
-        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
-        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password. Default is true.
+        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password.
+        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password.
         :param pulumi.Input[bool] password_lowercase_required: Indicates whether passwords require at least one lowercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_number_required: Indicates whether passwords require at least one number. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_symbol_required: Indicates whether passwords require at least one symbol character. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_uppercase_required: Indicates whether passwords require at least one uppercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[str] performance_bar_allowed_group_path: Path of the group that is allowed to toggle the performance bar.
         :param pulumi.Input[str] personal_access_token_prefix: Prefix for all generated personal access tokens.
-        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
-        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit.
+        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration.
         :param pulumi.Input[str] plantuml_url: The PlantUML instance URL for integration.
         :param pulumi.Input[float] polling_interval_multiplier: Interval multiplier used by endpoints that perform polling. Set to 0 to disable polling.
         :param pulumi.Input[bool] project_export_enabled: Enable project export.
         :param pulumi.Input[bool] prometheus_metrics_enabled: Enable Prometheus metrics.
         :param pulumi.Input[bool] protected_ci_variables: CI/CD variables are protected by default.
         :param pulumi.Input[int] push_event_activities_limit: Number of changes (branches or tags) in a single push to determine whether individual push events or bulk push events are created. Bulk push events are created if it surpasses that value.
         :param pulumi.Input[int] push_event_hooks_limit: Number of changes (branches or tags) in a single push to determine whether webhooks and services fire or not. Webhooks and services aren’t submitted if it surpasses that value.
         :param pulumi.Input[bool] pypi_package_requests_forwarding: Use pypi.org as a default remote repository when the package is not found in the GitLab Package Registry for PyPI.
         :param pulumi.Input[str] rate_limiting_response_text: When rate limiting is enabled via the throttle_* settings, send this plain text response when a rate limit is exceeded. ‘Retry later’ is sent if this is blank.
-        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. To disable throttling set to 0.
         :param pulumi.Input[bool] recaptcha_enabled: (If enabled, requires: recaptcha*private*key and recaptcha*site*key) Enable reCAPTCHA.
         :param pulumi.Input[str] recaptcha_private_key: Private key for reCAPTCHA.
         :param pulumi.Input[str] recaptcha_site_key: Site key for reCAPTCHA.
         :param pulumi.Input[int] receive_max_input_size: Maximum push size (MB).
         :param pulumi.Input[bool] repository_checks_enabled: GitLab periodically runs git fsck in all project and wiki repositories to look for silent disk corruption issues.
         :param pulumi.Input[int] repository_size_limit: Size limit per repository (MB).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repository_storages: (GitLab 13.0 and earlier) List of names of enabled storage paths, taken from gitlab.yml. New projects are created in one of these stores, chosen at random.
         :param pulumi.Input[Mapping[str, pulumi.Input[int]]] repository_storages_weighted: (GitLab 13.1 and later) Hash of names of taken from gitlab.yml to weights. New projects are created in one of these stores, chosen by a weighted random selection.
         :param pulumi.Input[bool] require_admin_approval_after_user_signup: When enabled, any user that signs up for an account using the registration form is placed under a Pending approval state and has to be explicitly approved by an administrator.
         :param pulumi.Input[bool] require_two_factor_authentication: (If enabled, requires: two*factor*grace_period) Require all users to set up Two-factor authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
-        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
-        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
-        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
+        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
+        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
+        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         :param pulumi.Input[bool] send_user_confirmation_email: Send confirmation email on sign-up.
         :param pulumi.Input[int] session_expire_delay: Session duration in minutes. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] shared_runners_enabled: (If enabled, requires: shared*runners*text and shared*runners*minutes) Enable shared runners for new projects.
         :param pulumi.Input[int] shared_runners_minutes: Set the maximum number of CI/CD minutes that a group can use on shared runners per month.
         :param pulumi.Input[str] shared_runners_text: Shared runners text.
-        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
-        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
-        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
+        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
+        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits.
         :param pulumi.Input[str] sign_in_text: Text on the login page.
-        :param pulumi.Input[bool] signup_enabled: Enable registration. Default is true.
+        :param pulumi.Input[bool] signup_enabled: Enable registration.
         :param pulumi.Input[bool] slack_app_enabled: (If enabled, requires: slack*app*id, slack*app*secret and slack*app*secret) Enable Slack app.
         :param pulumi.Input[str] slack_app_id: The app ID of the Slack-app.
         :param pulumi.Input[str] slack_app_secret: The app secret of the Slack-app.
         :param pulumi.Input[str] slack_app_signing_secret: The signing secret of the Slack-app.
         :param pulumi.Input[str] slack_app_verification_token: The verification token of the Slack-app.
-        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes.
         :param pulumi.Input[str] snowplow_app_id: The Snowplow site name / application ID. (for example, gitlab)
         :param pulumi.Input[str] snowplow_collector_hostname: The Snowplow collector hostname. (for example, snowplow.trx.gitlab.net)
         :param pulumi.Input[str] snowplow_cookie_domain: The Snowplow cookie domain. (for example, .gitlab.com)
         :param pulumi.Input[bool] snowplow_enabled: Enable snowplow tracking.
-        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
-        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
+        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects.
         :param pulumi.Input[str] sourcegraph_url: The Sourcegraph instance URL for integration.
         :param pulumi.Input[str] spam_check_api_key: API key used by GitLab for accessing the Spam Check service endpoint.
-        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint. Default is false.
+        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint.
         :param pulumi.Input[str] spam_check_endpoint_url: URL of the external Spamcheck service endpoint. Valid URI schemes are grpc or tls. Specifying tls forces communication to be encrypted.
         :param pulumi.Input[bool] suggest_pipeline_enabled: Enable pipeline suggestion banner.
         :param pulumi.Input[int] terminal_max_session_time: Maximum time for web terminal websocket connection (in seconds). Set to 0 for unlimited time.
         :param pulumi.Input[str] terms: (Required by: enforce_terms) Markdown content for the ToS.
         :param pulumi.Input[bool] throttle_authenticated_api_enabled: (If enabled, requires: throttle*authenticated*api*period*in*seconds and throttle*authenticated*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_authenticated_api_period_in_seconds: Rate limit period (in seconds).
         :param pulumi.Input[int] throttle_authenticated_api_requests_per_period: Maximum requests per period per user.
@@ -4325,29 +4361,29 @@
         :param pulumi.Input[int] throttle_unauthenticated_api_requests_per_period: Max requests per period per IP.
         :param pulumi.Input[bool] throttle_unauthenticated_packages_api_enabled: (If enabled, requires: throttle*unauthenticated*packages*api*period*in*seconds and throttle*unauthenticated*packages*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_period_in_seconds: Rate limit period (in seconds). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_requests_per_period: Maximum requests per period per user. View Package Registry rate limits for more details.
         :param pulumi.Input[bool] throttle_unauthenticated_web_enabled: (If enabled, requires: throttle*unauthenticated*web*period*in*seconds and throttle*unauthenticated*web*requests*per*period) Enable unauthenticated web request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_unauthenticated_web_period_in_seconds: Rate limit period in seconds.
         :param pulumi.Input[int] throttle_unauthenticated_web_requests_per_period: Max requests per period per IP.
-        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours. Default is false.
+        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours.
         :param pulumi.Input[int] two_factor_grace_period: Amount of time (in hours) that users are allowed to skip forced configuration of two-factor authentication.
         :param pulumi.Input[bool] unique_ips_limit_enabled: (If enabled, requires: unique*ips*limit*per*user and unique*ips*limit*time*window) Limit sign in from multiple IPs.
         :param pulumi.Input[int] unique_ips_limit_per_user: Maximum number of IPs per user.
         :param pulumi.Input[int] unique_ips_limit_time_window: How many seconds an IP is counted towards the limit.
         :param pulumi.Input[bool] usage_ping_enabled: Every week GitLab reports license usage back to GitLab, Inc.
         :param pulumi.Input[bool] user_deactivation_emails_enabled: Send an email to users upon account deactivation.
         :param pulumi.Input[bool] user_default_external: Newly registered users are external by default.
         :param pulumi.Input[str] user_default_internal_regex: Specify an email address regex pattern to identify default internal users.
         :param pulumi.Input[bool] user_oauth_applications: Allow users to register any application to use GitLab as an OAuth provider.
         :param pulumi.Input[bool] user_show_add_ssh_key_message: When set to false disable the You won't be able to pull or push project code via SSH warning shown to users with no uploaded SSH key.
         :param pulumi.Input[bool] version_check_enabled: Let GitLab inform you when an update is available.
         :param pulumi.Input[bool] web_ide_clientside_preview_enabled: Live Preview (allow live previews of JavaScript projects in the Web IDE using CodeSandbox Live Preview).
         :param pulumi.Input[str] whats_new_variant: What’s new variant, possible values: all*tiers, current*tier, and disabled.
-        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         if abuse_notification_email is not None:
             pulumi.set(__self__, "abuse_notification_email", abuse_notification_email)
         if admin_mode is not None:
             pulumi.set(__self__, "admin_mode", admin_mode)
         if after_sign_out_path is not None:
             pulumi.set(__self__, "after_sign_out_path", after_sign_out_path)
@@ -4377,14 +4413,16 @@
             pulumi.set(__self__, "authorized_keys_enabled", authorized_keys_enabled)
         if auto_devops_domain is not None:
             pulumi.set(__self__, "auto_devops_domain", auto_devops_domain)
         if auto_devops_enabled is not None:
             pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
         if automatic_purchased_storage_allocation is not None:
             pulumi.set(__self__, "automatic_purchased_storage_allocation", automatic_purchased_storage_allocation)
+        if can_create_group is not None:
+            pulumi.set(__self__, "can_create_group", can_create_group)
         if check_namespace_plan is not None:
             pulumi.set(__self__, "check_namespace_plan", check_namespace_plan)
         if commit_email_hostname is not None:
             pulumi.set(__self__, "commit_email_hostname", commit_email_hostname)
         if container_expiration_policies_enable_historic_entries is not None:
             pulumi.set(__self__, "container_expiration_policies_enable_historic_entries", container_expiration_policies_enable_historic_entries)
         if container_registry_cleanup_tags_service_max_list_size is not None:
@@ -4543,14 +4581,16 @@
             pulumi.set(__self__, "gitaly_timeout_medium", gitaly_timeout_medium)
         if grafana_enabled is not None:
             pulumi.set(__self__, "grafana_enabled", grafana_enabled)
         if grafana_url is not None:
             pulumi.set(__self__, "grafana_url", grafana_url)
         if gravatar_enabled is not None:
             pulumi.set(__self__, "gravatar_enabled", gravatar_enabled)
+        if group_owners_can_manage_default_branch_protection is not None:
+            pulumi.set(__self__, "group_owners_can_manage_default_branch_protection", group_owners_can_manage_default_branch_protection)
         if hashed_storage_enabled is not None:
             pulumi.set(__self__, "hashed_storage_enabled", hashed_storage_enabled)
         if help_page_hide_commercial_content is not None:
             pulumi.set(__self__, "help_page_hide_commercial_content", help_page_hide_commercial_content)
         if help_page_support_url is not None:
             pulumi.set(__self__, "help_page_support_url", help_page_support_url)
         if help_page_text is not None:
@@ -5039,14 +5079,26 @@
         return pulumi.get(self, "automatic_purchased_storage_allocation")
 
     @automatic_purchased_storage_allocation.setter
     def automatic_purchased_storage_allocation(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "automatic_purchased_storage_allocation", value)
 
     @property
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
+        """
+        return pulumi.get(self, "can_create_group")
+
+    @can_create_group.setter
+    def can_create_group(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "can_create_group", value)
+
+    @property
     @pulumi.getter(name="checkNamespacePlan")
     def check_namespace_plan(self) -> Optional[pulumi.Input[bool]]:
         """
         Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         """
         return pulumi.get(self, "check_namespace_plan")
 
@@ -5198,15 +5250,15 @@
     def default_ci_config_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_ci_config_path", value)
 
     @property
     @pulumi.getter(name="defaultGroupVisibility")
     def default_group_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new groups receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_group_visibility")
 
     @default_group_visibility.setter
     def default_group_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_group_visibility", value)
 
@@ -5222,87 +5274,87 @@
     def default_project_creation(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_project_creation", value)
 
     @property
     @pulumi.getter(name="defaultProjectVisibility")
     def default_project_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new projects receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_project_visibility")
 
     @default_project_visibility.setter
     def default_project_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_project_visibility", value)
 
     @property
     @pulumi.getter(name="defaultProjectsLimit")
     def default_projects_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Project limit per user. Default is 100000.
+        Project limit per user.
         """
         return pulumi.get(self, "default_projects_limit")
 
     @default_projects_limit.setter
     def default_projects_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_projects_limit", value)
 
     @property
     @pulumi.getter(name="defaultSnippetVisibility")
     def default_snippet_visibility(self) -> Optional[pulumi.Input[str]]:
         """
-        What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new snippets receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_snippet_visibility")
 
     @default_snippet_visibility.setter
     def default_snippet_visibility(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_snippet_visibility", value)
 
     @property
     @pulumi.getter(name="delayedGroupDeletion")
     def delayed_group_deletion(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
         """
         return pulumi.get(self, "delayed_group_deletion")
 
     @delayed_group_deletion.setter
     def delayed_group_deletion(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delayed_group_deletion", value)
 
     @property
     @pulumi.getter(name="delayedProjectDeletion")
     def delayed_project_deletion(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
         """
         return pulumi.get(self, "delayed_project_deletion")
 
     @delayed_project_deletion.setter
     def delayed_project_deletion(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delayed_project_deletion", value)
 
     @property
     @pulumi.getter(name="deleteInactiveProjects")
     def delete_inactive_projects(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
+        Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
         """
         return pulumi.get(self, "delete_inactive_projects")
 
     @delete_inactive_projects.setter
     def delete_inactive_projects(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delete_inactive_projects", value)
 
     @property
     @pulumi.getter(name="deletionAdjournedPeriod")
     def deletion_adjourned_period(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         """
         return pulumi.get(self, "deletion_adjourned_period")
 
     @deletion_adjourned_period.setter
     def deletion_adjourned_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "deletion_adjourned_period", value)
 
@@ -5378,15 +5430,15 @@
     def dns_rebinding_protection_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "dns_rebinding_protection_enabled", value)
 
     @property
     @pulumi.getter(name="domainAllowlists")
     def domain_allowlists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        Force people to use only corporate emails for sign-up. Null means there is no restriction.
         """
         return pulumi.get(self, "domain_allowlists")
 
     @domain_allowlists.setter
     def domain_allowlists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "domain_allowlists", value)
 
@@ -5414,63 +5466,63 @@
     def domain_denylists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "domain_denylists", value)
 
     @property
     @pulumi.getter(name="dsaKeyRestriction")
     def dsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
+        The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
         """
         return pulumi.get(self, "dsa_key_restriction")
 
     @dsa_key_restriction.setter
     def dsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "dsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="ecdsaKeyRestriction")
     def ecdsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
         """
         return pulumi.get(self, "ecdsa_key_restriction")
 
     @ecdsa_key_restriction.setter
     def ecdsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ecdsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="ecdsaSkKeyRestriction")
     def ecdsa_sk_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
         """
         return pulumi.get(self, "ecdsa_sk_key_restriction")
 
     @ecdsa_sk_key_restriction.setter
     def ecdsa_sk_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ecdsa_sk_key_restriction", value)
 
     @property
     @pulumi.getter(name="ed25519KeyRestriction")
     def ed25519_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
         """
         return pulumi.get(self, "ed25519_key_restriction")
 
     @ed25519_key_restriction.setter
     def ed25519_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ed25519_key_restriction", value)
 
     @property
     @pulumi.getter(name="ed25519SkKeyRestriction")
     def ed25519_sk_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         """
         return pulumi.get(self, "ed25519_sk_key_restriction")
 
     @ed25519_sk_key_restriction.setter
     def ed25519_sk_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "ed25519_sk_key_restriction", value)
 
@@ -5906,15 +5958,15 @@
     def file_template_project_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "file_template_project_id", value)
 
     @property
     @pulumi.getter(name="firstDayOfWeek")
     def first_day_of_week(self) -> Optional[pulumi.Input[int]]:
         """
-        Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         """
         return pulumi.get(self, "first_day_of_week")
 
     @first_day_of_week.setter
     def first_day_of_week(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "first_day_of_week", value)
 
@@ -5942,15 +5994,15 @@
     def geo_status_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "geo_status_timeout", value)
 
     @property
     @pulumi.getter(name="gitRateLimitUsersAllowlists")
     def git_rate_limit_users_allowlists(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         """
         return pulumi.get(self, "git_rate_limit_users_allowlists")
 
     @git_rate_limit_users_allowlists.setter
     def git_rate_limit_users_allowlists(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "git_rate_limit_users_allowlists", value)
 
@@ -6035,14 +6087,26 @@
         return pulumi.get(self, "gravatar_enabled")
 
     @gravatar_enabled.setter
     def gravatar_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "gravatar_enabled", value)
 
     @property
+    @pulumi.getter(name="groupOwnersCanManageDefaultBranchProtection")
+    def group_owners_can_manage_default_branch_protection(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Prevent overrides of default branch protection.
+        """
+        return pulumi.get(self, "group_owners_can_manage_default_branch_protection")
+
+    @group_owners_can_manage_default_branch_protection.setter
+    def group_owners_can_manage_default_branch_protection(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "group_owners_can_manage_default_branch_protection", value)
+
+    @property
     @pulumi.getter(name="hashedStorageEnabled")
     def hashed_storage_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         """
         return pulumi.get(self, "hashed_storage_enabled")
 
@@ -6194,87 +6258,87 @@
     def import_sources(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "import_sources", value)
 
     @property
     @pulumi.getter(name="inProductMarketingEmailsEnabled")
     def in_product_marketing_emails_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable in-product marketing emails. Enabled by default.
+        Enable in-product marketing emails.
         """
         return pulumi.get(self, "in_product_marketing_emails_enabled")
 
     @in_product_marketing_emails_enabled.setter
     def in_product_marketing_emails_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "in_product_marketing_emails_enabled", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsDeleteAfterMonths")
     def inactive_projects_delete_after_months(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_delete_after_months")
 
     @inactive_projects_delete_after_months.setter
     def inactive_projects_delete_after_months(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_delete_after_months", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsMinSizeMb")
     def inactive_projects_min_size_mb(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_min_size_mb")
 
     @inactive_projects_min_size_mb.setter
     def inactive_projects_min_size_mb(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_min_size_mb", value)
 
     @property
     @pulumi.getter(name="inactiveProjectsSendWarningEmailAfterMonths")
     def inactive_projects_send_warning_email_after_months(self) -> Optional[pulumi.Input[int]]:
         """
-        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_send_warning_email_after_months")
 
     @inactive_projects_send_warning_email_after_months.setter
     def inactive_projects_send_warning_email_after_months(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "inactive_projects_send_warning_email_after_months", value)
 
     @property
     @pulumi.getter(name="invisibleCaptchaEnabled")
     def invisible_captcha_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
+        Enable Invisible CAPTCHA spam detection during sign-up.
         """
         return pulumi.get(self, "invisible_captcha_enabled")
 
     @invisible_captcha_enabled.setter
     def invisible_captcha_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "invisible_captcha_enabled", value)
 
     @property
     @pulumi.getter(name="issuesCreateLimit")
     def issues_create_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of issue creation requests per minute per user. Disabled by default.
+        Max number of issue creation requests per minute per user.
         """
         return pulumi.get(self, "issues_create_limit")
 
     @issues_create_limit.setter
     def issues_create_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "issues_create_limit", value)
 
     @property
     @pulumi.getter(name="keepLatestArtifact")
     def keep_latest_artifact(self) -> Optional[pulumi.Input[bool]]:
         """
-        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         """
         return pulumi.get(self, "keep_latest_artifact")
 
     @keep_latest_artifact.setter
     def keep_latest_artifact(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "keep_latest_artifact", value)
 
@@ -6362,51 +6426,51 @@
     def max_attachment_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_attachment_size", value)
 
     @property
     @pulumi.getter(name="maxExportSize")
     def max_export_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
+        Maximum export size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_export_size")
 
     @max_export_size.setter
     def max_export_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_export_size", value)
 
     @property
     @pulumi.getter(name="maxImportSize")
     def max_import_size(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
+        Maximum import size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_import_size")
 
     @max_import_size.setter
     def max_import_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_import_size", value)
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloads")
     def max_number_of_repository_downloads(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads")
 
     @max_number_of_repository_downloads.setter
     def max_number_of_repository_downloads(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_number_of_repository_downloads", value)
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloadsWithinTimePeriod")
     def max_number_of_repository_downloads_within_time_period(self) -> Optional[pulumi.Input[int]]:
         """
-        Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads_within_time_period")
 
     @max_number_of_repository_downloads_within_time_period.setter
     def max_number_of_repository_downloads_within_time_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_number_of_repository_downloads_within_time_period", value)
 
@@ -6554,27 +6618,27 @@
     def pages_domain_verification_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pages_domain_verification_enabled", value)
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForGit")
     def password_authentication_enabled_for_git(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
+        Enable authentication for Git over HTTP(S) via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_git")
 
     @password_authentication_enabled_for_git.setter
     def password_authentication_enabled_for_git(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "password_authentication_enabled_for_git", value)
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForWeb")
     def password_authentication_enabled_for_web(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable authentication for the web interface via a GitLab account password. Default is true.
+        Enable authentication for the web interface via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_web")
 
     @password_authentication_enabled_for_web.setter
     def password_authentication_enabled_for_web(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "password_authentication_enabled_for_web", value)
 
@@ -6650,27 +6714,27 @@
     def personal_access_token_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "personal_access_token_prefix", value)
 
     @property
     @pulumi.getter(name="pipelineLimitPerProjectUserSha")
     def pipeline_limit_per_project_user_sha(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
+        Maximum number of pipeline creation requests per minute per user and commit.
         """
         return pulumi.get(self, "pipeline_limit_per_project_user_sha")
 
     @pipeline_limit_per_project_user_sha.setter
     def pipeline_limit_per_project_user_sha(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "pipeline_limit_per_project_user_sha", value)
 
     @property
     @pulumi.getter(name="plantumlEnabled")
     def plantuml_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        (If enabled, requires: plantuml_url) Enable PlantUML integration.
         """
         return pulumi.get(self, "plantuml_enabled")
 
     @plantuml_enabled.setter
     def plantuml_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "plantuml_enabled", value)
 
@@ -6782,15 +6846,15 @@
     def rate_limiting_response_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "rate_limiting_response_text", value)
 
     @property
     @pulumi.getter(name="rawBlobRequestLimit")
     def raw_blob_request_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        Max number of requests per minute for each raw path. To disable throttling set to 0.
         """
         return pulumi.get(self, "raw_blob_request_limit")
 
     @raw_blob_request_limit.setter
     def raw_blob_request_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "raw_blob_request_limit", value)
 
@@ -6914,51 +6978,51 @@
     def require_two_factor_authentication(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "require_two_factor_authentication", value)
 
     @property
     @pulumi.getter(name="restrictedVisibilityLevels")
     def restricted_visibility_levels(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
+        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
         """
         return pulumi.get(self, "restricted_visibility_levels")
 
     @restricted_visibility_levels.setter
     def restricted_visibility_levels(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "restricted_visibility_levels", value)
 
     @property
     @pulumi.getter(name="rsaKeyRestriction")
     def rsa_key_restriction(self) -> Optional[pulumi.Input[int]]:
         """
-        The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
+        The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
         """
         return pulumi.get(self, "rsa_key_restriction")
 
     @rsa_key_restriction.setter
     def rsa_key_restriction(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "rsa_key_restriction", value)
 
     @property
     @pulumi.getter(name="searchRateLimit")
     def search_rate_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit")
 
     @search_rate_limit.setter
     def search_rate_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "search_rate_limit", value)
 
     @property
     @pulumi.getter(name="searchRateLimitUnauthenticated")
     def search_rate_limit_unauthenticated(self) -> Optional[pulumi.Input[int]]:
         """
-        Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit_unauthenticated")
 
     @search_rate_limit_unauthenticated.setter
     def search_rate_limit_unauthenticated(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "search_rate_limit_unauthenticated", value)
 
@@ -7022,39 +7086,39 @@
     def shared_runners_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "shared_runners_text", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterCompressionThresholdBytes")
     def sidekiq_job_limiter_compression_threshold_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
+        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
         """
         return pulumi.get(self, "sidekiq_job_limiter_compression_threshold_bytes")
 
     @sidekiq_job_limiter_compression_threshold_bytes.setter
     def sidekiq_job_limiter_compression_threshold_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sidekiq_job_limiter_compression_threshold_bytes", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterLimitBytes")
     def sidekiq_job_limiter_limit_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
+        The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
         """
         return pulumi.get(self, "sidekiq_job_limiter_limit_bytes")
 
     @sidekiq_job_limiter_limit_bytes.setter
     def sidekiq_job_limiter_limit_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "sidekiq_job_limiter_limit_bytes", value)
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterMode")
     def sidekiq_job_limiter_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        track or compress. Sets the behavior for Sidekiq job size limits.
         """
         return pulumi.get(self, "sidekiq_job_limiter_mode")
 
     @sidekiq_job_limiter_mode.setter
     def sidekiq_job_limiter_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sidekiq_job_limiter_mode", value)
 
@@ -7070,15 +7134,15 @@
     def sign_in_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sign_in_text", value)
 
     @property
     @pulumi.getter(name="signupEnabled")
     def signup_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable registration. Default is true.
+        Enable registration.
         """
         return pulumi.get(self, "signup_enabled")
 
     @signup_enabled.setter
     def signup_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "signup_enabled", value)
 
@@ -7142,15 +7206,15 @@
     def slack_app_verification_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "slack_app_verification_token", value)
 
     @property
     @pulumi.getter(name="snippetSizeLimit")
     def snippet_size_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        Max snippet content size in bytes.
         """
         return pulumi.get(self, "snippet_size_limit")
 
     @snippet_size_limit.setter
     def snippet_size_limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "snippet_size_limit", value)
 
@@ -7202,27 +7266,27 @@
     def snowplow_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "snowplow_enabled", value)
 
     @property
     @pulumi.getter(name="sourcegraphEnabled")
     def sourcegraph_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
+        Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
         """
         return pulumi.get(self, "sourcegraph_enabled")
 
     @sourcegraph_enabled.setter
     def sourcegraph_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sourcegraph_enabled", value)
 
     @property
     @pulumi.getter(name="sourcegraphPublicOnly")
     def sourcegraph_public_only(self) -> Optional[pulumi.Input[bool]]:
         """
-        Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        Blocks Sourcegraph from being loaded on private and internal projects.
         """
         return pulumi.get(self, "sourcegraph_public_only")
 
     @sourcegraph_public_only.setter
     def sourcegraph_public_only(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "sourcegraph_public_only", value)
 
@@ -7250,15 +7314,15 @@
     def spam_check_api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "spam_check_api_key", value)
 
     @property
     @pulumi.getter(name="spamCheckEndpointEnabled")
     def spam_check_endpoint_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enables spam checking using external Spam Check API endpoint. Default is false.
+        Enables spam checking using external Spam Check API endpoint.
         """
         return pulumi.get(self, "spam_check_endpoint_enabled")
 
     @spam_check_endpoint_enabled.setter
     def spam_check_endpoint_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "spam_check_endpoint_enabled", value)
 
@@ -7526,15 +7590,15 @@
     def throttle_unauthenticated_web_requests_per_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "throttle_unauthenticated_web_requests_per_period", value)
 
     @property
     @pulumi.getter(name="timeTrackingLimitToHours")
     def time_tracking_limit_to_hours(self) -> Optional[pulumi.Input[bool]]:
         """
-        Limit display of time tracking units to hours. Default is false.
+        Limit display of time tracking units to hours.
         """
         return pulumi.get(self, "time_tracking_limit_to_hours")
 
     @time_tracking_limit_to_hours.setter
     def time_tracking_limit_to_hours(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "time_tracking_limit_to_hours", value)
 
@@ -7694,15 +7758,15 @@
     def whats_new_variant(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "whats_new_variant", value)
 
     @property
     @pulumi.getter(name="wikiPageMaxContentBytes")
     def wiki_page_max_content_bytes(self) -> Optional[pulumi.Input[int]]:
         """
-        Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         return pulumi.get(self, "wiki_page_max_content_bytes")
 
     @wiki_page_max_content_bytes.setter
     def wiki_page_max_content_bytes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "wiki_page_max_content_bytes", value)
 
@@ -7726,14 +7790,15 @@
                  asset_proxy_enabled: Optional[pulumi.Input[bool]] = None,
                  asset_proxy_secret_key: Optional[pulumi.Input[str]] = None,
                  asset_proxy_url: Optional[pulumi.Input[str]] = None,
                  authorized_keys_enabled: Optional[pulumi.Input[bool]] = None,
                  auto_devops_domain: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  automatic_purchased_storage_allocation: Optional[pulumi.Input[bool]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
                  check_namespace_plan: Optional[pulumi.Input[bool]] = None,
                  commit_email_hostname: Optional[pulumi.Input[str]] = None,
                  container_expiration_policies_enable_historic_entries: Optional[pulumi.Input[bool]] = None,
                  container_registry_cleanup_tags_service_max_list_size: Optional[pulumi.Input[int]] = None,
                  container_registry_delete_tags_service_timeout: Optional[pulumi.Input[int]] = None,
                  container_registry_expiration_policies_caching: Optional[pulumi.Input[bool]] = None,
                  container_registry_expiration_policies_worker_capacity: Optional[pulumi.Input[int]] = None,
@@ -7809,14 +7874,15 @@
                  git_two_factor_session_expiry: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_default: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_fast: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_medium: Optional[pulumi.Input[int]] = None,
                  grafana_enabled: Optional[pulumi.Input[bool]] = None,
                  grafana_url: Optional[pulumi.Input[str]] = None,
                  gravatar_enabled: Optional[pulumi.Input[bool]] = None,
+                 group_owners_can_manage_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  hashed_storage_enabled: Optional[pulumi.Input[bool]] = None,
                  help_page_hide_commercial_content: Optional[pulumi.Input[bool]] = None,
                  help_page_support_url: Optional[pulumi.Input[str]] = None,
                  help_page_text: Optional[pulumi.Input[str]] = None,
                  help_text: Optional[pulumi.Input[str]] = None,
                  hide_third_party_offers: Optional[pulumi.Input[bool]] = None,
                  home_page_url: Optional[pulumi.Input[str]] = None,
@@ -7982,50 +8048,51 @@
         :param pulumi.Input[bool] asset_proxy_enabled: (If enabled, requires: asset*proxy*url) Enable proxying of assets. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_secret_key: Shared secret with the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_url: URL of the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] authorized_keys_enabled: By default, we write to the authorized_keys file to support Git over SSH without additional configuration. GitLab can be optimized to authenticate SSH keys via the database file. Only disable this if you have configured your OpenSSH server to use the AuthorizedKeysCommand.
         :param pulumi.Input[str] auto_devops_domain: Specify a domain to use by default for every project’s Auto Review Apps and Auto Deploy stages.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for projects by default. It automatically builds, tests, and deploys applications based on a predefined CI/CD configuration.
         :param pulumi.Input[bool] automatic_purchased_storage_allocation: Enabling this permits automatic allocation of purchased storage in a namespace.
+        :param pulumi.Input[bool] can_create_group: Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
         :param pulumi.Input[bool] check_namespace_plan: Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         :param pulumi.Input[str] commit_email_hostname: Custom hostname (for private commit emails).
         :param pulumi.Input[bool] container_expiration_policies_enable_historic_entries: Enable cleanup policies for all projects.
         :param pulumi.Input[int] container_registry_cleanup_tags_service_max_list_size: The maximum number of tags that can be deleted in a single execution of cleanup policies.
         :param pulumi.Input[int] container_registry_delete_tags_service_timeout: The maximum time, in seconds, that the cleanup process can take to delete a batch of tags for cleanup policies.
         :param pulumi.Input[bool] container_registry_expiration_policies_caching: Caching during the execution of cleanup policies.
         :param pulumi.Input[int] container_registry_expiration_policies_worker_capacity: Number of workers for cleanup policies.
         :param pulumi.Input[int] container_registry_token_expire_delay: Container Registry token duration in minutes.
         :param pulumi.Input[bool] deactivate_dormant_users: Enable automatic deactivation of dormant users.
         :param pulumi.Input[str] default_artifacts_expire_in: Set the default expiration time for each job’s artifacts.
         :param pulumi.Input[str] default_branch_name: Instance-level custom initial branch name (introduced in GitLab 13.2).
         :param pulumi.Input[int] default_branch_protection: Determine if developers can push to the default branch. Can take: 0 (not protected, both users with the Developer role or Maintainer role can push new commits and force push), 1 (partially protected, users with the Developer role or Maintainer role can push new commits, but cannot force push) or 2 (fully protected, users with the Developer or Maintainer role cannot push new commits, but users with the Developer or Maintainer role can; no one can force push) as a parameter. Default is 2.
         :param pulumi.Input[str] default_ci_config_path: Default CI/CD configuration file and path for new projects (.gitlab-ci.yml if not set).
-        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter.
         :param pulumi.Input[int] default_project_creation: Default project creation protection. Can take: 0 (No one), 1 (Maintainers) or 2 (Developers + Maintainers).
-        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[int] default_projects_limit: Project limit per user. Default is 100000.
-        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
-        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
-        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
-        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[int] default_projects_limit: Project limit per user.
+        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
+        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         :param pulumi.Input[int] diff_max_files: Maximum files in a diff.
         :param pulumi.Input[int] diff_max_lines: Maximum lines in a diff.
         :param pulumi.Input[int] diff_max_patch_bytes: Maximum diff patch size, in bytes.
         :param pulumi.Input[bool] disable_feed_token: Disable display of RSS/Atom and calendar feed tokens (introduced in GitLab 13.7).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disabled_oauth_sign_in_sources: Disabled OAuth sign-in sources.
         :param pulumi.Input[bool] dns_rebinding_protection_enabled: Enforce DNS rebinding attack protection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Null means there is no restriction.
         :param pulumi.Input[bool] domain_denylist_enabled: (If enabled, requires: domain_denylist) Allows blocking sign-ups from emails from specific domains.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_denylists: Users with email addresses that match these domains cannot sign up. Wildcards allowed. Use separate lines for multiple entries. Ex: domain.com, *.domain.com.
-        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
-        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
-        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
-        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
-        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
+        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
+        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
+        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
+        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         :param pulumi.Input[str] eks_access_key_id: AWS IAM access key ID.
         :param pulumi.Input[str] eks_account_id: Amazon account ID.
         :param pulumi.Input[bool] eks_integration_enabled: Enable integration with Amazon EKS.
         :param pulumi.Input[str] eks_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[bool] elasticsearch_aws: Enable the use of AWS hosted Elasticsearch.
         :param pulumi.Input[str] elasticsearch_aws_access_key: AWS IAM access key.
         :param pulumi.Input[str] elasticsearch_aws_region: The AWS region the Elasticsearch domain is configured.
@@ -8054,127 +8121,128 @@
         :param pulumi.Input[bool] external_authorization_service_enabled: (If enabled, requires: external*authorization*service*default*label, external*authorization*service*timeout and external*authorization*service*url) Enable using an external authorization service for accessing projects.
         :param pulumi.Input[float] external_authorization_service_timeout: The timeout after which an authorization request is aborted, in seconds. When a request times out, access is denied to the user. (min: 0.001, max: 10, step: 0.001).
         :param pulumi.Input[str] external_authorization_service_url: URL to which authorization requests are directed.
         :param pulumi.Input[int] external_pipeline_validation_service_timeout: How long to wait for a response from the pipeline validation service. Assumes OK if it times out.
         :param pulumi.Input[str] external_pipeline_validation_service_token: Optional. Token to include as the X-Gitlab-Token header in requests to the URL in external*pipeline*validation*service*url.
         :param pulumi.Input[str] external_pipeline_validation_service_url: URL to use for pipeline validation requests.
         :param pulumi.Input[int] file_template_project_id: The ID of a project to load custom file templates from.
-        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         :param pulumi.Input[str] geo_node_allowed_ips: Comma-separated list of IPs and CIDRs of allowed secondary nodes. For example, 1.1.1.1, 2.2.2.0/24.
         :param pulumi.Input[int] geo_status_timeout: The amount of seconds after which a request to get a secondary node status times out.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         :param pulumi.Input[int] git_two_factor_session_expiry: Maximum duration (in minutes) of a session for Git operations when 2FA is enabled.
         :param pulumi.Input[int] gitaly_timeout_default: Default Gitaly timeout, in seconds. This timeout is not enforced for Git fetch/push operations or Sidekiq jobs. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_fast: Gitaly fast operation timeout, in seconds. Some Gitaly operations are expected to be fast. If they exceed this threshold, there may be a problem with a storage shard and ‘failing fast’ can help maintain the stability of the GitLab instance. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_medium: Medium Gitaly timeout, in seconds. This should be a value between the Fast and the Default timeout. Set to 0 to disable timeouts.
         :param pulumi.Input[bool] grafana_enabled: Enable Grafana.
         :param pulumi.Input[str] grafana_url: Grafana URL.
         :param pulumi.Input[bool] gravatar_enabled: Enable Gravatar.
+        :param pulumi.Input[bool] group_owners_can_manage_default_branch_protection: Prevent overrides of default branch protection.
         :param pulumi.Input[bool] hashed_storage_enabled: Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         :param pulumi.Input[bool] help_page_hide_commercial_content: Hide marketing-related entries from help.
         :param pulumi.Input[str] help_page_support_url: Alternate support URL for help page and help dropdown.
         :param pulumi.Input[str] help_page_text: Custom text displayed on the help page.
         :param pulumi.Input[str] help_text: GitLab server administrator information.
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
-        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails. Enabled by default.
-        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
-        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user. Disabled by default.
-        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
+        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
+        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
+        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         :param pulumi.Input[int] local_markdown_version: Increase this value when any cached Markdown should be invalidated.
         :param pulumi.Input[bool] mailgun_events_enabled: Enable Mailgun event receiver.
         :param pulumi.Input[str] mailgun_signing_key: The Mailgun HTTP webhook signing key for receiving events from webhook.
         :param pulumi.Input[bool] maintenance_mode: When instance is in maintenance mode, non-administrative users can sign in with read-only access and make read-only API requests.
         :param pulumi.Input[str] maintenance_mode_message: Message displayed when instance is in maintenance mode.
         :param pulumi.Input[int] max_artifacts_size: Maximum artifacts size in MB.
         :param pulumi.Input[int] max_attachment_size: Limit attachment size in MB.
-        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
-        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
-        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
-        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         :param pulumi.Input[int] max_pages_size: Maximum size of pages repositories in MB.
         :param pulumi.Input[int] max_personal_access_token_lifetime: Maximum allowable lifetime for access tokens in days.
         :param pulumi.Input[int] max_ssh_key_lifetime: Maximum allowable lifetime for SSH keys in days. Introduced in GitLab 14.6.
         :param pulumi.Input[int] metrics_method_call_threshold: A method call is only tracked when it takes longer than the given amount of milliseconds.
         :param pulumi.Input[bool] mirror_available: Allow repository mirroring to configured by project Maintainers. If disabled, only Administrators can configure repository mirroring.
         :param pulumi.Input[int] mirror_capacity_threshold: Minimum capacity to be available before scheduling more mirrors preemptively.
         :param pulumi.Input[int] mirror_max_capacity: Maximum number of mirrors that can be synchronizing at the same time.
         :param pulumi.Input[int] mirror_max_delay: Maximum time (in minutes) between updates that a mirror can have when scheduled to synchronize.
         :param pulumi.Input[bool] npm_package_requests_forwarding: Use npmjs.org as a default remote repository when the package is not found in the GitLab Package Registry for npm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] outbound_local_requests_whitelists: Define a list of trusted domains or IP addresses to which local requests are allowed when local requests for hooks and services are disabled.
         :param pulumi.Input[int] package_registry_cleanup_policies_worker_capacity: Number of workers assigned to the packages cleanup policies.
         :param pulumi.Input[bool] pages_domain_verification_enabled: Require users to prove ownership of custom domains. Domain verification is an essential security measure for public GitLab sites. Users are required to demonstrate they control a domain before it is enabled.
-        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
-        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password. Default is true.
+        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password.
+        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password.
         :param pulumi.Input[bool] password_lowercase_required: Indicates whether passwords require at least one lowercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_number_required: Indicates whether passwords require at least one number. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_symbol_required: Indicates whether passwords require at least one symbol character. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_uppercase_required: Indicates whether passwords require at least one uppercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[str] performance_bar_allowed_group_path: Path of the group that is allowed to toggle the performance bar.
         :param pulumi.Input[str] personal_access_token_prefix: Prefix for all generated personal access tokens.
-        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
-        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit.
+        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration.
         :param pulumi.Input[str] plantuml_url: The PlantUML instance URL for integration.
         :param pulumi.Input[float] polling_interval_multiplier: Interval multiplier used by endpoints that perform polling. Set to 0 to disable polling.
         :param pulumi.Input[bool] project_export_enabled: Enable project export.
         :param pulumi.Input[bool] prometheus_metrics_enabled: Enable Prometheus metrics.
         :param pulumi.Input[bool] protected_ci_variables: CI/CD variables are protected by default.
         :param pulumi.Input[int] push_event_activities_limit: Number of changes (branches or tags) in a single push to determine whether individual push events or bulk push events are created. Bulk push events are created if it surpasses that value.
         :param pulumi.Input[int] push_event_hooks_limit: Number of changes (branches or tags) in a single push to determine whether webhooks and services fire or not. Webhooks and services aren’t submitted if it surpasses that value.
         :param pulumi.Input[bool] pypi_package_requests_forwarding: Use pypi.org as a default remote repository when the package is not found in the GitLab Package Registry for PyPI.
         :param pulumi.Input[str] rate_limiting_response_text: When rate limiting is enabled via the throttle_* settings, send this plain text response when a rate limit is exceeded. ‘Retry later’ is sent if this is blank.
-        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. To disable throttling set to 0.
         :param pulumi.Input[bool] recaptcha_enabled: (If enabled, requires: recaptcha*private*key and recaptcha*site*key) Enable reCAPTCHA.
         :param pulumi.Input[str] recaptcha_private_key: Private key for reCAPTCHA.
         :param pulumi.Input[str] recaptcha_site_key: Site key for reCAPTCHA.
         :param pulumi.Input[int] receive_max_input_size: Maximum push size (MB).
         :param pulumi.Input[bool] repository_checks_enabled: GitLab periodically runs git fsck in all project and wiki repositories to look for silent disk corruption issues.
         :param pulumi.Input[int] repository_size_limit: Size limit per repository (MB).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repository_storages: (GitLab 13.0 and earlier) List of names of enabled storage paths, taken from gitlab.yml. New projects are created in one of these stores, chosen at random.
         :param pulumi.Input[Mapping[str, pulumi.Input[int]]] repository_storages_weighted: (GitLab 13.1 and later) Hash of names of taken from gitlab.yml to weights. New projects are created in one of these stores, chosen by a weighted random selection.
         :param pulumi.Input[bool] require_admin_approval_after_user_signup: When enabled, any user that signs up for an account using the registration form is placed under a Pending approval state and has to be explicitly approved by an administrator.
         :param pulumi.Input[bool] require_two_factor_authentication: (If enabled, requires: two*factor*grace_period) Require all users to set up Two-factor authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
-        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
-        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
-        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
+        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
+        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
+        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         :param pulumi.Input[bool] send_user_confirmation_email: Send confirmation email on sign-up.
         :param pulumi.Input[int] session_expire_delay: Session duration in minutes. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] shared_runners_enabled: (If enabled, requires: shared*runners*text and shared*runners*minutes) Enable shared runners for new projects.
         :param pulumi.Input[int] shared_runners_minutes: Set the maximum number of CI/CD minutes that a group can use on shared runners per month.
         :param pulumi.Input[str] shared_runners_text: Shared runners text.
-        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
-        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
-        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
+        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
+        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits.
         :param pulumi.Input[str] sign_in_text: Text on the login page.
-        :param pulumi.Input[bool] signup_enabled: Enable registration. Default is true.
+        :param pulumi.Input[bool] signup_enabled: Enable registration.
         :param pulumi.Input[bool] slack_app_enabled: (If enabled, requires: slack*app*id, slack*app*secret and slack*app*secret) Enable Slack app.
         :param pulumi.Input[str] slack_app_id: The app ID of the Slack-app.
         :param pulumi.Input[str] slack_app_secret: The app secret of the Slack-app.
         :param pulumi.Input[str] slack_app_signing_secret: The signing secret of the Slack-app.
         :param pulumi.Input[str] slack_app_verification_token: The verification token of the Slack-app.
-        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes.
         :param pulumi.Input[str] snowplow_app_id: The Snowplow site name / application ID. (for example, gitlab)
         :param pulumi.Input[str] snowplow_collector_hostname: The Snowplow collector hostname. (for example, snowplow.trx.gitlab.net)
         :param pulumi.Input[str] snowplow_cookie_domain: The Snowplow cookie domain. (for example, .gitlab.com)
         :param pulumi.Input[bool] snowplow_enabled: Enable snowplow tracking.
-        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
-        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
+        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects.
         :param pulumi.Input[str] sourcegraph_url: The Sourcegraph instance URL for integration.
         :param pulumi.Input[str] spam_check_api_key: API key used by GitLab for accessing the Spam Check service endpoint.
-        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint. Default is false.
+        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint.
         :param pulumi.Input[str] spam_check_endpoint_url: URL of the external Spamcheck service endpoint. Valid URI schemes are grpc or tls. Specifying tls forces communication to be encrypted.
         :param pulumi.Input[bool] suggest_pipeline_enabled: Enable pipeline suggestion banner.
         :param pulumi.Input[int] terminal_max_session_time: Maximum time for web terminal websocket connection (in seconds). Set to 0 for unlimited time.
         :param pulumi.Input[str] terms: (Required by: enforce_terms) Markdown content for the ToS.
         :param pulumi.Input[bool] throttle_authenticated_api_enabled: (If enabled, requires: throttle*authenticated*api*period*in*seconds and throttle*authenticated*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_authenticated_api_period_in_seconds: Rate limit period (in seconds).
         :param pulumi.Input[int] throttle_authenticated_api_requests_per_period: Maximum requests per period per user.
@@ -8189,29 +8257,29 @@
         :param pulumi.Input[int] throttle_unauthenticated_api_requests_per_period: Max requests per period per IP.
         :param pulumi.Input[bool] throttle_unauthenticated_packages_api_enabled: (If enabled, requires: throttle*unauthenticated*packages*api*period*in*seconds and throttle*unauthenticated*packages*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_period_in_seconds: Rate limit period (in seconds). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_requests_per_period: Maximum requests per period per user. View Package Registry rate limits for more details.
         :param pulumi.Input[bool] throttle_unauthenticated_web_enabled: (If enabled, requires: throttle*unauthenticated*web*period*in*seconds and throttle*unauthenticated*web*requests*per*period) Enable unauthenticated web request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_unauthenticated_web_period_in_seconds: Rate limit period in seconds.
         :param pulumi.Input[int] throttle_unauthenticated_web_requests_per_period: Max requests per period per IP.
-        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours. Default is false.
+        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours.
         :param pulumi.Input[int] two_factor_grace_period: Amount of time (in hours) that users are allowed to skip forced configuration of two-factor authentication.
         :param pulumi.Input[bool] unique_ips_limit_enabled: (If enabled, requires: unique*ips*limit*per*user and unique*ips*limit*time*window) Limit sign in from multiple IPs.
         :param pulumi.Input[int] unique_ips_limit_per_user: Maximum number of IPs per user.
         :param pulumi.Input[int] unique_ips_limit_time_window: How many seconds an IP is counted towards the limit.
         :param pulumi.Input[bool] usage_ping_enabled: Every week GitLab reports license usage back to GitLab, Inc.
         :param pulumi.Input[bool] user_deactivation_emails_enabled: Send an email to users upon account deactivation.
         :param pulumi.Input[bool] user_default_external: Newly registered users are external by default.
         :param pulumi.Input[str] user_default_internal_regex: Specify an email address regex pattern to identify default internal users.
         :param pulumi.Input[bool] user_oauth_applications: Allow users to register any application to use GitLab as an OAuth provider.
         :param pulumi.Input[bool] user_show_add_ssh_key_message: When set to false disable the You won't be able to pull or push project code via SSH warning shown to users with no uploaded SSH key.
         :param pulumi.Input[bool] version_check_enabled: Let GitLab inform you when an update is available.
         :param pulumi.Input[bool] web_ide_clientside_preview_enabled: Live Preview (allow live previews of JavaScript projects in the Web IDE using CodeSandbox Live Preview).
         :param pulumi.Input[str] whats_new_variant: What’s new variant, possible values: all*tiers, current*tier, and disabled.
-        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApplicationSettingsArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -8257,14 +8325,15 @@
                  asset_proxy_enabled: Optional[pulumi.Input[bool]] = None,
                  asset_proxy_secret_key: Optional[pulumi.Input[str]] = None,
                  asset_proxy_url: Optional[pulumi.Input[str]] = None,
                  authorized_keys_enabled: Optional[pulumi.Input[bool]] = None,
                  auto_devops_domain: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  automatic_purchased_storage_allocation: Optional[pulumi.Input[bool]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
                  check_namespace_plan: Optional[pulumi.Input[bool]] = None,
                  commit_email_hostname: Optional[pulumi.Input[str]] = None,
                  container_expiration_policies_enable_historic_entries: Optional[pulumi.Input[bool]] = None,
                  container_registry_cleanup_tags_service_max_list_size: Optional[pulumi.Input[int]] = None,
                  container_registry_delete_tags_service_timeout: Optional[pulumi.Input[int]] = None,
                  container_registry_expiration_policies_caching: Optional[pulumi.Input[bool]] = None,
                  container_registry_expiration_policies_worker_capacity: Optional[pulumi.Input[int]] = None,
@@ -8340,14 +8409,15 @@
                  git_two_factor_session_expiry: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_default: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_fast: Optional[pulumi.Input[int]] = None,
                  gitaly_timeout_medium: Optional[pulumi.Input[int]] = None,
                  grafana_enabled: Optional[pulumi.Input[bool]] = None,
                  grafana_url: Optional[pulumi.Input[str]] = None,
                  gravatar_enabled: Optional[pulumi.Input[bool]] = None,
+                 group_owners_can_manage_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  hashed_storage_enabled: Optional[pulumi.Input[bool]] = None,
                  help_page_hide_commercial_content: Optional[pulumi.Input[bool]] = None,
                  help_page_support_url: Optional[pulumi.Input[str]] = None,
                  help_page_text: Optional[pulumi.Input[str]] = None,
                  help_text: Optional[pulumi.Input[str]] = None,
                  hide_third_party_offers: Optional[pulumi.Input[bool]] = None,
                  home_page_url: Optional[pulumi.Input[str]] = None,
@@ -8506,14 +8576,15 @@
             __props__.__dict__["asset_proxy_enabled"] = asset_proxy_enabled
             __props__.__dict__["asset_proxy_secret_key"] = None if asset_proxy_secret_key is None else pulumi.Output.secret(asset_proxy_secret_key)
             __props__.__dict__["asset_proxy_url"] = asset_proxy_url
             __props__.__dict__["authorized_keys_enabled"] = authorized_keys_enabled
             __props__.__dict__["auto_devops_domain"] = auto_devops_domain
             __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
             __props__.__dict__["automatic_purchased_storage_allocation"] = automatic_purchased_storage_allocation
+            __props__.__dict__["can_create_group"] = can_create_group
             __props__.__dict__["check_namespace_plan"] = check_namespace_plan
             __props__.__dict__["commit_email_hostname"] = commit_email_hostname
             __props__.__dict__["container_expiration_policies_enable_historic_entries"] = container_expiration_policies_enable_historic_entries
             __props__.__dict__["container_registry_cleanup_tags_service_max_list_size"] = container_registry_cleanup_tags_service_max_list_size
             __props__.__dict__["container_registry_delete_tags_service_timeout"] = container_registry_delete_tags_service_timeout
             __props__.__dict__["container_registry_expiration_policies_caching"] = container_registry_expiration_policies_caching
             __props__.__dict__["container_registry_expiration_policies_worker_capacity"] = container_registry_expiration_policies_worker_capacity
@@ -8589,14 +8660,15 @@
             __props__.__dict__["git_two_factor_session_expiry"] = git_two_factor_session_expiry
             __props__.__dict__["gitaly_timeout_default"] = gitaly_timeout_default
             __props__.__dict__["gitaly_timeout_fast"] = gitaly_timeout_fast
             __props__.__dict__["gitaly_timeout_medium"] = gitaly_timeout_medium
             __props__.__dict__["grafana_enabled"] = grafana_enabled
             __props__.__dict__["grafana_url"] = grafana_url
             __props__.__dict__["gravatar_enabled"] = gravatar_enabled
+            __props__.__dict__["group_owners_can_manage_default_branch_protection"] = group_owners_can_manage_default_branch_protection
             __props__.__dict__["hashed_storage_enabled"] = hashed_storage_enabled
             __props__.__dict__["help_page_hide_commercial_content"] = help_page_hide_commercial_content
             __props__.__dict__["help_page_support_url"] = help_page_support_url
             __props__.__dict__["help_page_text"] = help_page_text
             __props__.__dict__["help_text"] = help_text
             __props__.__dict__["hide_third_party_offers"] = hide_third_party_offers
             __props__.__dict__["home_page_url"] = home_page_url
@@ -8758,14 +8830,15 @@
             asset_proxy_enabled: Optional[pulumi.Input[bool]] = None,
             asset_proxy_secret_key: Optional[pulumi.Input[str]] = None,
             asset_proxy_url: Optional[pulumi.Input[str]] = None,
             authorized_keys_enabled: Optional[pulumi.Input[bool]] = None,
             auto_devops_domain: Optional[pulumi.Input[str]] = None,
             auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
             automatic_purchased_storage_allocation: Optional[pulumi.Input[bool]] = None,
+            can_create_group: Optional[pulumi.Input[bool]] = None,
             check_namespace_plan: Optional[pulumi.Input[bool]] = None,
             commit_email_hostname: Optional[pulumi.Input[str]] = None,
             container_expiration_policies_enable_historic_entries: Optional[pulumi.Input[bool]] = None,
             container_registry_cleanup_tags_service_max_list_size: Optional[pulumi.Input[int]] = None,
             container_registry_delete_tags_service_timeout: Optional[pulumi.Input[int]] = None,
             container_registry_expiration_policies_caching: Optional[pulumi.Input[bool]] = None,
             container_registry_expiration_policies_worker_capacity: Optional[pulumi.Input[int]] = None,
@@ -8841,14 +8914,15 @@
             git_two_factor_session_expiry: Optional[pulumi.Input[int]] = None,
             gitaly_timeout_default: Optional[pulumi.Input[int]] = None,
             gitaly_timeout_fast: Optional[pulumi.Input[int]] = None,
             gitaly_timeout_medium: Optional[pulumi.Input[int]] = None,
             grafana_enabled: Optional[pulumi.Input[bool]] = None,
             grafana_url: Optional[pulumi.Input[str]] = None,
             gravatar_enabled: Optional[pulumi.Input[bool]] = None,
+            group_owners_can_manage_default_branch_protection: Optional[pulumi.Input[bool]] = None,
             hashed_storage_enabled: Optional[pulumi.Input[bool]] = None,
             help_page_hide_commercial_content: Optional[pulumi.Input[bool]] = None,
             help_page_support_url: Optional[pulumi.Input[str]] = None,
             help_page_text: Optional[pulumi.Input[str]] = None,
             help_text: Optional[pulumi.Input[str]] = None,
             hide_third_party_offers: Optional[pulumi.Input[bool]] = None,
             home_page_url: Optional[pulumi.Input[str]] = None,
@@ -9005,50 +9079,51 @@
         :param pulumi.Input[bool] asset_proxy_enabled: (If enabled, requires: asset*proxy*url) Enable proxying of assets. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_secret_key: Shared secret with the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[str] asset_proxy_url: URL of the asset proxy server. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] authorized_keys_enabled: By default, we write to the authorized_keys file to support Git over SSH without additional configuration. GitLab can be optimized to authenticate SSH keys via the database file. Only disable this if you have configured your OpenSSH server to use the AuthorizedKeysCommand.
         :param pulumi.Input[str] auto_devops_domain: Specify a domain to use by default for every project’s Auto Review Apps and Auto Deploy stages.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for projects by default. It automatically builds, tests, and deploys applications based on a predefined CI/CD configuration.
         :param pulumi.Input[bool] automatic_purchased_storage_allocation: Enabling this permits automatic allocation of purchased storage in a namespace.
+        :param pulumi.Input[bool] can_create_group: Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
         :param pulumi.Input[bool] check_namespace_plan: Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         :param pulumi.Input[str] commit_email_hostname: Custom hostname (for private commit emails).
         :param pulumi.Input[bool] container_expiration_policies_enable_historic_entries: Enable cleanup policies for all projects.
         :param pulumi.Input[int] container_registry_cleanup_tags_service_max_list_size: The maximum number of tags that can be deleted in a single execution of cleanup policies.
         :param pulumi.Input[int] container_registry_delete_tags_service_timeout: The maximum time, in seconds, that the cleanup process can take to delete a batch of tags for cleanup policies.
         :param pulumi.Input[bool] container_registry_expiration_policies_caching: Caching during the execution of cleanup policies.
         :param pulumi.Input[int] container_registry_expiration_policies_worker_capacity: Number of workers for cleanup policies.
         :param pulumi.Input[int] container_registry_token_expire_delay: Container Registry token duration in minutes.
         :param pulumi.Input[bool] deactivate_dormant_users: Enable automatic deactivation of dormant users.
         :param pulumi.Input[str] default_artifacts_expire_in: Set the default expiration time for each job’s artifacts.
         :param pulumi.Input[str] default_branch_name: Instance-level custom initial branch name (introduced in GitLab 13.2).
         :param pulumi.Input[int] default_branch_protection: Determine if developers can push to the default branch. Can take: 0 (not protected, both users with the Developer role or Maintainer role can push new commits and force push), 1 (partially protected, users with the Developer role or Maintainer role can push new commits, but cannot force push) or 2 (fully protected, users with the Developer or Maintainer role cannot push new commits, but users with the Developer or Maintainer role can; no one can force push) as a parameter. Default is 2.
         :param pulumi.Input[str] default_ci_config_path: Default CI/CD configuration file and path for new projects (.gitlab-ci.yml if not set).
-        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        :param pulumi.Input[str] default_group_visibility: What visibility level new groups receive. Can take private, internal and public as a parameter.
         :param pulumi.Input[int] default_project_creation: Default project creation protection. Can take: 0 (No one), 1 (Maintainers) or 2 (Developers + Maintainers).
-        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[int] default_projects_limit: Project limit per user. Default is 100000.
-        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
-        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
-        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
-        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
-        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        :param pulumi.Input[str] default_project_visibility: What visibility level new projects receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[int] default_projects_limit: Project limit per user.
+        :param pulumi.Input[str] default_snippet_visibility: What visibility level new snippets receive. Can take private, internal and public as a parameter.
+        :param pulumi.Input[bool] delayed_group_deletion: Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        :param pulumi.Input[bool] delayed_project_deletion: Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        :param pulumi.Input[bool] delete_inactive_projects: Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
+        :param pulumi.Input[int] deletion_adjourned_period: The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         :param pulumi.Input[int] diff_max_files: Maximum files in a diff.
         :param pulumi.Input[int] diff_max_lines: Maximum lines in a diff.
         :param pulumi.Input[int] diff_max_patch_bytes: Maximum diff patch size, in bytes.
         :param pulumi.Input[bool] disable_feed_token: Disable display of RSS/Atom and calendar feed tokens (introduced in GitLab 13.7).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disabled_oauth_sign_in_sources: Disabled OAuth sign-in sources.
         :param pulumi.Input[bool] dns_rebinding_protection_enabled: Enforce DNS rebinding attack protection.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_allowlists: Force people to use only corporate emails for sign-up. Null means there is no restriction.
         :param pulumi.Input[bool] domain_denylist_enabled: (If enabled, requires: domain_denylist) Allows blocking sign-ups from emails from specific domains.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] domain_denylists: Users with email addresses that match these domains cannot sign up. Wildcards allowed. Use separate lines for multiple entries. Ex: domain.com, *.domain.com.
-        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
-        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
-        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
-        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
-        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        :param pulumi.Input[int] dsa_key_restriction: The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
+        :param pulumi.Input[int] ecdsa_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
+        :param pulumi.Input[int] ecdsa_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
+        :param pulumi.Input[int] ed25519_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
+        :param pulumi.Input[int] ed25519_sk_key_restriction: The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         :param pulumi.Input[str] eks_access_key_id: AWS IAM access key ID.
         :param pulumi.Input[str] eks_account_id: Amazon account ID.
         :param pulumi.Input[bool] eks_integration_enabled: Enable integration with Amazon EKS.
         :param pulumi.Input[str] eks_secret_access_key: AWS IAM secret access key.
         :param pulumi.Input[bool] elasticsearch_aws: Enable the use of AWS hosted Elasticsearch.
         :param pulumi.Input[str] elasticsearch_aws_access_key: AWS IAM access key.
         :param pulumi.Input[str] elasticsearch_aws_region: The AWS region the Elasticsearch domain is configured.
@@ -9077,127 +9152,128 @@
         :param pulumi.Input[bool] external_authorization_service_enabled: (If enabled, requires: external*authorization*service*default*label, external*authorization*service*timeout and external*authorization*service*url) Enable using an external authorization service for accessing projects.
         :param pulumi.Input[float] external_authorization_service_timeout: The timeout after which an authorization request is aborted, in seconds. When a request times out, access is denied to the user. (min: 0.001, max: 10, step: 0.001).
         :param pulumi.Input[str] external_authorization_service_url: URL to which authorization requests are directed.
         :param pulumi.Input[int] external_pipeline_validation_service_timeout: How long to wait for a response from the pipeline validation service. Assumes OK if it times out.
         :param pulumi.Input[str] external_pipeline_validation_service_token: Optional. Token to include as the X-Gitlab-Token header in requests to the URL in external*pipeline*validation*service*url.
         :param pulumi.Input[str] external_pipeline_validation_service_url: URL to use for pipeline validation requests.
         :param pulumi.Input[int] file_template_project_id: The ID of a project to load custom file templates from.
-        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        :param pulumi.Input[int] first_day_of_week: Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         :param pulumi.Input[str] geo_node_allowed_ips: Comma-separated list of IPs and CIDRs of allowed secondary nodes. For example, 1.1.1.1, 2.2.2.0/24.
         :param pulumi.Input[int] geo_status_timeout: The amount of seconds after which a request to get a secondary node status times out.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] git_rate_limit_users_allowlists: List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         :param pulumi.Input[int] git_two_factor_session_expiry: Maximum duration (in minutes) of a session for Git operations when 2FA is enabled.
         :param pulumi.Input[int] gitaly_timeout_default: Default Gitaly timeout, in seconds. This timeout is not enforced for Git fetch/push operations or Sidekiq jobs. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_fast: Gitaly fast operation timeout, in seconds. Some Gitaly operations are expected to be fast. If they exceed this threshold, there may be a problem with a storage shard and ‘failing fast’ can help maintain the stability of the GitLab instance. Set to 0 to disable timeouts.
         :param pulumi.Input[int] gitaly_timeout_medium: Medium Gitaly timeout, in seconds. This should be a value between the Fast and the Default timeout. Set to 0 to disable timeouts.
         :param pulumi.Input[bool] grafana_enabled: Enable Grafana.
         :param pulumi.Input[str] grafana_url: Grafana URL.
         :param pulumi.Input[bool] gravatar_enabled: Enable Gravatar.
+        :param pulumi.Input[bool] group_owners_can_manage_default_branch_protection: Prevent overrides of default branch protection.
         :param pulumi.Input[bool] hashed_storage_enabled: Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         :param pulumi.Input[bool] help_page_hide_commercial_content: Hide marketing-related entries from help.
         :param pulumi.Input[str] help_page_support_url: Alternate support URL for help page and help dropdown.
         :param pulumi.Input[str] help_page_text: Custom text displayed on the help page.
         :param pulumi.Input[str] help_text: GitLab server administrator information.
         :param pulumi.Input[bool] hide_third_party_offers: Do not display offers from third parties in GitLab.
         :param pulumi.Input[str] home_page_url: Redirect to this URL when not logged in.
         :param pulumi.Input[bool] housekeeping_enabled: (If enabled, requires: housekeeping*bitmaps*enabled, housekeeping*full*repack*period, housekeeping*gc*period, and housekeeping*incremental*repack*period) Enable or disable Git housekeeping.
         :param pulumi.Input[int] housekeeping_full_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[int] housekeeping_gc_period: Number of Git pushes after which git gc is run.
         :param pulumi.Input[int] housekeeping_incremental_repack_period: Number of Git pushes after which an incremental git repack is run.
         :param pulumi.Input[bool] html_emails_enabled: Enable HTML emails.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] import_sources: Sources to allow project import from, possible values: github, bitbucket, bitbucket*server, gitlab, fogbugz, git, gitlab*project, gitea, manifest, and phabricator.
-        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails. Enabled by default.
-        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
-        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
-        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user. Disabled by default.
-        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        :param pulumi.Input[bool] in_product_marketing_emails_enabled: Enable in-product marketing emails.
+        :param pulumi.Input[int] inactive_projects_delete_after_months: If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_min_size_mb: If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[int] inactive_projects_send_warning_email_after_months: If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        :param pulumi.Input[bool] invisible_captcha_enabled: Enable Invisible CAPTCHA spam detection during sign-up.
+        :param pulumi.Input[int] issues_create_limit: Max number of issue creation requests per minute per user.
+        :param pulumi.Input[bool] keep_latest_artifact: Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         :param pulumi.Input[int] local_markdown_version: Increase this value when any cached Markdown should be invalidated.
         :param pulumi.Input[bool] mailgun_events_enabled: Enable Mailgun event receiver.
         :param pulumi.Input[str] mailgun_signing_key: The Mailgun HTTP webhook signing key for receiving events from webhook.
         :param pulumi.Input[bool] maintenance_mode: When instance is in maintenance mode, non-administrative users can sign in with read-only access and make read-only API requests.
         :param pulumi.Input[str] maintenance_mode_message: Message displayed when instance is in maintenance mode.
         :param pulumi.Input[int] max_artifacts_size: Maximum artifacts size in MB.
         :param pulumi.Input[int] max_attachment_size: Limit attachment size in MB.
-        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
-        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
-        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
-        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_export_size: Maximum export size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_import_size: Maximum import size in MB. 0 for unlimited.
+        :param pulumi.Input[int] max_number_of_repository_downloads: Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        :param pulumi.Input[int] max_number_of_repository_downloads_within_time_period: Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         :param pulumi.Input[int] max_pages_size: Maximum size of pages repositories in MB.
         :param pulumi.Input[int] max_personal_access_token_lifetime: Maximum allowable lifetime for access tokens in days.
         :param pulumi.Input[int] max_ssh_key_lifetime: Maximum allowable lifetime for SSH keys in days. Introduced in GitLab 14.6.
         :param pulumi.Input[int] metrics_method_call_threshold: A method call is only tracked when it takes longer than the given amount of milliseconds.
         :param pulumi.Input[bool] mirror_available: Allow repository mirroring to configured by project Maintainers. If disabled, only Administrators can configure repository mirroring.
         :param pulumi.Input[int] mirror_capacity_threshold: Minimum capacity to be available before scheduling more mirrors preemptively.
         :param pulumi.Input[int] mirror_max_capacity: Maximum number of mirrors that can be synchronizing at the same time.
         :param pulumi.Input[int] mirror_max_delay: Maximum time (in minutes) between updates that a mirror can have when scheduled to synchronize.
         :param pulumi.Input[bool] npm_package_requests_forwarding: Use npmjs.org as a default remote repository when the package is not found in the GitLab Package Registry for npm.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] outbound_local_requests_whitelists: Define a list of trusted domains or IP addresses to which local requests are allowed when local requests for hooks and services are disabled.
         :param pulumi.Input[int] package_registry_cleanup_policies_worker_capacity: Number of workers assigned to the packages cleanup policies.
         :param pulumi.Input[bool] pages_domain_verification_enabled: Require users to prove ownership of custom domains. Domain verification is an essential security measure for public GitLab sites. Users are required to demonstrate they control a domain before it is enabled.
-        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
-        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password. Default is true.
+        :param pulumi.Input[bool] password_authentication_enabled_for_git: Enable authentication for Git over HTTP(S) via a GitLab account password.
+        :param pulumi.Input[bool] password_authentication_enabled_for_web: Enable authentication for the web interface via a GitLab account password.
         :param pulumi.Input[bool] password_lowercase_required: Indicates whether passwords require at least one lowercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_number_required: Indicates whether passwords require at least one number. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_symbol_required: Indicates whether passwords require at least one symbol character. Introduced in GitLab 15.1.
         :param pulumi.Input[bool] password_uppercase_required: Indicates whether passwords require at least one uppercase letter. Introduced in GitLab 15.1.
         :param pulumi.Input[str] performance_bar_allowed_group_path: Path of the group that is allowed to toggle the performance bar.
         :param pulumi.Input[str] personal_access_token_prefix: Prefix for all generated personal access tokens.
-        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
-        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        :param pulumi.Input[int] pipeline_limit_per_project_user_sha: Maximum number of pipeline creation requests per minute per user and commit.
+        :param pulumi.Input[bool] plantuml_enabled: (If enabled, requires: plantuml_url) Enable PlantUML integration.
         :param pulumi.Input[str] plantuml_url: The PlantUML instance URL for integration.
         :param pulumi.Input[float] polling_interval_multiplier: Interval multiplier used by endpoints that perform polling. Set to 0 to disable polling.
         :param pulumi.Input[bool] project_export_enabled: Enable project export.
         :param pulumi.Input[bool] prometheus_metrics_enabled: Enable Prometheus metrics.
         :param pulumi.Input[bool] protected_ci_variables: CI/CD variables are protected by default.
         :param pulumi.Input[int] push_event_activities_limit: Number of changes (branches or tags) in a single push to determine whether individual push events or bulk push events are created. Bulk push events are created if it surpasses that value.
         :param pulumi.Input[int] push_event_hooks_limit: Number of changes (branches or tags) in a single push to determine whether webhooks and services fire or not. Webhooks and services aren’t submitted if it surpasses that value.
         :param pulumi.Input[bool] pypi_package_requests_forwarding: Use pypi.org as a default remote repository when the package is not found in the GitLab Package Registry for PyPI.
         :param pulumi.Input[str] rate_limiting_response_text: When rate limiting is enabled via the throttle_* settings, send this plain text response when a rate limit is exceeded. ‘Retry later’ is sent if this is blank.
-        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        :param pulumi.Input[int] raw_blob_request_limit: Max number of requests per minute for each raw path. To disable throttling set to 0.
         :param pulumi.Input[bool] recaptcha_enabled: (If enabled, requires: recaptcha*private*key and recaptcha*site*key) Enable reCAPTCHA.
         :param pulumi.Input[str] recaptcha_private_key: Private key for reCAPTCHA.
         :param pulumi.Input[str] recaptcha_site_key: Site key for reCAPTCHA.
         :param pulumi.Input[int] receive_max_input_size: Maximum push size (MB).
         :param pulumi.Input[bool] repository_checks_enabled: GitLab periodically runs git fsck in all project and wiki repositories to look for silent disk corruption issues.
         :param pulumi.Input[int] repository_size_limit: Size limit per repository (MB).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] repository_storages: (GitLab 13.0 and earlier) List of names of enabled storage paths, taken from gitlab.yml. New projects are created in one of these stores, chosen at random.
         :param pulumi.Input[Mapping[str, pulumi.Input[int]]] repository_storages_weighted: (GitLab 13.1 and later) Hash of names of taken from gitlab.yml to weights. New projects are created in one of these stores, chosen by a weighted random selection.
         :param pulumi.Input[bool] require_admin_approval_after_user_signup: When enabled, any user that signs up for an account using the registration form is placed under a Pending approval state and has to be explicitly approved by an administrator.
         :param pulumi.Input[bool] require_two_factor_authentication: (If enabled, requires: two*factor*grace_period) Require all users to set up Two-factor authentication.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
-        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
-        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
-        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] restricted_visibility_levels: Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
+        :param pulumi.Input[int] rsa_key_restriction: The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
+        :param pulumi.Input[int] search_rate_limit: Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
+        :param pulumi.Input[int] search_rate_limit_unauthenticated: Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         :param pulumi.Input[bool] send_user_confirmation_email: Send confirmation email on sign-up.
         :param pulumi.Input[int] session_expire_delay: Session duration in minutes. GitLab restart is required to apply changes.
         :param pulumi.Input[bool] shared_runners_enabled: (If enabled, requires: shared*runners*text and shared*runners*minutes) Enable shared runners for new projects.
         :param pulumi.Input[int] shared_runners_minutes: Set the maximum number of CI/CD minutes that a group can use on shared runners per month.
         :param pulumi.Input[str] shared_runners_text: Shared runners text.
-        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
-        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
-        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        :param pulumi.Input[int] sidekiq_job_limiter_compression_threshold_bytes: The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
+        :param pulumi.Input[int] sidekiq_job_limiter_limit_bytes: The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
+        :param pulumi.Input[str] sidekiq_job_limiter_mode: track or compress. Sets the behavior for Sidekiq job size limits.
         :param pulumi.Input[str] sign_in_text: Text on the login page.
-        :param pulumi.Input[bool] signup_enabled: Enable registration. Default is true.
+        :param pulumi.Input[bool] signup_enabled: Enable registration.
         :param pulumi.Input[bool] slack_app_enabled: (If enabled, requires: slack*app*id, slack*app*secret and slack*app*secret) Enable Slack app.
         :param pulumi.Input[str] slack_app_id: The app ID of the Slack-app.
         :param pulumi.Input[str] slack_app_secret: The app secret of the Slack-app.
         :param pulumi.Input[str] slack_app_signing_secret: The signing secret of the Slack-app.
         :param pulumi.Input[str] slack_app_verification_token: The verification token of the Slack-app.
-        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        :param pulumi.Input[int] snippet_size_limit: Max snippet content size in bytes.
         :param pulumi.Input[str] snowplow_app_id: The Snowplow site name / application ID. (for example, gitlab)
         :param pulumi.Input[str] snowplow_collector_hostname: The Snowplow collector hostname. (for example, snowplow.trx.gitlab.net)
         :param pulumi.Input[str] snowplow_cookie_domain: The Snowplow cookie domain. (for example, .gitlab.com)
         :param pulumi.Input[bool] snowplow_enabled: Enable snowplow tracking.
-        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
-        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        :param pulumi.Input[bool] sourcegraph_enabled: Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
+        :param pulumi.Input[bool] sourcegraph_public_only: Blocks Sourcegraph from being loaded on private and internal projects.
         :param pulumi.Input[str] sourcegraph_url: The Sourcegraph instance URL for integration.
         :param pulumi.Input[str] spam_check_api_key: API key used by GitLab for accessing the Spam Check service endpoint.
-        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint. Default is false.
+        :param pulumi.Input[bool] spam_check_endpoint_enabled: Enables spam checking using external Spam Check API endpoint.
         :param pulumi.Input[str] spam_check_endpoint_url: URL of the external Spamcheck service endpoint. Valid URI schemes are grpc or tls. Specifying tls forces communication to be encrypted.
         :param pulumi.Input[bool] suggest_pipeline_enabled: Enable pipeline suggestion banner.
         :param pulumi.Input[int] terminal_max_session_time: Maximum time for web terminal websocket connection (in seconds). Set to 0 for unlimited time.
         :param pulumi.Input[str] terms: (Required by: enforce_terms) Markdown content for the ToS.
         :param pulumi.Input[bool] throttle_authenticated_api_enabled: (If enabled, requires: throttle*authenticated*api*period*in*seconds and throttle*authenticated*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_authenticated_api_period_in_seconds: Rate limit period (in seconds).
         :param pulumi.Input[int] throttle_authenticated_api_requests_per_period: Maximum requests per period per user.
@@ -9212,29 +9288,29 @@
         :param pulumi.Input[int] throttle_unauthenticated_api_requests_per_period: Max requests per period per IP.
         :param pulumi.Input[bool] throttle_unauthenticated_packages_api_enabled: (If enabled, requires: throttle*unauthenticated*packages*api*period*in*seconds and throttle*unauthenticated*packages*api*requests*per*period) Enable authenticated API request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_period_in_seconds: Rate limit period (in seconds). View Package Registry rate limits for more details.
         :param pulumi.Input[int] throttle_unauthenticated_packages_api_requests_per_period: Maximum requests per period per user. View Package Registry rate limits for more details.
         :param pulumi.Input[bool] throttle_unauthenticated_web_enabled: (If enabled, requires: throttle*unauthenticated*web*period*in*seconds and throttle*unauthenticated*web*requests*per*period) Enable unauthenticated web request rate limit. Helps reduce request volume (for example, from crawlers or abusive bots).
         :param pulumi.Input[int] throttle_unauthenticated_web_period_in_seconds: Rate limit period in seconds.
         :param pulumi.Input[int] throttle_unauthenticated_web_requests_per_period: Max requests per period per IP.
-        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours. Default is false.
+        :param pulumi.Input[bool] time_tracking_limit_to_hours: Limit display of time tracking units to hours.
         :param pulumi.Input[int] two_factor_grace_period: Amount of time (in hours) that users are allowed to skip forced configuration of two-factor authentication.
         :param pulumi.Input[bool] unique_ips_limit_enabled: (If enabled, requires: unique*ips*limit*per*user and unique*ips*limit*time*window) Limit sign in from multiple IPs.
         :param pulumi.Input[int] unique_ips_limit_per_user: Maximum number of IPs per user.
         :param pulumi.Input[int] unique_ips_limit_time_window: How many seconds an IP is counted towards the limit.
         :param pulumi.Input[bool] usage_ping_enabled: Every week GitLab reports license usage back to GitLab, Inc.
         :param pulumi.Input[bool] user_deactivation_emails_enabled: Send an email to users upon account deactivation.
         :param pulumi.Input[bool] user_default_external: Newly registered users are external by default.
         :param pulumi.Input[str] user_default_internal_regex: Specify an email address regex pattern to identify default internal users.
         :param pulumi.Input[bool] user_oauth_applications: Allow users to register any application to use GitLab as an OAuth provider.
         :param pulumi.Input[bool] user_show_add_ssh_key_message: When set to false disable the You won't be able to pull or push project code via SSH warning shown to users with no uploaded SSH key.
         :param pulumi.Input[bool] version_check_enabled: Let GitLab inform you when an update is available.
         :param pulumi.Input[bool] web_ide_clientside_preview_enabled: Live Preview (allow live previews of JavaScript projects in the Web IDE using CodeSandbox Live Preview).
         :param pulumi.Input[str] whats_new_variant: What’s new variant, possible values: all*tiers, current*tier, and disabled.
-        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        :param pulumi.Input[int] wiki_page_max_content_bytes: Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ApplicationSettingsState.__new__(_ApplicationSettingsState)
 
         __props__.__dict__["abuse_notification_email"] = abuse_notification_email
         __props__.__dict__["admin_mode"] = admin_mode
@@ -9250,14 +9326,15 @@
         __props__.__dict__["asset_proxy_enabled"] = asset_proxy_enabled
         __props__.__dict__["asset_proxy_secret_key"] = asset_proxy_secret_key
         __props__.__dict__["asset_proxy_url"] = asset_proxy_url
         __props__.__dict__["authorized_keys_enabled"] = authorized_keys_enabled
         __props__.__dict__["auto_devops_domain"] = auto_devops_domain
         __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
         __props__.__dict__["automatic_purchased_storage_allocation"] = automatic_purchased_storage_allocation
+        __props__.__dict__["can_create_group"] = can_create_group
         __props__.__dict__["check_namespace_plan"] = check_namespace_plan
         __props__.__dict__["commit_email_hostname"] = commit_email_hostname
         __props__.__dict__["container_expiration_policies_enable_historic_entries"] = container_expiration_policies_enable_historic_entries
         __props__.__dict__["container_registry_cleanup_tags_service_max_list_size"] = container_registry_cleanup_tags_service_max_list_size
         __props__.__dict__["container_registry_delete_tags_service_timeout"] = container_registry_delete_tags_service_timeout
         __props__.__dict__["container_registry_expiration_policies_caching"] = container_registry_expiration_policies_caching
         __props__.__dict__["container_registry_expiration_policies_worker_capacity"] = container_registry_expiration_policies_worker_capacity
@@ -9333,14 +9410,15 @@
         __props__.__dict__["git_two_factor_session_expiry"] = git_two_factor_session_expiry
         __props__.__dict__["gitaly_timeout_default"] = gitaly_timeout_default
         __props__.__dict__["gitaly_timeout_fast"] = gitaly_timeout_fast
         __props__.__dict__["gitaly_timeout_medium"] = gitaly_timeout_medium
         __props__.__dict__["grafana_enabled"] = grafana_enabled
         __props__.__dict__["grafana_url"] = grafana_url
         __props__.__dict__["gravatar_enabled"] = gravatar_enabled
+        __props__.__dict__["group_owners_can_manage_default_branch_protection"] = group_owners_can_manage_default_branch_protection
         __props__.__dict__["hashed_storage_enabled"] = hashed_storage_enabled
         __props__.__dict__["help_page_hide_commercial_content"] = help_page_hide_commercial_content
         __props__.__dict__["help_page_support_url"] = help_page_support_url
         __props__.__dict__["help_page_text"] = help_page_text
         __props__.__dict__["help_text"] = help_text
         __props__.__dict__["hide_third_party_offers"] = hide_third_party_offers
         __props__.__dict__["home_page_url"] = home_page_url
@@ -9619,14 +9697,22 @@
     def automatic_purchased_storage_allocation(self) -> pulumi.Output[bool]:
         """
         Enabling this permits automatic allocation of purchased storage in a namespace.
         """
         return pulumi.get(self, "automatic_purchased_storage_allocation")
 
     @property
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> pulumi.Output[bool]:
+        """
+        Indicates whether users can create top-level groups. Introduced in GitLab 15.5.
+        """
+        return pulumi.get(self, "can_create_group")
+
+    @property
     @pulumi.getter(name="checkNamespacePlan")
     def check_namespace_plan(self) -> pulumi.Output[bool]:
         """
         Enabling this makes only licensed EE features available to projects if the project namespace’s plan includes the feature or if the project is public.
         """
         return pulumi.get(self, "check_namespace_plan")
 
@@ -9726,15 +9812,15 @@
         """
         return pulumi.get(self, "default_ci_config_path")
 
     @property
     @pulumi.getter(name="defaultGroupVisibility")
     def default_group_visibility(self) -> pulumi.Output[str]:
         """
-        What visibility level new groups receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new groups receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_group_visibility")
 
     @property
     @pulumi.getter(name="defaultProjectCreation")
     def default_project_creation(self) -> pulumi.Output[int]:
         """
@@ -9742,63 +9828,63 @@
         """
         return pulumi.get(self, "default_project_creation")
 
     @property
     @pulumi.getter(name="defaultProjectVisibility")
     def default_project_visibility(self) -> pulumi.Output[str]:
         """
-        What visibility level new projects receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new projects receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_project_visibility")
 
     @property
     @pulumi.getter(name="defaultProjectsLimit")
     def default_projects_limit(self) -> pulumi.Output[int]:
         """
-        Project limit per user. Default is 100000.
+        Project limit per user.
         """
         return pulumi.get(self, "default_projects_limit")
 
     @property
     @pulumi.getter(name="defaultSnippetVisibility")
     def default_snippet_visibility(self) -> pulumi.Output[str]:
         """
-        What visibility level new snippets receive. Can take private, internal and public as a parameter. Default is private.
+        What visibility level new snippets receive. Can take private, internal and public as a parameter.
         """
         return pulumi.get(self, "default_snippet_visibility")
 
     @property
     @pulumi.getter(name="delayedGroupDeletion")
     def delayed_group_deletion(self) -> pulumi.Output[bool]:
         """
-        Enable delayed group deletion. Default is true. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
+        Enable delayed group deletion. Introduced in GitLab 15.0. From GitLab 15.1, disables and locks the group-level setting for delayed protect deletion when set to false.
         """
         return pulumi.get(self, "delayed_group_deletion")
 
     @property
     @pulumi.getter(name="delayedProjectDeletion")
     def delayed_project_deletion(self) -> pulumi.Output[bool]:
         """
-        Enable delayed project deletion by default in new groups. Default is false. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
+        Enable delayed project deletion by default in new groups. From GitLab 15.1, can only be enabled when delayed*group*deletion is true.
         """
         return pulumi.get(self, "delayed_project_deletion")
 
     @property
     @pulumi.getter(name="deleteInactiveProjects")
     def delete_inactive_projects(self) -> pulumi.Output[bool]:
         """
-        Enable inactive project deletion feature. Default is false. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion, disabled by default).
+        Enable inactive project deletion feature. Introduced in GitLab 14.10. Became operational in GitLab 15.0 (with feature flag inactive*projects*deletion).
         """
         return pulumi.get(self, "delete_inactive_projects")
 
     @property
     @pulumi.getter(name="deletionAdjournedPeriod")
     def deletion_adjourned_period(self) -> pulumi.Output[int]:
         """
-        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. Defaults to 7. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
+        The number of days to wait before deleting a project or group that is marked for deletion. Value must be between 1 and 90. From GitLab 15.1, a hook on deletion*adjourned*period sets the period to 1 on every update, and sets both delayed*project*deletion and delayed*group*deletion to false if the period is 0.
         """
         return pulumi.get(self, "deletion_adjourned_period")
 
     @property
     @pulumi.getter(name="diffMaxFiles")
     def diff_max_files(self) -> pulumi.Output[int]:
         """
@@ -9846,15 +9932,15 @@
         """
         return pulumi.get(self, "dns_rebinding_protection_enabled")
 
     @property
     @pulumi.getter(name="domainAllowlists")
     def domain_allowlists(self) -> pulumi.Output[Sequence[str]]:
         """
-        Force people to use only corporate emails for sign-up. Default is null, meaning there is no restriction.
+        Force people to use only corporate emails for sign-up. Null means there is no restriction.
         """
         return pulumi.get(self, "domain_allowlists")
 
     @property
     @pulumi.getter(name="domainDenylistEnabled")
     def domain_denylist_enabled(self) -> pulumi.Output[bool]:
         """
@@ -9870,47 +9956,47 @@
         """
         return pulumi.get(self, "domain_denylists")
 
     @property
     @pulumi.getter(name="dsaKeyRestriction")
     def dsa_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed bit length of an uploaded DSA key. Default is 0 (no restriction). -1 disables DSA keys.
+        The minimum allowed bit length of an uploaded DSA key. 0 means no restriction. -1 disables DSA keys.
         """
         return pulumi.get(self, "dsa_key_restriction")
 
     @property
     @pulumi.getter(name="ecdsaKeyRestriction")
     def ecdsa_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA key. Default is 0 (no restriction). -1 disables ECDSA keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA key. 0 means no restriction. -1 disables ECDSA keys.
         """
         return pulumi.get(self, "ecdsa_key_restriction")
 
     @property
     @pulumi.getter(name="ecdsaSkKeyRestriction")
     def ecdsa_sk_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. Default is 0 (no restriction). -1 disables ECDSA*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ECDSA*SK key. 0 means no restriction. -1 disables ECDSA*SK keys.
         """
         return pulumi.get(self, "ecdsa_sk_key_restriction")
 
     @property
     @pulumi.getter(name="ed25519KeyRestriction")
     def ed25519_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519 key. Default is 0 (no restriction). -1 disables ED25519 keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519 key. 0 means no restriction. -1 disables ED25519 keys.
         """
         return pulumi.get(self, "ed25519_key_restriction")
 
     @property
     @pulumi.getter(name="ed25519SkKeyRestriction")
     def ed25519_sk_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. Default is 0 (no restriction). -1 disables ED25519*SK keys.
+        The minimum allowed curve size (in bits) of an uploaded ED25519*SK key. 0 means no restriction. -1 disables ED25519*SK keys.
         """
         return pulumi.get(self, "ed25519_sk_key_restriction")
 
     @property
     @pulumi.getter(name="eksAccessKeyId")
     def eks_access_key_id(self) -> pulumi.Output[str]:
         """
@@ -10198,15 +10284,15 @@
         """
         return pulumi.get(self, "file_template_project_id")
 
     @property
     @pulumi.getter(name="firstDayOfWeek")
     def first_day_of_week(self) -> pulumi.Output[int]:
         """
-        Start day of the week for calendar views and date pickers. Valid values are 0 (default) for Sunday, 1 for Monday, and 6 for Saturday.
+        Start day of the week for calendar views and date pickers. Valid values are 0 for Sunday, 1 for Monday, and 6 for Saturday.
         """
         return pulumi.get(self, "first_day_of_week")
 
     @property
     @pulumi.getter(name="geoNodeAllowedIps")
     def geo_node_allowed_ips(self) -> pulumi.Output[str]:
         """
@@ -10222,15 +10308,15 @@
         """
         return pulumi.get(self, "geo_status_timeout")
 
     @property
     @pulumi.getter(name="gitRateLimitUsersAllowlists")
     def git_rate_limit_users_allowlists(self) -> pulumi.Output[Sequence[str]]:
         """
-        List of usernames excluded from Git anti-abuse rate limits. Default: [], Maximum: 100 usernames. Introduced in GitLab 15.2.
+        List of usernames excluded from Git anti-abuse rate limits. Maximum: 100 usernames. Introduced in GitLab 15.2.
         """
         return pulumi.get(self, "git_rate_limit_users_allowlists")
 
     @property
     @pulumi.getter(name="gitTwoFactorSessionExpiry")
     def git_two_factor_session_expiry(self) -> pulumi.Output[int]:
         """
@@ -10283,14 +10369,22 @@
     def gravatar_enabled(self) -> pulumi.Output[bool]:
         """
         Enable Gravatar.
         """
         return pulumi.get(self, "gravatar_enabled")
 
     @property
+    @pulumi.getter(name="groupOwnersCanManageDefaultBranchProtection")
+    def group_owners_can_manage_default_branch_protection(self) -> pulumi.Output[bool]:
+        """
+        Prevent overrides of default branch protection.
+        """
+        return pulumi.get(self, "group_owners_can_manage_default_branch_protection")
+
+    @property
     @pulumi.getter(name="hashedStorageEnabled")
     def hashed_storage_enabled(self) -> pulumi.Output[bool]:
         """
         Create new projects using hashed storage paths: Enable immutable, hash-based paths and repository names to store repositories on disk. This prevents repositories from having to be moved or renamed when the Project URL changes and may improve disk I/O performance. (Always enabled in GitLab versions 13.0 and later, configuration is scheduled for removal in 14.0).
         """
         return pulumi.get(self, "hashed_storage_enabled")
 
@@ -10390,63 +10484,63 @@
         """
         return pulumi.get(self, "import_sources")
 
     @property
     @pulumi.getter(name="inProductMarketingEmailsEnabled")
     def in_product_marketing_emails_enabled(self) -> pulumi.Output[bool]:
         """
-        Enable in-product marketing emails. Enabled by default.
+        Enable in-product marketing emails.
         """
         return pulumi.get(self, "in_product_marketing_emails_enabled")
 
     @property
     @pulumi.getter(name="inactiveProjectsDeleteAfterMonths")
     def inactive_projects_delete_after_months(self) -> pulumi.Output[int]:
         """
-        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Default is 2. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the time (in months) to wait before deleting inactive projects. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_delete_after_months")
 
     @property
     @pulumi.getter(name="inactiveProjectsMinSizeMb")
     def inactive_projects_min_size_mb(self) -> pulumi.Output[int]:
         """
-        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Default is 0. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, the minimum repository size for projects to be checked for inactivity. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_min_size_mb")
 
     @property
     @pulumi.getter(name="inactiveProjectsSendWarningEmailAfterMonths")
     def inactive_projects_send_warning_email_after_months(self) -> pulumi.Output[int]:
         """
-        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Default is 1. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
+        If delete*inactive*projects is true, sets the time (in months) to wait before emailing maintainers that the project is scheduled be deleted because it is inactive. Introduced in GitLab 14.10. Became operational in GitLab 15.0.
         """
         return pulumi.get(self, "inactive_projects_send_warning_email_after_months")
 
     @property
     @pulumi.getter(name="invisibleCaptchaEnabled")
     def invisible_captcha_enabled(self) -> pulumi.Output[bool]:
         """
-        Enable Invisible CAPTCHA spam detection during sign-up. Disabled by default.
+        Enable Invisible CAPTCHA spam detection during sign-up.
         """
         return pulumi.get(self, "invisible_captcha_enabled")
 
     @property
     @pulumi.getter(name="issuesCreateLimit")
     def issues_create_limit(self) -> pulumi.Output[int]:
         """
-        Max number of issue creation requests per minute per user. Disabled by default.
+        Max number of issue creation requests per minute per user.
         """
         return pulumi.get(self, "issues_create_limit")
 
     @property
     @pulumi.getter(name="keepLatestArtifact")
     def keep_latest_artifact(self) -> pulumi.Output[bool]:
         """
-        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time. Enabled by default.
+        Prevent the deletion of the artifacts from the most recent successful jobs, regardless of the expiry time.
         """
         return pulumi.get(self, "keep_latest_artifact")
 
     @property
     @pulumi.getter(name="localMarkdownVersion")
     def local_markdown_version(self) -> pulumi.Output[int]:
         """
@@ -10502,39 +10596,39 @@
         """
         return pulumi.get(self, "max_attachment_size")
 
     @property
     @pulumi.getter(name="maxExportSize")
     def max_export_size(self) -> pulumi.Output[int]:
         """
-        Maximum export size in MB. 0 for unlimited. Default = 0 (unlimited).
+        Maximum export size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_export_size")
 
     @property
     @pulumi.getter(name="maxImportSize")
     def max_import_size(self) -> pulumi.Output[int]:
         """
-        Maximum import size in MB. 0 for unlimited. Default = 0 (unlimited) Modified from 50MB to 0 in GitLab 13.8.
+        Maximum import size in MB. 0 for unlimited.
         """
         return pulumi.get(self, "max_import_size")
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloads")
     def max_number_of_repository_downloads(self) -> pulumi.Output[int]:
         """
-        Maximum number of unique repositories a user can download in the specified time period before they are banned. Default: 0, Maximum: 10,000 repositories. Introduced in GitLab 15.1.
+        Maximum number of unique repositories a user can download in the specified time period before they are banned. Maximum: 10,000 repositories. Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads")
 
     @property
     @pulumi.getter(name="maxNumberOfRepositoryDownloadsWithinTimePeriod")
     def max_number_of_repository_downloads_within_time_period(self) -> pulumi.Output[int]:
         """
-        Reporting time period (in seconds). Default: 0, Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
+        Reporting time period (in seconds). Maximum: 864000 seconds (10 days). Introduced in GitLab 15.1.
         """
         return pulumi.get(self, "max_number_of_repository_downloads_within_time_period")
 
     @property
     @pulumi.getter(name="maxPagesSize")
     def max_pages_size(self) -> pulumi.Output[int]:
         """
@@ -10630,23 +10724,23 @@
         """
         return pulumi.get(self, "pages_domain_verification_enabled")
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForGit")
     def password_authentication_enabled_for_git(self) -> pulumi.Output[bool]:
         """
-        Enable authentication for Git over HTTP(S) via a GitLab account password. Default is true.
+        Enable authentication for Git over HTTP(S) via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_git")
 
     @property
     @pulumi.getter(name="passwordAuthenticationEnabledForWeb")
     def password_authentication_enabled_for_web(self) -> pulumi.Output[bool]:
         """
-        Enable authentication for the web interface via a GitLab account password. Default is true.
+        Enable authentication for the web interface via a GitLab account password.
         """
         return pulumi.get(self, "password_authentication_enabled_for_web")
 
     @property
     @pulumi.getter(name="passwordLowercaseRequired")
     def password_lowercase_required(self) -> pulumi.Output[bool]:
         """
@@ -10694,23 +10788,23 @@
         """
         return pulumi.get(self, "personal_access_token_prefix")
 
     @property
     @pulumi.getter(name="pipelineLimitPerProjectUserSha")
     def pipeline_limit_per_project_user_sha(self) -> pulumi.Output[int]:
         """
-        Maximum number of pipeline creation requests per minute per user and commit. Disabled by default.
+        Maximum number of pipeline creation requests per minute per user and commit.
         """
         return pulumi.get(self, "pipeline_limit_per_project_user_sha")
 
     @property
     @pulumi.getter(name="plantumlEnabled")
     def plantuml_enabled(self) -> pulumi.Output[bool]:
         """
-        (If enabled, requires: plantuml_url) Enable PlantUML integration. Default is false.
+        (If enabled, requires: plantuml_url) Enable PlantUML integration.
         """
         return pulumi.get(self, "plantuml_enabled")
 
     @property
     @pulumi.getter(name="plantumlUrl")
     def plantuml_url(self) -> pulumi.Output[str]:
         """
@@ -10782,15 +10876,15 @@
         """
         return pulumi.get(self, "rate_limiting_response_text")
 
     @property
     @pulumi.getter(name="rawBlobRequestLimit")
     def raw_blob_request_limit(self) -> pulumi.Output[int]:
         """
-        Max number of requests per minute for each raw path. Default: 300. To disable throttling set to 0.
+        Max number of requests per minute for each raw path. To disable throttling set to 0.
         """
         return pulumi.get(self, "raw_blob_request_limit")
 
     @property
     @pulumi.getter(name="recaptchaEnabled")
     def recaptcha_enabled(self) -> pulumi.Output[bool]:
         """
@@ -10870,39 +10964,39 @@
         """
         return pulumi.get(self, "require_two_factor_authentication")
 
     @property
     @pulumi.getter(name="restrictedVisibilityLevels")
     def restricted_visibility_levels(self) -> pulumi.Output[Sequence[str]]:
         """
-        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Default is null which means there is no restriction.
+        Selected levels cannot be used by non-Administrator users for groups, projects or snippets. Can take private, internal and public as a parameter. Null means there is no restriction.
         """
         return pulumi.get(self, "restricted_visibility_levels")
 
     @property
     @pulumi.getter(name="rsaKeyRestriction")
     def rsa_key_restriction(self) -> pulumi.Output[int]:
         """
-        The minimum allowed bit length of an uploaded RSA key. Default is 0 (no restriction). -1 disables RSA keys.
+        The minimum allowed bit length of an uploaded RSA key. 0 means no restriction. -1 disables RSA keys.
         """
         return pulumi.get(self, "rsa_key_restriction")
 
     @property
     @pulumi.getter(name="searchRateLimit")
     def search_rate_limit(self) -> pulumi.Output[int]:
         """
-        Max number of requests per minute for performing a search while authenticated. Default: 30. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while authenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit")
 
     @property
     @pulumi.getter(name="searchRateLimitUnauthenticated")
     def search_rate_limit_unauthenticated(self) -> pulumi.Output[int]:
         """
-        Max number of requests per minute for performing a search while unauthenticated. Default: 10. To disable throttling set to 0.
+        Max number of requests per minute for performing a search while unauthenticated. To disable throttling set to 0.
         """
         return pulumi.get(self, "search_rate_limit_unauthenticated")
 
     @property
     @pulumi.getter(name="sendUserConfirmationEmail")
     def send_user_confirmation_email(self) -> pulumi.Output[bool]:
         """
@@ -10942,31 +11036,31 @@
         """
         return pulumi.get(self, "shared_runners_text")
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterCompressionThresholdBytes")
     def sidekiq_job_limiter_compression_threshold_bytes(self) -> pulumi.Output[int]:
         """
-        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis. Default: 100 000 bytes (100KB).
+        The threshold in bytes at which Sidekiq jobs are compressed before being stored in Redis.
         """
         return pulumi.get(self, "sidekiq_job_limiter_compression_threshold_bytes")
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterLimitBytes")
     def sidekiq_job_limiter_limit_bytes(self) -> pulumi.Output[int]:
         """
-        The threshold in bytes at which Sidekiq jobs are rejected. Default: 0 bytes (doesn’t reject any job).
+        The threshold in bytes at which Sidekiq jobs are rejected. 0 means do not reject any job.
         """
         return pulumi.get(self, "sidekiq_job_limiter_limit_bytes")
 
     @property
     @pulumi.getter(name="sidekiqJobLimiterMode")
     def sidekiq_job_limiter_mode(self) -> pulumi.Output[str]:
         """
-        track or compress. Sets the behavior for Sidekiq job size limits. Default: ‘compress’.
+        track or compress. Sets the behavior for Sidekiq job size limits.
         """
         return pulumi.get(self, "sidekiq_job_limiter_mode")
 
     @property
     @pulumi.getter(name="signInText")
     def sign_in_text(self) -> pulumi.Output[str]:
         """
@@ -10974,15 +11068,15 @@
         """
         return pulumi.get(self, "sign_in_text")
 
     @property
     @pulumi.getter(name="signupEnabled")
     def signup_enabled(self) -> pulumi.Output[bool]:
         """
-        Enable registration. Default is true.
+        Enable registration.
         """
         return pulumi.get(self, "signup_enabled")
 
     @property
     @pulumi.getter(name="slackAppEnabled")
     def slack_app_enabled(self) -> pulumi.Output[bool]:
         """
@@ -11022,15 +11116,15 @@
         """
         return pulumi.get(self, "slack_app_verification_token")
 
     @property
     @pulumi.getter(name="snippetSizeLimit")
     def snippet_size_limit(self) -> pulumi.Output[int]:
         """
-        Max snippet content size in bytes. Default: 52428800 Bytes (50MB).
+        Max snippet content size in bytes.
         """
         return pulumi.get(self, "snippet_size_limit")
 
     @property
     @pulumi.getter(name="snowplowAppId")
     def snowplow_app_id(self) -> pulumi.Output[str]:
         """
@@ -11062,23 +11156,23 @@
         """
         return pulumi.get(self, "snowplow_enabled")
 
     @property
     @pulumi.getter(name="sourcegraphEnabled")
     def sourcegraph_enabled(self) -> pulumi.Output[bool]:
         """
-        Enables Sourcegraph integration. Default is false. If enabled, requires sourcegraph_url.
+        Enables Sourcegraph integration. If enabled, requires sourcegraph_url.
         """
         return pulumi.get(self, "sourcegraph_enabled")
 
     @property
     @pulumi.getter(name="sourcegraphPublicOnly")
     def sourcegraph_public_only(self) -> pulumi.Output[bool]:
         """
-        Blocks Sourcegraph from being loaded on private and internal projects. Default is true.
+        Blocks Sourcegraph from being loaded on private and internal projects.
         """
         return pulumi.get(self, "sourcegraph_public_only")
 
     @property
     @pulumi.getter(name="sourcegraphUrl")
     def sourcegraph_url(self) -> pulumi.Output[str]:
         """
@@ -11094,15 +11188,15 @@
         """
         return pulumi.get(self, "spam_check_api_key")
 
     @property
     @pulumi.getter(name="spamCheckEndpointEnabled")
     def spam_check_endpoint_enabled(self) -> pulumi.Output[bool]:
         """
-        Enables spam checking using external Spam Check API endpoint. Default is false.
+        Enables spam checking using external Spam Check API endpoint.
         """
         return pulumi.get(self, "spam_check_endpoint_enabled")
 
     @property
     @pulumi.getter(name="spamCheckEndpointUrl")
     def spam_check_endpoint_url(self) -> pulumi.Output[str]:
         """
@@ -11278,15 +11372,15 @@
         """
         return pulumi.get(self, "throttle_unauthenticated_web_requests_per_period")
 
     @property
     @pulumi.getter(name="timeTrackingLimitToHours")
     def time_tracking_limit_to_hours(self) -> pulumi.Output[bool]:
         """
-        Limit display of time tracking units to hours. Default is false.
+        Limit display of time tracking units to hours.
         """
         return pulumi.get(self, "time_tracking_limit_to_hours")
 
     @property
     @pulumi.getter(name="twoFactorGracePeriod")
     def two_factor_grace_period(self) -> pulumi.Output[int]:
         """
@@ -11390,11 +11484,11 @@
         """
         return pulumi.get(self, "whats_new_variant")
 
     @property
     @pulumi.getter(name="wikiPageMaxContentBytes")
     def wiki_page_max_content_bytes(self) -> pulumi.Output[int]:
         """
-        Maximum wiki page content size in bytes. Default: 52428800 Bytes (50 MB). The minimum value is 1024 bytes.
+        Maximum wiki page content size in bytes. The minimum value is 1024 bytes.
         """
         return pulumi.get(self, "wiki_page_max_content_bytes")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
         example_branch = gitlab.Branch("exampleBranch",
             ref="main",
             project=example_project.id)
         ```
 
         ## Import
 
-        Gitlab protected branches can be imported with a key composed of `<project_id>:<branch_name>`, e.g.
+        Gitlab branches can be imported with a key composed of `<project_id>:<branch_name>`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/branch:Branch example "12345:develop"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -318,15 +318,15 @@
         example_branch = gitlab.Branch("exampleBranch",
             ref="main",
             project=example_project.id)
         ```
 
         ## Import
 
-        Gitlab protected branches can be imported with a key composed of `<project_id>:<branch_name>`, e.g.
+        Gitlab branches can be imported with a key composed of `<project_id>:<branch_name>`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/branch:Branch example "12345:develop"
         ```
 
         :param str resource_name: The name of the resource.
         :param BranchArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/branch_protection.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
         The set of arguments for constructing a BranchProtection resource.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToMergeArgs']]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToPushArgs']]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
-        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging.
+        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         pulumi.set(__self__, "branch", branch)
         pulumi.set(__self__, "project", project)
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
@@ -130,15 +130,15 @@
     def allowed_to_unprotects(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]]]):
         pulumi.set(self, "allowed_to_unprotects", value)
 
     @property
     @pulumi.getter(name="codeOwnerApprovalRequired")
     def code_owner_approval_required(self) -> Optional[pulumi.Input[bool]]:
         """
-        Can be set to true to require code owner approval before merging.
+        Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         """
         return pulumi.get(self, "code_owner_approval_required")
 
     @code_owner_approval_required.setter
     def code_owner_approval_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "code_owner_approval_required", value)
 
@@ -166,15 +166,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -197,19 +197,19 @@
         Input properties used for looking up and filtering BranchProtection resources.
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToMergeArgs']]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToPushArgs']]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
-        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging.
+        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
         if allowed_to_pushes is not None:
             pulumi.set(__self__, "allowed_to_pushes", allowed_to_pushes)
@@ -302,15 +302,15 @@
     def branch_protection_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "branch_protection_id", value)
 
     @property
     @pulumi.getter(name="codeOwnerApprovalRequired")
     def code_owner_approval_required(self) -> Optional[pulumi.Input[bool]]:
         """
-        Can be set to true to require code owner approval before merging.
+        Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         """
         return pulumi.get(self, "code_owner_approval_required")
 
     @code_owner_approval_required.setter
     def code_owner_approval_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "code_owner_approval_required", value)
 
@@ -350,15 +350,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -391,19 +391,19 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToMergeArgs']]]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToPushArgs']]]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
-        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging.
+        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BranchProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -495,19 +495,19 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToMergeArgs']]]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToPushArgs']]]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
-        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging.
+        :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BranchProtectionState.__new__(_BranchProtectionState)
 
         __props__.__dict__["allow_force_push"] = allow_force_push
         __props__.__dict__["allowed_to_merges"] = allowed_to_merges
@@ -570,15 +570,15 @@
         """
         return pulumi.get(self, "branch_protection_id")
 
     @property
     @pulumi.getter(name="codeOwnerApprovalRequired")
     def code_owner_approval_required(self) -> pulumi.Output[Optional[bool]]:
         """
-        Can be set to true to require code owner approval before merging.
+        Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         """
         return pulumi.get(self, "code_owner_approval_required")
 
     @property
     @pulumi.getter(name="mergeAccessLevel")
     def merge_access_level(self) -> pulumi.Output[Optional[str]]:
         """
@@ -602,11 +602,11 @@
         """
         return pulumi.get(self, "push_access_level")
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> pulumi.Output[Optional[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/config/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,18 @@
         """
         return __config__.get('clientKey')
 
     @property
     def early_auth_check(self) -> Optional[bool]:
         """
         (Experimental) By default the provider does a dummy request to get the current user in order to verify that the provider
-        configuration is correct and the GitLab API is reachable. Turn it off, to skip this check. This may be useful if the
-        GitLab instance does not yet exist and is created within the same terraform module. This is an experimental feature and
-        may change in the future. Please make sure to always keep backups of your state.
+        configuration is correct and the GitLab API is reachable. Set this to `false` to skip this check. This may be useful if
+        the GitLab instance does not yet exist and is created within the same terraform module. It may be sourced from the
+        `GITLAB_EARLY_AUTH_CHECK`. This is an experimental feature and may change in the future. Please make sure to always keep
+        backups of your state.
         """
         return __config__.get_bool('earlyAuthCheck')
 
     @property
     def insecure(self) -> Optional[bool]:
         """
         When set to true this disables SSL verification of the connection to the GitLab instance.
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example = gitlab.DeployKey("example",
-            key="ssh-rsa AAAA...",
+            key="ssh-ed25519 AAAA...",
             project="example/deploying",
             title="Example deploy key")
         ```
 
         ## Import
 
         GitLab deploy keys can be imported using an id made up of `{project_id}:{deploy_key_id}`, e.g. `project_id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
@@ -216,15 +216,15 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example = gitlab.DeployKey("example",
-            key="ssh-rsa AAAA...",
+            key="ssh-ed25519 AAAA...",
             project="example/deploying",
             title="Example deploy key")
         ```
 
         ## Import
 
         GitLab deploy keys can be imported using an id made up of `{project_id}:{deploy_key_id}`, e.g. `project_id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_key_enable.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         parent_project = gitlab.Project("parentProject")
         # A second repo to use the deployment key from the parent project
         foo_project = gitlab.Project("fooProject")
         # Upload a deployment key for the parent repo
         parent_deploy_key = gitlab.DeployKey("parentDeployKey",
             project=parent_project.id,
             title="Example deploy key",
-            key="ssh-rsa AAAA...")
+            key="ssh-ed25519 AAAA...")
         # Enable the deployment key on the second repo
         foo_deploy_key_enable = gitlab.DeployKeyEnable("fooDeployKeyEnable",
             project=foo_project.id,
             key_id=parent_deploy_key.id)
         ```
 
         ## Import
@@ -263,15 +263,15 @@
         parent_project = gitlab.Project("parentProject")
         # A second repo to use the deployment key from the parent project
         foo_project = gitlab.Project("fooProject")
         # Upload a deployment key for the parent repo
         parent_deploy_key = gitlab.DeployKey("parentDeployKey",
             project=parent_project.id,
             title="Example deploy key",
-            key="ssh-rsa AAAA...")
+            key="ssh-ed25519 AAAA...")
         # Enable the deployment key on the second repo
         foo_deploy_key_enable = gitlab.DeployKeyEnable("fooDeployKeyEnable",
             project=foo_project.id,
             key_id=parent_deploy_key.id)
         ```
 
         ## Import
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/deploy_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_cluster_agents.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_current_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,23 @@
 
 
 def get_current_user(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCurrentUserResult:
     """
     The `get_current_user` data source allows details of the current user (determined by `token` provider attribute) to be retrieved.
 
     **Upstream API**: [GitLab GraphQL API docs](https://docs.gitlab.com/ee/api/graphql/reference/index.html#querycurrentuser)
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_gitlab as gitlab
+
+    example = gitlab.get_current_user()
+    ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getCurrentUser:getCurrentUser', __args__, opts=opts, typ=GetCurrentUserResult).value
 
     return AwaitableGetCurrentUserResult(
         bot=__ret__.bot,
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_repository_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,277 +6,260 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
-    'GetGroupResult',
-    'AwaitableGetGroupResult',
-    'get_group',
-    'get_group_output',
+    'GetRepositoryFileResult',
+    'AwaitableGetRepositoryFileResult',
+    'get_repository_file',
+    'get_repository_file_output',
 ]
 
 @pulumi.output_type
-class GetGroupResult:
+class GetRepositoryFileResult:
     """
-    A collection of values returned by getGroup.
+    A collection of values returned by getRepositoryFile.
     """
-    def __init__(__self__, default_branch_protection=None, description=None, full_name=None, full_path=None, group_id=None, id=None, lfs_enabled=None, name=None, parent_id=None, path=None, prevent_forking_outside_group=None, request_access_enabled=None, runners_token=None, visibility_level=None, web_url=None):
-        if default_branch_protection and not isinstance(default_branch_protection, int):
-            raise TypeError("Expected argument 'default_branch_protection' to be a int")
-        pulumi.set(__self__, "default_branch_protection", default_branch_protection)
-        if description and not isinstance(description, str):
-            raise TypeError("Expected argument 'description' to be a str")
-        pulumi.set(__self__, "description", description)
-        if full_name and not isinstance(full_name, str):
-            raise TypeError("Expected argument 'full_name' to be a str")
-        pulumi.set(__self__, "full_name", full_name)
-        if full_path and not isinstance(full_path, str):
-            raise TypeError("Expected argument 'full_path' to be a str")
-        pulumi.set(__self__, "full_path", full_path)
-        if group_id and not isinstance(group_id, int):
-            raise TypeError("Expected argument 'group_id' to be a int")
-        pulumi.set(__self__, "group_id", group_id)
+    def __init__(__self__, blob_id=None, commit_id=None, content=None, content_sha256=None, encoding=None, execute_filemode=None, file_name=None, file_path=None, id=None, last_commit_id=None, project=None, ref=None, size=None):
+        if blob_id and not isinstance(blob_id, str):
+            raise TypeError("Expected argument 'blob_id' to be a str")
+        pulumi.set(__self__, "blob_id", blob_id)
+        if commit_id and not isinstance(commit_id, str):
+            raise TypeError("Expected argument 'commit_id' to be a str")
+        pulumi.set(__self__, "commit_id", commit_id)
+        if content and not isinstance(content, str):
+            raise TypeError("Expected argument 'content' to be a str")
+        pulumi.set(__self__, "content", content)
+        if content_sha256 and not isinstance(content_sha256, str):
+            raise TypeError("Expected argument 'content_sha256' to be a str")
+        pulumi.set(__self__, "content_sha256", content_sha256)
+        if encoding and not isinstance(encoding, str):
+            raise TypeError("Expected argument 'encoding' to be a str")
+        pulumi.set(__self__, "encoding", encoding)
+        if execute_filemode and not isinstance(execute_filemode, bool):
+            raise TypeError("Expected argument 'execute_filemode' to be a bool")
+        pulumi.set(__self__, "execute_filemode", execute_filemode)
+        if file_name and not isinstance(file_name, str):
+            raise TypeError("Expected argument 'file_name' to be a str")
+        pulumi.set(__self__, "file_name", file_name)
+        if file_path and not isinstance(file_path, str):
+            raise TypeError("Expected argument 'file_path' to be a str")
+        pulumi.set(__self__, "file_path", file_path)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
-        if lfs_enabled and not isinstance(lfs_enabled, bool):
-            raise TypeError("Expected argument 'lfs_enabled' to be a bool")
-        pulumi.set(__self__, "lfs_enabled", lfs_enabled)
-        if name and not isinstance(name, str):
-            raise TypeError("Expected argument 'name' to be a str")
-        pulumi.set(__self__, "name", name)
-        if parent_id and not isinstance(parent_id, int):
-            raise TypeError("Expected argument 'parent_id' to be a int")
-        pulumi.set(__self__, "parent_id", parent_id)
-        if path and not isinstance(path, str):
-            raise TypeError("Expected argument 'path' to be a str")
-        pulumi.set(__self__, "path", path)
-        if prevent_forking_outside_group and not isinstance(prevent_forking_outside_group, bool):
-            raise TypeError("Expected argument 'prevent_forking_outside_group' to be a bool")
-        pulumi.set(__self__, "prevent_forking_outside_group", prevent_forking_outside_group)
-        if request_access_enabled and not isinstance(request_access_enabled, bool):
-            raise TypeError("Expected argument 'request_access_enabled' to be a bool")
-        pulumi.set(__self__, "request_access_enabled", request_access_enabled)
-        if runners_token and not isinstance(runners_token, str):
-            raise TypeError("Expected argument 'runners_token' to be a str")
-        pulumi.set(__self__, "runners_token", runners_token)
-        if visibility_level and not isinstance(visibility_level, str):
-            raise TypeError("Expected argument 'visibility_level' to be a str")
-        pulumi.set(__self__, "visibility_level", visibility_level)
-        if web_url and not isinstance(web_url, str):
-            raise TypeError("Expected argument 'web_url' to be a str")
-        pulumi.set(__self__, "web_url", web_url)
+        if last_commit_id and not isinstance(last_commit_id, str):
+            raise TypeError("Expected argument 'last_commit_id' to be a str")
+        pulumi.set(__self__, "last_commit_id", last_commit_id)
+        if project and not isinstance(project, str):
+            raise TypeError("Expected argument 'project' to be a str")
+        pulumi.set(__self__, "project", project)
+        if ref and not isinstance(ref, str):
+            raise TypeError("Expected argument 'ref' to be a str")
+        pulumi.set(__self__, "ref", ref)
+        if size and not isinstance(size, int):
+            raise TypeError("Expected argument 'size' to be a int")
+        pulumi.set(__self__, "size", size)
 
     @property
-    @pulumi.getter(name="defaultBranchProtection")
-    def default_branch_protection(self) -> int:
+    @pulumi.getter(name="blobId")
+    def blob_id(self) -> str:
         """
-        Whether developers and maintainers can push to the applicable default branch.
+        The blob id.
         """
-        return pulumi.get(self, "default_branch_protection")
+        return pulumi.get(self, "blob_id")
 
     @property
-    @pulumi.getter
-    def description(self) -> str:
-        """
-        The description of the group.
-        """
-        return pulumi.get(self, "description")
-
-    @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> str:
+    @pulumi.getter(name="commitId")
+    def commit_id(self) -> str:
         """
-        The full name of the group.
+        The commit id.
         """
-        return pulumi.get(self, "full_name")
+        return pulumi.get(self, "commit_id")
 
     @property
-    @pulumi.getter(name="fullPath")
-    def full_path(self) -> str:
+    @pulumi.getter
+    def content(self) -> str:
         """
-        The full path of the group.
+        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
         """
-        return pulumi.get(self, "full_path")
+        return pulumi.get(self, "content")
 
     @property
-    @pulumi.getter(name="groupId")
-    def group_id(self) -> int:
+    @pulumi.getter(name="contentSha256")
+    def content_sha256(self) -> str:
         """
-        The ID of the group.
+        File content sha256 digest.
         """
-        return pulumi.get(self, "group_id")
+        return pulumi.get(self, "content_sha256")
 
     @property
     @pulumi.getter
-    def id(self) -> str:
+    def encoding(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        The file content encoding.
         """
-        return pulumi.get(self, "id")
+        return pulumi.get(self, "encoding")
 
     @property
-    @pulumi.getter(name="lfsEnabled")
-    def lfs_enabled(self) -> bool:
+    @pulumi.getter(name="executeFilemode")
+    def execute_filemode(self) -> bool:
         """
-        Boolean, is LFS enabled for projects in this group.
+        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         """
-        return pulumi.get(self, "lfs_enabled")
+        return pulumi.get(self, "execute_filemode")
 
     @property
-    @pulumi.getter
-    def name(self) -> str:
+    @pulumi.getter(name="fileName")
+    def file_name(self) -> str:
         """
-        The name of this group.
+        The filename.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "file_name")
 
     @property
-    @pulumi.getter(name="parentId")
-    def parent_id(self) -> int:
+    @pulumi.getter(name="filePath")
+    def file_path(self) -> str:
         """
-        Integer, ID of the parent group.
+        The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         """
-        return pulumi.get(self, "parent_id")
+        return pulumi.get(self, "file_path")
 
     @property
     @pulumi.getter
-    def path(self) -> str:
-        """
-        The path of the group.
-        """
-        return pulumi.get(self, "path")
-
-    @property
-    @pulumi.getter(name="preventForkingOutsideGroup")
-    def prevent_forking_outside_group(self) -> bool:
+    def id(self) -> str:
         """
-        When enabled, users can not fork projects from this group to external namespaces.
+        The provider-assigned unique ID for this managed resource.
         """
-        return pulumi.get(self, "prevent_forking_outside_group")
+        return pulumi.get(self, "id")
 
     @property
-    @pulumi.getter(name="requestAccessEnabled")
-    def request_access_enabled(self) -> bool:
+    @pulumi.getter(name="lastCommitId")
+    def last_commit_id(self) -> str:
         """
-        Boolean, is request for access enabled to the group.
+        The last known commit id.
         """
-        return pulumi.get(self, "request_access_enabled")
+        return pulumi.get(self, "last_commit_id")
 
     @property
-    @pulumi.getter(name="runnersToken")
-    def runners_token(self) -> str:
+    @pulumi.getter
+    def project(self) -> str:
         """
-        The group level registration token to use during runner setup.
+        The name or ID of the project.
         """
-        return pulumi.get(self, "runners_token")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter(name="visibilityLevel")
-    def visibility_level(self) -> str:
+    @pulumi.getter
+    def ref(self) -> str:
         """
-        Visibility level of the group. Possible values are `private`, `internal`, `public`.
+        The name of branch, tag or commit.
         """
-        return pulumi.get(self, "visibility_level")
+        return pulumi.get(self, "ref")
 
     @property
-    @pulumi.getter(name="webUrl")
-    def web_url(self) -> str:
+    @pulumi.getter
+    def size(self) -> int:
         """
-        Web URL of the group.
+        The file size.
         """
-        return pulumi.get(self, "web_url")
+        return pulumi.get(self, "size")
 
 
-class AwaitableGetGroupResult(GetGroupResult):
+class AwaitableGetRepositoryFileResult(GetRepositoryFileResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
-        return GetGroupResult(
-            default_branch_protection=self.default_branch_protection,
-            description=self.description,
-            full_name=self.full_name,
-            full_path=self.full_path,
-            group_id=self.group_id,
+        return GetRepositoryFileResult(
+            blob_id=self.blob_id,
+            commit_id=self.commit_id,
+            content=self.content,
+            content_sha256=self.content_sha256,
+            encoding=self.encoding,
+            execute_filemode=self.execute_filemode,
+            file_name=self.file_name,
+            file_path=self.file_path,
             id=self.id,
-            lfs_enabled=self.lfs_enabled,
-            name=self.name,
-            parent_id=self.parent_id,
-            path=self.path,
-            prevent_forking_outside_group=self.prevent_forking_outside_group,
-            request_access_enabled=self.request_access_enabled,
-            runners_token=self.runners_token,
-            visibility_level=self.visibility_level,
-            web_url=self.web_url)
+            last_commit_id=self.last_commit_id,
+            project=self.project,
+            ref=self.ref,
+            size=self.size)
 
 
-def get_group(full_path: Optional[str] = None,
-              group_id: Optional[int] = None,
-              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupResult:
+def get_repository_file(file_path: Optional[str] = None,
+                        project: Optional[str] = None,
+                        ref: Optional[str] = None,
+                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRepositoryFileResult:
     """
-    The `Group` data source allows details of a group to be retrieved by its id or full path.
+    The `RepositoryFile` data source allows details of a file in a repository to be retrieved.
 
-    **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#details-of-a-group)
+    **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/repository_files.html)
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    foo = gitlab.get_group(full_path="foo/bar")
+    example = gitlab.get_repository_file(file_path="README.md",
+        project="example",
+        ref="main")
     ```
 
 
-    :param str full_path: The full path of the group.
-    :param int group_id: The ID of the group.
+    :param str file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+    :param str project: The name or ID of the project.
+    :param str ref: The name of branch, tag or commit.
     """
     __args__ = dict()
-    __args__['fullPath'] = full_path
-    __args__['groupId'] = group_id
+    __args__['filePath'] = file_path
+    __args__['project'] = project
+    __args__['ref'] = ref
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
-    __ret__ = pulumi.runtime.invoke('gitlab:index/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
+    __ret__ = pulumi.runtime.invoke('gitlab:index/getRepositoryFile:getRepositoryFile', __args__, opts=opts, typ=GetRepositoryFileResult).value
 
-    return AwaitableGetGroupResult(
-        default_branch_protection=__ret__.default_branch_protection,
-        description=__ret__.description,
-        full_name=__ret__.full_name,
-        full_path=__ret__.full_path,
-        group_id=__ret__.group_id,
+    return AwaitableGetRepositoryFileResult(
+        blob_id=__ret__.blob_id,
+        commit_id=__ret__.commit_id,
+        content=__ret__.content,
+        content_sha256=__ret__.content_sha256,
+        encoding=__ret__.encoding,
+        execute_filemode=__ret__.execute_filemode,
+        file_name=__ret__.file_name,
+        file_path=__ret__.file_path,
         id=__ret__.id,
-        lfs_enabled=__ret__.lfs_enabled,
-        name=__ret__.name,
-        parent_id=__ret__.parent_id,
-        path=__ret__.path,
-        prevent_forking_outside_group=__ret__.prevent_forking_outside_group,
-        request_access_enabled=__ret__.request_access_enabled,
-        runners_token=__ret__.runners_token,
-        visibility_level=__ret__.visibility_level,
-        web_url=__ret__.web_url)
+        last_commit_id=__ret__.last_commit_id,
+        project=__ret__.project,
+        ref=__ret__.ref,
+        size=__ret__.size)
 
 
-@_utilities.lift_output_func(get_group)
-def get_group_output(full_path: Optional[pulumi.Input[Optional[str]]] = None,
-                     group_id: Optional[pulumi.Input[Optional[int]]] = None,
-                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
+@_utilities.lift_output_func(get_repository_file)
+def get_repository_file_output(file_path: Optional[pulumi.Input[str]] = None,
+                               project: Optional[pulumi.Input[str]] = None,
+                               ref: Optional[pulumi.Input[str]] = None,
+                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryFileResult]:
     """
-    The `Group` data source allows details of a group to be retrieved by its id or full path.
+    The `RepositoryFile` data source allows details of a file in a repository to be retrieved.
 
-    **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#details-of-a-group)
+    **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/repository_files.html)
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    foo = gitlab.get_group(full_path="foo/bar")
+    example = gitlab.get_repository_file(file_path="README.md",
+        project="example",
+        ref="main")
     ```
 
 
-    :param str full_path: The full path of the group.
-    :param int group_id: The ID of the group.
+    :param str file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+    :param str project: The name or ID of the project.
+    :param str ref: The name of branch, tag or commit.
     """
     ...
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,30 @@
 ]
 
 @pulumi.output_type
 class GetGroupMembershipResult:
     """
     A collection of values returned by getGroupMembership.
     """
-    def __init__(__self__, access_level=None, full_path=None, group_id=None, id=None, members=None):
+    def __init__(__self__, access_level=None, full_path=None, group_id=None, id=None, inherited=None, members=None):
         if access_level and not isinstance(access_level, str):
             raise TypeError("Expected argument 'access_level' to be a str")
         pulumi.set(__self__, "access_level", access_level)
         if full_path and not isinstance(full_path, str):
             raise TypeError("Expected argument 'full_path' to be a str")
         pulumi.set(__self__, "full_path", full_path)
         if group_id and not isinstance(group_id, int):
             raise TypeError("Expected argument 'group_id' to be a int")
         pulumi.set(__self__, "group_id", group_id)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if inherited and not isinstance(inherited, bool):
+            raise TypeError("Expected argument 'inherited' to be a bool")
+        pulumi.set(__self__, "inherited", inherited)
         if members and not isinstance(members, list):
             raise TypeError("Expected argument 'members' to be a list")
         pulumi.set(__self__, "members", members)
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> str:
@@ -69,14 +72,22 @@
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
+    def inherited(self) -> Optional[bool]:
+        """
+        Return all project members including members through ancestor groups.
+        """
+        return pulumi.get(self, "inherited")
+
+    @property
+    @pulumi.getter
     def members(self) -> Sequence['outputs.GetGroupMembershipMemberResult']:
         """
         The list of group members.
         """
         return pulumi.get(self, "members")
 
 
@@ -86,20 +97,22 @@
         if False:
             yield self
         return GetGroupMembershipResult(
             access_level=self.access_level,
             full_path=self.full_path,
             group_id=self.group_id,
             id=self.id,
+            inherited=self.inherited,
             members=self.members)
 
 
 def get_group_membership(access_level: Optional[str] = None,
                          full_path: Optional[str] = None,
                          group_id: Optional[int] = None,
+                         inherited: Optional[bool] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGroupMembershipResult:
     """
     The `GroupMembership` data source allows to list and filter all members of a group specified by either its id or full path.
 
     **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html#list-all-members-of-a-group-or-project)
 
     ## Example Usage
@@ -111,34 +124,38 @@
     example = gitlab.get_group_membership(full_path="foo/bar")
     ```
 
 
     :param str access_level: Only return members with the desired access level. Acceptable values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
     :param str full_path: The full path of the group.
     :param int group_id: The ID of the group.
+    :param bool inherited: Return all project members including members through ancestor groups.
     """
     __args__ = dict()
     __args__['accessLevel'] = access_level
     __args__['fullPath'] = full_path
     __args__['groupId'] = group_id
+    __args__['inherited'] = inherited
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupMembership:getGroupMembership', __args__, opts=opts, typ=GetGroupMembershipResult).value
 
     return AwaitableGetGroupMembershipResult(
         access_level=__ret__.access_level,
         full_path=__ret__.full_path,
         group_id=__ret__.group_id,
         id=__ret__.id,
+        inherited=__ret__.inherited,
         members=__ret__.members)
 
 
 @_utilities.lift_output_func(get_group_membership)
 def get_group_membership_output(access_level: Optional[pulumi.Input[Optional[str]]] = None,
                                 full_path: Optional[pulumi.Input[Optional[str]]] = None,
                                 group_id: Optional[pulumi.Input[Optional[int]]] = None,
+                                inherited: Optional[pulumi.Input[Optional[bool]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupMembershipResult]:
     """
     The `GroupMembership` data source allows to list and filter all members of a group specified by either its id or full path.
 
     **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html#list-all-members-of-a-group-or-project)
 
     ## Example Usage
@@ -150,9 +167,10 @@
     example = gitlab.get_group_membership(full_path="foo/bar")
     ```
 
 
     :param str access_level: Only return members with the desired access level. Acceptable values are: `guest`, `reporter`, `developer`, `maintainer`, `owner`.
     :param str full_path: The full path of the group.
     :param int group_id: The ID of the group.
+    :param bool inherited: Return all project members including members through ancestor groups.
     """
     ...
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_group_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_instance_variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 
 
 def get_instance_variables(opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstanceVariablesResult:
     """
     The `get_instance_variables` data source allows to retrieve all instance-level CI/CD variables.
 
     **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/instance_level_ci_variables.html)
+
+    ## Example Usage
+
+    ```python
+    import pulumi
+    import pulumi_gitlab as gitlab
+
+    vars = gitlab.get_instance_variables()
+    ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getInstanceVariables:getInstanceVariables', __args__, opts=opts, typ=GetInstanceVariablesResult).value
 
     return AwaitableGetInstanceVariablesResult(
         id=__ret__.id,
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetProjectResult:
     """
     A collection of values returned by getProject.
     """
-    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, external_authorization_classification_label=None, forking_access_level=None, http_url_to_repo=None, id=None, issues_access_level=None, issues_enabled=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, name=None, namespace_id=None, operations_access_level=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, runners_token=None, security_and_compliance_access_level=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
+    def __init__(__self__, analytics_access_level=None, archived=None, auto_cancel_pending_pipelines=None, auto_devops_deploy_strategy=None, auto_devops_enabled=None, autoclose_referenced_issues=None, build_git_strategy=None, build_timeout=None, builds_access_level=None, ci_config_path=None, ci_default_git_depth=None, ci_separated_caches=None, container_expiration_policies=None, container_registry_access_level=None, default_branch=None, description=None, emails_disabled=None, environments_access_level=None, external_authorization_classification_label=None, feature_flags_access_level=None, forking_access_level=None, http_url_to_repo=None, id=None, import_url=None, infrastructure_access_level=None, issues_access_level=None, issues_enabled=None, keep_latest_artifact=None, lfs_enabled=None, merge_commit_template=None, merge_pipelines_enabled=None, merge_requests_access_level=None, merge_requests_enabled=None, merge_trains_enabled=None, monitor_access_level=None, name=None, namespace_id=None, operations_access_level=None, path=None, path_with_namespace=None, pipelines_enabled=None, printing_merge_request_link_enabled=None, public_builds=None, push_rules=None, releases_access_level=None, remove_source_branch_after_merge=None, repository_access_level=None, repository_storage=None, request_access_enabled=None, requirements_access_level=None, resolve_outdated_diff_discussions=None, restrict_user_defined_variables=None, runners_token=None, security_and_compliance_access_level=None, snippets_access_level=None, snippets_enabled=None, squash_commit_template=None, ssh_url_to_repo=None, suggestion_commit_message=None, topics=None, visibility_level=None, web_url=None, wiki_access_level=None, wiki_enabled=None):
         if analytics_access_level and not isinstance(analytics_access_level, str):
             raise TypeError("Expected argument 'analytics_access_level' to be a str")
         pulumi.set(__self__, "analytics_access_level", analytics_access_level)
         if archived and not isinstance(archived, bool):
             raise TypeError("Expected argument 'archived' to be a bool")
         pulumi.set(__self__, "archived", archived)
         if auto_cancel_pending_pipelines and not isinstance(auto_cancel_pending_pipelines, str):
@@ -52,14 +52,17 @@
         pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path and not isinstance(ci_config_path, str):
             raise TypeError("Expected argument 'ci_config_path' to be a str")
         pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth and not isinstance(ci_default_git_depth, int):
             raise TypeError("Expected argument 'ci_default_git_depth' to be a int")
         pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
+        if ci_separated_caches and not isinstance(ci_separated_caches, bool):
+            raise TypeError("Expected argument 'ci_separated_caches' to be a bool")
+        pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policies and not isinstance(container_expiration_policies, list):
             raise TypeError("Expected argument 'container_expiration_policies' to be a list")
         pulumi.set(__self__, "container_expiration_policies", container_expiration_policies)
         if container_registry_access_level and not isinstance(container_registry_access_level, str):
             raise TypeError("Expected argument 'container_registry_access_level' to be a str")
         pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         if default_branch and not isinstance(default_branch, str):
@@ -67,32 +70,47 @@
         pulumi.set(__self__, "default_branch", default_branch)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
         if emails_disabled and not isinstance(emails_disabled, bool):
             raise TypeError("Expected argument 'emails_disabled' to be a bool")
         pulumi.set(__self__, "emails_disabled", emails_disabled)
+        if environments_access_level and not isinstance(environments_access_level, str):
+            raise TypeError("Expected argument 'environments_access_level' to be a str")
+        pulumi.set(__self__, "environments_access_level", environments_access_level)
         if external_authorization_classification_label and not isinstance(external_authorization_classification_label, str):
             raise TypeError("Expected argument 'external_authorization_classification_label' to be a str")
         pulumi.set(__self__, "external_authorization_classification_label", external_authorization_classification_label)
+        if feature_flags_access_level and not isinstance(feature_flags_access_level, str):
+            raise TypeError("Expected argument 'feature_flags_access_level' to be a str")
+        pulumi.set(__self__, "feature_flags_access_level", feature_flags_access_level)
         if forking_access_level and not isinstance(forking_access_level, str):
             raise TypeError("Expected argument 'forking_access_level' to be a str")
         pulumi.set(__self__, "forking_access_level", forking_access_level)
         if http_url_to_repo and not isinstance(http_url_to_repo, str):
             raise TypeError("Expected argument 'http_url_to_repo' to be a str")
         pulumi.set(__self__, "http_url_to_repo", http_url_to_repo)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if import_url and not isinstance(import_url, str):
+            raise TypeError("Expected argument 'import_url' to be a str")
+        pulumi.set(__self__, "import_url", import_url)
+        if infrastructure_access_level and not isinstance(infrastructure_access_level, str):
+            raise TypeError("Expected argument 'infrastructure_access_level' to be a str")
+        pulumi.set(__self__, "infrastructure_access_level", infrastructure_access_level)
         if issues_access_level and not isinstance(issues_access_level, str):
             raise TypeError("Expected argument 'issues_access_level' to be a str")
         pulumi.set(__self__, "issues_access_level", issues_access_level)
         if issues_enabled and not isinstance(issues_enabled, bool):
             raise TypeError("Expected argument 'issues_enabled' to be a bool")
         pulumi.set(__self__, "issues_enabled", issues_enabled)
+        if keep_latest_artifact and not isinstance(keep_latest_artifact, bool):
+            raise TypeError("Expected argument 'keep_latest_artifact' to be a bool")
+        pulumi.set(__self__, "keep_latest_artifact", keep_latest_artifact)
         if lfs_enabled and not isinstance(lfs_enabled, bool):
             raise TypeError("Expected argument 'lfs_enabled' to be a bool")
         pulumi.set(__self__, "lfs_enabled", lfs_enabled)
         if merge_commit_template and not isinstance(merge_commit_template, str):
             raise TypeError("Expected argument 'merge_commit_template' to be a str")
         pulumi.set(__self__, "merge_commit_template", merge_commit_template)
         if merge_pipelines_enabled and not isinstance(merge_pipelines_enabled, bool):
@@ -103,14 +121,17 @@
         pulumi.set(__self__, "merge_requests_access_level", merge_requests_access_level)
         if merge_requests_enabled and not isinstance(merge_requests_enabled, bool):
             raise TypeError("Expected argument 'merge_requests_enabled' to be a bool")
         pulumi.set(__self__, "merge_requests_enabled", merge_requests_enabled)
         if merge_trains_enabled and not isinstance(merge_trains_enabled, bool):
             raise TypeError("Expected argument 'merge_trains_enabled' to be a bool")
         pulumi.set(__self__, "merge_trains_enabled", merge_trains_enabled)
+        if monitor_access_level and not isinstance(monitor_access_level, str):
+            raise TypeError("Expected argument 'monitor_access_level' to be a str")
+        pulumi.set(__self__, "monitor_access_level", monitor_access_level)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if namespace_id and not isinstance(namespace_id, int):
             raise TypeError("Expected argument 'namespace_id' to be a int")
         pulumi.set(__self__, "namespace_id", namespace_id)
         if operations_access_level and not isinstance(operations_access_level, str):
@@ -127,17 +148,20 @@
         pulumi.set(__self__, "pipelines_enabled", pipelines_enabled)
         if printing_merge_request_link_enabled and not isinstance(printing_merge_request_link_enabled, bool):
             raise TypeError("Expected argument 'printing_merge_request_link_enabled' to be a bool")
         pulumi.set(__self__, "printing_merge_request_link_enabled", printing_merge_request_link_enabled)
         if public_builds and not isinstance(public_builds, bool):
             raise TypeError("Expected argument 'public_builds' to be a bool")
         pulumi.set(__self__, "public_builds", public_builds)
-        if push_rules and not isinstance(push_rules, dict):
-            raise TypeError("Expected argument 'push_rules' to be a dict")
+        if push_rules and not isinstance(push_rules, list):
+            raise TypeError("Expected argument 'push_rules' to be a list")
         pulumi.set(__self__, "push_rules", push_rules)
+        if releases_access_level and not isinstance(releases_access_level, str):
+            raise TypeError("Expected argument 'releases_access_level' to be a str")
+        pulumi.set(__self__, "releases_access_level", releases_access_level)
         if remove_source_branch_after_merge and not isinstance(remove_source_branch_after_merge, bool):
             raise TypeError("Expected argument 'remove_source_branch_after_merge' to be a bool")
         pulumi.set(__self__, "remove_source_branch_after_merge", remove_source_branch_after_merge)
         if repository_access_level and not isinstance(repository_access_level, str):
             raise TypeError("Expected argument 'repository_access_level' to be a str")
         pulumi.set(__self__, "repository_access_level", repository_access_level)
         if repository_storage and not isinstance(repository_storage, str):
@@ -148,14 +172,17 @@
         pulumi.set(__self__, "request_access_enabled", request_access_enabled)
         if requirements_access_level and not isinstance(requirements_access_level, str):
             raise TypeError("Expected argument 'requirements_access_level' to be a str")
         pulumi.set(__self__, "requirements_access_level", requirements_access_level)
         if resolve_outdated_diff_discussions and not isinstance(resolve_outdated_diff_discussions, bool):
             raise TypeError("Expected argument 'resolve_outdated_diff_discussions' to be a bool")
         pulumi.set(__self__, "resolve_outdated_diff_discussions", resolve_outdated_diff_discussions)
+        if restrict_user_defined_variables and not isinstance(restrict_user_defined_variables, bool):
+            raise TypeError("Expected argument 'restrict_user_defined_variables' to be a bool")
+        pulumi.set(__self__, "restrict_user_defined_variables", restrict_user_defined_variables)
         if runners_token and not isinstance(runners_token, str):
             raise TypeError("Expected argument 'runners_token' to be a str")
         pulumi.set(__self__, "runners_token", runners_token)
         if security_and_compliance_access_level and not isinstance(security_and_compliance_access_level, str):
             raise TypeError("Expected argument 'security_and_compliance_access_level' to be a str")
         pulumi.set(__self__, "security_and_compliance_access_level", security_and_compliance_access_level)
         if snippets_access_level and not isinstance(snippets_access_level, str):
@@ -166,14 +193,17 @@
         pulumi.set(__self__, "snippets_enabled", snippets_enabled)
         if squash_commit_template and not isinstance(squash_commit_template, str):
             raise TypeError("Expected argument 'squash_commit_template' to be a str")
         pulumi.set(__self__, "squash_commit_template", squash_commit_template)
         if ssh_url_to_repo and not isinstance(ssh_url_to_repo, str):
             raise TypeError("Expected argument 'ssh_url_to_repo' to be a str")
         pulumi.set(__self__, "ssh_url_to_repo", ssh_url_to_repo)
+        if suggestion_commit_message and not isinstance(suggestion_commit_message, str):
+            raise TypeError("Expected argument 'suggestion_commit_message' to be a str")
+        pulumi.set(__self__, "suggestion_commit_message", suggestion_commit_message)
         if topics and not isinstance(topics, list):
             raise TypeError("Expected argument 'topics' to be a list")
         pulumi.set(__self__, "topics", topics)
         if visibility_level and not isinstance(visibility_level, str):
             raise TypeError("Expected argument 'visibility_level' to be a str")
         pulumi.set(__self__, "visibility_level", visibility_level)
         if web_url and not isinstance(web_url, str):
@@ -271,14 +301,22 @@
     def ci_default_git_depth(self) -> int:
         """
         Default number of revisions for shallow cloning.
         """
         return pulumi.get(self, "ci_default_git_depth")
 
     @property
+    @pulumi.getter(name="ciSeparatedCaches")
+    def ci_separated_caches(self) -> bool:
+        """
+        Use separate caches for protected branches.
+        """
+        return pulumi.get(self, "ci_separated_caches")
+
+    @property
     @pulumi.getter(name="containerExpirationPolicies")
     def container_expiration_policies(self) -> Sequence['outputs.GetProjectContainerExpirationPolicyResult']:
         """
         Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         """
         return pulumi.get(self, "container_expiration_policies")
 
@@ -311,22 +349,38 @@
     def emails_disabled(self) -> bool:
         """
         Disable email notifications.
         """
         return pulumi.get(self, "emails_disabled")
 
     @property
+    @pulumi.getter(name="environmentsAccessLevel")
+    def environments_access_level(self) -> str:
+        """
+        Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "environments_access_level")
+
+    @property
     @pulumi.getter(name="externalAuthorizationClassificationLabel")
     def external_authorization_classification_label(self) -> str:
         """
         The classification label for the project.
         """
         return pulumi.get(self, "external_authorization_classification_label")
 
     @property
+    @pulumi.getter(name="featureFlagsAccessLevel")
+    def feature_flags_access_level(self) -> str:
+        """
+        Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "feature_flags_access_level")
+
+    @property
     @pulumi.getter(name="forkingAccessLevel")
     def forking_access_level(self) -> str:
         """
         Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "forking_access_level")
 
@@ -338,19 +392,35 @@
         """
         return pulumi.get(self, "http_url_to_repo")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The integer or path with namespace that uniquely identifies the project within the gitlab install.
+        The integer that uniquely identifies the project within the gitlab install.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="importUrl")
+    def import_url(self) -> str:
+        """
+        URL the project was imported from.
+        """
+        return pulumi.get(self, "import_url")
+
+    @property
+    @pulumi.getter(name="infrastructureAccessLevel")
+    def infrastructure_access_level(self) -> str:
+        """
+        Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "infrastructure_access_level")
+
+    @property
     @pulumi.getter(name="issuesAccessLevel")
     def issues_access_level(self) -> str:
         """
         Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "issues_access_level")
 
@@ -359,14 +429,22 @@
     def issues_enabled(self) -> bool:
         """
         Enable issue tracking for the project.
         """
         return pulumi.get(self, "issues_enabled")
 
     @property
+    @pulumi.getter(name="keepLatestArtifact")
+    def keep_latest_artifact(self) -> bool:
+        """
+        Disable or enable the ability to keep the latest artifact for this project.
+        """
+        return pulumi.get(self, "keep_latest_artifact")
+
+    @property
     @pulumi.getter(name="lfsEnabled")
     def lfs_enabled(self) -> bool:
         """
         Enable LFS for the project.
         """
         return pulumi.get(self, "lfs_enabled")
 
@@ -407,14 +485,22 @@
     def merge_trains_enabled(self) -> bool:
         """
         Enable or disable merge trains.
         """
         return pulumi.get(self, "merge_trains_enabled")
 
     @property
+    @pulumi.getter(name="monitorAccessLevel")
+    def monitor_access_level(self) -> str:
+        """
+        Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "monitor_access_level")
+
+    @property
     @pulumi.getter
     def name(self) -> str:
         """
         The name of the project.
         """
         return pulumi.get(self, "name")
 
@@ -472,21 +558,29 @@
         """
         If true, jobs can be viewed by non-project members.
         """
         return pulumi.get(self, "public_builds")
 
     @property
     @pulumi.getter(name="pushRules")
-    def push_rules(self) -> 'outputs.GetProjectPushRulesResult':
+    def push_rules(self) -> Sequence['outputs.GetProjectPushRuleResult']:
         """
-        Push rules for the project.
+        Push rules for the project. Push rules are only available on Enterprise plans and if the authenticated has permissions to read them.
         """
         return pulumi.get(self, "push_rules")
 
     @property
+    @pulumi.getter(name="releasesAccessLevel")
+    def releases_access_level(self) -> str:
+        """
+        Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "releases_access_level")
+
+    @property
     @pulumi.getter(name="removeSourceBranchAfterMerge")
     def remove_source_branch_after_merge(self) -> bool:
         """
         Enable `Delete source branch` option by default for all new merge requests
         """
         return pulumi.get(self, "remove_source_branch_after_merge")
 
@@ -527,14 +621,22 @@
     def resolve_outdated_diff_discussions(self) -> bool:
         """
         Automatically resolve merge request diffs discussions on lines changed with a push.
         """
         return pulumi.get(self, "resolve_outdated_diff_discussions")
 
     @property
+    @pulumi.getter(name="restrictUserDefinedVariables")
+    def restrict_user_defined_variables(self) -> bool:
+        """
+        Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
+        """
+        return pulumi.get(self, "restrict_user_defined_variables")
+
+    @property
     @pulumi.getter(name="runnersToken")
     def runners_token(self) -> str:
         """
         Registration token to use during runner setup.
         """
         return pulumi.get(self, "runners_token")
 
@@ -575,14 +677,22 @@
     def ssh_url_to_repo(self) -> str:
         """
         URL that can be provided to `git clone` to clone the
         """
         return pulumi.get(self, "ssh_url_to_repo")
 
     @property
+    @pulumi.getter(name="suggestionCommitMessage")
+    def suggestion_commit_message(self) -> str:
+        """
+        The commit message used to apply merge request suggestions.
+        """
+        return pulumi.get(self, "suggestion_commit_message")
+
+    @property
     @pulumi.getter
     def topics(self) -> Sequence[str]:
         """
         The list of topics for the project.
         """
         return pulumi.get(self, "topics")
 
@@ -632,52 +742,62 @@
             auto_devops_enabled=self.auto_devops_enabled,
             autoclose_referenced_issues=self.autoclose_referenced_issues,
             build_git_strategy=self.build_git_strategy,
             build_timeout=self.build_timeout,
             builds_access_level=self.builds_access_level,
             ci_config_path=self.ci_config_path,
             ci_default_git_depth=self.ci_default_git_depth,
+            ci_separated_caches=self.ci_separated_caches,
             container_expiration_policies=self.container_expiration_policies,
             container_registry_access_level=self.container_registry_access_level,
             default_branch=self.default_branch,
             description=self.description,
             emails_disabled=self.emails_disabled,
+            environments_access_level=self.environments_access_level,
             external_authorization_classification_label=self.external_authorization_classification_label,
+            feature_flags_access_level=self.feature_flags_access_level,
             forking_access_level=self.forking_access_level,
             http_url_to_repo=self.http_url_to_repo,
             id=self.id,
+            import_url=self.import_url,
+            infrastructure_access_level=self.infrastructure_access_level,
             issues_access_level=self.issues_access_level,
             issues_enabled=self.issues_enabled,
+            keep_latest_artifact=self.keep_latest_artifact,
             lfs_enabled=self.lfs_enabled,
             merge_commit_template=self.merge_commit_template,
             merge_pipelines_enabled=self.merge_pipelines_enabled,
             merge_requests_access_level=self.merge_requests_access_level,
             merge_requests_enabled=self.merge_requests_enabled,
             merge_trains_enabled=self.merge_trains_enabled,
+            monitor_access_level=self.monitor_access_level,
             name=self.name,
             namespace_id=self.namespace_id,
             operations_access_level=self.operations_access_level,
             path=self.path,
             path_with_namespace=self.path_with_namespace,
             pipelines_enabled=self.pipelines_enabled,
             printing_merge_request_link_enabled=self.printing_merge_request_link_enabled,
             public_builds=self.public_builds,
             push_rules=self.push_rules,
+            releases_access_level=self.releases_access_level,
             remove_source_branch_after_merge=self.remove_source_branch_after_merge,
             repository_access_level=self.repository_access_level,
             repository_storage=self.repository_storage,
             request_access_enabled=self.request_access_enabled,
             requirements_access_level=self.requirements_access_level,
             resolve_outdated_diff_discussions=self.resolve_outdated_diff_discussions,
+            restrict_user_defined_variables=self.restrict_user_defined_variables,
             runners_token=self.runners_token,
             security_and_compliance_access_level=self.security_and_compliance_access_level,
             snippets_access_level=self.snippets_access_level,
             snippets_enabled=self.snippets_enabled,
             squash_commit_template=self.squash_commit_template,
             ssh_url_to_repo=self.ssh_url_to_repo,
+            suggestion_commit_message=self.suggestion_commit_message,
             topics=self.topics,
             visibility_level=self.visibility_level,
             web_url=self.web_url,
             wiki_access_level=self.wiki_access_level,
             wiki_enabled=self.wiki_enabled)
 
 
@@ -693,20 +813,20 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    example = gitlab.get_project(id="foo/bar/baz")
+    example = gitlab.get_project(path_with_namespace="foo/bar/baz")
     ```
 
 
     :param int ci_default_git_depth: Default number of revisions for shallow cloning.
-    :param str id: The integer or path with namespace that uniquely identifies the project within the gitlab install.
+    :param str id: The integer that uniquely identifies the project within the gitlab install.
     :param str path_with_namespace: The path of the repository with namespace.
     :param bool public_builds: If true, jobs can be viewed by non-project members.
     """
     __args__ = dict()
     __args__['ciDefaultGitDepth'] = ci_default_git_depth
     __args__['id'] = id
     __args__['pathWithNamespace'] = path_with_namespace
@@ -722,52 +842,62 @@
         auto_devops_enabled=__ret__.auto_devops_enabled,
         autoclose_referenced_issues=__ret__.autoclose_referenced_issues,
         build_git_strategy=__ret__.build_git_strategy,
         build_timeout=__ret__.build_timeout,
         builds_access_level=__ret__.builds_access_level,
         ci_config_path=__ret__.ci_config_path,
         ci_default_git_depth=__ret__.ci_default_git_depth,
+        ci_separated_caches=__ret__.ci_separated_caches,
         container_expiration_policies=__ret__.container_expiration_policies,
         container_registry_access_level=__ret__.container_registry_access_level,
         default_branch=__ret__.default_branch,
         description=__ret__.description,
         emails_disabled=__ret__.emails_disabled,
+        environments_access_level=__ret__.environments_access_level,
         external_authorization_classification_label=__ret__.external_authorization_classification_label,
+        feature_flags_access_level=__ret__.feature_flags_access_level,
         forking_access_level=__ret__.forking_access_level,
         http_url_to_repo=__ret__.http_url_to_repo,
         id=__ret__.id,
+        import_url=__ret__.import_url,
+        infrastructure_access_level=__ret__.infrastructure_access_level,
         issues_access_level=__ret__.issues_access_level,
         issues_enabled=__ret__.issues_enabled,
+        keep_latest_artifact=__ret__.keep_latest_artifact,
         lfs_enabled=__ret__.lfs_enabled,
         merge_commit_template=__ret__.merge_commit_template,
         merge_pipelines_enabled=__ret__.merge_pipelines_enabled,
         merge_requests_access_level=__ret__.merge_requests_access_level,
         merge_requests_enabled=__ret__.merge_requests_enabled,
         merge_trains_enabled=__ret__.merge_trains_enabled,
+        monitor_access_level=__ret__.monitor_access_level,
         name=__ret__.name,
         namespace_id=__ret__.namespace_id,
         operations_access_level=__ret__.operations_access_level,
         path=__ret__.path,
         path_with_namespace=__ret__.path_with_namespace,
         pipelines_enabled=__ret__.pipelines_enabled,
         printing_merge_request_link_enabled=__ret__.printing_merge_request_link_enabled,
         public_builds=__ret__.public_builds,
         push_rules=__ret__.push_rules,
+        releases_access_level=__ret__.releases_access_level,
         remove_source_branch_after_merge=__ret__.remove_source_branch_after_merge,
         repository_access_level=__ret__.repository_access_level,
         repository_storage=__ret__.repository_storage,
         request_access_enabled=__ret__.request_access_enabled,
         requirements_access_level=__ret__.requirements_access_level,
         resolve_outdated_diff_discussions=__ret__.resolve_outdated_diff_discussions,
+        restrict_user_defined_variables=__ret__.restrict_user_defined_variables,
         runners_token=__ret__.runners_token,
         security_and_compliance_access_level=__ret__.security_and_compliance_access_level,
         snippets_access_level=__ret__.snippets_access_level,
         snippets_enabled=__ret__.snippets_enabled,
         squash_commit_template=__ret__.squash_commit_template,
         ssh_url_to_repo=__ret__.ssh_url_to_repo,
+        suggestion_commit_message=__ret__.suggestion_commit_message,
         topics=__ret__.topics,
         visibility_level=__ret__.visibility_level,
         web_url=__ret__.web_url,
         wiki_access_level=__ret__.wiki_access_level,
         wiki_enabled=__ret__.wiki_enabled)
 
 
@@ -784,17 +914,17 @@
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_gitlab as gitlab
 
-    example = gitlab.get_project(id="foo/bar/baz")
+    example = gitlab.get_project(path_with_namespace="foo/bar/baz")
     ```
 
 
     :param int ci_default_git_depth: Default number of revisions for shallow cloning.
-    :param str id: The integer or path with namespace that uniquely identifies the project within the gitlab install.
+    :param str id: The integer that uniquely identifies the project within the gitlab install.
     :param str path_with_namespace: The path of the repository with namespace.
     :param bool public_builds: If true, jobs can be viewed by non-project members.
     """
     ...
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_issue.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,14 @@
         return pulumi.get(self, "downvotes")
 
     @property
     @pulumi.getter(name="dueDate")
     def due_date(self) -> str:
         """
         The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         """
         return pulumi.get(self, "due_date")
 
     @property
     @pulumi.getter(name="epicId")
     def epic_id(self) -> int:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_issues.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_milestone.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         """
         return pulumi.get(self, "due_date")
 
     @property
     @pulumi.getter
     def expired(self) -> bool:
         """
-        Bool, true if milestore expired.
+        Bool, true if milestone expired.
         """
         return pulumi.get(self, "expired")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_milestones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_protected_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_protected_branches.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             project_id=self.project_id,
             protected_branches=self.protected_branches)
 
 
 def get_project_protected_branches(project_id: Optional[str] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectProtectedBranchesResult:
     """
-    The `gitlab_protected_branches` data source allows details of the protected branches of a given project.
+    The `get_project_protected_branches` data source allows details of the protected branches of a given project.
 
     **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/protected_branches.html#list-protected-branches)
 
     ## Example Usage
 
     ```python
     import pulumi
@@ -99,15 +99,15 @@
         protected_branches=__ret__.protected_branches)
 
 
 @_utilities.lift_output_func(get_project_protected_branches)
 def get_project_protected_branches_output(project_id: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectProtectedBranchesResult]:
     """
-    The `gitlab_protected_branches` data source allows details of the protected branches of a given project.
+    The `get_project_protected_branches` data source allows details of the protected branches of a given project.
 
     **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/protected_branches.html#list-protected-branches)
 
     ## Example Usage
 
     ```python
     import pulumi
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_project_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_projects.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         """
         return pulumi.get(self, "min_access_level")
 
     @property
     @pulumi.getter(name="orderBy")
     def order_by(self) -> Optional[str]:
         """
-        Return projects ordered by `id`, `name`, `path`, `created_at`, `updated_at`, or `last_activity_at` fields. Default is `created_at`.
+        Return projects ordered ordered by: `id`, `name`, `path`, `created_at`, `updated_at`, `last_activity_at`, `similarity`, `repository_size`, `storage_size`, `packages_size`, `wiki_size`. Some values or only available in certain circumstances. See [upstream docs](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) for details.
         """
         return pulumi.get(self, "order_by")
 
     @property
     @pulumi.getter
     def owned(self) -> Optional[bool]:
         """
@@ -358,15 +358,15 @@
 
     :param bool archived: Limit by archived status.
     :param int group_id: The ID of the group owned by the authenticated user to look projects for within. Cannot be used with `min_access_level`, `with_programming_language` or `statistics`.
     :param bool include_subgroups: Include projects in subgroups of this group. Default is `false`. Needs `group_id`.
     :param int max_queryable_pages: The maximum number of project results pages that may be queried. Prevents overloading your Gitlab instance in case of a misconfiguration.
     :param bool membership: Limit by projects that the current user is a member of.
     :param int min_access_level: Limit to projects where current user has at least this access level, refer to the [official documentation](https://docs.gitlab.com/ee/api/members.html) for values. Cannot be used with `group_id`.
-    :param str order_by: Return projects ordered by `id`, `name`, `path`, `created_at`, `updated_at`, or `last_activity_at` fields. Default is `created_at`.
+    :param str order_by: Return projects ordered ordered by: `id`, `name`, `path`, `created_at`, `updated_at`, `last_activity_at`, `similarity`, `repository_size`, `storage_size`, `packages_size`, `wiki_size`. Some values or only available in certain circumstances. See [upstream docs](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) for details.
     :param bool owned: Limit by projects owned by the current user.
     :param int page: The first page to begin the query on.
     :param int per_page: The number of results to return per page.
     :param str search: Return list of authorized projects matching the search criteria.
     :param bool simple: Return only the ID, URL, name, and path of each project.
     :param str sort: Return projects sorted in `asc` or `desc` order. Default is `desc`.
     :param bool starred: Limit by projects starred by the current user.
@@ -479,15 +479,15 @@
 
     :param bool archived: Limit by archived status.
     :param int group_id: The ID of the group owned by the authenticated user to look projects for within. Cannot be used with `min_access_level`, `with_programming_language` or `statistics`.
     :param bool include_subgroups: Include projects in subgroups of this group. Default is `false`. Needs `group_id`.
     :param int max_queryable_pages: The maximum number of project results pages that may be queried. Prevents overloading your Gitlab instance in case of a misconfiguration.
     :param bool membership: Limit by projects that the current user is a member of.
     :param int min_access_level: Limit to projects where current user has at least this access level, refer to the [official documentation](https://docs.gitlab.com/ee/api/members.html) for values. Cannot be used with `group_id`.
-    :param str order_by: Return projects ordered by `id`, `name`, `path`, `created_at`, `updated_at`, or `last_activity_at` fields. Default is `created_at`.
+    :param str order_by: Return projects ordered ordered by: `id`, `name`, `path`, `created_at`, `updated_at`, `last_activity_at`, `similarity`, `repository_size`, `storage_size`, `packages_size`, `wiki_size`. Some values or only available in certain circumstances. See [upstream docs](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) for details.
     :param bool owned: Limit by projects owned by the current user.
     :param int page: The first page to begin the query on.
     :param int per_page: The number of results to return per page.
     :param str search: Return list of authorized projects matching the search criteria.
     :param bool simple: Return only the ID, URL, name, and path of each project.
     :param str sort: Return projects sorted in `asc` or `desc` order. Default is `desc`.
     :param bool starred: Limit by projects starred by the current user.
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_release_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_repository_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_user.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_users.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/repository_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,1070 +5,805 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['GroupArgs', 'Group']
+__all__ = ['RepositoryFileArgs', 'RepositoryFile']
 
 @pulumi.input_type
-class GroupArgs:
+class RepositoryFileArgs:
     def __init__(__self__, *,
-                 path: pulumi.Input[str],
-                 auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
-                 default_branch_protection: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 emails_disabled: Optional[pulumi.Input[bool]] = None,
-                 lfs_enabled: Optional[pulumi.Input[bool]] = None,
-                 mentions_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 parent_id: Optional[pulumi.Input[int]] = None,
-                 prevent_forking_outside_group: Optional[pulumi.Input[bool]] = None,
-                 project_creation_level: Optional[pulumi.Input[str]] = None,
-                 request_access_enabled: Optional[pulumi.Input[bool]] = None,
-                 require_two_factor_authentication: Optional[pulumi.Input[bool]] = None,
-                 share_with_group_lock: Optional[pulumi.Input[bool]] = None,
-                 subgroup_creation_level: Optional[pulumi.Input[str]] = None,
-                 two_factor_grace_period: Optional[pulumi.Input[int]] = None,
-                 visibility_level: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a Group resource.
-        :param pulumi.Input[str] path: The path of the group.
-        :param pulumi.Input[bool] auto_devops_enabled: Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        :param pulumi.Input[int] default_branch_protection: Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        :param pulumi.Input[str] description: The description of the group.
-        :param pulumi.Input[bool] emails_disabled: Defaults to false. Disable email notifications.
-        :param pulumi.Input[bool] lfs_enabled: Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
-        :param pulumi.Input[bool] mentions_disabled: Defaults to false. Disable the capability of a group from getting mentioned.
-        :param pulumi.Input[str] name: The name of this group.
-        :param pulumi.Input[int] parent_id: Id of the parent group (creates a nested group).
-        :param pulumi.Input[bool] prevent_forking_outside_group: Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
-        :param pulumi.Input[str] project_creation_level: Defaults to maintainer. Determine if developers can create projects in the group.
-        :param pulumi.Input[bool] request_access_enabled: Defaults to false. Allow users to request member access.
-        :param pulumi.Input[bool] require_two_factor_authentication: Defaults to false. Require all users in this group to setup Two-factor authentication.
-        :param pulumi.Input[bool] share_with_group_lock: Defaults to false. Prevent sharing a project with another group within this group.
-        :param pulumi.Input[str] subgroup_creation_level: Defaults to owner. Allowed to create subgroups.
-        :param pulumi.Input[int] two_factor_grace_period: Defaults to 48. Time before Two-factor authentication is enforced (in hours).
-        :param pulumi.Input[str] visibility_level: The group's visibility. Can be `private`, `internal`, or `public`.
-        """
-        pulumi.set(__self__, "path", path)
-        if auto_devops_enabled is not None:
-            pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
-        if default_branch_protection is not None:
-            pulumi.set(__self__, "default_branch_protection", default_branch_protection)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if emails_disabled is not None:
-            pulumi.set(__self__, "emails_disabled", emails_disabled)
-        if lfs_enabled is not None:
-            pulumi.set(__self__, "lfs_enabled", lfs_enabled)
-        if mentions_disabled is not None:
-            pulumi.set(__self__, "mentions_disabled", mentions_disabled)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if parent_id is not None:
-            pulumi.set(__self__, "parent_id", parent_id)
-        if prevent_forking_outside_group is not None:
-            pulumi.set(__self__, "prevent_forking_outside_group", prevent_forking_outside_group)
-        if project_creation_level is not None:
-            pulumi.set(__self__, "project_creation_level", project_creation_level)
-        if request_access_enabled is not None:
-            pulumi.set(__self__, "request_access_enabled", request_access_enabled)
-        if require_two_factor_authentication is not None:
-            pulumi.set(__self__, "require_two_factor_authentication", require_two_factor_authentication)
-        if share_with_group_lock is not None:
-            pulumi.set(__self__, "share_with_group_lock", share_with_group_lock)
-        if subgroup_creation_level is not None:
-            pulumi.set(__self__, "subgroup_creation_level", subgroup_creation_level)
-        if two_factor_grace_period is not None:
-            pulumi.set(__self__, "two_factor_grace_period", two_factor_grace_period)
-        if visibility_level is not None:
-            pulumi.set(__self__, "visibility_level", visibility_level)
+                 branch: pulumi.Input[str],
+                 commit_message: pulumi.Input[str],
+                 content: pulumi.Input[str],
+                 file_path: pulumi.Input[str],
+                 project: pulumi.Input[str],
+                 author_email: Optional[pulumi.Input[str]] = None,
+                 author_name: Optional[pulumi.Input[str]] = None,
+                 execute_filemode: Optional[pulumi.Input[bool]] = None,
+                 overwrite_on_create: Optional[pulumi.Input[bool]] = None,
+                 start_branch: Optional[pulumi.Input[str]] = None):
+        """
+        The set of arguments for constructing a RepositoryFile resource.
+        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
+        :param pulumi.Input[str] commit_message: Commit message.
+        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+        :param pulumi.Input[str] project: The name or ID of the project.
+        :param pulumi.Input[str] author_email: Email of the commit author.
+        :param pulumi.Input[str] author_name: Name of the commit author.
+        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
+        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
+        """
+        pulumi.set(__self__, "branch", branch)
+        pulumi.set(__self__, "commit_message", commit_message)
+        pulumi.set(__self__, "content", content)
+        pulumi.set(__self__, "file_path", file_path)
+        pulumi.set(__self__, "project", project)
+        if author_email is not None:
+            pulumi.set(__self__, "author_email", author_email)
+        if author_name is not None:
+            pulumi.set(__self__, "author_name", author_name)
+        if execute_filemode is not None:
+            pulumi.set(__self__, "execute_filemode", execute_filemode)
+        if overwrite_on_create is not None:
+            pulumi.set(__self__, "overwrite_on_create", overwrite_on_create)
+        if start_branch is not None:
+            pulumi.set(__self__, "start_branch", start_branch)
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Input[str]:
+    def branch(self) -> pulumi.Input[str]:
         """
-        The path of the group.
+        Name of the branch to which to commit to.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "branch")
 
-    @path.setter
-    def path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "path", value)
+    @branch.setter
+    def branch(self, value: pulumi.Input[str]):
+        pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="autoDevopsEnabled")
-    def auto_devops_enabled(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="commitMessage")
+    def commit_message(self) -> pulumi.Input[str]:
         """
-        Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
+        Commit message.
         """
-        return pulumi.get(self, "auto_devops_enabled")
+        return pulumi.get(self, "commit_message")
 
-    @auto_devops_enabled.setter
-    def auto_devops_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "auto_devops_enabled", value)
-
-    @property
-    @pulumi.getter(name="defaultBranchProtection")
-    def default_branch_protection(self) -> Optional[pulumi.Input[int]]:
-        """
-        Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        """
-        return pulumi.get(self, "default_branch_protection")
-
-    @default_branch_protection.setter
-    def default_branch_protection(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "default_branch_protection", value)
+    @commit_message.setter
+    def commit_message(self, value: pulumi.Input[str]):
+        pulumi.set(self, "commit_message", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        The description of the group.
+    def content(self) -> pulumi.Input[str]:
         """
-        return pulumi.get(self, "description")
-
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
-
-    @property
-    @pulumi.getter(name="emailsDisabled")
-    def emails_disabled(self) -> Optional[pulumi.Input[bool]]:
+        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
         """
-        Defaults to false. Disable email notifications.
-        """
-        return pulumi.get(self, "emails_disabled")
+        return pulumi.get(self, "content")
 
-    @emails_disabled.setter
-    def emails_disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "emails_disabled", value)
+    @content.setter
+    def content(self, value: pulumi.Input[str]):
+        pulumi.set(self, "content", value)
 
     @property
-    @pulumi.getter(name="lfsEnabled")
-    def lfs_enabled(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="filePath")
+    def file_path(self) -> pulumi.Input[str]:
         """
-        Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
+        The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         """
-        return pulumi.get(self, "lfs_enabled")
+        return pulumi.get(self, "file_path")
 
-    @lfs_enabled.setter
-    def lfs_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "lfs_enabled", value)
-
-    @property
-    @pulumi.getter(name="mentionsDisabled")
-    def mentions_disabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Defaults to false. Disable the capability of a group from getting mentioned.
-        """
-        return pulumi.get(self, "mentions_disabled")
-
-    @mentions_disabled.setter
-    def mentions_disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "mentions_disabled", value)
+    @file_path.setter
+    def file_path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "file_path", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        The name of this group.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter(name="parentId")
-    def parent_id(self) -> Optional[pulumi.Input[int]]:
-        """
-        Id of the parent group (creates a nested group).
-        """
-        return pulumi.get(self, "parent_id")
-
-    @parent_id.setter
-    def parent_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "parent_id", value)
-
-    @property
-    @pulumi.getter(name="preventForkingOutsideGroup")
-    def prevent_forking_outside_group(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
-        """
-        return pulumi.get(self, "prevent_forking_outside_group")
-
-    @prevent_forking_outside_group.setter
-    def prevent_forking_outside_group(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "prevent_forking_outside_group", value)
-
-    @property
-    @pulumi.getter(name="projectCreationLevel")
-    def project_creation_level(self) -> Optional[pulumi.Input[str]]:
-        """
-        Defaults to maintainer. Determine if developers can create projects in the group.
-        """
-        return pulumi.get(self, "project_creation_level")
-
-    @project_creation_level.setter
-    def project_creation_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_creation_level", value)
-
-    @property
-    @pulumi.getter(name="requestAccessEnabled")
-    def request_access_enabled(self) -> Optional[pulumi.Input[bool]]:
+    def project(self) -> pulumi.Input[str]:
         """
-        Defaults to false. Allow users to request member access.
+        The name or ID of the project.
         """
-        return pulumi.get(self, "request_access_enabled")
+        return pulumi.get(self, "project")
 
-    @request_access_enabled.setter
-    def request_access_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "request_access_enabled", value)
+    @project.setter
+    def project(self, value: pulumi.Input[str]):
+        pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="requireTwoFactorAuthentication")
-    def require_two_factor_authentication(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="authorEmail")
+    def author_email(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. Require all users in this group to setup Two-factor authentication.
+        Email of the commit author.
         """
-        return pulumi.get(self, "require_two_factor_authentication")
+        return pulumi.get(self, "author_email")
 
-    @require_two_factor_authentication.setter
-    def require_two_factor_authentication(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "require_two_factor_authentication", value)
+    @author_email.setter
+    def author_email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "author_email", value)
 
     @property
-    @pulumi.getter(name="shareWithGroupLock")
-    def share_with_group_lock(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="authorName")
+    def author_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. Prevent sharing a project with another group within this group.
+        Name of the commit author.
         """
-        return pulumi.get(self, "share_with_group_lock")
+        return pulumi.get(self, "author_name")
 
-    @share_with_group_lock.setter
-    def share_with_group_lock(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "share_with_group_lock", value)
+    @author_name.setter
+    def author_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "author_name", value)
 
     @property
-    @pulumi.getter(name="subgroupCreationLevel")
-    def subgroup_creation_level(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="executeFilemode")
+    def execute_filemode(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defaults to owner. Allowed to create subgroups.
+        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         """
-        return pulumi.get(self, "subgroup_creation_level")
+        return pulumi.get(self, "execute_filemode")
 
-    @subgroup_creation_level.setter
-    def subgroup_creation_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "subgroup_creation_level", value)
+    @execute_filemode.setter
+    def execute_filemode(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "execute_filemode", value)
 
     @property
-    @pulumi.getter(name="twoFactorGracePeriod")
-    def two_factor_grace_period(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="overwriteOnCreate")
+    def overwrite_on_create(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defaults to 48. Time before Two-factor authentication is enforced (in hours).
+        Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
         """
-        return pulumi.get(self, "two_factor_grace_period")
+        return pulumi.get(self, "overwrite_on_create")
 
-    @two_factor_grace_period.setter
-    def two_factor_grace_period(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "two_factor_grace_period", value)
+    @overwrite_on_create.setter
+    def overwrite_on_create(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "overwrite_on_create", value)
 
     @property
-    @pulumi.getter(name="visibilityLevel")
-    def visibility_level(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="startBranch")
+    def start_branch(self) -> Optional[pulumi.Input[str]]:
         """
-        The group's visibility. Can be `private`, `internal`, or `public`.
+        Name of the branch to start the new commit from.
         """
-        return pulumi.get(self, "visibility_level")
+        return pulumi.get(self, "start_branch")
 
-    @visibility_level.setter
-    def visibility_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "visibility_level", value)
+    @start_branch.setter
+    def start_branch(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start_branch", value)
 
 
 @pulumi.input_type
-class _GroupState:
+class _RepositoryFileState:
     def __init__(__self__, *,
-                 auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
-                 default_branch_protection: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 emails_disabled: Optional[pulumi.Input[bool]] = None,
-                 full_name: Optional[pulumi.Input[str]] = None,
-                 full_path: Optional[pulumi.Input[str]] = None,
-                 lfs_enabled: Optional[pulumi.Input[bool]] = None,
-                 mentions_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 parent_id: Optional[pulumi.Input[int]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 prevent_forking_outside_group: Optional[pulumi.Input[bool]] = None,
-                 project_creation_level: Optional[pulumi.Input[str]] = None,
-                 request_access_enabled: Optional[pulumi.Input[bool]] = None,
-                 require_two_factor_authentication: Optional[pulumi.Input[bool]] = None,
-                 runners_token: Optional[pulumi.Input[str]] = None,
-                 share_with_group_lock: Optional[pulumi.Input[bool]] = None,
-                 subgroup_creation_level: Optional[pulumi.Input[str]] = None,
-                 two_factor_grace_period: Optional[pulumi.Input[int]] = None,
-                 visibility_level: Optional[pulumi.Input[str]] = None,
-                 web_url: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering Group resources.
-        :param pulumi.Input[bool] auto_devops_enabled: Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        :param pulumi.Input[int] default_branch_protection: Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        :param pulumi.Input[str] description: The description of the group.
-        :param pulumi.Input[bool] emails_disabled: Defaults to false. Disable email notifications.
-        :param pulumi.Input[str] full_name: The full name of the group.
-        :param pulumi.Input[str] full_path: The full path of the group.
-        :param pulumi.Input[bool] lfs_enabled: Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
-        :param pulumi.Input[bool] mentions_disabled: Defaults to false. Disable the capability of a group from getting mentioned.
-        :param pulumi.Input[str] name: The name of this group.
-        :param pulumi.Input[int] parent_id: Id of the parent group (creates a nested group).
-        :param pulumi.Input[str] path: The path of the group.
-        :param pulumi.Input[bool] prevent_forking_outside_group: Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
-        :param pulumi.Input[str] project_creation_level: Defaults to maintainer. Determine if developers can create projects in the group.
-        :param pulumi.Input[bool] request_access_enabled: Defaults to false. Allow users to request member access.
-        :param pulumi.Input[bool] require_two_factor_authentication: Defaults to false. Require all users in this group to setup Two-factor authentication.
-        :param pulumi.Input[str] runners_token: The group level registration token to use during runner setup.
-        :param pulumi.Input[bool] share_with_group_lock: Defaults to false. Prevent sharing a project with another group within this group.
-        :param pulumi.Input[str] subgroup_creation_level: Defaults to owner. Allowed to create subgroups.
-        :param pulumi.Input[int] two_factor_grace_period: Defaults to 48. Time before Two-factor authentication is enforced (in hours).
-        :param pulumi.Input[str] visibility_level: The group's visibility. Can be `private`, `internal`, or `public`.
-        :param pulumi.Input[str] web_url: Web URL of the group.
-        """
-        if auto_devops_enabled is not None:
-            pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
-        if default_branch_protection is not None:
-            pulumi.set(__self__, "default_branch_protection", default_branch_protection)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if emails_disabled is not None:
-            pulumi.set(__self__, "emails_disabled", emails_disabled)
-        if full_name is not None:
-            pulumi.set(__self__, "full_name", full_name)
-        if full_path is not None:
-            pulumi.set(__self__, "full_path", full_path)
-        if lfs_enabled is not None:
-            pulumi.set(__self__, "lfs_enabled", lfs_enabled)
-        if mentions_disabled is not None:
-            pulumi.set(__self__, "mentions_disabled", mentions_disabled)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if parent_id is not None:
-            pulumi.set(__self__, "parent_id", parent_id)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
-        if prevent_forking_outside_group is not None:
-            pulumi.set(__self__, "prevent_forking_outside_group", prevent_forking_outside_group)
-        if project_creation_level is not None:
-            pulumi.set(__self__, "project_creation_level", project_creation_level)
-        if request_access_enabled is not None:
-            pulumi.set(__self__, "request_access_enabled", request_access_enabled)
-        if require_two_factor_authentication is not None:
-            pulumi.set(__self__, "require_two_factor_authentication", require_two_factor_authentication)
-        if runners_token is not None:
-            pulumi.set(__self__, "runners_token", runners_token)
-        if share_with_group_lock is not None:
-            pulumi.set(__self__, "share_with_group_lock", share_with_group_lock)
-        if subgroup_creation_level is not None:
-            pulumi.set(__self__, "subgroup_creation_level", subgroup_creation_level)
-        if two_factor_grace_period is not None:
-            pulumi.set(__self__, "two_factor_grace_period", two_factor_grace_period)
-        if visibility_level is not None:
-            pulumi.set(__self__, "visibility_level", visibility_level)
-        if web_url is not None:
-            pulumi.set(__self__, "web_url", web_url)
-
-    @property
-    @pulumi.getter(name="autoDevopsEnabled")
-    def auto_devops_enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        """
-        return pulumi.get(self, "auto_devops_enabled")
-
-    @auto_devops_enabled.setter
-    def auto_devops_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "auto_devops_enabled", value)
-
-    @property
-    @pulumi.getter(name="defaultBranchProtection")
-    def default_branch_protection(self) -> Optional[pulumi.Input[int]]:
-        """
-        Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        """
-        return pulumi.get(self, "default_branch_protection")
-
-    @default_branch_protection.setter
-    def default_branch_protection(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "default_branch_protection", value)
+                 author_email: Optional[pulumi.Input[str]] = None,
+                 author_name: Optional[pulumi.Input[str]] = None,
+                 blob_id: Optional[pulumi.Input[str]] = None,
+                 branch: Optional[pulumi.Input[str]] = None,
+                 commit_id: Optional[pulumi.Input[str]] = None,
+                 commit_message: Optional[pulumi.Input[str]] = None,
+                 content: Optional[pulumi.Input[str]] = None,
+                 content_sha256: Optional[pulumi.Input[str]] = None,
+                 encoding: Optional[pulumi.Input[str]] = None,
+                 execute_filemode: Optional[pulumi.Input[bool]] = None,
+                 file_name: Optional[pulumi.Input[str]] = None,
+                 file_path: Optional[pulumi.Input[str]] = None,
+                 last_commit_id: Optional[pulumi.Input[str]] = None,
+                 overwrite_on_create: Optional[pulumi.Input[bool]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
+                 size: Optional[pulumi.Input[int]] = None,
+                 start_branch: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering RepositoryFile resources.
+        :param pulumi.Input[str] author_email: Email of the commit author.
+        :param pulumi.Input[str] author_name: Name of the commit author.
+        :param pulumi.Input[str] blob_id: The blob id.
+        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
+        :param pulumi.Input[str] commit_id: The commit id.
+        :param pulumi.Input[str] commit_message: Commit message.
+        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content_sha256: File content sha256 digest.
+        :param pulumi.Input[str] encoding: The file content encoding.
+        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        :param pulumi.Input[str] file_name: The filename.
+        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+        :param pulumi.Input[str] last_commit_id: The last known commit id.
+        :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
+        :param pulumi.Input[str] project: The name or ID of the project.
+        :param pulumi.Input[str] ref: The name of branch, tag or commit.
+        :param pulumi.Input[int] size: The file size.
+        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
+        """
+        if author_email is not None:
+            pulumi.set(__self__, "author_email", author_email)
+        if author_name is not None:
+            pulumi.set(__self__, "author_name", author_name)
+        if blob_id is not None:
+            pulumi.set(__self__, "blob_id", blob_id)
+        if branch is not None:
+            pulumi.set(__self__, "branch", branch)
+        if commit_id is not None:
+            pulumi.set(__self__, "commit_id", commit_id)
+        if commit_message is not None:
+            pulumi.set(__self__, "commit_message", commit_message)
+        if content is not None:
+            pulumi.set(__self__, "content", content)
+        if content_sha256 is not None:
+            pulumi.set(__self__, "content_sha256", content_sha256)
+        if encoding is not None:
+            pulumi.set(__self__, "encoding", encoding)
+        if execute_filemode is not None:
+            pulumi.set(__self__, "execute_filemode", execute_filemode)
+        if file_name is not None:
+            pulumi.set(__self__, "file_name", file_name)
+        if file_path is not None:
+            pulumi.set(__self__, "file_path", file_path)
+        if last_commit_id is not None:
+            pulumi.set(__self__, "last_commit_id", last_commit_id)
+        if overwrite_on_create is not None:
+            pulumi.set(__self__, "overwrite_on_create", overwrite_on_create)
+        if project is not None:
+            pulumi.set(__self__, "project", project)
+        if ref is not None:
+            pulumi.set(__self__, "ref", ref)
+        if size is not None:
+            pulumi.set(__self__, "size", size)
+        if start_branch is not None:
+            pulumi.set(__self__, "start_branch", start_branch)
+
+    @property
+    @pulumi.getter(name="authorEmail")
+    def author_email(self) -> Optional[pulumi.Input[str]]:
+        """
+        Email of the commit author.
+        """
+        return pulumi.get(self, "author_email")
+
+    @author_email.setter
+    def author_email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "author_email", value)
+
+    @property
+    @pulumi.getter(name="authorName")
+    def author_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the commit author.
+        """
+        return pulumi.get(self, "author_name")
+
+    @author_name.setter
+    def author_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "author_name", value)
+
+    @property
+    @pulumi.getter(name="blobId")
+    def blob_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The blob id.
+        """
+        return pulumi.get(self, "blob_id")
+
+    @blob_id.setter
+    def blob_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "blob_id", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def branch(self) -> Optional[pulumi.Input[str]]:
         """
-        The description of the group.
+        Name of the branch to which to commit to.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "branch")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @branch.setter
+    def branch(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "branch", value)
 
     @property
-    @pulumi.getter(name="emailsDisabled")
-    def emails_disabled(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="commitId")
+    def commit_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. Disable email notifications.
+        The commit id.
         """
-        return pulumi.get(self, "emails_disabled")
+        return pulumi.get(self, "commit_id")
 
-    @emails_disabled.setter
-    def emails_disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "emails_disabled", value)
+    @commit_id.setter
+    def commit_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "commit_id", value)
 
     @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="commitMessage")
+    def commit_message(self) -> Optional[pulumi.Input[str]]:
         """
-        The full name of the group.
+        Commit message.
         """
-        return pulumi.get(self, "full_name")
+        return pulumi.get(self, "commit_message")
 
-    @full_name.setter
-    def full_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "full_name", value)
-
-    @property
-    @pulumi.getter(name="fullPath")
-    def full_path(self) -> Optional[pulumi.Input[str]]:
-        """
-        The full path of the group.
-        """
-        return pulumi.get(self, "full_path")
-
-    @full_path.setter
-    def full_path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "full_path", value)
-
-    @property
-    @pulumi.getter(name="lfsEnabled")
-    def lfs_enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
-        """
-        return pulumi.get(self, "lfs_enabled")
-
-    @lfs_enabled.setter
-    def lfs_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "lfs_enabled", value)
-
-    @property
-    @pulumi.getter(name="mentionsDisabled")
-    def mentions_disabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Defaults to false. Disable the capability of a group from getting mentioned.
-        """
-        return pulumi.get(self, "mentions_disabled")
-
-    @mentions_disabled.setter
-    def mentions_disabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "mentions_disabled", value)
+    @commit_message.setter
+    def commit_message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "commit_message", value)
 
     @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def content(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of this group.
+        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "content")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @content.setter
+    def content(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "content", value)
 
     @property
-    @pulumi.getter(name="parentId")
-    def parent_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="contentSha256")
+    def content_sha256(self) -> Optional[pulumi.Input[str]]:
         """
-        Id of the parent group (creates a nested group).
+        File content sha256 digest.
         """
-        return pulumi.get(self, "parent_id")
+        return pulumi.get(self, "content_sha256")
 
-    @parent_id.setter
-    def parent_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "parent_id", value)
+    @content_sha256.setter
+    def content_sha256(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "content_sha256", value)
 
     @property
     @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        The path of the group.
-        """
-        return pulumi.get(self, "path")
-
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
-
-    @property
-    @pulumi.getter(name="preventForkingOutsideGroup")
-    def prevent_forking_outside_group(self) -> Optional[pulumi.Input[bool]]:
+    def encoding(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
+        The file content encoding.
         """
-        return pulumi.get(self, "prevent_forking_outside_group")
+        return pulumi.get(self, "encoding")
 
-    @prevent_forking_outside_group.setter
-    def prevent_forking_outside_group(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "prevent_forking_outside_group", value)
+    @encoding.setter
+    def encoding(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "encoding", value)
 
     @property
-    @pulumi.getter(name="projectCreationLevel")
-    def project_creation_level(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="executeFilemode")
+    def execute_filemode(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defaults to maintainer. Determine if developers can create projects in the group.
+        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         """
-        return pulumi.get(self, "project_creation_level")
+        return pulumi.get(self, "execute_filemode")
 
-    @project_creation_level.setter
-    def project_creation_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project_creation_level", value)
+    @execute_filemode.setter
+    def execute_filemode(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "execute_filemode", value)
 
     @property
-    @pulumi.getter(name="requestAccessEnabled")
-    def request_access_enabled(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="fileName")
+    def file_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. Allow users to request member access.
+        The filename.
         """
-        return pulumi.get(self, "request_access_enabled")
+        return pulumi.get(self, "file_name")
 
-    @request_access_enabled.setter
-    def request_access_enabled(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "request_access_enabled", value)
+    @file_name.setter
+    def file_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "file_name", value)
 
     @property
-    @pulumi.getter(name="requireTwoFactorAuthentication")
-    def require_two_factor_authentication(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="filePath")
+    def file_path(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to false. Require all users in this group to setup Two-factor authentication.
+        The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         """
-        return pulumi.get(self, "require_two_factor_authentication")
+        return pulumi.get(self, "file_path")
 
-    @require_two_factor_authentication.setter
-    def require_two_factor_authentication(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "require_two_factor_authentication", value)
+    @file_path.setter
+    def file_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "file_path", value)
 
     @property
-    @pulumi.getter(name="runnersToken")
-    def runners_token(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="lastCommitId")
+    def last_commit_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The group level registration token to use during runner setup.
+        The last known commit id.
         """
-        return pulumi.get(self, "runners_token")
+        return pulumi.get(self, "last_commit_id")
 
-    @runners_token.setter
-    def runners_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "runners_token", value)
+    @last_commit_id.setter
+    def last_commit_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "last_commit_id", value)
 
     @property
-    @pulumi.getter(name="shareWithGroupLock")
-    def share_with_group_lock(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="overwriteOnCreate")
+    def overwrite_on_create(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defaults to false. Prevent sharing a project with another group within this group.
+        Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
         """
-        return pulumi.get(self, "share_with_group_lock")
+        return pulumi.get(self, "overwrite_on_create")
 
-    @share_with_group_lock.setter
-    def share_with_group_lock(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "share_with_group_lock", value)
+    @overwrite_on_create.setter
+    def overwrite_on_create(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "overwrite_on_create", value)
 
     @property
-    @pulumi.getter(name="subgroupCreationLevel")
-    def subgroup_creation_level(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def project(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to owner. Allowed to create subgroups.
+        The name or ID of the project.
         """
-        return pulumi.get(self, "subgroup_creation_level")
+        return pulumi.get(self, "project")
 
-    @subgroup_creation_level.setter
-    def subgroup_creation_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "subgroup_creation_level", value)
+    @project.setter
+    def project(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "project", value)
 
     @property
-    @pulumi.getter(name="twoFactorGracePeriod")
-    def two_factor_grace_period(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def ref(self) -> Optional[pulumi.Input[str]]:
         """
-        Defaults to 48. Time before Two-factor authentication is enforced (in hours).
+        The name of branch, tag or commit.
         """
-        return pulumi.get(self, "two_factor_grace_period")
+        return pulumi.get(self, "ref")
 
-    @two_factor_grace_period.setter
-    def two_factor_grace_period(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "two_factor_grace_period", value)
+    @ref.setter
+    def ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ref", value)
 
     @property
-    @pulumi.getter(name="visibilityLevel")
-    def visibility_level(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def size(self) -> Optional[pulumi.Input[int]]:
         """
-        The group's visibility. Can be `private`, `internal`, or `public`.
+        The file size.
         """
-        return pulumi.get(self, "visibility_level")
+        return pulumi.get(self, "size")
 
-    @visibility_level.setter
-    def visibility_level(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "visibility_level", value)
+    @size.setter
+    def size(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "size", value)
 
     @property
-    @pulumi.getter(name="webUrl")
-    def web_url(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="startBranch")
+    def start_branch(self) -> Optional[pulumi.Input[str]]:
         """
-        Web URL of the group.
+        Name of the branch to start the new commit from.
         """
-        return pulumi.get(self, "web_url")
+        return pulumi.get(self, "start_branch")
 
-    @web_url.setter
-    def web_url(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "web_url", value)
+    @start_branch.setter
+    def start_branch(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "start_branch", value)
 
 
-class Group(pulumi.CustomResource):
+class RepositoryFile(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
-                 default_branch_protection: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 emails_disabled: Optional[pulumi.Input[bool]] = None,
-                 lfs_enabled: Optional[pulumi.Input[bool]] = None,
-                 mentions_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 parent_id: Optional[pulumi.Input[int]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 prevent_forking_outside_group: Optional[pulumi.Input[bool]] = None,
-                 project_creation_level: Optional[pulumi.Input[str]] = None,
-                 request_access_enabled: Optional[pulumi.Input[bool]] = None,
-                 require_two_factor_authentication: Optional[pulumi.Input[bool]] = None,
-                 share_with_group_lock: Optional[pulumi.Input[bool]] = None,
-                 subgroup_creation_level: Optional[pulumi.Input[str]] = None,
-                 two_factor_grace_period: Optional[pulumi.Input[int]] = None,
-                 visibility_level: Optional[pulumi.Input[str]] = None,
+                 author_email: Optional[pulumi.Input[str]] = None,
+                 author_name: Optional[pulumi.Input[str]] = None,
+                 branch: Optional[pulumi.Input[str]] = None,
+                 commit_message: Optional[pulumi.Input[str]] = None,
+                 content: Optional[pulumi.Input[str]] = None,
+                 execute_filemode: Optional[pulumi.Input[bool]] = None,
+                 file_path: Optional[pulumi.Input[str]] = None,
+                 overwrite_on_create: Optional[pulumi.Input[bool]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 start_branch: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `Group` resource allows to manage the lifecycle of a group.
-
-        > On GitLab SaaS, you must use the GitLab UI to create groups without a parent group. You cannot use this provider nor the API to do this.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html)
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_group = gitlab.Group("exampleGroup",
-            path="example",
-            description="An example group")
-        # Create a project in the example group
-        example_project = gitlab.Project("exampleProject",
-            description="An example project",
-            namespace_id=example_group.id)
-        ```
-
         ## Import
 
-        ```sh
-         $ pulumi import gitlab:index/group:Group You can import a group state using `<resource> <id>`. The
-        ```
-
-         `id` can be whatever the [details of a group][details_of_a_group] api takes for its `:id` value, so for example
+        A Repository File can be imported using an id made up of `<project-id>:<branch-name>:<file-path>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/group:Group example example
+         $ pulumi import gitlab:index/repositoryFile:RepositoryFile this 1:main:foo/bar.txt
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] auto_devops_enabled: Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        :param pulumi.Input[int] default_branch_protection: Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        :param pulumi.Input[str] description: The description of the group.
-        :param pulumi.Input[bool] emails_disabled: Defaults to false. Disable email notifications.
-        :param pulumi.Input[bool] lfs_enabled: Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
-        :param pulumi.Input[bool] mentions_disabled: Defaults to false. Disable the capability of a group from getting mentioned.
-        :param pulumi.Input[str] name: The name of this group.
-        :param pulumi.Input[int] parent_id: Id of the parent group (creates a nested group).
-        :param pulumi.Input[str] path: The path of the group.
-        :param pulumi.Input[bool] prevent_forking_outside_group: Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
-        :param pulumi.Input[str] project_creation_level: Defaults to maintainer. Determine if developers can create projects in the group.
-        :param pulumi.Input[bool] request_access_enabled: Defaults to false. Allow users to request member access.
-        :param pulumi.Input[bool] require_two_factor_authentication: Defaults to false. Require all users in this group to setup Two-factor authentication.
-        :param pulumi.Input[bool] share_with_group_lock: Defaults to false. Prevent sharing a project with another group within this group.
-        :param pulumi.Input[str] subgroup_creation_level: Defaults to owner. Allowed to create subgroups.
-        :param pulumi.Input[int] two_factor_grace_period: Defaults to 48. Time before Two-factor authentication is enforced (in hours).
-        :param pulumi.Input[str] visibility_level: The group's visibility. Can be `private`, `internal`, or `public`.
+        :param pulumi.Input[str] author_email: Email of the commit author.
+        :param pulumi.Input[str] author_name: Name of the commit author.
+        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
+        :param pulumi.Input[str] commit_message: Commit message.
+        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+        :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
+        :param pulumi.Input[str] project: The name or ID of the project.
+        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: GroupArgs,
+                 args: RepositoryFileArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `Group` resource allows to manage the lifecycle of a group.
-
-        > On GitLab SaaS, you must use the GitLab UI to create groups without a parent group. You cannot use this provider nor the API to do this.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html)
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_group = gitlab.Group("exampleGroup",
-            path="example",
-            description="An example group")
-        # Create a project in the example group
-        example_project = gitlab.Project("exampleProject",
-            description="An example project",
-            namespace_id=example_group.id)
-        ```
-
         ## Import
 
-        ```sh
-         $ pulumi import gitlab:index/group:Group You can import a group state using `<resource> <id>`. The
-        ```
-
-         `id` can be whatever the [details of a group][details_of_a_group] api takes for its `:id` value, so for example
+        A Repository File can be imported using an id made up of `<project-id>:<branch-name>:<file-path>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/group:Group example example
+         $ pulumi import gitlab:index/repositoryFile:RepositoryFile this 1:main:foo/bar.txt
         ```
 
         :param str resource_name: The name of the resource.
-        :param GroupArgs args: The arguments to use to populate this resource's properties.
+        :param RepositoryFileArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(GroupArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(RepositoryFileArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
-                 default_branch_protection: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 emails_disabled: Optional[pulumi.Input[bool]] = None,
-                 lfs_enabled: Optional[pulumi.Input[bool]] = None,
-                 mentions_disabled: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 parent_id: Optional[pulumi.Input[int]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 prevent_forking_outside_group: Optional[pulumi.Input[bool]] = None,
-                 project_creation_level: Optional[pulumi.Input[str]] = None,
-                 request_access_enabled: Optional[pulumi.Input[bool]] = None,
-                 require_two_factor_authentication: Optional[pulumi.Input[bool]] = None,
-                 share_with_group_lock: Optional[pulumi.Input[bool]] = None,
-                 subgroup_creation_level: Optional[pulumi.Input[str]] = None,
-                 two_factor_grace_period: Optional[pulumi.Input[int]] = None,
-                 visibility_level: Optional[pulumi.Input[str]] = None,
+                 author_email: Optional[pulumi.Input[str]] = None,
+                 author_name: Optional[pulumi.Input[str]] = None,
+                 branch: Optional[pulumi.Input[str]] = None,
+                 commit_message: Optional[pulumi.Input[str]] = None,
+                 content: Optional[pulumi.Input[str]] = None,
+                 execute_filemode: Optional[pulumi.Input[bool]] = None,
+                 file_path: Optional[pulumi.Input[str]] = None,
+                 overwrite_on_create: Optional[pulumi.Input[bool]] = None,
+                 project: Optional[pulumi.Input[str]] = None,
+                 start_branch: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = GroupArgs.__new__(GroupArgs)
+            __props__ = RepositoryFileArgs.__new__(RepositoryFileArgs)
 
-            __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
-            __props__.__dict__["default_branch_protection"] = default_branch_protection
-            __props__.__dict__["description"] = description
-            __props__.__dict__["emails_disabled"] = emails_disabled
-            __props__.__dict__["lfs_enabled"] = lfs_enabled
-            __props__.__dict__["mentions_disabled"] = mentions_disabled
-            __props__.__dict__["name"] = name
-            __props__.__dict__["parent_id"] = parent_id
-            if path is None and not opts.urn:
-                raise TypeError("Missing required property 'path'")
-            __props__.__dict__["path"] = path
-            __props__.__dict__["prevent_forking_outside_group"] = prevent_forking_outside_group
-            __props__.__dict__["project_creation_level"] = project_creation_level
-            __props__.__dict__["request_access_enabled"] = request_access_enabled
-            __props__.__dict__["require_two_factor_authentication"] = require_two_factor_authentication
-            __props__.__dict__["share_with_group_lock"] = share_with_group_lock
-            __props__.__dict__["subgroup_creation_level"] = subgroup_creation_level
-            __props__.__dict__["two_factor_grace_period"] = two_factor_grace_period
-            __props__.__dict__["visibility_level"] = visibility_level
-            __props__.__dict__["full_name"] = None
-            __props__.__dict__["full_path"] = None
-            __props__.__dict__["runners_token"] = None
-            __props__.__dict__["web_url"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["runnersToken"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(Group, __self__).__init__(
-            'gitlab:index/group:Group',
+            __props__.__dict__["author_email"] = author_email
+            __props__.__dict__["author_name"] = author_name
+            if branch is None and not opts.urn:
+                raise TypeError("Missing required property 'branch'")
+            __props__.__dict__["branch"] = branch
+            if commit_message is None and not opts.urn:
+                raise TypeError("Missing required property 'commit_message'")
+            __props__.__dict__["commit_message"] = commit_message
+            if content is None and not opts.urn:
+                raise TypeError("Missing required property 'content'")
+            __props__.__dict__["content"] = content
+            __props__.__dict__["execute_filemode"] = execute_filemode
+            if file_path is None and not opts.urn:
+                raise TypeError("Missing required property 'file_path'")
+            __props__.__dict__["file_path"] = file_path
+            __props__.__dict__["overwrite_on_create"] = overwrite_on_create
+            if project is None and not opts.urn:
+                raise TypeError("Missing required property 'project'")
+            __props__.__dict__["project"] = project
+            __props__.__dict__["start_branch"] = start_branch
+            __props__.__dict__["blob_id"] = None
+            __props__.__dict__["commit_id"] = None
+            __props__.__dict__["content_sha256"] = None
+            __props__.__dict__["encoding"] = None
+            __props__.__dict__["file_name"] = None
+            __props__.__dict__["last_commit_id"] = None
+            __props__.__dict__["ref"] = None
+            __props__.__dict__["size"] = None
+        super(RepositoryFile, __self__).__init__(
+            'gitlab:index/repositoryFile:RepositoryFile',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
-            default_branch_protection: Optional[pulumi.Input[int]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            emails_disabled: Optional[pulumi.Input[bool]] = None,
-            full_name: Optional[pulumi.Input[str]] = None,
-            full_path: Optional[pulumi.Input[str]] = None,
-            lfs_enabled: Optional[pulumi.Input[bool]] = None,
-            mentions_disabled: Optional[pulumi.Input[bool]] = None,
-            name: Optional[pulumi.Input[str]] = None,
-            parent_id: Optional[pulumi.Input[int]] = None,
-            path: Optional[pulumi.Input[str]] = None,
-            prevent_forking_outside_group: Optional[pulumi.Input[bool]] = None,
-            project_creation_level: Optional[pulumi.Input[str]] = None,
-            request_access_enabled: Optional[pulumi.Input[bool]] = None,
-            require_two_factor_authentication: Optional[pulumi.Input[bool]] = None,
-            runners_token: Optional[pulumi.Input[str]] = None,
-            share_with_group_lock: Optional[pulumi.Input[bool]] = None,
-            subgroup_creation_level: Optional[pulumi.Input[str]] = None,
-            two_factor_grace_period: Optional[pulumi.Input[int]] = None,
-            visibility_level: Optional[pulumi.Input[str]] = None,
-            web_url: Optional[pulumi.Input[str]] = None) -> 'Group':
+            author_email: Optional[pulumi.Input[str]] = None,
+            author_name: Optional[pulumi.Input[str]] = None,
+            blob_id: Optional[pulumi.Input[str]] = None,
+            branch: Optional[pulumi.Input[str]] = None,
+            commit_id: Optional[pulumi.Input[str]] = None,
+            commit_message: Optional[pulumi.Input[str]] = None,
+            content: Optional[pulumi.Input[str]] = None,
+            content_sha256: Optional[pulumi.Input[str]] = None,
+            encoding: Optional[pulumi.Input[str]] = None,
+            execute_filemode: Optional[pulumi.Input[bool]] = None,
+            file_name: Optional[pulumi.Input[str]] = None,
+            file_path: Optional[pulumi.Input[str]] = None,
+            last_commit_id: Optional[pulumi.Input[str]] = None,
+            overwrite_on_create: Optional[pulumi.Input[bool]] = None,
+            project: Optional[pulumi.Input[str]] = None,
+            ref: Optional[pulumi.Input[str]] = None,
+            size: Optional[pulumi.Input[int]] = None,
+            start_branch: Optional[pulumi.Input[str]] = None) -> 'RepositoryFile':
         """
-        Get an existing Group resource's state with the given name, id, and optional extra
+        Get an existing RepositoryFile resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] auto_devops_enabled: Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        :param pulumi.Input[int] default_branch_protection: Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        :param pulumi.Input[str] description: The description of the group.
-        :param pulumi.Input[bool] emails_disabled: Defaults to false. Disable email notifications.
-        :param pulumi.Input[str] full_name: The full name of the group.
-        :param pulumi.Input[str] full_path: The full path of the group.
-        :param pulumi.Input[bool] lfs_enabled: Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
-        :param pulumi.Input[bool] mentions_disabled: Defaults to false. Disable the capability of a group from getting mentioned.
-        :param pulumi.Input[str] name: The name of this group.
-        :param pulumi.Input[int] parent_id: Id of the parent group (creates a nested group).
-        :param pulumi.Input[str] path: The path of the group.
-        :param pulumi.Input[bool] prevent_forking_outside_group: Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
-        :param pulumi.Input[str] project_creation_level: Defaults to maintainer. Determine if developers can create projects in the group.
-        :param pulumi.Input[bool] request_access_enabled: Defaults to false. Allow users to request member access.
-        :param pulumi.Input[bool] require_two_factor_authentication: Defaults to false. Require all users in this group to setup Two-factor authentication.
-        :param pulumi.Input[str] runners_token: The group level registration token to use during runner setup.
-        :param pulumi.Input[bool] share_with_group_lock: Defaults to false. Prevent sharing a project with another group within this group.
-        :param pulumi.Input[str] subgroup_creation_level: Defaults to owner. Allowed to create subgroups.
-        :param pulumi.Input[int] two_factor_grace_period: Defaults to 48. Time before Two-factor authentication is enforced (in hours).
-        :param pulumi.Input[str] visibility_level: The group's visibility. Can be `private`, `internal`, or `public`.
-        :param pulumi.Input[str] web_url: Web URL of the group.
+        :param pulumi.Input[str] author_email: Email of the commit author.
+        :param pulumi.Input[str] author_name: Name of the commit author.
+        :param pulumi.Input[str] blob_id: The blob id.
+        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
+        :param pulumi.Input[str] commit_id: The commit id.
+        :param pulumi.Input[str] commit_message: Commit message.
+        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        :param pulumi.Input[str] content_sha256: File content sha256 digest.
+        :param pulumi.Input[str] encoding: The file content encoding.
+        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        :param pulumi.Input[str] file_name: The filename.
+        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
+        :param pulumi.Input[str] last_commit_id: The last known commit id.
+        :param pulumi.Input[bool] overwrite_on_create: Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
+        :param pulumi.Input[str] project: The name or ID of the project.
+        :param pulumi.Input[str] ref: The name of branch, tag or commit.
+        :param pulumi.Input[int] size: The file size.
+        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _GroupState.__new__(_GroupState)
+        __props__ = _RepositoryFileState.__new__(_RepositoryFileState)
 
-        __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
-        __props__.__dict__["default_branch_protection"] = default_branch_protection
-        __props__.__dict__["description"] = description
-        __props__.__dict__["emails_disabled"] = emails_disabled
-        __props__.__dict__["full_name"] = full_name
-        __props__.__dict__["full_path"] = full_path
-        __props__.__dict__["lfs_enabled"] = lfs_enabled
-        __props__.__dict__["mentions_disabled"] = mentions_disabled
-        __props__.__dict__["name"] = name
-        __props__.__dict__["parent_id"] = parent_id
-        __props__.__dict__["path"] = path
-        __props__.__dict__["prevent_forking_outside_group"] = prevent_forking_outside_group
-        __props__.__dict__["project_creation_level"] = project_creation_level
-        __props__.__dict__["request_access_enabled"] = request_access_enabled
-        __props__.__dict__["require_two_factor_authentication"] = require_two_factor_authentication
-        __props__.__dict__["runners_token"] = runners_token
-        __props__.__dict__["share_with_group_lock"] = share_with_group_lock
-        __props__.__dict__["subgroup_creation_level"] = subgroup_creation_level
-        __props__.__dict__["two_factor_grace_period"] = two_factor_grace_period
-        __props__.__dict__["visibility_level"] = visibility_level
-        __props__.__dict__["web_url"] = web_url
-        return Group(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="autoDevopsEnabled")
-    def auto_devops_enabled(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Defaults to false. Default to Auto DevOps pipeline for all projects within this group.
-        """
-        return pulumi.get(self, "auto_devops_enabled")
-
-    @property
-    @pulumi.getter(name="defaultBranchProtection")
-    def default_branch_protection(self) -> pulumi.Output[Optional[int]]:
-        """
-        Defaults to 2. See https://docs.gitlab.com/ee/api/groups.html#options-for-default*branch*protection
-        """
-        return pulumi.get(self, "default_branch_protection")
+        __props__.__dict__["author_email"] = author_email
+        __props__.__dict__["author_name"] = author_name
+        __props__.__dict__["blob_id"] = blob_id
+        __props__.__dict__["branch"] = branch
+        __props__.__dict__["commit_id"] = commit_id
+        __props__.__dict__["commit_message"] = commit_message
+        __props__.__dict__["content"] = content
+        __props__.__dict__["content_sha256"] = content_sha256
+        __props__.__dict__["encoding"] = encoding
+        __props__.__dict__["execute_filemode"] = execute_filemode
+        __props__.__dict__["file_name"] = file_name
+        __props__.__dict__["file_path"] = file_path
+        __props__.__dict__["last_commit_id"] = last_commit_id
+        __props__.__dict__["overwrite_on_create"] = overwrite_on_create
+        __props__.__dict__["project"] = project
+        __props__.__dict__["ref"] = ref
+        __props__.__dict__["size"] = size
+        __props__.__dict__["start_branch"] = start_branch
+        return RepositoryFile(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="authorEmail")
+    def author_email(self) -> pulumi.Output[Optional[str]]:
         """
-        The description of the group.
+        Email of the commit author.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "author_email")
 
     @property
-    @pulumi.getter(name="emailsDisabled")
-    def emails_disabled(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="authorName")
+    def author_name(self) -> pulumi.Output[Optional[str]]:
         """
-        Defaults to false. Disable email notifications.
+        Name of the commit author.
         """
-        return pulumi.get(self, "emails_disabled")
+        return pulumi.get(self, "author_name")
 
     @property
-    @pulumi.getter(name="fullName")
-    def full_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="blobId")
+    def blob_id(self) -> pulumi.Output[str]:
         """
-        The full name of the group.
+        The blob id.
         """
-        return pulumi.get(self, "full_name")
+        return pulumi.get(self, "blob_id")
 
     @property
-    @pulumi.getter(name="fullPath")
-    def full_path(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def branch(self) -> pulumi.Output[str]:
         """
-        The full path of the group.
+        Name of the branch to which to commit to.
         """
-        return pulumi.get(self, "full_path")
+        return pulumi.get(self, "branch")
 
     @property
-    @pulumi.getter(name="lfsEnabled")
-    def lfs_enabled(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="commitId")
+    def commit_id(self) -> pulumi.Output[str]:
         """
-        Defaults to true. Enable/disable Large File Storage (LFS) for the projects in this group.
+        The commit id.
         """
-        return pulumi.get(self, "lfs_enabled")
+        return pulumi.get(self, "commit_id")
 
     @property
-    @pulumi.getter(name="mentionsDisabled")
-    def mentions_disabled(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="commitMessage")
+    def commit_message(self) -> pulumi.Output[str]:
         """
-        Defaults to false. Disable the capability of a group from getting mentioned.
+        Commit message.
         """
-        return pulumi.get(self, "mentions_disabled")
+        return pulumi.get(self, "commit_message")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def content(self) -> pulumi.Output[str]:
         """
-        The name of this group.
+        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "content")
 
     @property
-    @pulumi.getter(name="parentId")
-    def parent_id(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="contentSha256")
+    def content_sha256(self) -> pulumi.Output[str]:
         """
-        Id of the parent group (creates a nested group).
+        File content sha256 digest.
         """
-        return pulumi.get(self, "parent_id")
+        return pulumi.get(self, "content_sha256")
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Output[str]:
+    def encoding(self) -> pulumi.Output[str]:
         """
-        The path of the group.
+        The file content encoding.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "encoding")
 
     @property
-    @pulumi.getter(name="preventForkingOutsideGroup")
-    def prevent_forking_outside_group(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="executeFilemode")
+    def execute_filemode(self) -> pulumi.Output[Optional[bool]]:
         """
-        Defaults to false. When enabled, users can not fork projects from this group to external namespaces.
+        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
         """
-        return pulumi.get(self, "prevent_forking_outside_group")
+        return pulumi.get(self, "execute_filemode")
 
     @property
-    @pulumi.getter(name="projectCreationLevel")
-    def project_creation_level(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="fileName")
+    def file_name(self) -> pulumi.Output[str]:
         """
-        Defaults to maintainer. Determine if developers can create projects in the group.
+        The filename.
         """
-        return pulumi.get(self, "project_creation_level")
+        return pulumi.get(self, "file_name")
 
     @property
-    @pulumi.getter(name="requestAccessEnabled")
-    def request_access_enabled(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="filePath")
+    def file_path(self) -> pulumi.Output[str]:
         """
-        Defaults to false. Allow users to request member access.
+        The full path of the file. It must be relative to the root of the project without a leading slash `/` or `./`.
         """
-        return pulumi.get(self, "request_access_enabled")
+        return pulumi.get(self, "file_path")
 
     @property
-    @pulumi.getter(name="requireTwoFactorAuthentication")
-    def require_two_factor_authentication(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="lastCommitId")
+    def last_commit_id(self) -> pulumi.Output[str]:
         """
-        Defaults to false. Require all users in this group to setup Two-factor authentication.
+        The last known commit id.
         """
-        return pulumi.get(self, "require_two_factor_authentication")
+        return pulumi.get(self, "last_commit_id")
 
     @property
-    @pulumi.getter(name="runnersToken")
-    def runners_token(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="overwriteOnCreate")
+    def overwrite_on_create(self) -> pulumi.Output[Optional[bool]]:
         """
-        The group level registration token to use during runner setup.
+        Enable overwriting existing files, defaults to `false`. This attribute is only used during `create` and must be use carefully. We suggest to use `imports` whenever possible and limit the use of this attribute for when the project was imported on the same `apply`. This attribute is not supported during a resource import.
         """
-        return pulumi.get(self, "runners_token")
+        return pulumi.get(self, "overwrite_on_create")
 
     @property
-    @pulumi.getter(name="shareWithGroupLock")
-    def share_with_group_lock(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Defaults to false. Prevent sharing a project with another group within this group.
-        """
-        return pulumi.get(self, "share_with_group_lock")
-
-    @property
-    @pulumi.getter(name="subgroupCreationLevel")
-    def subgroup_creation_level(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def project(self) -> pulumi.Output[str]:
         """
-        Defaults to owner. Allowed to create subgroups.
+        The name or ID of the project.
         """
-        return pulumi.get(self, "subgroup_creation_level")
+        return pulumi.get(self, "project")
 
     @property
-    @pulumi.getter(name="twoFactorGracePeriod")
-    def two_factor_grace_period(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def ref(self) -> pulumi.Output[str]:
         """
-        Defaults to 48. Time before Two-factor authentication is enforced (in hours).
+        The name of branch, tag or commit.
         """
-        return pulumi.get(self, "two_factor_grace_period")
+        return pulumi.get(self, "ref")
 
     @property
-    @pulumi.getter(name="visibilityLevel")
-    def visibility_level(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def size(self) -> pulumi.Output[int]:
         """
-        The group's visibility. Can be `private`, `internal`, or `public`.
+        The file size.
         """
-        return pulumi.get(self, "visibility_level")
+        return pulumi.get(self, "size")
 
     @property
-    @pulumi.getter(name="webUrl")
-    def web_url(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="startBranch")
+    def start_branch(self) -> pulumi.Output[Optional[str]]:
         """
-        Web URL of the group.
+        Name of the branch to start the new commit from.
         """
-        return pulumi.get(self, "web_url")
+        return pulumi.get(self, "start_branch")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_label.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_ldap_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_membership.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
                  expires_at: Optional[pulumi.Input[str]] = None,
                  group_id: Optional[pulumi.Input[str]] = None,
                  skip_subresources_on_destroy: Optional[pulumi.Input[bool]] = None,
                  unassign_issuables_on_destroy: Optional[pulumi.Input[bool]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        The `GroupMembership` resource allows to manage the lifecycle of a users group membersip.
+        The `GroupMembership` resource allows to manage the lifecycle of a users group membership.
 
         > If a group should grant membership to another group use the `GroupShareGroup` resource instead.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html)
 
         ## Example Usage
 
@@ -268,15 +268,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupMembershipArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `GroupMembership` resource allows to manage the lifecycle of a users group membersip.
+        The `GroupMembership` resource allows to manage the lifecycle of a users group membership.
 
         > If a group should grant membership to another group use the `GroupShareGroup` resource instead.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html)
 
         ## Example Usage
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_project_file_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,32 @@
         For more information about which file types are available as templates, view
         [GitLab's documentation](https://docs.gitlab.com/ee/user/group/custom_project_templates.html)
 
         > This resource requires a GitLab Enterprise instance with a Premium license.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#update-group)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        foo = gitlab.Group("foo",
+            path="group",
+            description="An example group")
+        bar = gitlab.Project("bar",
+            description="contains file templates",
+            visibility_level="public",
+            namespace_id=foo.id)
+        template_link = gitlab.GroupProjectFileTemplate("templateLink",
+            group_id=foo.id,
+            file_template_project_id=bar.id)
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] file_template_project_id: The ID of the project that will be used for file templates. This project must be the direct
                			child of the project defined by the group_id
         :param pulumi.Input[int] group_id: The ID of the group that will use the file template project. This group must be the direct
                            parent of the project defined by project_id
         """
@@ -136,14 +154,32 @@
         For more information about which file types are available as templates, view
         [GitLab's documentation](https://docs.gitlab.com/ee/user/group/custom_project_templates.html)
 
         > This resource requires a GitLab Enterprise instance with a Premium license.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#update-group)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        foo = gitlab.Group("foo",
+            path="group",
+            description="An example group")
+        bar = gitlab.Project("bar",
+            description="contains file templates",
+            visibility_level="public",
+            namespace_id=foo.id)
+        template_link = gitlab.GroupProjectFileTemplate("templateLink",
+            group_id=foo.id,
+            file_template_project_id=bar.id)
+        ```
+
         :param str resource_name: The name of the resource.
         :param GroupProjectFileTemplateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(GroupProjectFileTemplateArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_saml_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,26 @@
                  saml_group_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `GroupSamlLink` resource allows to manage the lifecycle of an SAML integration with a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#saml-group-links)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        test = gitlab.GroupSamlLink("test",
+            access_level="developer",
+            group="12345",
+            saml_group_name="samlgroupname1")
+        ```
+
         ## Import
 
         GitLab group saml links can be imported using an id made up of `group_id:saml_group_name`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/groupSamlLink:GroupSamlLink test "12345:samlgroupname1"
         ```
@@ -155,14 +167,26 @@
                  args: GroupSamlLinkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `GroupSamlLink` resource allows to manage the lifecycle of an SAML integration with a group.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/groups.html#saml-group-links)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        test = gitlab.GroupSamlLink("test",
+            access_level="developer",
+            group="12345",
+            saml_group_name="samlgroupname1")
+        ```
+
         ## Import
 
         GitLab group saml links can be imported using an id made up of `group_id:saml_group_name`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/groupSamlLink:GroupSamlLink test "12345:samlgroupname1"
         ```
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/label.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/managed_license.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/managed_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/outputs.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,46 +22,52 @@
     'ProjectPushRules',
     'ProjectTagCommit',
     'ProjectTagRelease',
     'GetBranchCommitResult',
     'GetClusterAgentsClusterAgentResult',
     'GetGroupHooksHookResult',
     'GetGroupMembershipMemberResult',
+    'GetGroupSubgroupsSubgroupResult',
     'GetGroupVariablesVariableResult',
+    'GetGroupsGroupResult',
     'GetInstanceDeployKeysDeployKeyResult',
     'GetInstanceDeployKeysDeployKeyProjectsWithWriteAccessResult',
     'GetInstanceVariablesVariableResult',
+    'GetMetadataKasResult',
+    'GetProjectBranchesBranchResult',
+    'GetProjectBranchesBranchCommitResult',
     'GetProjectContainerExpirationPolicyResult',
     'GetProjectHooksHookResult',
     'GetProjectIssueTaskCompletionStatusResult',
     'GetProjectIssuesIssueResult',
     'GetProjectIssuesIssueTaskCompletionStatusResult',
     'GetProjectMembershipMemberResult',
     'GetProjectMilestonesMilestoneResult',
     'GetProjectProtectedBranchMergeAccessLevelResult',
     'GetProjectProtectedBranchPushAccessLevelResult',
     'GetProjectProtectedBranchesProtectedBranchResult',
     'GetProjectProtectedBranchesProtectedBranchMergeAccessLevelResult',
     'GetProjectProtectedBranchesProtectedBranchPushAccessLevelResult',
-    'GetProjectPushRulesResult',
+    'GetProjectPushRuleResult',
     'GetProjectTagCommitResult',
     'GetProjectTagReleaseResult',
     'GetProjectTagsTagResult',
     'GetProjectTagsTagCommitResult',
     'GetProjectTagsTagReleaseResult',
     'GetProjectVariablesVariableResult',
     'GetProjectsProjectResult',
     'GetProjectsProjectContainerExpirationPolicyResult',
     'GetProjectsProjectForkedFromProjectResult',
     'GetProjectsProjectNamespaceResult',
     'GetProjectsProjectOwnerResult',
-    'GetProjectsProjectPermissionsResult',
+    'GetProjectsProjectPermissionResult',
     'GetProjectsProjectSharedWithGroupResult',
     'GetReleaseLinksReleaseLinkResult',
     'GetRepositoryTreeTreeResult',
+    'GetUserSshkeysKeyResult',
     'GetUsersUserResult',
 ]
 
 @pulumi.output_type
 class BranchCommit(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -428,14 +434,16 @@
 @pulumi.output_type
 class ProjectContainerExpirationPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "keepN":
             suggest = "keep_n"
+        elif key == "nameRegex":
+            suggest = "name_regex"
         elif key == "nameRegexDelete":
             suggest = "name_regex_delete"
         elif key == "nameRegexKeep":
             suggest = "name_regex_keep"
         elif key == "nextRunAt":
             suggest = "next_run_at"
         elif key == "olderThan":
@@ -452,33 +460,37 @@
         ProjectContainerExpirationPolicy.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cadence: Optional[str] = None,
                  enabled: Optional[bool] = None,
                  keep_n: Optional[int] = None,
+                 name_regex: Optional[str] = None,
                  name_regex_delete: Optional[str] = None,
                  name_regex_keep: Optional[str] = None,
                  next_run_at: Optional[str] = None,
                  older_than: Optional[str] = None):
         """
         :param str cadence: The cadence of the policy. Valid values are: `1d`, `7d`, `14d`, `1month`, `3month`.
         :param bool enabled: If true, the policy is enabled.
         :param int keep_n: The number of images to keep.
-        :param str name_regex_delete: The regular expression to match image names to delete. **Note**: the upstream API has some inconsistencies with the `name_regex` field here. It's basically unusable at the moment.
+        :param str name_regex: The regular expression to match image names to delete.
+        :param str name_regex_delete: The regular expression to match image names to delete.
         :param str name_regex_keep: The regular expression to match image names to keep.
         :param str next_run_at: The next time the policy will run.
         :param str older_than: The number of days to keep images.
         """
         if cadence is not None:
             pulumi.set(__self__, "cadence", cadence)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if keep_n is not None:
             pulumi.set(__self__, "keep_n", keep_n)
+        if name_regex is not None:
+            pulumi.set(__self__, "name_regex", name_regex)
         if name_regex_delete is not None:
             pulumi.set(__self__, "name_regex_delete", name_regex_delete)
         if name_regex_keep is not None:
             pulumi.set(__self__, "name_regex_keep", name_regex_keep)
         if next_run_at is not None:
             pulumi.set(__self__, "next_run_at", next_run_at)
         if older_than is not None:
@@ -505,18 +517,26 @@
     def keep_n(self) -> Optional[int]:
         """
         The number of images to keep.
         """
         return pulumi.get(self, "keep_n")
 
     @property
+    @pulumi.getter(name="nameRegex")
+    def name_regex(self) -> Optional[str]:
+        """
+        The regular expression to match image names to delete.
+        """
+        return pulumi.get(self, "name_regex")
+
+    @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> Optional[str]:
         """
-        The regular expression to match image names to delete. **Note**: the upstream API has some inconsistencies with the `name_regex` field here. It's basically unusable at the moment.
+        The regular expression to match image names to delete.
         """
         return pulumi.get(self, "name_regex_delete")
 
     @property
     @pulumi.getter(name="nameRegexKeep")
     def name_regex_keep(self) -> Optional[str]:
         """
@@ -813,15 +833,15 @@
         """
         :param str author_email_regex: All commit author emails must match this regex, e.g. `@my-company.com$`.
         :param str branch_name_regex: All branch names must match this regex, e.g. `(feature|hotfix)\\/*`.
         :param bool commit_committer_check: Users can only push commits to this repository that were committed with one of their own verified emails.
         :param str commit_message_negative_regex: No commit message is allowed to match this regex, for example `ssh\\:\\/\\/`.
         :param str commit_message_regex: All commit messages must match this regex, e.g. `Fixed \\d+\\..*`.
         :param bool deny_delete_tag: Deny deleting a tag.
-        :param str file_name_regex: All commited filenames must not match this regex, e.g. `(jar|exe)$`.
+        :param str file_name_regex: All committed filenames must not match this regex, e.g. `(jar|exe)$`.
         :param int max_file_size: Maximum file size (MB).
         :param bool member_check: Restrict commits by author (email) to existing GitLab users.
         :param bool prevent_secrets: GitLab will reject any files that are likely to contain secrets.
         :param bool reject_unsigned_commits: Reject commit when it’s not signed through GPG.
         """
         if author_email_regex is not None:
             pulumi.set(__self__, "author_email_regex", author_email_regex)
@@ -894,15 +914,15 @@
         """
         return pulumi.get(self, "deny_delete_tag")
 
     @property
     @pulumi.getter(name="fileNameRegex")
     def file_name_regex(self) -> Optional[str]:
         """
-        All commited filenames must not match this regex, e.g. `(jar|exe)$`.
+        All committed filenames must not match this regex, e.g. `(jar|exe)$`.
         """
         return pulumi.get(self, "file_name_regex")
 
     @property
     @pulumi.getter(name="maxFileSize")
     def max_file_size(self) -> Optional[int]:
         """
@@ -1460,14 +1480,204 @@
     @property
     @pulumi.getter(name="webUrl")
     def web_url(self) -> str:
         return pulumi.get(self, "web_url")
 
 
 @pulumi.output_type
+class GetGroupSubgroupsSubgroupResult(dict):
+    def __init__(__self__, *,
+                 auto_devops_enabled: bool,
+                 avatar_url: str,
+                 created_at: str,
+                 default_branch_protection: int,
+                 description: str,
+                 emails_disabled: bool,
+                 file_template_project_id: int,
+                 full_name: str,
+                 full_path: str,
+                 group_id: int,
+                 ip_restriction_ranges: str,
+                 lfs_enabled: bool,
+                 mentions_disabled: bool,
+                 name: str,
+                 parent_id: int,
+                 path: str,
+                 project_creation_level: str,
+                 request_access_enabled: bool,
+                 require_two_factor_authentication: bool,
+                 share_with_group_lock: bool,
+                 statistics: Mapping[str, str],
+                 subgroup_creation_level: str,
+                 two_factor_grace_period: int,
+                 visibility: str,
+                 web_url: str):
+        """
+        :param int group_id: The ID of the group.
+        :param Mapping[str, str] statistics: Include group statistics (administrators only).
+        """
+        pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
+        pulumi.set(__self__, "avatar_url", avatar_url)
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "default_branch_protection", default_branch_protection)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "emails_disabled", emails_disabled)
+        pulumi.set(__self__, "file_template_project_id", file_template_project_id)
+        pulumi.set(__self__, "full_name", full_name)
+        pulumi.set(__self__, "full_path", full_path)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "ip_restriction_ranges", ip_restriction_ranges)
+        pulumi.set(__self__, "lfs_enabled", lfs_enabled)
+        pulumi.set(__self__, "mentions_disabled", mentions_disabled)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "parent_id", parent_id)
+        pulumi.set(__self__, "path", path)
+        pulumi.set(__self__, "project_creation_level", project_creation_level)
+        pulumi.set(__self__, "request_access_enabled", request_access_enabled)
+        pulumi.set(__self__, "require_two_factor_authentication", require_two_factor_authentication)
+        pulumi.set(__self__, "share_with_group_lock", share_with_group_lock)
+        pulumi.set(__self__, "statistics", statistics)
+        pulumi.set(__self__, "subgroup_creation_level", subgroup_creation_level)
+        pulumi.set(__self__, "two_factor_grace_period", two_factor_grace_period)
+        pulumi.set(__self__, "visibility", visibility)
+        pulumi.set(__self__, "web_url", web_url)
+
+    @property
+    @pulumi.getter(name="autoDevopsEnabled")
+    def auto_devops_enabled(self) -> bool:
+        return pulumi.get(self, "auto_devops_enabled")
+
+    @property
+    @pulumi.getter(name="avatarUrl")
+    def avatar_url(self) -> str:
+        return pulumi.get(self, "avatar_url")
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter(name="defaultBranchProtection")
+    def default_branch_protection(self) -> int:
+        return pulumi.get(self, "default_branch_protection")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter(name="emailsDisabled")
+    def emails_disabled(self) -> bool:
+        return pulumi.get(self, "emails_disabled")
+
+    @property
+    @pulumi.getter(name="fileTemplateProjectId")
+    def file_template_project_id(self) -> int:
+        return pulumi.get(self, "file_template_project_id")
+
+    @property
+    @pulumi.getter(name="fullName")
+    def full_name(self) -> str:
+        return pulumi.get(self, "full_name")
+
+    @property
+    @pulumi.getter(name="fullPath")
+    def full_path(self) -> str:
+        return pulumi.get(self, "full_path")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> int:
+        """
+        The ID of the group.
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter(name="ipRestrictionRanges")
+    def ip_restriction_ranges(self) -> str:
+        return pulumi.get(self, "ip_restriction_ranges")
+
+    @property
+    @pulumi.getter(name="lfsEnabled")
+    def lfs_enabled(self) -> bool:
+        return pulumi.get(self, "lfs_enabled")
+
+    @property
+    @pulumi.getter(name="mentionsDisabled")
+    def mentions_disabled(self) -> bool:
+        return pulumi.get(self, "mentions_disabled")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> int:
+        return pulumi.get(self, "parent_id")
+
+    @property
+    @pulumi.getter
+    def path(self) -> str:
+        return pulumi.get(self, "path")
+
+    @property
+    @pulumi.getter(name="projectCreationLevel")
+    def project_creation_level(self) -> str:
+        return pulumi.get(self, "project_creation_level")
+
+    @property
+    @pulumi.getter(name="requestAccessEnabled")
+    def request_access_enabled(self) -> bool:
+        return pulumi.get(self, "request_access_enabled")
+
+    @property
+    @pulumi.getter(name="requireTwoFactorAuthentication")
+    def require_two_factor_authentication(self) -> bool:
+        return pulumi.get(self, "require_two_factor_authentication")
+
+    @property
+    @pulumi.getter(name="shareWithGroupLock")
+    def share_with_group_lock(self) -> bool:
+        return pulumi.get(self, "share_with_group_lock")
+
+    @property
+    @pulumi.getter
+    def statistics(self) -> Mapping[str, str]:
+        """
+        Include group statistics (administrators only).
+        """
+        return pulumi.get(self, "statistics")
+
+    @property
+    @pulumi.getter(name="subgroupCreationLevel")
+    def subgroup_creation_level(self) -> str:
+        return pulumi.get(self, "subgroup_creation_level")
+
+    @property
+    @pulumi.getter(name="twoFactorGracePeriod")
+    def two_factor_grace_period(self) -> int:
+        return pulumi.get(self, "two_factor_grace_period")
+
+    @property
+    @pulumi.getter
+    def visibility(self) -> str:
+        return pulumi.get(self, "visibility")
+
+    @property
+    @pulumi.getter(name="webUrl")
+    def web_url(self) -> str:
+        return pulumi.get(self, "web_url")
+
+
+@pulumi.output_type
 class GetGroupVariablesVariableResult(dict):
     def __init__(__self__, *,
                  environment_scope: str,
                  group: str,
                  key: str,
                  masked: bool,
                  protected: bool,
@@ -1524,14 +1734,117 @@
     @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> str:
         return pulumi.get(self, "variable_type")
 
 
 @pulumi.output_type
+class GetGroupsGroupResult(dict):
+    def __init__(__self__, *,
+                 default_branch_protection: int,
+                 description: str,
+                 full_name: str,
+                 full_path: str,
+                 group_id: int,
+                 lfs_enabled: bool,
+                 name: str,
+                 parent_id: int,
+                 path: str,
+                 prevent_forking_outside_group: bool,
+                 request_access_enabled: bool,
+                 runners_token: str,
+                 visibility_level: str,
+                 web_url: str):
+        pulumi.set(__self__, "default_branch_protection", default_branch_protection)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "full_name", full_name)
+        pulumi.set(__self__, "full_path", full_path)
+        pulumi.set(__self__, "group_id", group_id)
+        pulumi.set(__self__, "lfs_enabled", lfs_enabled)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "parent_id", parent_id)
+        pulumi.set(__self__, "path", path)
+        pulumi.set(__self__, "prevent_forking_outside_group", prevent_forking_outside_group)
+        pulumi.set(__self__, "request_access_enabled", request_access_enabled)
+        pulumi.set(__self__, "runners_token", runners_token)
+        pulumi.set(__self__, "visibility_level", visibility_level)
+        pulumi.set(__self__, "web_url", web_url)
+
+    @property
+    @pulumi.getter(name="defaultBranchProtection")
+    def default_branch_protection(self) -> int:
+        return pulumi.get(self, "default_branch_protection")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter(name="fullName")
+    def full_name(self) -> str:
+        return pulumi.get(self, "full_name")
+
+    @property
+    @pulumi.getter(name="fullPath")
+    def full_path(self) -> str:
+        return pulumi.get(self, "full_path")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> int:
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter(name="lfsEnabled")
+    def lfs_enabled(self) -> bool:
+        return pulumi.get(self, "lfs_enabled")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="parentId")
+    def parent_id(self) -> int:
+        return pulumi.get(self, "parent_id")
+
+    @property
+    @pulumi.getter
+    def path(self) -> str:
+        return pulumi.get(self, "path")
+
+    @property
+    @pulumi.getter(name="preventForkingOutsideGroup")
+    def prevent_forking_outside_group(self) -> bool:
+        return pulumi.get(self, "prevent_forking_outside_group")
+
+    @property
+    @pulumi.getter(name="requestAccessEnabled")
+    def request_access_enabled(self) -> bool:
+        return pulumi.get(self, "request_access_enabled")
+
+    @property
+    @pulumi.getter(name="runnersToken")
+    def runners_token(self) -> str:
+        return pulumi.get(self, "runners_token")
+
+    @property
+    @pulumi.getter(name="visibilityLevel")
+    def visibility_level(self) -> str:
+        return pulumi.get(self, "visibility_level")
+
+    @property
+    @pulumi.getter(name="webUrl")
+    def web_url(self) -> str:
+        return pulumi.get(self, "web_url")
+
+
+@pulumi.output_type
 class GetInstanceDeployKeysDeployKeyResult(dict):
     def __init__(__self__, *,
                  created_at: str,
                  fingerprint: str,
                  id: int,
                  key: str,
                  projects_with_write_accesses: Sequence['outputs.GetInstanceDeployKeysDeployKeyProjectsWithWriteAccessResult'],
@@ -1677,26 +1990,224 @@
     @property
     @pulumi.getter(name="variableType")
     def variable_type(self) -> str:
         return pulumi.get(self, "variable_type")
 
 
 @pulumi.output_type
+class GetMetadataKasResult(dict):
+    def __init__(__self__, *,
+                 enabled: bool,
+                 external_url: str,
+                 version: str):
+        """
+        :param bool enabled: Indicates whether KAS is enabled.
+        :param str external_url: URL used by the agents to communicate with KAS. It’s null if kas.enabled is false.
+        :param str version: Version of KAS. It’s null if kas.enabled is false.
+        """
+        pulumi.set(__self__, "enabled", enabled)
+        pulumi.set(__self__, "external_url", external_url)
+        pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def enabled(self) -> bool:
+        """
+        Indicates whether KAS is enabled.
+        """
+        return pulumi.get(self, "enabled")
+
+    @property
+    @pulumi.getter(name="externalUrl")
+    def external_url(self) -> str:
+        """
+        URL used by the agents to communicate with KAS. It’s null if kas.enabled is false.
+        """
+        return pulumi.get(self, "external_url")
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        Version of KAS. It’s null if kas.enabled is false.
+        """
+        return pulumi.get(self, "version")
+
+
+@pulumi.output_type
+class GetProjectBranchesBranchResult(dict):
+    def __init__(__self__, *,
+                 can_push: bool,
+                 commits: Sequence['outputs.GetProjectBranchesBranchCommitResult'],
+                 default: bool,
+                 developers_can_merge: bool,
+                 developers_can_push: bool,
+                 merged: bool,
+                 name: str,
+                 protected: bool,
+                 web_url: str):
+        pulumi.set(__self__, "can_push", can_push)
+        pulumi.set(__self__, "commits", commits)
+        pulumi.set(__self__, "default", default)
+        pulumi.set(__self__, "developers_can_merge", developers_can_merge)
+        pulumi.set(__self__, "developers_can_push", developers_can_push)
+        pulumi.set(__self__, "merged", merged)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "protected", protected)
+        pulumi.set(__self__, "web_url", web_url)
+
+    @property
+    @pulumi.getter(name="canPush")
+    def can_push(self) -> bool:
+        return pulumi.get(self, "can_push")
+
+    @property
+    @pulumi.getter
+    def commits(self) -> Sequence['outputs.GetProjectBranchesBranchCommitResult']:
+        return pulumi.get(self, "commits")
+
+    @property
+    @pulumi.getter
+    def default(self) -> bool:
+        return pulumi.get(self, "default")
+
+    @property
+    @pulumi.getter(name="developersCanMerge")
+    def developers_can_merge(self) -> bool:
+        return pulumi.get(self, "developers_can_merge")
+
+    @property
+    @pulumi.getter(name="developersCanPush")
+    def developers_can_push(self) -> bool:
+        return pulumi.get(self, "developers_can_push")
+
+    @property
+    @pulumi.getter
+    def merged(self) -> bool:
+        return pulumi.get(self, "merged")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def protected(self) -> bool:
+        return pulumi.get(self, "protected")
+
+    @property
+    @pulumi.getter(name="webUrl")
+    def web_url(self) -> str:
+        return pulumi.get(self, "web_url")
+
+
+@pulumi.output_type
+class GetProjectBranchesBranchCommitResult(dict):
+    def __init__(__self__, *,
+                 author_email: str,
+                 author_name: str,
+                 authored_date: str,
+                 committed_date: str,
+                 committer_email: str,
+                 committer_name: str,
+                 id: str,
+                 message: str,
+                 parent_ids: Sequence[str],
+                 short_id: str,
+                 title: str):
+        """
+        :param str id: The ID of this resource.
+        """
+        pulumi.set(__self__, "author_email", author_email)
+        pulumi.set(__self__, "author_name", author_name)
+        pulumi.set(__self__, "authored_date", authored_date)
+        pulumi.set(__self__, "committed_date", committed_date)
+        pulumi.set(__self__, "committer_email", committer_email)
+        pulumi.set(__self__, "committer_name", committer_name)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "message", message)
+        pulumi.set(__self__, "parent_ids", parent_ids)
+        pulumi.set(__self__, "short_id", short_id)
+        pulumi.set(__self__, "title", title)
+
+    @property
+    @pulumi.getter(name="authorEmail")
+    def author_email(self) -> str:
+        return pulumi.get(self, "author_email")
+
+    @property
+    @pulumi.getter(name="authorName")
+    def author_name(self) -> str:
+        return pulumi.get(self, "author_name")
+
+    @property
+    @pulumi.getter(name="authoredDate")
+    def authored_date(self) -> str:
+        return pulumi.get(self, "authored_date")
+
+    @property
+    @pulumi.getter(name="committedDate")
+    def committed_date(self) -> str:
+        return pulumi.get(self, "committed_date")
+
+    @property
+    @pulumi.getter(name="committerEmail")
+    def committer_email(self) -> str:
+        return pulumi.get(self, "committer_email")
+
+    @property
+    @pulumi.getter(name="committerName")
+    def committer_name(self) -> str:
+        return pulumi.get(self, "committer_name")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The ID of this resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def message(self) -> str:
+        return pulumi.get(self, "message")
+
+    @property
+    @pulumi.getter(name="parentIds")
+    def parent_ids(self) -> Sequence[str]:
+        return pulumi.get(self, "parent_ids")
+
+    @property
+    @pulumi.getter(name="shortId")
+    def short_id(self) -> str:
+        return pulumi.get(self, "short_id")
+
+    @property
+    @pulumi.getter
+    def title(self) -> str:
+        return pulumi.get(self, "title")
+
+
+@pulumi.output_type
 class GetProjectContainerExpirationPolicyResult(dict):
     def __init__(__self__, *,
                  cadence: str,
                  enabled: bool,
                  keep_n: int,
+                 name_regex: str,
                  name_regex_delete: str,
                  name_regex_keep: str,
                  next_run_at: str,
                  older_than: str):
         pulumi.set(__self__, "cadence", cadence)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "keep_n", keep_n)
+        pulumi.set(__self__, "name_regex", name_regex)
         pulumi.set(__self__, "name_regex_delete", name_regex_delete)
         pulumi.set(__self__, "name_regex_keep", name_regex_keep)
         pulumi.set(__self__, "next_run_at", next_run_at)
         pulumi.set(__self__, "older_than", older_than)
 
     @property
     @pulumi.getter
@@ -1710,14 +2221,19 @@
 
     @property
     @pulumi.getter(name="keepN")
     def keep_n(self) -> int:
         return pulumi.get(self, "keep_n")
 
     @property
+    @pulumi.getter(name="nameRegex")
+    def name_regex(self) -> str:
+        return pulumi.get(self, "name_regex")
+
+    @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> str:
         return pulumi.get(self, "name_regex_delete")
 
     @property
     @pulumi.getter(name="nameRegexKeep")
     def name_regex_keep(self) -> str:
@@ -2583,15 +3099,15 @@
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> int:
         return pulumi.get(self, "user_id")
 
 
 @pulumi.output_type
-class GetProjectPushRulesResult(dict):
+class GetProjectPushRuleResult(dict):
     def __init__(__self__, *,
                  author_email_regex: str,
                  branch_name_regex: str,
                  commit_committer_check: bool,
                  commit_message_negative_regex: str,
                  commit_message_regex: str,
                  deny_delete_tag: bool,
@@ -3022,68 +3538,77 @@
                  container_registry_enabled: bool,
                  created_at: str,
                  creator_id: int,
                  custom_attributes: Sequence[Mapping[str, str]],
                  default_branch: str,
                  description: str,
                  emails_disabled: bool,
+                 environments_access_level: str,
                  external_authorization_classification_label: str,
-                 forked_from_project: 'outputs.GetProjectsProjectForkedFromProjectResult',
+                 feature_flags_access_level: str,
+                 forked_from_projects: Sequence['outputs.GetProjectsProjectForkedFromProjectResult'],
                  forking_access_level: str,
                  forks_count: int,
                  http_url_to_repo: str,
                  id: int,
                  import_error: str,
                  import_status: str,
+                 import_url: str,
+                 infrastructure_access_level: str,
                  issues_access_level: str,
                  issues_enabled: bool,
                  jobs_enabled: bool,
+                 keep_latest_artifact: bool,
                  last_activity_at: str,
                  lfs_enabled: bool,
                  merge_commit_template: str,
                  merge_method: str,
                  merge_pipelines_enabled: bool,
                  merge_requests_access_level: str,
                  merge_requests_enabled: bool,
                  merge_trains_enabled: bool,
                  mirror: bool,
                  mirror_overwrites_diverged_branches: bool,
                  mirror_trigger_builds: bool,
                  mirror_user_id: int,
+                 monitor_access_level: str,
                  name: str,
                  name_with_namespace: str,
-                 namespace: 'outputs.GetProjectsProjectNamespaceResult',
+                 namespaces: Sequence['outputs.GetProjectsProjectNamespaceResult'],
                  only_allow_merge_if_all_discussions_are_resolved: bool,
                  only_allow_merge_if_pipeline_succeeds: bool,
                  only_mirror_protected_branches: bool,
                  open_issues_count: int,
                  operations_access_level: str,
-                 owner: 'outputs.GetProjectsProjectOwnerResult',
+                 owners: Sequence['outputs.GetProjectsProjectOwnerResult'],
                  packages_enabled: bool,
                  path: str,
                  path_with_namespace: str,
-                 permissions: 'outputs.GetProjectsProjectPermissionsResult',
+                 permissions: Sequence['outputs.GetProjectsProjectPermissionResult'],
                  public: bool,
                  public_builds: bool,
                  readme_url: str,
+                 releases_access_level: str,
                  repository_access_level: str,
                  repository_storage: str,
                  request_access_enabled: bool,
                  requirements_access_level: str,
                  resolve_outdated_diff_discussions: bool,
+                 restrict_user_defined_variables: bool,
                  runners_token: str,
                  security_and_compliance_access_level: str,
                  shared_runners_enabled: bool,
                  shared_with_groups: Sequence['outputs.GetProjectsProjectSharedWithGroupResult'],
                  snippets_access_level: str,
                  snippets_enabled: bool,
                  squash_commit_template: str,
                  ssh_url_to_repo: str,
                  star_count: int,
                  statistics: Mapping[str, int],
+                 suggestion_commit_message: str,
                  tag_lists: Sequence[str],
                  topics: Sequence[str],
                  visibility: str,
                  web_url: str,
                  wiki_access_level: str,
                  wiki_enabled: bool):
         """
@@ -3114,68 +3639,77 @@
         pulumi.set(__self__, "container_registry_enabled", container_registry_enabled)
         pulumi.set(__self__, "created_at", created_at)
         pulumi.set(__self__, "creator_id", creator_id)
         pulumi.set(__self__, "custom_attributes", custom_attributes)
         pulumi.set(__self__, "default_branch", default_branch)
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "emails_disabled", emails_disabled)
+        pulumi.set(__self__, "environments_access_level", environments_access_level)
         pulumi.set(__self__, "external_authorization_classification_label", external_authorization_classification_label)
-        pulumi.set(__self__, "forked_from_project", forked_from_project)
+        pulumi.set(__self__, "feature_flags_access_level", feature_flags_access_level)
+        pulumi.set(__self__, "forked_from_projects", forked_from_projects)
         pulumi.set(__self__, "forking_access_level", forking_access_level)
         pulumi.set(__self__, "forks_count", forks_count)
         pulumi.set(__self__, "http_url_to_repo", http_url_to_repo)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "import_error", import_error)
         pulumi.set(__self__, "import_status", import_status)
+        pulumi.set(__self__, "import_url", import_url)
+        pulumi.set(__self__, "infrastructure_access_level", infrastructure_access_level)
         pulumi.set(__self__, "issues_access_level", issues_access_level)
         pulumi.set(__self__, "issues_enabled", issues_enabled)
         pulumi.set(__self__, "jobs_enabled", jobs_enabled)
+        pulumi.set(__self__, "keep_latest_artifact", keep_latest_artifact)
         pulumi.set(__self__, "last_activity_at", last_activity_at)
         pulumi.set(__self__, "lfs_enabled", lfs_enabled)
         pulumi.set(__self__, "merge_commit_template", merge_commit_template)
         pulumi.set(__self__, "merge_method", merge_method)
         pulumi.set(__self__, "merge_pipelines_enabled", merge_pipelines_enabled)
         pulumi.set(__self__, "merge_requests_access_level", merge_requests_access_level)
         pulumi.set(__self__, "merge_requests_enabled", merge_requests_enabled)
         pulumi.set(__self__, "merge_trains_enabled", merge_trains_enabled)
         pulumi.set(__self__, "mirror", mirror)
         pulumi.set(__self__, "mirror_overwrites_diverged_branches", mirror_overwrites_diverged_branches)
         pulumi.set(__self__, "mirror_trigger_builds", mirror_trigger_builds)
         pulumi.set(__self__, "mirror_user_id", mirror_user_id)
+        pulumi.set(__self__, "monitor_access_level", monitor_access_level)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "name_with_namespace", name_with_namespace)
-        pulumi.set(__self__, "namespace", namespace)
+        pulumi.set(__self__, "namespaces", namespaces)
         pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         pulumi.set(__self__, "only_allow_merge_if_pipeline_succeeds", only_allow_merge_if_pipeline_succeeds)
         pulumi.set(__self__, "only_mirror_protected_branches", only_mirror_protected_branches)
         pulumi.set(__self__, "open_issues_count", open_issues_count)
         pulumi.set(__self__, "operations_access_level", operations_access_level)
-        pulumi.set(__self__, "owner", owner)
+        pulumi.set(__self__, "owners", owners)
         pulumi.set(__self__, "packages_enabled", packages_enabled)
         pulumi.set(__self__, "path", path)
         pulumi.set(__self__, "path_with_namespace", path_with_namespace)
         pulumi.set(__self__, "permissions", permissions)
         pulumi.set(__self__, "public", public)
         pulumi.set(__self__, "public_builds", public_builds)
         pulumi.set(__self__, "readme_url", readme_url)
+        pulumi.set(__self__, "releases_access_level", releases_access_level)
         pulumi.set(__self__, "repository_access_level", repository_access_level)
         pulumi.set(__self__, "repository_storage", repository_storage)
         pulumi.set(__self__, "request_access_enabled", request_access_enabled)
         pulumi.set(__self__, "requirements_access_level", requirements_access_level)
         pulumi.set(__self__, "resolve_outdated_diff_discussions", resolve_outdated_diff_discussions)
+        pulumi.set(__self__, "restrict_user_defined_variables", restrict_user_defined_variables)
         pulumi.set(__self__, "runners_token", runners_token)
         pulumi.set(__self__, "security_and_compliance_access_level", security_and_compliance_access_level)
         pulumi.set(__self__, "shared_runners_enabled", shared_runners_enabled)
         pulumi.set(__self__, "shared_with_groups", shared_with_groups)
         pulumi.set(__self__, "snippets_access_level", snippets_access_level)
         pulumi.set(__self__, "snippets_enabled", snippets_enabled)
         pulumi.set(__self__, "squash_commit_template", squash_commit_template)
         pulumi.set(__self__, "ssh_url_to_repo", ssh_url_to_repo)
         pulumi.set(__self__, "star_count", star_count)
         pulumi.set(__self__, "statistics", statistics)
+        pulumi.set(__self__, "suggestion_commit_message", suggestion_commit_message)
         pulumi.set(__self__, "tag_lists", tag_lists)
         pulumi.set(__self__, "topics", topics)
         pulumi.set(__self__, "visibility", visibility)
         pulumi.set(__self__, "web_url", web_url)
         pulumi.set(__self__, "wiki_access_level", wiki_access_level)
         pulumi.set(__self__, "wiki_enabled", wiki_enabled)
 
@@ -3309,22 +3843,32 @@
 
     @property
     @pulumi.getter(name="emailsDisabled")
     def emails_disabled(self) -> bool:
         return pulumi.get(self, "emails_disabled")
 
     @property
+    @pulumi.getter(name="environmentsAccessLevel")
+    def environments_access_level(self) -> str:
+        return pulumi.get(self, "environments_access_level")
+
+    @property
     @pulumi.getter(name="externalAuthorizationClassificationLabel")
     def external_authorization_classification_label(self) -> str:
         return pulumi.get(self, "external_authorization_classification_label")
 
     @property
-    @pulumi.getter(name="forkedFromProject")
-    def forked_from_project(self) -> 'outputs.GetProjectsProjectForkedFromProjectResult':
-        return pulumi.get(self, "forked_from_project")
+    @pulumi.getter(name="featureFlagsAccessLevel")
+    def feature_flags_access_level(self) -> str:
+        return pulumi.get(self, "feature_flags_access_level")
+
+    @property
+    @pulumi.getter(name="forkedFromProjects")
+    def forked_from_projects(self) -> Sequence['outputs.GetProjectsProjectForkedFromProjectResult']:
+        return pulumi.get(self, "forked_from_projects")
 
     @property
     @pulumi.getter(name="forkingAccessLevel")
     def forking_access_level(self) -> str:
         return pulumi.get(self, "forking_access_level")
 
     @property
@@ -3352,14 +3896,24 @@
 
     @property
     @pulumi.getter(name="importStatus")
     def import_status(self) -> str:
         return pulumi.get(self, "import_status")
 
     @property
+    @pulumi.getter(name="importUrl")
+    def import_url(self) -> str:
+        return pulumi.get(self, "import_url")
+
+    @property
+    @pulumi.getter(name="infrastructureAccessLevel")
+    def infrastructure_access_level(self) -> str:
+        return pulumi.get(self, "infrastructure_access_level")
+
+    @property
     @pulumi.getter(name="issuesAccessLevel")
     def issues_access_level(self) -> str:
         return pulumi.get(self, "issues_access_level")
 
     @property
     @pulumi.getter(name="issuesEnabled")
     def issues_enabled(self) -> bool:
@@ -3367,14 +3921,19 @@
 
     @property
     @pulumi.getter(name="jobsEnabled")
     def jobs_enabled(self) -> bool:
         return pulumi.get(self, "jobs_enabled")
 
     @property
+    @pulumi.getter(name="keepLatestArtifact")
+    def keep_latest_artifact(self) -> bool:
+        return pulumi.get(self, "keep_latest_artifact")
+
+    @property
     @pulumi.getter(name="lastActivityAt")
     def last_activity_at(self) -> str:
         return pulumi.get(self, "last_activity_at")
 
     @property
     @pulumi.getter(name="lfsEnabled")
     def lfs_enabled(self) -> bool:
@@ -3427,27 +3986,32 @@
 
     @property
     @pulumi.getter(name="mirrorUserId")
     def mirror_user_id(self) -> int:
         return pulumi.get(self, "mirror_user_id")
 
     @property
+    @pulumi.getter(name="monitorAccessLevel")
+    def monitor_access_level(self) -> str:
+        return pulumi.get(self, "monitor_access_level")
+
+    @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="nameWithNamespace")
     def name_with_namespace(self) -> str:
         return pulumi.get(self, "name_with_namespace")
 
     @property
     @pulumi.getter
-    def namespace(self) -> 'outputs.GetProjectsProjectNamespaceResult':
-        return pulumi.get(self, "namespace")
+    def namespaces(self) -> Sequence['outputs.GetProjectsProjectNamespaceResult']:
+        return pulumi.get(self, "namespaces")
 
     @property
     @pulumi.getter(name="onlyAllowMergeIfAllDiscussionsAreResolved")
     def only_allow_merge_if_all_discussions_are_resolved(self) -> bool:
         return pulumi.get(self, "only_allow_merge_if_all_discussions_are_resolved")
 
     @property
@@ -3468,16 +4032,16 @@
     @property
     @pulumi.getter(name="operationsAccessLevel")
     def operations_access_level(self) -> str:
         return pulumi.get(self, "operations_access_level")
 
     @property
     @pulumi.getter
-    def owner(self) -> 'outputs.GetProjectsProjectOwnerResult':
-        return pulumi.get(self, "owner")
+    def owners(self) -> Sequence['outputs.GetProjectsProjectOwnerResult']:
+        return pulumi.get(self, "owners")
 
     @property
     @pulumi.getter(name="packagesEnabled")
     def packages_enabled(self) -> bool:
         return pulumi.get(self, "packages_enabled")
 
     @property
@@ -3488,15 +4052,15 @@
     @property
     @pulumi.getter(name="pathWithNamespace")
     def path_with_namespace(self) -> str:
         return pulumi.get(self, "path_with_namespace")
 
     @property
     @pulumi.getter
-    def permissions(self) -> 'outputs.GetProjectsProjectPermissionsResult':
+    def permissions(self) -> Sequence['outputs.GetProjectsProjectPermissionResult']:
         return pulumi.get(self, "permissions")
 
     @property
     @pulumi.getter
     def public(self) -> bool:
         return pulumi.get(self, "public")
 
@@ -3507,14 +4071,19 @@
 
     @property
     @pulumi.getter(name="readmeUrl")
     def readme_url(self) -> str:
         return pulumi.get(self, "readme_url")
 
     @property
+    @pulumi.getter(name="releasesAccessLevel")
+    def releases_access_level(self) -> str:
+        return pulumi.get(self, "releases_access_level")
+
+    @property
     @pulumi.getter(name="repositoryAccessLevel")
     def repository_access_level(self) -> str:
         return pulumi.get(self, "repository_access_level")
 
     @property
     @pulumi.getter(name="repositoryStorage")
     def repository_storage(self) -> str:
@@ -3532,14 +4101,19 @@
 
     @property
     @pulumi.getter(name="resolveOutdatedDiffDiscussions")
     def resolve_outdated_diff_discussions(self) -> bool:
         return pulumi.get(self, "resolve_outdated_diff_discussions")
 
     @property
+    @pulumi.getter(name="restrictUserDefinedVariables")
+    def restrict_user_defined_variables(self) -> bool:
+        return pulumi.get(self, "restrict_user_defined_variables")
+
+    @property
     @pulumi.getter(name="runnersToken")
     def runners_token(self) -> str:
         return pulumi.get(self, "runners_token")
 
     @property
     @pulumi.getter(name="securityAndComplianceAccessLevel")
     def security_and_compliance_access_level(self) -> str:
@@ -3585,14 +4159,19 @@
     def statistics(self) -> Mapping[str, int]:
         """
         Include project statistics. Cannot be used with `group_id`.
         """
         return pulumi.get(self, "statistics")
 
     @property
+    @pulumi.getter(name="suggestionCommitMessage")
+    def suggestion_commit_message(self) -> str:
+        return pulumi.get(self, "suggestion_commit_message")
+
+    @property
     @pulumi.getter(name="tagLists")
     def tag_lists(self) -> Sequence[str]:
         return pulumi.get(self, "tag_lists")
 
     @property
     @pulumi.getter
     def topics(self) -> Sequence[str]:
@@ -3624,21 +4203,23 @@
 
 @pulumi.output_type
 class GetProjectsProjectContainerExpirationPolicyResult(dict):
     def __init__(__self__, *,
                  cadence: str,
                  enabled: bool,
                  keep_n: int,
+                 name_regex: str,
                  name_regex_delete: str,
                  name_regex_keep: str,
                  next_run_at: str,
                  older_than: str):
         pulumi.set(__self__, "cadence", cadence)
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "keep_n", keep_n)
+        pulumi.set(__self__, "name_regex", name_regex)
         pulumi.set(__self__, "name_regex_delete", name_regex_delete)
         pulumi.set(__self__, "name_regex_keep", name_regex_keep)
         pulumi.set(__self__, "next_run_at", next_run_at)
         pulumi.set(__self__, "older_than", older_than)
 
     @property
     @pulumi.getter
@@ -3652,14 +4233,19 @@
 
     @property
     @pulumi.getter(name="keepN")
     def keep_n(self) -> int:
         return pulumi.get(self, "keep_n")
 
     @property
+    @pulumi.getter(name="nameRegex")
+    def name_regex(self) -> str:
+        return pulumi.get(self, "name_regex")
+
+    @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> str:
         return pulumi.get(self, "name_regex_delete")
 
     @property
     @pulumi.getter(name="nameRegexKeep")
     def name_regex_keep(self) -> str:
@@ -3832,15 +4418,15 @@
     @property
     @pulumi.getter(name="websiteUrl")
     def website_url(self) -> str:
         return pulumi.get(self, "website_url")
 
 
 @pulumi.output_type
-class GetProjectsProjectPermissionsResult(dict):
+class GetProjectsProjectPermissionResult(dict):
     def __init__(__self__, *,
                  group_access: Mapping[str, int],
                  project_access: Mapping[str, int]):
         pulumi.set(__self__, "group_access", group_access)
         pulumi.set(__self__, "project_access", project_access)
 
     @property
@@ -4011,14 +4597,67 @@
     @property
     @pulumi.getter
     def type(self) -> str:
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
+class GetUserSshkeysKeyResult(dict):
+    def __init__(__self__, *,
+                 created_at: str,
+                 expires_at: str,
+                 key: str,
+                 key_id: int,
+                 title: str,
+                 user_id: int):
+        """
+        :param int user_id: ID of the user to get the SSH keys for.
+        """
+        pulumi.set(__self__, "created_at", created_at)
+        pulumi.set(__self__, "expires_at", expires_at)
+        pulumi.set(__self__, "key", key)
+        pulumi.set(__self__, "key_id", key_id)
+        pulumi.set(__self__, "title", title)
+        pulumi.set(__self__, "user_id", user_id)
+
+    @property
+    @pulumi.getter(name="createdAt")
+    def created_at(self) -> str:
+        return pulumi.get(self, "created_at")
+
+    @property
+    @pulumi.getter(name="expiresAt")
+    def expires_at(self) -> str:
+        return pulumi.get(self, "expires_at")
+
+    @property
+    @pulumi.getter
+    def key(self) -> str:
+        return pulumi.get(self, "key")
+
+    @property
+    @pulumi.getter(name="keyId")
+    def key_id(self) -> int:
+        return pulumi.get(self, "key_id")
+
+    @property
+    @pulumi.getter
+    def title(self) -> str:
+        return pulumi.get(self, "title")
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> int:
+        """
+        ID of the user to get the SSH keys for.
+        """
+        return pulumi.get(self, "user_id")
+
+
+@pulumi.output_type
 class GetUsersUserResult(dict):
     def __init__(__self__, *,
                  avatar_url: str,
                  bio: str,
                  can_create_group: bool,
                  can_create_project: bool,
                  color_scheme_id: int,
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/personal_access_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(__self__, *,
                  scopes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  user_id: pulumi.Input[int],
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PersonalAccessToken resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[int] user_id: The id of the user.
         :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
         :param pulumi.Input[str] name: The name of the personal access token.
         """
         pulumi.set(__self__, "scopes", scopes)
         pulumi.set(__self__, "user_id", user_id)
         if expires_at is not None:
@@ -32,15 +32,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter
     def scopes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         """
         return pulumi.get(self, "scopes")
 
     @scopes.setter
     def scopes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "scopes", value)
 
@@ -95,15 +95,15 @@
         """
         Input properties used for looking up and filtering PersonalAccessToken resources.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
         :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
         :param pulumi.Input[str] name: The name of the personal access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[str] token: The personal access token. This is only populated when creating a new personal access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
@@ -180,15 +180,15 @@
     def revoked(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "revoked", value)
 
     @property
     @pulumi.getter
     def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         """
         return pulumi.get(self, "scopes")
 
     @scopes.setter
     def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "scopes", value)
 
@@ -260,15 +260,15 @@
 
          NOTEthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
         :param pulumi.Input[str] name: The name of the personal access token.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PersonalAccessTokenArgs,
@@ -374,15 +374,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
         :param pulumi.Input[str] expires_at: The token expires at midnight UTC on that date. The date must be in the format YYYY-MM-DD. Default is never.
         :param pulumi.Input[str] name: The name of the personal access token.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         :param pulumi.Input[str] token: The personal access token. This is only populated when creating a new personal access token. This attribute is not available for imported resources.
         :param pulumi.Input[int] user_id: The id of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PersonalAccessTokenState.__new__(_PersonalAccessTokenState)
 
@@ -436,15 +436,15 @@
         """
         return pulumi.get(self, "revoked")
 
     @property
     @pulumi.getter
     def scopes(self) -> pulumi.Output[Sequence[str]]:
         """
-        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`.
+        The scope for the personal access token. It determines the actions which can be performed when authenticating with this token. Valid values are: `api`, `read_user`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`, `sudo`, `admin_mode`.
         """
         return pulumi.get(self, "scopes")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,16 @@
 
         example_pipeline_schedule = gitlab.PipelineSchedule("examplePipelineSchedule",
             project="12345",
             description="Used to schedule builds",
             ref="master",
             cron="0 1 * * *")
         example_pipeline_schedule_variable = gitlab.PipelineScheduleVariable("examplePipelineScheduleVariable",
-            project=gitlab_pipeline_schedule["project"],
-            pipeline_schedule_id=gitlab_pipeline_schedule["id"],
+            project=example_pipeline_schedule.project,
+            pipeline_schedule_id=example_pipeline_schedule.id,
             key="EXAMPLE_KEY",
             value="example")
         ```
 
         ## Import
 
         Pipeline schedule variables can be imported using an id made up of `project_id:pipeline_schedule_id:key`, e.g.
@@ -218,16 +218,16 @@
 
         example_pipeline_schedule = gitlab.PipelineSchedule("examplePipelineSchedule",
             project="12345",
             description="Used to schedule builds",
             ref="master",
             cron="0 1 * * *")
         example_pipeline_schedule_variable = gitlab.PipelineScheduleVariable("examplePipelineScheduleVariable",
-            project=gitlab_pipeline_schedule["project"],
-            pipeline_schedule_id=gitlab_pipeline_schedule["id"],
+            project=example_pipeline_schedule.project,
+            pipeline_schedule_id=example_pipeline_schedule.id,
             key="EXAMPLE_KEY",
             value="example")
         ```
 
         ## Import
 
         Pipeline schedule variables can be imported using an id made up of `project_id:pipeline_schedule_id:key`, e.g.
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,72 +21,87 @@
                  approvals_before_merge: Optional[pulumi.Input[int]] = None,
                  archive_on_destroy: Optional[pulumi.Input[bool]] = None,
                  archived: Optional[pulumi.Input[bool]] = None,
                  auto_cancel_pending_pipelines: Optional[pulumi.Input[str]] = None,
                  auto_devops_deploy_strategy: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  autoclose_referenced_issues: Optional[pulumi.Input[bool]] = None,
+                 avatar: Optional[pulumi.Input[str]] = None,
+                 avatar_hash: Optional[pulumi.Input[str]] = None,
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
+                 environments_access_level: Optional[pulumi.Input[str]] = None,
                  external_authorization_classification_label: Optional[pulumi.Input[str]] = None,
+                 feature_flags_access_level: Optional[pulumi.Input[str]] = None,
+                 forked_from_project_id: Optional[pulumi.Input[int]] = None,
                  forking_access_level: Optional[pulumi.Input[str]] = None,
                  group_with_project_templates_id: Optional[pulumi.Input[int]] = None,
                  import_url: Optional[pulumi.Input[str]] = None,
+                 import_url_password: Optional[pulumi.Input[str]] = None,
+                 import_url_username: Optional[pulumi.Input[str]] = None,
+                 infrastructure_access_level: Optional[pulumi.Input[str]] = None,
                  initialize_with_readme: Optional[pulumi.Input[bool]] = None,
                  issues_access_level: Optional[pulumi.Input[str]] = None,
                  issues_enabled: Optional[pulumi.Input[bool]] = None,
                  issues_template: Optional[pulumi.Input[str]] = None,
+                 keep_latest_artifact: Optional[pulumi.Input[bool]] = None,
                  lfs_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_commit_template: Optional[pulumi.Input[str]] = None,
                  merge_method: Optional[pulumi.Input[str]] = None,
                  merge_pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_access_level: Optional[pulumi.Input[str]] = None,
                  merge_requests_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_template: Optional[pulumi.Input[str]] = None,
                  merge_trains_enabled: Optional[pulumi.Input[bool]] = None,
                  mirror: Optional[pulumi.Input[bool]] = None,
                  mirror_overwrites_diverged_branches: Optional[pulumi.Input[bool]] = None,
                  mirror_trigger_builds: Optional[pulumi.Input[bool]] = None,
+                 monitor_access_level: Optional[pulumi.Input[str]] = None,
+                 mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
                  operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input['ProjectPushRulesArgs']] = None,
+                 releases_access_level: Optional[pulumi.Input[str]] = None,
                  remove_source_branch_after_merge: Optional[pulumi.Input[bool]] = None,
                  repository_access_level: Optional[pulumi.Input[str]] = None,
                  repository_storage: Optional[pulumi.Input[str]] = None,
                  request_access_enabled: Optional[pulumi.Input[bool]] = None,
                  requirements_access_level: Optional[pulumi.Input[str]] = None,
                  resolve_outdated_diff_discussions: Optional[pulumi.Input[bool]] = None,
+                 restrict_user_defined_variables: Optional[pulumi.Input[bool]] = None,
                  security_and_compliance_access_level: Optional[pulumi.Input[str]] = None,
                  shared_runners_enabled: Optional[pulumi.Input[bool]] = None,
                  skip_wait_for_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  snippets_access_level: Optional[pulumi.Input[str]] = None,
                  snippets_enabled: Optional[pulumi.Input[bool]] = None,
                  squash_commit_template: Optional[pulumi.Input[str]] = None,
                  squash_option: Optional[pulumi.Input[str]] = None,
+                 suggestion_commit_message: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  template_project_id: Optional[pulumi.Input[int]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_custom_template: Optional[pulumi.Input[bool]] = None,
                  visibility_level: Optional[pulumi.Input[str]] = None,
                  wiki_access_level: Optional[pulumi.Input[str]] = None,
@@ -101,80 +116,104 @@
                In the meantime we recommend against using this attribute and use `ProjectApprovalRule` instead.
         :param pulumi.Input[bool] archive_on_destroy: Set to `true` to archive the project instead of deleting on destroy. If set to `true` it will entire omit the `DELETE` operation.
         :param pulumi.Input[bool] archived: Whether the project is in read-only mode (archived). Repositories can be archived/unarchived by toggling this parameter.
         :param pulumi.Input[str] auto_cancel_pending_pipelines: Auto-cancel pending pipelines. This isn’t a boolean, but enabled/disabled.
         :param pulumi.Input[str] auto_devops_deploy_strategy: Auto Deploy strategy. Valid values are `continuous`, `manual`, `timed_incremental`.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for this project.
         :param pulumi.Input[bool] autoclose_referenced_issues: Set whether auto-closing referenced issues on default branch.
+        :param pulumi.Input[str] avatar: A local path to the avatar image to upload. **Note**: not available for imported resources.
+        :param pulumi.Input[str] avatar_hash: The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input['ProjectContainerExpirationPolicyArgs'] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
+        :param pulumi.Input[str] environments_access_level: Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] external_authorization_classification_label: The classification label for the project.
+        :param pulumi.Input[str] feature_flags_access_level: Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[int] forked_from_project_id: The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
         :param pulumi.Input[str] forking_access_level: Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[int] group_with_project_templates_id: For group-level custom templates, specifies ID of group from which all the custom project templates are sourced. Leave empty for instance-level templates. Requires use*custom*template to be true (enterprise edition).
-        :param pulumi.Input[str] import_url: Git URL to a repository to be imported.
+        :param pulumi.Input[str] import_url: Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+               together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+               Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+               credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+               `terraform import`. See the examples section for how to properly use it.
+        :param pulumi.Input[str] import_url_password: The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] import_url_username: The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] infrastructure_access_level: Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] initialize_with_readme: Create main branch with first commit containing a README.md file.
         :param pulumi.Input[str] issues_access_level: Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] issues_enabled: Enable issue tracking for the project.
         :param pulumi.Input[str] issues_template: Sets the template for new issues in the project.
+        :param pulumi.Input[bool] keep_latest_artifact: Disable or enable the ability to keep the latest artifact for this project.
         :param pulumi.Input[bool] lfs_enabled: Enable LFS for the project.
         :param pulumi.Input[str] merge_commit_template: Template used to create merge commit message in merge requests. (Introduced in GitLab 14.5.)
-        :param pulumi.Input[str] merge_method: Set to `ff` to create fast-forward merges
+        :param pulumi.Input[str] merge_method: Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         :param pulumi.Input[bool] merge_pipelines_enabled: Enable or disable merge pipelines.
         :param pulumi.Input[str] merge_requests_access_level: Set the merge requests access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] merge_requests_enabled: Enable merge requests for the project.
         :param pulumi.Input[str] merge_requests_template: Sets the template for new merge requests in the project.
         :param pulumi.Input[bool] merge_trains_enabled: Enable or disable merge trains. Requires `merge_pipelines_enabled` to be set to `true` to take effect.
         :param pulumi.Input[bool] mirror: Enable project pull mirror.
         :param pulumi.Input[bool] mirror_overwrites_diverged_branches: Enable overwrite diverged branches for a mirrored project.
         :param pulumi.Input[bool] mirror_trigger_builds: Enable trigger builds on pushes for a mirrored project.
+        :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
         :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
-        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project.
+        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input['ProjectPushRulesArgs'] push_rules: Push rules for the project.
+        :param pulumi.Input[str] releases_access_level: Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] remove_source_branch_after_merge: Enable `Delete source branch` option by default for all new merge requests.
         :param pulumi.Input[str] repository_access_level: Set the repository access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] repository_storage: Which storage shard the repository is on. (administrator only)
         :param pulumi.Input[bool] request_access_enabled: Allow users to request member access.
         :param pulumi.Input[str] requirements_access_level: Set the requirements access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] resolve_outdated_diff_discussions: Automatically resolve merge request diffs discussions on lines changed with a push.
+        :param pulumi.Input[bool] restrict_user_defined_variables: Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
         :param pulumi.Input[str] security_and_compliance_access_level: Set the security and compliance access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] shared_runners_enabled: Enable shared runners for this project.
         :param pulumi.Input[bool] skip_wait_for_default_branch_protection: If `true`, the default behavior to wait for the default branch protection to be created is skipped.
                This is necessary if the current user is not an admin and the default branch protection is disabled on an instance-level.
                There is currently no known way to determine if the default branch protection is disabled on an instance-level for non-admin users.
                This attribute is only used during resource creation, thus changes are suppressed and the attribute cannot be imported.
         :param pulumi.Input[str] snippets_access_level: Set the snippets access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] snippets_enabled: Enable snippets for the project.
         :param pulumi.Input[str] squash_commit_template: Template used to create squash commit message in merge requests. (Introduced in GitLab 14.6.)
         :param pulumi.Input[str] squash_option: Squash commits when merge request. Valid values are `never`, `always`, `default_on`, or `default_off`. The default value is `default_off`. [GitLab >= 14.1]
+        :param pulumi.Input[str] suggestion_commit_message: The commit message used to apply merge request suggestions.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         :param pulumi.Input[str] template_name: When used without use*custom*template, name of a built-in project template. When used with use*custom*template, name of a custom project template. This option is mutually exclusive with `template_project_id`.
         :param pulumi.Input[int] template_project_id: When used with use*custom*template, project ID of a custom project template. This is preferable to using template*name since template*name may be ambiguous (enterprise edition). This option is mutually exclusive with `template_name`. See `GroupProjectFileTemplate` to set a project as a template project. If a project has not been set as a template, using it here will result in an error.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] topics: The list of topics for the project.
         :param pulumi.Input[bool] use_custom_template: Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+               	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         :param pulumi.Input[str] visibility_level: Set to `public` to create a public project.
         :param pulumi.Input[str] wiki_access_level: Set the wiki access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] wiki_enabled: Enable wiki for the project.
         """
         if allow_merge_on_skipped_pipeline is not None:
             pulumi.set(__self__, "allow_merge_on_skipped_pipeline", allow_merge_on_skipped_pipeline)
         if analytics_access_level is not None:
@@ -189,14 +228,18 @@
             pulumi.set(__self__, "auto_cancel_pending_pipelines", auto_cancel_pending_pipelines)
         if auto_devops_deploy_strategy is not None:
             pulumi.set(__self__, "auto_devops_deploy_strategy", auto_devops_deploy_strategy)
         if auto_devops_enabled is not None:
             pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
         if autoclose_referenced_issues is not None:
             pulumi.set(__self__, "autoclose_referenced_issues", autoclose_referenced_issues)
+        if avatar is not None:
+            pulumi.set(__self__, "avatar", avatar)
+        if avatar_hash is not None:
+            pulumi.set(__self__, "avatar_hash", avatar_hash)
         if build_coverage_regex is not None:
             warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
             pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
         if build_coverage_regex is not None:
             pulumi.set(__self__, "build_coverage_regex", build_coverage_regex)
         if build_git_strategy is not None:
             pulumi.set(__self__, "build_git_strategy", build_git_strategy)
@@ -206,42 +249,61 @@
             pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path is not None:
             pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth is not None:
             pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
         if ci_forward_deployment_enabled is not None:
             pulumi.set(__self__, "ci_forward_deployment_enabled", ci_forward_deployment_enabled)
+        if ci_separated_caches is not None:
+            pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policy is not None:
             pulumi.set(__self__, "container_expiration_policy", container_expiration_policy)
         if container_registry_access_level is not None:
             pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         if container_registry_enabled is not None:
+            warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+            pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
+        if container_registry_enabled is not None:
             pulumi.set(__self__, "container_registry_enabled", container_registry_enabled)
         if default_branch is not None:
             pulumi.set(__self__, "default_branch", default_branch)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if emails_disabled is not None:
             pulumi.set(__self__, "emails_disabled", emails_disabled)
+        if environments_access_level is not None:
+            pulumi.set(__self__, "environments_access_level", environments_access_level)
         if external_authorization_classification_label is not None:
             pulumi.set(__self__, "external_authorization_classification_label", external_authorization_classification_label)
+        if feature_flags_access_level is not None:
+            pulumi.set(__self__, "feature_flags_access_level", feature_flags_access_level)
+        if forked_from_project_id is not None:
+            pulumi.set(__self__, "forked_from_project_id", forked_from_project_id)
         if forking_access_level is not None:
             pulumi.set(__self__, "forking_access_level", forking_access_level)
         if group_with_project_templates_id is not None:
             pulumi.set(__self__, "group_with_project_templates_id", group_with_project_templates_id)
         if import_url is not None:
             pulumi.set(__self__, "import_url", import_url)
+        if import_url_password is not None:
+            pulumi.set(__self__, "import_url_password", import_url_password)
+        if import_url_username is not None:
+            pulumi.set(__self__, "import_url_username", import_url_username)
+        if infrastructure_access_level is not None:
+            pulumi.set(__self__, "infrastructure_access_level", infrastructure_access_level)
         if initialize_with_readme is not None:
             pulumi.set(__self__, "initialize_with_readme", initialize_with_readme)
         if issues_access_level is not None:
             pulumi.set(__self__, "issues_access_level", issues_access_level)
         if issues_enabled is not None:
             pulumi.set(__self__, "issues_enabled", issues_enabled)
         if issues_template is not None:
             pulumi.set(__self__, "issues_template", issues_template)
+        if keep_latest_artifact is not None:
+            pulumi.set(__self__, "keep_latest_artifact", keep_latest_artifact)
         if lfs_enabled is not None:
             pulumi.set(__self__, "lfs_enabled", lfs_enabled)
         if merge_commit_template is not None:
             pulumi.set(__self__, "merge_commit_template", merge_commit_template)
         if merge_method is not None:
             pulumi.set(__self__, "merge_method", merge_method)
         if merge_pipelines_enabled is not None:
@@ -256,14 +318,18 @@
             pulumi.set(__self__, "merge_trains_enabled", merge_trains_enabled)
         if mirror is not None:
             pulumi.set(__self__, "mirror", mirror)
         if mirror_overwrites_diverged_branches is not None:
             pulumi.set(__self__, "mirror_overwrites_diverged_branches", mirror_overwrites_diverged_branches)
         if mirror_trigger_builds is not None:
             pulumi.set(__self__, "mirror_trigger_builds", mirror_trigger_builds)
+        if monitor_access_level is not None:
+            pulumi.set(__self__, "monitor_access_level", monitor_access_level)
+        if mr_default_target_self is not None:
+            pulumi.set(__self__, "mr_default_target_self", mr_default_target_self)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace_id is not None:
             pulumi.set(__self__, "namespace_id", namespace_id)
         if only_allow_merge_if_all_discussions_are_resolved is not None:
             pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         if only_allow_merge_if_pipeline_succeeds is not None:
@@ -275,47 +341,56 @@
         if packages_enabled is not None:
             pulumi.set(__self__, "packages_enabled", packages_enabled)
         if pages_access_level is not None:
             pulumi.set(__self__, "pages_access_level", pages_access_level)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if pipelines_enabled is not None:
+            warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+            pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
+        if pipelines_enabled is not None:
             pulumi.set(__self__, "pipelines_enabled", pipelines_enabled)
         if printing_merge_request_link_enabled is not None:
             pulumi.set(__self__, "printing_merge_request_link_enabled", printing_merge_request_link_enabled)
         if public_builds is not None:
             pulumi.set(__self__, "public_builds", public_builds)
         if push_rules is not None:
             pulumi.set(__self__, "push_rules", push_rules)
+        if releases_access_level is not None:
+            pulumi.set(__self__, "releases_access_level", releases_access_level)
         if remove_source_branch_after_merge is not None:
             pulumi.set(__self__, "remove_source_branch_after_merge", remove_source_branch_after_merge)
         if repository_access_level is not None:
             pulumi.set(__self__, "repository_access_level", repository_access_level)
         if repository_storage is not None:
             pulumi.set(__self__, "repository_storage", repository_storage)
         if request_access_enabled is not None:
             pulumi.set(__self__, "request_access_enabled", request_access_enabled)
         if requirements_access_level is not None:
             pulumi.set(__self__, "requirements_access_level", requirements_access_level)
         if resolve_outdated_diff_discussions is not None:
             pulumi.set(__self__, "resolve_outdated_diff_discussions", resolve_outdated_diff_discussions)
+        if restrict_user_defined_variables is not None:
+            pulumi.set(__self__, "restrict_user_defined_variables", restrict_user_defined_variables)
         if security_and_compliance_access_level is not None:
             pulumi.set(__self__, "security_and_compliance_access_level", security_and_compliance_access_level)
         if shared_runners_enabled is not None:
             pulumi.set(__self__, "shared_runners_enabled", shared_runners_enabled)
         if skip_wait_for_default_branch_protection is not None:
             pulumi.set(__self__, "skip_wait_for_default_branch_protection", skip_wait_for_default_branch_protection)
         if snippets_access_level is not None:
             pulumi.set(__self__, "snippets_access_level", snippets_access_level)
         if snippets_enabled is not None:
             pulumi.set(__self__, "snippets_enabled", snippets_enabled)
         if squash_commit_template is not None:
             pulumi.set(__self__, "squash_commit_template", squash_commit_template)
         if squash_option is not None:
             pulumi.set(__self__, "squash_option", squash_option)
+        if suggestion_commit_message is not None:
+            pulumi.set(__self__, "suggestion_commit_message", suggestion_commit_message)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template_name is not None:
             pulumi.set(__self__, "template_name", template_name)
         if template_project_id is not None:
             pulumi.set(__self__, "template_project_id", template_project_id)
         if topics is not None:
@@ -437,14 +512,38 @@
         return pulumi.get(self, "autoclose_referenced_issues")
 
     @autoclose_referenced_issues.setter
     def autoclose_referenced_issues(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "autoclose_referenced_issues", value)
 
     @property
+    @pulumi.getter
+    def avatar(self) -> Optional[pulumi.Input[str]]:
+        """
+        A local path to the avatar image to upload. **Note**: not available for imported resources.
+        """
+        return pulumi.get(self, "avatar")
+
+    @avatar.setter
+    def avatar(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "avatar", value)
+
+    @property
+    @pulumi.getter(name="avatarHash")
+    def avatar_hash(self) -> Optional[pulumi.Input[str]]:
+        """
+        The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
+        """
+        return pulumi.get(self, "avatar_hash")
+
+    @avatar_hash.setter
+    def avatar_hash(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "avatar_hash", value)
+
+    @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> Optional[pulumi.Input[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
         return pulumi.get(self, "build_coverage_regex")
 
@@ -521,14 +620,26 @@
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @ci_forward_deployment_enabled.setter
     def ci_forward_deployment_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ci_forward_deployment_enabled", value)
 
     @property
+    @pulumi.getter(name="ciSeparatedCaches")
+    def ci_separated_caches(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Use separate caches for protected branches.
+        """
+        return pulumi.get(self, "ci_separated_caches")
+
+    @ci_separated_caches.setter
+    def ci_separated_caches(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ci_separated_caches", value)
+
+    @property
     @pulumi.getter(name="containerExpirationPolicy")
     def container_expiration_policy(self) -> Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']]:
         """
         Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         """
         return pulumi.get(self, "container_expiration_policy")
 
@@ -593,26 +704,62 @@
         return pulumi.get(self, "emails_disabled")
 
     @emails_disabled.setter
     def emails_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "emails_disabled", value)
 
     @property
+    @pulumi.getter(name="environmentsAccessLevel")
+    def environments_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "environments_access_level")
+
+    @environments_access_level.setter
+    def environments_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "environments_access_level", value)
+
+    @property
     @pulumi.getter(name="externalAuthorizationClassificationLabel")
     def external_authorization_classification_label(self) -> Optional[pulumi.Input[str]]:
         """
         The classification label for the project.
         """
         return pulumi.get(self, "external_authorization_classification_label")
 
     @external_authorization_classification_label.setter
     def external_authorization_classification_label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_authorization_classification_label", value)
 
     @property
+    @pulumi.getter(name="featureFlagsAccessLevel")
+    def feature_flags_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "feature_flags_access_level")
+
+    @feature_flags_access_level.setter
+    def feature_flags_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "feature_flags_access_level", value)
+
+    @property
+    @pulumi.getter(name="forkedFromProjectId")
+    def forked_from_project_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
+        """
+        return pulumi.get(self, "forked_from_project_id")
+
+    @forked_from_project_id.setter
+    def forked_from_project_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "forked_from_project_id", value)
+
+    @property
     @pulumi.getter(name="forkingAccessLevel")
     def forking_access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "forking_access_level")
 
@@ -632,23 +779,67 @@
     def group_with_project_templates_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "group_with_project_templates_id", value)
 
     @property
     @pulumi.getter(name="importUrl")
     def import_url(self) -> Optional[pulumi.Input[str]]:
         """
-        Git URL to a repository to be imported.
+        Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+        together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+        Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+        credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+        `terraform import`. See the examples section for how to properly use it.
         """
         return pulumi.get(self, "import_url")
 
     @import_url.setter
     def import_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "import_url", value)
 
     @property
+    @pulumi.getter(name="importUrlPassword")
+    def import_url_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_password")
+
+    @import_url_password.setter
+    def import_url_password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "import_url_password", value)
+
+    @property
+    @pulumi.getter(name="importUrlUsername")
+    def import_url_username(self) -> Optional[pulumi.Input[str]]:
+        """
+        The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_username")
+
+    @import_url_username.setter
+    def import_url_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "import_url_username", value)
+
+    @property
+    @pulumi.getter(name="infrastructureAccessLevel")
+    def infrastructure_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "infrastructure_access_level")
+
+    @infrastructure_access_level.setter
+    def infrastructure_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "infrastructure_access_level", value)
+
+    @property
     @pulumi.getter(name="initializeWithReadme")
     def initialize_with_readme(self) -> Optional[pulumi.Input[bool]]:
         """
         Create main branch with first commit containing a README.md file.
         """
         return pulumi.get(self, "initialize_with_readme")
 
@@ -689,14 +880,26 @@
         return pulumi.get(self, "issues_template")
 
     @issues_template.setter
     def issues_template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issues_template", value)
 
     @property
+    @pulumi.getter(name="keepLatestArtifact")
+    def keep_latest_artifact(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Disable or enable the ability to keep the latest artifact for this project.
+        """
+        return pulumi.get(self, "keep_latest_artifact")
+
+    @keep_latest_artifact.setter
+    def keep_latest_artifact(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "keep_latest_artifact", value)
+
+    @property
     @pulumi.getter(name="lfsEnabled")
     def lfs_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable LFS for the project.
         """
         return pulumi.get(self, "lfs_enabled")
 
@@ -716,15 +919,15 @@
     def merge_commit_template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "merge_commit_template", value)
 
     @property
     @pulumi.getter(name="mergeMethod")
     def merge_method(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to `ff` to create fast-forward merges
+        Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         """
         return pulumi.get(self, "merge_method")
 
     @merge_method.setter
     def merge_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "merge_method", value)
 
@@ -821,14 +1024,38 @@
         return pulumi.get(self, "mirror_trigger_builds")
 
     @mirror_trigger_builds.setter
     def mirror_trigger_builds(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mirror_trigger_builds", value)
 
     @property
+    @pulumi.getter(name="monitorAccessLevel")
+    def monitor_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "monitor_access_level")
+
+    @monitor_access_level.setter
+    def monitor_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "monitor_access_level", value)
+
+    @property
+    @pulumi.getter(name="mrDefaultTargetSelf")
+    def mr_default_target_self(self) -> Optional[pulumi.Input[bool]]:
+        """
+        For forked projects, target merge requests to this project. If false, the target will be the upstream project.
+        """
+        return pulumi.get(self, "mr_default_target_self")
+
+    @mr_default_target_self.setter
+    def mr_default_target_self(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mr_default_target_self", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the project.
         """
         return pulumi.get(self, "name")
 
@@ -932,15 +1159,15 @@
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
     def pipelines_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable pipelines for the project.
+        Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
         return pulumi.get(self, "pipelines_enabled")
 
     @pipelines_enabled.setter
     def pipelines_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pipelines_enabled", value)
 
@@ -977,14 +1204,26 @@
         return pulumi.get(self, "push_rules")
 
     @push_rules.setter
     def push_rules(self, value: Optional[pulumi.Input['ProjectPushRulesArgs']]):
         pulumi.set(self, "push_rules", value)
 
     @property
+    @pulumi.getter(name="releasesAccessLevel")
+    def releases_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "releases_access_level")
+
+    @releases_access_level.setter
+    def releases_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "releases_access_level", value)
+
+    @property
     @pulumi.getter(name="removeSourceBranchAfterMerge")
     def remove_source_branch_after_merge(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable `Delete source branch` option by default for all new merge requests.
         """
         return pulumi.get(self, "remove_source_branch_after_merge")
 
@@ -1049,14 +1288,26 @@
         return pulumi.get(self, "resolve_outdated_diff_discussions")
 
     @resolve_outdated_diff_discussions.setter
     def resolve_outdated_diff_discussions(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "resolve_outdated_diff_discussions", value)
 
     @property
+    @pulumi.getter(name="restrictUserDefinedVariables")
+    def restrict_user_defined_variables(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
+        """
+        return pulumi.get(self, "restrict_user_defined_variables")
+
+    @restrict_user_defined_variables.setter
+    def restrict_user_defined_variables(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "restrict_user_defined_variables", value)
+
+    @property
     @pulumi.getter(name="securityAndComplianceAccessLevel")
     def security_and_compliance_access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Set the security and compliance access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "security_and_compliance_access_level")
 
@@ -1136,14 +1387,26 @@
         return pulumi.get(self, "squash_option")
 
     @squash_option.setter
     def squash_option(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "squash_option", value)
 
     @property
+    @pulumi.getter(name="suggestionCommitMessage")
+    def suggestion_commit_message(self) -> Optional[pulumi.Input[str]]:
+        """
+        The commit message used to apply merge request suggestions.
+        """
+        return pulumi.get(self, "suggestion_commit_message")
+
+    @suggestion_commit_message.setter
+    def suggestion_commit_message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "suggestion_commit_message", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         """
         return pulumi.get(self, "tags")
 
@@ -1188,14 +1451,15 @@
         pulumi.set(self, "topics", value)
 
     @property
     @pulumi.getter(name="useCustomTemplate")
     def use_custom_template(self) -> Optional[pulumi.Input[bool]]:
         """
         Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+        	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         """
         return pulumi.get(self, "use_custom_template")
 
     @use_custom_template.setter
     def use_custom_template(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_custom_template", value)
 
@@ -1244,76 +1508,92 @@
                  approvals_before_merge: Optional[pulumi.Input[int]] = None,
                  archive_on_destroy: Optional[pulumi.Input[bool]] = None,
                  archived: Optional[pulumi.Input[bool]] = None,
                  auto_cancel_pending_pipelines: Optional[pulumi.Input[str]] = None,
                  auto_devops_deploy_strategy: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  autoclose_referenced_issues: Optional[pulumi.Input[bool]] = None,
+                 avatar: Optional[pulumi.Input[str]] = None,
+                 avatar_hash: Optional[pulumi.Input[str]] = None,
+                 avatar_url: Optional[pulumi.Input[str]] = None,
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
+                 environments_access_level: Optional[pulumi.Input[str]] = None,
                  external_authorization_classification_label: Optional[pulumi.Input[str]] = None,
+                 feature_flags_access_level: Optional[pulumi.Input[str]] = None,
+                 forked_from_project_id: Optional[pulumi.Input[int]] = None,
                  forking_access_level: Optional[pulumi.Input[str]] = None,
                  group_with_project_templates_id: Optional[pulumi.Input[int]] = None,
                  http_url_to_repo: Optional[pulumi.Input[str]] = None,
                  import_url: Optional[pulumi.Input[str]] = None,
+                 import_url_password: Optional[pulumi.Input[str]] = None,
+                 import_url_username: Optional[pulumi.Input[str]] = None,
+                 infrastructure_access_level: Optional[pulumi.Input[str]] = None,
                  initialize_with_readme: Optional[pulumi.Input[bool]] = None,
                  issues_access_level: Optional[pulumi.Input[str]] = None,
                  issues_enabled: Optional[pulumi.Input[bool]] = None,
                  issues_template: Optional[pulumi.Input[str]] = None,
+                 keep_latest_artifact: Optional[pulumi.Input[bool]] = None,
                  lfs_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_commit_template: Optional[pulumi.Input[str]] = None,
                  merge_method: Optional[pulumi.Input[str]] = None,
                  merge_pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_access_level: Optional[pulumi.Input[str]] = None,
                  merge_requests_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_template: Optional[pulumi.Input[str]] = None,
                  merge_trains_enabled: Optional[pulumi.Input[bool]] = None,
                  mirror: Optional[pulumi.Input[bool]] = None,
                  mirror_overwrites_diverged_branches: Optional[pulumi.Input[bool]] = None,
                  mirror_trigger_builds: Optional[pulumi.Input[bool]] = None,
+                 monitor_access_level: Optional[pulumi.Input[str]] = None,
+                 mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
                  operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  path_with_namespace: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input['ProjectPushRulesArgs']] = None,
+                 releases_access_level: Optional[pulumi.Input[str]] = None,
                  remove_source_branch_after_merge: Optional[pulumi.Input[bool]] = None,
                  repository_access_level: Optional[pulumi.Input[str]] = None,
                  repository_storage: Optional[pulumi.Input[str]] = None,
                  request_access_enabled: Optional[pulumi.Input[bool]] = None,
                  requirements_access_level: Optional[pulumi.Input[str]] = None,
                  resolve_outdated_diff_discussions: Optional[pulumi.Input[bool]] = None,
+                 restrict_user_defined_variables: Optional[pulumi.Input[bool]] = None,
                  runners_token: Optional[pulumi.Input[str]] = None,
                  security_and_compliance_access_level: Optional[pulumi.Input[str]] = None,
                  shared_runners_enabled: Optional[pulumi.Input[bool]] = None,
                  skip_wait_for_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  snippets_access_level: Optional[pulumi.Input[str]] = None,
                  snippets_enabled: Optional[pulumi.Input[bool]] = None,
                  squash_commit_template: Optional[pulumi.Input[str]] = None,
                  squash_option: Optional[pulumi.Input[str]] = None,
                  ssh_url_to_repo: Optional[pulumi.Input[str]] = None,
+                 suggestion_commit_message: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  template_project_id: Optional[pulumi.Input[int]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_custom_template: Optional[pulumi.Input[bool]] = None,
                  visibility_level: Optional[pulumi.Input[str]] = None,
                  web_url: Optional[pulumi.Input[str]] = None,
@@ -1329,84 +1609,109 @@
                In the meantime we recommend against using this attribute and use `ProjectApprovalRule` instead.
         :param pulumi.Input[bool] archive_on_destroy: Set to `true` to archive the project instead of deleting on destroy. If set to `true` it will entire omit the `DELETE` operation.
         :param pulumi.Input[bool] archived: Whether the project is in read-only mode (archived). Repositories can be archived/unarchived by toggling this parameter.
         :param pulumi.Input[str] auto_cancel_pending_pipelines: Auto-cancel pending pipelines. This isn’t a boolean, but enabled/disabled.
         :param pulumi.Input[str] auto_devops_deploy_strategy: Auto Deploy strategy. Valid values are `continuous`, `manual`, `timed_incremental`.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for this project.
         :param pulumi.Input[bool] autoclose_referenced_issues: Set whether auto-closing referenced issues on default branch.
+        :param pulumi.Input[str] avatar: A local path to the avatar image to upload. **Note**: not available for imported resources.
+        :param pulumi.Input[str] avatar_hash: The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
+        :param pulumi.Input[str] avatar_url: The URL of the avatar image.
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input['ProjectContainerExpirationPolicyArgs'] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
+        :param pulumi.Input[str] environments_access_level: Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] external_authorization_classification_label: The classification label for the project.
+        :param pulumi.Input[str] feature_flags_access_level: Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[int] forked_from_project_id: The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
         :param pulumi.Input[str] forking_access_level: Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[int] group_with_project_templates_id: For group-level custom templates, specifies ID of group from which all the custom project templates are sourced. Leave empty for instance-level templates. Requires use*custom*template to be true (enterprise edition).
         :param pulumi.Input[str] http_url_to_repo: URL that can be provided to `git clone` to clone the
-        :param pulumi.Input[str] import_url: Git URL to a repository to be imported.
+        :param pulumi.Input[str] import_url: Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+               together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+               Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+               credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+               `terraform import`. See the examples section for how to properly use it.
+        :param pulumi.Input[str] import_url_password: The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] import_url_username: The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] infrastructure_access_level: Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] initialize_with_readme: Create main branch with first commit containing a README.md file.
         :param pulumi.Input[str] issues_access_level: Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] issues_enabled: Enable issue tracking for the project.
         :param pulumi.Input[str] issues_template: Sets the template for new issues in the project.
+        :param pulumi.Input[bool] keep_latest_artifact: Disable or enable the ability to keep the latest artifact for this project.
         :param pulumi.Input[bool] lfs_enabled: Enable LFS for the project.
         :param pulumi.Input[str] merge_commit_template: Template used to create merge commit message in merge requests. (Introduced in GitLab 14.5.)
-        :param pulumi.Input[str] merge_method: Set to `ff` to create fast-forward merges
+        :param pulumi.Input[str] merge_method: Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         :param pulumi.Input[bool] merge_pipelines_enabled: Enable or disable merge pipelines.
         :param pulumi.Input[str] merge_requests_access_level: Set the merge requests access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] merge_requests_enabled: Enable merge requests for the project.
         :param pulumi.Input[str] merge_requests_template: Sets the template for new merge requests in the project.
         :param pulumi.Input[bool] merge_trains_enabled: Enable or disable merge trains. Requires `merge_pipelines_enabled` to be set to `true` to take effect.
         :param pulumi.Input[bool] mirror: Enable project pull mirror.
         :param pulumi.Input[bool] mirror_overwrites_diverged_branches: Enable overwrite diverged branches for a mirrored project.
         :param pulumi.Input[bool] mirror_trigger_builds: Enable trigger builds on pushes for a mirrored project.
+        :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
         :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[str] path_with_namespace: The path of the repository with namespace.
-        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project.
+        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input['ProjectPushRulesArgs'] push_rules: Push rules for the project.
+        :param pulumi.Input[str] releases_access_level: Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] remove_source_branch_after_merge: Enable `Delete source branch` option by default for all new merge requests.
         :param pulumi.Input[str] repository_access_level: Set the repository access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] repository_storage: Which storage shard the repository is on. (administrator only)
         :param pulumi.Input[bool] request_access_enabled: Allow users to request member access.
         :param pulumi.Input[str] requirements_access_level: Set the requirements access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] resolve_outdated_diff_discussions: Automatically resolve merge request diffs discussions on lines changed with a push.
+        :param pulumi.Input[bool] restrict_user_defined_variables: Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
         :param pulumi.Input[str] runners_token: Registration token to use during runner setup.
         :param pulumi.Input[str] security_and_compliance_access_level: Set the security and compliance access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] shared_runners_enabled: Enable shared runners for this project.
         :param pulumi.Input[bool] skip_wait_for_default_branch_protection: If `true`, the default behavior to wait for the default branch protection to be created is skipped.
                This is necessary if the current user is not an admin and the default branch protection is disabled on an instance-level.
                There is currently no known way to determine if the default branch protection is disabled on an instance-level for non-admin users.
                This attribute is only used during resource creation, thus changes are suppressed and the attribute cannot be imported.
         :param pulumi.Input[str] snippets_access_level: Set the snippets access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] snippets_enabled: Enable snippets for the project.
         :param pulumi.Input[str] squash_commit_template: Template used to create squash commit message in merge requests. (Introduced in GitLab 14.6.)
         :param pulumi.Input[str] squash_option: Squash commits when merge request. Valid values are `never`, `always`, `default_on`, or `default_off`. The default value is `default_off`. [GitLab >= 14.1]
         :param pulumi.Input[str] ssh_url_to_repo: URL that can be provided to `git clone` to clone the
+        :param pulumi.Input[str] suggestion_commit_message: The commit message used to apply merge request suggestions.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         :param pulumi.Input[str] template_name: When used without use*custom*template, name of a built-in project template. When used with use*custom*template, name of a custom project template. This option is mutually exclusive with `template_project_id`.
         :param pulumi.Input[int] template_project_id: When used with use*custom*template, project ID of a custom project template. This is preferable to using template*name since template*name may be ambiguous (enterprise edition). This option is mutually exclusive with `template_name`. See `GroupProjectFileTemplate` to set a project as a template project. If a project has not been set as a template, using it here will result in an error.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] topics: The list of topics for the project.
         :param pulumi.Input[bool] use_custom_template: Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+               	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         :param pulumi.Input[str] visibility_level: Set to `public` to create a public project.
         :param pulumi.Input[str] web_url: URL that can be used to find the project in a browser.
         :param pulumi.Input[str] wiki_access_level: Set the wiki access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] wiki_enabled: Enable wiki for the project.
         """
         if allow_merge_on_skipped_pipeline is not None:
             pulumi.set(__self__, "allow_merge_on_skipped_pipeline", allow_merge_on_skipped_pipeline)
@@ -1422,14 +1727,20 @@
             pulumi.set(__self__, "auto_cancel_pending_pipelines", auto_cancel_pending_pipelines)
         if auto_devops_deploy_strategy is not None:
             pulumi.set(__self__, "auto_devops_deploy_strategy", auto_devops_deploy_strategy)
         if auto_devops_enabled is not None:
             pulumi.set(__self__, "auto_devops_enabled", auto_devops_enabled)
         if autoclose_referenced_issues is not None:
             pulumi.set(__self__, "autoclose_referenced_issues", autoclose_referenced_issues)
+        if avatar is not None:
+            pulumi.set(__self__, "avatar", avatar)
+        if avatar_hash is not None:
+            pulumi.set(__self__, "avatar_hash", avatar_hash)
+        if avatar_url is not None:
+            pulumi.set(__self__, "avatar_url", avatar_url)
         if build_coverage_regex is not None:
             warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
             pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
         if build_coverage_regex is not None:
             pulumi.set(__self__, "build_coverage_regex", build_coverage_regex)
         if build_git_strategy is not None:
             pulumi.set(__self__, "build_git_strategy", build_git_strategy)
@@ -1439,44 +1750,63 @@
             pulumi.set(__self__, "builds_access_level", builds_access_level)
         if ci_config_path is not None:
             pulumi.set(__self__, "ci_config_path", ci_config_path)
         if ci_default_git_depth is not None:
             pulumi.set(__self__, "ci_default_git_depth", ci_default_git_depth)
         if ci_forward_deployment_enabled is not None:
             pulumi.set(__self__, "ci_forward_deployment_enabled", ci_forward_deployment_enabled)
+        if ci_separated_caches is not None:
+            pulumi.set(__self__, "ci_separated_caches", ci_separated_caches)
         if container_expiration_policy is not None:
             pulumi.set(__self__, "container_expiration_policy", container_expiration_policy)
         if container_registry_access_level is not None:
             pulumi.set(__self__, "container_registry_access_level", container_registry_access_level)
         if container_registry_enabled is not None:
+            warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+            pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
+        if container_registry_enabled is not None:
             pulumi.set(__self__, "container_registry_enabled", container_registry_enabled)
         if default_branch is not None:
             pulumi.set(__self__, "default_branch", default_branch)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if emails_disabled is not None:
             pulumi.set(__self__, "emails_disabled", emails_disabled)
+        if environments_access_level is not None:
+            pulumi.set(__self__, "environments_access_level", environments_access_level)
         if external_authorization_classification_label is not None:
             pulumi.set(__self__, "external_authorization_classification_label", external_authorization_classification_label)
+        if feature_flags_access_level is not None:
+            pulumi.set(__self__, "feature_flags_access_level", feature_flags_access_level)
+        if forked_from_project_id is not None:
+            pulumi.set(__self__, "forked_from_project_id", forked_from_project_id)
         if forking_access_level is not None:
             pulumi.set(__self__, "forking_access_level", forking_access_level)
         if group_with_project_templates_id is not None:
             pulumi.set(__self__, "group_with_project_templates_id", group_with_project_templates_id)
         if http_url_to_repo is not None:
             pulumi.set(__self__, "http_url_to_repo", http_url_to_repo)
         if import_url is not None:
             pulumi.set(__self__, "import_url", import_url)
+        if import_url_password is not None:
+            pulumi.set(__self__, "import_url_password", import_url_password)
+        if import_url_username is not None:
+            pulumi.set(__self__, "import_url_username", import_url_username)
+        if infrastructure_access_level is not None:
+            pulumi.set(__self__, "infrastructure_access_level", infrastructure_access_level)
         if initialize_with_readme is not None:
             pulumi.set(__self__, "initialize_with_readme", initialize_with_readme)
         if issues_access_level is not None:
             pulumi.set(__self__, "issues_access_level", issues_access_level)
         if issues_enabled is not None:
             pulumi.set(__self__, "issues_enabled", issues_enabled)
         if issues_template is not None:
             pulumi.set(__self__, "issues_template", issues_template)
+        if keep_latest_artifact is not None:
+            pulumi.set(__self__, "keep_latest_artifact", keep_latest_artifact)
         if lfs_enabled is not None:
             pulumi.set(__self__, "lfs_enabled", lfs_enabled)
         if merge_commit_template is not None:
             pulumi.set(__self__, "merge_commit_template", merge_commit_template)
         if merge_method is not None:
             pulumi.set(__self__, "merge_method", merge_method)
         if merge_pipelines_enabled is not None:
@@ -1491,14 +1821,18 @@
             pulumi.set(__self__, "merge_trains_enabled", merge_trains_enabled)
         if mirror is not None:
             pulumi.set(__self__, "mirror", mirror)
         if mirror_overwrites_diverged_branches is not None:
             pulumi.set(__self__, "mirror_overwrites_diverged_branches", mirror_overwrites_diverged_branches)
         if mirror_trigger_builds is not None:
             pulumi.set(__self__, "mirror_trigger_builds", mirror_trigger_builds)
+        if monitor_access_level is not None:
+            pulumi.set(__self__, "monitor_access_level", monitor_access_level)
+        if mr_default_target_self is not None:
+            pulumi.set(__self__, "mr_default_target_self", mr_default_target_self)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if namespace_id is not None:
             pulumi.set(__self__, "namespace_id", namespace_id)
         if only_allow_merge_if_all_discussions_are_resolved is not None:
             pulumi.set(__self__, "only_allow_merge_if_all_discussions_are_resolved", only_allow_merge_if_all_discussions_are_resolved)
         if only_allow_merge_if_pipeline_succeeds is not None:
@@ -1512,33 +1846,40 @@
         if pages_access_level is not None:
             pulumi.set(__self__, "pages_access_level", pages_access_level)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if path_with_namespace is not None:
             pulumi.set(__self__, "path_with_namespace", path_with_namespace)
         if pipelines_enabled is not None:
+            warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+            pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
+        if pipelines_enabled is not None:
             pulumi.set(__self__, "pipelines_enabled", pipelines_enabled)
         if printing_merge_request_link_enabled is not None:
             pulumi.set(__self__, "printing_merge_request_link_enabled", printing_merge_request_link_enabled)
         if public_builds is not None:
             pulumi.set(__self__, "public_builds", public_builds)
         if push_rules is not None:
             pulumi.set(__self__, "push_rules", push_rules)
+        if releases_access_level is not None:
+            pulumi.set(__self__, "releases_access_level", releases_access_level)
         if remove_source_branch_after_merge is not None:
             pulumi.set(__self__, "remove_source_branch_after_merge", remove_source_branch_after_merge)
         if repository_access_level is not None:
             pulumi.set(__self__, "repository_access_level", repository_access_level)
         if repository_storage is not None:
             pulumi.set(__self__, "repository_storage", repository_storage)
         if request_access_enabled is not None:
             pulumi.set(__self__, "request_access_enabled", request_access_enabled)
         if requirements_access_level is not None:
             pulumi.set(__self__, "requirements_access_level", requirements_access_level)
         if resolve_outdated_diff_discussions is not None:
             pulumi.set(__self__, "resolve_outdated_diff_discussions", resolve_outdated_diff_discussions)
+        if restrict_user_defined_variables is not None:
+            pulumi.set(__self__, "restrict_user_defined_variables", restrict_user_defined_variables)
         if runners_token is not None:
             pulumi.set(__self__, "runners_token", runners_token)
         if security_and_compliance_access_level is not None:
             pulumi.set(__self__, "security_and_compliance_access_level", security_and_compliance_access_level)
         if shared_runners_enabled is not None:
             pulumi.set(__self__, "shared_runners_enabled", shared_runners_enabled)
         if skip_wait_for_default_branch_protection is not None:
@@ -1549,14 +1890,16 @@
             pulumi.set(__self__, "snippets_enabled", snippets_enabled)
         if squash_commit_template is not None:
             pulumi.set(__self__, "squash_commit_template", squash_commit_template)
         if squash_option is not None:
             pulumi.set(__self__, "squash_option", squash_option)
         if ssh_url_to_repo is not None:
             pulumi.set(__self__, "ssh_url_to_repo", ssh_url_to_repo)
+        if suggestion_commit_message is not None:
+            pulumi.set(__self__, "suggestion_commit_message", suggestion_commit_message)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if template_name is not None:
             pulumi.set(__self__, "template_name", template_name)
         if template_project_id is not None:
             pulumi.set(__self__, "template_project_id", template_project_id)
         if topics is not None:
@@ -1680,14 +2023,50 @@
         return pulumi.get(self, "autoclose_referenced_issues")
 
     @autoclose_referenced_issues.setter
     def autoclose_referenced_issues(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "autoclose_referenced_issues", value)
 
     @property
+    @pulumi.getter
+    def avatar(self) -> Optional[pulumi.Input[str]]:
+        """
+        A local path to the avatar image to upload. **Note**: not available for imported resources.
+        """
+        return pulumi.get(self, "avatar")
+
+    @avatar.setter
+    def avatar(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "avatar", value)
+
+    @property
+    @pulumi.getter(name="avatarHash")
+    def avatar_hash(self) -> Optional[pulumi.Input[str]]:
+        """
+        The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
+        """
+        return pulumi.get(self, "avatar_hash")
+
+    @avatar_hash.setter
+    def avatar_hash(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "avatar_hash", value)
+
+    @property
+    @pulumi.getter(name="avatarUrl")
+    def avatar_url(self) -> Optional[pulumi.Input[str]]:
+        """
+        The URL of the avatar image.
+        """
+        return pulumi.get(self, "avatar_url")
+
+    @avatar_url.setter
+    def avatar_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "avatar_url", value)
+
+    @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> Optional[pulumi.Input[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
         return pulumi.get(self, "build_coverage_regex")
 
@@ -1764,14 +2143,26 @@
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @ci_forward_deployment_enabled.setter
     def ci_forward_deployment_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ci_forward_deployment_enabled", value)
 
     @property
+    @pulumi.getter(name="ciSeparatedCaches")
+    def ci_separated_caches(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Use separate caches for protected branches.
+        """
+        return pulumi.get(self, "ci_separated_caches")
+
+    @ci_separated_caches.setter
+    def ci_separated_caches(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ci_separated_caches", value)
+
+    @property
     @pulumi.getter(name="containerExpirationPolicy")
     def container_expiration_policy(self) -> Optional[pulumi.Input['ProjectContainerExpirationPolicyArgs']]:
         """
         Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         """
         return pulumi.get(self, "container_expiration_policy")
 
@@ -1836,26 +2227,62 @@
         return pulumi.get(self, "emails_disabled")
 
     @emails_disabled.setter
     def emails_disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "emails_disabled", value)
 
     @property
+    @pulumi.getter(name="environmentsAccessLevel")
+    def environments_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "environments_access_level")
+
+    @environments_access_level.setter
+    def environments_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "environments_access_level", value)
+
+    @property
     @pulumi.getter(name="externalAuthorizationClassificationLabel")
     def external_authorization_classification_label(self) -> Optional[pulumi.Input[str]]:
         """
         The classification label for the project.
         """
         return pulumi.get(self, "external_authorization_classification_label")
 
     @external_authorization_classification_label.setter
     def external_authorization_classification_label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "external_authorization_classification_label", value)
 
     @property
+    @pulumi.getter(name="featureFlagsAccessLevel")
+    def feature_flags_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "feature_flags_access_level")
+
+    @feature_flags_access_level.setter
+    def feature_flags_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "feature_flags_access_level", value)
+
+    @property
+    @pulumi.getter(name="forkedFromProjectId")
+    def forked_from_project_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
+        """
+        return pulumi.get(self, "forked_from_project_id")
+
+    @forked_from_project_id.setter
+    def forked_from_project_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "forked_from_project_id", value)
+
+    @property
     @pulumi.getter(name="forkingAccessLevel")
     def forking_access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "forking_access_level")
 
@@ -1887,23 +2314,67 @@
     def http_url_to_repo(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "http_url_to_repo", value)
 
     @property
     @pulumi.getter(name="importUrl")
     def import_url(self) -> Optional[pulumi.Input[str]]:
         """
-        Git URL to a repository to be imported.
+        Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+        together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+        Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+        credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+        `terraform import`. See the examples section for how to properly use it.
         """
         return pulumi.get(self, "import_url")
 
     @import_url.setter
     def import_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "import_url", value)
 
     @property
+    @pulumi.getter(name="importUrlPassword")
+    def import_url_password(self) -> Optional[pulumi.Input[str]]:
+        """
+        The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_password")
+
+    @import_url_password.setter
+    def import_url_password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "import_url_password", value)
+
+    @property
+    @pulumi.getter(name="importUrlUsername")
+    def import_url_username(self) -> Optional[pulumi.Input[str]]:
+        """
+        The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_username")
+
+    @import_url_username.setter
+    def import_url_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "import_url_username", value)
+
+    @property
+    @pulumi.getter(name="infrastructureAccessLevel")
+    def infrastructure_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "infrastructure_access_level")
+
+    @infrastructure_access_level.setter
+    def infrastructure_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "infrastructure_access_level", value)
+
+    @property
     @pulumi.getter(name="initializeWithReadme")
     def initialize_with_readme(self) -> Optional[pulumi.Input[bool]]:
         """
         Create main branch with first commit containing a README.md file.
         """
         return pulumi.get(self, "initialize_with_readme")
 
@@ -1944,14 +2415,26 @@
         return pulumi.get(self, "issues_template")
 
     @issues_template.setter
     def issues_template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issues_template", value)
 
     @property
+    @pulumi.getter(name="keepLatestArtifact")
+    def keep_latest_artifact(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Disable or enable the ability to keep the latest artifact for this project.
+        """
+        return pulumi.get(self, "keep_latest_artifact")
+
+    @keep_latest_artifact.setter
+    def keep_latest_artifact(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "keep_latest_artifact", value)
+
+    @property
     @pulumi.getter(name="lfsEnabled")
     def lfs_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable LFS for the project.
         """
         return pulumi.get(self, "lfs_enabled")
 
@@ -1971,15 +2454,15 @@
     def merge_commit_template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "merge_commit_template", value)
 
     @property
     @pulumi.getter(name="mergeMethod")
     def merge_method(self) -> Optional[pulumi.Input[str]]:
         """
-        Set to `ff` to create fast-forward merges
+        Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         """
         return pulumi.get(self, "merge_method")
 
     @merge_method.setter
     def merge_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "merge_method", value)
 
@@ -2076,14 +2559,38 @@
         return pulumi.get(self, "mirror_trigger_builds")
 
     @mirror_trigger_builds.setter
     def mirror_trigger_builds(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "mirror_trigger_builds", value)
 
     @property
+    @pulumi.getter(name="monitorAccessLevel")
+    def monitor_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "monitor_access_level")
+
+    @monitor_access_level.setter
+    def monitor_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "monitor_access_level", value)
+
+    @property
+    @pulumi.getter(name="mrDefaultTargetSelf")
+    def mr_default_target_self(self) -> Optional[pulumi.Input[bool]]:
+        """
+        For forked projects, target merge requests to this project. If false, the target will be the upstream project.
+        """
+        return pulumi.get(self, "mr_default_target_self")
+
+    @mr_default_target_self.setter
+    def mr_default_target_self(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mr_default_target_self", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the project.
         """
         return pulumi.get(self, "name")
 
@@ -2199,15 +2706,15 @@
     def path_with_namespace(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path_with_namespace", value)
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
     def pipelines_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable pipelines for the project.
+        Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
         return pulumi.get(self, "pipelines_enabled")
 
     @pipelines_enabled.setter
     def pipelines_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pipelines_enabled", value)
 
@@ -2244,14 +2751,26 @@
         return pulumi.get(self, "push_rules")
 
     @push_rules.setter
     def push_rules(self, value: Optional[pulumi.Input['ProjectPushRulesArgs']]):
         pulumi.set(self, "push_rules", value)
 
     @property
+    @pulumi.getter(name="releasesAccessLevel")
+    def releases_access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "releases_access_level")
+
+    @releases_access_level.setter
+    def releases_access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "releases_access_level", value)
+
+    @property
     @pulumi.getter(name="removeSourceBranchAfterMerge")
     def remove_source_branch_after_merge(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable `Delete source branch` option by default for all new merge requests.
         """
         return pulumi.get(self, "remove_source_branch_after_merge")
 
@@ -2316,14 +2835,26 @@
         return pulumi.get(self, "resolve_outdated_diff_discussions")
 
     @resolve_outdated_diff_discussions.setter
     def resolve_outdated_diff_discussions(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "resolve_outdated_diff_discussions", value)
 
     @property
+    @pulumi.getter(name="restrictUserDefinedVariables")
+    def restrict_user_defined_variables(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
+        """
+        return pulumi.get(self, "restrict_user_defined_variables")
+
+    @restrict_user_defined_variables.setter
+    def restrict_user_defined_variables(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "restrict_user_defined_variables", value)
+
+    @property
     @pulumi.getter(name="runnersToken")
     def runners_token(self) -> Optional[pulumi.Input[str]]:
         """
         Registration token to use during runner setup.
         """
         return pulumi.get(self, "runners_token")
 
@@ -2427,14 +2958,26 @@
         return pulumi.get(self, "ssh_url_to_repo")
 
     @ssh_url_to_repo.setter
     def ssh_url_to_repo(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_url_to_repo", value)
 
     @property
+    @pulumi.getter(name="suggestionCommitMessage")
+    def suggestion_commit_message(self) -> Optional[pulumi.Input[str]]:
+        """
+        The commit message used to apply merge request suggestions.
+        """
+        return pulumi.get(self, "suggestion_commit_message")
+
+    @suggestion_commit_message.setter
+    def suggestion_commit_message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "suggestion_commit_message", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         """
         return pulumi.get(self, "tags")
 
@@ -2479,14 +3022,15 @@
         pulumi.set(self, "topics", value)
 
     @property
     @pulumi.getter(name="useCustomTemplate")
     def use_custom_template(self) -> Optional[pulumi.Input[bool]]:
         """
         Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+        	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         """
         return pulumi.get(self, "use_custom_template")
 
     @use_custom_template.setter
     def use_custom_template(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_custom_template", value)
 
@@ -2549,72 +3093,87 @@
                  approvals_before_merge: Optional[pulumi.Input[int]] = None,
                  archive_on_destroy: Optional[pulumi.Input[bool]] = None,
                  archived: Optional[pulumi.Input[bool]] = None,
                  auto_cancel_pending_pipelines: Optional[pulumi.Input[str]] = None,
                  auto_devops_deploy_strategy: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  autoclose_referenced_issues: Optional[pulumi.Input[bool]] = None,
+                 avatar: Optional[pulumi.Input[str]] = None,
+                 avatar_hash: Optional[pulumi.Input[str]] = None,
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
+                 environments_access_level: Optional[pulumi.Input[str]] = None,
                  external_authorization_classification_label: Optional[pulumi.Input[str]] = None,
+                 feature_flags_access_level: Optional[pulumi.Input[str]] = None,
+                 forked_from_project_id: Optional[pulumi.Input[int]] = None,
                  forking_access_level: Optional[pulumi.Input[str]] = None,
                  group_with_project_templates_id: Optional[pulumi.Input[int]] = None,
                  import_url: Optional[pulumi.Input[str]] = None,
+                 import_url_password: Optional[pulumi.Input[str]] = None,
+                 import_url_username: Optional[pulumi.Input[str]] = None,
+                 infrastructure_access_level: Optional[pulumi.Input[str]] = None,
                  initialize_with_readme: Optional[pulumi.Input[bool]] = None,
                  issues_access_level: Optional[pulumi.Input[str]] = None,
                  issues_enabled: Optional[pulumi.Input[bool]] = None,
                  issues_template: Optional[pulumi.Input[str]] = None,
+                 keep_latest_artifact: Optional[pulumi.Input[bool]] = None,
                  lfs_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_commit_template: Optional[pulumi.Input[str]] = None,
                  merge_method: Optional[pulumi.Input[str]] = None,
                  merge_pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_access_level: Optional[pulumi.Input[str]] = None,
                  merge_requests_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_template: Optional[pulumi.Input[str]] = None,
                  merge_trains_enabled: Optional[pulumi.Input[bool]] = None,
                  mirror: Optional[pulumi.Input[bool]] = None,
                  mirror_overwrites_diverged_branches: Optional[pulumi.Input[bool]] = None,
                  mirror_trigger_builds: Optional[pulumi.Input[bool]] = None,
+                 monitor_access_level: Optional[pulumi.Input[str]] = None,
+                 mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
                  operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']]] = None,
+                 releases_access_level: Optional[pulumi.Input[str]] = None,
                  remove_source_branch_after_merge: Optional[pulumi.Input[bool]] = None,
                  repository_access_level: Optional[pulumi.Input[str]] = None,
                  repository_storage: Optional[pulumi.Input[str]] = None,
                  request_access_enabled: Optional[pulumi.Input[bool]] = None,
                  requirements_access_level: Optional[pulumi.Input[str]] = None,
                  resolve_outdated_diff_discussions: Optional[pulumi.Input[bool]] = None,
+                 restrict_user_defined_variables: Optional[pulumi.Input[bool]] = None,
                  security_and_compliance_access_level: Optional[pulumi.Input[str]] = None,
                  shared_runners_enabled: Optional[pulumi.Input[bool]] = None,
                  skip_wait_for_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  snippets_access_level: Optional[pulumi.Input[str]] = None,
                  snippets_enabled: Optional[pulumi.Input[bool]] = None,
                  squash_commit_template: Optional[pulumi.Input[str]] = None,
                  squash_option: Optional[pulumi.Input[str]] = None,
+                 suggestion_commit_message: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  template_project_id: Optional[pulumi.Input[int]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_custom_template: Optional[pulumi.Input[bool]] = None,
                  visibility_level: Optional[pulumi.Input[str]] = None,
                  wiki_access_level: Optional[pulumi.Input[str]] = None,
@@ -2637,108 +3196,165 @@
             member_check=True,
             prevent_secrets=True,
         ))
         peter_parker = gitlab.get_user(username="peter_parker")
         peters_repo = gitlab.Project("petersRepo",
             description="This is a description",
             namespace_id=peter_parker.namespace_id)
+        # Fork a project
+        fork_project = gitlab.Project("forkProject",
+            description="This is a fork",
+            forked_from_project_id=example.id)
+        # Fork a project and setup a pull mirror
+        fork_index_project_project = gitlab.Project("forkIndex/projectProject",
+            description="This is a fork",
+            forked_from_project_id=example.id,
+            import_url=example.http_url_to_repo,
+            mirror=True)
+        # Create a project by importing it from a public project
+        import_public = gitlab.Project("importPublic", import_url="https://gitlab.example.com/repo.git")
+        # Create a project by importing it from a public project and setup the pull mirror
+        import_public_with_mirror = gitlab.Project("importPublicWithMirror",
+            import_url="https://gitlab.example.com/repo.git",
+            mirror=True)
+        # Create a project by importing it from a private project
+        import_private_project = gitlab.Project("importPrivateProject",
+            import_url="https://gitlab.example.com/repo.git",
+            import_url_username="user",
+            import_url_password="pass")
+        # Create a project by importing it from a private project and setup the pull mirror
+        import_private_with_mirror = gitlab.Project("importPrivateWithMirror",
+            import_url="https://gitlab.example.com/repo.git",
+            import_url_username="user",
+            import_url_password="pass",
+            mirror=True)
+        # Create a project by importing it from a private project and provide credentials in `import_url`
+        # NOTE: only use this if you really must, use `import_url_username` and `import_url_password` whenever possible
+        #       GitLab API will always return the `import_url` without credentials, therefore you must ignore the `import_url` for changes:
+        import_private_index_project_project = gitlab.Project("importPrivateIndex/projectProject", import_url="https://user:pass@gitlab.example.com/repo.git")
         ```
 
         ## Import
 
         ```sh
          $ pulumi import gitlab:index/project:Project You can import a project state using `<resource> <id>`. The
         ```
 
          `id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
 
         ```sh
          $ pulumi import gitlab:index/project:Project example richardc/example
         ```
 
+         NOTEthe `import_url_username` and `import_url_password` cannot be imported.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_merge_on_skipped_pipeline: Set to true if you want to treat skipped pipelines as if they finished with success.
         :param pulumi.Input[str] analytics_access_level: Set the analytics access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[int] approvals_before_merge: Number of merge request approvals required for merging. Default is 0.
                This field **does not** work well in combination with the `ProjectApprovalRule` resource
                and is most likely gonna be deprecated in a future GitLab version (see [this upstream epic](https://gitlab.com/groups/gitlab-org/-/epics/7572)).
                In the meantime we recommend against using this attribute and use `ProjectApprovalRule` instead.
         :param pulumi.Input[bool] archive_on_destroy: Set to `true` to archive the project instead of deleting on destroy. If set to `true` it will entire omit the `DELETE` operation.
         :param pulumi.Input[bool] archived: Whether the project is in read-only mode (archived). Repositories can be archived/unarchived by toggling this parameter.
         :param pulumi.Input[str] auto_cancel_pending_pipelines: Auto-cancel pending pipelines. This isn’t a boolean, but enabled/disabled.
         :param pulumi.Input[str] auto_devops_deploy_strategy: Auto Deploy strategy. Valid values are `continuous`, `manual`, `timed_incremental`.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for this project.
         :param pulumi.Input[bool] autoclose_referenced_issues: Set whether auto-closing referenced issues on default branch.
+        :param pulumi.Input[str] avatar: A local path to the avatar image to upload. **Note**: not available for imported resources.
+        :param pulumi.Input[str] avatar_hash: The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
+        :param pulumi.Input[str] environments_access_level: Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] external_authorization_classification_label: The classification label for the project.
+        :param pulumi.Input[str] feature_flags_access_level: Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[int] forked_from_project_id: The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
         :param pulumi.Input[str] forking_access_level: Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[int] group_with_project_templates_id: For group-level custom templates, specifies ID of group from which all the custom project templates are sourced. Leave empty for instance-level templates. Requires use*custom*template to be true (enterprise edition).
-        :param pulumi.Input[str] import_url: Git URL to a repository to be imported.
+        :param pulumi.Input[str] import_url: Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+               together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+               Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+               credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+               `terraform import`. See the examples section for how to properly use it.
+        :param pulumi.Input[str] import_url_password: The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] import_url_username: The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] infrastructure_access_level: Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] initialize_with_readme: Create main branch with first commit containing a README.md file.
         :param pulumi.Input[str] issues_access_level: Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] issues_enabled: Enable issue tracking for the project.
         :param pulumi.Input[str] issues_template: Sets the template for new issues in the project.
+        :param pulumi.Input[bool] keep_latest_artifact: Disable or enable the ability to keep the latest artifact for this project.
         :param pulumi.Input[bool] lfs_enabled: Enable LFS for the project.
         :param pulumi.Input[str] merge_commit_template: Template used to create merge commit message in merge requests. (Introduced in GitLab 14.5.)
-        :param pulumi.Input[str] merge_method: Set to `ff` to create fast-forward merges
+        :param pulumi.Input[str] merge_method: Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         :param pulumi.Input[bool] merge_pipelines_enabled: Enable or disable merge pipelines.
         :param pulumi.Input[str] merge_requests_access_level: Set the merge requests access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] merge_requests_enabled: Enable merge requests for the project.
         :param pulumi.Input[str] merge_requests_template: Sets the template for new merge requests in the project.
         :param pulumi.Input[bool] merge_trains_enabled: Enable or disable merge trains. Requires `merge_pipelines_enabled` to be set to `true` to take effect.
         :param pulumi.Input[bool] mirror: Enable project pull mirror.
         :param pulumi.Input[bool] mirror_overwrites_diverged_branches: Enable overwrite diverged branches for a mirrored project.
         :param pulumi.Input[bool] mirror_trigger_builds: Enable trigger builds on pushes for a mirrored project.
+        :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
         :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
-        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project.
+        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']] push_rules: Push rules for the project.
+        :param pulumi.Input[str] releases_access_level: Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] remove_source_branch_after_merge: Enable `Delete source branch` option by default for all new merge requests.
         :param pulumi.Input[str] repository_access_level: Set the repository access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] repository_storage: Which storage shard the repository is on. (administrator only)
         :param pulumi.Input[bool] request_access_enabled: Allow users to request member access.
         :param pulumi.Input[str] requirements_access_level: Set the requirements access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] resolve_outdated_diff_discussions: Automatically resolve merge request diffs discussions on lines changed with a push.
+        :param pulumi.Input[bool] restrict_user_defined_variables: Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
         :param pulumi.Input[str] security_and_compliance_access_level: Set the security and compliance access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] shared_runners_enabled: Enable shared runners for this project.
         :param pulumi.Input[bool] skip_wait_for_default_branch_protection: If `true`, the default behavior to wait for the default branch protection to be created is skipped.
                This is necessary if the current user is not an admin and the default branch protection is disabled on an instance-level.
                There is currently no known way to determine if the default branch protection is disabled on an instance-level for non-admin users.
                This attribute is only used during resource creation, thus changes are suppressed and the attribute cannot be imported.
         :param pulumi.Input[str] snippets_access_level: Set the snippets access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] snippets_enabled: Enable snippets for the project.
         :param pulumi.Input[str] squash_commit_template: Template used to create squash commit message in merge requests. (Introduced in GitLab 14.6.)
         :param pulumi.Input[str] squash_option: Squash commits when merge request. Valid values are `never`, `always`, `default_on`, or `default_off`. The default value is `default_off`. [GitLab >= 14.1]
+        :param pulumi.Input[str] suggestion_commit_message: The commit message used to apply merge request suggestions.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         :param pulumi.Input[str] template_name: When used without use*custom*template, name of a built-in project template. When used with use*custom*template, name of a custom project template. This option is mutually exclusive with `template_project_id`.
         :param pulumi.Input[int] template_project_id: When used with use*custom*template, project ID of a custom project template. This is preferable to using template*name since template*name may be ambiguous (enterprise edition). This option is mutually exclusive with `template_name`. See `GroupProjectFileTemplate` to set a project as a template project. If a project has not been set as a template, using it here will result in an error.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] topics: The list of topics for the project.
         :param pulumi.Input[bool] use_custom_template: Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+               	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         :param pulumi.Input[str] visibility_level: Set to `public` to create a public project.
         :param pulumi.Input[str] wiki_access_level: Set the wiki access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] wiki_enabled: Enable wiki for the project.
         """
         ...
     @overload
     def __init__(__self__,
@@ -2762,28 +3378,61 @@
             member_check=True,
             prevent_secrets=True,
         ))
         peter_parker = gitlab.get_user(username="peter_parker")
         peters_repo = gitlab.Project("petersRepo",
             description="This is a description",
             namespace_id=peter_parker.namespace_id)
+        # Fork a project
+        fork_project = gitlab.Project("forkProject",
+            description="This is a fork",
+            forked_from_project_id=example.id)
+        # Fork a project and setup a pull mirror
+        fork_index_project_project = gitlab.Project("forkIndex/projectProject",
+            description="This is a fork",
+            forked_from_project_id=example.id,
+            import_url=example.http_url_to_repo,
+            mirror=True)
+        # Create a project by importing it from a public project
+        import_public = gitlab.Project("importPublic", import_url="https://gitlab.example.com/repo.git")
+        # Create a project by importing it from a public project and setup the pull mirror
+        import_public_with_mirror = gitlab.Project("importPublicWithMirror",
+            import_url="https://gitlab.example.com/repo.git",
+            mirror=True)
+        # Create a project by importing it from a private project
+        import_private_project = gitlab.Project("importPrivateProject",
+            import_url="https://gitlab.example.com/repo.git",
+            import_url_username="user",
+            import_url_password="pass")
+        # Create a project by importing it from a private project and setup the pull mirror
+        import_private_with_mirror = gitlab.Project("importPrivateWithMirror",
+            import_url="https://gitlab.example.com/repo.git",
+            import_url_username="user",
+            import_url_password="pass",
+            mirror=True)
+        # Create a project by importing it from a private project and provide credentials in `import_url`
+        # NOTE: only use this if you really must, use `import_url_username` and `import_url_password` whenever possible
+        #       GitLab API will always return the `import_url` without credentials, therefore you must ignore the `import_url` for changes:
+        import_private_index_project_project = gitlab.Project("importPrivateIndex/projectProject", import_url="https://user:pass@gitlab.example.com/repo.git")
         ```
 
         ## Import
 
         ```sh
          $ pulumi import gitlab:index/project:Project You can import a project state using `<resource> <id>`. The
         ```
 
          `id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
 
         ```sh
          $ pulumi import gitlab:index/project:Project example richardc/example
         ```
 
+         NOTEthe `import_url_username` and `import_url_password` cannot be imported.
+
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ProjectArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -2800,72 +3449,87 @@
                  approvals_before_merge: Optional[pulumi.Input[int]] = None,
                  archive_on_destroy: Optional[pulumi.Input[bool]] = None,
                  archived: Optional[pulumi.Input[bool]] = None,
                  auto_cancel_pending_pipelines: Optional[pulumi.Input[str]] = None,
                  auto_devops_deploy_strategy: Optional[pulumi.Input[str]] = None,
                  auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
                  autoclose_referenced_issues: Optional[pulumi.Input[bool]] = None,
+                 avatar: Optional[pulumi.Input[str]] = None,
+                 avatar_hash: Optional[pulumi.Input[str]] = None,
                  build_coverage_regex: Optional[pulumi.Input[str]] = None,
                  build_git_strategy: Optional[pulumi.Input[str]] = None,
                  build_timeout: Optional[pulumi.Input[int]] = None,
                  builds_access_level: Optional[pulumi.Input[str]] = None,
                  ci_config_path: Optional[pulumi.Input[str]] = None,
                  ci_default_git_depth: Optional[pulumi.Input[int]] = None,
                  ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+                 ci_separated_caches: Optional[pulumi.Input[bool]] = None,
                  container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
                  container_registry_access_level: Optional[pulumi.Input[str]] = None,
                  container_registry_enabled: Optional[pulumi.Input[bool]] = None,
                  default_branch: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  emails_disabled: Optional[pulumi.Input[bool]] = None,
+                 environments_access_level: Optional[pulumi.Input[str]] = None,
                  external_authorization_classification_label: Optional[pulumi.Input[str]] = None,
+                 feature_flags_access_level: Optional[pulumi.Input[str]] = None,
+                 forked_from_project_id: Optional[pulumi.Input[int]] = None,
                  forking_access_level: Optional[pulumi.Input[str]] = None,
                  group_with_project_templates_id: Optional[pulumi.Input[int]] = None,
                  import_url: Optional[pulumi.Input[str]] = None,
+                 import_url_password: Optional[pulumi.Input[str]] = None,
+                 import_url_username: Optional[pulumi.Input[str]] = None,
+                 infrastructure_access_level: Optional[pulumi.Input[str]] = None,
                  initialize_with_readme: Optional[pulumi.Input[bool]] = None,
                  issues_access_level: Optional[pulumi.Input[str]] = None,
                  issues_enabled: Optional[pulumi.Input[bool]] = None,
                  issues_template: Optional[pulumi.Input[str]] = None,
+                 keep_latest_artifact: Optional[pulumi.Input[bool]] = None,
                  lfs_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_commit_template: Optional[pulumi.Input[str]] = None,
                  merge_method: Optional[pulumi.Input[str]] = None,
                  merge_pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_access_level: Optional[pulumi.Input[str]] = None,
                  merge_requests_enabled: Optional[pulumi.Input[bool]] = None,
                  merge_requests_template: Optional[pulumi.Input[str]] = None,
                  merge_trains_enabled: Optional[pulumi.Input[bool]] = None,
                  mirror: Optional[pulumi.Input[bool]] = None,
                  mirror_overwrites_diverged_branches: Optional[pulumi.Input[bool]] = None,
                  mirror_trigger_builds: Optional[pulumi.Input[bool]] = None,
+                 monitor_access_level: Optional[pulumi.Input[str]] = None,
+                 mr_default_target_self: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  namespace_id: Optional[pulumi.Input[int]] = None,
                  only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
                  only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
                  only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
                  operations_access_level: Optional[pulumi.Input[str]] = None,
                  packages_enabled: Optional[pulumi.Input[bool]] = None,
                  pages_access_level: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  pipelines_enabled: Optional[pulumi.Input[bool]] = None,
                  printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
                  public_builds: Optional[pulumi.Input[bool]] = None,
                  push_rules: Optional[pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']]] = None,
+                 releases_access_level: Optional[pulumi.Input[str]] = None,
                  remove_source_branch_after_merge: Optional[pulumi.Input[bool]] = None,
                  repository_access_level: Optional[pulumi.Input[str]] = None,
                  repository_storage: Optional[pulumi.Input[str]] = None,
                  request_access_enabled: Optional[pulumi.Input[bool]] = None,
                  requirements_access_level: Optional[pulumi.Input[str]] = None,
                  resolve_outdated_diff_discussions: Optional[pulumi.Input[bool]] = None,
+                 restrict_user_defined_variables: Optional[pulumi.Input[bool]] = None,
                  security_and_compliance_access_level: Optional[pulumi.Input[str]] = None,
                  shared_runners_enabled: Optional[pulumi.Input[bool]] = None,
                  skip_wait_for_default_branch_protection: Optional[pulumi.Input[bool]] = None,
                  snippets_access_level: Optional[pulumi.Input[str]] = None,
                  snippets_enabled: Optional[pulumi.Input[bool]] = None,
                  squash_commit_template: Optional[pulumi.Input[str]] = None,
                  squash_option: Optional[pulumi.Input[str]] = None,
+                 suggestion_commit_message: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  template_name: Optional[pulumi.Input[str]] = None,
                  template_project_id: Optional[pulumi.Input[int]] = None,
                  topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  use_custom_template: Optional[pulumi.Input[bool]] = None,
                  visibility_level: Optional[pulumi.Input[str]] = None,
                  wiki_access_level: Optional[pulumi.Input[str]] = None,
@@ -2884,89 +3548,111 @@
             __props__.__dict__["approvals_before_merge"] = approvals_before_merge
             __props__.__dict__["archive_on_destroy"] = archive_on_destroy
             __props__.__dict__["archived"] = archived
             __props__.__dict__["auto_cancel_pending_pipelines"] = auto_cancel_pending_pipelines
             __props__.__dict__["auto_devops_deploy_strategy"] = auto_devops_deploy_strategy
             __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
             __props__.__dict__["autoclose_referenced_issues"] = autoclose_referenced_issues
+            __props__.__dict__["avatar"] = avatar
+            __props__.__dict__["avatar_hash"] = avatar_hash
             if build_coverage_regex is not None and not opts.urn:
                 warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
                 pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
             __props__.__dict__["build_coverage_regex"] = build_coverage_regex
             __props__.__dict__["build_git_strategy"] = build_git_strategy
             __props__.__dict__["build_timeout"] = build_timeout
             __props__.__dict__["builds_access_level"] = builds_access_level
             __props__.__dict__["ci_config_path"] = ci_config_path
             __props__.__dict__["ci_default_git_depth"] = ci_default_git_depth
             __props__.__dict__["ci_forward_deployment_enabled"] = ci_forward_deployment_enabled
+            __props__.__dict__["ci_separated_caches"] = ci_separated_caches
             __props__.__dict__["container_expiration_policy"] = container_expiration_policy
             __props__.__dict__["container_registry_access_level"] = container_registry_access_level
+            if container_registry_enabled is not None and not opts.urn:
+                warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+                pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
             __props__.__dict__["container_registry_enabled"] = container_registry_enabled
             __props__.__dict__["default_branch"] = default_branch
             __props__.__dict__["description"] = description
             __props__.__dict__["emails_disabled"] = emails_disabled
+            __props__.__dict__["environments_access_level"] = environments_access_level
             __props__.__dict__["external_authorization_classification_label"] = external_authorization_classification_label
+            __props__.__dict__["feature_flags_access_level"] = feature_flags_access_level
+            __props__.__dict__["forked_from_project_id"] = forked_from_project_id
             __props__.__dict__["forking_access_level"] = forking_access_level
             __props__.__dict__["group_with_project_templates_id"] = group_with_project_templates_id
             __props__.__dict__["import_url"] = import_url
+            __props__.__dict__["import_url_password"] = None if import_url_password is None else pulumi.Output.secret(import_url_password)
+            __props__.__dict__["import_url_username"] = import_url_username
+            __props__.__dict__["infrastructure_access_level"] = infrastructure_access_level
             __props__.__dict__["initialize_with_readme"] = initialize_with_readme
             __props__.__dict__["issues_access_level"] = issues_access_level
             __props__.__dict__["issues_enabled"] = issues_enabled
             __props__.__dict__["issues_template"] = issues_template
+            __props__.__dict__["keep_latest_artifact"] = keep_latest_artifact
             __props__.__dict__["lfs_enabled"] = lfs_enabled
             __props__.__dict__["merge_commit_template"] = merge_commit_template
             __props__.__dict__["merge_method"] = merge_method
             __props__.__dict__["merge_pipelines_enabled"] = merge_pipelines_enabled
             __props__.__dict__["merge_requests_access_level"] = merge_requests_access_level
             __props__.__dict__["merge_requests_enabled"] = merge_requests_enabled
             __props__.__dict__["merge_requests_template"] = merge_requests_template
             __props__.__dict__["merge_trains_enabled"] = merge_trains_enabled
             __props__.__dict__["mirror"] = mirror
             __props__.__dict__["mirror_overwrites_diverged_branches"] = mirror_overwrites_diverged_branches
             __props__.__dict__["mirror_trigger_builds"] = mirror_trigger_builds
+            __props__.__dict__["monitor_access_level"] = monitor_access_level
+            __props__.__dict__["mr_default_target_self"] = mr_default_target_self
             __props__.__dict__["name"] = name
             __props__.__dict__["namespace_id"] = namespace_id
             __props__.__dict__["only_allow_merge_if_all_discussions_are_resolved"] = only_allow_merge_if_all_discussions_are_resolved
             __props__.__dict__["only_allow_merge_if_pipeline_succeeds"] = only_allow_merge_if_pipeline_succeeds
             __props__.__dict__["only_mirror_protected_branches"] = only_mirror_protected_branches
             __props__.__dict__["operations_access_level"] = operations_access_level
             __props__.__dict__["packages_enabled"] = packages_enabled
             __props__.__dict__["pages_access_level"] = pages_access_level
             __props__.__dict__["path"] = path
+            if pipelines_enabled is not None and not opts.urn:
+                warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+                pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
             __props__.__dict__["pipelines_enabled"] = pipelines_enabled
             __props__.__dict__["printing_merge_request_link_enabled"] = printing_merge_request_link_enabled
             __props__.__dict__["public_builds"] = public_builds
             __props__.__dict__["push_rules"] = push_rules
+            __props__.__dict__["releases_access_level"] = releases_access_level
             __props__.__dict__["remove_source_branch_after_merge"] = remove_source_branch_after_merge
             __props__.__dict__["repository_access_level"] = repository_access_level
             __props__.__dict__["repository_storage"] = repository_storage
             __props__.__dict__["request_access_enabled"] = request_access_enabled
             __props__.__dict__["requirements_access_level"] = requirements_access_level
             __props__.__dict__["resolve_outdated_diff_discussions"] = resolve_outdated_diff_discussions
+            __props__.__dict__["restrict_user_defined_variables"] = restrict_user_defined_variables
             __props__.__dict__["security_and_compliance_access_level"] = security_and_compliance_access_level
             __props__.__dict__["shared_runners_enabled"] = shared_runners_enabled
             __props__.__dict__["skip_wait_for_default_branch_protection"] = skip_wait_for_default_branch_protection
             __props__.__dict__["snippets_access_level"] = snippets_access_level
             __props__.__dict__["snippets_enabled"] = snippets_enabled
             __props__.__dict__["squash_commit_template"] = squash_commit_template
             __props__.__dict__["squash_option"] = squash_option
+            __props__.__dict__["suggestion_commit_message"] = suggestion_commit_message
             __props__.__dict__["tags"] = tags
             __props__.__dict__["template_name"] = template_name
             __props__.__dict__["template_project_id"] = template_project_id
             __props__.__dict__["topics"] = topics
             __props__.__dict__["use_custom_template"] = use_custom_template
             __props__.__dict__["visibility_level"] = visibility_level
             __props__.__dict__["wiki_access_level"] = wiki_access_level
             __props__.__dict__["wiki_enabled"] = wiki_enabled
+            __props__.__dict__["avatar_url"] = None
             __props__.__dict__["http_url_to_repo"] = None
             __props__.__dict__["path_with_namespace"] = None
             __props__.__dict__["runners_token"] = None
             __props__.__dict__["ssh_url_to_repo"] = None
             __props__.__dict__["web_url"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["runnersToken"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["importUrlPassword", "runnersToken"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Project, __self__).__init__(
             'gitlab:index/project:Project',
             resource_name,
             __props__,
             opts)
 
@@ -2979,76 +3665,92 @@
             approvals_before_merge: Optional[pulumi.Input[int]] = None,
             archive_on_destroy: Optional[pulumi.Input[bool]] = None,
             archived: Optional[pulumi.Input[bool]] = None,
             auto_cancel_pending_pipelines: Optional[pulumi.Input[str]] = None,
             auto_devops_deploy_strategy: Optional[pulumi.Input[str]] = None,
             auto_devops_enabled: Optional[pulumi.Input[bool]] = None,
             autoclose_referenced_issues: Optional[pulumi.Input[bool]] = None,
+            avatar: Optional[pulumi.Input[str]] = None,
+            avatar_hash: Optional[pulumi.Input[str]] = None,
+            avatar_url: Optional[pulumi.Input[str]] = None,
             build_coverage_regex: Optional[pulumi.Input[str]] = None,
             build_git_strategy: Optional[pulumi.Input[str]] = None,
             build_timeout: Optional[pulumi.Input[int]] = None,
             builds_access_level: Optional[pulumi.Input[str]] = None,
             ci_config_path: Optional[pulumi.Input[str]] = None,
             ci_default_git_depth: Optional[pulumi.Input[int]] = None,
             ci_forward_deployment_enabled: Optional[pulumi.Input[bool]] = None,
+            ci_separated_caches: Optional[pulumi.Input[bool]] = None,
             container_expiration_policy: Optional[pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']]] = None,
             container_registry_access_level: Optional[pulumi.Input[str]] = None,
             container_registry_enabled: Optional[pulumi.Input[bool]] = None,
             default_branch: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             emails_disabled: Optional[pulumi.Input[bool]] = None,
+            environments_access_level: Optional[pulumi.Input[str]] = None,
             external_authorization_classification_label: Optional[pulumi.Input[str]] = None,
+            feature_flags_access_level: Optional[pulumi.Input[str]] = None,
+            forked_from_project_id: Optional[pulumi.Input[int]] = None,
             forking_access_level: Optional[pulumi.Input[str]] = None,
             group_with_project_templates_id: Optional[pulumi.Input[int]] = None,
             http_url_to_repo: Optional[pulumi.Input[str]] = None,
             import_url: Optional[pulumi.Input[str]] = None,
+            import_url_password: Optional[pulumi.Input[str]] = None,
+            import_url_username: Optional[pulumi.Input[str]] = None,
+            infrastructure_access_level: Optional[pulumi.Input[str]] = None,
             initialize_with_readme: Optional[pulumi.Input[bool]] = None,
             issues_access_level: Optional[pulumi.Input[str]] = None,
             issues_enabled: Optional[pulumi.Input[bool]] = None,
             issues_template: Optional[pulumi.Input[str]] = None,
+            keep_latest_artifact: Optional[pulumi.Input[bool]] = None,
             lfs_enabled: Optional[pulumi.Input[bool]] = None,
             merge_commit_template: Optional[pulumi.Input[str]] = None,
             merge_method: Optional[pulumi.Input[str]] = None,
             merge_pipelines_enabled: Optional[pulumi.Input[bool]] = None,
             merge_requests_access_level: Optional[pulumi.Input[str]] = None,
             merge_requests_enabled: Optional[pulumi.Input[bool]] = None,
             merge_requests_template: Optional[pulumi.Input[str]] = None,
             merge_trains_enabled: Optional[pulumi.Input[bool]] = None,
             mirror: Optional[pulumi.Input[bool]] = None,
             mirror_overwrites_diverged_branches: Optional[pulumi.Input[bool]] = None,
             mirror_trigger_builds: Optional[pulumi.Input[bool]] = None,
+            monitor_access_level: Optional[pulumi.Input[str]] = None,
+            mr_default_target_self: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             namespace_id: Optional[pulumi.Input[int]] = None,
             only_allow_merge_if_all_discussions_are_resolved: Optional[pulumi.Input[bool]] = None,
             only_allow_merge_if_pipeline_succeeds: Optional[pulumi.Input[bool]] = None,
             only_mirror_protected_branches: Optional[pulumi.Input[bool]] = None,
             operations_access_level: Optional[pulumi.Input[str]] = None,
             packages_enabled: Optional[pulumi.Input[bool]] = None,
             pages_access_level: Optional[pulumi.Input[str]] = None,
             path: Optional[pulumi.Input[str]] = None,
             path_with_namespace: Optional[pulumi.Input[str]] = None,
             pipelines_enabled: Optional[pulumi.Input[bool]] = None,
             printing_merge_request_link_enabled: Optional[pulumi.Input[bool]] = None,
             public_builds: Optional[pulumi.Input[bool]] = None,
             push_rules: Optional[pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']]] = None,
+            releases_access_level: Optional[pulumi.Input[str]] = None,
             remove_source_branch_after_merge: Optional[pulumi.Input[bool]] = None,
             repository_access_level: Optional[pulumi.Input[str]] = None,
             repository_storage: Optional[pulumi.Input[str]] = None,
             request_access_enabled: Optional[pulumi.Input[bool]] = None,
             requirements_access_level: Optional[pulumi.Input[str]] = None,
             resolve_outdated_diff_discussions: Optional[pulumi.Input[bool]] = None,
+            restrict_user_defined_variables: Optional[pulumi.Input[bool]] = None,
             runners_token: Optional[pulumi.Input[str]] = None,
             security_and_compliance_access_level: Optional[pulumi.Input[str]] = None,
             shared_runners_enabled: Optional[pulumi.Input[bool]] = None,
             skip_wait_for_default_branch_protection: Optional[pulumi.Input[bool]] = None,
             snippets_access_level: Optional[pulumi.Input[str]] = None,
             snippets_enabled: Optional[pulumi.Input[bool]] = None,
             squash_commit_template: Optional[pulumi.Input[str]] = None,
             squash_option: Optional[pulumi.Input[str]] = None,
             ssh_url_to_repo: Optional[pulumi.Input[str]] = None,
+            suggestion_commit_message: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             template_name: Optional[pulumi.Input[str]] = None,
             template_project_id: Optional[pulumi.Input[int]] = None,
             topics: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             use_custom_template: Optional[pulumi.Input[bool]] = None,
             visibility_level: Optional[pulumi.Input[str]] = None,
             web_url: Optional[pulumi.Input[str]] = None,
@@ -3069,84 +3771,109 @@
                In the meantime we recommend against using this attribute and use `ProjectApprovalRule` instead.
         :param pulumi.Input[bool] archive_on_destroy: Set to `true` to archive the project instead of deleting on destroy. If set to `true` it will entire omit the `DELETE` operation.
         :param pulumi.Input[bool] archived: Whether the project is in read-only mode (archived). Repositories can be archived/unarchived by toggling this parameter.
         :param pulumi.Input[str] auto_cancel_pending_pipelines: Auto-cancel pending pipelines. This isn’t a boolean, but enabled/disabled.
         :param pulumi.Input[str] auto_devops_deploy_strategy: Auto Deploy strategy. Valid values are `continuous`, `manual`, `timed_incremental`.
         :param pulumi.Input[bool] auto_devops_enabled: Enable Auto DevOps for this project.
         :param pulumi.Input[bool] autoclose_referenced_issues: Set whether auto-closing referenced issues on default branch.
+        :param pulumi.Input[str] avatar: A local path to the avatar image to upload. **Note**: not available for imported resources.
+        :param pulumi.Input[str] avatar_hash: The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
+        :param pulumi.Input[str] avatar_url: The URL of the avatar image.
         :param pulumi.Input[str] build_coverage_regex: Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         :param pulumi.Input[str] build_git_strategy: The Git strategy. Defaults to fetch.
         :param pulumi.Input[int] build_timeout: The maximum amount of time, in seconds, that a job can run.
         :param pulumi.Input[str] builds_access_level: Set the builds access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] ci_config_path: Custom Path to CI config file.
         :param pulumi.Input[int] ci_default_git_depth: Default number of revisions for shallow cloning.
         :param pulumi.Input[bool] ci_forward_deployment_enabled: When a new deployment job starts, skip older deployment jobs that are still pending.
+        :param pulumi.Input[bool] ci_separated_caches: Use separate caches for protected branches.
         :param pulumi.Input[pulumi.InputType['ProjectContainerExpirationPolicyArgs']] container_expiration_policy: Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         :param pulumi.Input[str] container_registry_access_level: Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] container_registry_enabled: Enable container registry for the project.
         :param pulumi.Input[str] default_branch: The default branch for the project.
         :param pulumi.Input[str] description: A description of the project.
         :param pulumi.Input[bool] emails_disabled: Disable email notifications.
+        :param pulumi.Input[str] environments_access_level: Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] external_authorization_classification_label: The classification label for the project.
+        :param pulumi.Input[str] feature_flags_access_level: Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[int] forked_from_project_id: The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
         :param pulumi.Input[str] forking_access_level: Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[int] group_with_project_templates_id: For group-level custom templates, specifies ID of group from which all the custom project templates are sourced. Leave empty for instance-level templates. Requires use*custom*template to be true (enterprise edition).
         :param pulumi.Input[str] http_url_to_repo: URL that can be provided to `git clone` to clone the
-        :param pulumi.Input[str] import_url: Git URL to a repository to be imported.
+        :param pulumi.Input[str] import_url: Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+               together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+               Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+               credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+               `terraform import`. See the examples section for how to properly use it.
+        :param pulumi.Input[str] import_url_password: The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] import_url_username: The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+               to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+               use it.
+        :param pulumi.Input[str] infrastructure_access_level: Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] initialize_with_readme: Create main branch with first commit containing a README.md file.
         :param pulumi.Input[str] issues_access_level: Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] issues_enabled: Enable issue tracking for the project.
         :param pulumi.Input[str] issues_template: Sets the template for new issues in the project.
+        :param pulumi.Input[bool] keep_latest_artifact: Disable or enable the ability to keep the latest artifact for this project.
         :param pulumi.Input[bool] lfs_enabled: Enable LFS for the project.
         :param pulumi.Input[str] merge_commit_template: Template used to create merge commit message in merge requests. (Introduced in GitLab 14.5.)
-        :param pulumi.Input[str] merge_method: Set to `ff` to create fast-forward merges
+        :param pulumi.Input[str] merge_method: Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         :param pulumi.Input[bool] merge_pipelines_enabled: Enable or disable merge pipelines.
         :param pulumi.Input[str] merge_requests_access_level: Set the merge requests access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] merge_requests_enabled: Enable merge requests for the project.
         :param pulumi.Input[str] merge_requests_template: Sets the template for new merge requests in the project.
         :param pulumi.Input[bool] merge_trains_enabled: Enable or disable merge trains. Requires `merge_pipelines_enabled` to be set to `true` to take effect.
         :param pulumi.Input[bool] mirror: Enable project pull mirror.
         :param pulumi.Input[bool] mirror_overwrites_diverged_branches: Enable overwrite diverged branches for a mirrored project.
         :param pulumi.Input[bool] mirror_trigger_builds: Enable trigger builds on pushes for a mirrored project.
+        :param pulumi.Input[str] monitor_access_level: Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        :param pulumi.Input[bool] mr_default_target_self: For forked projects, target merge requests to this project. If false, the target will be the upstream project.
         :param pulumi.Input[str] name: The name of the project.
         :param pulumi.Input[int] namespace_id: The namespace (group or user) of the project. Defaults to your user.
         :param pulumi.Input[bool] only_allow_merge_if_all_discussions_are_resolved: Set to true if you want allow merges only if all discussions are resolved.
         :param pulumi.Input[bool] only_allow_merge_if_pipeline_succeeds: Set to true if you want allow merges only if a pipeline succeeds.
         :param pulumi.Input[bool] only_mirror_protected_branches: Enable only mirror protected branches for a mirrored project.
         :param pulumi.Input[str] operations_access_level: Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] packages_enabled: Enable packages repository for the project.
         :param pulumi.Input[str] pages_access_level: Enable pages access control
         :param pulumi.Input[str] path: The path of the repository.
         :param pulumi.Input[str] path_with_namespace: The path of the repository with namespace.
-        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project.
+        :param pulumi.Input[bool] pipelines_enabled: Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         :param pulumi.Input[bool] printing_merge_request_link_enabled: Show link to create/view merge request when pushing from the command line
         :param pulumi.Input[bool] public_builds: If true, jobs can be viewed by non-project members.
         :param pulumi.Input[pulumi.InputType['ProjectPushRulesArgs']] push_rules: Push rules for the project.
+        :param pulumi.Input[str] releases_access_level: Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] remove_source_branch_after_merge: Enable `Delete source branch` option by default for all new merge requests.
         :param pulumi.Input[str] repository_access_level: Set the repository access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[str] repository_storage: Which storage shard the repository is on. (administrator only)
         :param pulumi.Input[bool] request_access_enabled: Allow users to request member access.
         :param pulumi.Input[str] requirements_access_level: Set the requirements access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] resolve_outdated_diff_discussions: Automatically resolve merge request diffs discussions on lines changed with a push.
+        :param pulumi.Input[bool] restrict_user_defined_variables: Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
         :param pulumi.Input[str] runners_token: Registration token to use during runner setup.
         :param pulumi.Input[str] security_and_compliance_access_level: Set the security and compliance access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] shared_runners_enabled: Enable shared runners for this project.
         :param pulumi.Input[bool] skip_wait_for_default_branch_protection: If `true`, the default behavior to wait for the default branch protection to be created is skipped.
                This is necessary if the current user is not an admin and the default branch protection is disabled on an instance-level.
                There is currently no known way to determine if the default branch protection is disabled on an instance-level for non-admin users.
                This attribute is only used during resource creation, thus changes are suppressed and the attribute cannot be imported.
         :param pulumi.Input[str] snippets_access_level: Set the snippets access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] snippets_enabled: Enable snippets for the project.
         :param pulumi.Input[str] squash_commit_template: Template used to create squash commit message in merge requests. (Introduced in GitLab 14.6.)
         :param pulumi.Input[str] squash_option: Squash commits when merge request. Valid values are `never`, `always`, `default_on`, or `default_off`. The default value is `default_off`. [GitLab >= 14.1]
         :param pulumi.Input[str] ssh_url_to_repo: URL that can be provided to `git clone` to clone the
+        :param pulumi.Input[str] suggestion_commit_message: The commit message used to apply merge request suggestions.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         :param pulumi.Input[str] template_name: When used without use*custom*template, name of a built-in project template. When used with use*custom*template, name of a custom project template. This option is mutually exclusive with `template_project_id`.
         :param pulumi.Input[int] template_project_id: When used with use*custom*template, project ID of a custom project template. This is preferable to using template*name since template*name may be ambiguous (enterprise edition). This option is mutually exclusive with `template_name`. See `GroupProjectFileTemplate` to set a project as a template project. If a project has not been set as a template, using it here will result in an error.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] topics: The list of topics for the project.
         :param pulumi.Input[bool] use_custom_template: Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+               	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         :param pulumi.Input[str] visibility_level: Set to `public` to create a public project.
         :param pulumi.Input[str] web_url: URL that can be used to find the project in a browser.
         :param pulumi.Input[str] wiki_access_level: Set the wiki access level. Valid values are `disabled`, `private`, `enabled`.
         :param pulumi.Input[bool] wiki_enabled: Enable wiki for the project.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -3157,90 +3884,106 @@
         __props__.__dict__["approvals_before_merge"] = approvals_before_merge
         __props__.__dict__["archive_on_destroy"] = archive_on_destroy
         __props__.__dict__["archived"] = archived
         __props__.__dict__["auto_cancel_pending_pipelines"] = auto_cancel_pending_pipelines
         __props__.__dict__["auto_devops_deploy_strategy"] = auto_devops_deploy_strategy
         __props__.__dict__["auto_devops_enabled"] = auto_devops_enabled
         __props__.__dict__["autoclose_referenced_issues"] = autoclose_referenced_issues
+        __props__.__dict__["avatar"] = avatar
+        __props__.__dict__["avatar_hash"] = avatar_hash
+        __props__.__dict__["avatar_url"] = avatar_url
         __props__.__dict__["build_coverage_regex"] = build_coverage_regex
         __props__.__dict__["build_git_strategy"] = build_git_strategy
         __props__.__dict__["build_timeout"] = build_timeout
         __props__.__dict__["builds_access_level"] = builds_access_level
         __props__.__dict__["ci_config_path"] = ci_config_path
         __props__.__dict__["ci_default_git_depth"] = ci_default_git_depth
         __props__.__dict__["ci_forward_deployment_enabled"] = ci_forward_deployment_enabled
+        __props__.__dict__["ci_separated_caches"] = ci_separated_caches
         __props__.__dict__["container_expiration_policy"] = container_expiration_policy
         __props__.__dict__["container_registry_access_level"] = container_registry_access_level
         __props__.__dict__["container_registry_enabled"] = container_registry_enabled
         __props__.__dict__["default_branch"] = default_branch
         __props__.__dict__["description"] = description
         __props__.__dict__["emails_disabled"] = emails_disabled
+        __props__.__dict__["environments_access_level"] = environments_access_level
         __props__.__dict__["external_authorization_classification_label"] = external_authorization_classification_label
+        __props__.__dict__["feature_flags_access_level"] = feature_flags_access_level
+        __props__.__dict__["forked_from_project_id"] = forked_from_project_id
         __props__.__dict__["forking_access_level"] = forking_access_level
         __props__.__dict__["group_with_project_templates_id"] = group_with_project_templates_id
         __props__.__dict__["http_url_to_repo"] = http_url_to_repo
         __props__.__dict__["import_url"] = import_url
+        __props__.__dict__["import_url_password"] = import_url_password
+        __props__.__dict__["import_url_username"] = import_url_username
+        __props__.__dict__["infrastructure_access_level"] = infrastructure_access_level
         __props__.__dict__["initialize_with_readme"] = initialize_with_readme
         __props__.__dict__["issues_access_level"] = issues_access_level
         __props__.__dict__["issues_enabled"] = issues_enabled
         __props__.__dict__["issues_template"] = issues_template
+        __props__.__dict__["keep_latest_artifact"] = keep_latest_artifact
         __props__.__dict__["lfs_enabled"] = lfs_enabled
         __props__.__dict__["merge_commit_template"] = merge_commit_template
         __props__.__dict__["merge_method"] = merge_method
         __props__.__dict__["merge_pipelines_enabled"] = merge_pipelines_enabled
         __props__.__dict__["merge_requests_access_level"] = merge_requests_access_level
         __props__.__dict__["merge_requests_enabled"] = merge_requests_enabled
         __props__.__dict__["merge_requests_template"] = merge_requests_template
         __props__.__dict__["merge_trains_enabled"] = merge_trains_enabled
         __props__.__dict__["mirror"] = mirror
         __props__.__dict__["mirror_overwrites_diverged_branches"] = mirror_overwrites_diverged_branches
         __props__.__dict__["mirror_trigger_builds"] = mirror_trigger_builds
+        __props__.__dict__["monitor_access_level"] = monitor_access_level
+        __props__.__dict__["mr_default_target_self"] = mr_default_target_self
         __props__.__dict__["name"] = name
         __props__.__dict__["namespace_id"] = namespace_id
         __props__.__dict__["only_allow_merge_if_all_discussions_are_resolved"] = only_allow_merge_if_all_discussions_are_resolved
         __props__.__dict__["only_allow_merge_if_pipeline_succeeds"] = only_allow_merge_if_pipeline_succeeds
         __props__.__dict__["only_mirror_protected_branches"] = only_mirror_protected_branches
         __props__.__dict__["operations_access_level"] = operations_access_level
         __props__.__dict__["packages_enabled"] = packages_enabled
         __props__.__dict__["pages_access_level"] = pages_access_level
         __props__.__dict__["path"] = path
         __props__.__dict__["path_with_namespace"] = path_with_namespace
         __props__.__dict__["pipelines_enabled"] = pipelines_enabled
         __props__.__dict__["printing_merge_request_link_enabled"] = printing_merge_request_link_enabled
         __props__.__dict__["public_builds"] = public_builds
         __props__.__dict__["push_rules"] = push_rules
+        __props__.__dict__["releases_access_level"] = releases_access_level
         __props__.__dict__["remove_source_branch_after_merge"] = remove_source_branch_after_merge
         __props__.__dict__["repository_access_level"] = repository_access_level
         __props__.__dict__["repository_storage"] = repository_storage
         __props__.__dict__["request_access_enabled"] = request_access_enabled
         __props__.__dict__["requirements_access_level"] = requirements_access_level
         __props__.__dict__["resolve_outdated_diff_discussions"] = resolve_outdated_diff_discussions
+        __props__.__dict__["restrict_user_defined_variables"] = restrict_user_defined_variables
         __props__.__dict__["runners_token"] = runners_token
         __props__.__dict__["security_and_compliance_access_level"] = security_and_compliance_access_level
         __props__.__dict__["shared_runners_enabled"] = shared_runners_enabled
         __props__.__dict__["skip_wait_for_default_branch_protection"] = skip_wait_for_default_branch_protection
         __props__.__dict__["snippets_access_level"] = snippets_access_level
         __props__.__dict__["snippets_enabled"] = snippets_enabled
         __props__.__dict__["squash_commit_template"] = squash_commit_template
         __props__.__dict__["squash_option"] = squash_option
         __props__.__dict__["ssh_url_to_repo"] = ssh_url_to_repo
+        __props__.__dict__["suggestion_commit_message"] = suggestion_commit_message
         __props__.__dict__["tags"] = tags
         __props__.__dict__["template_name"] = template_name
         __props__.__dict__["template_project_id"] = template_project_id
         __props__.__dict__["topics"] = topics
         __props__.__dict__["use_custom_template"] = use_custom_template
         __props__.__dict__["visibility_level"] = visibility_level
         __props__.__dict__["web_url"] = web_url
         __props__.__dict__["wiki_access_level"] = wiki_access_level
         __props__.__dict__["wiki_enabled"] = wiki_enabled
         return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="allowMergeOnSkippedPipeline")
-    def allow_merge_on_skipped_pipeline(self) -> pulumi.Output[Optional[bool]]:
+    def allow_merge_on_skipped_pipeline(self) -> pulumi.Output[bool]:
         """
         Set to true if you want to treat skipped pipelines as if they finished with success.
         """
         return pulumi.get(self, "allow_merge_on_skipped_pipeline")
 
     @property
     @pulumi.getter(name="analyticsAccessLevel")
@@ -3306,14 +4049,38 @@
     def autoclose_referenced_issues(self) -> pulumi.Output[bool]:
         """
         Set whether auto-closing referenced issues on default branch.
         """
         return pulumi.get(self, "autoclose_referenced_issues")
 
     @property
+    @pulumi.getter
+    def avatar(self) -> pulumi.Output[Optional[str]]:
+        """
+        A local path to the avatar image to upload. **Note**: not available for imported resources.
+        """
+        return pulumi.get(self, "avatar")
+
+    @property
+    @pulumi.getter(name="avatarHash")
+    def avatar_hash(self) -> pulumi.Output[str]:
+        """
+        The hash of the avatar image. Use `filesha256("path/to/avatar.png")` whenever possible. **Note**: this is used to trigger an update of the avatar. If it's not given, but an avatar is given, the avatar will be updated each time.
+        """
+        return pulumi.get(self, "avatar_hash")
+
+    @property
+    @pulumi.getter(name="avatarUrl")
+    def avatar_url(self) -> pulumi.Output[str]:
+        """
+        The URL of the avatar image.
+        """
+        return pulumi.get(self, "avatar_url")
+
+    @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> pulumi.Output[Optional[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
         return pulumi.get(self, "build_coverage_regex")
 
@@ -3355,21 +4122,29 @@
         """
         Default number of revisions for shallow cloning.
         """
         return pulumi.get(self, "ci_default_git_depth")
 
     @property
     @pulumi.getter(name="ciForwardDeploymentEnabled")
-    def ci_forward_deployment_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def ci_forward_deployment_enabled(self) -> pulumi.Output[bool]:
         """
         When a new deployment job starts, skip older deployment jobs that are still pending.
         """
         return pulumi.get(self, "ci_forward_deployment_enabled")
 
     @property
+    @pulumi.getter(name="ciSeparatedCaches")
+    def ci_separated_caches(self) -> pulumi.Output[bool]:
+        """
+        Use separate caches for protected branches.
+        """
+        return pulumi.get(self, "ci_separated_caches")
+
+    @property
     @pulumi.getter(name="containerExpirationPolicy")
     def container_expiration_policy(self) -> pulumi.Output['outputs.ProjectContainerExpirationPolicy']:
         """
         Set the image cleanup policy for this project. **Note**: this field is sometimes named `container_expiration_policy_attributes` in the GitLab Upstream API.
         """
         return pulumi.get(self, "container_expiration_policy")
 
@@ -3379,15 +4154,15 @@
         """
         Set visibility of container registry, for this project. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "container_registry_access_level")
 
     @property
     @pulumi.getter(name="containerRegistryEnabled")
-    def container_registry_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def container_registry_enabled(self) -> pulumi.Output[bool]:
         """
         Enable container registry for the project.
         """
         return pulumi.get(self, "container_registry_enabled")
 
     @property
     @pulumi.getter(name="defaultBranch")
@@ -3410,22 +4185,46 @@
     def emails_disabled(self) -> pulumi.Output[Optional[bool]]:
         """
         Disable email notifications.
         """
         return pulumi.get(self, "emails_disabled")
 
     @property
+    @pulumi.getter(name="environmentsAccessLevel")
+    def environments_access_level(self) -> pulumi.Output[str]:
+        """
+        Set the environments access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "environments_access_level")
+
+    @property
     @pulumi.getter(name="externalAuthorizationClassificationLabel")
     def external_authorization_classification_label(self) -> pulumi.Output[Optional[str]]:
         """
         The classification label for the project.
         """
         return pulumi.get(self, "external_authorization_classification_label")
 
     @property
+    @pulumi.getter(name="featureFlagsAccessLevel")
+    def feature_flags_access_level(self) -> pulumi.Output[str]:
+        """
+        Set the feature flags access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "feature_flags_access_level")
+
+    @property
+    @pulumi.getter(name="forkedFromProjectId")
+    def forked_from_project_id(self) -> pulumi.Output[Optional[int]]:
+        """
+        The id of the project to fork. During create the project is forked and during an update the fork relation is changed.
+        """
+        return pulumi.get(self, "forked_from_project_id")
+
+    @property
     @pulumi.getter(name="forkingAccessLevel")
     def forking_access_level(self) -> pulumi.Output[str]:
         """
         Set the forking access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "forking_access_level")
 
@@ -3445,19 +4244,51 @@
         """
         return pulumi.get(self, "http_url_to_repo")
 
     @property
     @pulumi.getter(name="importUrl")
     def import_url(self) -> pulumi.Output[Optional[str]]:
         """
-        Git URL to a repository to be imported.
+        Git URL to a repository to be imported. Together with `mirror = true` it will setup a Pull Mirror. This can also be used
+        together with `forked_from_project_id` to setup a Pull Mirror for a fork. The fork takes precedence over the import.
+        Make sure to provide the credentials in `import_url_username` and `import_url_password`. GitLab never returns the
+        credentials, thus the provider cannot detect configuration drift in the credentials. They can also not be imported using
+        `terraform import`. See the examples section for how to properly use it.
         """
         return pulumi.get(self, "import_url")
 
     @property
+    @pulumi.getter(name="importUrlPassword")
+    def import_url_password(self) -> pulumi.Output[Optional[str]]:
+        """
+        The password for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_password")
+
+    @property
+    @pulumi.getter(name="importUrlUsername")
+    def import_url_username(self) -> pulumi.Output[Optional[str]]:
+        """
+        The username for the `import_url`. The value of this field is used to construct a valid `import_url` and is only related
+        to the provider. This field cannot be imported using `terraform import`. See the examples section for how to properly
+        use it.
+        """
+        return pulumi.get(self, "import_url_username")
+
+    @property
+    @pulumi.getter(name="infrastructureAccessLevel")
+    def infrastructure_access_level(self) -> pulumi.Output[str]:
+        """
+        Set the infrastructure access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "infrastructure_access_level")
+
+    @property
     @pulumi.getter(name="initializeWithReadme")
     def initialize_with_readme(self) -> pulumi.Output[Optional[bool]]:
         """
         Create main branch with first commit containing a README.md file.
         """
         return pulumi.get(self, "initialize_with_readme")
 
@@ -3467,31 +4298,39 @@
         """
         Set the issues access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "issues_access_level")
 
     @property
     @pulumi.getter(name="issuesEnabled")
-    def issues_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def issues_enabled(self) -> pulumi.Output[bool]:
         """
         Enable issue tracking for the project.
         """
         return pulumi.get(self, "issues_enabled")
 
     @property
     @pulumi.getter(name="issuesTemplate")
     def issues_template(self) -> pulumi.Output[Optional[str]]:
         """
         Sets the template for new issues in the project.
         """
         return pulumi.get(self, "issues_template")
 
     @property
+    @pulumi.getter(name="keepLatestArtifact")
+    def keep_latest_artifact(self) -> pulumi.Output[bool]:
+        """
+        Disable or enable the ability to keep the latest artifact for this project.
+        """
+        return pulumi.get(self, "keep_latest_artifact")
+
+    @property
     @pulumi.getter(name="lfsEnabled")
-    def lfs_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def lfs_enabled(self) -> pulumi.Output[bool]:
         """
         Enable LFS for the project.
         """
         return pulumi.get(self, "lfs_enabled")
 
     @property
     @pulumi.getter(name="mergeCommitTemplate")
@@ -3499,23 +4338,23 @@
         """
         Template used to create merge commit message in merge requests. (Introduced in GitLab 14.5.)
         """
         return pulumi.get(self, "merge_commit_template")
 
     @property
     @pulumi.getter(name="mergeMethod")
-    def merge_method(self) -> pulumi.Output[Optional[str]]:
+    def merge_method(self) -> pulumi.Output[str]:
         """
-        Set to `ff` to create fast-forward merges
+        Set the merge method. Valid values are `merge`, `rebase_merge`, `ff`.
         """
         return pulumi.get(self, "merge_method")
 
     @property
     @pulumi.getter(name="mergePipelinesEnabled")
-    def merge_pipelines_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def merge_pipelines_enabled(self) -> pulumi.Output[bool]:
         """
         Enable or disable merge pipelines.
         """
         return pulumi.get(self, "merge_pipelines_enabled")
 
     @property
     @pulumi.getter(name="mergeRequestsAccessLevel")
@@ -3523,15 +4362,15 @@
         """
         Set the merge requests access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "merge_requests_access_level")
 
     @property
     @pulumi.getter(name="mergeRequestsEnabled")
-    def merge_requests_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def merge_requests_enabled(self) -> pulumi.Output[bool]:
         """
         Enable merge requests for the project.
         """
         return pulumi.get(self, "merge_requests_enabled")
 
     @property
     @pulumi.getter(name="mergeRequestsTemplate")
@@ -3539,15 +4378,15 @@
         """
         Sets the template for new merge requests in the project.
         """
         return pulumi.get(self, "merge_requests_template")
 
     @property
     @pulumi.getter(name="mergeTrainsEnabled")
-    def merge_trains_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def merge_trains_enabled(self) -> pulumi.Output[bool]:
         """
         Enable or disable merge trains. Requires `merge_pipelines_enabled` to be set to `true` to take effect.
         """
         return pulumi.get(self, "merge_trains_enabled")
 
     @property
     @pulumi.getter
@@ -3555,29 +4394,45 @@
         """
         Enable project pull mirror.
         """
         return pulumi.get(self, "mirror")
 
     @property
     @pulumi.getter(name="mirrorOverwritesDivergedBranches")
-    def mirror_overwrites_diverged_branches(self) -> pulumi.Output[Optional[bool]]:
+    def mirror_overwrites_diverged_branches(self) -> pulumi.Output[bool]:
         """
         Enable overwrite diverged branches for a mirrored project.
         """
         return pulumi.get(self, "mirror_overwrites_diverged_branches")
 
     @property
     @pulumi.getter(name="mirrorTriggerBuilds")
-    def mirror_trigger_builds(self) -> pulumi.Output[Optional[bool]]:
+    def mirror_trigger_builds(self) -> pulumi.Output[bool]:
         """
         Enable trigger builds on pushes for a mirrored project.
         """
         return pulumi.get(self, "mirror_trigger_builds")
 
     @property
+    @pulumi.getter(name="monitorAccessLevel")
+    def monitor_access_level(self) -> pulumi.Output[str]:
+        """
+        Set the monitor access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "monitor_access_level")
+
+    @property
+    @pulumi.getter(name="mrDefaultTargetSelf")
+    def mr_default_target_self(self) -> pulumi.Output[Optional[bool]]:
+        """
+        For forked projects, target merge requests to this project. If false, the target will be the upstream project.
+        """
+        return pulumi.get(self, "mr_default_target_self")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the project.
         """
         return pulumi.get(self, "name")
 
@@ -3587,31 +4442,31 @@
         """
         The namespace (group or user) of the project. Defaults to your user.
         """
         return pulumi.get(self, "namespace_id")
 
     @property
     @pulumi.getter(name="onlyAllowMergeIfAllDiscussionsAreResolved")
-    def only_allow_merge_if_all_discussions_are_resolved(self) -> pulumi.Output[Optional[bool]]:
+    def only_allow_merge_if_all_discussions_are_resolved(self) -> pulumi.Output[bool]:
         """
         Set to true if you want allow merges only if all discussions are resolved.
         """
         return pulumi.get(self, "only_allow_merge_if_all_discussions_are_resolved")
 
     @property
     @pulumi.getter(name="onlyAllowMergeIfPipelineSucceeds")
-    def only_allow_merge_if_pipeline_succeeds(self) -> pulumi.Output[Optional[bool]]:
+    def only_allow_merge_if_pipeline_succeeds(self) -> pulumi.Output[bool]:
         """
         Set to true if you want allow merges only if a pipeline succeeds.
         """
         return pulumi.get(self, "only_allow_merge_if_pipeline_succeeds")
 
     @property
     @pulumi.getter(name="onlyMirrorProtectedBranches")
-    def only_mirror_protected_branches(self) -> pulumi.Output[Optional[bool]]:
+    def only_mirror_protected_branches(self) -> pulumi.Output[bool]:
         """
         Enable only mirror protected branches for a mirrored project.
         """
         return pulumi.get(self, "only_mirror_protected_branches")
 
     @property
     @pulumi.getter(name="operationsAccessLevel")
@@ -3619,23 +4474,23 @@
         """
         Set the operations access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "operations_access_level")
 
     @property
     @pulumi.getter(name="packagesEnabled")
-    def packages_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def packages_enabled(self) -> pulumi.Output[bool]:
         """
         Enable packages repository for the project.
         """
         return pulumi.get(self, "packages_enabled")
 
     @property
     @pulumi.getter(name="pagesAccessLevel")
-    def pages_access_level(self) -> pulumi.Output[Optional[str]]:
+    def pages_access_level(self) -> pulumi.Output[str]:
         """
         Enable pages access control
         """
         return pulumi.get(self, "pages_access_level")
 
     @property
     @pulumi.getter
@@ -3651,47 +4506,55 @@
         """
         The path of the repository with namespace.
         """
         return pulumi.get(self, "path_with_namespace")
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
-    def pipelines_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def pipelines_enabled(self) -> pulumi.Output[bool]:
         """
-        Enable pipelines for the project.
+        Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
         return pulumi.get(self, "pipelines_enabled")
 
     @property
     @pulumi.getter(name="printingMergeRequestLinkEnabled")
-    def printing_merge_request_link_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def printing_merge_request_link_enabled(self) -> pulumi.Output[bool]:
         """
         Show link to create/view merge request when pushing from the command line
         """
         return pulumi.get(self, "printing_merge_request_link_enabled")
 
     @property
     @pulumi.getter(name="publicBuilds")
-    def public_builds(self) -> pulumi.Output[Optional[bool]]:
+    def public_builds(self) -> pulumi.Output[bool]:
         """
         If true, jobs can be viewed by non-project members.
         """
         return pulumi.get(self, "public_builds")
 
     @property
     @pulumi.getter(name="pushRules")
     def push_rules(self) -> pulumi.Output['outputs.ProjectPushRules']:
         """
         Push rules for the project.
         """
         return pulumi.get(self, "push_rules")
 
     @property
+    @pulumi.getter(name="releasesAccessLevel")
+    def releases_access_level(self) -> pulumi.Output[str]:
+        """
+        Set the releases access level. Valid values are `disabled`, `private`, `enabled`.
+        """
+        return pulumi.get(self, "releases_access_level")
+
+    @property
     @pulumi.getter(name="removeSourceBranchAfterMerge")
-    def remove_source_branch_after_merge(self) -> pulumi.Output[Optional[bool]]:
+    def remove_source_branch_after_merge(self) -> pulumi.Output[bool]:
         """
         Enable `Delete source branch` option by default for all new merge requests.
         """
         return pulumi.get(self, "remove_source_branch_after_merge")
 
     @property
     @pulumi.getter(name="repositoryAccessLevel")
@@ -3707,15 +4570,15 @@
         """
         Which storage shard the repository is on. (administrator only)
         """
         return pulumi.get(self, "repository_storage")
 
     @property
     @pulumi.getter(name="requestAccessEnabled")
-    def request_access_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def request_access_enabled(self) -> pulumi.Output[bool]:
         """
         Allow users to request member access.
         """
         return pulumi.get(self, "request_access_enabled")
 
     @property
     @pulumi.getter(name="requirementsAccessLevel")
@@ -3730,14 +4593,22 @@
     def resolve_outdated_diff_discussions(self) -> pulumi.Output[Optional[bool]]:
         """
         Automatically resolve merge request diffs discussions on lines changed with a push.
         """
         return pulumi.get(self, "resolve_outdated_diff_discussions")
 
     @property
+    @pulumi.getter(name="restrictUserDefinedVariables")
+    def restrict_user_defined_variables(self) -> pulumi.Output[Optional[bool]]:
+        """
+        Allow only users with the Maintainer role to pass user-defined variables when triggering a pipeline.
+        """
+        return pulumi.get(self, "restrict_user_defined_variables")
+
+    @property
     @pulumi.getter(name="runnersToken")
     def runners_token(self) -> pulumi.Output[str]:
         """
         Registration token to use during runner setup.
         """
         return pulumi.get(self, "runners_token")
 
@@ -3774,15 +4645,15 @@
         """
         Set the snippets access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "snippets_access_level")
 
     @property
     @pulumi.getter(name="snippetsEnabled")
-    def snippets_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def snippets_enabled(self) -> pulumi.Output[bool]:
         """
         Enable snippets for the project.
         """
         return pulumi.get(self, "snippets_enabled")
 
     @property
     @pulumi.getter(name="squashCommitTemplate")
@@ -3790,29 +4661,37 @@
         """
         Template used to create squash commit message in merge requests. (Introduced in GitLab 14.6.)
         """
         return pulumi.get(self, "squash_commit_template")
 
     @property
     @pulumi.getter(name="squashOption")
-    def squash_option(self) -> pulumi.Output[Optional[str]]:
+    def squash_option(self) -> pulumi.Output[str]:
         """
         Squash commits when merge request. Valid values are `never`, `always`, `default_on`, or `default_off`. The default value is `default_off`. [GitLab >= 14.1]
         """
         return pulumi.get(self, "squash_option")
 
     @property
     @pulumi.getter(name="sshUrlToRepo")
     def ssh_url_to_repo(self) -> pulumi.Output[str]:
         """
         URL that can be provided to `git clone` to clone the
         """
         return pulumi.get(self, "ssh_url_to_repo")
 
     @property
+    @pulumi.getter(name="suggestionCommitMessage")
+    def suggestion_commit_message(self) -> pulumi.Output[Optional[str]]:
+        """
+        The commit message used to apply merge request suggestions.
+        """
+        return pulumi.get(self, "suggestion_commit_message")
+
+    @property
     @pulumi.getter
     def tags(self) -> pulumi.Output[Sequence[str]]:
         """
         The list of tags for a project; put array of tags, that should be finally assigned to a project. Use topics instead.
         """
         return pulumi.get(self, "tags")
 
@@ -3841,20 +4720,21 @@
         return pulumi.get(self, "topics")
 
     @property
     @pulumi.getter(name="useCustomTemplate")
     def use_custom_template(self) -> pulumi.Output[Optional[bool]]:
         """
         Use either custom instance or group (with group*with*project*templates*id) project template (enterprise edition).
+        	> When using a custom template, [Group Tokens won't work](https://docs.gitlab.com/15.7/ee/user/project/settings/import_export_troubleshooting.html#import-using-the-rest-api-fails-when-using-a-group-access-token). You must use a real user's Personal Access Token.
         """
         return pulumi.get(self, "use_custom_template")
 
     @property
     @pulumi.getter(name="visibilityLevel")
-    def visibility_level(self) -> pulumi.Output[Optional[str]]:
+    def visibility_level(self) -> pulumi.Output[str]:
         """
         Set to `public` to create a public project.
         """
         return pulumi.get(self, "visibility_level")
 
     @property
     @pulumi.getter(name="webUrl")
@@ -3870,13 +4750,13 @@
         """
         Set the wiki access level. Valid values are `disabled`, `private`, `enabled`.
         """
         return pulumi.get(self, "wiki_access_level")
 
     @property
     @pulumi.getter(name="wikiEnabled")
-    def wiki_enabled(self) -> pulumi.Output[Optional[bool]]:
+    def wiki_enabled(self) -> pulumi.Output[bool]:
         """
         Enable wiki for the project.
         """
         return pulumi.get(self, "wiki_enabled")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_access_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  scopes: pulumi.Input[Sequence[pulumi.Input[str]]],
                  access_level: Optional[pulumi.Input[str]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ProjectAccessToken resource.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
         :param pulumi.Input[str] name: A name to describe the project access token.
         """
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "scopes", scopes)
         if access_level is not None:
@@ -48,15 +48,15 @@
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def scopes(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         """
         return pulumi.get(self, "scopes")
 
     @scopes.setter
     def scopes(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "scopes", value)
 
@@ -115,15 +115,15 @@
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
         :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] token: The secret token. **Note**: the token is not available for imported resources.
         :param pulumi.Input[int] user_id: The user_id associated to the token.
         """
         if access_level is not None:
             pulumi.set(__self__, "access_level", access_level)
         if active is not None:
             pulumi.set(__self__, "active", active)
@@ -228,15 +228,15 @@
     def revoked(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "revoked", value)
 
     @property
     @pulumi.getter
     def scopes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         """
         return pulumi.get(self, "scopes")
 
     @scopes.setter
     def scopes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "scopes", value)
 
@@ -310,15 +310,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectAccessTokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -429,15 +429,15 @@
         :param pulumi.Input[str] access_level: The access level for the project access token. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`. Default is `maintainer`.
         :param pulumi.Input[bool] active: True if the token is active.
         :param pulumi.Input[str] created_at: Time the token has been created, RFC3339 format.
         :param pulumi.Input[str] expires_at: Time the token will expire it, YYYY-MM-DD format. Will not expire per default.
         :param pulumi.Input[str] name: A name to describe the project access token.
         :param pulumi.Input[str] project: The id of the project to add the project access token to.
         :param pulumi.Input[bool] revoked: True if the token is revoked.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] scopes: Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         :param pulumi.Input[str] token: The secret token. **Note**: the token is not available for imported resources.
         :param pulumi.Input[int] user_id: The user_id associated to the token.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectAccessTokenState.__new__(_ProjectAccessTokenState)
 
@@ -509,15 +509,15 @@
         """
         return pulumi.get(self, "revoked")
 
     @property
     @pulumi.getter
     def scopes(self) -> pulumi.Output[Sequence[str]]:
         """
-        Valid values: `api`, `read_api`, `read_repository`, `write_repository`.
+        Valid values: `api`, `read_api`, `read_repository`, `write_repository`, `read_registry`, `write_registry`.
         """
         return pulumi.get(self, "scopes")
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_approval_rule.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,35 @@
 __all__ = ['ProjectApprovalRuleArgs', 'ProjectApprovalRule']
 
 @pulumi.input_type
 class ProjectApprovalRuleArgs:
     def __init__(__self__, *,
                  approvals_required: pulumi.Input[int],
                  project: pulumi.Input[str],
+                 disable_importing_default_any_approver_rule_on_create: Optional[pulumi.Input[bool]] = None,
                  group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protected_branch_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  rule_type: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
         """
         The set of arguments for constructing a ProjectApprovalRule resource.
         :param pulumi.Input[int] approvals_required: The number of approvals required for this rule.
         :param pulumi.Input[str] project: The name or id of the project to add the approval rules.
+        :param pulumi.Input[bool] disable_importing_default_any_approver_rule_on_create: When this flag is set, the default `any_approver` rule will not be imported if present.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] group_ids: A list of group IDs whose members can approve of the merge request.
         :param pulumi.Input[str] name: The name of the approval rule.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] protected_branch_ids: A list of protected branch IDs (not branch names) for which the rule applies.
         :param pulumi.Input[str] rule_type: String, defaults to 'regular'. The type of rule. `any_approver` is a pre-configured default rule with `approvals_required` at `0`. Valid values are `regular`, `any_approver`.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] user_ids: A list of specific User IDs to add to the list of approvers.
         """
         pulumi.set(__self__, "approvals_required", approvals_required)
         pulumi.set(__self__, "project", project)
+        if disable_importing_default_any_approver_rule_on_create is not None:
+            pulumi.set(__self__, "disable_importing_default_any_approver_rule_on_create", disable_importing_default_any_approver_rule_on_create)
         if group_ids is not None:
             pulumi.set(__self__, "group_ids", group_ids)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if protected_branch_ids is not None:
             pulumi.set(__self__, "protected_branch_ids", protected_branch_ids)
         if rule_type is not None:
@@ -65,14 +69,26 @@
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
+    @pulumi.getter(name="disableImportingDefaultAnyApproverRuleOnCreate")
+    def disable_importing_default_any_approver_rule_on_create(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When this flag is set, the default `any_approver` rule will not be imported if present.
+        """
+        return pulumi.get(self, "disable_importing_default_any_approver_rule_on_create")
+
+    @disable_importing_default_any_approver_rule_on_create.setter
+    def disable_importing_default_any_approver_rule_on_create(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_importing_default_any_approver_rule_on_create", value)
+
+    @property
     @pulumi.getter(name="groupIds")
     def group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         A list of group IDs whose members can approve of the merge request.
         """
         return pulumi.get(self, "group_ids")
 
@@ -129,32 +145,36 @@
         pulumi.set(self, "user_ids", value)
 
 
 @pulumi.input_type
 class _ProjectApprovalRuleState:
     def __init__(__self__, *,
                  approvals_required: Optional[pulumi.Input[int]] = None,
+                 disable_importing_default_any_approver_rule_on_create: Optional[pulumi.Input[bool]] = None,
                  group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected_branch_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  rule_type: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
         """
         Input properties used for looking up and filtering ProjectApprovalRule resources.
         :param pulumi.Input[int] approvals_required: The number of approvals required for this rule.
+        :param pulumi.Input[bool] disable_importing_default_any_approver_rule_on_create: When this flag is set, the default `any_approver` rule will not be imported if present.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] group_ids: A list of group IDs whose members can approve of the merge request.
         :param pulumi.Input[str] name: The name of the approval rule.
         :param pulumi.Input[str] project: The name or id of the project to add the approval rules.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] protected_branch_ids: A list of protected branch IDs (not branch names) for which the rule applies.
         :param pulumi.Input[str] rule_type: String, defaults to 'regular'. The type of rule. `any_approver` is a pre-configured default rule with `approvals_required` at `0`. Valid values are `regular`, `any_approver`.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] user_ids: A list of specific User IDs to add to the list of approvers.
         """
         if approvals_required is not None:
             pulumi.set(__self__, "approvals_required", approvals_required)
+        if disable_importing_default_any_approver_rule_on_create is not None:
+            pulumi.set(__self__, "disable_importing_default_any_approver_rule_on_create", disable_importing_default_any_approver_rule_on_create)
         if group_ids is not None:
             pulumi.set(__self__, "group_ids", group_ids)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if protected_branch_ids is not None:
@@ -173,14 +193,26 @@
         return pulumi.get(self, "approvals_required")
 
     @approvals_required.setter
     def approvals_required(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "approvals_required", value)
 
     @property
+    @pulumi.getter(name="disableImportingDefaultAnyApproverRuleOnCreate")
+    def disable_importing_default_any_approver_rule_on_create(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When this flag is set, the default `any_approver` rule will not be imported if present.
+        """
+        return pulumi.get(self, "disable_importing_default_any_approver_rule_on_create")
+
+    @disable_importing_default_any_approver_rule_on_create.setter
+    def disable_importing_default_any_approver_rule_on_create(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_importing_default_any_approver_rule_on_create", value)
+
+    @property
     @pulumi.getter(name="groupIds")
     def group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]:
         """
         A list of group IDs whose members can approve of the merge request.
         """
         return pulumi.get(self, "group_ids")
 
@@ -251,59 +283,49 @@
 
 class ProjectApprovalRule(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  approvals_required: Optional[pulumi.Input[int]] = None,
+                 disable_importing_default_any_approver_rule_on_create: Optional[pulumi.Input[bool]] = None,
                  group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected_branch_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  rule_type: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  __props__=None):
         """
-        The `ProjectApprovalRule` resource allows to manage the lifecycle of a project-level approval rule.
-
-        > This resource requires a GitLab Enterprise instance.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/merge_request_approvals.html#project-level-mr-approvals)
-
         ## Import
 
         GitLab project approval rules can be imported using a key composed of `<project-id>:<rule-id>`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/projectApprovalRule:ProjectApprovalRule example "12345:6"
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] approvals_required: The number of approvals required for this rule.
+        :param pulumi.Input[bool] disable_importing_default_any_approver_rule_on_create: When this flag is set, the default `any_approver` rule will not be imported if present.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] group_ids: A list of group IDs whose members can approve of the merge request.
         :param pulumi.Input[str] name: The name of the approval rule.
         :param pulumi.Input[str] project: The name or id of the project to add the approval rules.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] protected_branch_ids: A list of protected branch IDs (not branch names) for which the rule applies.
         :param pulumi.Input[str] rule_type: String, defaults to 'regular'. The type of rule. `any_approver` is a pre-configured default rule with `approvals_required` at `0`. Valid values are `regular`, `any_approver`.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] user_ids: A list of specific User IDs to add to the list of approvers.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectApprovalRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ProjectApprovalRule` resource allows to manage the lifecycle of a project-level approval rule.
-
-        > This resource requires a GitLab Enterprise instance.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/merge_request_approvals.html#project-level-mr-approvals)
-
         ## Import
 
         GitLab project approval rules can be imported using a key composed of `<project-id>:<rule-id>`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/projectApprovalRule:ProjectApprovalRule example "12345:6"
         ```
@@ -320,14 +342,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  approvals_required: Optional[pulumi.Input[int]] = None,
+                 disable_importing_default_any_approver_rule_on_create: Optional[pulumi.Input[bool]] = None,
                  group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  protected_branch_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  rule_type: Optional[pulumi.Input[str]] = None,
                  user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  __props__=None):
@@ -338,14 +361,15 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectApprovalRuleArgs.__new__(ProjectApprovalRuleArgs)
 
             if approvals_required is None and not opts.urn:
                 raise TypeError("Missing required property 'approvals_required'")
             __props__.__dict__["approvals_required"] = approvals_required
+            __props__.__dict__["disable_importing_default_any_approver_rule_on_create"] = disable_importing_default_any_approver_rule_on_create
             __props__.__dict__["group_ids"] = group_ids
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             __props__.__dict__["protected_branch_ids"] = protected_branch_ids
             __props__.__dict__["rule_type"] = rule_type
@@ -357,40 +381,43 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             approvals_required: Optional[pulumi.Input[int]] = None,
+            disable_importing_default_any_approver_rule_on_create: Optional[pulumi.Input[bool]] = None,
             group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             protected_branch_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
             rule_type: Optional[pulumi.Input[str]] = None,
             user_ids: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None) -> 'ProjectApprovalRule':
         """
         Get an existing ProjectApprovalRule resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] approvals_required: The number of approvals required for this rule.
+        :param pulumi.Input[bool] disable_importing_default_any_approver_rule_on_create: When this flag is set, the default `any_approver` rule will not be imported if present.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] group_ids: A list of group IDs whose members can approve of the merge request.
         :param pulumi.Input[str] name: The name of the approval rule.
         :param pulumi.Input[str] project: The name or id of the project to add the approval rules.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] protected_branch_ids: A list of protected branch IDs (not branch names) for which the rule applies.
         :param pulumi.Input[str] rule_type: String, defaults to 'regular'. The type of rule. `any_approver` is a pre-configured default rule with `approvals_required` at `0`. Valid values are `regular`, `any_approver`.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] user_ids: A list of specific User IDs to add to the list of approvers.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ProjectApprovalRuleState.__new__(_ProjectApprovalRuleState)
 
         __props__.__dict__["approvals_required"] = approvals_required
+        __props__.__dict__["disable_importing_default_any_approver_rule_on_create"] = disable_importing_default_any_approver_rule_on_create
         __props__.__dict__["group_ids"] = group_ids
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
         __props__.__dict__["protected_branch_ids"] = protected_branch_ids
         __props__.__dict__["rule_type"] = rule_type
         __props__.__dict__["user_ids"] = user_ids
         return ProjectApprovalRule(resource_name, opts=opts, __props__=__props__)
@@ -400,14 +427,22 @@
     def approvals_required(self) -> pulumi.Output[int]:
         """
         The number of approvals required for this rule.
         """
         return pulumi.get(self, "approvals_required")
 
     @property
+    @pulumi.getter(name="disableImportingDefaultAnyApproverRuleOnCreate")
+    def disable_importing_default_any_approver_rule_on_create(self) -> pulumi.Output[Optional[bool]]:
+        """
+        When this flag is set, the default `any_approver` rule will not be imported if present.
+        """
+        return pulumi.get(self, "disable_importing_default_any_approver_rule_on_create")
+
+    @property
     @pulumi.getter(name="groupIds")
     def group_ids(self) -> pulumi.Output[Optional[Sequence[int]]]:
         """
         A list of group IDs whose members can approve of the merge request.
         """
         return pulumi.get(self, "group_ids")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_freeze_period.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         :param pulumi.Input[bool] confidential: Set an issue to be confidential.
         :param pulumi.Input[str] created_at: When the issue was created. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z. Requires administrator or project/group owner rights.
         :param pulumi.Input[bool] delete_on_destroy: Whether the issue is deleted instead of closed during destroy.
         :param pulumi.Input[str] description: The description of an issue. Limited to 1,048,576 characters.
         :param pulumi.Input[bool] discussion_locked: Whether the issue is locked for discussions or not.
         :param pulumi.Input[str] discussion_to_resolve: The ID of a discussion to resolve. This fills out the issue with a default description and mark the discussion as resolved. Use in combination with merge*request*to*resolve*discussions_of.
         :param pulumi.Input[str] due_date: The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-               **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         :param pulumi.Input[int] epic_issue_id: The ID of the epic issue.
         :param pulumi.Input[int] iid: The internal ID of the project's issue.
         :param pulumi.Input[str] issue_type: The type of issue. Valid values are: `issue`, `incident`, `test_case`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] labels: The labels of an issue.
         :param pulumi.Input[int] merge_request_to_resolve_discussions_of: The IID of a merge request in which to resolve all issues. This fills out the issue with a default description and mark all discussions as resolved. When passing a description or title, these values take precedence over the default values.
         :param pulumi.Input[int] milestone_id: The global ID of a milestone to assign issue. To find the milestone_id associated with a milestone, view an issue with the milestone assigned and use the API to retrieve the issue's details.
         :param pulumi.Input[str] state: The state of the issue. Valid values are: `opened`, `closed`.
@@ -204,15 +203,14 @@
         pulumi.set(self, "discussion_to_resolve", value)
 
     @property
     @pulumi.getter(name="dueDate")
     def due_date(self) -> Optional[pulumi.Input[str]]:
         """
         The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         """
         return pulumi.get(self, "due_date")
 
     @due_date.setter
     def due_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "due_date", value)
 
@@ -378,15 +376,14 @@
         :param pulumi.Input[str] created_at: When the issue was created. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z. Requires administrator or project/group owner rights.
         :param pulumi.Input[bool] delete_on_destroy: Whether the issue is deleted instead of closed during destroy.
         :param pulumi.Input[str] description: The description of an issue. Limited to 1,048,576 characters.
         :param pulumi.Input[bool] discussion_locked: Whether the issue is locked for discussions or not.
         :param pulumi.Input[str] discussion_to_resolve: The ID of a discussion to resolve. This fills out the issue with a default description and mark the discussion as resolved. Use in combination with merge*request*to*resolve*discussions_of.
         :param pulumi.Input[int] downvotes: The number of downvotes the issue has received.
         :param pulumi.Input[str] due_date: The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-               **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         :param pulumi.Input[int] epic_id: ID of the epic to add the issue to. Valid values are greater than or equal to 0.
         :param pulumi.Input[int] epic_issue_id: The ID of the epic issue.
         :param pulumi.Input[str] external_id: The external ID of the issue.
         :param pulumi.Input[str] human_time_estimate: The human-readable time estimate of the issue.
         :param pulumi.Input[str] human_total_time_spent: The human-readable total time spent of the issue.
         :param pulumi.Input[int] iid: The internal ID of the project's issue.
         :param pulumi.Input[int] issue_id: The instance-wide ID of the issue.
@@ -626,15 +623,14 @@
         pulumi.set(self, "downvotes", value)
 
     @property
     @pulumi.getter(name="dueDate")
     def due_date(self) -> Optional[pulumi.Input[str]]:
         """
         The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         """
         return pulumi.get(self, "due_date")
 
     @due_date.setter
     def due_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "due_date", value)
 
@@ -1034,15 +1030,14 @@
         :param pulumi.Input[bool] confidential: Set an issue to be confidential.
         :param pulumi.Input[str] created_at: When the issue was created. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z. Requires administrator or project/group owner rights.
         :param pulumi.Input[bool] delete_on_destroy: Whether the issue is deleted instead of closed during destroy.
         :param pulumi.Input[str] description: The description of an issue. Limited to 1,048,576 characters.
         :param pulumi.Input[bool] discussion_locked: Whether the issue is locked for discussions or not.
         :param pulumi.Input[str] discussion_to_resolve: The ID of a discussion to resolve. This fills out the issue with a default description and mark the discussion as resolved. Use in combination with merge*request*to*resolve*discussions_of.
         :param pulumi.Input[str] due_date: The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-               **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         :param pulumi.Input[int] epic_issue_id: The ID of the epic issue.
         :param pulumi.Input[int] iid: The internal ID of the project's issue.
         :param pulumi.Input[str] issue_type: The type of issue. Valid values are: `issue`, `incident`, `test_case`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] labels: The labels of an issue.
         :param pulumi.Input[int] merge_request_to_resolve_discussions_of: The IID of a merge request in which to resolve all issues. This fills out the issue with a default description and mark all discussions as resolved. When passing a description or title, these values take precedence over the default values.
         :param pulumi.Input[int] milestone_id: The global ID of a milestone to assign issue. To find the milestone_id associated with a milestone, view an issue with the milestone assigned and use the API to retrieve the issue's details.
         :param pulumi.Input[str] project: The name or ID of the project.
@@ -1237,15 +1232,14 @@
         :param pulumi.Input[str] created_at: When the issue was created. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z. Requires administrator or project/group owner rights.
         :param pulumi.Input[bool] delete_on_destroy: Whether the issue is deleted instead of closed during destroy.
         :param pulumi.Input[str] description: The description of an issue. Limited to 1,048,576 characters.
         :param pulumi.Input[bool] discussion_locked: Whether the issue is locked for discussions or not.
         :param pulumi.Input[str] discussion_to_resolve: The ID of a discussion to resolve. This fills out the issue with a default description and mark the discussion as resolved. Use in combination with merge*request*to*resolve*discussions_of.
         :param pulumi.Input[int] downvotes: The number of downvotes the issue has received.
         :param pulumi.Input[str] due_date: The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-               **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         :param pulumi.Input[int] epic_id: ID of the epic to add the issue to. Valid values are greater than or equal to 0.
         :param pulumi.Input[int] epic_issue_id: The ID of the epic issue.
         :param pulumi.Input[str] external_id: The external ID of the issue.
         :param pulumi.Input[str] human_time_estimate: The human-readable time estimate of the issue.
         :param pulumi.Input[str] human_total_time_spent: The human-readable total time spent of the issue.
         :param pulumi.Input[int] iid: The internal ID of the project's issue.
         :param pulumi.Input[int] issue_id: The instance-wide ID of the issue.
@@ -1406,15 +1400,14 @@
         return pulumi.get(self, "downvotes")
 
     @property
     @pulumi.getter(name="dueDate")
     def due_date(self) -> pulumi.Output[Optional[str]]:
         """
         The due date. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        **Note:** removing a due date is currently not supported, see https://github.com/xanzy/go-gitlab/issues/1384 for details.
         """
         return pulumi.get(self, "due_date")
 
     @property
     @pulumi.getter(name="epicId")
     def epic_id(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_membership.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_level: Optional[pulumi.Input[str]] = None,
                  expires_at: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        The `ProjectMembership` resource allows to manage the lifecycle of a users project membersip.
+        The `ProjectMembership` resource allows to manage the lifecycle of a users project membership.
 
         > If a project should grant membership to an entire group use the `ProjectShareGroup` resource instead.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html)
 
         ## Example Usage
 
@@ -204,15 +204,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectMembershipArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ProjectMembership` resource allows to manage the lifecycle of a users project membersip.
+        The `ProjectMembership` resource allows to manage the lifecycle of a users project membership.
 
         > If a project should grant membership to an entire group use the `ProjectShareGroup` resource instead.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/members.html)
 
         ## Example Usage
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_milestone.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                  updated_at: Optional[pulumi.Input[str]] = None,
                  web_url: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ProjectMilestone resources.
         :param pulumi.Input[str] created_at: The time of creation of the milestone. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z.
         :param pulumi.Input[str] description: The description of the milestone.
         :param pulumi.Input[str] due_date: The due date of the milestone. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        :param pulumi.Input[bool] expired: Bool, true if milestore expired.
+        :param pulumi.Input[bool] expired: Bool, true if milestone expired.
         :param pulumi.Input[int] iid: The ID of the project's milestone.
         :param pulumi.Input[int] milestone_id: The instance-wide ID of the project’s milestone.
         :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
         :param pulumi.Input[int] project_id: The project ID of milestone.
         :param pulumi.Input[str] start_date: The start date of the milestone. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
         :param pulumi.Input[str] state: The state of the milestone. Valid values are: `active`, `closed`.
         :param pulumi.Input[str] title: The title of a milestone.
@@ -208,15 +208,15 @@
     def due_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "due_date", value)
 
     @property
     @pulumi.getter
     def expired(self) -> Optional[pulumi.Input[bool]]:
         """
-        Bool, true if milestore expired.
+        Bool, true if milestone expired.
         """
         return pulumi.get(self, "expired")
 
     @expired.setter
     def expired(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "expired", value)
 
@@ -488,15 +488,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The time of creation of the milestone. Date time string, ISO 8601 formatted, for example 2016-03-11T03:45:40Z.
         :param pulumi.Input[str] description: The description of the milestone.
         :param pulumi.Input[str] due_date: The due date of the milestone. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
-        :param pulumi.Input[bool] expired: Bool, true if milestore expired.
+        :param pulumi.Input[bool] expired: Bool, true if milestone expired.
         :param pulumi.Input[int] iid: The ID of the project's milestone.
         :param pulumi.Input[int] milestone_id: The instance-wide ID of the project’s milestone.
         :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
         :param pulumi.Input[int] project_id: The project ID of milestone.
         :param pulumi.Input[str] start_date: The start date of the milestone. Date time string in the format YYYY-MM-DD, for example 2016-03-11.
         :param pulumi.Input[str] state: The state of the milestone. Valid values are: `active`, `closed`.
         :param pulumi.Input[str] title: The title of a milestone.
@@ -546,15 +546,15 @@
         """
         return pulumi.get(self, "due_date")
 
     @property
     @pulumi.getter
     def expired(self) -> pulumi.Output[bool]:
         """
-        Bool, true if milestore expired.
+        Bool, true if milestone expired.
         """
         return pulumi.get(self, "expired")
 
     @property
     @pulumi.getter
     def iid(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_mirror.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_protected_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,44 +12,33 @@
 from ._inputs import *
 
 __all__ = ['ProjectProtectedEnvironmentArgs', 'ProjectProtectedEnvironment']
 
 @pulumi.input_type
 class ProjectProtectedEnvironmentArgs:
     def __init__(__self__, *,
-                 deploy_access_levels: pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]],
                  environment: pulumi.Input[str],
                  project: pulumi.Input[str],
+                 deploy_access_levels: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]]] = None,
                  required_approval_count: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a ProjectProtectedEnvironment resource.
-        :param pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]] deploy_access_levels: Array of access levels allowed to deploy, with each described by a hash.
         :param pulumi.Input[str] environment: The name of the environment.
         :param pulumi.Input[str] project: The ID or full path of the project which the protected environment is created against.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]] deploy_access_levels: Array of access levels allowed to deploy, with each described by a hash.
         :param pulumi.Input[int] required_approval_count: The number of approvals required to deploy to this environment.
         """
-        pulumi.set(__self__, "deploy_access_levels", deploy_access_levels)
         pulumi.set(__self__, "environment", environment)
         pulumi.set(__self__, "project", project)
+        if deploy_access_levels is not None:
+            pulumi.set(__self__, "deploy_access_levels", deploy_access_levels)
         if required_approval_count is not None:
             pulumi.set(__self__, "required_approval_count", required_approval_count)
 
     @property
-    @pulumi.getter(name="deployAccessLevels")
-    def deploy_access_levels(self) -> pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]]:
-        """
-        Array of access levels allowed to deploy, with each described by a hash.
-        """
-        return pulumi.get(self, "deploy_access_levels")
-
-    @deploy_access_levels.setter
-    def deploy_access_levels(self, value: pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]]):
-        pulumi.set(self, "deploy_access_levels", value)
-
-    @property
     @pulumi.getter
     def environment(self) -> pulumi.Input[str]:
         """
         The name of the environment.
         """
         return pulumi.get(self, "environment")
 
@@ -66,14 +55,26 @@
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
+    @pulumi.getter(name="deployAccessLevels")
+    def deploy_access_levels(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]]]:
+        """
+        Array of access levels allowed to deploy, with each described by a hash.
+        """
+        return pulumi.get(self, "deploy_access_levels")
+
+    @deploy_access_levels.setter
+    def deploy_access_levels(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectProtectedEnvironmentDeployAccessLevelArgs']]]]):
+        pulumi.set(self, "deploy_access_levels", value)
+
+    @property
     @pulumi.getter(name="requiredApprovalCount")
     def required_approval_count(self) -> Optional[pulumi.Input[int]]:
         """
         The number of approvals required to deploy to this environment.
         """
         return pulumi.get(self, "required_approval_count")
 
@@ -337,16 +338,14 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProjectProtectedEnvironmentArgs.__new__(ProjectProtectedEnvironmentArgs)
 
-            if deploy_access_levels is None and not opts.urn:
-                raise TypeError("Missing required property 'deploy_access_levels'")
             __props__.__dict__["deploy_access_levels"] = deploy_access_levels
             if environment is None and not opts.urn:
                 raise TypeError("Missing required property 'environment'")
             __props__.__dict__["environment"] = environment
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
@@ -385,15 +384,15 @@
         __props__.__dict__["environment"] = environment
         __props__.__dict__["project"] = project
         __props__.__dict__["required_approval_count"] = required_approval_count
         return ProjectProtectedEnvironment(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="deployAccessLevels")
-    def deploy_access_levels(self) -> pulumi.Output[Sequence['outputs.ProjectProtectedEnvironmentDeployAccessLevel']]:
+    def deploy_access_levels(self) -> pulumi.Output[Optional[Sequence['outputs.ProjectProtectedEnvironmentDeployAccessLevel']]]:
         """
         Array of access levels allowed to deploy, with each described by a hash.
         """
         return pulumi.get(self, "deploy_access_levels")
 
     @property
     @pulumi.getter
@@ -409,13 +408,13 @@
         """
         The ID or full path of the project which the protected environment is created against.
         """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter(name="requiredApprovalCount")
-    def required_approval_count(self) -> pulumi.Output[Optional[int]]:
+    def required_approval_count(self) -> pulumi.Output[int]:
         """
         The number of approvals required to deploy to this environment.
         """
         return pulumi.get(self, "required_approval_count")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_tag.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/provider.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,69 +10,56 @@
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
-                 token: pulumi.Input[str],
                  base_url: Optional[pulumi.Input[str]] = None,
                  cacert_file: Optional[pulumi.Input[str]] = None,
                  client_cert: Optional[pulumi.Input[str]] = None,
                  client_key: Optional[pulumi.Input[str]] = None,
                  early_auth_check: Optional[pulumi.Input[bool]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None):
+                 insecure: Optional[pulumi.Input[bool]] = None,
+                 token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] token: The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
-               used in this provider for authentication (using Bearer authorization token). See
-               https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
-               variable.
         :param pulumi.Input[str] base_url: This is the target GitLab base API endpoint. Providing a value is a requirement when working with GitLab CE or GitLab
                Enterprise e.g. `https://my.gitlab.server/api/v4/`. It is optional to provide this value and it can also be sourced from
                the `GITLAB_BASE_URL` environment variable. The value must end with a slash.
         :param pulumi.Input[str] cacert_file: This is a file containing the ca cert to verify the gitlab instance. This is available for use when working with GitLab
                CE or Gitlab Enterprise with a locally-issued or self-signed certificate chain.
         :param pulumi.Input[str] client_cert: File path to client certificate when GitLab instance is behind company proxy. File must contain PEM encoded data.
         :param pulumi.Input[str] client_key: File path to client key when GitLab instance is behind company proxy. File must contain PEM encoded data. Required when
                `client_cert` is set.
         :param pulumi.Input[bool] early_auth_check: (Experimental) By default the provider does a dummy request to get the current user in order to verify that the provider
-               configuration is correct and the GitLab API is reachable. Turn it off, to skip this check. This may be useful if the
-               GitLab instance does not yet exist and is created within the same terraform module. This is an experimental feature and
-               may change in the future. Please make sure to always keep backups of your state.
+               configuration is correct and the GitLab API is reachable. Set this to `false` to skip this check. This may be useful if
+               the GitLab instance does not yet exist and is created within the same terraform module. It may be sourced from the
+               `GITLAB_EARLY_AUTH_CHECK`. This is an experimental feature and may change in the future. Please make sure to always keep
+               backups of your state.
         :param pulumi.Input[bool] insecure: When set to true this disables SSL verification of the connection to the GitLab instance.
+        :param pulumi.Input[str] token: The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
+               used in this provider for authentication (using Bearer authorization token). See
+               https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
+               variable.
         """
-        pulumi.set(__self__, "token", token)
         if base_url is not None:
             pulumi.set(__self__, "base_url", base_url)
         if cacert_file is not None:
             pulumi.set(__self__, "cacert_file", cacert_file)
         if client_cert is not None:
             pulumi.set(__self__, "client_cert", client_cert)
         if client_key is not None:
             pulumi.set(__self__, "client_key", client_key)
         if early_auth_check is not None:
             pulumi.set(__self__, "early_auth_check", early_auth_check)
         if insecure is not None:
             pulumi.set(__self__, "insecure", insecure)
-
-    @property
-    @pulumi.getter
-    def token(self) -> pulumi.Input[str]:
-        """
-        The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
-        used in this provider for authentication (using Bearer authorization token). See
-        https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
-        variable.
-        """
-        return pulumi.get(self, "token")
-
-    @token.setter
-    def token(self, value: pulumi.Input[str]):
-        pulumi.set(self, "token", value)
+        if token is not None:
+            pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="baseUrl")
     def base_url(self) -> Optional[pulumi.Input[str]]:
         """
         This is the target GitLab base API endpoint. Providing a value is a requirement when working with GitLab CE or GitLab
         Enterprise e.g. `https://my.gitlab.server/api/v4/`. It is optional to provide this value and it can also be sourced from
@@ -123,17 +110,18 @@
         pulumi.set(self, "client_key", value)
 
     @property
     @pulumi.getter(name="earlyAuthCheck")
     def early_auth_check(self) -> Optional[pulumi.Input[bool]]:
         """
         (Experimental) By default the provider does a dummy request to get the current user in order to verify that the provider
-        configuration is correct and the GitLab API is reachable. Turn it off, to skip this check. This may be useful if the
-        GitLab instance does not yet exist and is created within the same terraform module. This is an experimental feature and
-        may change in the future. Please make sure to always keep backups of your state.
+        configuration is correct and the GitLab API is reachable. Set this to `false` to skip this check. This may be useful if
+        the GitLab instance does not yet exist and is created within the same terraform module. It may be sourced from the
+        `GITLAB_EARLY_AUTH_CHECK`. This is an experimental feature and may change in the future. Please make sure to always keep
+        backups of your state.
         """
         return pulumi.get(self, "early_auth_check")
 
     @early_auth_check.setter
     def early_auth_check(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "early_auth_check", value)
 
@@ -145,14 +133,29 @@
         """
         return pulumi.get(self, "insecure")
 
     @insecure.setter
     def insecure(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "insecure", value)
 
+    @property
+    @pulumi.getter
+    def token(self) -> Optional[pulumi.Input[str]]:
+        """
+        The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
+        used in this provider for authentication (using Bearer authorization token). See
+        https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
+        variable.
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token", value)
+
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  base_url: Optional[pulumi.Input[str]] = None,
@@ -176,28 +179,29 @@
                the `GITLAB_BASE_URL` environment variable. The value must end with a slash.
         :param pulumi.Input[str] cacert_file: This is a file containing the ca cert to verify the gitlab instance. This is available for use when working with GitLab
                CE or Gitlab Enterprise with a locally-issued or self-signed certificate chain.
         :param pulumi.Input[str] client_cert: File path to client certificate when GitLab instance is behind company proxy. File must contain PEM encoded data.
         :param pulumi.Input[str] client_key: File path to client key when GitLab instance is behind company proxy. File must contain PEM encoded data. Required when
                `client_cert` is set.
         :param pulumi.Input[bool] early_auth_check: (Experimental) By default the provider does a dummy request to get the current user in order to verify that the provider
-               configuration is correct and the GitLab API is reachable. Turn it off, to skip this check. This may be useful if the
-               GitLab instance does not yet exist and is created within the same terraform module. This is an experimental feature and
-               may change in the future. Please make sure to always keep backups of your state.
+               configuration is correct and the GitLab API is reachable. Set this to `false` to skip this check. This may be useful if
+               the GitLab instance does not yet exist and is created within the same terraform module. It may be sourced from the
+               `GITLAB_EARLY_AUTH_CHECK`. This is an experimental feature and may change in the future. Please make sure to always keep
+               backups of your state.
         :param pulumi.Input[bool] insecure: When set to true this disables SSL verification of the connection to the GitLab instance.
         :param pulumi.Input[str] token: The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
                used in this provider for authentication (using Bearer authorization token). See
                https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
                variable.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProviderArgs,
+                 args: Optional[ProviderArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The provider type for the gitlab package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
@@ -234,17 +238,17 @@
 
             __props__.__dict__["base_url"] = base_url
             __props__.__dict__["cacert_file"] = cacert_file
             __props__.__dict__["client_cert"] = client_cert
             __props__.__dict__["client_key"] = client_key
             __props__.__dict__["early_auth_check"] = pulumi.Output.from_input(early_auth_check).apply(pulumi.runtime.to_json) if early_auth_check is not None else None
             __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
-            if token is None and not opts.urn:
-                raise TypeError("Missing required property 'token'")
-            __props__.__dict__["token"] = token
+            __props__.__dict__["token"] = None if token is None else pulumi.Output.secret(token)
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["token"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Provider, __self__).__init__(
             'gitlab',
             resource_name,
             __props__,
             opts)
 
     @property
@@ -281,15 +285,15 @@
         File path to client key when GitLab instance is behind company proxy. File must contain PEM encoded data. Required when
         `client_cert` is set.
         """
         return pulumi.get(self, "client_key")
 
     @property
     @pulumi.getter
-    def token(self) -> pulumi.Output[str]:
+    def token(self) -> pulumi.Output[Optional[str]]:
         """
         The OAuth2 Token, Project, Group, Personal Access Token or CI Job Token used to connect to GitLab. The OAuth method is
         used in this provider for authentication (using Bearer authorization token). See
         https://docs.gitlab.com/ee/api/#authentication for details. It may be sourced from the `GITLAB_TOKEN` environment
         variable.
         """
         return pulumi.get(self, "token")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/release_link.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,758 +5,779 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['RepositoryFileArgs', 'RepositoryFile']
+__all__ = ['UserArgs', 'User']
 
 @pulumi.input_type
-class RepositoryFileArgs:
+class UserArgs:
     def __init__(__self__, *,
-                 branch: pulumi.Input[str],
-                 commit_message: pulumi.Input[str],
-                 content: pulumi.Input[str],
-                 file_path: pulumi.Input[str],
-                 project: pulumi.Input[str],
-                 author_email: Optional[pulumi.Input[str]] = None,
-                 author_name: Optional[pulumi.Input[str]] = None,
-                 execute_filemode: Optional[pulumi.Input[bool]] = None,
-                 start_branch: Optional[pulumi.Input[str]] = None):
+                 email: pulumi.Input[str],
+                 username: pulumi.Input[str],
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
+                 is_admin: Optional[pulumi.Input[bool]] = None,
+                 is_external: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 namespace_id: Optional[pulumi.Input[int]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 projects_limit: Optional[pulumi.Input[int]] = None,
+                 reset_password: Optional[pulumi.Input[bool]] = None,
+                 skip_confirmation: Optional[pulumi.Input[bool]] = None,
+                 state: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a RepositoryFile resource.
-        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
-        :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
-        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/`.
-        :param pulumi.Input[str] project: The name or ID of the project.
-        :param pulumi.Input[str] author_email: Email of the commit author.
-        :param pulumi.Input[str] author_name: Name of the commit author.
-        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
-        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
+        The set of arguments for constructing a User resource.
+        :param pulumi.Input[str] email: The e-mail address of the user.
+        :param pulumi.Input[str] username: The username of the user.
+        :param pulumi.Input[bool] can_create_group: Boolean, defaults to false. Whether to allow the user to create groups.
+        :param pulumi.Input[bool] is_admin: Boolean, defaults to false.  Whether to enable administrative privileges
+        :param pulumi.Input[bool] is_external: Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
+        :param pulumi.Input[str] name: The name of the user.
+        :param pulumi.Input[int] namespace_id: The ID of the user's namespace. Available since GitLab 14.10.
+        :param pulumi.Input[str] note: The note associated to the user.
+        :param pulumi.Input[str] password: The password of the user.
+        :param pulumi.Input[int] projects_limit: Integer, defaults to 0.  Number of projects user can create.
+        :param pulumi.Input[bool] reset_password: Boolean, defaults to false. Send user password reset link.
+        :param pulumi.Input[bool] skip_confirmation: Boolean, defaults to true. Whether to skip confirmation.
+        :param pulumi.Input[str] state: String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
         """
-        pulumi.set(__self__, "branch", branch)
-        pulumi.set(__self__, "commit_message", commit_message)
-        pulumi.set(__self__, "content", content)
-        pulumi.set(__self__, "file_path", file_path)
-        pulumi.set(__self__, "project", project)
-        if author_email is not None:
-            pulumi.set(__self__, "author_email", author_email)
-        if author_name is not None:
-            pulumi.set(__self__, "author_name", author_name)
-        if execute_filemode is not None:
-            pulumi.set(__self__, "execute_filemode", execute_filemode)
-        if start_branch is not None:
-            pulumi.set(__self__, "start_branch", start_branch)
+        pulumi.set(__self__, "email", email)
+        pulumi.set(__self__, "username", username)
+        if can_create_group is not None:
+            pulumi.set(__self__, "can_create_group", can_create_group)
+        if is_admin is not None:
+            pulumi.set(__self__, "is_admin", is_admin)
+        if is_external is not None:
+            pulumi.set(__self__, "is_external", is_external)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace_id is not None:
+            pulumi.set(__self__, "namespace_id", namespace_id)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if projects_limit is not None:
+            pulumi.set(__self__, "projects_limit", projects_limit)
+        if reset_password is not None:
+            pulumi.set(__self__, "reset_password", reset_password)
+        if skip_confirmation is not None:
+            pulumi.set(__self__, "skip_confirmation", skip_confirmation)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
 
     @property
     @pulumi.getter
-    def branch(self) -> pulumi.Input[str]:
+    def email(self) -> pulumi.Input[str]:
         """
-        Name of the branch to which to commit to.
+        The e-mail address of the user.
         """
-        return pulumi.get(self, "branch")
+        return pulumi.get(self, "email")
 
-    @branch.setter
-    def branch(self, value: pulumi.Input[str]):
-        pulumi.set(self, "branch", value)
+    @email.setter
+    def email(self, value: pulumi.Input[str]):
+        pulumi.set(self, "email", value)
 
     @property
-    @pulumi.getter(name="commitMessage")
-    def commit_message(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def username(self) -> pulumi.Input[str]:
         """
-        Commit message.
+        The username of the user.
         """
-        return pulumi.get(self, "commit_message")
+        return pulumi.get(self, "username")
 
-    @commit_message.setter
-    def commit_message(self, value: pulumi.Input[str]):
-        pulumi.set(self, "commit_message", value)
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
 
     @property
-    @pulumi.getter
-    def content(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> Optional[pulumi.Input[bool]]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        Boolean, defaults to false. Whether to allow the user to create groups.
         """
-        return pulumi.get(self, "content")
+        return pulumi.get(self, "can_create_group")
 
-    @content.setter
-    def content(self, value: pulumi.Input[str]):
-        pulumi.set(self, "content", value)
+    @can_create_group.setter
+    def can_create_group(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "can_create_group", value)
 
     @property
-    @pulumi.getter(name="filePath")
-    def file_path(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="isAdmin")
+    def is_admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        The full path of the file. It must be relative to the root of the project without a leading slash `/`.
+        Boolean, defaults to false.  Whether to enable administrative privileges
         """
-        return pulumi.get(self, "file_path")
+        return pulumi.get(self, "is_admin")
 
-    @file_path.setter
-    def file_path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "file_path", value)
+    @is_admin.setter
+    def is_admin(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "is_admin", value)
 
     @property
-    @pulumi.getter
-    def project(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="isExternal")
+    def is_external(self) -> Optional[pulumi.Input[bool]]:
         """
-        The name or ID of the project.
+        Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "is_external")
 
-    @project.setter
-    def project(self, value: pulumi.Input[str]):
-        pulumi.set(self, "project", value)
+    @is_external.setter
+    def is_external(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "is_external", value)
 
     @property
-    @pulumi.getter(name="authorEmail")
-    def author_email(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Email of the commit author.
+        The name of the user.
         """
-        return pulumi.get(self, "author_email")
+        return pulumi.get(self, "name")
 
-    @author_email.setter
-    def author_email(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "author_email", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="authorName")
-    def author_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="namespaceId")
+    def namespace_id(self) -> Optional[pulumi.Input[int]]:
         """
-        Name of the commit author.
+        The ID of the user's namespace. Available since GitLab 14.10.
         """
-        return pulumi.get(self, "author_name")
+        return pulumi.get(self, "namespace_id")
 
-    @author_name.setter
-    def author_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "author_name", value)
+    @namespace_id.setter
+    def namespace_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "namespace_id", value)
 
     @property
-    @pulumi.getter(name="executeFilemode")
-    def execute_filemode(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
         """
-        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        The note associated to the user.
         """
-        return pulumi.get(self, "execute_filemode")
+        return pulumi.get(self, "note")
 
-    @execute_filemode.setter
-    def execute_filemode(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "execute_filemode", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="startBranch")
-    def start_branch(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the branch to start the new commit from.
+        The password of the user.
         """
-        return pulumi.get(self, "start_branch")
-
-    @start_branch.setter
-    def start_branch(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start_branch", value)
+        return pulumi.get(self, "password")
 
-
-@pulumi.input_type
-class _RepositoryFileState:
-    def __init__(__self__, *,
-                 author_email: Optional[pulumi.Input[str]] = None,
-                 author_name: Optional[pulumi.Input[str]] = None,
-                 blob_id: Optional[pulumi.Input[str]] = None,
-                 branch: Optional[pulumi.Input[str]] = None,
-                 commit_id: Optional[pulumi.Input[str]] = None,
-                 commit_message: Optional[pulumi.Input[str]] = None,
-                 content: Optional[pulumi.Input[str]] = None,
-                 content_sha256: Optional[pulumi.Input[str]] = None,
-                 encoding: Optional[pulumi.Input[str]] = None,
-                 execute_filemode: Optional[pulumi.Input[bool]] = None,
-                 file_name: Optional[pulumi.Input[str]] = None,
-                 file_path: Optional[pulumi.Input[str]] = None,
-                 last_commit_id: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 ref: Optional[pulumi.Input[str]] = None,
-                 size: Optional[pulumi.Input[int]] = None,
-                 start_branch: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering RepositoryFile resources.
-        :param pulumi.Input[str] author_email: Email of the commit author.
-        :param pulumi.Input[str] author_name: Name of the commit author.
-        :param pulumi.Input[str] blob_id: The blob id.
-        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
-        :param pulumi.Input[str] commit_id: The commit id.
-        :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
-        :param pulumi.Input[str] content_sha256: File content sha256 digest.
-        :param pulumi.Input[str] encoding: The file content encoding.
-        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
-        :param pulumi.Input[str] file_name: The filename.
-        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/`.
-        :param pulumi.Input[str] last_commit_id: The last known commit id.
-        :param pulumi.Input[str] project: The name or ID of the project.
-        :param pulumi.Input[str] ref: The name of branch, tag or commit.
-        :param pulumi.Input[int] size: The file size.
-        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
-        """
-        if author_email is not None:
-            pulumi.set(__self__, "author_email", author_email)
-        if author_name is not None:
-            pulumi.set(__self__, "author_name", author_name)
-        if blob_id is not None:
-            pulumi.set(__self__, "blob_id", blob_id)
-        if branch is not None:
-            pulumi.set(__self__, "branch", branch)
-        if commit_id is not None:
-            pulumi.set(__self__, "commit_id", commit_id)
-        if commit_message is not None:
-            pulumi.set(__self__, "commit_message", commit_message)
-        if content is not None:
-            pulumi.set(__self__, "content", content)
-        if content_sha256 is not None:
-            pulumi.set(__self__, "content_sha256", content_sha256)
-        if encoding is not None:
-            pulumi.set(__self__, "encoding", encoding)
-        if execute_filemode is not None:
-            pulumi.set(__self__, "execute_filemode", execute_filemode)
-        if file_name is not None:
-            pulumi.set(__self__, "file_name", file_name)
-        if file_path is not None:
-            pulumi.set(__self__, "file_path", file_path)
-        if last_commit_id is not None:
-            pulumi.set(__self__, "last_commit_id", last_commit_id)
-        if project is not None:
-            pulumi.set(__self__, "project", project)
-        if ref is not None:
-            pulumi.set(__self__, "ref", ref)
-        if size is not None:
-            pulumi.set(__self__, "size", size)
-        if start_branch is not None:
-            pulumi.set(__self__, "start_branch", start_branch)
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
 
     @property
-    @pulumi.getter(name="authorEmail")
-    def author_email(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="projectsLimit")
+    def projects_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        Email of the commit author.
+        Integer, defaults to 0.  Number of projects user can create.
         """
-        return pulumi.get(self, "author_email")
+        return pulumi.get(self, "projects_limit")
 
-    @author_email.setter
-    def author_email(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "author_email", value)
+    @projects_limit.setter
+    def projects_limit(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "projects_limit", value)
 
     @property
-    @pulumi.getter(name="authorName")
-    def author_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="resetPassword")
+    def reset_password(self) -> Optional[pulumi.Input[bool]]:
         """
-        Name of the commit author.
+        Boolean, defaults to false. Send user password reset link.
         """
-        return pulumi.get(self, "author_name")
+        return pulumi.get(self, "reset_password")
 
-    @author_name.setter
-    def author_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "author_name", value)
+    @reset_password.setter
+    def reset_password(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "reset_password", value)
 
     @property
-    @pulumi.getter(name="blobId")
-    def blob_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="skipConfirmation")
+    def skip_confirmation(self) -> Optional[pulumi.Input[bool]]:
         """
-        The blob id.
+        Boolean, defaults to true. Whether to skip confirmation.
         """
-        return pulumi.get(self, "blob_id")
+        return pulumi.get(self, "skip_confirmation")
 
-    @blob_id.setter
-    def blob_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "blob_id", value)
+    @skip_confirmation.setter
+    def skip_confirmation(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_confirmation", value)
 
     @property
     @pulumi.getter
-    def branch(self) -> Optional[pulumi.Input[str]]:
+    def state(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the branch to which to commit to.
+        String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
         """
-        return pulumi.get(self, "branch")
+        return pulumi.get(self, "state")
+
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
 
-    @branch.setter
-    def branch(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "branch", value)
+
+@pulumi.input_type
+class _UserState:
+    def __init__(__self__, *,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 is_admin: Optional[pulumi.Input[bool]] = None,
+                 is_external: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 namespace_id: Optional[pulumi.Input[int]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 projects_limit: Optional[pulumi.Input[int]] = None,
+                 reset_password: Optional[pulumi.Input[bool]] = None,
+                 skip_confirmation: Optional[pulumi.Input[bool]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering User resources.
+        :param pulumi.Input[bool] can_create_group: Boolean, defaults to false. Whether to allow the user to create groups.
+        :param pulumi.Input[str] email: The e-mail address of the user.
+        :param pulumi.Input[bool] is_admin: Boolean, defaults to false.  Whether to enable administrative privileges
+        :param pulumi.Input[bool] is_external: Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
+        :param pulumi.Input[str] name: The name of the user.
+        :param pulumi.Input[int] namespace_id: The ID of the user's namespace. Available since GitLab 14.10.
+        :param pulumi.Input[str] note: The note associated to the user.
+        :param pulumi.Input[str] password: The password of the user.
+        :param pulumi.Input[int] projects_limit: Integer, defaults to 0.  Number of projects user can create.
+        :param pulumi.Input[bool] reset_password: Boolean, defaults to false. Send user password reset link.
+        :param pulumi.Input[bool] skip_confirmation: Boolean, defaults to true. Whether to skip confirmation.
+        :param pulumi.Input[str] state: String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
+        :param pulumi.Input[str] username: The username of the user.
+        """
+        if can_create_group is not None:
+            pulumi.set(__self__, "can_create_group", can_create_group)
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+        if is_admin is not None:
+            pulumi.set(__self__, "is_admin", is_admin)
+        if is_external is not None:
+            pulumi.set(__self__, "is_external", is_external)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if namespace_id is not None:
+            pulumi.set(__self__, "namespace_id", namespace_id)
+        if note is not None:
+            pulumi.set(__self__, "note", note)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if projects_limit is not None:
+            pulumi.set(__self__, "projects_limit", projects_limit)
+        if reset_password is not None:
+            pulumi.set(__self__, "reset_password", reset_password)
+        if skip_confirmation is not None:
+            pulumi.set(__self__, "skip_confirmation", skip_confirmation)
+        if state is not None:
+            pulumi.set(__self__, "state", state)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter(name="commitId")
-    def commit_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> Optional[pulumi.Input[bool]]:
         """
-        The commit id.
+        Boolean, defaults to false. Whether to allow the user to create groups.
         """
-        return pulumi.get(self, "commit_id")
+        return pulumi.get(self, "can_create_group")
 
-    @commit_id.setter
-    def commit_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "commit_id", value)
+    @can_create_group.setter
+    def can_create_group(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "can_create_group", value)
 
     @property
-    @pulumi.getter(name="commitMessage")
-    def commit_message(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def email(self) -> Optional[pulumi.Input[str]]:
         """
-        Commit message.
+        The e-mail address of the user.
         """
-        return pulumi.get(self, "commit_message")
+        return pulumi.get(self, "email")
 
-    @commit_message.setter
-    def commit_message(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "commit_message", value)
+    @email.setter
+    def email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "email", value)
 
     @property
-    @pulumi.getter
-    def content(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="isAdmin")
+    def is_admin(self) -> Optional[pulumi.Input[bool]]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        Boolean, defaults to false.  Whether to enable administrative privileges
         """
-        return pulumi.get(self, "content")
+        return pulumi.get(self, "is_admin")
 
-    @content.setter
-    def content(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "content", value)
+    @is_admin.setter
+    def is_admin(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "is_admin", value)
 
     @property
-    @pulumi.getter(name="contentSha256")
-    def content_sha256(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="isExternal")
+    def is_external(self) -> Optional[pulumi.Input[bool]]:
         """
-        File content sha256 digest.
+        Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
         """
-        return pulumi.get(self, "content_sha256")
+        return pulumi.get(self, "is_external")
 
-    @content_sha256.setter
-    def content_sha256(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "content_sha256", value)
+    @is_external.setter
+    def is_external(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "is_external", value)
 
     @property
     @pulumi.getter
-    def encoding(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The file content encoding.
+        The name of the user.
         """
-        return pulumi.get(self, "encoding")
+        return pulumi.get(self, "name")
 
-    @encoding.setter
-    def encoding(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "encoding", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="executeFilemode")
-    def execute_filemode(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="namespaceId")
+    def namespace_id(self) -> Optional[pulumi.Input[int]]:
         """
-        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        The ID of the user's namespace. Available since GitLab 14.10.
         """
-        return pulumi.get(self, "execute_filemode")
+        return pulumi.get(self, "namespace_id")
 
-    @execute_filemode.setter
-    def execute_filemode(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "execute_filemode", value)
+    @namespace_id.setter
+    def namespace_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "namespace_id", value)
 
     @property
-    @pulumi.getter(name="fileName")
-    def file_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def note(self) -> Optional[pulumi.Input[str]]:
         """
-        The filename.
+        The note associated to the user.
         """
-        return pulumi.get(self, "file_name")
+        return pulumi.get(self, "note")
 
-    @file_name.setter
-    def file_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "file_name", value)
+    @note.setter
+    def note(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "note", value)
 
     @property
-    @pulumi.getter(name="filePath")
-    def file_path(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The full path of the file. It must be relative to the root of the project without a leading slash `/`.
+        The password of the user.
         """
-        return pulumi.get(self, "file_path")
+        return pulumi.get(self, "password")
 
-    @file_path.setter
-    def file_path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "file_path", value)
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
 
     @property
-    @pulumi.getter(name="lastCommitId")
-    def last_commit_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="projectsLimit")
+    def projects_limit(self) -> Optional[pulumi.Input[int]]:
         """
-        The last known commit id.
+        Integer, defaults to 0.  Number of projects user can create.
         """
-        return pulumi.get(self, "last_commit_id")
+        return pulumi.get(self, "projects_limit")
 
-    @last_commit_id.setter
-    def last_commit_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_commit_id", value)
+    @projects_limit.setter
+    def projects_limit(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "projects_limit", value)
 
     @property
-    @pulumi.getter
-    def project(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="resetPassword")
+    def reset_password(self) -> Optional[pulumi.Input[bool]]:
         """
-        The name or ID of the project.
+        Boolean, defaults to false. Send user password reset link.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "reset_password")
 
-    @project.setter
-    def project(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "project", value)
+    @reset_password.setter
+    def reset_password(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "reset_password", value)
 
     @property
-    @pulumi.getter
-    def ref(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="skipConfirmation")
+    def skip_confirmation(self) -> Optional[pulumi.Input[bool]]:
         """
-        The name of branch, tag or commit.
+        Boolean, defaults to true. Whether to skip confirmation.
         """
-        return pulumi.get(self, "ref")
+        return pulumi.get(self, "skip_confirmation")
 
-    @ref.setter
-    def ref(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "ref", value)
+    @skip_confirmation.setter
+    def skip_confirmation(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "skip_confirmation", value)
 
     @property
     @pulumi.getter
-    def size(self) -> Optional[pulumi.Input[int]]:
+    def state(self) -> Optional[pulumi.Input[str]]:
         """
-        The file size.
+        String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
         """
-        return pulumi.get(self, "size")
+        return pulumi.get(self, "state")
 
-    @size.setter
-    def size(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "size", value)
+    @state.setter
+    def state(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "state", value)
 
     @property
-    @pulumi.getter(name="startBranch")
-    def start_branch(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the branch to start the new commit from.
+        The username of the user.
         """
-        return pulumi.get(self, "start_branch")
+        return pulumi.get(self, "username")
 
-    @start_branch.setter
-    def start_branch(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "start_branch", value)
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
 
 
-class RepositoryFile(pulumi.CustomResource):
+class User(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 author_email: Optional[pulumi.Input[str]] = None,
-                 author_name: Optional[pulumi.Input[str]] = None,
-                 branch: Optional[pulumi.Input[str]] = None,
-                 commit_message: Optional[pulumi.Input[str]] = None,
-                 content: Optional[pulumi.Input[str]] = None,
-                 execute_filemode: Optional[pulumi.Input[bool]] = None,
-                 file_path: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 start_branch: Optional[pulumi.Input[str]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 is_admin: Optional[pulumi.Input[bool]] = None,
+                 is_external: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 namespace_id: Optional[pulumi.Input[int]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 projects_limit: Optional[pulumi.Input[int]] = None,
+                 reset_password: Optional[pulumi.Input[bool]] = None,
+                 skip_confirmation: Optional[pulumi.Input[bool]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        The `User` resource allows to manage the lifecycle of a user.
+
+        > the provider needs to be configured with admin-level access for this resource to work.
+
+        > You must specify either password or reset_password.
+
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html)
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        example = gitlab.User("example",
+            can_create_group=False,
+            email="gitlab@user.create",
+            is_admin=True,
+            is_external=True,
+            password="superPassword",
+            projects_limit=4,
+            reset_password=False,
+            username="example")
+        ```
+
         ## Import
 
-        A Repository File can be imported using an id made up of `<project-id>:<branch-name>:<file-path>`, e.g.
+        ```sh
+         $ pulumi import gitlab:index/user:User You can import a user to terraform state using `<resource> <id>`.
+        ```
+
+         The `id` must be an integer for the id of the user you want to import, for example
 
         ```sh
-         $ pulumi import gitlab:index/repositoryFile:RepositoryFile this 1:main:foo/bar.txt
+         $ pulumi import gitlab:index/user:User example 42
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] author_email: Email of the commit author.
-        :param pulumi.Input[str] author_name: Name of the commit author.
-        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
-        :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
-        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
-        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/`.
-        :param pulumi.Input[str] project: The name or ID of the project.
-        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
+        :param pulumi.Input[bool] can_create_group: Boolean, defaults to false. Whether to allow the user to create groups.
+        :param pulumi.Input[str] email: The e-mail address of the user.
+        :param pulumi.Input[bool] is_admin: Boolean, defaults to false.  Whether to enable administrative privileges
+        :param pulumi.Input[bool] is_external: Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
+        :param pulumi.Input[str] name: The name of the user.
+        :param pulumi.Input[int] namespace_id: The ID of the user's namespace. Available since GitLab 14.10.
+        :param pulumi.Input[str] note: The note associated to the user.
+        :param pulumi.Input[str] password: The password of the user.
+        :param pulumi.Input[int] projects_limit: Integer, defaults to 0.  Number of projects user can create.
+        :param pulumi.Input[bool] reset_password: Boolean, defaults to false. Send user password reset link.
+        :param pulumi.Input[bool] skip_confirmation: Boolean, defaults to true. Whether to skip confirmation.
+        :param pulumi.Input[str] state: String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
+        :param pulumi.Input[str] username: The username of the user.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: RepositoryFileArgs,
+                 args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        The `User` resource allows to manage the lifecycle of a user.
+
+        > the provider needs to be configured with admin-level access for this resource to work.
+
+        > You must specify either password or reset_password.
+
+        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/users.html)
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        example = gitlab.User("example",
+            can_create_group=False,
+            email="gitlab@user.create",
+            is_admin=True,
+            is_external=True,
+            password="superPassword",
+            projects_limit=4,
+            reset_password=False,
+            username="example")
+        ```
+
         ## Import
 
-        A Repository File can be imported using an id made up of `<project-id>:<branch-name>:<file-path>`, e.g.
+        ```sh
+         $ pulumi import gitlab:index/user:User You can import a user to terraform state using `<resource> <id>`.
+        ```
+
+         The `id` must be an integer for the id of the user you want to import, for example
 
         ```sh
-         $ pulumi import gitlab:index/repositoryFile:RepositoryFile this 1:main:foo/bar.txt
+         $ pulumi import gitlab:index/user:User example 42
         ```
 
         :param str resource_name: The name of the resource.
-        :param RepositoryFileArgs args: The arguments to use to populate this resource's properties.
+        :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(RepositoryFileArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(UserArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 author_email: Optional[pulumi.Input[str]] = None,
-                 author_name: Optional[pulumi.Input[str]] = None,
-                 branch: Optional[pulumi.Input[str]] = None,
-                 commit_message: Optional[pulumi.Input[str]] = None,
-                 content: Optional[pulumi.Input[str]] = None,
-                 execute_filemode: Optional[pulumi.Input[bool]] = None,
-                 file_path: Optional[pulumi.Input[str]] = None,
-                 project: Optional[pulumi.Input[str]] = None,
-                 start_branch: Optional[pulumi.Input[str]] = None,
+                 can_create_group: Optional[pulumi.Input[bool]] = None,
+                 email: Optional[pulumi.Input[str]] = None,
+                 is_admin: Optional[pulumi.Input[bool]] = None,
+                 is_external: Optional[pulumi.Input[bool]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 namespace_id: Optional[pulumi.Input[int]] = None,
+                 note: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 projects_limit: Optional[pulumi.Input[int]] = None,
+                 reset_password: Optional[pulumi.Input[bool]] = None,
+                 skip_confirmation: Optional[pulumi.Input[bool]] = None,
+                 state: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = RepositoryFileArgs.__new__(RepositoryFileArgs)
+            __props__ = UserArgs.__new__(UserArgs)
 
-            __props__.__dict__["author_email"] = author_email
-            __props__.__dict__["author_name"] = author_name
-            if branch is None and not opts.urn:
-                raise TypeError("Missing required property 'branch'")
-            __props__.__dict__["branch"] = branch
-            if commit_message is None and not opts.urn:
-                raise TypeError("Missing required property 'commit_message'")
-            __props__.__dict__["commit_message"] = commit_message
-            if content is None and not opts.urn:
-                raise TypeError("Missing required property 'content'")
-            __props__.__dict__["content"] = content
-            __props__.__dict__["execute_filemode"] = execute_filemode
-            if file_path is None and not opts.urn:
-                raise TypeError("Missing required property 'file_path'")
-            __props__.__dict__["file_path"] = file_path
-            if project is None and not opts.urn:
-                raise TypeError("Missing required property 'project'")
-            __props__.__dict__["project"] = project
-            __props__.__dict__["start_branch"] = start_branch
-            __props__.__dict__["blob_id"] = None
-            __props__.__dict__["commit_id"] = None
-            __props__.__dict__["content_sha256"] = None
-            __props__.__dict__["encoding"] = None
-            __props__.__dict__["file_name"] = None
-            __props__.__dict__["last_commit_id"] = None
-            __props__.__dict__["ref"] = None
-            __props__.__dict__["size"] = None
-        super(RepositoryFile, __self__).__init__(
-            'gitlab:index/repositoryFile:RepositoryFile',
+            __props__.__dict__["can_create_group"] = can_create_group
+            if email is None and not opts.urn:
+                raise TypeError("Missing required property 'email'")
+            __props__.__dict__["email"] = email
+            __props__.__dict__["is_admin"] = is_admin
+            __props__.__dict__["is_external"] = is_external
+            __props__.__dict__["name"] = name
+            __props__.__dict__["namespace_id"] = namespace_id
+            __props__.__dict__["note"] = note
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
+            __props__.__dict__["projects_limit"] = projects_limit
+            __props__.__dict__["reset_password"] = reset_password
+            __props__.__dict__["skip_confirmation"] = skip_confirmation
+            __props__.__dict__["state"] = state
+            if username is None and not opts.urn:
+                raise TypeError("Missing required property 'username'")
+            __props__.__dict__["username"] = username
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(User, __self__).__init__(
+            'gitlab:index/user:User',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            author_email: Optional[pulumi.Input[str]] = None,
-            author_name: Optional[pulumi.Input[str]] = None,
-            blob_id: Optional[pulumi.Input[str]] = None,
-            branch: Optional[pulumi.Input[str]] = None,
-            commit_id: Optional[pulumi.Input[str]] = None,
-            commit_message: Optional[pulumi.Input[str]] = None,
-            content: Optional[pulumi.Input[str]] = None,
-            content_sha256: Optional[pulumi.Input[str]] = None,
-            encoding: Optional[pulumi.Input[str]] = None,
-            execute_filemode: Optional[pulumi.Input[bool]] = None,
-            file_name: Optional[pulumi.Input[str]] = None,
-            file_path: Optional[pulumi.Input[str]] = None,
-            last_commit_id: Optional[pulumi.Input[str]] = None,
-            project: Optional[pulumi.Input[str]] = None,
-            ref: Optional[pulumi.Input[str]] = None,
-            size: Optional[pulumi.Input[int]] = None,
-            start_branch: Optional[pulumi.Input[str]] = None) -> 'RepositoryFile':
+            can_create_group: Optional[pulumi.Input[bool]] = None,
+            email: Optional[pulumi.Input[str]] = None,
+            is_admin: Optional[pulumi.Input[bool]] = None,
+            is_external: Optional[pulumi.Input[bool]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            namespace_id: Optional[pulumi.Input[int]] = None,
+            note: Optional[pulumi.Input[str]] = None,
+            password: Optional[pulumi.Input[str]] = None,
+            projects_limit: Optional[pulumi.Input[int]] = None,
+            reset_password: Optional[pulumi.Input[bool]] = None,
+            skip_confirmation: Optional[pulumi.Input[bool]] = None,
+            state: Optional[pulumi.Input[str]] = None,
+            username: Optional[pulumi.Input[str]] = None) -> 'User':
         """
-        Get an existing RepositoryFile resource's state with the given name, id, and optional extra
+        Get an existing User resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] author_email: Email of the commit author.
-        :param pulumi.Input[str] author_name: Name of the commit author.
-        :param pulumi.Input[str] blob_id: The blob id.
-        :param pulumi.Input[str] branch: Name of the branch to which to commit to.
-        :param pulumi.Input[str] commit_id: The commit id.
-        :param pulumi.Input[str] commit_message: Commit message.
-        :param pulumi.Input[str] content: File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
-        :param pulumi.Input[str] content_sha256: File content sha256 digest.
-        :param pulumi.Input[str] encoding: The file content encoding.
-        :param pulumi.Input[bool] execute_filemode: Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
-        :param pulumi.Input[str] file_name: The filename.
-        :param pulumi.Input[str] file_path: The full path of the file. It must be relative to the root of the project without a leading slash `/`.
-        :param pulumi.Input[str] last_commit_id: The last known commit id.
-        :param pulumi.Input[str] project: The name or ID of the project.
-        :param pulumi.Input[str] ref: The name of branch, tag or commit.
-        :param pulumi.Input[int] size: The file size.
-        :param pulumi.Input[str] start_branch: Name of the branch to start the new commit from.
+        :param pulumi.Input[bool] can_create_group: Boolean, defaults to false. Whether to allow the user to create groups.
+        :param pulumi.Input[str] email: The e-mail address of the user.
+        :param pulumi.Input[bool] is_admin: Boolean, defaults to false.  Whether to enable administrative privileges
+        :param pulumi.Input[bool] is_external: Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
+        :param pulumi.Input[str] name: The name of the user.
+        :param pulumi.Input[int] namespace_id: The ID of the user's namespace. Available since GitLab 14.10.
+        :param pulumi.Input[str] note: The note associated to the user.
+        :param pulumi.Input[str] password: The password of the user.
+        :param pulumi.Input[int] projects_limit: Integer, defaults to 0.  Number of projects user can create.
+        :param pulumi.Input[bool] reset_password: Boolean, defaults to false. Send user password reset link.
+        :param pulumi.Input[bool] skip_confirmation: Boolean, defaults to true. Whether to skip confirmation.
+        :param pulumi.Input[str] state: String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
+        :param pulumi.Input[str] username: The username of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _RepositoryFileState.__new__(_RepositoryFileState)
-
-        __props__.__dict__["author_email"] = author_email
-        __props__.__dict__["author_name"] = author_name
-        __props__.__dict__["blob_id"] = blob_id
-        __props__.__dict__["branch"] = branch
-        __props__.__dict__["commit_id"] = commit_id
-        __props__.__dict__["commit_message"] = commit_message
-        __props__.__dict__["content"] = content
-        __props__.__dict__["content_sha256"] = content_sha256
-        __props__.__dict__["encoding"] = encoding
-        __props__.__dict__["execute_filemode"] = execute_filemode
-        __props__.__dict__["file_name"] = file_name
-        __props__.__dict__["file_path"] = file_path
-        __props__.__dict__["last_commit_id"] = last_commit_id
-        __props__.__dict__["project"] = project
-        __props__.__dict__["ref"] = ref
-        __props__.__dict__["size"] = size
-        __props__.__dict__["start_branch"] = start_branch
-        return RepositoryFile(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="authorEmail")
-    def author_email(self) -> pulumi.Output[Optional[str]]:
-        """
-        Email of the commit author.
-        """
-        return pulumi.get(self, "author_email")
+        __props__ = _UserState.__new__(_UserState)
 
-    @property
-    @pulumi.getter(name="authorName")
-    def author_name(self) -> pulumi.Output[Optional[str]]:
-        """
-        Name of the commit author.
-        """
-        return pulumi.get(self, "author_name")
+        __props__.__dict__["can_create_group"] = can_create_group
+        __props__.__dict__["email"] = email
+        __props__.__dict__["is_admin"] = is_admin
+        __props__.__dict__["is_external"] = is_external
+        __props__.__dict__["name"] = name
+        __props__.__dict__["namespace_id"] = namespace_id
+        __props__.__dict__["note"] = note
+        __props__.__dict__["password"] = password
+        __props__.__dict__["projects_limit"] = projects_limit
+        __props__.__dict__["reset_password"] = reset_password
+        __props__.__dict__["skip_confirmation"] = skip_confirmation
+        __props__.__dict__["state"] = state
+        __props__.__dict__["username"] = username
+        return User(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter(name="blobId")
-    def blob_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="canCreateGroup")
+    def can_create_group(self) -> pulumi.Output[Optional[bool]]:
         """
-        The blob id.
+        Boolean, defaults to false. Whether to allow the user to create groups.
         """
-        return pulumi.get(self, "blob_id")
+        return pulumi.get(self, "can_create_group")
 
     @property
     @pulumi.getter
-    def branch(self) -> pulumi.Output[str]:
+    def email(self) -> pulumi.Output[str]:
         """
-        Name of the branch to which to commit to.
+        The e-mail address of the user.
         """
-        return pulumi.get(self, "branch")
+        return pulumi.get(self, "email")
 
     @property
-    @pulumi.getter(name="commitId")
-    def commit_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="isAdmin")
+    def is_admin(self) -> pulumi.Output[Optional[bool]]:
         """
-        The commit id.
+        Boolean, defaults to false.  Whether to enable administrative privileges
         """
-        return pulumi.get(self, "commit_id")
+        return pulumi.get(self, "is_admin")
 
     @property
-    @pulumi.getter(name="commitMessage")
-    def commit_message(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="isExternal")
+    def is_external(self) -> pulumi.Output[Optional[bool]]:
         """
-        Commit message.
+        Boolean, defaults to false. Whether a user has access only to some internal or private projects. External users can only access projects to which they are explicitly granted access.
         """
-        return pulumi.get(self, "commit_message")
+        return pulumi.get(self, "is_external")
 
     @property
     @pulumi.getter
-    def content(self) -> pulumi.Output[str]:
+    def name(self) -> pulumi.Output[str]:
         """
-        File content. If the content is not yet base64 encoded, it will be encoded automatically. No other encoding is currently supported, because of a [GitLab API bug](https://gitlab.com/gitlab-org/gitlab/-/issues/342430).
+        The name of the user.
         """
-        return pulumi.get(self, "content")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="contentSha256")
-    def content_sha256(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="namespaceId")
+    def namespace_id(self) -> pulumi.Output[int]:
         """
-        File content sha256 digest.
+        The ID of the user's namespace. Available since GitLab 14.10.
         """
-        return pulumi.get(self, "content_sha256")
+        return pulumi.get(self, "namespace_id")
 
     @property
     @pulumi.getter
-    def encoding(self) -> pulumi.Output[str]:
-        """
-        The file content encoding.
-        """
-        return pulumi.get(self, "encoding")
-
-    @property
-    @pulumi.getter(name="executeFilemode")
-    def execute_filemode(self) -> pulumi.Output[Optional[bool]]:
+    def note(self) -> pulumi.Output[Optional[str]]:
         """
-        Enables or disables the execute flag on the file. **Note**: requires GitLab 14.10 or newer.
+        The note associated to the user.
         """
-        return pulumi.get(self, "execute_filemode")
+        return pulumi.get(self, "note")
 
     @property
-    @pulumi.getter(name="fileName")
-    def file_name(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def password(self) -> pulumi.Output[Optional[str]]:
         """
-        The filename.
+        The password of the user.
         """
-        return pulumi.get(self, "file_name")
+        return pulumi.get(self, "password")
 
     @property
-    @pulumi.getter(name="filePath")
-    def file_path(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="projectsLimit")
+    def projects_limit(self) -> pulumi.Output[Optional[int]]:
         """
-        The full path of the file. It must be relative to the root of the project without a leading slash `/`.
+        Integer, defaults to 0.  Number of projects user can create.
         """
-        return pulumi.get(self, "file_path")
+        return pulumi.get(self, "projects_limit")
 
     @property
-    @pulumi.getter(name="lastCommitId")
-    def last_commit_id(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="resetPassword")
+    def reset_password(self) -> pulumi.Output[Optional[bool]]:
         """
-        The last known commit id.
+        Boolean, defaults to false. Send user password reset link.
         """
-        return pulumi.get(self, "last_commit_id")
+        return pulumi.get(self, "reset_password")
 
     @property
-    @pulumi.getter
-    def project(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="skipConfirmation")
+    def skip_confirmation(self) -> pulumi.Output[Optional[bool]]:
         """
-        The name or ID of the project.
+        Boolean, defaults to true. Whether to skip confirmation.
         """
-        return pulumi.get(self, "project")
+        return pulumi.get(self, "skip_confirmation")
 
     @property
     @pulumi.getter
-    def ref(self) -> pulumi.Output[str]:
+    def state(self) -> pulumi.Output[Optional[str]]:
         """
-        The name of branch, tag or commit.
+        String, defaults to 'active'. The state of the user account. Valid values are `active`, `deactivated`, `blocked`.
         """
-        return pulumi.get(self, "ref")
+        return pulumi.get(self, "state")
 
     @property
     @pulumi.getter
-    def size(self) -> pulumi.Output[int]:
-        """
-        The file size.
-        """
-        return pulumi.get(self, "size")
-
-    @property
-    @pulumi.getter(name="startBranch")
-    def start_branch(self) -> pulumi.Output[Optional[str]]:
+    def username(self) -> pulumi.Output[str]:
         """
-        Name of the branch to start the new commit from.
+        The username of the user.
         """
-        return pulumi.get(self, "start_branch")
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/runner.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_github.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_microsoft_teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  pipeline_events: Optional[pulumi.Input[bool]] = None,
                  push_events: Optional[pulumi.Input[bool]] = None,
                  tag_push_events: Optional[pulumi.Input[bool]] = None,
                  wiki_page_events: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ServiceMicrosoftTeams resource.
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
-        :param pulumi.Input[str] webhook: The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        :param pulumi.Input[str] webhook: The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         :param pulumi.Input[str] branches_to_be_notified: Branches to send notifications for. Valid options are “all”, “default”, “protected”, and “default*and*protected”. The default value is “default”
         :param pulumi.Input[bool] confidential_issues_events: Enable notifications for confidential issue events
         :param pulumi.Input[bool] confidential_note_events: Enable notifications for confidential note events
         :param pulumi.Input[bool] issues_events: Enable notifications for issue events
         :param pulumi.Input[bool] merge_requests_events: Enable notifications for merge request events
         :param pulumi.Input[bool] note_events: Enable notifications for note events
         :param pulumi.Input[bool] notify_only_broken_pipelines: Send notifications for broken pipelines
@@ -80,15 +80,15 @@
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def webhook(self) -> pulumi.Input[str]:
         """
-        The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @webhook.setter
     def webhook(self, value: pulumi.Input[str]):
         pulumi.set(self, "webhook", value)
 
@@ -256,15 +256,15 @@
         :param pulumi.Input[bool] note_events: Enable notifications for note events
         :param pulumi.Input[bool] notify_only_broken_pipelines: Send notifications for broken pipelines
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[bool] push_events: Enable notifications for push events
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events
         :param pulumi.Input[str] updated_at: Update time.
-        :param pulumi.Input[str] webhook: The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        :param pulumi.Input[str] webhook: The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events
         """
         if active is not None:
             pulumi.set(__self__, "active", active)
         if branches_to_be_notified is not None:
             pulumi.set(__self__, "branches_to_be_notified", branches_to_be_notified)
         if confidential_issues_events is not None:
@@ -464,15 +464,15 @@
     def updated_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "updated_at", value)
 
     @property
     @pulumi.getter
     def webhook(self) -> Optional[pulumi.Input[str]]:
         """
-        The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @webhook.setter
     def webhook(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "webhook", value)
 
@@ -545,15 +545,15 @@
         :param pulumi.Input[bool] merge_requests_events: Enable notifications for merge request events
         :param pulumi.Input[bool] note_events: Enable notifications for note events
         :param pulumi.Input[bool] notify_only_broken_pipelines: Send notifications for broken pipelines
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[bool] push_events: Enable notifications for push events
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events
-        :param pulumi.Input[str] webhook: The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        :param pulumi.Input[str] webhook: The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceMicrosoftTeamsArgs,
@@ -686,15 +686,15 @@
         :param pulumi.Input[bool] note_events: Enable notifications for note events
         :param pulumi.Input[bool] notify_only_broken_pipelines: Send notifications for broken pipelines
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[bool] push_events: Enable notifications for push events
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events
         :param pulumi.Input[str] updated_at: Update time.
-        :param pulumi.Input[str] webhook: The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        :param pulumi.Input[str] webhook: The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceMicrosoftTeamsState.__new__(_ServiceMicrosoftTeamsState)
 
         __props__.__dict__["active"] = active
@@ -827,15 +827,15 @@
         """
         return pulumi.get(self, "updated_at")
 
     @property
     @pulumi.getter
     def webhook(self) -> pulumi.Output[str]:
         """
-        The Microsoft Teams webhook. For example, https://outlook.office.com/webhook/...
+        The Microsoft Teams webhook (Example, https://outlook.office.com/webhook/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @property
     @pulumi.getter(name="wikiPageEvents")
     def wiki_page_events(self) -> pulumi.Output[Optional[bool]]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/service_slack.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                  tag_push_events: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  wiki_page_channel: Optional[pulumi.Input[str]] = None,
                  wiki_page_events: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ServiceSlack resource.
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
-        :param pulumi.Input[str] webhook: Webhook URL (ex.: https://hooks.slack.com/services/...)
+        :param pulumi.Input[str] webhook: Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         :param pulumi.Input[str] branches_to_be_notified: Branches to send notifications for. Valid options are "all", "default", "protected", and "default*and*protected".
         :param pulumi.Input[str] confidential_issue_channel: The name of the channel to receive confidential issue events notifications.
         :param pulumi.Input[bool] confidential_issues_events: Enable notifications for confidential issues events.
         :param pulumi.Input[bool] confidential_note_events: Enable notifications for confidential note events.
         :param pulumi.Input[str] issue_channel: The name of the channel to receive issue events notifications.
         :param pulumi.Input[bool] issues_events: Enable notifications for issues events.
         :param pulumi.Input[str] merge_request_channel: The name of the channel to receive merge request events notifications.
@@ -123,15 +123,15 @@
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
     def webhook(self) -> pulumi.Input[str]:
         """
-        Webhook URL (ex.: https://hooks.slack.com/services/...)
+        Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @webhook.setter
     def webhook(self, value: pulumi.Input[str]):
         pulumi.set(self, "webhook", value)
 
@@ -434,15 +434,15 @@
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events.
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[str] push_channel: The name of the channel to receive push events notifications.
         :param pulumi.Input[bool] push_events: Enable notifications for push events.
         :param pulumi.Input[str] tag_push_channel: The name of the channel to receive tag push events notifications.
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events.
         :param pulumi.Input[str] username: Username to use.
-        :param pulumi.Input[str] webhook: Webhook URL (ex.: https://hooks.slack.com/services/...)
+        :param pulumi.Input[str] webhook: Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         :param pulumi.Input[str] wiki_page_channel: The name of the channel to receive wiki page events notifications.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events.
         """
         if branches_to_be_notified is not None:
             pulumi.set(__self__, "branches_to_be_notified", branches_to_be_notified)
         if confidential_issue_channel is not None:
             pulumi.set(__self__, "confidential_issue_channel", confidential_issue_channel)
@@ -746,15 +746,15 @@
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
     @property
     @pulumi.getter
     def webhook(self) -> Optional[pulumi.Input[str]]:
         """
-        Webhook URL (ex.: https://hooks.slack.com/services/...)
+        Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @webhook.setter
     def webhook(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "webhook", value)
 
@@ -860,15 +860,15 @@
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events.
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[str] push_channel: The name of the channel to receive push events notifications.
         :param pulumi.Input[bool] push_events: Enable notifications for push events.
         :param pulumi.Input[str] tag_push_channel: The name of the channel to receive tag push events notifications.
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events.
         :param pulumi.Input[str] username: Username to use.
-        :param pulumi.Input[str] webhook: Webhook URL (ex.: https://hooks.slack.com/services/...)
+        :param pulumi.Input[str] webhook: Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         :param pulumi.Input[str] wiki_page_channel: The name of the channel to receive wiki page events notifications.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -1040,15 +1040,15 @@
         :param pulumi.Input[bool] pipeline_events: Enable notifications for pipeline events.
         :param pulumi.Input[str] project: ID of the project you want to activate integration on.
         :param pulumi.Input[str] push_channel: The name of the channel to receive push events notifications.
         :param pulumi.Input[bool] push_events: Enable notifications for push events.
         :param pulumi.Input[str] tag_push_channel: The name of the channel to receive tag push events notifications.
         :param pulumi.Input[bool] tag_push_events: Enable notifications for tag push events.
         :param pulumi.Input[str] username: Username to use.
-        :param pulumi.Input[str] webhook: Webhook URL (ex.: https://hooks.slack.com/services/...)
+        :param pulumi.Input[str] webhook: Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         :param pulumi.Input[str] wiki_page_channel: The name of the channel to receive wiki page events notifications.
         :param pulumi.Input[bool] wiki_page_events: Enable notifications for wiki page events.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ServiceSlackState.__new__(_ServiceSlackState)
 
@@ -1246,15 +1246,15 @@
         """
         return pulumi.get(self, "username")
 
     @property
     @pulumi.getter
     def webhook(self) -> pulumi.Output[str]:
         """
-        Webhook URL (ex.: https://hooks.slack.com/services/...)
+        Webhook URL (Example, https://hooks.slack.com/services/...). This value cannot be imported.
         """
         return pulumi.get(self, "webhook")
 
     @property
     @pulumi.getter(name="wikiPageChannel")
     def wiki_page_channel(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/topic.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_gpg_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class UserGpgKeyArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a UserGpgKey resource.
         :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         pulumi.set(__self__, "key", key)
         if user_id is not None:
             pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter
@@ -37,15 +37,15 @@
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "user_id", value)
 
@@ -58,15 +58,15 @@
                  key_id: Optional[pulumi.Input[int]] = None,
                  user_id: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering UserGpgKey resources.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
         :param pulumi.Input[str] key: The armored GPG public key.
         :param pulumi.Input[int] key_id: The ID of the GPG key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if key_id is not None:
             pulumi.set(__self__, "key_id", key_id)
@@ -109,15 +109,15 @@
     def key_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "key_id", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "user_id", value)
 
@@ -169,15 +169,15 @@
         ```sh
          $ pulumi import gitlab:index/userGpgKey:UserGpgKey example_user 1
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: The armored GPG public key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserGpgKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -273,15 +273,15 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
         :param pulumi.Input[str] key: The armored GPG public key.
         :param pulumi.Input[int] key_id: The ID of the GPG key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        :param pulumi.Input[int] user_id: The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UserGpgKeyState.__new__(_UserGpgKeyState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["key"] = key
@@ -313,11 +313,11 @@
         """
         return pulumi.get(self, "key_id")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> pulumi.Output[Optional[int]]:
         """
-        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the speicifed user, and an admin token is required.
+        The ID of the user to add the GPG key to. If this field is omitted, this resource manages a GPG key for the current user. Otherwise, this resource manages a GPG key for the specified user, and an admin token is required.
         """
         return pulumi.get(self, "user_id")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab/user_ssh_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                  title: pulumi.Input[str],
                  user_id: pulumi.Input[int],
                  expires_at: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a UserSshKey resource.
         :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the ssh key to.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "title", title)
         pulumi.set(__self__, "user_id", user_id)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
@@ -55,15 +55,15 @@
     def title(self, value: pulumi.Input[str]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> pulumi.Input[int]:
         """
-        The ID of the user to add the ssh key to.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "user_id", value)
 
@@ -92,15 +92,15 @@
         """
         Input properties used for looking up and filtering UserSshKey resources.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
         :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
         :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         :param pulumi.Input[int] key_id: The ID of the ssh key.
         :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the ssh key to.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if expires_at is not None:
             pulumi.set(__self__, "expires_at", expires_at)
         if key is not None:
             pulumi.set(__self__, "key", key)
@@ -171,15 +171,15 @@
     def title(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "title", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[int]]:
         """
-        The ID of the user to add the ssh key to.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "user_id", value)
 
@@ -203,17 +203,17 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example_user = gitlab.get_user(username="example-user")
         example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
-            user_id=data["gitlab_user"]["id"],
+            user_id=example_user.id,
             title="example-key",
-            key="ssh-rsa AAAA...",
+            key="ssh-ed25519 AAAA...",
             expires_at="2016-01-21T00:00:00.000Z")
         ```
 
         ## Import
 
         You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
 
@@ -222,15 +222,15 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
         :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the ssh key to.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserSshKeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -243,17 +243,17 @@
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         example_user = gitlab.get_user(username="example-user")
         example_user_ssh_key = gitlab.UserSshKey("exampleUserSshKey",
-            user_id=data["gitlab_user"]["id"],
+            user_id=example_user.id,
             title="example-key",
-            key="ssh-rsa AAAA...",
+            key="ssh-ed25519 AAAA...",
             expires_at="2016-01-21T00:00:00.000Z")
         ```
 
         ## Import
 
         You can import a user ssh key using an id made up of `{user-id}:{key}`, e.g.
 
@@ -325,15 +325,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: The time when this key was created in GitLab.
         :param pulumi.Input[str] expires_at: The expiration date of the SSH key in ISO 8601 format (YYYY-MM-DDTHH:MM:SSZ)
         :param pulumi.Input[str] key: The ssh key. The SSH key `comment` (trailing part) is optional and ignored for diffing, because GitLab overrides it with the username and GitLab hostname.
         :param pulumi.Input[int] key_id: The ID of the ssh key.
         :param pulumi.Input[str] title: The title of the ssh key.
-        :param pulumi.Input[int] user_id: The ID of the user to add the ssh key to.
+        :param pulumi.Input[int] user_id: The ID or username of the user.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UserSshKeyState.__new__(_UserSshKeyState)
 
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["expires_at"] = expires_at
@@ -383,11 +383,11 @@
         """
         return pulumi.get(self, "title")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> pulumi.Output[int]:
         """
-        The ID of the user to add the ssh key to.
+        The ID or username of the user.
         """
         return pulumi.get(self, "user_id")
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pulumi-gitlab
-Version: 4.9.0a1666628674
+Version: 5.1.0a1684272302
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-gitlab/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-gitlab/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fgitlab.svg)](https://www.npmjs.com/package/@pulumi/gitlab)
 [![Python version](https://badge.fury.io/py/pulumi-gitlab.svg)](https://pypi.org/project/pulumi-gitlab)
 [![NuGet version](https://badge.fury.io/nu/pulumi.gitlab.svg)](https://badge.fury.io/nu/pulumi.gitlab)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v4/go)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-gitlab/sdk/v4/go)](https://pkg.go.dev/github.com/pulumi/pulumi-gitlab/sdk/v5/go)
 [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-gitlab/blob/master/LICENSE)
 
 # GitLab provider
 
 The GitLab resource provider for Pulumi lets you use GitLab resources in your cloud programs.  To use
 this package, please [install the Pulumi CLI first](https://pulumi.io/).
 
@@ -42,15 +43,15 @@
 
     $ pip install pulumi_gitlab
 
 ### Go
 
 To use from Go, use `go get` to grab the latest version of the library
 
-    $ go get github.com/pulumi/pulumi-gitlab/sdk/v4
+    $ go get github.com/pulumi/pulumi-gitlab/sdk/v5
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
     $ dotnet add package Pulumi.Gitlab
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-5.1.0a1684272302/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 README.md
 setup.py
 pulumi_gitlab/__init__.py
 pulumi_gitlab/_inputs.py
 pulumi_gitlab/_utilities.py
+pulumi_gitlab/application.py
 pulumi_gitlab/application_settings.py
 pulumi_gitlab/branch.py
 pulumi_gitlab/branch_protection.py
 pulumi_gitlab/cluster_agent.py
 pulumi_gitlab/cluster_agent_token.py
 pulumi_gitlab/deploy_key.py
 pulumi_gitlab/deploy_key_enable.py
 pulumi_gitlab/deploy_token.py
+pulumi_gitlab/get_application.py
 pulumi_gitlab/get_branch.py
 pulumi_gitlab/get_cluster_agent.py
 pulumi_gitlab/get_cluster_agents.py
 pulumi_gitlab/get_current_user.py
 pulumi_gitlab/get_group.py
 pulumi_gitlab/get_group_hook.py
 pulumi_gitlab/get_group_hooks.py
 pulumi_gitlab/get_group_membership.py
+pulumi_gitlab/get_group_subgroups.py
 pulumi_gitlab/get_group_variable.py
 pulumi_gitlab/get_group_variables.py
+pulumi_gitlab/get_groups.py
 pulumi_gitlab/get_instance_deploy_keys.py
 pulumi_gitlab/get_instance_variable.py
 pulumi_gitlab/get_instance_variables.py
+pulumi_gitlab/get_metadata.py
 pulumi_gitlab/get_project.py
+pulumi_gitlab/get_project_branches.py
 pulumi_gitlab/get_project_hook.py
 pulumi_gitlab/get_project_hooks.py
 pulumi_gitlab/get_project_issue.py
 pulumi_gitlab/get_project_issues.py
 pulumi_gitlab/get_project_membership.py
 pulumi_gitlab/get_project_milestone.py
 pulumi_gitlab/get_project_milestones.py
@@ -40,14 +46,15 @@
 pulumi_gitlab/get_project_variables.py
 pulumi_gitlab/get_projects.py
 pulumi_gitlab/get_release_link.py
 pulumi_gitlab/get_release_links.py
 pulumi_gitlab/get_repository_file.py
 pulumi_gitlab/get_repository_tree.py
 pulumi_gitlab/get_user.py
+pulumi_gitlab/get_user_sshkeys.py
 pulumi_gitlab/get_users.py
 pulumi_gitlab/group.py
 pulumi_gitlab/group_access_token.py
 pulumi_gitlab/group_badge.py
 pulumi_gitlab/group_cluster.py
 pulumi_gitlab/group_custom_attribute.py
 pulumi_gitlab/group_hook.py
@@ -59,14 +66,15 @@
 pulumi_gitlab/group_share_group.py
 pulumi_gitlab/group_variable.py
 pulumi_gitlab/instance_cluster.py
 pulumi_gitlab/instance_variable.py
 pulumi_gitlab/label.py
 pulumi_gitlab/managed_license.py
 pulumi_gitlab/outputs.py
+pulumi_gitlab/pages_domain.py
 pulumi_gitlab/personal_access_token.py
 pulumi_gitlab/pipeline_schedule.py
 pulumi_gitlab/pipeline_schedule_variable.py
 pulumi_gitlab/pipeline_trigger.py
 pulumi_gitlab/project.py
 pulumi_gitlab/project_access_token.py
 pulumi_gitlab/project_approval_rule.py
@@ -89,14 +97,16 @@
 pulumi_gitlab/project_variable.py
 pulumi_gitlab/provider.py
 pulumi_gitlab/pulumi-plugin.json
 pulumi_gitlab/py.typed
 pulumi_gitlab/release_link.py
 pulumi_gitlab/repository_file.py
 pulumi_gitlab/runner.py
+pulumi_gitlab/service_custom_issue_tracker.py
+pulumi_gitlab/service_emails_on_push.py
 pulumi_gitlab/service_external_wiki.py
 pulumi_gitlab/service_github.py
 pulumi_gitlab/service_jira.py
 pulumi_gitlab/service_microsoft_teams.py
 pulumi_gitlab/service_pipelines_email.py
 pulumi_gitlab/service_slack.py
 pulumi_gitlab/system_hook.py
```

### Comparing `pulumi_gitlab-4.9.0a1666628674/setup.py` & `pulumi_gitlab-5.1.0a1684272302/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.9.0a1666628674"
-PLUGIN_VERSION = "4.9.0-alpha.1666628674+a29b05ea"
+VERSION = "5.1.0a1684272302"
+PLUGIN_VERSION = "5.1.0-alpha.1684272302+de7c087d"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'gitlab', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "gitlab Pulumi Package - Development Version"
 
 
 setup(name='pulumi_gitlab',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing GitLab resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

