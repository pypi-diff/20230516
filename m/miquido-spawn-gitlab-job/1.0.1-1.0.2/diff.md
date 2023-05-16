# Comparing `tmp/miquido_spawn_gitlab_job-1.0.1.tar.gz` & `tmp/miquido_spawn_gitlab_job-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miquido_spawn_gitlab_job-1.0.1.tar", last modified: Tue May 16 10:49:59 2023, max compression
+gzip compressed data, was "miquido_spawn_gitlab_job-1.0.2.tar", last modified: Tue May 16 10:55:25 2023, max compression
```

## Comparing `miquido_spawn_gitlab_job-1.0.1.tar` & `miquido_spawn_gitlab_job-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:49:59.333927 miquido_spawn_gitlab_job-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-16 10:49:59.333927 miquido_spawn_gitlab_job-1.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:49:59.333927 miquido_spawn_gitlab_job-1.0.1/gitlab_env_spawner/
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-16 10:49:48.977002 miquido_spawn_gitlab_job-1.0.1/gitlab_env_spawner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-16 10:49:48.977002 miquido_spawn_gitlab_job-1.0.1/gitlab_env_spawner/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-16 10:17:05.917803 miquido_spawn_gitlab_job-1.0.1/gitlab_env_spawner/spawner.py
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-16 10:49:59.165912 miquido_spawn_gitlab_job-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:55:25.802473 miquido_spawn_gitlab_job-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-16 10:55:25.802473 miquido_spawn_gitlab_job-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:55:25.802473 miquido_spawn_gitlab_job-1.0.2/gitlab_env_spawner/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-05-16 10:49:02.655370 miquido_spawn_gitlab_job-1.0.2/gitlab_env_spawner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2023-05-16 10:49:02.655370 miquido_spawn_gitlab_job-1.0.2/gitlab_env_spawner/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-16 10:49:02.655370 miquido_spawn_gitlab_job-1.0.2/gitlab_env_spawner/spawner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-16 10:55:25.642460 miquido_spawn_gitlab_job-1.0.2/setup.py
```

### Comparing `miquido_spawn_gitlab_job-1.0.1/PKG-INFO` & `miquido_spawn_gitlab_job-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: miquido_spawn_gitlab_job
-Version: 1.0.1
+Version: 1.0.2
 Summary: Launches dynamic environment on AWS ECS
 Home-page: UNKNOWN
 Author: Marek
 Author-email: marek.moscichowski@miquido.com
 License: MIT
 Description: UNKNOWN
 Keywords: GITLAB
```

### Comparing `miquido_spawn_gitlab_job-1.0.1/gitlab_env_spawner/spawner.py` & `miquido_spawn_gitlab_job-1.0.2/gitlab_env_spawner/spawner.py`

 * *Files identical despite different names*

### Comparing `miquido_spawn_gitlab_job-1.0.1/setup.py` & `miquido_spawn_gitlab_job-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 
 setup(
     name='miquido_spawn_gitlab_job',  # How you named your package folder (MyLib)
     packages=['gitlab_env_spawner'],  # Chose the same as "name"
-    version='1.0.1',
+    version='1.0.2',
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Launches dynamic environment on AWS ECS',
     # Give a short description about your library
     author='Marek',  # Type in your name
     author_email='marek.moscichowski@miquido.com',  # Type in your E-Mail
     keywords=['GITLAB'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
-        'requests'
+        'boto3'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
```

