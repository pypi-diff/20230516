# Comparing `tmp/pytest_ogsm_plugin-3.5.1.tar.gz` & `tmp/pytest_ogsm_plugin-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ogsm_plugin-3.5.1.tar", last modified: Mon Apr 24 11:11:58 2023, max compression
+gzip compressed data, was "pytest_ogsm_plugin-3.5.2.tar", last modified: Tue May 16 09:43:51 2023, max compression
```

## Comparing `pytest_ogsm_plugin-3.5.1.tar` & `pytest_ogsm_plugin-3.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.108127 pytest_ogsm_plugin-3.5.1/
--rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-24 11:11:58.107472 pytest_ogsm_plugin-3.5.1/PKG-INFO
--rw-r--r--   0 taocw      (501) staff       (20)      565 2022-11-15 10:00:14.000000 pytest_ogsm_plugin-3.5.1/README.md
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.081063 pytest_ogsm_plugin-3.5.1/gic2api/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:34.000000 pytest_ogsm_plugin-3.5.1/gic2api/__init__.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.082712 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:47.000000 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)     1132 2023-02-16 08:42:54.000000 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/test_gic2_lvs.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.084483 pytest_ogsm_plugin-3.5.1/openapi/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:24.000000 pytest_ogsm_plugin-3.5.1/openapi/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)      213 2023-01-09 05:39:17.000000 pytest_ogsm_plugin-3.5.1/openapi/com.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.086812 pytest_ogsm_plugin-3.5.1/openapi/inpaas/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:37.000000 pytest_ogsm_plugin-3.5.1/openapi/inpaas/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)     1453 2023-03-02 06:38:49.000000 pytest_ogsm_plugin-3.5.1/openapi/inpaas/test_haproxy.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.088855 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/
--rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:20:25.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)    10112 2023-04-24 11:09:11.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/pytest_ogsm.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.093203 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/
--rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:21:06.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)    28151 2023-03-06 05:38:56.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/templates.html
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.101516 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/
--rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 taocw      (501) staff       (20)      622 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 taocw      (501) staff       (20)        1 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 taocw      (501) staff       (20)       55 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/entry_points.txt
--rw-r--r--   0 taocw      (501) staff       (20)       14 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/requires.txt
--rw-r--r--   0 taocw      (501) staff       (20)       39 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/top_level.txt
--rw-r--r--   0 taocw      (501) staff       (20)       38 2023-04-24 11:11:58.108420 pytest_ogsm_plugin-3.5.1/setup.cfg
--rw-r--r--   0 taocw      (501) staff       (20)     1196 2023-04-24 11:09:38.000000 pytest_ogsm_plugin-3.5.1/setup.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.104357 pytest_ogsm_plugin-3.5.1/tests/
--rw-r--r--   0 taocw      (501) staff       (20)       94 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.1/tests/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)      124 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.1/tests/conftest.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.298857 pytest_ogsm_plugin-3.5.2/
+-rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-05-16 09:43:51.298547 pytest_ogsm_plugin-3.5.2/PKG-INFO
+-rw-r--r--   0 taocw      (501) staff       (20)      565 2022-11-15 10:00:14.000000 pytest_ogsm_plugin-3.5.2/README.md
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.286541 pytest_ogsm_plugin-3.5.2/gic2api/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:34.000000 pytest_ogsm_plugin-3.5.2/gic2api/__init__.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.287919 pytest_ogsm_plugin-3.5.2/gic2api/inpaas/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:47.000000 pytest_ogsm_plugin-3.5.2/gic2api/inpaas/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)     1132 2023-02-16 08:42:54.000000 pytest_ogsm_plugin-3.5.2/gic2api/inpaas/test_gic2_lvs.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.289309 pytest_ogsm_plugin-3.5.2/openapi/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:24.000000 pytest_ogsm_plugin-3.5.2/openapi/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)      213 2023-01-09 05:39:17.000000 pytest_ogsm_plugin-3.5.2/openapi/com.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.290636 pytest_ogsm_plugin-3.5.2/openapi/inpaas/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:37.000000 pytest_ogsm_plugin-3.5.2/openapi/inpaas/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)     1453 2023-03-02 06:38:49.000000 pytest_ogsm_plugin-3.5.2/openapi/inpaas/test_haproxy.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.291957 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/
+-rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:20:25.000000 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)    10131 2023-05-16 09:43:40.000000 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/pytest_ogsm.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.293187 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/templates/
+-rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:21:06.000000 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/templates/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)    28151 2023-03-06 05:38:56.000000 pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/templates/templates.html
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.296613 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/
+-rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 taocw      (501) staff       (20)      622 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 taocw      (501) staff       (20)        1 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       55 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       14 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/requires.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       39 2023-05-16 09:43:51.000000 pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       38 2023-05-16 09:43:51.298965 pytest_ogsm_plugin-3.5.2/setup.cfg
+-rw-r--r--   0 taocw      (501) staff       (20)     1196 2023-05-16 09:43:40.000000 pytest_ogsm_plugin-3.5.2/setup.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-05-16 09:43:51.297684 pytest_ogsm_plugin-3.5.2/tests/
+-rw-r--r--   0 taocw      (501) staff       (20)       94 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.2/tests/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)      124 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.2/tests/conftest.py
```

### Comparing `pytest_ogsm_plugin-3.5.1/PKG-INFO` & `pytest_ogsm_plugin-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_ogsm_plugin
-Version: 3.5.1
+Version: 3.5.2
 Summary: 针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数
 Home-page: https://github.com/cw010/pytest_ogsm_plugin
 Author: cw
 Author-email: cwalk.t@gmail.com
 License: proprietary
 Keywords: pytest,py.test,pytest_ogsm_plugin
 Platform: UNKNOWN
```

### Comparing `pytest_ogsm_plugin-3.5.1/README.md` & `pytest_ogsm_plugin-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.1/gic2api/inpaas/test_gic2_lvs.py` & `pytest_ogsm_plugin-3.5.2/gic2api/inpaas/test_gic2_lvs.py`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.1/openapi/inpaas/test_haproxy.py` & `pytest_ogsm_plugin-3.5.2/openapi/inpaas/test_haproxy.py`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/pytest_ogsm.py` & `pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/pytest_ogsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     report.desc = item._obj.__doc__
     report.method = item.location[2].split('[')[0]
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("testreport")
     project_choices_value = ['all', 'openapi', 'gic2api', 'ui']
-    product_choices_value = ['all', 'inpaas', 'mongodb', 'ccs', 'bms', 'k8s', 'kafka',
+    product_choices_value = ['all', 'mysql', 'redis', 'haproxy', 'mongodb', 'ccs', 'bms', 'k8s', 'kafka',
                              'ecs_vm', 'nas', 'ebs', 'sec',
                              'vdc', 'vpc', 'platform', 'monitor', 'oss', 'cdn']
     group.addoption(
         "--report",
         action="store",
         metavar="path",
         default=None,
```

### Comparing `pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/templates.html` & `pytest_ogsm_plugin-3.5.2/pytestOGSMplugin/templates/templates.html`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/PKG-INFO` & `pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ogsm-plugin
-Version: 3.5.1
+Version: 3.5.2
 Summary: 针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数
 Home-page: https://github.com/cw010/pytest_ogsm_plugin
 Author: cw
 Author-email: cwalk.t@gmail.com
 License: proprietary
 Keywords: pytest,py.test,pytest_ogsm_plugin
 Platform: UNKNOWN
```

### Comparing `pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/SOURCES.txt` & `pytest_ogsm_plugin-3.5.2/pytest_ogsm_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.1/setup.py` & `pytest_ogsm_plugin-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest_ogsm_plugin',
     url='https://github.com/cw010/pytest_ogsm_plugin',
-    version='3.5.1',
+    version='3.5.2',
     author="cw",
     author_email='cwalk.t@gmail.com',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     description='针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数',
     classifiers=[
         'Framework :: Pytest',
```

