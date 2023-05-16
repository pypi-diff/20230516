# Comparing `tmp/skyeye-3.4.9.tar.gz` & `tmp/skyeye-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyeye-3.4.9.tar", last modified: Mon Apr 24 11:44:42 2023, max compression
+gzip compressed data, was "skyeye-3.5.0.tar", last modified: Tue May 16 07:53:12 2023, max compression
```

## Comparing `skyeye-3.4.9.tar` & `skyeye-3.5.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.294860 skyeye-3.4.9/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       36 2023-04-12 07:13:48.000000 skyeye-3.4.9/MANIFEST.in
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-04-24 11:44:42.295225 skyeye-3.4.9/PKG-INFO
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1883 2023-04-12 07:13:48.000000 skyeye-3.4.9/README.md
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      147 2023-04-24 11:44:42.297451 skyeye-3.4.9/setup.cfg
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      920 2023-04-12 07:13:48.000000 skyeye-3.4.9/setup.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.035717 skyeye-3.4.9/skyeye/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      209 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3857 2023-04-24 06:37:46.000000 skyeye-3.4.9/skyeye/apk_decompiling.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3546 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/apk_scanner.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2224 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/cli.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.068913 skyeye-3.4.9/skyeye/config/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      110 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/__init__.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.094935 skyeye-3.4.9/skyeye/config/__pycache__/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      271 2023-04-24 06:34:57.000000 skyeye-3.4.9/skyeye/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      182 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye/config/__pycache__/cli_config.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1288 2023-04-24 06:34:57.000000 skyeye-3.4.9/skyeye/config/__pycache__/config_center.cpython-310.pyc
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1278692 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/baksmali-2.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       39 2023-04-24 11:44:25.000000 skyeye-3.4.9/skyeye/config/cli_config.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      803 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/config_center.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.195213 skyeye-3.4.9/skyeye/config/dex-tools-2.1/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    11562 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/LICENSE.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      341 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/NOTICE.txt
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.196805 skyeye-3.4.9/skyeye/config/dex-tools-2.1/bin/
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     3277 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/bin/dex-tools.bat
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-baksmali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-baksmali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      845 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1371 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      843 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1369 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      847 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1373 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-access.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-access.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      831 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-smali.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1357 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-smali.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-std-apk.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-std-apk.sh
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      326 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j_invoke.bat
--rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1321 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j_invoke.sh
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.271177 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   239543 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1153819 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   167761 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1543336 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   374032 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   378662 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    17737 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174246 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   196809 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   237496 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    72149 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    76796 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174252 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   108508 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)   104543 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1030064 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3210 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/open-source-license.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)    25515 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)  3238491 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/config/jd-gui-1.6.6.jar
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.284954 skyeye-3.4.9/skyeye/dto/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      104 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/dto/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      923 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/dto/class_desc_dto.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      592 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/dto/config_dto.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.290169 skyeye-3.4.9/skyeye/parse/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      122 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/parse/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     5107 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/parse/method_block_parser.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3742 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/parse/smali_parser.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1858 2023-04-24 11:43:33.000000 skyeye-3.4.9/skyeye/result_wirter.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.293349 skyeye-3.4.9/skyeye/utils/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       58 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/utils/__init__.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       85 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/utils/string_util.py
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)      782 2023-04-12 07:13:48.000000 skyeye-3.4.9/skyeye/version_check.py
-drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-04-24 11:44:42.052909 skyeye-3.4.9/skyeye.egg-info/
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/PKG-INFO
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3558 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/SOURCES.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/dependency_links.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       42 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/entry_points.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)       16 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/requires.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        7 2023-04-24 11:44:41.000000 skyeye-3.4.9/skyeye.egg-info/top_level.txt
--rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-04-24 06:40:26.000000 skyeye-3.4.9/skyeye.egg-info/zip-safe
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.886971 skyeye-3.5.0/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       36 2023-04-12 07:13:48.000000 skyeye-3.5.0/MANIFEST.in
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-05-16 07:53:12.887147 skyeye-3.5.0/PKG-INFO
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1883 2023-04-12 07:13:48.000000 skyeye-3.5.0/README.md
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      147 2023-05-16 07:53:12.888093 skyeye-3.5.0/setup.cfg
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      920 2023-04-12 07:13:48.000000 skyeye-3.5.0/setup.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.605938 skyeye-3.5.0/skyeye/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      209 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3933 2023-05-16 07:50:55.000000 skyeye-3.5.0/skyeye/apk_decompiling.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3546 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/apk_scanner.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2224 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/cli.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.651265 skyeye-3.5.0/skyeye/config/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      110 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/__init__.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.668358 skyeye-3.5.0/skyeye/config/__pycache__/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      271 2023-04-24 06:34:57.000000 skyeye-3.5.0/skyeye/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      182 2023-05-16 07:51:28.000000 skyeye-3.5.0/skyeye/config/__pycache__/cli_config.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1288 2023-04-24 06:34:57.000000 skyeye-3.5.0/skyeye/config/__pycache__/config_center.cpython-310.pyc
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1278692 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/baksmali-2.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       39 2023-05-16 07:51:12.000000 skyeye-3.5.0/skyeye/config/cli_config.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      803 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/config_center.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.783524 skyeye-3.5.0/skyeye/config/dex-tools-2.1/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    11562 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/LICENSE.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      341 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/NOTICE.txt
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.785832 skyeye-3.5.0/skyeye/config/dex-tools-2.1/bin/
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     3277 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/bin/dex-tools.bat
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-baksmali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-baksmali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      845 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1371 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      843 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1369 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      847 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1373 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-access.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-access.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      839 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1365 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      834 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1360 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      837 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1363 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      831 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-smali.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1357 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-smali.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      836 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-std-apk.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1362 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-std-apk.sh
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      326 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j_invoke.bat
+-rwxr-xr-x   0 wangshuwen15222   (501) staff       (20)     1321 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j_invoke.sh
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.873938 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   239543 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1153819 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   167761 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1543336 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   374032 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   378662 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    17737 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174246 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   196809 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   237496 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    72149 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    76796 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   174252 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   108508 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)   104543 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  1030064 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3210 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/open-source-license.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)    25515 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)  3238491 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/config/jd-gui-1.6.6.jar
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.879491 skyeye-3.5.0/skyeye/dto/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      104 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/dto/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      923 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/dto/class_desc_dto.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      592 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/dto/config_dto.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.883793 skyeye-3.5.0/skyeye/parse/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      122 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/parse/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     5107 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/parse/method_block_parser.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3742 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/parse/smali_parser.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     1858 2023-04-24 11:43:33.000000 skyeye-3.5.0/skyeye/result_wirter.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.886122 skyeye-3.5.0/skyeye/utils/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       58 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/utils/__init__.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       85 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/utils/string_util.py
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)      782 2023-04-12 07:13:48.000000 skyeye-3.5.0/skyeye/version_check.py
+drwxr-xr-x   0 wangshuwen15222   (501) staff       (20)        0 2023-05-16 07:53:12.624440 skyeye-3.5.0/skyeye.egg-info/
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     2140 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/PKG-INFO
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)     3558 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/SOURCES.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/dependency_links.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       42 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/entry_points.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)       16 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/requires.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        7 2023-05-16 07:53:12.000000 skyeye-3.5.0/skyeye.egg-info/top_level.txt
+-rw-r--r--   0 wangshuwen15222   (501) staff       (20)        1 2023-04-24 06:40:26.000000 skyeye-3.5.0/skyeye.egg-info/zip-safe
```

### Comparing `skyeye-3.4.9/PKG-INFO` & `skyeye-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyeye
-Version: 3.4.9
+Version: 3.5.0
 Summary: APK扫描工具
 Home-page: https://github.com/wangshuwen1107/skyeye
 Author: wangshuwen
 Author-email: wnwn7375@outlook.com
 License: MIT
 Keywords: apk scanner
 Description-Content-Type: text/markdown
```

### Comparing `skyeye-3.4.9/README.md` & `skyeye-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/setup.py` & `skyeye-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/apk_decompiling.py` & `skyeye-3.5.0/skyeye/apk_decompiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,17 @@
     if not os.path.exists(dexPath):
         return ""
     (dexName,_) = os.path.splitext(dexPath)
     current_file_dir = os.path.dirname(__file__)
     dexDir = os.path.dirname(dexPath)
     jarPath = os.path.join(dexDir,dexName+".jar")
     dex2JarShPath=  os.path.join(current_file_dir,'config/dex-tools-2.1/d2j-dex2jar.sh')
-    d2jInvokeShPath=  os.path.join(current_file_dir,'config/dex-tools-2.1/d2j_invoke.sh')
-    command ="sudo chmod +x "+d2jInvokeShPath+"&& sh "+ dex2JarShPath+" "+dexPath+" -o "+jarPath+" --force"     
+    # d2jInvokeShPath=  os.path.join(current_file_dir,'config/dex-tools-2.1/d2j_invoke.sh')
+    # command ="sudo chmod +x "+d2jInvokeShPath+"&& sh "+ dex2JarShPath+" "+dexPath+" -o "+jarPath+" --force"
+    command ="sh "+ dex2JarShPath+" "+dexPath+" -o "+jarPath+" --force"     
     commandResult = os.popen(command).readlines()      
     return jarPath
     
 def delFiles(filePath):
     if os.path.exists(filePath):
        print("正在删除->"+filePath)
        if os.path.isdir(filePath):
```

### Comparing `skyeye-3.4.9/skyeye/apk_scanner.py` & `skyeye-3.5.0/skyeye/apk_scanner.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/cli.py` & `skyeye-3.5.0/skyeye/cli.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/__pycache__/config_center.cpython-310.pyc` & `skyeye-3.5.0/skyeye/config/__pycache__/config_center.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/baksmali-2.5.2.jar` & `skyeye-3.5.0/skyeye/config/baksmali-2.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/config_center.py` & `skyeye-3.5.0/skyeye/config/config_center.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/LICENSE.txt` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/bin/dex-tools.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/bin/dex-tools.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-apk-sign.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-apk-sign.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-asm-verify.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-asm-verify.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-baksmali.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-baksmali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-baksmali.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-baksmali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-class-version-switch.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-class-version-switch.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-decrypt-string.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-decrypt-string.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-recompute-checksum.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-weaver.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex-weaver.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2jar.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2jar.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2smali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-dex2smali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-access.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-access.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-access.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-access.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-weaver.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar-weaver.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2dex.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2dex.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jar2jasmin.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-jasmin2jar.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-smali.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-smali.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-smali.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-smali.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-std-apk.bat` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-std-apk.bat`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j-std-apk.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j-std-apk.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/d2j_invoke.sh` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/d2j_invoke.sh`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/ST4-4.0.8.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr-3.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr-runtime-3.5.2.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr4-4.5.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/antlr4-runtime-4.5.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/asm-debug-all-5.0.3.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-base-cmd-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-jasmin-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/d2j-smali-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-ir-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-reader-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-reader-api-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-tools-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-translator-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dex-writer-2.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/dx-27.0.3.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/open-source-license.txt` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/open-source-license.txt`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar` & `skyeye-3.5.0/skyeye/config/dex-tools-2.1/lib/org.abego.treelayout.core-1.0.1.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/config/jd-gui-1.6.6.jar` & `skyeye-3.5.0/skyeye/config/jd-gui-1.6.6.jar`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/dto/class_desc_dto.py` & `skyeye-3.5.0/skyeye/dto/class_desc_dto.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/dto/config_dto.py` & `skyeye-3.5.0/skyeye/dto/config_dto.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/parse/method_block_parser.py` & `skyeye-3.5.0/skyeye/parse/method_block_parser.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/parse/smali_parser.py` & `skyeye-3.5.0/skyeye/parse/smali_parser.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/result_wirter.py` & `skyeye-3.5.0/skyeye/result_wirter.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye/version_check.py` & `skyeye-3.5.0/skyeye/version_check.py`

 * *Files identical despite different names*

### Comparing `skyeye-3.4.9/skyeye.egg-info/PKG-INFO` & `skyeye-3.5.0/skyeye.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyeye
-Version: 3.4.9
+Version: 3.5.0
 Summary: APK扫描工具
 Home-page: https://github.com/wangshuwen1107/skyeye
 Author: wangshuwen
 Author-email: wnwn7375@outlook.com
 License: MIT
 Keywords: apk scanner
 Description-Content-Type: text/markdown
```

### Comparing `skyeye-3.4.9/skyeye.egg-info/SOURCES.txt` & `skyeye-3.5.0/skyeye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

