# Comparing `tmp/azureml-assets-0.0.1.tar.gz` & `tmp/azureml-assets-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-0.0.1.tar", last modified: Sat May  6 13:20:38 2023, max compression
+gzip compressed data, was "azureml-assets-1.0.0.tar", last modified: Tue May 16 20:28:07 2023, max compression
```

## Comparing `azureml-assets-0.0.1.tar` & `azureml-assets-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,37 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-05-06 13:20:38.396550 azureml-assets-0.0.1/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 azureml-assets-0.0.1/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 azureml-assets-0.0.1/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      868 2023-05-06 13:20:38.396605 azureml-assets-0.0.1/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)        0 2022-10-14 17:54:03.000000 azureml-assets-0.0.1/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-05-06 13:20:38.395219 azureml-assets-0.0.1/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 azureml-assets-0.0.1/data/data_file
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 azureml-assets-0.0.1/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2023-05-06 13:20:38.396830 azureml-assets-0.0.1/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)     8489 2023-05-06 13:20:27.000000 azureml-assets-0.0.1/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-05-06 13:20:38.394108 azureml-assets-0.0.1/src/
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-05-06 13:20:38.396169 azureml-assets-0.0.1/src/azureml_assets.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      868 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      357 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)       39 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/entry_points.txt
--rw-r--r--   0 kotko      (501) staff       (20)       77 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2023-05-06 13:20:38.000000 azureml-assets-0.0.1/src/azureml_assets.egg-info/top_level.txt
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-05-06 13:20:38.396306 azureml-assets-0.0.1/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 azureml-assets-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.464835 azureml-assets-1.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.456835 azureml-assets-1.0.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      609 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3788 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35954 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4737 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/copy_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15375 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4773 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10152 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15082 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-16 20:28:07.460835 azureml-assets-1.0.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      618 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      943 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-05-16 20:28:07.000000 azureml-assets-1.0.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-16 20:28:07.464835 azureml-assets-1.0.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      954 2023-05-16 20:27:33.000000 azureml-assets-1.0.0/setup.py
```

