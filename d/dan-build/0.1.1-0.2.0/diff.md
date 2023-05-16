# Comparing `tmp/dan-build-0.1.1.tar.gz` & `tmp/dan-build-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dan-build-0.1.1.tar", last modified: Sat May 13 23:52:19 2023, max compression
+gzip compressed data, was "dan-build-0.2.0.tar", last modified: Tue May 16 12:28:02 2023, max compression
```

## Comparing `dan-build-0.1.1.tar` & `dan-build-0.2.0.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.531222 dan-build-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-05-13 13:14:52.000000 dan-build-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2358 2023-05-13 23:52:19.530225 dan-build-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1828 2023-05-13 16:18:25.000000 dan-build-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.445451 dan-build-0.1.1/dan/
--rw-rw-rw-   0        0        0      365 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/__init__.py
--rw-rw-rw-   0        0        0       65 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/__main__.py
--rw-rw-rw-   0        0        0    11767 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.448443 dan-build-0.1.1/dan/cmake/
--rw-rw-rw-   0        0        0       51 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cmake/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cmake/configure_file.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.452434 dan-build-0.1.1/dan/conan/
--rw-rw-rw-   0        0        0       34 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/conan/__init__.py
--rw-rw-rw-   0        0        0     3135 2023-05-13 16:29:34.000000 dan-build-0.1.1/dan/conan/requirements.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.487339 dan-build-0.1.1/dan/core/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/__init__.py
--rw-rw-rw-   0        0        0      933 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/aiofiles.py
--rw-rw-rw-   0        0        0     9952 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/asyncio.py
--rw-rw-rw-   0        0        0     2986 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/cache.py
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/detect.py
--rw-rw-rw-   0        0        0      100 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/errors.py
--rw-rw-rw-   0        0        0     1951 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/find.py
--rw-rw-rw-   0        0        0     1053 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/functools.py
--rw-rw-rw-   0        0        0     1063 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/generator.py
--rw-rw-rw-   0        0        0     5226 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/core/include.py
--rw-rw-rw-   0        0        0     4693 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/core/makefile.py
--rw-rw-rw-   0        0        0    14158 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/osinfo.py
--rw-rw-rw-   0        0        0      814 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/pathlib.py
--rw-rw-rw-   0        0        0     1100 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/pm.py
--rw-rw-rw-   0        0        0      602 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/register.py
--rw-rw-rw-   0        0        0     3698 2023-05-13 16:29:34.000000 dan-build-0.1.1/dan/core/requirements.py
--rw-rw-rw-   0        0        0     5733 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/runners.py
--rw-rw-rw-   0        0        0     2322 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/settings.py
--rw-rw-rw-   0        0        0    15359 2023-05-13 23:34:02.000000 dan-build-0.1.1/dan/core/target.py
--rw-rw-rw-   0        0        0     4634 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/test.py
--rw-rw-rw-   0        0        0     1672 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/utils.py
--rw-rw-rw-   0        0        0     3821 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/version.py
--rw-rw-rw-   0        0        0     3407 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/core/win.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.496315 dan-build-0.1.1/dan/cxx/
--rw-rw-rw-   0        0        0     2678 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cxx/__init__.py
--rw-rw-rw-   0        0        0     1395 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/compile_commands.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.500304 dan-build-0.1.1/dan/cxx/data/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/__init__.py
--rwxrwxrwx   0        0        0       29 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/detect.cmd
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/data/empty.c
--rw-rw-rw-   0        0        0    21030 2023-05-13 16:18:25.000000 dan-build-0.1.1/dan/cxx/detect.py
--rw-rw-rw-   0        0        0     5974 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/msvc_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.502301 dan-build-0.1.1/dan/cxx/support/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/support/__init__.py
--rw-rw-rw-   0        0        0     3524 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/support/qt.py
--rw-rw-rw-   0        0        0    17233 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/targets.py
--rw-rw-rw-   0        0        0     7265 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/toolchain.py
--rw-rw-rw-   0        0        0     6509 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/cxx/unix_toolchain.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.506288 dan-build-0.1.1/dan/io/
--rw-rw-rw-   0        0        0       35 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/io/__init__.py
--rw-rw-rw-   0        0        0     4824 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/io/package.py
--rw-rw-rw-   0        0        0     1392 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/io/repositories.py
--rw-rw-rw-   0        0        0     1679 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/jinja.py
--rw-rw-rw-   0        0        0     4023 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/logging.py
--rw-rw-rw-   0        0        0    15674 2023-05-13 23:45:04.000000 dan-build-0.1.1/dan/make.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.509292 dan-build-0.1.1/dan/pkgconfig/
--rw-rw-rw-   0        0        0       71 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/__init__.py
--rw-rw-rw-   0        0        0     9345 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/package.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.511275 dan-build-0.1.1/dan/pkgconfig/templates/
--rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/templates/__init__.py
--rw-rw-rw-   0        0        0      429 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/pkgconfig/templates/pkg.pc.jinja2
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.515265 dan-build-0.1.1/dan/smc/
--rw-rw-rw-   0        0        0       56 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/git.py
--rw-rw-rw-   0        0        0     1071 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/smc/tar.py
--rw-rw-rw-   0        0        0       37 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/testing.py
--rw-rw-rw-   0        0        0     6360 2023-05-13 15:47:33.000000 dan-build-0.1.1/dan/vscode.py
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.524242 dan-build-0.1.1/dan_build.egg-info/
--rw-rw-rw-   0        0        0     2358 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1488 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-13 23:52:19.000000 dan-build-0.1.1/dan_build.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1222 2023-05-13 23:51:29.000000 dan-build-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 23:52:19.531222 dan-build-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 23:52:19.528230 dan-build-0.1.1/tests/
--rw-rw-rw-   0        0        0     3114 2023-05-13 15:47:33.000000 dan-build-0.1.1/tests/test_cxx_libraries.py
--rw-rw-rw-   0        0        0     2950 2023-05-13 15:47:33.000000 dan-build-0.1.1/tests/test_cxx_simple.py
--rw-rw-rw-   0        0        0     2268 2023-05-13 13:04:49.000000 dan-build-0.1.1/tests/test_cxx_smc_catch2.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.467818 dan-build-0.2.0/
+-rw-rw-rw-   0        0        0     1092 2023-05-13 13:14:52.000000 dan-build-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3629 2023-05-16 12:28:02.467818 dan-build-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1828 2023-05-13 16:18:25.000000 dan-build-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.340174 dan-build-0.2.0/completion/
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.355119 dan-build-0.2.0/completion/bash/
+-rw-rw-rw-   0        0        0      654 2023-05-13 16:11:33.000000 dan-build-0.2.0/completion/bash/dan.sh
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.368085 dan-build-0.2.0/dan/
+-rw-rw-rw-   0        0        0      365 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/__init__.py
+-rw-rw-rw-   0        0        0       65 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/__main__.py
+-rw-rw-rw-   0        0        0    11767 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.371077 dan-build-0.2.0/dan/cmake/
+-rw-rw-rw-   0        0        0       51 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cmake/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cmake/configure_file.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.375067 dan-build-0.2.0/dan/conan/
+-rw-rw-rw-   0        0        0       34 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/conan/__init__.py
+-rw-rw-rw-   0        0        0     3117 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/conan/requirements.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.414959 dan-build-0.2.0/dan/core/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/__init__.py
+-rw-rw-rw-   0        0        0      933 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/aiofiles.py
+-rw-rw-rw-   0        0        0     9952 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/asyncio.py
+-rw-rw-rw-   0        0        0     3029 2023-05-14 09:30:30.000000 dan-build-0.2.0/dan/core/cache.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/detect.py
+-rw-rw-rw-   0        0        0      100 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/errors.py
+-rw-rw-rw-   0        0        0     1951 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/find.py
+-rw-rw-rw-   0        0        0     1053 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/functools.py
+-rw-rw-rw-   0        0        0     1063 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/generator.py
+-rw-rw-rw-   0        0        0     5669 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/include.py
+-rw-rw-rw-   0        0        0     4670 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/makefile.py
+-rw-rw-rw-   0        0        0    14158 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/osinfo.py
+-rw-rw-rw-   0        0        0      814 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/pathlib.py
+-rw-rw-rw-   0        0        0     1100 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/pm.py
+-rw-rw-rw-   0        0        0      602 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/register.py
+-rw-rw-rw-   0        0        0     4461 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/requirements.py
+-rw-rw-rw-   0        0        0     5733 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/runners.py
+-rw-rw-rw-   0        0        0     2322 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/settings.py
+-rw-rw-rw-   0        0        0    15715 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/target.py
+-rw-rw-rw-   0        0        0     4634 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/test.py
+-rw-rw-rw-   0        0        0     1672 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/utils.py
+-rw-rw-rw-   0        0        0     4203 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/core/version.py
+-rw-rw-rw-   0        0        0     3407 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/core/win.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.424932 dan-build-0.2.0/dan/cxx/
+-rw-rw-rw-   0        0        0     2678 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cxx/__init__.py
+-rw-rw-rw-   0        0        0     1395 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/compile_commands.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.428922 dan-build-0.2.0/dan/cxx/data/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/__init__.py
+-rwxrwxrwx   0        0        0       29 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/detect.cmd
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/data/empty.c
+-rw-rw-rw-   0        0        0    21030 2023-05-13 16:18:25.000000 dan-build-0.2.0/dan/cxx/detect.py
+-rw-rw-rw-   0        0        0     5974 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/msvc_toolchain.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.431914 dan-build-0.2.0/dan/cxx/support/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/support/__init__.py
+-rw-rw-rw-   0        0        0     3524 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/support/qt.py
+-rw-rw-rw-   0        0        0    17115 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/cxx/targets.py
+-rw-rw-rw-   0        0        0     7231 2023-05-14 12:16:57.000000 dan-build-0.2.0/dan/cxx/toolchain.py
+-rw-rw-rw-   0        0        0     6509 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/cxx/unix_toolchain.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.437901 dan-build-0.2.0/dan/io/
+-rw-rw-rw-   0        0        0       35 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/io/__init__.py
+-rw-rw-rw-   0        0        0     8536 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/io/package.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/io/repositories.py
+-rw-rw-rw-   0        0        0     1679 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/jinja.py
+-rw-rw-rw-   0        0        0     4023 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/logging.py
+-rw-rw-rw-   0        0        0    15674 2023-05-13 23:45:04.000000 dan-build-0.2.0/dan/make.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.441889 dan-build-0.2.0/dan/pkgconfig/
+-rw-rw-rw-   0        0        0       71 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/__init__.py
+-rw-rw-rw-   0        0        0     9318 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/pkgconfig/package.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.444880 dan-build-0.2.0/dan/pkgconfig/templates/
+-rw-rw-rw-   0        0        0        0 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/templates/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/pkgconfig/templates/pkg.pc.jinja2
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.449866 dan-build-0.2.0/dan/smc/
+-rw-rw-rw-   0        0        0       56 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/smc/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/smc/git.py
+-rw-rw-rw-   0        0        0     1033 2023-05-16 12:08:59.000000 dan-build-0.2.0/dan/smc/tar.py
+-rw-rw-rw-   0        0        0       37 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/testing.py
+-rw-rw-rw-   0        0        0     6360 2023-05-13 15:47:33.000000 dan-build-0.2.0/dan/vscode.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.461834 dan-build-0.2.0/dan_build.egg-info/
+-rw-rw-rw-   0        0        0     3629 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1511 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-16 12:28:02.000000 dan-build-0.2.0/dan_build.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1313 2023-05-16 12:21:25.000000 dan-build-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:28:02.468815 dan-build-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 12:28:02.465823 dan-build-0.2.0/tests/
+-rw-rw-rw-   0        0        0     3114 2023-05-13 15:47:33.000000 dan-build-0.2.0/tests/test_cxx_libraries.py
+-rw-rw-rw-   0        0        0     2950 2023-05-13 15:47:33.000000 dan-build-0.2.0/tests/test_cxx_simple.py
+-rw-rw-rw-   0        0        0     2268 2023-05-13 13:04:49.000000 dan-build-0.2.0/tests/test_cxx_smc_catch2.py
```

### Comparing `dan-build-0.1.1/LICENSE` & `dan-build-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/PKG-INFO` & `dan-build-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: dan-build
-Version: 0.1.1
-Summary: Python-based build system.
-Author-email: Garcia Sylvain <garcia.6l20@gmail.com>, garcia.6l20@gmail.com
-Project-URL: homepage, https://github.com/Garcia6L20/dan
-Project-URL: documentation, https://github.com/Garcia6L20/dan
-Project-URL: repository, https://github.com/Garcia6L20/dan
-Keywords: packaging,dependency,build system
-Classifier: Topic :: Software Development
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dan
 
 > _Do Anything Now_
 
 _dan_ is a build system inspired from _GNU make_, _cmake_, _meson_, ... but only in python.
 
 ## Features
```

### Comparing `dan-build-0.1.1/dan/cli.py` & `dan-build-0.2.0/dan/cli.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cmake/configure_file.py` & `dan-build-0.2.0/dan/cmake/configure_file.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/conan/requirements.py` & `dan-build-0.2.0/dan/conan/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 """
 
 
 class ConanFile(Target, internal=True):
     def __init__(self, makefile) -> None:
         super().__init__('conanfile', makefile=makefile)
         self.__reqs = list()
-        self.output = self.build_path / 'conanfile.txt'
+        self.output = 'conanfile.txt'
 
     def add(self, pkg: 'Package'):
         self.__reqs.append(pkg)
 
     async def __build__(self):
         template = jinja2.Environment(
             loader=jinja2.BaseLoader).from_string(_conanfile_template)
```

### Comparing `dan-build-0.1.1/dan/core/aiofiles.py` & `dan-build-0.2.0/dan/core/aiofiles.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/asyncio.py` & `dan-build-0.2.0/dan/core/asyncio.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/cache.py` & `dan-build-0.2.0/dan/core/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,16 @@
 
     @classmethod
     def get(cls, name) -> 'Cache':
         if name in cls.__caches:
             return cls.__caches[name]
 
     def ignore(self):
-        del self.__caches[self.name]
+        if self.name in self.__caches:
+            del self.__caches[self.name]
 
 
 def once_method(fn):    
     result_name = f'_{fn.__name__}_result'
 
     @functools.wraps(fn)
     def wrapper(self, *args, **kwds):
```

### Comparing `dan-build-0.1.1/dan/core/find.py` & `dan-build-0.2.0/dan/core/find.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/functools.py` & `dan-build-0.2.0/dan/core/functools.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/generator.py` & `dan-build-0.2.0/dan/core/generator.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/include.py` & `dan-build-0.2.0/dan/core/include.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import importlib.util
 import os
-import re
+
 from dan.core.asyncio import sync_wait
 from dan.core.makefile import MakeFile
-
 from dan.core.pathlib import Path
 from dan.core.requirements import load_requirements
-
 from dan.core.target import Target
 from dan.logging import Logging
-from dan.pkgconfig.package import MissingPackage, Package, RequiredPackage, parse_requirement
+from dan.pkgconfig.package import parse_requirement
 
 
 class TargetNotFound(RuntimeError):
     def __init__(self, name) -> None:
         super().__init__(f'package {name} not found')
 
 
@@ -89,38 +87,46 @@
     global context
     for m in context.all_makefiles:
         del m
     del context
     context = Context()
 
 
-def _init_makefile(module, name: str = 'root', build_path: Path = None, requirements: MakeFile = None):
+def _init_makefile(module, name: str = 'root', build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None):
     global context
     source_path = Path(module.__file__).parent
-    if not build_path:
-        assert context.current
-        build_path = build_path or context.current.build_path / name
+    if parent is None and context.current is not None:
+        parent = context.current
+
+    if build_path is None:
+        assert parent is not None
+        build_path = build_path or parent.build_path / name
     build_path.mkdir(parents=True, exist_ok=True)
 
     module.__class__ = MakeFile
     context.current = module
     module._setup(
         name,
         source_path,
         build_path,
-        requirements)
+        requirements,
+        parent)
 
+_imported_makefiles: dict[Path, MakeFile] = dict()
 
-def load_makefile(module_path: Path, name: str = None, module_name: str = None, build_path: Path = None, requirements: MakeFile = None) -> MakeFile:
+def load_makefile(module_path: Path, name: str = None, module_name: str = None, build_path: Path = None, requirements: MakeFile = None, parent: MakeFile = None) -> MakeFile:
     name = name or module_path.stem
     module_name = module_name or name
+    if module_path in _imported_makefiles:
+        return _imported_makefiles[module_path]
     spec = importlib.util.spec_from_file_location(
         module_name, module_path)
     module = importlib.util.module_from_spec(spec)
-    _init_makefile(module, name, build_path, requirements)
+    _imported_makefiles[module_path] = module
+    _init_makefile(module, name, build_path, requirements, parent)
     spec.loader.exec_module(module)
     context.up()
     return module
 
 
 def include_makefile(name: str | Path, build_path: Path = None) -> set[Target]:
     ''' Include a sub-directory (or a sub-makefile).
@@ -143,15 +149,20 @@
             if module_path.exists():
                 spec = importlib.util.spec_from_file_location(
                     f'{context.current.name}.{name}', module_path)
                 break
         else:
             raise RuntimeError(
                 f'Cannot find anything to include for "{name}" (looked for: {", ".join(lookups)})')
+        
+    if module_path in _imported_makefiles:
+        return _imported_makefiles[module_path]
+
     module = importlib.util.module_from_spec(spec)
+    _imported_makefiles[module_path] = module
     _init_makefile(module, name, build_path)
 
     requirements_file = module_path.with_stem('dan-requires')
     if module_path.stem == 'dan-build' and requirements_file.exists():
         context.current.requirements = load_makefile(
             requirements_file, name='dan-requires', module_name=f'{name}.requirements')
```

### Comparing `dan-build-0.1.1/dan/core/makefile.py` & `dan-build-0.2.0/dan/core/makefile.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 class MakeFile(sys.__class__):
 
     def _setup(self,
                name: str,
                source_path: Path,
                build_path: Path,
-               requirements: 'MakeFile' = None) -> None:
+               requirements: 'MakeFile' = None,
+               parent: 'MakeFile' = None) -> None:
         self.name = name
         self.description = None
         self.version = None
         self.source_path = source_path
         self.build_path = build_path
         self.__requirements = requirements
-        self.parent: MakeFile = self.parent if hasattr(
-            self, 'parent') else None
+        self.parent = parent
         self.__cache: Cache = None
         self.children: list[MakeFile] = list()
         if self.name != 'dan-requires' and self.parent:
             self.parent.children.append(self)
         self.options = Options(self)
         self.__targets: set[Target] = set()
         self.__tests: set[Test] = set()
```

### Comparing `dan-build-0.1.1/dan/core/osinfo.py` & `dan-build-0.2.0/dan/core/osinfo.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/pathlib.py` & `dan-build-0.2.0/dan/core/pathlib.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/pm.py` & `dan-build-0.2.0/dan/core/pm.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/register.py` & `dan-build-0.2.0/dan/core/register.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/requirements.py` & `dan-build-0.2.0/dan/core/requirements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 
 import functools
 import re
 import typing as t
 from dan.core import asyncio
+from dan.core.pm import re_match
 from dan.core.settings import InstallMode, InstallSettings
 
 from dan.core.version import Version, VersionSpec
 from dan.logging import Logging
 
 
 class RequiredPackage(Logging):
     def __init__(self, name: str, version_spec: VersionSpec = None):
-        self.name = name
         self.version_spec = version_spec
         super().__init__(name)
         self.target : 'Target' = None
 
+        match re_match(name):
+            case r'(.+?)@(.+)' as m:
+                self.name = m[1]
+                self.provider = m[2]
+            case _:
+                self.name = name
+                self.provider = None
+
     def is_compatible(self, t: 'Target'):
         if self.version_spec is not None:
             version_ok = self.version_spec.is_compatible(t.version)
         else:
             version_ok = True
         return t.name == self.name and version_ok
     
@@ -44,68 +52,75 @@
         if self.version_spec:
             return f'RequiredPackage[{self.name} {self.version_spec}]'
         return f'RequiredPackage[{self.name}]'
     
 
 def parse_requirement(req: str) -> RequiredPackage:
     req = req.strip()
-    m = re.match(r'(.+?)\s+([><]=?|=)\s+([\d\.]+)', req)
-    if m:
-        name = m[1]
-        op = m[2]
-        version = Version(m[3])
-        return RequiredPackage(name, VersionSpec(version, op))
+    name, spec = VersionSpec.parse(req)
+    if spec:
+        return RequiredPackage(name, spec)
     else:
         return RequiredPackage(req)
 
 async def load_requirements(requirements: t.Iterable[RequiredPackage], makefile, logger = None, install = True):
 
     from dan.pkgconfig.package import find_package
     from dan.logging import _get_makefile_logger
     from dan.core.include import context
+    from dan.io import Package
 
     if logger is None:
         logger = _get_makefile_logger()
 
     deps_install_path = makefile.pkgs_path
     deps_settings = InstallSettings(deps_install_path)
 
     pkgs_search_paths = [deps_install_path]
     if makefile.requirements:
         pkgs_search_paths.append(makefile.requirements.pkgs_path)
 
-    result = list()
-    unresolved = list()
+    resolved: list[RequiredPackage] = list()
+    unresolved: list[RequiredPackage] = list()
 
     async with asyncio.TaskGroup('requirement loading') as group:
         for req in requirements:
             if req.found:
-                result.append(req.target)
+                resolved.append(req)
                 continue
 
             t = context.root.find(req.name)
             if t and not t.is_requirement and req.is_compatible(t):
+                logger.debug('%s: already fullfilled by %s', req, t.fullname)
                 req.target = t
-                result.append(req.target)
+                resolved.append(req)
                 continue
 
             t = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
             if t is not None and req.is_compatible(t):
+                logger.debug('%s: using package %s', req, t.fullname)
                 req.target = t
-                result.append(t)
+                resolved.append(req)
             elif install:
-                t = makefile.requirements.find(req.name)
-                if not t:
-                    raise RuntimeError(f'Unresolved requirement {req}')
-                logger.debug('installing requirement: %s %s', req.name, req.version_spec)
+                if makefile.requirements:
+                    # install requirement from dan-requires.py
+                    t = makefile.requirements.find(req.name)
+                    if not t:
+                        raise RuntimeError(f'Unresolved requirement {req}, it should have been defined in {makefile.requirements.__file__}')
+                    logger.debug('%s using requirements\' target %s', req, t.fullname)
+                else:
+                    t = Package(req.name, req.version_spec, repository=req.provider, makefile=makefile)
+                    logger.debug('%s: adding package %s', req, t.fullname)
                 unresolved.append(req)                
                 group.create_task(t.install(deps_settings, InstallMode.dev))
 
+
+
     if install:
         for req in unresolved:
             pkg = find_package(req.name, req.version_spec, search_paths=pkgs_search_paths, makefile=makefile)
             if pkg is None:
                 raise RuntimeError(f'Unresolved requirement {req}')
             req.target = pkg
-            result.append(pkg)
+            resolved.append(req)
 
-    return result
+    return [req.target for req in resolved]
```

### Comparing `dan-build-0.1.1/dan/core/runners.py` & `dan-build-0.2.0/dan/core/runners.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/settings.py` & `dan-build-0.2.0/dan/core/settings.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/target.py` & `dan-build-0.2.0/dan/core/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,17 +226,17 @@
     preload_dependencies: set[TargetDependencyLike] = set()
 
     def __init__(self,
                  name: str = None,
                  parent: 'Target' = None,
                  version: str = None,
                  default: bool = None,
-                 makefile=None,
-                 build_path: Path = None) -> None:
-        self.version = Version(self.version) if self.version else None
+                 makefile=None) -> None:
+        if isinstance(self.version, str):
+            self.version = Version(self.version)
         self.parent = parent
         self.__cache: dict = None
 
         if name is not None:
             self.name = name
 
         if self.name is None:
@@ -254,18 +254,14 @@
 
         if makefile:
             self.makefile = makefile
 
         if self.makefile is None:
             raise RuntimeError('Makefile not resolved')
 
-        if build_path is None:
-            self.__build_path = self.makefile.build_path
-        else:
-            self.__build_path = build_path
 
         if self.fullname is None:
             self.fullname = f'{self.makefile.fullname}.{self.name}'
 
         self.options = Options(self, self.options)
 
         if self.version is None:
@@ -277,31 +273,48 @@
         self.other_generated_files: set[Path] = set()
         self.dependencies = Dependencies(self, self.dependencies)
         self.preload_dependencies = Dependencies(
             self, self.preload_dependencies)
 
         super().__init__(self.fullname)
 
-        if self.output is not None:
-            self.output = Path(self.output)
-            if not self.output.is_absolute():
-                self.output = self.build_path / self.output
+        self._output: Path = None
+
+        if type(self).output != Target.output:
+            # hack class-defined output
+            #   transform it to classproperty for build_path resolution
+            output = self.output
+            type(self).output = utils.classproperty(lambda: self.build_path / output)
+
+    
+    @property
+    def output(self):
+        if self._output is None:
+            return None
+        return self.build_path / self._output
+
+    @output.setter
+    def output(self, path):
+        path = Path(path)
+        if path.is_absolute() and self.build_path in path.parents:
+            raise RuntimeError(f'output must not be an absolute path within build directory')
+        self._output = path
 
     @property
     def is_requirement(self) -> bool:
         return self.makefile.name.endswith('requirements')
 
     @property
     def source_path(self) -> Path:
         return self.makefile.source_path
 
     @property
     def build_path(self) -> Path:
-        return self.__build_path
-
+        return self.makefile.build_path
+    
     @property
     def requires(self):
         from dan.pkgconfig.package import RequiredPackage
         return [dep for dep in self.dependencies if isinstance(dep, RequiredPackage)]
 
     @cached_property
     def fullname(self) -> str:
@@ -339,21 +352,21 @@
         return res
 
     @asyncio.cached
     async def initialize(self):
         await self.preload()
         self.debug('initializing...')
 
+        if isinstance(self.version, Option):
+            self.version = self.version.value
+
         async with asyncio.TaskGroup(f'initializing {self.name}\'s target dependencies') as group:
             for dep in self.target_dependencies:
                 group.create_task(dep.initialize())
 
-        if self.output and not self.output.is_absolute():
-            self.output = self.build_path / self.output
-
         res = self.__initialize__()
         if inspect.iscoroutine(res):
             res = await res
         return res
 
     @property
     def modification_time(self):
```

### Comparing `dan-build-0.1.1/dan/core/test.py` & `dan-build-0.2.0/dan/core/test.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/utils.py` & `dan-build-0.2.0/dan/core/utils.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/core/version.py` & `dan-build-0.2.0/dan/core/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 import re
 
 
 class Version:
-    version_pattern = re.compile('[.-]')
+    version_pattern = re.compile(r'[\.-]')
 
     def __init__(self, *args) -> None:
         if len(args) == 1 and isinstance(args[0], str):
-            args = Version.version_pattern.split(args[0])
+            parts = Version.version_pattern.split(args[0])
+            args = list()
+            # cleanup
+            for a in parts:
+                # drop non numeric parts (ie.: v0.11.0 -> 0.11.0, 1.2-preview5, mylib-3.2, etc...)
+                while not a.isnumeric() and len(a):
+                    a = a[1:]
+                if len(a):
+                    args.append(a)
         else:
             args = list(args)
+        
         self._parts = tuple(int(a) for a in args)
 
     @property
     def major(self):
         return self._parts[0]
 
     @property
@@ -46,61 +55,76 @@
         return True
 
     def __gt__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.major >= other.major \
-            or (self.minor or 0) > (other.minor or 0) \
-            or (self.patch or 0) > (other.patch or 0) \
-            or (self.build or 0) > (other.build or 0)
+        for mine, their in zip(self._parts, other._parts):
+            if mine > their:
+                return True
+            if mine < their:
+                return False
+        return False
+
 
     def __ge__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.major >= other.major \
-            or (self.minor or 0) >= (other.minor or 0) \
-            or (self.patch or 0) >= (other.patch or 0) \
-            or (self.build or 0) >= (other.build or 0)
+        return self.__eq__(other) or self.__gt__(other)
     
     def __lt__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.major < other.major \
-            or (self.minor or 0) < (other.minor or 0) \
-            or (self.patch or 0) < (other.patch or 0) \
-            or (self.build or 0) < (other.build or 0)
+        for mine, their in zip(self._parts, other._parts):
+            if mine < their:
+                return True
+            if mine > their:
+                return False
+        return False
+
     
     def __le__(self, other: 'Version'):
         if isinstance(other, str):
             other = Version(other)
         elif not isinstance(other, Version):
             return False
-        return self.major < other.major \
-            or (self.minor or 0) <= (other.minor or 0) \
-            or (self.patch or 0) <= (other.patch or 0) \
-            or (self.build or 0) <= (other.build or 0)
+        return self.__eq__(other) or self.__le__(other)
 
     def __str__(self) -> str:
         res = str(self.major)
         if self.minor is not None:
             res += f'.{self.minor}'
             if self.patch is not None:
                 res += f'.{self.patch}'
                 if self.build is not None:
                     res += f'.{self.build}'
         return res
+    
+    def __repr__(self) -> str:
+        return f'Version[{self}]'
 
 
 class VersionSpec:
+
+    @staticmethod
+    def parse(data: str) -> tuple[str|None, 'VersionSpec']:
+        m = re.match(r'(.+?)?\s+?([><]=?|=)\s+([\d\.]+)', data)
+        if m:
+            name = m[1]
+            op = m[2]
+            version = Version(m[3])
+            return name, VersionSpec(version, op)
+        return None, None
+
+
     def __init__(self, version: Version, op: str) -> None:
         self.version = version
         self.op = op
         
     def is_compatible(self, version: Version):
         match self.op:
             case '==' | '=':
```

### Comparing `dan-build-0.1.1/dan/core/win.py` & `dan-build-0.2.0/dan/core/win.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/__init__.py` & `dan-build-0.2.0/dan/cxx/__init__.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/compile_commands.py` & `dan-build-0.2.0/dan/cxx/compile_commands.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/detect.py` & `dan-build-0.2.0/dan/cxx/detect.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/msvc_toolchain.py` & `dan-build-0.2.0/dan/cxx/msvc_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/support/qt.py` & `dan-build-0.2.0/dan/cxx/support/qt.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/cxx/targets.py` & `dan-build-0.2.0/dan/cxx/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     def compile_definitions(self):
         return self.parent.compile_definitions
 
     async def __initialize__(self):
         await self.parent.preload()
 
         ext = 'o' if os.name != 'nt' else 'obj'
-        self.output: Path = self.build_path / \
-            Path(f'{self.source.stem}.{ext}')
+        self.output: Path = Path(f'{self.source.stem}.{ext}')
 
         deps = self.cache.get('deps')
         if deps is not None:
             self.dependencies.update(deps)
 
         self.dependencies.add(self.source)
 
@@ -328,18 +327,17 @@
 
         from .msvc_toolchain import MSVCToolchain
         if self.shared and isinstance(self.toolchain, MSVCToolchain):
             self.compile_definitions.add(f'{self.name.upper()}_EXPORT=1')
 
         if self.library_type != LibraryType.INTERFACE:
             self.dependencies.update(self.objs)
-            self.output = self.build_path / \
-                self.toolchain.make_library_name(self.name, self.shared)
+            self.output = self.toolchain.make_library_name(self.name, self.shared)
         else:
-            self.output = self.build_path / f"lib{self.name}.stamp"
+            self.output = f"lib{self.name}.stamp"
         await super().__initialize__()
 
         previous_args = self.cache.get('generate_args')
         generate = None
         match self.library_type:
             case LibraryType.STATIC:
                 generate = self.toolchain.static_lib
@@ -445,16 +443,15 @@
         return await super().__build__()
 
 class Executable(CXXObjectsTarget, internal=True):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.output = self.build_path / \
-            self.toolchain.make_executable_name(self.name)
+        self.output = self.toolchain.make_executable_name(self.name)
         self.__dirty = False
 
     async def __initialize__(self):
         await super().__initialize__()
 
         previous_args = self.cache.get('link_args')
         if previous_args:
```

### Comparing `dan-build-0.1.1/dan/cxx/toolchain.py` & `dan-build-0.2.0/dan/cxx/toolchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,15 @@
         with tempfile.NamedTemporaryFile('w', suffix=extension) as f:
             f.write(source)
             f.flush()
             try:
                 fname = Path(f.name)
                 sync_run(self.make_compile_commands(fname, fname.with_suffix('.o'), options)[0])
                 return True
-            except CommandError as err:
-                print(err)
+            except CommandError:
                 return False
 
     def has_include(self, *includes, options: set[str] = set(), extension='.cpp'):
         source = '\n'.join([f'#include {inc}' for inc in includes])
         return self.can_compile(source, options, extension)
 
     def has_definition(self, *definitions, options: set[str] = set(), extension='.cpp'):
```

### Comparing `dan-build-0.1.1/dan/cxx/unix_toolchain.py` & `dan-build-0.2.0/dan/cxx/unix_toolchain.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/io/repositories.py` & `dan-build-0.2.0/dan/io/repositories.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,35 +5,43 @@
 from dan.core.runners import async_run
 from dan.core import aiofiles
 
 class PackageRepository(Target, internal=True):
 
     url: str = None
 
+    # never up-to-date
+    up_to_date = False
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.output = get_dan_path() / 'repositories' / self.name
-
+    
     async def __build__(self):
-        try:
-            self.output.parent.mkdir(exist_ok=True, parents=True)
-            await async_run(f'git clone --mirror {self.url} {self.name}', logger=self, cwd=self.output.parent)
-
-        except Exception as e:
-            await aiofiles.rmtree(self.output)
-            raise e
+        if not self.output.exists():
+            try:
+                self.output.parent.mkdir(exist_ok=True, parents=True)
+                await async_run(f'git clone {self.url} {self.name}', logger=self, cwd=self.output.parent)
+
+            except Exception as e:
+                await aiofiles.rmtree(self.output)
+                raise e
+        else:
+                await async_run(f'git pull', logger=self, cwd=self.output)
 
 
 repositories : dict[str, dict] = {
     'dan.io': {
         'url': 'https://github.com/Garcia6l20/dan.io.git',
     }
 }
 
 def get_repo_instance(repo_name:str, makefile) -> PackageRepository:
+    if repo_name is None:
+        repo_name = next(iter(repositories.keys()))
     if not repo_name in repositories:
         raise RuntimeError(f'Unknown repository: {repo_name}')
     repo_data = repositories[repo_name]
     if not 'instance' in repo_data:
         class PackageRepositoryImpl(PackageRepository, internal=True):
             name = repo_name
             url = repo_data['url']
```

### Comparing `dan-build-0.1.1/dan/jinja.py` & `dan-build-0.2.0/dan/jinja.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/logging.py` & `dan-build-0.2.0/dan/logging.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/make.py` & `dan-build-0.2.0/dan/make.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan/pkgconfig/package.py` & `dan-build-0.2.0/dan/pkgconfig/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,14 @@
 
 class Package(CXXTarget, internal=True):
     all: dict[str, 'Package'] = dict()
 
     default = False
 
     def __init__(self, name, search_paths: list[str] = list(), config_path: Path = None, data: Data = None, **kwargs) -> None:
-        self.output = None
         if data is not None:
             self.config_path = data.path
             self.data = data
         else:
             self.config_path = config_path or find_pkg_config(name, search_paths)
             self.data: Data = None
         self.search_paths = search_paths
```

### Comparing `dan-build-0.1.1/dan/smc/git.py` & `dan-build-0.2.0/dan/smc/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         if url is not None:
             self.url = url
         if refspec is not None:
             self.refspec = refspec
         if patches is not None:
             self.patches = patches
         self.sha1 = None
-        self.output: Path = self.build_path / dirname
+        self.output: Path = dirname
         self.git_dir: Path = self.output / '.git'
         self.subdirectory = subdirectory
 
     async def __build__(self):
         try:
             self.output.mkdir()            
             await async_run(f'git init -q', logger=self, cwd=self.output)
```

### Comparing `dan-build-0.1.1/dan/smc/tar.py` & `dan-build-0.2.0/dan/smc/tar.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 class TarSources(Target, internal=True):
 
     url: str
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self.archive_name = self.url.split("/")[-1]
-        self.output: Path = self.build_path / 'sources'
+        self.output: Path = 'sources'
 
     async def __build__(self):
         self.info(f'downloading {self.url}')
-        await fetch_file(self.url, self.build_path / self.archive_name)
-        with tarfile.open(self.build_path / self.archive_name) as f:
-            self.info(f'extracting {self.archive_name}')
+        archive_name = self.url.split("/")[-1]
+        await fetch_file(self.url, self.build_path / archive_name)
+        with tarfile.open(self.build_path / archive_name) as f:
+            self.info(f'extracting {archive_name}')
             f.extractall(self.output)
```

### Comparing `dan-build-0.1.1/dan/vscode.py` & `dan-build-0.2.0/dan/vscode.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/dan_build.egg-info/SOURCES.txt` & `dan-build-0.2.0/dan_build.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+completion/bash/dan.sh
 dan/__init__.py
 dan/__main__.py
 dan/cli.py
 dan/jinja.py
 dan/logging.py
 dan/make.py
 dan/testing.py
```

### Comparing `dan-build-0.1.1/pyproject.toml` & `dan-build-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "dan-build"
-version = "0.1.1"
+version = "0.2.0"
 description = "Python-based build system."
 authors = [
     {name = "Garcia Sylvain", email="garcia.6l20@gmail.com"},
     {email = "garcia.6l20@gmail.com"}
 ]
-license = {file = "LICENSE.txt"}
+license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 
 keywords = ["packaging", "dependency", "build system"]
 
 classifiers = [
     "Topic :: Software Development"
@@ -35,14 +35,19 @@
 [tool.setuptools.packages.find]
 include = ["dan*"]
 
 [tool.setuptools.package-data]
 "dan.pkgconfig.templates" = ["*.jinja2"]
 "dan.cxx.data" = ["*"]
 
+[tool.setuptools.data-files]
+"etc/bash_completion.d" = [
+    "completion/bash/dan.sh",
+]
+
 
 [project.optional-dependencies]
 #dev = [
 #    "black>=18.3-alpha.0",
 #]
 
 [project.urls]
```

### Comparing `dan-build-0.1.1/tests/test_cxx_libraries.py` & `dan-build-0.2.0/tests/test_cxx_libraries.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/tests/test_cxx_simple.py` & `dan-build-0.2.0/tests/test_cxx_simple.py`

 * *Files identical despite different names*

### Comparing `dan-build-0.1.1/tests/test_cxx_smc_catch2.py` & `dan-build-0.2.0/tests/test_cxx_smc_catch2.py`

 * *Files identical despite different names*

