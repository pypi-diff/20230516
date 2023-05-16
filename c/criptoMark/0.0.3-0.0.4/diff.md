# Comparing `tmp/criptoMark-0.0.3.tar.gz` & `tmp/criptoMark-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criptoMark-0.0.3.tar", last modified: Mon May 15 23:53:05 2023, max compression
+gzip compressed data, was "criptoMark-0.0.4.tar", last modified: Tue May 16 00:09:51 2023, max compression
```

## Comparing `criptoMark-0.0.3.tar` & `criptoMark-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.641227 criptoMark-0.0.3/
--rw-rw-rw-   0        0        0      504 2023-05-15 23:53:05.640227 criptoMark-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.611200 criptoMark-0.0.3/criptoMark/
--rw-rw-rw-   0        0        0       54 2023-05-15 23:51:27.000000 criptoMark-0.0.3/criptoMark/__init__.py
--rw-rw-rw-   0        0        0     1018 2023-05-15 23:51:30.000000 criptoMark-0.0.3/criptoMark/get_supported.py
-drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.638224 criptoMark-0.0.3/criptoMark.egg-info/
--rw-rw-rw-   0        0        0      504 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 23:53:05.641227 criptoMark-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-05-15 23:51:47.000000 criptoMark-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.505587 criptoMark-0.0.4/
+-rw-rw-rw-   0        0        0      504 2023-05-16 00:09:51.504747 criptoMark-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.490575 criptoMark-0.0.4/criptoMark/
+-rw-rw-rw-   0        0        0        0 2023-05-16 00:05:35.000000 criptoMark-0.0.4/criptoMark/__init__.py
+-rw-rw-rw-   0        0        0     6990 2023-05-16 00:05:52.000000 criptoMark-0.0.4/criptoMark/requisicaocripto.py
+drwxrwxrwx   0        0        0        0 2023-05-16 00:09:51.500586 criptoMark-0.0.4/criptoMark.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 00:09:51.000000 criptoMark-0.0.4/criptoMark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 00:09:51.505587 criptoMark-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-05-16 00:09:43.000000 criptoMark-0.0.4/setup.py
```

### Comparing `criptoMark-0.0.3/setup.py` & `criptoMark-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'Pacote de consultas'
 LONG_DESCRIPTION = 'Pacote de Consultas de cripto'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="criptoMark",
```

