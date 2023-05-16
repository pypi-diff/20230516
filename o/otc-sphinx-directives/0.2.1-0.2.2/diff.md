# Comparing `tmp/otc_sphinx_directives-0.2.1.tar.gz` & `tmp/otc_sphinx_directives-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otc_sphinx_directives-0.2.1.tar", last modified: Tue May 16 07:46:59 2023, max compression
+gzip compressed data, was "otc_sphinx_directives-0.2.2.tar", last modified: Tue May 16 09:15:08 2023, max compression
```

## Comparing `otc_sphinx_directives-0.2.1.tar` & `otc_sphinx_directives-0.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.916083 otc_sphinx_directives-0.2.1/
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/.stestr.conf
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-16 07:46:59.916083 otc_sphinx_directives-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.913083 otc_sphinx_directives-0.2.1/doc/
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.913083 otc_sphinx_directives-0.2.1/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.913083 otc_sphinx_directives-0.2.1/doc/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/_static/.placeholder
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.913083 otc_sphinx_directives-0.2.1/doc/source/examples/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/examples/directives_docsportal.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/examples/directives_ecs.rst
--rw-r--r--   0 root         (0) root         (0)     1386 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/examples/directives_obs.rst
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/examples/directives_obs_clean.rst
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/examples/index.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.914083 otc_sphinx_directives-0.2.1/otc_sphinx_directives/
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/container_item.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3002 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/document_navigator.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/navigator.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/otc_sphinx_directives_setup.py
--rw-r--r--   0 root         (0) root         (0)     3321 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_card.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_group.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_navigator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.915083 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.911083 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.916083 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/directive_wrapper/
--rw-r--r--   0 root         (0) root         (0)      791 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.916083 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/service_card/
--rw-r--r--   0 root         (0) root         (0)      791 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/service_card/conf.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/service_card/index.rst
--rw-r--r--   0 root         (0) root         (0)     2330 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/test_directive_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/test_service_card.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 07:46:59.915083 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1523 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 07:46:59.000000 otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      586 2023-05-16 07:46:59.916083 otc_sphinx_directives-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/tox.ini
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-16 07:45:36.000000 otc_sphinx_directives-0.2.1/zuul.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.019431 otc_sphinx_directives-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/.stestr.conf
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-16 09:15:08.019431 otc_sphinx_directives-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.015431 otc_sphinx_directives-0.2.2/doc/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.016431 otc_sphinx_directives-0.2.2/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.016431 otc_sphinx_directives-0.2.2/doc/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/_static/.placeholder
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.016431 otc_sphinx_directives-0.2.2/doc/source/examples/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/examples/directives_docsportal.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/examples/directives_ecs.rst
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/examples/directives_obs.rst
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/examples/directives_obs_clean.rst
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/examples/index.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.017431 otc_sphinx_directives-0.2.2/otc_sphinx_directives/
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/container_item.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3002 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/document_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/navigator.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/otc_sphinx_directives_setup.py
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_card.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_group.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_navigator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.018431 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.014431 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.019431 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/directive_wrapper/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/directive_wrapper/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.019431 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/service_card/
+-rw-r--r--   0 root         (0) root         (0)      791 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/service_card/conf.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/service_card/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/test_directive_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/test_service_card.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:15:08.018431 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-05-16 09:15:08.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 09:15:07.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-16 09:15:08.000000 otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      586 2023-05-16 09:15:08.020431 otc_sphinx_directives-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/tox.ini
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-16 09:13:47.000000 otc_sphinx_directives-0.2.2/zuul.yaml
```

### Comparing `otc_sphinx_directives-0.2.1/ChangeLog` & `otc_sphinx_directives-0.2.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 CHANGES
 =======
 
-0.2.1
+0.2.2
 -----
 
 * Added service\_uri functionality to docsportal startpage (#16)
 
 0.2.0
 -----
```

### Comparing `otc_sphinx_directives-0.2.1/LICENSE` & `otc_sphinx_directives-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/PKG-INFO` & `otc_sphinx_directives-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc_sphinx_directives
-Version: 0.2.1
+Version: 0.2.2
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.1/doc/source/examples/directives_ecs.rst` & `otc_sphinx_directives-0.2.2/doc/source/examples/directives_ecs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/doc/source/examples/directives_obs.rst` & `otc_sphinx_directives-0.2.2/doc/source/examples/directives_obs.rst`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/container_item.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/container_item.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/directive_wrapper.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/document_navigator.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/document_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/navigator.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/otc_sphinx_directives_setup.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/otc_sphinx_directives_setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_card.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_card.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_group.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_group.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/service_navigator.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/service_navigator.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/base.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/base.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/directive_wrapper/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/templates/service_card/conf.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/templates/service_card/conf.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/test_directive_wrapper.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/test_directive_wrapper.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives/tests/test_service_card.py` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives/tests/test_service_card.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/PKG-INFO` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otc-sphinx-directives
-Version: 0.2.1
+Version: 0.2.2
 Summary: Open Telekom Cloud Sphinx Directives
 Home-page: UNKNOWN
 Author: Open Telekom Cloud Ecosystem Squad
 License: UNKNOWN
 Keywords: Sphinx, Sphinx Directives, Open Telekom Cloud
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx
```

### Comparing `otc_sphinx_directives-0.2.1/otc_sphinx_directives.egg-info/SOURCES.txt` & `otc_sphinx_directives-0.2.2/otc_sphinx_directives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/setup.cfg` & `otc_sphinx_directives-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/setup.py` & `otc_sphinx_directives-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `otc_sphinx_directives-0.2.1/tox.ini` & `otc_sphinx_directives-0.2.2/tox.ini`

 * *Files identical despite different names*

