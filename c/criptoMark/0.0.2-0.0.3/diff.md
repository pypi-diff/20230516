# Comparing `tmp/criptoMark-0.0.2.tar.gz` & `tmp/criptoMark-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criptoMark-0.0.2.tar", last modified: Mon May 15 22:59:05 2023, max compression
+gzip compressed data, was "criptoMark-0.0.3.tar", last modified: Mon May 15 23:53:05 2023, max compression
```

## Comparing `criptoMark-0.0.2.tar` & `criptoMark-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 22:59:05.125112 criptoMark-0.0.2/
--rw-rw-rw-   0        0        0      504 2023-05-15 22:59:05.125112 criptoMark-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 22:59:05.111109 criptoMark-0.0.2/criptoMark/
--rw-rw-rw-   0        0        0       69 2023-05-15 22:47:15.000000 criptoMark-0.0.2/criptoMark/__init__.py
--rw-rw-rw-   0        0        0     1035 2023-05-15 22:44:48.000000 criptoMark-0.0.2/criptoMark/get_supported_future_markets.py
-drwxrwxrwx   0        0        0        0 2023-05-15 22:59:05.122119 criptoMark-0.0.2/criptoMark.egg-info/
--rw-rw-rw-   0        0        0      504 2023-05-15 22:59:04.000000 criptoMark-0.0.2/criptoMark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-15 22:59:05.000000 criptoMark-0.0.2/criptoMark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 22:59:04.000000 criptoMark-0.0.2/criptoMark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 22:59:04.000000 criptoMark-0.0.2/criptoMark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 22:59:05.126123 criptoMark-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-05-15 22:59:01.000000 criptoMark-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.641227 criptoMark-0.0.3/
+-rw-rw-rw-   0        0        0      504 2023-05-15 23:53:05.640227 criptoMark-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.611200 criptoMark-0.0.3/criptoMark/
+-rw-rw-rw-   0        0        0       54 2023-05-15 23:51:27.000000 criptoMark-0.0.3/criptoMark/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-05-15 23:51:30.000000 criptoMark-0.0.3/criptoMark/get_supported.py
+drwxrwxrwx   0        0        0        0 2023-05-15 23:53:05.638224 criptoMark-0.0.3/criptoMark.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 23:53:05.000000 criptoMark-0.0.3/criptoMark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 23:53:05.641227 criptoMark-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-05-15 23:51:47.000000 criptoMark-0.0.3/setup.py
```

### Comparing `criptoMark-0.0.2/criptoMark/get_supported_future_markets.py` & `criptoMark-0.0.3/criptoMark/get_supported.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import requests
 def get_supported_future_markets():
    """Parametros:
       ----------
                   `Sem parametros`
```

### Comparing `criptoMark-0.0.2/setup.py` & `criptoMark-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'Pacote de consultas'
 LONG_DESCRIPTION = 'Pacote de Consultas de cripto'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="criptoMark",
```

