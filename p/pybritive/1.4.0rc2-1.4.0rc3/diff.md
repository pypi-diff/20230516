# Comparing `tmp/pybritive-1.4.0rc2.tar.gz` & `tmp/pybritive-1.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybritive-1.4.0rc2.tar", last modified: Tue May  9 14:54:25 2023, max compression
+gzip compressed data, was "pybritive-1.4.0rc3.tar", last modified: Tue May 16 13:10:55 2023, max compression
```

## Comparing `pybritive-1.4.0rc2.tar` & `pybritive-1.4.0rc3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.295921 pybritive-1.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 14:54:25.295921 pybritive-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 14:54:25.299921 pybritive-1.4.0rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.279920 pybritive-1.4.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.283920 pybritive-1.4.0rc2/src/pybritive/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/britive_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.283920 pybritive-1.4.0rc2/src/pybritive/choices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/choices/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/cli_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.287921 pybritive-1.4.0rc2/src/pybritive/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/commands/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.287921 pybritive-1.4.0rc2/src/pybritive/completers/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/api_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/bash_gte_42.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/powershell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/completers/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.291921 pybritive-1.4.0rc2/src/pybritive/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/api_method_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/aws_credential_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/build_britive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/cloud_credential_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/profile_argument_dectorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/helpers/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.295921 pybritive-1.4.0rc2/src/pybritive/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/aws_console_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/aws_credentials_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/blocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/britive_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/checked_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/configure_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/configure_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/configure_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/configure_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/federation_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/force_renew.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/gcloud_key_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/justification.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/maxpolltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/output_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/passphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/silent.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/ssh_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/ssh_key_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/ssh_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/ssh_push_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/ssh_username.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/src/pybritive/options/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.283920 pybritive-1.4.0rc2/src/pybritive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 14:54:25.000000 pybritive-1.4.0rc2/src/pybritive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:54:25.295921 pybritive-1.4.0rc2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0100_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0200_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0300_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0400_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0450_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0500_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0600_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0700_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0800_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0850_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_0900_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 14:54:10.000000 pybritive-1.4.0rc2/tests/test_1000_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 13:10:55.253538 pybritive-1.4.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.233538 pybritive-1.4.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.233538 pybritive-1.4.0rc3/src/pybritive/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43430 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/britive_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/choices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/choices/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/cli_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/commands/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive/completers/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/api_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/bash_gte_42.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/powershell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/completers/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.241538 pybritive-1.4.0rc3/src/pybritive/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/api_method_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/aws_credential_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/build_britive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/cloud_credential_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/profile_argument_dectorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/helpers/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/src/pybritive/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_console_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_credentials_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/blocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/britive_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/checked_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/configure_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/federation_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/force_renew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/gcloud_key_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/justification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/maxpolltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/passphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/silent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_key_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_push_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/ssh_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/src/pybritive/options/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.237538 pybritive-1.4.0rc3/src/pybritive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 13:10:55.000000 pybritive-1.4.0rc3/src/pybritive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:10:55.249538 pybritive-1.4.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0100_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0200_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0300_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0400_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0450_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0500_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0600_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0700_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0800_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0850_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_0900_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 13:10:43.000000 pybritive-1.4.0rc3/tests/test_1000_logout.py
```

### Comparing `pybritive-1.4.0rc2/LICENSE` & `pybritive-1.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/PKG-INFO` & `pybritive-1.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc2/README.md` & `pybritive-1.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/setup.cfg` & `pybritive-1.4.0rc3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybritive
-version = 1.4.0rc2
+version = 1.4.0rc3
 author = Britive Inc.
 author_email = support@britive.com
 description = A pure Python CLI for Britive
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.britive.com
 classifiers =
```

### Comparing `pybritive-1.4.0rc2/src/pybritive/britive_cli.py` & `pybritive-1.4.0rc3/src/pybritive/britive_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,34 +373,48 @@
                 credentials=credentials,
                 silent=silent,
                 cli=self
             )
 
     def checkin(self, profile):
         self.login()
+        self._set_available_profiles()
         parts = self._split_profile_into_parts(profile)
 
         ids = self._convert_names_to_ids(
             profile_name=parts['profile'],
             environment_name=parts['env'],
             application_name=parts['app']
         )
 
         transaction_id = None
-        for profile in self.b.my_access.list_checked_out_profiles():
-            if profile['environmentId'] == ids['environment_id'] and profile['papId'] == ids['profile_id']:
-                transaction_id = profile['transactionId']
+        application_type = None
+        for checked_out_profile in self.b.my_access.list_checked_out_profiles():
+            same_env = checked_out_profile['environmentId'] == ids['environment_id']
+            same_profile = checked_out_profile['papId'] == ids['profile_id']
+            if all([same_env, same_profile]):
+                transaction_id = checked_out_profile['transactionId']
+
+                for available_profile in self.available_profiles:
+                    same_env_2 = checked_out_profile['environmentId'] == available_profile['env_id']
+                    same_profile_2 = checked_out_profile['papId'] == available_profile['profile_id']
+                    if all([same_env_2, same_profile_2]):
+                        application_type = available_profile['app_type'].lower()
+                        break
                 break
         if not transaction_id:
             raise ValueError(f'no checked out profile found for the given profile')
 
         self.b.my_access.checkin(
             transaction_id=transaction_id
         )
 
+        if application_type in ('aws', 'aws standalone'):
+            self.clear_cached_aws_credentials(profile)
+
     def _checkout(self, profile_name, env_name, app_name, programmatic, blocktime, maxpolltime, justification):
         try:
             self.login()
 
             ids = self._convert_names_to_ids(
                 profile_name=profile_name,
                 environment_name=env_name,
@@ -1026,7 +1040,18 @@
     def request_disposition(self, request_id, decision):
         self.login()
 
         if decision == 'approve':
             self.b.my_access.approve_request(request_id=request_id)
         if decision == 'reject':
             self.b.my_access.reject_request(request_id=request_id)
+
+    def clear_cached_aws_credentials(self, profile):
+        # start with the profile name that was passed in from the command
+        Cache().clear_awscredentialprocess(profile_name=profile)
+
+        # then we can try to split it into parts and clear that version of the
+        # profile name as well - it will not hurt anything to try to clear
+        # both versions
+        parts = self._split_profile_into_parts(profile)
+        Cache().clear_awscredentialprocess(profile_name=f"{parts['app']}/{parts['env']}/{parts['profile']}")
+
```

### Comparing `pybritive-1.4.0rc2/src/pybritive/choices/mode.py` & `pybritive-1.4.0rc3/src/pybritive/choices/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/choices/output_format.py` & `pybritive-1.4.0rc3/src/pybritive/choices/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/cli_interface.py` & `pybritive-1.4.0rc3/src/pybritive/cli_interface.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/api.py` & `pybritive-1.4.0rc3/src/pybritive/commands/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/aws.py` & `pybritive-1.4.0rc3/src/pybritive/commands/aws.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/cache.py` & `pybritive-1.4.0rc3/src/pybritive/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/checkin.py` & `pybritive-1.4.0rc3/src/pybritive/commands/checkin.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/checkout.py` & `pybritive-1.4.0rc3/src/pybritive/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/configure.py` & `pybritive-1.4.0rc3/src/pybritive/commands/configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/login.py` & `pybritive-1.4.0rc3/src/pybritive/commands/login.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/ls.py` & `pybritive-1.4.0rc3/src/pybritive/commands/ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/request.py` & `pybritive-1.4.0rc3/src/pybritive/commands/request.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/secret.py` & `pybritive-1.4.0rc3/src/pybritive/commands/secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/commands/ssh.py` & `pybritive-1.4.0rc3/src/pybritive/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/completers/api.py` & `pybritive-1.4.0rc3/src/pybritive/completers/api.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/completers/api_command.py` & `pybritive-1.4.0rc3/src/pybritive/completers/api_command.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/completers/bash_gte_42.py` & `pybritive-1.4.0rc3/src/pybritive/completers/bash_gte_42.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/completers/powershell_completion.py` & `pybritive-1.4.0rc3/src/pybritive/completers/powershell_completion.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/completers/profile.py` & `pybritive-1.4.0rc3/src/pybritive/completers/profile.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/aws_credential_process.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/aws_credential_process.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/build_britive.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/build_britive.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/cache.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 import json
 import os
+
+
 from .encryption import StringEncryption, InvalidPassphraseException
 
 
 class Cache:
     def __init__(self, passphrase: str = None):
         self.passphrase = passphrase
         self.string_encryptor = StringEncryption(passphrase=self.passphrase)
@@ -50,18 +52,22 @@
     def clear(self):
         self.cache['profiles'] = []
         self.cache['awscredentialprocess'] = {}
         self.write()
 
     def get_awscredentialprocess(self, profile_name: str):
         try:
-            ciphertext = self.cache['awscredentialprocess'].get(profile_name)
+            ciphertext = self.cache['awscredentialprocess'].get(profile_name.lower())
             if not ciphertext:
                 return None
             return json.loads(self.string_encryptor.decrypt(ciphertext))
         except InvalidPassphraseException:  # if we cannot decrypt don't error - just make the API call to get the creds
             return None
 
     def save_awscredentialprocess(self, profile_name: str, credentials: dict):
         ciphertext = self.string_encryptor.encrypt(json.dumps(credentials, default=str))
-        self.cache['awscredentialprocess'][profile_name] = ciphertext
+        self.cache['awscredentialprocess'][profile_name.lower()] = ciphertext
+        self.write()
+
+    def clear_awscredentialprocess(self, profile_name: str):
+        self.cache['awscredentialprocess'].pop(profile_name.lower(), None)
         self.write()
```

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/cloud_credential_printer.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/cloud_credential_printer.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/config.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/config.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/credentials.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/credentials.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/encryption.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/encryption.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/helpers/split.py` & `pybritive-1.4.0rc3/src/pybritive/helpers/split.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/options/britive_options.py` & `pybritive-1.4.0rc3/src/pybritive/options/britive_options.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/options/browser.py` & `pybritive-1.4.0rc3/src/pybritive/options/browser.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/options/mode.py` & `pybritive-1.4.0rc3/src/pybritive/options/mode.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/options/output_format.py` & `pybritive-1.4.0rc3/src/pybritive/options/output_format.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive/options/version.py` & `pybritive-1.4.0rc3/src/pybritive/options/version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/src/pybritive.egg-info/PKG-INFO` & `pybritive-1.4.0rc3/src/pybritive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybritive
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: A pure Python CLI for Britive
 Home-page: https://www.britive.com
 Author: Britive Inc.
 Author-email: support@britive.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybritive-1.4.0rc2/src/pybritive.egg-info/SOURCES.txt` & `pybritive-1.4.0rc3/src/pybritive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0100_version.py` & `pybritive-1.4.0rc3/tests/test_0100_version.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0200_configure.py` & `pybritive-1.4.0rc3/tests/test_0200_configure.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0400_ls.py` & `pybritive-1.4.0rc3/tests/test_0400_ls.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0500_secret.py` & `pybritive-1.4.0rc3/tests/test_0500_secret.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0700_checkout.py` & `pybritive-1.4.0rc3/tests/test_0700_checkout.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0850_clear.py` & `pybritive-1.4.0rc3/tests/test_0850_clear.py`

 * *Files identical despite different names*

### Comparing `pybritive-1.4.0rc2/tests/test_0900_login.py` & `pybritive-1.4.0rc3/tests/test_0900_login.py`

 * *Files identical despite different names*

