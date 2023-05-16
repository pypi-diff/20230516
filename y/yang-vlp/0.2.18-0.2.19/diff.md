# Comparing `tmp/yang-vlp-0.2.18.tar.gz` & `tmp/yang-vlp-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-hg13a9na\yang-vlp-0.2.18.tar", last modified: Tue May  9 11:45:53 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-de3eu8l2\yang-vlp-0.2.19.tar", last modified: Tue May 16 07:20:44 2023, max compression
```

## Comparing `yang-vlp-0.2.18.tar` & `yang-vlp-0.2.19.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.635440 yang-vlp-0.2.18/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.18/LICENSE
--rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.18/MANIFEST.in
--rw-rw-rw-   0        0        0     2686 2023-05-09 11:45:53.634439 yang-vlp-0.2.18/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-06 06:53:58.000000 yang-vlp-0.2.18/README.md
--rw-rw-rw-   0        0        0      639 2023-05-09 11:44:59.000000 yang-vlp-0.2.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 11:45:53.635440 yang-vlp-0.2.18/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-09 11:45:04.000000 yang-vlp-0.2.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.406656 yang-vlp-0.2.18/vlppy/
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.409620 yang-vlp-0.2.18/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.18/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.18/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.18/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.424621 yang-vlp-0.2.18/vlppy/demo/
--rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.18/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.18/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.445620 yang-vlp-0.2.18/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.18/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.18/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.18/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.18/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.18/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     3096 2023-05-09 01:51:31.000000 yang-vlp-0.2.18/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.461620 yang-vlp-0.2.18/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.18/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.18/vlppy/error/error.py
--rw-rw-rw-   0        0        0      108 2023-05-09 11:44:52.000000 yang-vlp-0.2.18/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.466626 yang-vlp-0.2.18/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.18/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.18/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.478623 yang-vlp-0.2.18/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.18/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.539370 yang-vlp-0.2.18/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.18/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.18/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.18/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.18/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.18/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6177 2023-05-09 02:19:05.000000 yang-vlp-0.2.18/vlppy/model/led.py
--rw-rw-rw-   0        0        0    17602 2023-05-09 11:44:20.000000 yang-vlp-0.2.18/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17673 2023-05-06 06:55:51.000000 yang-vlp-0.2.18/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.558396 yang-vlp-0.2.18/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.18/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.582400 yang-vlp-0.2.18/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.18/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.18/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.18/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.18/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.605468 yang-vlp-0.2.18/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.18/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.18/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.18/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.610430 yang-vlp-0.2.18/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.18/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.18/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.616445 yang-vlp-0.2.18/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.18/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.18/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-09 11:45:53.631440 yang-vlp-0.2.18/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2686 2023-05-09 11:45:53.000000 yang-vlp-0.2.18/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-05-09 11:45:53.000000 yang-vlp-0.2.18/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 11:45:53.000000 yang-vlp-0.2.18/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-09 11:45:53.000000 yang-vlp-0.2.18/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 11:45:53.000000 yang-vlp-0.2.18/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.891974 yang-vlp-0.2.19/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.19/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.19/MANIFEST.in
+-rw-rw-rw-   0        0        0     2686 2023-05-16 07:20:44.890979 yang-vlp-0.2.19/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-06 06:53:58.000000 yang-vlp-0.2.19/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-09 12:15:04.000000 yang-vlp-0.2.19/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:20:44.891974 yang-vlp-0.2.19/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-09 12:15:10.000000 yang-vlp-0.2.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.700493 yang-vlp-0.2.19/vlppy/
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.704475 yang-vlp-0.2.19/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.19/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.19/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.19/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.721475 yang-vlp-0.2.19/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.19/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.19/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.730473 yang-vlp-0.2.19/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.19/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.19/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     2950 2023-05-16 06:59:59.000000 yang-vlp-0.2.19/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.738497 yang-vlp-0.2.19/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.19/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.19/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      108 2023-05-09 12:14:50.000000 yang-vlp-0.2.19/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.743473 yang-vlp-0.2.19/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.19/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.19/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.799613 yang-vlp-0.2.19/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.19/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.816477 yang-vlp-0.2.19/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6303 2023-05-16 07:19:55.000000 yang-vlp-0.2.19/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    18199 2023-05-16 07:07:32.000000 yang-vlp-0.2.19/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    17948 2023-05-16 06:59:05.000000 yang-vlp-0.2.19/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.841688 yang-vlp-0.2.19/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.19/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.846675 yang-vlp-0.2.19/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.19/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.19/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.19/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.856676 yang-vlp-0.2.19/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.19/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.19/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.19/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.861698 yang-vlp-0.2.19/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.19/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.19/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.868682 yang-vlp-0.2.19/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.19/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.19/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.885991 yang-vlp-0.2.19/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2686 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.18/LICENSE` & `yang-vlp-0.2.19/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/PKG-INFO` & `yang-vlp-0.2.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.18
+Version: 0.2.19
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.18/README.md` & `yang-vlp-0.2.19/README.md`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/pyproject.toml` & `yang-vlp-0.2.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.18"
+version = "0.2.19"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `yang-vlp-0.2.18/setup.py` & `yang-vlp-0.2.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.18',  #版本号
+    version = '0.2.19',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `yang-vlp-0.2.18/vlppy/LICENSE.txt` & `yang-vlp-0.2.19/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.19/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/demo/demo_main.py` & `yang-vlp-0.2.19/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.19/vlppy/demo/vlp_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,16 +42,17 @@
         """
         # PD接收各LED的信号 (l*w*h)
         P_PD1 = self.pd1.recv_led_signal(led=self.led1, room=self.room) 
         P_PD2 = self.pd2.recv_led_signal(led=self.led1, room=self.room)
         P_PD3 = self.pd3.recv_led_signal(led=self.led1, room=self.room) 
         P_PD4 = self.pd4.recv_led_signal(led=self.led1, room=self.room) 
 
-        xr, yr, zr = np.split(self.room.tp_pos, indices_or_sections=3, axis=-1) # 在最后一个维度上进行分割操作#（l*w*h,3） -> 3*（l*w*h,1)
-        Xr, Yr, Zr = xr.flatten(), yr.flatten(), zr.flatten()  #（l*w*h）
+        # 参考点
+        Xr, Yr, Zr = self.room.tp_raw_pos  #（l*w*h）
+        
         return (P_PD1,P_PD2,P_PD3,P_PD4,Xr,Yr,Zr)  
       
     def show(self,z,savepath=...,showfig=True):
         """绘图
         z: 第三维度数据
         """
         xr, yr, _ = self.room.tp_grid
```

### Comparing `yang-vlp-0.2.18/vlppy/error/error.py` & `yang-vlp-0.2.19/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/io/io.py` & `yang-vlp-0.2.19/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/model/led.py` & `yang-vlp-0.2.19/vlppy/model/led.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,32 +142,36 @@
         return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
         pos = np.asarray(pos)
-        if not pos.shape[-1] == 3:
-            raise VLPSequenceLenError(pos.shape[-1],3)
-        self._pos = np.asarray(pos)
+        assert len(pos) == 3 or pos.shape[-1] == 3
+        if len(pos) == 3:
+            xr,yr,zr = pos
+            pos = np.stack([xr,yr,zr], axis=-1)
+        self._pos = pos # (3)
         
     @property
     def Nv(self):  
         """获取LED法向量  
         """  
         return self._Nv
 
     @Nv.setter
     def Nv(self, n): 
         """设置LED法向量 
         """
-        n = np.asarray(n)
-        if not n.shape[-1] == 3:
-            raise VLPSequenceLenError(n,3)
-        self._Nv = n
+        N = np.asarray(n)
+        assert len(n) == 3 or n.shape[-1] == 3
+        if len(n) == 3:
+            Nx,Ny,Nz = N
+            N = np.stack([Nx,Ny,Nz], axis=-1)
+        self._Nv = N
 
     @property
     def theta(self):  
         """获取半功率点半角 (单位: 度)  
         """  
         return self._theta
```

### Comparing `yang-vlp-0.2.18/vlppy/model/pd.py` & `yang-vlp-0.2.19/vlppy/model/pd.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,71 +42,89 @@
             alpha: PD摆放角(单位:度)
             beta: PD倾斜面倾斜角(单位:度)
             center_tp_pos: 水平中心测试点位置
         Return
             pos: 倾斜PD位置
             Nv: 倾斜PD的法向量
         """
-        x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
+        if len(center_tp_pos) == 3:
+            x0, y0, z0 = center_tp_pos
+        else:
+            x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
         x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
 
-        # 倾斜PD的方位角和倾斜角,角度制转弧度制
+        # 角度制转弧度制
         alpha_rad, beta_rad = np.radians([alpha, beta])
 
+        # 倾斜PD和中心参考点位置关系
         xr = x0 + l * np.cos(alpha_rad) * np.cos(beta_rad) 
         yr = y0 + l * np.sin(alpha_rad) * np.cos(beta_rad)
         zr = z0 + l * np.sin(beta_rad)
-        pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
         
         # alpha_rad+np.pi: PD的方位角和PD倾斜面的摆放角反向
         # beta_rad: PD的法向量与z轴的夹角和PD倾斜面的倾斜角相等
         Nx = np.cos(alpha_rad+np.pi) * np.sin(beta_rad)
         Ny = np.sin(alpha_rad+np.pi) * np.sin(beta_rad)
         Nz = np.cos(beta_rad)
-        Nv = np.stack([Nx,Ny,Nz],axis=-1) 
 
+        if len(center_tp_pos) == 3:
+            pos = (xr,yr,zr)
+            Nv = (Nx,Ny,Nz)
+        else:
+            pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
+            Nv = np.stack([Nx,Ny,Nz], axis=-1)
+        
         return pos, Nv
 
     @staticmethod
     def recv_surface_model(r:Union[Number,tuple], alpha, beta, center_tp_pos:tuple):
         """接收机模型:安全帽椭球面(倾斜PD和中心参考点位置关系)
         Params
             r: 曲球面半径(单位:米)
-            alpha:PD摆放角(单位:度)
-            beta: PD倾斜面倾斜角(单位:度)
+            alpha: PD摆放角(单位:度)
+            beta: 椭球球心与PD连线与z轴夹角(单位:度)
             center_tp_pos: 椭球面顶部中心测试点位置
         Return
             pos: 倾斜PD位置
             Nv: 倾斜PD的法向量
         """
         r = np.asarray(r)
         assert r.size in (1,3)
         a, b, c = np.full(shape=(3), fill_value=r) if r.size == 1 else r
 
-        # 倾斜PD的方位角和倾斜角
-        alpha_rad, beta_rad = np.radians([alpha,beta]) # 角度制转弧度制
+        # 角度制转弧度制
+        alpha_rad, beta_rad = np.radians([alpha,beta]) 
 
         if not 0 <= beta_rad <= 90: # 限定
             raise VLPValueRangeError(beta, 0, 90)
         
-        x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
+        if len(center_tp_pos) == 3:
+            x0, y0, z0 = center_tp_pos
+        else:
+            x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
         x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
-
+        
         # 倾斜PD位置
         xr = x0 + a * np.cos(alpha_rad) * np.sin(beta_rad)
         yr = y0 + b * np.sin(alpha_rad) * np.sin(beta_rad)
         zr = z0 - c * (1 - np.cos(beta_rad))
-        pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
 
         # alpha_rad: PD的方位角和PD倾斜面的摆放角相等
-        # beta_rad: PD的法向量与z轴的夹角和PD倾斜面的倾斜角相等
+        # beta_rad: 椭球球心与PD连线与z轴夹角
         Nx = 1/a * np.cos(alpha_rad) * np.sin(beta_rad)
         Ny = 1/b * np.sin(alpha_rad) * np.sin(beta_rad)
         Nz = 1/c * np.cos(beta_rad)
-        Nv = np.stack([Nx,Ny,Nz],axis=-1)
+
+        # PD位置与法向量
+        if len(center_tp_pos) == 3:
+            pos = (xr,yr,zr)
+            Nv = (Nx,Ny,Nz)
+        else:
+            pos = np.stack([xr,yr,zr], axis=-1)
+            Nv = np.stack([Nx,Ny,Nz], axis=-1)
 
         return pos, Nv
 
     @staticmethod
     def recv_hemisphere_model(r, l, alpha, center_tp_pos:tuple):
         """接收机模型:半球面模型(倾斜PD和中心参考点位置关系)
         Params
@@ -115,15 +133,15 @@
             alpha:倾斜PD方位角(单位:度) 
             center_tp_pos: 测试点位置 
         Return
             pos: 倾斜PD位置
             Nv: 倾斜PD的法向量
         """
         # 倾斜PD的方位角和倾斜角
-        beta_rad = l/r   # PD倾斜角
+        beta_rad = l/r   # 椭球球心与PD连线与z轴夹角(PD倾斜角)
         beta = np.degrees(beta_rad) # 弧度制转角度制
         pos, Nv = PD.recv_surface_model(r, alpha, beta, center_tp_pos)
         return pos, Nv
 
     def recv_led_radiation_intensity(self, led:LED):
         """计算LED辐射强度(LOS链路):
         Parameters
@@ -334,30 +352,34 @@
         return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
         pos = np.asarray(pos)
-        if not pos.shape[-1] == 3:
-            raise VLPSequenceLenError(pos.shape[-1],3)
-        self._pos = np.asarray(pos)
+        assert len(pos) == 3 or pos.shape[-1] == 3
+        if len(pos) == 3:
+            xr,yr,zr = pos
+            pos = np.stack([xr,yr,zr], axis=-1)
+        self._pos = pos # (L*w*h,3)
 
     @property
     def Nv(self):  
         """获取PD法向量  
         """  
         return self._Nv
     
     @Nv.setter
     def Nv(self, n):
-        n = np.asarray(n)
-        if not n.shape[-1] == 3:
-            raise VLPSequenceLenError(n,3)
-        self._Nv = n
+        N = np.asarray(n)
+        assert len(n) == 3 or n.shape[-1] == 3
+        if len(n) == 3:
+            Nx,Ny,Nz = N
+            N = np.stack([Nx,Ny,Nz], axis=-1)
+        self._Nv = N
 
     @property
     def fov(self):
         """获取接收视场角 (单位: 度)
         """    
         return self._fov
```

### Comparing `yang-vlp-0.2.18/vlppy/model/room.py` & `yang-vlp-0.2.19/vlppy/model/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,14 +324,23 @@
         """获取测试点位置
         """
         xr, yr, zr = self.tp_grid
         pos = np.stack([xr,yr,zr], axis=-1)
         return pos
 
     @property
+    def tp_raw_pos(self) -> tuple:
+        """获取测试点位置
+            shape:(l*w*h)、(l*w*h)、(l*w*h)
+        """
+        xr, yr, zr = self.tp_grid
+        xr, yr, zr = xr.flatten(), yr.flatten(), zr.flatten()
+        return (xr, yr, zr) 
+
+    @property
     def wall_gap(self):
         """获取墙壁划分网格的间隔 
         """
         return self._wall_gap
     
     @wall_gap.setter
     def wall_gap(self, gap:Union[Number, Sequence]):
```

### Comparing `yang-vlp-0.2.18/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.19/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/setting/json_setting.py` & `yang-vlp-0.2.19/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/setting/settings.json` & `yang-vlp-0.2.19/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/signal/filter.py` & `yang-vlp-0.2.19/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/signal/plot.py` & `yang-vlp-0.2.19/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/vlppy/vis/vis.py` & `yang-vlp-0.2.19/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.18/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.19/yang_vlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.18
+Version: 0.2.19
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.18/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.19/yang_vlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

