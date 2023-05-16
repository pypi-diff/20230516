# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar", last modified: Fri Apr 21 19:48:12 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar", last modified: Tue May 16 15:53:29 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1.tar` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    32810 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    31256 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6151 2023-03-16 20:46:35.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23857 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    39116 2023-04-21 18:38:06.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10454 2023-03-06 20:52:28.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21693 2023-04-13 08:25:20.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    32810 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-04-21 19:48:12.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-04-21 19:48:10.000000 apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    34370 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    32816 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-05-16 15:39:21.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4081 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-05-12 08:38:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4383 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24886 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    40094 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    10367 2023-04-24 21:04:25.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23045 2023-05-16 07:40:59.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34370 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-05-16 15:53:29.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-16 15:53:28.000000 apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/LICENSE` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.1.0rc1
+Version: 6.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.1.0rc1``
+Release: ``6.2.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
-``apache-airflow``      ``>=2.3.0``
+``apache-airflow``      ``>=2.4.0``
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -112,14 +112,53 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+.. note::
+  If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
+  This should make it easier to mitigate breaking change introduced in 6.0.0
+
+* ``K8s hook should still work with missing default conn (#31187)``
+* ``Add protocol to define methods relied upon by KubernetesPodOperator (#31298)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix kubernetes task decorator pickle error (#31110)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Empty xcom result file log message more specific (#31228)``
+* ``Add options to KubernetesPodOperator (#30992)``
+* ``add missing read for K8S config file from conn in deferred 'KubernetesPodOperator'  (#29498)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Fix pod describing on system test failure (#31191)``
+
 6.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -248,16 +287,17 @@
    * ``Prepare for follow-up relase for November providers (#27774)``
 
 .. Review and move the new changes to one of the sections above:
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Previously KubernetesPodOperator considered some settings from the Airflow config's ``kubernetes`` section.
 Such consideration was deprecated in 4.1.0 and is now removed.  If you previously relied on the Airflow
 config, and you want client generation to have non-default configuration, you will need to define your
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/README.rst` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.1.0rc1``
+Release: ``6.2.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
-``apache-airflow``      ``>=2.3.0``
+``apache-airflow``      ``>=2.4.0``
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -79,14 +79,53 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+.. note::
+  If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
+  This should make it easier to mitigate breaking change introduced in 6.0.0
+
+* ``K8s hook should still work with missing default conn (#31187)``
+* ``Add protocol to define methods relied upon by KubernetesPodOperator (#31298)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix kubernetes task decorator pickle error (#31110)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Empty xcom result file log message more specific (#31228)``
+* ``Add options to KubernetesPodOperator (#30992)``
+* ``add missing read for K8S config file from conn in deferred 'KubernetesPodOperator'  (#29498)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Fix pod describing on system test failure (#31191)``
+
 6.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -215,16 +254,17 @@
    * ``Prepare for follow-up relase for November providers (#27774)``
 
 .. Review and move the new changes to one of the sections above:
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Previously KubernetesPodOperator considered some settings from the Airflow config's ``kubernetes`` section.
 Such consideration was deprecated in 4.1.0 and is now removed.  If you previously relied on the Airflow
 config, and you want client generation to have non-default configuration, you will need to define your
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     )
 
     # Since we won't mutate the arguments, we should just do the shallow copy
     # there are some cases we can't deepcopy the objects (e.g protobuf).
     shallow_copy_attrs: Sequence[str] = ("python_callable",)
 
     def __init__(self, namespace: str = "default", use_dill: bool = False, **kwargs) -> None:
-        self.pickling_library = dill if use_dill else pickle
+        self.use_dill = use_dill
         super().__init__(
             namespace=namespace,
             name=kwargs.pop("name", f"k8s_airflow_pod_{uuid.uuid4().hex}"),
             cmds=["placeholder-command"],
             **kwargs,
         )
 
@@ -108,25 +108,26 @@
                     exec_python_cmd,
                 ]
             ),
         ]
 
     def execute(self, context: Context):
         with TemporaryDirectory(prefix="venv") as tmp_dir:
+            pickling_library = dill if self.use_dill else pickle
             script_filename = os.path.join(tmp_dir, "script.py")
             input_filename = os.path.join(tmp_dir, "script.in")
 
             with open(input_filename, "wb") as file:
-                self.pickling_library.dump({"args": self.op_args, "kwargs": self.op_kwargs}, file)
+                pickling_library.dump({"args": self.op_args, "kwargs": self.op_kwargs}, file)
 
             py_source = self.get_python_source()
             jinja_context = {
                 "op_args": self.op_args,
                 "op_kwargs": self.op_kwargs,
-                "pickling_library": self.pickling_library.__name__,
+                "pickling_library": pickling_library.__name__,
                 "python_callable": self.python_callable.__name__,
                 "python_callable_source": py_source,
                 "string_args_global": False,
             }
             write_python_script(jinja_context=jinja_context, filename=script_filename)
 
             self.env_vars = [
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "6.2.0",
             "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
             "5.1.1",
@@ -60,15 +61,15 @@
             "1.2.0",
             "1.1.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "asgiref>=3.5.2",
             "cryptography>=2.0.0",
             "kubernetes>=21.7.0,<24",
             "kubernetes_asyncio>=18.20.1,<25",
         ],
         "integrations": [
             {
@@ -106,15 +107,15 @@
                 "integration-name": "Kubernetes",
                 "python-modules": ["airflow.providers.cncf.kubernetes.hooks.kubernetes"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Kubernetes",
-                "python-modules": ["airflow.providers.cncf.kubernetes.triggers.pod"],
+                "class-names": ["airflow.providers.cncf.kubernetes.triggers.pod.KubernetesPodTrigger"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.cncf.kubernetes.hooks.kubernetes.KubernetesHook",
                 "connection-type": "kubernetes",
             }
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,31 +26,33 @@
 from kubernetes import client, config, watch
 from kubernetes.client.models import V1Pod
 from kubernetes.config import ConfigException
 from kubernetes_asyncio import client as async_client, config as async_config
 from urllib3.exceptions import HTTPError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowNotFoundException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
+from airflow.models import Connection
+from airflow.providers.cncf.kubernetes.utils.pod_manager import PodOperatorHookProtocol
 from airflow.utils import yaml
 
 LOADING_KUBE_CONFIG_FILE_RESOURCE = "Loading Kubernetes configuration file kube_config from {}..."
 
 
 def _load_body_to_dict(body: str) -> dict:
     try:
         body_dict = yaml.safe_load(body)
     except yaml.YAMLError as e:
         raise AirflowException(f"Exception when loading resource definition: {e}\n")
     return body_dict
 
 
-class KubernetesHook(BaseHook):
+class KubernetesHook(BaseHook, PodOperatorHookProtocol):
     """
     Creates Kubernetes API connection.
 
     - use in cluster configuration by using extra field ``in_cluster`` in connection
     - use custom config by providing path to the file using extra field ``kube_config_path`` in connection
     - use custom configuration by providing content of kubeconfig file via
         extra field ``kube_config`` in connection
@@ -137,14 +139,30 @@
 
     @staticmethod
     def _coalesce_param(*params):
         for param in params:
             if param is not None:
                 return param
 
+    @classmethod
+    def get_connection(cls, conn_id: str) -> Connection:
+        """
+        Return requested connection.
+
+        If missing and conn_id is "kubernetes_default", will return empty connection so that hook will
+        default to cluster-derived credentials.
+        """
+        try:
+            return super().get_connection(conn_id)
+        except AirflowNotFoundException:
+            if conn_id == cls.default_conn_name:
+                return Connection(conn_id=cls.default_conn_name)
+            else:
+                raise
+
     @cached_property
     def conn_extras(self):
         if self.conn_id:
             connection = self.get_connection(self.conn_id)
             extras = connection.extra_dejson
         else:
             extras = {}
@@ -347,15 +365,15 @@
         if self.conn_id and not namespace:
             warnings.warn(
                 "Airflow connection defined but namespace is not set; returning 'default'.  In "
                 "cncf.kubernetes provider version 6.0 we will return None when namespace is "
                 "not defined in the connection so that it's clear whether user intends 'default' or "
                 "whether namespace is unset (which is required in order to apply precedence logic in "
                 "KubernetesPodOperator).",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
             )
             return "default"
         return namespace
 
     def _get_namespace(self) -> str | None:
         """
         Returns the namespace that defined in the connection
@@ -418,14 +436,15 @@
             name=pod_name,
             container=container,
             _preload_content=False,
             namespace=namespace or self._get_namespace() or self.DEFAULT_NAMESPACE,
         )
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
+        """Read pod object from kubernetes API."""
         return self.core_v1_client.read_namespaced_pod(
             name=name,
             namespace=namespace,
         )
 
     def get_namespaced_pod_list(
         self,
@@ -463,44 +482,48 @@
             return False
     return None
 
 
 class AsyncKubernetesHook(KubernetesHook):
     """Hook to use Kubernetes SDK asynchronously."""
 
-    def __init__(self, config_dict: dict | None = None, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.config_dict = config_dict
-
         self._extras: dict | None = None
 
     async def _load_config(self):
         """Returns Kubernetes API session for use with requests"""
         in_cluster = self._coalesce_param(self.in_cluster, await self._get_field("in_cluster"))
         cluster_context = self._coalesce_param(self.cluster_context, await self._get_field("cluster_context"))
+        kubeconfig_path = self._coalesce_param(self.config_file, await self._get_field("kube_config_path"))
         kubeconfig = await self._get_field("kube_config")
 
-        num_selected_configuration = len([o for o in [in_cluster, kubeconfig, self.config_dict] if o])
+        num_selected_configuration = len([o for o in [in_cluster, kubeconfig, kubeconfig_path] if o])
 
         if num_selected_configuration > 1:
             raise AirflowException(
                 "Invalid connection configuration. Options kube_config_path, "
                 "kube_config, in_cluster are mutually exclusive. "
                 "You can only use one option at a time."
             )
 
         if in_cluster:
             self.log.debug(LOADING_KUBE_CONFIG_FILE_RESOURCE.format("within a pod"))
             self._is_in_cluster = True
             async_config.load_incluster_config()
             return async_client.ApiClient()
 
-        if self.config_dict:
-            self.log.debug(LOADING_KUBE_CONFIG_FILE_RESOURCE.format("config dictionary"))
-            await async_config.load_kube_config_from_dict(self.config_dict)
+        if kubeconfig_path:
+            self.log.debug(LOADING_KUBE_CONFIG_FILE_RESOURCE.format("kube_config"))
+            self._is_in_cluster = False
+            await async_config.load_kube_config(
+                config_file=kubeconfig_path,
+                client_configuration=self.client_configuration,
+                context=cluster_context,
+            )
             return async_client.ApiClient()
 
         if kubeconfig is not None:
             with tempfile.NamedTemporaryFile() as temp_config:
                 self.log.debug(
                     "Reading kubernetes configuration file from connection "
                     "object and writing temporary config file with its content",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -11,7 +10,10 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
+
+__all__ = ["xcom_sidecar", "pod_manager"]
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 
-from airflow.providers.cncf.kubernetes.operators.pod import *  # noqa
+from airflow.exceptions import AirflowProviderDeprecationWarning
+from airflow.providers.cncf.kubernetes.triggers.pod import *  # noqa
 
 warnings.warn(
-    "This module is deprecated. Please use `airflow.providers.cncf.kubernetes.operators.pod` instead.",
-    DeprecationWarning,
+    "This module is deprecated. Please use `airflow.providers.cncf.kubernetes.triggers.pod` instead.",
+    AirflowProviderDeprecationWarning,
     stacklevel=2,
 )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException, AirflowSkipException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
 from airflow.kubernetes import pod_generator
 from airflow.kubernetes.pod_generator import PodGenerator
 from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
     convert_configmap,
@@ -52,14 +52,15 @@
 )
 from airflow.providers.cncf.kubernetes.hooks.kubernetes import KubernetesHook
 from airflow.providers.cncf.kubernetes.triggers.pod import KubernetesPodTrigger
 from airflow.providers.cncf.kubernetes.utils import xcom_sidecar  # type: ignore[attr-defined]
 from airflow.providers.cncf.kubernetes.utils.pod_manager import (
     PodLaunchFailedException,
     PodManager,
+    PodOperatorHookProtocol,
     PodPhase,
     get_container_termination_message,
 )
 from airflow.settings import pod_mutation_hook
 from airflow.utils import yaml
 from airflow.utils.helpers import prune_dict, validate_key
 from airflow.utils.timezone import utcnow
@@ -193,14 +194,17 @@
         state, or the execution is interrupted. If True (default), delete the
         pod; if False, leave the pod.
     :param hostnetwork: If True enable host networking on the pod.
     :param tolerations: A list of kubernetes tolerations.
     :param security_context: security options the pod should run with (PodSecurityContext).
     :param container_security_context: security options the container should run with.
     :param dnspolicy: dnspolicy for the pod.
+    :param dns_config: dns configuration (ip addresses, searches, options) for the pod.
+    :param hostname: hostname for the pod.
+    :param subdomain: subdomain for the pod.
     :param schedulername: Specify a schedulername for the pod
     :param full_pod_spec: The complete podSpec
     :param init_containers: init container for the launched Pod
     :param log_events_on_failure: Log the pod's events if a failure occurs
     :param do_xcom_push: If True, the content of the file
         /airflow/xcom/return.json in the container will also be pushed to an
         XCom when the container completes.
@@ -278,14 +282,17 @@
         service_account_name: str | None = None,
         is_delete_operator_pod: bool = True,
         hostnetwork: bool = False,
         tolerations: list[k8s.V1Toleration] | None = None,
         security_context: dict | None = None,
         container_security_context: dict | None = None,
         dnspolicy: str | None = None,
+        dns_config: k8s.V1PodDNSConfig | None = None,
+        hostname: str | None = None,
+        subdomain: str | None = None,
         schedulername: str | None = None,
         full_pod_spec: k8s.V1Pod | None = None,
         init_containers: list[k8s.V1Container] | None = None,
         log_events_on_failure: bool = False,
         do_xcom_push: bool = False,
         pod_template_file: str | None = None,
         priority_class_name: str | None = None,
@@ -347,14 +354,17 @@
         self.hostnetwork = hostnetwork
         self.tolerations = (
             [convert_toleration(toleration) for toleration in tolerations] if tolerations else []
         )
         self.security_context = security_context or {}
         self.container_security_context = container_security_context
         self.dnspolicy = dnspolicy
+        self.dns_config = dns_config
+        self.hostname = hostname
+        self.subdomain = subdomain
         self.schedulername = schedulername
         self.full_pod_spec = full_pod_spec
         self.init_containers = init_containers or []
         self.log_events_on_failure = log_events_on_failure
         self.priority_class_name = priority_class_name
         self.pod_template_file = pod_template_file
         self.name = self._set_name(name)
@@ -369,16 +379,15 @@
             if skip_on_exit_code
             else []
         )
         self.base_container_name = base_container_name or self.BASE_CONTAINER_NAME
         self.deferrable = deferrable
         self.poll_interval = poll_interval
         self.remote_pod: k8s.V1Pod | None = None
-
-        self._config_dict: dict | None = None
+        self._config_dict: dict | None = None  # TODO: remove it when removing convert_config_file_to_dict
 
     @cached_property
     def _incluster_namespace(self):
         from pathlib import Path
 
         path = Path("/var/run/secrets/kubernetes.io/serviceaccount/namespace")
         return path.exists() and path.read_text() or None
@@ -451,25 +460,29 @@
         return labels
 
     @cached_property
     def pod_manager(self) -> PodManager:
         return PodManager(kube_client=self.client)
 
     @cached_property
-    def hook(self) -> KubernetesHook:
+    def hook(self) -> PodOperatorHookProtocol:
         hook = KubernetesHook(
             conn_id=self.kubernetes_conn_id,
             in_cluster=self.in_cluster,
             config_file=self.config_file,
             cluster_context=self.cluster_context,
         )
         return hook
 
     def get_hook(self):
-        warnings.warn("get_hook is deprecated. Please use hook instead.", DeprecationWarning, stacklevel=2)
+        warnings.warn(
+            "get_hook is deprecated. Please use hook instead.",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
+        )
         return self.hook
 
     @cached_property
     def client(self) -> CoreV1Api:
         return self.hook.core_v1_client
 
     def find_pod(self, namespace: str, context: Context, *, exclude_checked: bool = True) -> k8s.V1Pod | None:
@@ -511,15 +524,15 @@
                     self.log.error("Pod Event: %s - %s", event.reason, event.message)
             raise
 
     def extract_xcom(self, pod: k8s.V1Pod):
         """Retrieves xcom value and kills xcom sidecar container"""
         result = self.pod_manager.extract_xcom(pod)
         if isinstance(result, str) and result.rstrip() == "__airflow_xcom_result_empty__":
-            self.log.info("Result file is empty.")
+            self.log.info("xcom result file is empty.")
             return None
         else:
             self.log.info("xcom result: \n%s", result)
             return json.loads(result)
 
     def execute(self, context: Context):
         """Based on the deferrable parameter runs the pod asynchronously or synchronously"""
@@ -531,14 +544,19 @@
     def execute_sync(self, context: Context):
         try:
             self.pod_request_obj = self.build_pod_request_obj(context)
             self.pod = self.get_or_create_pod(  # must set `self.pod` for `on_kill`
                 pod_request_obj=self.pod_request_obj,
                 context=context,
             )
+            # push to xcom now so that if there is an error we still have the values
+            ti = context["ti"]
+            ti.xcom_push(key="pod_name", value=self.pod.metadata.name)
+            ti.xcom_push(key="pod_namespace", value=self.pod.metadata.namespace)
+
             # get remote pod for use in cleanup methods
             self.remote_pod = self.find_pod(self.pod.metadata.namespace, context=context)
             self.await_pod_start(pod=self.pod)
 
             if self.get_logs:
                 self.pod_manager.fetch_container_logs(
                     pod=self.pod,
@@ -556,31 +574,32 @@
                 result = self.extract_xcom(pod=self.pod)
             self.remote_pod = self.pod_manager.await_pod_completion(self.pod)
         finally:
             self.cleanup(
                 pod=self.pod or self.pod_request_obj,
                 remote_pod=self.remote_pod,
             )
-        ti = context["ti"]
-        ti.xcom_push(key="pod_name", value=self.pod.metadata.name)
-        ti.xcom_push(key="pod_namespace", value=self.pod.metadata.namespace)
         if self.do_xcom_push:
             return result
 
     def execute_async(self, context: Context):
         self.pod_request_obj = self.build_pod_request_obj(context)
         self.pod = self.get_or_create_pod(  # must set `self.pod` for `on_kill`
             pod_request_obj=self.pod_request_obj,
             context=context,
         )
-        self.convert_config_file_to_dict()
         self.invoke_defer_method()
 
     def convert_config_file_to_dict(self):
         """Converts passed config_file to dict format."""
+        warnings.warn(
+            "This method is deprecated and will be removed in a future version.",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
+        )
         config_file = self.config_file if self.config_file else os.environ.get(KUBE_CONFIG_ENV_VAR)
         if config_file:
             with open(config_file) as f:
                 self._config_dict = yaml.safe_load(f)
         else:
             self._config_dict = None
 
@@ -590,15 +609,15 @@
         self.defer(
             trigger=KubernetesPodTrigger(
                 pod_name=self.pod.metadata.name,
                 pod_namespace=self.pod.metadata.namespace,
                 trigger_start_time=trigger_start_time,
                 kubernetes_conn_id=self.kubernetes_conn_id,
                 cluster_context=self.cluster_context,
-                config_dict=self._config_dict,
+                config_file=self.config_file,
                 in_cluster=self.in_cluster,
                 poll_interval=self.poll_interval,
                 should_delete_pod=self.is_delete_operator_pod,
                 get_logs=self.get_logs,
                 startup_timeout=self.startup_timeout_seconds,
                 base_container_name=self.base_container_name,
             ),
@@ -805,16 +824,19 @@
                         env_from=self.env_from,
                         security_context=self.container_security_context,
                     )
                 ],
                 image_pull_secrets=self.image_pull_secrets,
                 service_account_name=self.service_account_name,
                 host_network=self.hostnetwork,
+                hostname=self.hostname,
+                subdomain=self.subdomain,
                 security_context=self.security_context,
                 dns_policy=self.dnspolicy,
+                dns_config=self.dns_config,
                 scheduler_name=self.schedulername,
                 restart_policy="Never",
                 priority_class_name=self.priority_class_name,
                 volumes=self.volumes,
             ),
         )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 
-from airflow.providers.cncf.kubernetes.triggers.pod import *  # noqa
+from airflow.exceptions import AirflowProviderDeprecationWarning
+from airflow.providers.cncf.kubernetes.operators.pod import *  # noqa
 
 warnings.warn(
-    "This module is deprecated. Please use `airflow.providers.cncf.kubernetes.triggers.pod` instead.",
-    DeprecationWarning,
+    "This module is deprecated. Please use `airflow.providers.cncf.kubernetes.operators.pod` instead.",
+    AirflowProviderDeprecationWarning,
     stacklevel=2,
 )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
     KubernetesPodTrigger run on the trigger worker to check the state of Pod.
 
     :param pod_name: The name of the pod.
     :param pod_namespace: The namespace of the pod.
     :param kubernetes_conn_id: The :ref:`kubernetes connection id <howto/connection:kubernetes>`
         for the Kubernetes cluster.
     :param cluster_context: Context that points to kubernetes cluster.
-    :param config_dict: Kubernetes config file content in dict format. If not specified,
-        default value is ``~/.kube/config``
+    :param config_file: Path to kubeconfig file.
     :param poll_interval: Polling period in seconds to check for the status.
     :param trigger_start_time: time in Datetime format when the trigger was started
     :param in_cluster: run kubernetes client with in_cluster configuration.
     :param should_delete_pod: What to do when the pod reaches its final
         state, or the execution is interrupted. If True (default), delete the
         pod; if False, leave the pod.
     :param get_logs: get the stdout of the container as logs of the tasks.
@@ -69,29 +68,29 @@
         pod_name: str,
         pod_namespace: str,
         trigger_start_time: datetime,
         base_container_name: str,
         kubernetes_conn_id: str | None = None,
         poll_interval: float = 2,
         cluster_context: str | None = None,
-        config_dict: dict | None = None,
+        config_file: str | None = None,
         in_cluster: bool | None = None,
         should_delete_pod: bool = True,
         get_logs: bool = True,
         startup_timeout: int = 120,
     ):
         super().__init__()
         self.pod_name = pod_name
         self.pod_namespace = pod_namespace
         self.trigger_start_time = trigger_start_time
         self.base_container_name = base_container_name
         self.kubernetes_conn_id = kubernetes_conn_id
         self.poll_interval = poll_interval
         self.cluster_context = cluster_context
-        self.config_dict = config_dict
+        self.config_file = config_file
         self.in_cluster = in_cluster
         self.should_delete_pod = should_delete_pod
         self.get_logs = get_logs
         self.startup_timeout = startup_timeout
 
         self._hook: AsyncKubernetesHook | None = None
         self._since_time = None
@@ -103,24 +102,24 @@
             {
                 "pod_name": self.pod_name,
                 "pod_namespace": self.pod_namespace,
                 "base_container_name": self.base_container_name,
                 "kubernetes_conn_id": self.kubernetes_conn_id,
                 "poll_interval": self.poll_interval,
                 "cluster_context": self.cluster_context,
-                "config_dict": self.config_dict,
+                "config_file": self.config_file,
                 "in_cluster": self.in_cluster,
                 "should_delete_pod": self.should_delete_pod,
                 "get_logs": self.get_logs,
                 "startup_timeout": self.startup_timeout,
                 "trigger_start_time": self.trigger_start_time,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:  # type: ignore[override]
+    async def run(self) -> AsyncIterator[TriggerEvent]:  # type: ignore[override]
         """Gets current pod status and yields a TriggerEvent"""
         hook = self._get_async_hook()
         self.log.info("Checking pod %r in namespace %r.", self.pod_name, self.pod_namespace)
         while True:
             try:
                 pod = await hook.get_pod(
                     name=self.pod_name,
@@ -211,15 +210,15 @@
                 return
 
     def _get_async_hook(self) -> AsyncKubernetesHook:
         if self._hook is None:
             self._hook = AsyncKubernetesHook(
                 conn_id=self.kubernetes_conn_id,
                 in_cluster=self.in_cluster,
-                config_dict=self.config_dict,
+                config_file=self.config_file,
                 cluster_context=self.cluster_context,
             )
         return self._hook
 
     def define_container_state(self, pod: V1Pod) -> ContainerState:
         pod_containers = pod.status.container_statuses
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import stream as kubernetes_stream
 from pendulum import DateTime
 from pendulum.parsing.exceptions import ParserError
 from urllib3.exceptions import HTTPError as BaseHTTPError
 from urllib3.response import HTTPResponse
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.kubernetes.pod_generator import PodDefaults
+from airflow.typing_compat import Protocol
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.timezone import utcnow
 
 if TYPE_CHECKING:
     from kubernetes.client.models.core_v1_event_list import CoreV1EventList
 
 
@@ -68,14 +69,48 @@
     RUNNING = "Running"
     FAILED = "Failed"
     SUCCEEDED = "Succeeded"
 
     terminal_states = {FAILED, SUCCEEDED}
 
 
+class PodOperatorHookProtocol(Protocol):
+    """
+    Protocol to define methods relied upon by KubernetesPodOperator
+
+    Subclasses of KubernetesPodOperator, such as GKEStartPodOperator, may use
+    hooks that don't extend KubernetesHook.  We use this protocol to document the
+    methods used by KPO and ensure that these methods exist on such other hooks.
+    """
+
+    @property
+    def core_v1_client(self) -> client.CoreV1Api:
+        """Get authenticated CoreV1Api object."""
+
+    @property
+    def is_in_cluster(self) -> bool:
+        """Expose whether the hook is configured with ``load_incluster_config`` or not"""
+
+    def get_pod(self, name: str, namespace: str) -> V1Pod:
+        """Read pod object from kubernetes API."""
+
+    def _get_namespace(self) -> str | None:
+        """
+        Returns the namespace that defined in the connection
+
+        TODO: in provider version 6.0, get rid of this method and make it the behavior of get_namespace.
+        """
+
+    def get_xcom_sidecar_container_image(self) -> str | None:
+        """Returns the xcom sidecar image that defined in the connection"""
+
+    def get_xcom_sidecar_container_resources(self) -> str | None:
+        """Returns the xcom sidecar resources that defined in the connection"""
+
+
 def get_container_status(pod: V1Pod, container_name: str) -> V1ContainerStatus | None:
     """Retrieves container status"""
     container_statuses = pod.status.container_statuses if pod and pod.status else None
     if container_statuses:
         # In general the variable container_statuses can store multiple items matching different containers.
         # The following generator expression yields all items that have name equal to the container_name.
         # The function next() here calls the generator to get only the first value. If there's nothing found
@@ -292,15 +327,15 @@
                 raise PodLaunchFailedException(msg)
             time.sleep(1)
 
     def follow_container_logs(self, pod: V1Pod, container_name: str) -> PodLoggingStatus:
         warnings.warn(
             "Method `follow_container_logs` is deprecated.  Use `fetch_container_logs` instead"
             "with option `follow=True`.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
         )
         return self.fetch_container_logs(pod=pod, container_name=container_name, follow=True)
 
     def fetch_container_logs(
         self,
         pod: V1Pod,
         container_name: str,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 6.1.0rc1
+Version: 6.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``6.1.0rc1``
+Release: ``6.2.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
-``apache-airflow``      ``>=2.3.0``
+``apache-airflow``      ``>=2.4.0``
 ``asgiref``             ``>=3.5.2``
 ``cryptography``        ``>=2.0.0``
 ``kubernetes``          ``>=21.7.0,<24``
 ``kubernetes_asyncio``  ``>=18.20.1,<25``
 ======================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -112,14 +112,53 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+6.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+.. note::
+  If ``kubernetes_default`` connection is not defined, then KubernetesHook / KubernetesPodOperator will behave as though given ``conn_id=None``.
+  This should make it easier to mitigate breaking change introduced in 6.0.0
+
+* ``K8s hook should still work with missing default conn (#31187)``
+* ``Add protocol to define methods relied upon by KubernetesPodOperator (#31298)``
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Fix kubernetes task decorator pickle error (#31110)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Empty xcom result file log message more specific (#31228)``
+* ``Add options to KubernetesPodOperator (#30992)``
+* ``add missing read for K8S config file from conn in deferred 'KubernetesPodOperator'  (#29498)``
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Fix pod describing on system test failure (#31191)``
+
 6.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -248,16 +287,17 @@
    * ``Prepare for follow-up relase for November providers (#27774)``
 
 .. Review and move the new changes to one of the sections above:
 
 5.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 Previously KubernetesPodOperator considered some settings from the Airflow config's ``kubernetes`` section.
 Such consideration was deprecated in 4.1.0 and is now removed.  If you previously relied on the Airflow
 config, and you want client generation to have non-default configuration, you will need to define your
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 target-version = "py37"
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
+    # implicit single-line string concatenation
+    "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/6.2.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,15 +42,15 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	asgiref>=3.5.2
 	cryptography>=2.0.0
 	kubernetes>=21.7.0,<24
 	kubernetes_asyncio>=18.20.1,<25
 
 [options.entry_points]
 apache_airflow_provider =
```

### Comparing `apache-airflow-providers-cncf-kubernetes-6.1.0rc1/setup.py` & `apache-airflow-providers-cncf-kubernetes-6.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.0"
+version = "6.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

