# Comparing `tmp/deploy_django_nginx-1.0.0.tar.gz` & `tmp/deploy_django_nginx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploy_django_nginx-1.0.0.tar", last modified: Tue May 16 07:35:07 2023, max compression
+gzip compressed data, was "deploy_django_nginx-1.0.1.tar", last modified: Tue May 16 07:37:37 2023, max compression
```

## Comparing `deploy_django_nginx-1.0.0.tar` & `deploy_django_nginx-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:35:07.512389 deploy_django_nginx-1.0.0/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       66 2023-05-16 07:11:05.000000 deploy_django_nginx-1.0.0/MANIFEST.in
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1949 2023-05-16 07:35:07.506173 deploy_django_nginx-1.0.0/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      940 2023-05-16 07:27:18.000000 deploy_django_nginx-1.0.0/README.md
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:35:07.365927 deploy_django_nginx-1.0.0/deploy_django_nginx/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      188 2023-05-16 07:13:20.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/__init__.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1594 2023-05-16 02:26:05.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/build.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1715 2023-05-16 05:31:35.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/config.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     3188 2023-05-16 07:32:44.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/main.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      533 2023-05-16 02:26:05.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/setup_cython.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1235 2023-05-16 07:31:55.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/util.py
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      266 2023-05-16 07:09:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx/version.json
-drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:35:07.485127 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1949 2023-05-16 07:35:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/PKG-INFO
--rw-r--r--   0 suqingdong  (1000) disease   (8039)      523 2023-05-16 07:35:07.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/SOURCES.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-05-16 07:35:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/dependency_links.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       56 2023-05-16 07:35:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/entry_points.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       25 2023-05-16 07:35:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/requires.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2023-05-16 07:35:06.000000 deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/top_level.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       25 2023-05-16 07:10:01.000000 deploy_django_nginx-1.0.0/requirements.txt
--rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-05-16 07:35:07.516192 deploy_django_nginx-1.0.0/setup.cfg
--rw-r--r--   0 suqingdong  (1000) disease   (8039)     1288 2023-05-16 07:11:21.000000 deploy_django_nginx-1.0.0/setup.py
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:37:37.578375 deploy_django_nginx-1.0.1/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       66 2023-05-16 07:11:05.000000 deploy_django_nginx-1.0.1/MANIFEST.in
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1949 2023-05-16 07:37:37.572290 deploy_django_nginx-1.0.1/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      940 2023-05-16 07:27:18.000000 deploy_django_nginx-1.0.1/README.md
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:37:37.432929 deploy_django_nginx-1.0.1/deploy_django_nginx/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      188 2023-05-16 07:13:20.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/__init__.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1594 2023-05-16 02:26:05.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/build.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1715 2023-05-16 05:31:35.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/config.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     3188 2023-05-16 07:32:44.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/main.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      533 2023-05-16 02:26:05.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/setup_cython.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1235 2023-05-16 07:31:55.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/util.py
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      266 2023-05-16 07:37:34.000000 deploy_django_nginx-1.0.1/deploy_django_nginx/version.json
+drwxr-xr-x   0 suqingdong  (1000) disease   (8039)        0 2023-05-16 07:37:37.550845 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1949 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/PKG-INFO
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)      523 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/SOURCES.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)        1 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/dependency_links.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       71 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/entry_points.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       25 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/requires.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       20 2023-05-16 07:37:37.000000 deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/top_level.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       25 2023-05-16 07:10:01.000000 deploy_django_nginx-1.0.1/requirements.txt
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)       38 2023-05-16 07:37:37.582170 deploy_django_nginx-1.0.1/setup.cfg
+-rw-r--r--   0 suqingdong  (1000) disease   (8039)     1303 2023-05-16 07:37:27.000000 deploy_django_nginx-1.0.1/setup.py
```

### Comparing `deploy_django_nginx-1.0.0/PKG-INFO` & `deploy_django_nginx-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy_django_nginx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deploy Django with uWSGI and Frontend with Nginx
 Home-page: https://github.com/suqingdong/deploy_django_nginx
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # Deploy Django with uWSGI and Frontend with Nginx
         - Nginx + uWSGI + Django
```

### Comparing `deploy_django_nginx-1.0.0/README.md` & `deploy_django_nginx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx/build.py` & `deploy_django_nginx-1.0.1/deploy_django_nginx/build.py`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx/config.py` & `deploy_django_nginx-1.0.1/deploy_django_nginx/config.py`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx/main.py` & `deploy_django_nginx-1.0.1/deploy_django_nginx/main.py`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx/setup_cython.py` & `deploy_django_nginx-1.0.1/deploy_django_nginx/setup_cython.py`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx/util.py` & `deploy_django_nginx-1.0.1/deploy_django_nginx/util.py`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/PKG-INFO` & `deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploy-django-nginx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deploy Django with uWSGI and Frontend with Nginx
 Home-page: https://github.com/suqingdong/deploy_django_nginx
 Author: suqingdong
 Author-email: suqingdong1114@gmail.com
 License: MIT License
 Description: # Deploy Django with uWSGI and Frontend with Nginx
         - Nginx + uWSGI + Django
```

### Comparing `deploy_django_nginx-1.0.0/deploy_django_nginx.egg-info/SOURCES.txt` & `deploy_django_nginx-1.0.1/deploy_django_nginx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deploy_django_nginx-1.0.0/setup.py` & `deploy_django_nginx-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     long_description_content_type='text/markdown',
     url=version_info['url'],
     license='MIT License',
     install_requires=BASE_DIR.joinpath('requirements.txt').read_text().strip().split(),
     packages=find_packages(),
     include_package_data=True,
     entry_points={'console_scripts': [
-        'name = deploy_django_nginx.main:main',
+        'deploy_django_nginx = deploy_django_nginx.main:main',
     ]},
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
```

