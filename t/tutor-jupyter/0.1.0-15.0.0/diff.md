# Comparing `tmp/tutor-jupyter-0.1.0.tar.gz` & `tmp/tutor-jupyter-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-jupyter-0.1.0.tar", last modified: Fri May 12 15:34:24 2023, max compression
+gzip compressed data, was "dist/tutor-jupyter-15.0.0.tar", last modified: Tue May 16 13:48:49 2023, max compression
```

## Comparing `tutor-jupyter-0.1.0.tar` & `tutor-jupyter-15.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     3836 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     2936 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     3836 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1134 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutor_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/dev-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/apps/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/hub/
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/lab/
--rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/lab/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:24.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/init/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-12 15:34:13.000000 tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     5843 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4942 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     5843 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1134 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/dev-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/
+-rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/
+-rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
```

### Comparing `tutor-jupyter-0.1.0/LICENSE.txt` & `tutor-jupyter-15.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/setup.py` & `tutor-jupyter-15.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/tutor_jupyter.egg-info/SOURCES.txt` & `tutor-jupyter-15.0.0/tutor_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/tutorjupyter/plugin.py` & `tutor-jupyter-15.0.0/tutorjupyter/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py` & `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 c.JupyterHub.db_url = "mysql+pymysql://{{ JUPYTER_HUB_MYSQL_USERNAME }}:{{ JUPYTER_HUB_MYSQL_PASSWORD }}@{{ MYSQL_HOST }}:{{ MYSQL_PORT }}/{{ JUPYTER_HUB_MYSQL_DATABASE }}"
 c.JupyterHub.cookie_secret = "{{ JUPYTER_HUB_COOKIE_SECRET }}"
 
 # Authorise embedding in some iframes.
 # Add "*" to allow embedding in all iframes (though it's dangerous and you probably
 # shouldn't do it).
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy/frame-ancestors
-content_security_policy = "frame-ancestors 'self' "
-content_security_policy += " ".join(
-    [
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}:8000",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ CMS_HOST }}",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ CMS_HOST }}:8001",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ MFE_HOST }}",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ MFE_HOST }}:2000",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ PREVIEW_LMS_HOST }}",
-        "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ PREVIEW_LMS_HOST }}:8000",
-    ]
-)
-content_security_policy += ";"
+frame_ancestors = [
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ LMS_HOST }}:8000",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ CMS_HOST }}",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ CMS_HOST }}:8001",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ PREVIEW_LMS_HOST }}",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ PREVIEW_LMS_HOST }}:8000",
+]
+{% if MFE_HOST is defined %}
+frame_ancestors += [
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ MFE_HOST }}",
+    "{% if ENABLE_HTTPS %}https{% else %}http{% endif %}://{{ MFE_HOST }}:2000",
+]
+{% endif %}
+content_security_policy = "frame-ancestors 'self' " + " ".join(frame_ancestors) + ";"
 c.JupyterHub.tornado_settings = {
     "headers": {"Content-Security-Policy": content_security_policy}
 }
 
 # Authenticator
 # note that the JUPYTERHUB_CRYPT_KEY env var must be defined
 c.Authenticator.enable_auth_state = True
@@ -85,7 +86,9 @@
 c.DockerSpawner.notebook_dir = notebook_dir
 c.DockerSpawner.volumes = {"jupyterhub-user-{username}": notebook_dir}
 # Limit spawner cpu and memory
 {% if JUPYTER_LAB_CPU_LIMIT %}
 c.Spawner.cpu_limit = {{ JUPYTER_LAB_CPU_LIMIT }}
 {% endif %}
 c.Spawner.mem_limit = "{{ JUPYTER_LAB_MEMORY_LIMIT }}"
+
+{{ patch("jupyterhub-config") }}
```

### Comparing `tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile` & `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile` & `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-0.1.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh` & `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh`

 * *Files identical despite different names*

