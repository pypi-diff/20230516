# Comparing `tmp/cool_cache-0.3.1.tar.gz` & `tmp/cool_cache-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cool_cache-0.3.1.tar", last modified: Thu Apr 20 04:08:34 2023, max compression
+gzip compressed data, was "cool_cache-0.3.4.tar", last modified: Tue May 16 17:26:25 2023, max compression
```

## Comparing `cool_cache-0.3.1.tar` & `cool_cache-0.3.4.tar`

### file list

```diff
@@ -1,12 +1,401 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.173319 cool_cache-0.3.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-20 04:08:34.173138 cool_cache-0.3.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.172066 cool_cache-0.3.1/cool_cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7261 2023-04-20 03:52:36.000000 cool_cache-0.3.1/cool_cache/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:08:34.172969 cool_cache-0.3.1/cool_cache.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-04-20 04:08:33.000000 cool_cache-0.3.1/cool_cache.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      200 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-20 04:08:33.000000 cool_cache-0.3.1/cool_cache.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       57 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-04-20 04:08:34.000000 cool_cache-0.3.1/cool_cache.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-20 04:08:34.173378 cool_cache-0.3.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1208 2022-11-09 13:57:56.000000 cool_cache-0.3.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.557391 cool_cache-0.3.4/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-16 17:26:25.557223 cool_cache-0.3.4/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.400934 cool_cache-0.3.4/cool_cache/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.401772 cool_cache-0.3.4/cool_cache/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-04-20 16:21:52.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.402111 cool_cache-0.3.4/cool_cache/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7125 2023-04-20 04:15:05.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.397157 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.404326 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.407000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.412904 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.413584 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.420290 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.422011 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.422671 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.422936 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11916 2023-04-20 04:20:51.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.423618 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10589 2023-04-20 04:19:09.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.424503 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.424727 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.425101 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.426290 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.427892 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.428820 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.439521 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.446682 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.396848 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.447163 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.395194 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.395366 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.450208 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.451798 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.454452 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.456423 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.458241 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.396541 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.460247 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.460891 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.461184 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.461316 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.461509 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.463240 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.463447 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.466817 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.467226 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.467417 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.479619 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.485750 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.486839 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.489410 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.493141 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.496184 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.496827 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.498167 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.498343 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.499664 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.505514 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.507704 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.509066 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.518329 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.519971 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.397559 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.397599 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.520256 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.520557 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3435 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.397774 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.521762 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      821 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.522202 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       19 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      656 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__dependencies__/simple_namespace/main/simple_namespace/main.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11162 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/build/lib/super_hash/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.523605 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/dist/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8109 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6-py3-none-any.whl
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7986 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/dist/super_hash-1.2.6.tar.gz
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.523786 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11225 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.526394 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8146 2023-04-20 04:19:09.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.526095 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1872 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-04-20 04:18:55.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/main/super_hash.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.526687 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.526976 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.533365 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.534113 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.534624 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.540886 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.542759 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.399828 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.542915 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.398668 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.398827 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.543746 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.544777 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.545827 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.546420 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.546748 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.399596 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.546958 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.547194 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.547450 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.547605 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.547855 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.548062 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.548185 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.548288 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.548398 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.548508 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.552886 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.553940 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.554412 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.554860 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.555380 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.555674 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.556048 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.556182 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/tests/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      497 2023-04-20 04:13:48.000000 cool_cache-0.3.4/cool_cache/__dependencies__/__sources__/super_hash/tests/test.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7304 2023-04-20 04:21:13.000000 cool_cache-0.3.4/cool_cache/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.556878 cool_cache-0.3.4/cool_cache/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4340 2022-12-15 16:26:17.000000 cool_cache-0.3.4/cool_cache/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4530 2023-04-20 04:15:05.000000 cool_cache-0.3.4/cool_cache/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      242 2023-04-20 16:25:12.000000 cool_cache-0.3.4/cool_cache/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-16 17:26:25.401653 cool_cache-0.3.4/cool_cache.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3273 2023-05-16 17:26:24.000000 cool_cache-0.3.4/cool_cache.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    28377 2023-05-16 17:26:25.000000 cool_cache-0.3.4/cool_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-16 17:26:25.000000 cool_cache-0.3.4/cool_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       11 2023-05-16 17:26:25.000000 cool_cache-0.3.4/cool_cache.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-16 17:26:25.557445 cool_cache-0.3.4/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1421 2023-05-16 16:55:18.000000 cool_cache-0.3.4/setup.py
```

### Comparing `cool_cache-0.3.1/PKG-INFO` & `cool_cache-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool_cache
-Version: 0.3.1
+Version: 0.3.4
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.1/cool_cache/__init__.py` & `cool_cache-0.3.4/cool_cache/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 import pickle
 import queue
 import threading
 from os import path
 from threading import Thread
 from copy import deepcopy
 
-import file_system_py as FS
-from super_hash import super_hash, hash_file
-from super_map import LazyDict
+from .__dependencies__ import file_system_py as FS
+from .__dependencies__.super_hash import super_hash, hash_file
 
 try:
     # use dill if its available
     import dill as pickle
 except ImportError as error:
     pass
 
-settings = LazyDict(
-    default_folder="cache.ignore/",
-    worker_que_size=1000,
-)
+class Object:
+    pass
 
 class NotGiven:
     pass
 
+settings = Object()
+settings.default_folder = "cache.ignore/"
+settings.worker_que_size = 1000
+
 class CacheData:
     calculated = False
     cache_file_name = ""
     deep_hash = ""
     cache = {}
 
 # since we only care about latest
```

### Comparing `cool_cache-0.3.1/cool_cache.egg-info/PKG-INFO` & `cool_cache-0.3.4/cool_cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cool-cache
-Version: 0.3.1
+Version: 0.3.4
 Summary: Cache any function to disk
 Home-page: https://github.com/jeff-hykin/cool_cache.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cool_cache-0.3.1/setup.py` & `cool_cache-0.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import setuptools
 import toml
+from file_system_py import iterate_paths_in
 
 # 
 # get the data out of the toml file
 # 
 toml_info = toml.load("../pyproject.toml")
 package_info = {**toml_info["tool"]["poetry"], **toml_info["tool"]["extra"]}
 
@@ -21,18 +22,22 @@
     version=package_info["version"],
     description=package_info["description"],
     url=package_info["url"],
     author=package_info["author"],
     author_email=package_info["author_email"],
     license=package_info["license"],
     packages=[package_info["name"]],
+    package_data={
+        # include all files/folders in the module (recursively)
+        package_info["name"]: [
+            each[len(package_info["name"])+1:]
+                for each in iterate_paths_in(package_info["name"], recursively=True)
+        ],
+    },
     install_requires=[
-        "file-system-py >= 0.0.6",
-        "super-hash >= 1.2.2",
-        "super-map >= 1.2.1",
     ],
     classifiers=[
         # examples:
         # 'Development Status :: 5 - Production/Stable',
         # 'Intended Audience :: Developers',
         # 'Programming Language :: Python',
         # "Programming Language :: Python :: 3",
```

