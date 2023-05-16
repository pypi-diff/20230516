# Comparing `tmp/jupyterlab_nbgallery-2.0.0a4.tar.gz` & `tmp/jupyterlab_nbgallery-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_nbgallery-2.0.0a4.tar", last modified: Fri Apr  7 14:55:54 2023, max compression
+gzip compressed data, was "jupyterlab_nbgallery-2.0.2.tar", last modified: Tue May 16 11:51:17 2023, max compression
```

## Comparing `jupyterlab_nbgallery-2.0.0a4.tar` & `jupyterlab_nbgallery-2.0.2.tar`

### file list

```diff
@@ -1,119 +1,118 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.357939 jupyterlab_nbgallery-2.0.0a4/
--rw-r--r--   0 jovyan    (1000) users      (100)     1066 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/LICENSE
--rw-r--r--   0 jovyan    (1000) users      (100)      388 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     2694 2023-04-07 14:55:54.357939 jupyterlab_nbgallery-2.0.0a4/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     2014 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/README.md
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.341940 jupyterlab_nbgallery-2.0.0a4/jupyter-config/
--rw-r--r--   0 jovyan    (1000) users      (100)       96 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/jupyter-config/jupyterlab_nbgallery.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.341940 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/
--rw-r--r--   0 jovyan    (1000) users      (100)      596 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)       76 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/_version.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3640 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/handlers.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.341940 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     2694 2023-04-07 14:55:54.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     4503 2023-04-07 14:55:54.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-04-07 14:55:54.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-04-07 14:46:08.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       61 2023-04-07 14:55:54.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       21 2023-04-07 14:55:54.000000 jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/top_level.txt
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.341940 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/
--rw-r--r--   0 jovyan    (1000) users      (100)     2596 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.341940 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/
--rw-r--r--   0 jovyan    (1000) users      (100)      335 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2454 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     3438 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
--rw-r--r--   0 jovyan    (1000) users      (100)     1969 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/568.017b32a913356ad383e7.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90038 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     6936 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/remoteEntry.1353121aacb4a50d2fe1.js
--rw-r--r--   0 jovyan    (1000) users      (100)      178 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-04-07 14:55:18.000000 jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/
--rw-r--r--   0 jovyan    (1000) users      (100)     2618 2023-04-07 14:55:13.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/
--rw-r--r--   0 jovyan    (1000) users      (100)     2476 2023-04-07 14:55:09.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     1213 2023-04-07 14:55:12.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/248.644879940d9faca2b389.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3446 2023-04-07 14:55:12.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
--rw-r--r--   0 jovyan    (1000) users      (100)     6680 2023-04-07 14:55:12.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/remoteEntry.c977e6e35771b75265ee.js
--rw-r--r--   0 jovyan    (1000) users      (100)      182 2023-04-07 14:55:09.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     2452 2023-04-07 14:55:12.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/
--rw-r--r--   0 jovyan    (1000) users      (100)     2579 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.345939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/
--rw-r--r--   0 jovyan    (1000) users      (100)      680 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2437 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     3460 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/542.feae6c397f33f9138fea.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90062 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/638.36e464d3233849b6b07a.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     1520 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/784.f151a96d5dde1a095c86.js
--rw-r--r--   0 jovyan    (1000) users      (100)     7076 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/remoteEntry.5a586807c39202b9c488.js
--rw-r--r--   0 jovyan    (1000) users      (100)      190 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/
--rw-r--r--   0 jovyan    (1000) users      (100)     2698 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.333939 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/
--rw-r--r--   0 jovyan    (1000) users      (100)     2556 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     4018 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/542.18fd91d86aaf6286edd0.js
--rw-r--r--   0 jovyan    (1000) users      (100)    10503 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/56.a4862cb4315ce0eea068.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90036 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/638.95e0186307171588df5b.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     7213 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/remoteEntry.f6acbd64cdadb94c1dff.js
--rw-r--r--   0 jovyan    (1000) users      (100)      177 2023-04-07 14:55:10.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-04-07 14:55:19.000000 jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/
--rw-r--r--   0 jovyan    (1000) users      (100)     2444 2023-04-07 14:55:46.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.349939 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/
--rw-r--r--   0 jovyan    (1000) users      (100)     2328 2023-04-07 14:55:45.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.353939 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/
--rw-r--r--   0 jovyan    (1000) users      (100)      931 2023-04-07 14:55:46.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/568.0616ffe42e5ee3230288.js
--rw-r--r--   0 jovyan    (1000) users      (100)     6315 2023-04-07 14:55:46.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/remoteEntry.6def7b207d91856938f3.js
--rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-04-07 14:55:45.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)       20 2023-04-07 14:55:46.000000 jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.353939 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/
--rw-r--r--   0 jovyan    (1000) users      (100)     2527 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.353939 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/
--rw-r--r--   0 jovyan    (1000) users      (100)      345 2023-04-07 14:55:47.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
--rw-r--r--   0 jovyan    (1000) users      (100)     2411 2023-04-07 14:55:47.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.353939 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     1721 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/568.7f1ab65a55b54297cd7b.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/638.b95125ed695cee42aae4.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     8425 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
--rw-r--r--   0 jovyan    (1000) users      (100)     7597 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/remoteEntry.ae4d1ce402e6ac0dddb5.js
--rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-04-07 14:55:47.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     2479 2023-04-07 14:55:52.000000 jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/third-party-licenses.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.353939 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/
--rw-r--r--   0 jovyan    (1000) users      (100)     2709 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/package.json
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/schemas/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.337939 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/schemas/@jupyterlab-nbgallery/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.357939 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/
--rw-r--r--   0 jovyan    (1000) users      (100)     2567 2023-04-07 14:55:48.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-04-07 14:55:54.357939 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/
--rw-r--r--   0 jovyan    (1000) users      (100)     4026 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
--rw-r--r--   0 jovyan    (1000) users      (100)     4115 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/568.0ac7cbac0996e718a0d9.js
--rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/638.e5080f99954048969f76.js
--rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
--rw-r--r--   0 jovyan    (1000) users      (100)     7136 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/remoteEntry.3f8d9d3f425bc3ff0a80.js
--rw-r--r--   0 jovyan    (1000) users      (100)      181 2023-04-07 14:55:48.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/style.js
--rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-04-07 14:55:53.000000 jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/third-party-licenses.json
--rw-r--r--   0 jovyan    (1000) users      (100)     1103 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/package.json
--rw-r--r--   0 jovyan    (1000) users      (100)      145 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-04-07 14:55:54.357939 jupyterlab_nbgallery-2.0.0a4/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)     3928 2023-04-07 14:52:37.000000 jupyterlab_nbgallery-2.0.0a4/setup.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1066 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/LICENSE
+-rw-r--r--   0 jovyan    (1000) users      (100)      388 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     2014 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/README.md
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyter-config/
+-rw-r--r--   0 jovyan    (1000) users      (100)       96 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyter-config/jupyterlab_nbgallery.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/
+-rw-r--r--   0 jovyan    (1000) users      (100)      596 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)       72 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/_version.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3640 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/handlers.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2692 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     4443 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/not-zip-safe
+-rw-r--r--   0 jovyan    (1000) users      (100)       61 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       21 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/top_level.txt
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2503 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.107679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/
+-rw-r--r--   0 jovyan    (1000) users      (100)      335 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2361 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     3438 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2142 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/568.8bc32e058afbf3d8a017.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90038 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     6914 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      178 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2644 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2502 2023-05-16 11:50:34.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1162 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/248.19732aba6894a502e197.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3446 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     6651 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      182 2023-05-16 11:50:34.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2452 2023-05-16 11:50:37.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2525 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.111679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/
+-rw-r--r--   0 jovyan    (1000) users      (100)      680 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2383 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     3460 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/542.feae6c397f33f9138fea.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90062 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     1648 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/784.201d6fbbedd26339ab72.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     7044 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      190 2023-05-16 11:50:35.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:50:44.000000 jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2481 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.099679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2365 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)    11664 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90036 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     7108 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:50:36.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     1262 2023-05-16 11:50:45.000000 jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2418 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2302 2023-05-16 11:51:06.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1259 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/568.bde16f9395a112a349ee.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     6305 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:51:06.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)       20 2023-05-16 11:51:08.000000 jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.115679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2434 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/
+-rw-r--r--   0 jovyan    (1000) users      (100)      345 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     2318 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     1929 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     8425 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     7555 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      118 2023-05-16 11:51:10.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     2479 2023-05-16 11:51:15.000000 jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/third-party-licenses.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2590 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/package.json
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.103679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.119679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/
+-rw-r--r--   0 jovyan    (1000) users      (100)     2448 2023-05-16 11:51:11.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/
+-rw-r--r--   0 jovyan    (1000) users      (100)     4026 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     4448 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js
+-rw-r--r--   0 jovyan    (1000) users      (100)    90044 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      476 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)     7158 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js
+-rw-r--r--   0 jovyan    (1000) users      (100)      181 2023-05-16 11:51:11.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/style.js
+-rw-r--r--   0 jovyan    (1000) users      (100)     3692 2023-05-16 11:51:16.000000 jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/third-party-licenses.json
+-rw-r--r--   0 jovyan    (1000) users      (100)     1135 2023-05-16 11:49:22.000000 jupyterlab_nbgallery-2.0.2/package.json
+-rw-r--r--   0 jovyan    (1000) users      (100)      146 2023-05-16 11:49:23.000000 jupyterlab_nbgallery-2.0.2/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-16 11:51:17.123679 jupyterlab_nbgallery-2.0.2/setup.cfg
+-rw-r--r--   0 jovyan    (1000) users      (100)     3928 2023-05-16 11:49:22.000000 jupyterlab_nbgallery-2.0.2/setup.py
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/LICENSE` & `jupyterlab_nbgallery-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/PKG-INFO` & `jupyterlab_nbgallery-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbgallery
-Version: 2.0.0a4
+Version: 2.0.2
 Summary: A JupyterLab Extension for NBGallery integration
 Home-page: https://github.com/nbgallery/lab-extensions
 Author: NBGallery
 License: MIT
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/README.md` & `jupyterlab_nbgallery-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/__init__.py` & `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery/handlers.py` & `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/PKG-INFO` & `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-nbgallery
-Version: 2.0.0a4
+Version: 2.0.2
 Summary: A JupyterLab Extension for NBGallery integration
 Home-page: https://github.com/nbgallery/lab-extensions
 Author: NBGallery
 License: MIT
 Keywords: Jupyter,JupyterLab
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/jupyterlab_nbgallery.egg-info/SOURCES.txt` & `jupyterlab_nbgallery-2.0.2/jupyterlab_nbgallery.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,64 +14,63 @@
 jupyterlab_nbgallery.egg-info/not-zip-safe
 jupyterlab_nbgallery.egg-info/requires.txt
 jupyterlab_nbgallery.egg-info/top_level.txt
 labextension/autodownload/package.json
 labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/autodownload.json
 labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig
 labextension/autodownload/static/542.51fb91347d8a3d9a657a.js
-labextension/autodownload/static/568.017b32a913356ad383e7.js
+labextension/autodownload/static/568.8bc32e058afbf3d8a017.js
 labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js
 labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js.LICENSE.txt
-labextension/autodownload/static/remoteEntry.1353121aacb4a50d2fe1.js
+labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js
 labextension/autodownload/static/style.js
 labextension/autodownload/static/third-party-licenses.json
 labextension/environment-life/package.json
 labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig
-labextension/environment-life/static/248.644879940d9faca2b389.js
+labextension/environment-life/static/248.19732aba6894a502e197.js
 labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js
-labextension/environment-life/static/remoteEntry.c977e6e35771b75265ee.js
+labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js
 labextension/environment-life/static/style.js
 labextension/environment-life/static/third-party-licenses.json
 labextension/environment-registration/package.json
 labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json
 labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig
 labextension/environment-registration/static/542.feae6c397f33f9138fea.js
 labextension/environment-registration/static/638.36e464d3233849b6b07a.js
 labextension/environment-registration/static/638.36e464d3233849b6b07a.js.LICENSE.txt
-labextension/environment-registration/static/784.f151a96d5dde1a095c86.js
-labextension/environment-registration/static/remoteEntry.5a586807c39202b9c488.js
+labextension/environment-registration/static/784.201d6fbbedd26339ab72.js
+labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js
 labextension/environment-registration/static/style.js
 labextension/environment-registration/static/third-party-licenses.json
 labextension/gallerymenu/package.json
 labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig
-labextension/gallerymenu/static/542.18fd91d86aaf6286edd0.js
-labextension/gallerymenu/static/56.a4862cb4315ce0eea068.js
+labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js
 labextension/gallerymenu/static/638.95e0186307171588df5b.js
 labextension/gallerymenu/static/638.95e0186307171588df5b.js.LICENSE.txt
-labextension/gallerymenu/static/remoteEntry.f6acbd64cdadb94c1dff.js
+labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js
 labextension/gallerymenu/static/style.js
 labextension/gallerymenu/static/third-party-licenses.json
 labextension/inject-uuid/package.json
 labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig
-labextension/inject-uuid/static/568.0616ffe42e5ee3230288.js
-labextension/inject-uuid/static/remoteEntry.6def7b207d91856938f3.js
+labextension/inject-uuid/static/568.bde16f9395a112a349ee.js
+labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js
 labextension/inject-uuid/static/style.js
 labextension/inject-uuid/static/third-party-licenses.json
 labextension/instrumentation/package.json
 labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/instrumentation.json
 labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig
-labextension/instrumentation/static/568.7f1ab65a55b54297cd7b.js
+labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js
 labextension/instrumentation/static/638.b95125ed695cee42aae4.js
 labextension/instrumentation/static/638.b95125ed695cee42aae4.js.LICENSE.txt
 labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js
-labextension/instrumentation/static/remoteEntry.ae4d1ce402e6ac0dddb5.js
+labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js
 labextension/instrumentation/static/style.js
 labextension/instrumentation/static/third-party-licenses.json
 labextension/userpreferences/package.json
 labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig
 labextension/userpreferences/static/542.d1718a50e23f3808ba62.js
-labextension/userpreferences/static/568.0ac7cbac0996e718a0d9.js
+labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js
 labextension/userpreferences/static/638.e5080f99954048969f76.js
 labextension/userpreferences/static/638.e5080f99954048969f76.js.LICENSE.txt
-labextension/userpreferences/static/remoteEntry.3f8d9d3f425bc3ff0a80.js
+labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js
 labextension/userpreferences/static/style.js
 labextension/userpreferences/static/third-party-licenses.json
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.960648148148148%*

 * *Differences: {"'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -9,16 +9,14 @@
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
     "description": "NBGallery Auto Download Notebooks that are starred or recently executed",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -27,19 +25,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.1353121aacb4a50d2fe1.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../labextension/autodownload",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -71,9 +64,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.1.0"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/schemas/@jupyterlab-nbgallery/autodownload/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8462962962962962%*

 * *Differences: {"'dependencies'": "{'ts-md5': '^1.2.9'}",*

 * * "'description'": "'Track cell execution Metrics'",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/instrumentation'}",*

 * * "'name'": "'@jupyterlab-nbgallery/instrumentation'",*

 * * "'version'": "'2.1.0'",*

 * * 'delete': "['style']"}*

```diff
@@ -3,22 +3,21 @@
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/coreutils": ">=5.2.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0"
+        "jquery": "^3.5.0",
+        "ts-md5": "^1.2.9"
     },
-    "description": "NBGallery Auto Download Notebooks that are starred or recently executed",
+    "description": "Track cell execution Metrics",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -28,25 +27,25 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "../labextension/autodownload",
+        "outputDir": "../labextension/instrumentation",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/autodownload",
+    "name": "@jupyterlab-nbgallery/instrumentation",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -64,11 +63,10 @@
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
-    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "2.1.0"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/542.51fb91347d8a3d9a657a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/568.017b32a913356ad383e7.js` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/568.8bc32e058afbf3d8a017.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,46 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_autodownload = self.webpackChunk_jupyterlab_nbgallery_autodownload || []).push([
     [568], {
         568: (e, o, t) => {
             t.r(o), t.d(o, {
-                default: () => s
+                default: () => l
             });
-            var n = t(225),
-                a = t(281),
-                c = t(569),
-                r = t.n(c);
-            const s = {
+            var n = t(38),
+                a = t(142),
+                r = t(569),
+                c = t.n(r);
+            const l = {
                 id: "@jupyterlab-nbgallery/autodownload",
                 autoStart: !0,
                 requires: [n.ISettingRegistry],
                 activate: async (e, o) => {
                     let t = "",
                         n = 0,
-                        c = !1;
+                        r = !1;
 
-                    function s() {
+                    function l() {
                         return a.PageConfig.getBaseUrl()
                     }
 
-                    function l(e, o, t) {
-                        r().ajax({
+                    function s(e, o, t) {
+                        c().ajax({
                             method: "GET",
                             headers: {
                                 Accept: "application/json"
                             },
                             url: e,
                             cache: !1,
                             xhrFields: {
                                 withCredentials: !0
                             },
                             success: function(e) {
                                 !async function(e, o, t) {
-                                    r().ajax({
-                                        url: s() + "post/" + e + "/" + encodeURIComponent(o) + ".ipynb",
+                                    c().ajax({
+                                        url: l() + "post/" + e + "/" + encodeURIComponent(o) + ".ipynb",
                                         type: "POST",
                                         success: function() {},
                                         error: function(e) {
                                             console.error("Failed upload: " + o)
                                         },
                                         data: JSON.stringify({
                                             type: "notebook",
@@ -49,72 +49,79 @@
                                     })
                                 }(o, t, e)
                             }
                         })
                     }
 
                     function i(e, o, t) {
-                        r().ajax({
+                        c().ajax({
                             method: "GET",
-                            url: s() + "api/contents/" + encodeURIComponent(e),
+                            url: l() + "api/contents/" + encodeURIComponent(e),
                             cache: !1,
                             xhrFields: {
                                 withCredentials: !0
                             },
                             success: function(e) {},
                             error: function(n) {
-                                console.info("Downloading notebooks to " + e), r().ajax({
+                                console.info("Downloading notebooks to " + e), c().ajax({
                                     method: "POST",
-                                    url: s() + "post/" + encodeURIComponent(e),
+                                    url: l() + "post/" + encodeURIComponent(e),
                                     data: JSON.stringify({
                                         type: "directory"
                                     }),
                                     cache: !1,
                                     success: function(n) {
-                                        r().ajax({
+                                        c().ajax({
                                             method: "GET",
                                             headers: {
                                                 Accept: "application/json"
                                             },
                                             url: o + t,
                                             cache: !1,
                                             xhrFields: {
                                                 withCredentials: !0
                                             },
                                             success: function(t) {
                                                 let n;
                                                 for (n in t) {
                                                     var a = t[n];
-                                                    l(o + "/notebooks/" + a.uuid + "/download?clickstream=false", e, a.title.replace(/\//g, "⁄"))
+                                                    s(o + "/notebooks/" + a.uuid + "/download?clickstream=false", e, a.title.replace(/\//g, "⁄"))
                                                 }
                                             }
                                         })
                                     }
                                 })
                             }
                         })
                     }
-                    Promise.all([e.restored, o.load("@jupyterlab-nbgallery/autodownload:autodownload")]).then((([, e]) => {
+                    Promise.all([e.restored, o.load("@jupyterlab-nbgallery/autodownload:autodownload")]).then((([, a]) => {
                         try {
-                            ! function(e) {
-                                r().ajax({
+                            ! function(a) {
+                                c().ajax({
                                     method: "GET",
                                     headers: {
                                         Accept: "application/json"
                                     },
-                                    url: s() + "jupyterlab_nbgallery/environment",
+                                    url: l() + "jupyterlab_nbgallery/environment",
                                     cache: !1,
                                     xhrFields: {
                                         withCredentials: !0
                                     },
-                                    success: function(o) {
-                                        t = o.NBGALLERY_URL, n = o.NBGALLERY_ENABLE_AUTODOWNLOAD, c = e.get("enabled").composite, console.info("Auto Downloading Notebooks"), (1 == n || c) && (i("Starred", t, "/notebooks/stars"), i("Recently Executed", t, "/notebooks/recently_executed"))
+                                    success: function(c) {
+                                        try {
+                                            Promise.all([e.restored, o.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
+                                                t = e.get("nbgallery_url").composite
+                                            }))
+                                        } catch (e) {
+                                            t = c.NBGALLERY_URL
+                                        }
+                                        n = c.NBGALLERY_ENABLE_AUTODOWNLOAD, r = a.get("enabled").composite, console.info("Auto Downloading Notebooks"), (1 == n || r) && (i("Starred", t, "/notebooks/stars"), i("Recently Executed", t, "/notebooks/recently_executed"))
                                     }
                                 })
-                            }(e)
+                            }(a)
                         } catch (e) {
                             console.error(`Problem downloading notebooks \n ${e}`)
                         }
                     }))
                 }
             }
         }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/638.0ed295d9378dea7c5c7b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/remoteEntry.1353121aacb4a50d2fe1.js` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/remoteEntry.77e4acbd8dd372ff3fad.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, d, s, f, p, c, h, b, v, g, y = {
+    var e, r, t, n, o, a, i, l, u, d, f, s, p, c, h, b, v, g, y = {
             735: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(542).then((() => () => t(542)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,50 +44,50 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "51fb91347d8a3d9a657a",
-        568: "017b32a913356ad383e7",
+        568: "8bc32e058afbf3d8a017",
         638: "0ed295d9378dea7c5c7b"
     } [e] + ".js?v=" + {
         542: "51fb91347d8a3d9a657a",
-        568: "017b32a913356ad383e7",
+        568: "8bc32e058afbf3d8a017",
         638: "0ed295d9378dea7c5c7b"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/autodownload:", w.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var s = u[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var s = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -109,15 +109,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-nbgallery/autodownload", "1.0.3", (() => w.e(568).then((() => () => w(568))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-nbgallery/autodownload", "1.1.0", (() => w.e(568).then((() => () => w(568))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -166,33 +166,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > n && !o : "" == s != o);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (f == s)
+                    if (s == f)
                         if (l <= n) {
                             if (d != e[l]) return !1
                         } else {
                             if (o ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < f != o) return !1;
+                    if (l <= n || f < s != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -203,30 +203,30 @@
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), f(e[t][o])
-    }, s = (e, r, t) => {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), s(e[t][o])
+    }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
+    }, s = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
         var a = w.I(r);
         return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
-        var a = r && w.o(r, t) && s(r, t, n);
-        return a ? f(a) : o()
+        var a = r && w.o(r, t) && f(r, t, n);
+        return a ? s(a) : o()
     })), b = {}, v = {
-        225: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 0]),
-        281: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
+        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638)))))
     }, g = {
-        568: [225, 281, 569]
+        568: [38, 142, 569]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
             if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/autodownload/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8876157407407407%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/coreutils': '>=5.2.0', '@jupyterlab/services': '>=6.6.0'}",*

 * * "'description'": "'Register NBGallery Environment'",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'files'": "{insert: [(2, 'schema/**/*.json')]}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/environment-registration', '_build': {'load': "*

 * *                 "'static/remoteEntry.54aae520a7b7fc99d9fd.js'}}",*

 * * "'name'": "'@jupyterlab-nbgallery/environment-r […]*

```diff
@@ -1,55 +1,56 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
+        "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
-    "description": "Allow an expiration data to be displayed in the bottom right corner when operating in an environment where jupyter instances have a defined lifetime.",
+    "description": "Register NBGallery Environment",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c977e6e35771b75265ee.js",
+            "load": "static/remoteEntry.54aae520a7b7fc99d9fd.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../labextension/environment-life",
+        "outputDir": "../labextension/environment-registration",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/environment-life",
+    "name": "@jupyterlab-nbgallery/environment-registration",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -69,9 +70,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "1.0.5"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.887037037037037%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/coreutils': '>=5.2.0', '@jupyterlab/services': '>=6.6.0'}",*

 * * "'description'": "'Register NBGallery Environment'",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'files'": "{insert: [(2, 'schema/**/*.json')]}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/environment-registration'}",*

 * * "'name'": "'@jupyterlab-nbgallery/environment-registration'",*

 * * "'version'": "'1.0.5'"}*

```diff
@@ -1,50 +1,51 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
+        "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
-    "description": "Allow an expiration data to be displayed in the bottom right corner when operating in an environment where jupyter instances have a defined lifetime.",
+    "description": "Register NBGallery Environment",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "../labextension/environment-life",
+        "outputDir": "../labextension/environment-registration",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/environment-life",
+    "name": "@jupyterlab-nbgallery/environment-registration",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -64,9 +65,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "1.0.5"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/248.644879940d9faca2b389.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/248.19732aba6894a502e197.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_environment_life = self.webpackChunk_jupyterlab_nbgallery_environment_life || []).push([
     [248], {
         248: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => s
+                default: () => l
             });
-            var r = n(144),
-                i = n(791),
-                o = n(281),
-                a = n(530);
-            const s = {
+            var r = n(832),
+                i = n(583),
+                o = n(142),
+                a = n(820);
+            const l = {
                 id: "@jupyterlab-nbgallery/environment-life",
                 autoStart: !0,
                 requires: [i.IStatusBar],
                 activate: async (e, t) => {
                     let n = "";
                     try {
                         const e = await async function(e = "", t = {}) {
@@ -21,35 +21,30 @@
                                 r = o.URLExt.join(n.baseUrl, "jupyterlab_nbgallery", e);
                             let i;
                             try {
                                 i = await a.ServerConnection.makeRequest(r, t, n)
                             } catch (e) {
                                 throw new a.ServerConnection.NetworkError(e)
                             }
-                            const s = await i.json();
-                            if (!i.ok) throw new a.ServerConnection.ResponseError(i, s.message);
-                            return s
+                            const l = await i.json();
+                            if (!i.ok) throw new a.ServerConnection.ResponseError(i, l.message);
+                            return l
                         }("expiration");
                         n = e.NBGALLERY_TERMINATION_TIME,
                             function() {
                                 if (console.log(`termination Time: ${n}`), n && n.length > 0) {
                                     let e = new Date(n + " UTC");
-                                    const r = new l;
-                                    r.node.textContent = "Expires: " + e.toLocaleString(), t.registerStatusItem("bench-expiration", {
+                                    const i = new r.Widget;
+                                    i.title.label = "Jupyter Environment Expires", i.addClass("jp-expiration-widget"), i.id = "environment_expires", i.node.textContent = "Expires: " + e.toLocaleString(), t.registerStatusItem("bench-expiration", {
                                         align: "right",
-                                        item: r
+                                        item: i
                                     })
                                 }
                             }()
                     } catch (e) {
                         console.error(`ERROR on get /jupyter_nbgallery/environment.\n ${e}`)
                     }
                 }
-            };
-            class l extends r.Widget {
-                constructor() {
-                    super(), this.addClass("jp-expiration-widget"), this.id = "environment_expires", this.title.label = "Jupyter Environment Expires"
-                }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/542.e4d405f3b0e4f693ab53.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/remoteEntry.c977e6e35771b75265ee.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/remoteEntry.fe9e40141faed985c15b.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -43,18 +43,18 @@
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + "." + {
-        248: "644879940d9faca2b389",
+        248: "19732aba6894a502e197",
         542: "e4d405f3b0e4f693ab53"
     } [e] + ".js?v=" + {
-        248: "644879940d9faca2b389",
+        248: "19732aba6894a502e197",
         542: "e4d405f3b0e4f693ab53"
     } [e], g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (o[r] = {
                         get: () => g.e(248).then((() => () => g(248))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab-nbgallery/environment-life", "0.2.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@jupyterlab-nbgallery/environment-life", "0.2.4"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -205,20 +205,20 @@
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), s(e[t][o])
     }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        144: () => d("default", "@lumino/widgets", [1, 2, 0, 0]),
-        281: () => d("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
-        530: () => d("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 0]),
-        791: () => d("default", "@jupyterlab/statusbar", [1, 4, 0, 0, , "beta", 0])
+        142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        583: () => d("default", "@jupyterlab/statusbar", [1, 3, 6, 3]),
+        820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
     }, h = {
-        248: [144, 281, 530, 791]
+        248: [142, 583, 820, 832]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
             if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-life/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.829122150997151%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/notebook': '>=3.6.0', delete: ['@jupyterlab/coreutils']}",*

 * * "'description'": "'Inject the notebook UUID into the kernel.'",*

 * * "'devDependencies'": "{'prettier': '>=1.13.0', delete: ['@typescript-eslint/eslint-plugin', "*

 * *                      "'@typescript-eslint/parser']}",*

 * * "'files'": '{delete: [2]}',*

 * * "'jupyterlab'": "{'outputDir': '../labextension/inject-uuid', '_build': {'load': "*

 * *                 "'static/remoteEntry.f32354aac49e7b8ba738.js', delete: ['style']}}",*

 * * "'na […]*

```diff
@@ -1,57 +1,54 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
-        "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
-    "description": "Register NBGallery Environment",
+    "description": "Inject the notebook UUID into the kernel.",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
+        "prettier": ">=1.13.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/**/*.json"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5a586807c39202b9c488.js",
-            "style": "./style"
+            "load": "static/remoteEntry.f32354aac49e7b8ba738.js"
         },
         "extension": true,
-        "outputDir": "../labextension/environment-registration",
+        "outputDir": "../labextension/inject-uuid",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/environment-registration",
+    "name": "@jupyterlab-nbgallery/inject-uuid",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -69,11 +66,10 @@
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
-    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "2.0.1"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/environment-registration.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/schemas/@jupyterlab-nbgallery/environment-registration/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/autodownload/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9016203703703702%*

 * *Differences: {"'description'": "'NBGallery Auto Download Notebooks that are starred or recently executed'",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/autodownload', '_build': OrderedDict([('load', "*

 * *                 "'static/remoteEntry.77e4acbd8dd372ff3fad.js'), ('extension', './extension'), "*

 * *                 "('style', './style')])}",*

 * * "'name'": "'@jupyterlab-nbgallery/autodownload'",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -5,20 +5,18 @@
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/coreutils": ">=5.2.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
-    "description": "Register NBGallery Environment",
+    "description": "NBGallery Auto Download Notebooks that are starred or recently executed",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -27,26 +25,31 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.77e4acbd8dd372ff3fad.js",
+            "style": "./style"
+        },
         "extension": true,
-        "outputDir": "../labextension/environment-registration",
+        "outputDir": "../labextension/autodownload",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/environment-registration",
+    "name": "@jupyterlab-nbgallery/autodownload",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -66,9 +69,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.1.0"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/542.feae6c397f33f9138fea.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/542.feae6c397f33f9138fea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/638.36e464d3233849b6b07a.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/638.36e464d3233849b6b07a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/784.f151a96d5dde1a095c86.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/784.201d6fbbedd26339ab72.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,57 +1,61 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_environment_registration = self.webpackChunk_jupyterlab_nbgallery_environment_registration || []).push([
     [784], {
         784: (e, n, t) => {
             t.r(n), t.d(n, {
                 default: () => s
             });
-            var r = t(225),
-                a = t(281),
-                o = t(530),
+            var r = t(38),
+                o = t(142),
+                a = t(820),
                 i = t(569),
                 l = t.n(i);
             const s = {
                 id: "@jupyterlab-nbgallery/environment-registration",
                 autoStart: !0,
                 requires: [r.ISettingRegistry],
                 activate: async (e, n) => {
                     let t = !1,
                         r = "",
-                        i = "";
+                        i = "",
+                        s = "",
+                        g = "";
                     try {
                         const e = await async function(e = "", n = {}) {
-                            const t = o.ServerConnection.makeSettings(),
-                                r = a.URLExt.join(t.baseUrl, "jupyterlab_nbgallery", e);
+                            const t = a.ServerConnection.makeSettings(),
+                                r = o.URLExt.join(t.baseUrl, "jupyterlab_nbgallery", e);
                             let i;
                             try {
-                                i = await o.ServerConnection.makeRequest(r, n, t)
+                                i = await a.ServerConnection.makeRequest(r, n, t)
                             } catch (e) {
-                                throw new o.ServerConnection.NetworkError(e)
+                                throw new a.ServerConnection.NetworkError(e)
                             }
                             const l = await i.json();
-                            if (!i.ok) throw new o.ServerConnection.ResponseError(i, l.message);
+                            if (!i.ok) throw new a.ServerConnection.ResponseError(i, l.message);
                             return l
                         }("environment");
-                        r = e.NBGALLERY_URL, i = e.NBGALLERY_CLIENT_NAME
+                        s = e.NBGALLERY_URL, g = e.NBGALLERY_CLIENT_NAME
                     } catch (e) {
                         console.error(`ERROR on get /jupyter_nbgallery/environment.\n ${e}`)
                     }
                     Promise.all([e.restored, n.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
                         ! function(e) {
-                            r && r.length > 0 ? e.set("nbgallery_url", r) : r = e.get("nbgallery_url").composite, i && i.length > 0 ? e.set("nbgallery_client_name", i) : i = e.get("nbgallery_client_name").composite, t = e.get("registered").composite, !t && r && r.length > 0 && l().ajax({
+                            r = e.get("nbgallery_url").composite, (!r || 0 == r.length) && s && s.length > 0 && (r = s, e.set("nbgallery_url", r)), i = e.get("nbgallery_client_name").composite, (!i || 0 == i.length) && g && g.length > 0 && (i = g, e.set("nbgallery_client_name", i)), t = e.get("registered").composite;
+                            let n = "lab";
+                            "" != o.PageConfig.getOption("notebookPage") && (n = "notebook"), !t && r && r.length > 0 && l().ajax({
                                 method: "POST",
                                 headers: {
                                     Accept: "application/json"
                                 },
                                 url: r + "/environments",
                                 data: {
                                     name: i,
-                                    url: a.PageConfig.getBaseUrl(),
-                                    user_interface: "lab"
+                                    url: o.PageConfig.getBaseUrl(),
+                                    user_interface: n
                                 },
                                 xhrFields: {
                                     withCredentials: !0
                                 },
                                 success: function(n) {
                                     e.set("registered", !0), console.log("Environment Registered to NBGallery")
                                 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/remoteEntry.5a586807c39202b9c488.js` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/remoteEntry.54aae520a7b7fc99d9fd.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, s, f, d, c, p, h, v, g, b, y = {
+    var e, r, t, n, o, a, i, l, u, s, d, f, p, c, h, v, g, b, y = {
             374: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(784).then((() => () => t(784))),
                         "./extension": () => t.e(784).then((() => () => t(784))),
                         "./style": () => t.e(542).then((() => () => t(542)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         m = {};
 
     function w(e) {
         var r = m[e];
@@ -45,79 +45,79 @@
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "feae6c397f33f9138fea",
         638: "36e464d3233849b6b07a",
-        784: "f151a96d5dde1a095c86"
+        784: "201d6fbbedd26339ab72"
     } [e] + ".js?v=" + {
         542: "feae6c397f33f9138fea",
         638: "36e464d3233849b6b07a",
-        784: "f151a96d5dde1a095c86"
+        784: "201d6fbbedd26339ab72"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/environment-registration:", w.l = (t, n, a, o) => {
+    }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/environment-registration:", w.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== a)
+            if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var f = u[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
-                        i = f;
+                    var d = u[s];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
+                        i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         w.S = {};
         var e = {},
             r = {};
         w.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
-                var o = w.S[t],
+                var a = w.S[t],
                     i = "@jupyterlab-nbgallery/environment-registration",
                     l = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            l = a[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            l = o[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@jupyterlab-nbgallery/environment-registration", "1.0.3", (() => w.e(784).then((() => () => w(784))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@jupyterlab-nbgallery/environment-registration", "1.0.5", (() => w.e(784).then((() => () => w(784))))), l("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -131,153 +131,153 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 l = (typeof i)[0];
-            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
+        for (a = 1; a < e.length; a++) {
+            var l = e[a];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
         return u();
 
         function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var s, f, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
-                if ("u" == f) {
-                    if (!u || "u" != d) return !1
+                var s, d, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == d) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (d == f)
+                    if (f == d)
                         if (l <= n) {
                             if (s != e[l]) return !1
                         } else {
-                            if (a ? s > e[l] : s < e[l]) return !1;
+                            if (o ? s > e[l] : s < e[l]) return !1;
                             s != e[l] && (u = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (a || l <= n) return !1;
+                else if ("s" != f && "n" != f) {
+                    if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || f < d != a) return !1;
+                    if (l <= n || d < f != o) return !1;
                     u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), d(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
-        var o = w.I(r);
-        return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && f(r, t, n);
-        return o ? d(o) : a()
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+        var o = l(e, t);
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(u(e, t, o, n)), f(e[t][o])
+    }, d = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, o) {
+        var a = w.I(r);
+        return a && a.then ? a.then(e.bind(e, r, w.S[r], t, n, o)) : e(r, w.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, o) => {
+        var a = r && w.o(r, t) && d(r, t, n);
+        return a ? f(a) : o()
     })), v = {}, g = {
-        225: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 0]),
-        281: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
-        530: () => p("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 0]),
-        569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638)))))
+        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
+        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3])
     }, b = {
-        784: [225, 281, 530, 569]
+        784: [38, 142, 569, 820]
     }, w.f.consumes = (e, r) => {
         w.o(b, e) && b[e].forEach((e => {
             if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var a = g[e]();
-                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                var o = g[e]();
+                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             908: 0
         };
         w.f.j = (r, t) => {
             var n = w.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = w.p + w.u(r),
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = w.p + w.u(r),
                         i = new Error;
-                    w.l(o, (t => {
+                    w.l(a, (t => {
                         if (w.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, l] = t,
+                var n, o, [a, i, l] = t,
                     u = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) w.o(i, n) && (w.m[n] = i[n]);
                     l && l(w)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], w.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyterlab_nbgallery_environment_registration = self.webpackChunk_jupyterlab_nbgallery_environment_registration || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), w.nc = void 0;
     var j = w(374);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab-nbgallery/environment-registration"] = j
 })();
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/environment-registration/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-registration/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9276620370370371%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/mainmenu': '>=3.6.0 ||', delete: ['fa-icons']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '>=3.3.2', delete: "*

 * *                      "['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/userpreferences', '_build': {'load': "*

 * *                 "'static/remoteEntry.0c562dfea5f20371ffe8.js'}}",*

 * * "'name'": "'@jupyterlab-nbgallery/userpreferences'",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -1,26 +1,23 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
-        "@jupyterlab/mainmenu": ">=3.6.0",
+        "@jupyterlab/mainmenu": ">=3.6.0 ||",
         "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "fa-icons": "^0.2.0",
         "jquery": "^3.5.0"
     },
     "description": "All the menu capabilities needed for saving/forking notebooks and submitting change request to Notebook Gallery",
     "devDependencies": {
-        "@jupyterlab/builder": ">=3.6.0",
+        "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -31,29 +28,29 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f6acbd64cdadb94c1dff.js",
+            "load": "static/remoteEntry.0c562dfea5f20371ffe8.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../labextension/gallerymenu",
+        "outputDir": "../labextension/userpreferences",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/gallerymenu",
+    "name": "@jupyterlab-nbgallery/userpreferences",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -73,9 +70,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "1.0.2"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/schemas/@jupyterlab-nbgallery/gallerymenu/package.json.orig`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8518518518518517%*

 * *Differences: {"'dependencies'": "{delete: ['fa-icons']}",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'version'": "'2.0.2'",*

 * * 'delete': "['style', 'sideEffects']"}*

```diff
@@ -4,23 +4,20 @@
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/mainmenu": ">=3.6.0",
         "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "fa-icons": "^0.2.0",
         "jquery": "^3.5.0"
     },
     "description": "All the menu capabilities needed for saving/forking notebooks and submitting change request to Notebook Gallery",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.6.0",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -63,14 +60,10 @@
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "sideEffects": [
-        "style/*.css"
-    ],
-    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.2"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/542.18fd91d86aaf6286edd0.js` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/542.d1718a50e23f3808ba62.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 "use strict";
-(self.webpackChunk_jupyterlab_nbgallery_gallerymenu = self.webpackChunk_jupyterlab_nbgallery_gallerymenu || []).push([
+(self.webpackChunk_jupyterlab_nbgallery_userpreferences = self.webpackChunk_jupyterlab_nbgallery_userpreferences || []).push([
     [542], {
         230: (e, n, t) => {
             t.d(n, {
                 Z: () => a
             });
             var r = t(476),
                 o = t.n(r)()((function(e) {
@@ -76,27 +76,27 @@
                     } return n
             }
 
             function l(e, n) {
                 for (var t = {}, r = [], o = 0; o < e.length; o++) {
                     var l = e[o],
                         c = n.base ? l[0] + n.base : l[0],
-                        u = t[c] || 0,
-                        s = "".concat(c, " ").concat(u);
-                    t[c] = u + 1;
-                    var f = i(s),
+                        s = t[c] || 0,
+                        u = "".concat(c, " ").concat(s);
+                    t[c] = s + 1;
+                    var f = i(u),
                         d = {
                             css: l[1],
                             media: l[2],
                             sourceMap: l[3]
                         }; - 1 !== f ? (a[f].references++, a[f].updater(d)) : a.push({
-                        identifier: s,
+                        identifier: u,
                         updater: b(d, n),
                         references: 1
-                    }), r.push(s)
+                    }), r.push(u)
                 }
                 return r
             }
 
             function c(e) {
                 var n = document.createElement("style"),
                     r = e.attributes || {};
@@ -110,21 +110,21 @@
                 else {
                     var i = o(e.insert || "head");
                     if (!i) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                     i.appendChild(n)
                 }
                 return n
             }
-            var u, s = (u = [], function(e, n) {
-                return u[e] = n, u.filter(Boolean).join("\n")
+            var s, u = (s = [], function(e, n) {
+                return s[e] = n, s.filter(Boolean).join("\n")
             });
 
             function f(e, n, t, r) {
                 var o = t ? "" : r.media ? "@media ".concat(r.media, " {").concat(r.css, "}") : r.css;
-                if (e.styleSheet) e.styleSheet.cssText = s(n, o);
+                if (e.styleSheet) e.styleSheet.cssText = u(n, o);
                 else {
                     var a = document.createTextNode(o),
                         i = e.childNodes;
                     i[n] && e.removeChild(i[n]), i.length ? e.insertBefore(a, i[n]) : e.appendChild(a)
                 }
             }
 
@@ -165,17 +165,17 @@
                 var t = l(e = e || [], n);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
                         for (var r = 0; r < t.length; r++) {
                             var o = i(t[r]);
                             a[o].references--
                         }
-                        for (var c = l(e, n), u = 0; u < t.length; u++) {
-                            var s = i(t[u]);
-                            0 === a[s].references && (a[s].updater(), a.splice(s, 1))
+                        for (var c = l(e, n), s = 0; s < t.length; s++) {
+                            var u = i(t[s]);
+                            0 === a[u].references && (a[u].updater(), a.splice(u, 1))
                         }
                         t = c
                     }
                 }
             }
         }
     }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/56.a4862cb4315ce0eea068.js` & `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/56.2f2a1bce28a94a6668e1.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,61 +1,64 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_gallerymenu = self.webpackChunk_jupyterlab_nbgallery_gallerymenu || []).push([
     [56], {
         56: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => k
+                default: () => y
             });
-            var l = a(551),
-                i = a(678),
-                o = a(144),
-                n = a(598),
-                s = a(530),
-                r = a(281),
-                d = a(29);
-            class h extends i.ReactWidget {
+            var l = a(344),
+                i = a(33),
+                o = a(832),
+                n = a(123),
+                s = a(820),
+                r = a(142),
+                d = a(38),
+                h = a(271);
+            class u extends i.ReactWidget {
                 constructor() {
                     super(), this.addClass("jp-ReactWidget")
                 }
                 render() {
-                    return d.createElement("div", {
+                    return h.createElement("div", {
                         dangerouslySetInnerHTML: {
                             __html: this.content
                         }
                     })
                 }
             }
-            var u = a(569),
-                c = a.n(u);
-            const g = {
+            var c = a(569),
+                g = a.n(c);
+            const b = {
                 id: "@jupyterlab-nbgallery/gallerymenu",
                 autoStart: !0,
-                requires: [l.IMainMenu, n.INotebookTracker],
-                activate: function(e, t, a) {
-                    if (!a) return;
-                    let l = r.PageConfig.getOption("retroPage");
-                    switch ("" == l && (l = r.PageConfig.getOption("notebookPage")), l) {
-                        case "tree":
-                        case "terminals":
-                        case "consoles":
-                            return
+                requires: [l.IMainMenu, n.INotebookTracker, d.ISettingRegistry],
+                activate: function(e, t, a, l) {
+                    if (a) {
+                        switch (r.PageConfig.getOption("notebookPage")) {
+                            case "tree":
+                            case "terminals":
+                            case "consoles":
+                                return
+                        }
+                        new k(e, t, a, l)
                     }
-                    new b(e, t, a).initialize()
                 }
             };
-            class b {
-                constructor(e, t, a) {
-                    this.dialogPromiseCache = new Map, this.gallery_url = "", this.app = e, this.mainMenu = t, this.notebooks = a
+            class k {
+                constructor(e, t, a, l) {
+                    this.dialogPromiseCache = new Map, this.gallery_url = "", this.app = e, this.mainMenu = t, this.notebooks = a, this.settingsRegistry = l, Promise.all([this.app.restored, this.settingsRegistry.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
+                        this.settings = e, this.initialize()
+                    }))
                 }
                 async initialize() {
-                    await Promise.all([this.app.restored]);
                     const e = s.ServerConnection.makeSettings(),
                         t = r.URLExt.join(e.baseUrl, "jupyterlab_nbgallery", "environment");
+                    this.gallery_url = this.settings.get("nbgallery_url").composite;
                     let a = this;
-                    await c().ajax({
+                    await g().ajax({
                         method: "GET",
                         headers: {
                             Accept: "application/json"
                         },
                         url: t,
                         cache: !1,
                         xhrFields: {
@@ -88,28 +91,66 @@
                     for (a in t.cells) "code" == t.cells[a].cell_type ? (t.cells[a].outputs = [], t.cells[a].execution_count = null) : null != t.cells[a].outputs && delete t.cells[a].outputs;
                     return t
                 }
                 async checkForUpdates(e, t) {
                     let a = this.getGalleryMetadata(e);
                     try {
                         let e = r.URLExt.join(t.origin, "notebooks", a.uuid, "metadata");
-                        return (await c().ajax({
+                        return (await g().ajax({
                             method: "GET",
                             url: e,
                             headers: {
                                 Accept: "application/json"
                             },
                             xhrFields: {
                                 withCredentials: !0
                             }
                         })).commit_id != a.commit
                     } catch (e) {
                         (0, i.showErrorMessage)("Staging Failed", "An error occured checking for updates to the specified notebook.  Please ensure that you are logged in to the Gallery.")
                     }
                 }
+                async diffCallback() {
+                    let e = [],
+                        t = this.getGalleryLink(),
+                        a = this.currentNotebook(),
+                        l = this.getGalleryMetadata(a);
+                    e[e.length] = i.Dialog.cancelButton({
+                        label: "Close"
+                    });
+                    let o = new u,
+                        n = await g().ajax({
+                            method: "POST",
+                            url: t.origin + "/notebooks/" + l.uuid + "/diff",
+                            dataType: "json",
+                            contentType: "text/plain",
+                            headers: {
+                                accept: "application/json"
+                            },
+                            data: JSON.stringify(this.stripOutput(a)),
+                            xhrFields: {
+                                withCredentials: !0
+                            }
+                        });
+                    n.different ? o.content = n.css + n.inline : o.content = "<div>No Changes</div>";
+                    const s = l.uuid + "changedDialog",
+                        r = this.dialogPromiseCache.get(s);
+                    if (r) return r; {
+                        const t = (0, i.showDialog)({
+                            title: "Diff with Remote Notebook",
+                            body: o,
+                            buttons: e
+                        }).then((async e => {
+                            this.dialogPromiseCache.delete(s)
+                        }), (e => {
+                            throw this.dialogPromiseCache.delete(s), e
+                        }));
+                        return this.dialogPromiseCache.set(s, t), t
+                    }
+                }
                 async changedDialog(e) {
                     let t = [],
                         a = this.getGalleryLink(),
                         l = this.currentNotebook(),
                         o = this.getGalleryMetadata(l);
                     t[t.length] = i.Dialog.cancelButton({
                         label: "Cancel"
@@ -118,17 +159,17 @@
                     })), t[t.length] = i.Dialog.okButton({
                         label: "Download and Replace Local",
                         displayType: "warn"
                     }), o.link && (t[t.length] = i.Dialog.okButton({
                         label: "Upload and Replace Remote",
                         displayType: "warn"
                     }));
-                    let n = new h;
+                    let n = new u;
                     if (e) {
-                        let e = await c().ajax({
+                        let e = await g().ajax({
                             method: "POST",
                             url: a.origin + "/notebooks/" + o.link + "/diff",
                             dataType: "json",
                             contentType: "text/plain",
                             headers: {
                                 accept: "application/json"
                             },
@@ -159,28 +200,28 @@
                         return this.dialogPromiseCache.set(s, e), e
                     }
                 }
                 async downloadReplace(e, t) {
                     let a = this.getGalleryMetadata(e),
                         l = r.URLExt.join(t.origin, "notebooks", a.uuid, "download");
                     try {
-                        let t = await c().ajax({
+                        let t = await g().ajax({
                                 url: l
                             }),
                             i = JSON.parse(t);
                         a.link && (i.metadata.gallery.link = a.link, i.metadata.gallery.clone = null), e.model.fromJSON(i), this.triggerSave()
                     } catch (e) {
                         (0, i.showErrorMessage)("Download Error", "An error occured attempting to download the specified notebook.")
                     }
                 }
                 async stageNotebook(e, t, a) {
                     let l = "";
                     console.log("Attempting to stage"), l = t.origin + "/stages?agree=yes", a && a.length > 0 && (l = l + "&id=" + a);
                     try {
-                        return await c().ajax({
+                        return await g().ajax({
                             method: "POST",
                             url: l,
                             dataType: "json",
                             contentType: "text/plain",
                             headers: {
                                 Accept: "application/json"
                             },
@@ -237,28 +278,28 @@
                         this.linkNotebookIfExsists(this.currentNotebook(), e.value)
                     }))
                 }
                 async linkNotebookIfExsists(e, t) {
                     let a = this;
                     var l = new URL(t);
                     let i = r.URLExt.join(t, "uuid");
-                    c().ajax({
+                    g().ajax({
                         method: "GET",
                         headers: {
                             Accept: "application/json"
                         },
                         url: i,
                         cache: !1,
                         xhrFields: {
                             withCredentials: !0
                         },
                         success: function(t) {
                             if (null != t) {
                                 let i = r.URLExt.join(l.origin, "notebooks", t.uuid, "metadata");
-                                c().ajax({
+                                g().ajax({
                                     method: "GET",
                                     headers: {
                                         Accept: "application/json"
                                     },
                                     url: i,
                                     cache: !1,
                                     xhrFields: {
@@ -372,14 +413,21 @@
                     }), e.addCommand("gallery-checkupdates", {
                         label: "Check for Changes",
                         isEnabled: () => this.hasUUID(),
                         isVisible: () => this.hasUUID(),
                         execute: () => {
                             this.changesCallback()
                         }
+                    }), e.addCommand("gallery-showdiff", {
+                        label: "Show Diff with Gallery",
+                        isEnabled: () => this.hasUUID(),
+                        isVisible: () => this.hasUUID(),
+                        execute: () => {
+                            this.diffCallback()
+                        }
                     }), e.addCommand("gallery-unlink", {
                         label: "Unlink from Gallery",
                         isEnabled: () => this.hasUUID(),
                         isVisible: () => this.hasUUID(),
                         execute: () => {
                             this.unlinkCallback()
                         }
@@ -406,17 +454,19 @@
                     }), t.addItem({
                         command: "gallery-link"
                     }), t.addItem({
                         command: "gallery-unlink"
                     }), t.addItem({
                         command: "gallery-checkupdates"
                     }), t.addItem({
+                        command: "gallery-showdiff"
+                    }), t.addItem({
                         type: "separator"
                     }), t.addItem({
                         command: "gallery-visit"
                     }), t
                 }
             }
-            const k = g
+            const y = b
         }
     }
 ]);
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/638.95e0186307171588df5b.js` & `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/638.95e0186307171588df5b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/remoteEntry.f6acbd64cdadb94c1dff.js` & `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/static/remoteEntry.fadc9f3eb62fb570716e.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, l, i, u, f, s, d, p, c, h, b, v, y, g = {
-            421: (e, r, t) => {
+    var e, r, t, n, a, o, l, u, i, f, s, d, p, c, h, v, b, g, y = {
+            70: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(56).then((() => () => t(56))),
-                        "./extension": () => t.e(56).then((() => () => t(56))),
-                        "./style": () => t.e(542).then((() => () => t(542)))
+                        "./extension": () => t.e(56).then((() => () => t(56)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -27,67 +26,64 @@
         },
         m = {};
 
     function w(e) {
         var r = m[e];
         if (void 0 !== r) return r.exports;
         var t = m[e] = {
-            id: e,
             exports: {}
         };
-        return g[e].call(t.exports, t, t.exports, w), t.exports
+        return y[e].call(t.exports, t, t.exports, w), t.exports
     }
-    w.m = g, w.c = m, w.n = e => {
+    w.m = y, w.c = m, w.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return w.d(r, {
             a: r
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        56: "a4862cb4315ce0eea068",
-        542: "18fd91d86aaf6286edd0",
+        56: "2f2a1bce28a94a6668e1",
         638: "95e0186307171588df5b"
     } [e] + ".js?v=" + {
-        56: "a4862cb4315ce0eea068",
-        542: "18fd91d86aaf6286edd0",
+        56: "2f2a1bce28a94a6668e1",
         638: "95e0186307171588df5b"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/gallerymenu:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
-            var l, i;
+            var l, u;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
+                for (var i = document.getElementsByTagName("script"), f = 0; f < i.length; f++) {
+                    var s = i[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
                         l = s;
                         break
                     }
                 }
-            l || (i = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, w.nc && l.setAttribute("nonce", w.nc), l.setAttribute("data-webpack", r + a), l.src = t), e[t] = [n];
+            l || (u = !0, (l = document.createElement("script")).charset = "utf-8", l.timeout = 120, w.nc && l.setAttribute("nonce", w.nc), l.setAttribute("data-webpack", r + a), l.src = t), e[t] = [n];
             var d = (r, n) => {
                     l.onerror = l.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], l.parentNode && l.parentNode.removeChild(l), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: l
                 }), 12e4);
-            l.onerror = d.bind(null, l.onerror), l.onload = d.bind(null, l.onload), i && document.head.appendChild(l)
+            l.onerror = d.bind(null, l.onerror), l.onload = d.bind(null, l.onload), u && document.head.appendChild(l)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -99,25 +95,25 @@
             n || (n = []);
             var a = r[t];
             if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
                 if (n.push(a), e[t]) return e[t];
                 w.o(w.S, t) || (w.S[t] = {});
                 var o = w.S[t],
                     l = "@jupyterlab-nbgallery/gallerymenu",
-                    i = (e, r, t, n) => {
+                    u = (e, r, t, n) => {
                         var a = o[e] = o[e] || {},
-                            i = a[r];
-                        (!i || !i.loaded && (!n != !i.eager ? n : l > i.from)) && (a[r] = {
+                            u = a[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : l > u.from)) && (a[r] = {
                             get: t,
                             from: l,
                             eager: !!n
                         })
                     },
-                    u = [];
-                return "default" === t && (i("@jupyterlab-nbgallery/gallerymenu", "2.0.0", (() => w.e(56).then((() => () => w(56))))), i("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    i = [];
+                return "default" === t && (u("@jupyterlab-nbgallery/gallerymenu", "2.0.2", (() => w.e(56).then((() => () => w(56))))), u("jquery", "3.6.4", (() => w.e(638).then((() => () => w(638)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -135,119 +131,120 @@
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var a = e[n],
                 o = (typeof a)[0];
             if (n >= r.length) return "u" == o;
             var l = r[n],
-                i = (typeof l)[0];
-            if (o != i) return "o" == o && "n" == i || "s" == i || "u" == o;
+                u = (typeof l)[0];
+            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
             if ("o" != o && "u" != o && a != l) return a < l;
             n++
         }
     }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var l = [];
         for (o = 1; o < e.length; o++) {
-            var i = e[o];
-            l.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? l.pop() + " " + l.pop() : a(i))
+            var u = e[o];
+            l.push(0 === u ? "not(" + i() + ")" : 1 === u ? "(" + i() + " || " + i() + ")" : 2 === u ? l.pop() + " " + l.pop() : a(u))
         }
-        return u();
+        return i();
 
-        function u() {
+        function i() {
             return l.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
-            for (var l = 0, i = 1, u = !0;; i++, l++) {
-                var f, s, d = i < e.length ? (typeof e[i])[0] : "";
-                if (l >= r.length || "o" == (s = (typeof(f = r[l]))[0])) return !u || ("u" == d ? i > n && !a : "" == d != a);
+            for (var l = 0, u = 1, i = !0;; u++, l++) {
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (l >= r.length || "o" == (s = (typeof(f = r[l]))[0])) return !i || ("u" == d ? u > n && !a : "" == d != a);
                 if ("u" == s) {
-                    if (!u || "u" != d) return !1
-                } else if (u)
+                    if (!i || "u" != d) return !1
+                } else if (i)
                     if (d == s)
-                        if (i <= n) {
-                            if (f != e[i]) return !1
+                        if (u <= n) {
+                            if (f != e[u]) return !1
                         } else {
-                            if (a ? f > e[i] : f < e[i]) return !1;
-                            f != e[i] && (u = !1)
+                            if (a ? f > e[u] : f < e[u]) return !1;
+                            f != e[u] && (i = !1)
                         }
                 else if ("s" != d && "n" != d) {
-                    if (a || i <= n) return !1;
-                    u = !1, i--
+                    if (a || u <= n) return !1;
+                    i = !1, u--
                 } else {
-                    if (i <= n || s < d != a) return !1;
-                    u = !1
-                } else "s" != d && "n" != d && (u = !1, i--)
+                    if (u <= n || s < d != a) return !1;
+                    i = !1
+                } else "s" != d && "n" != d && (i = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (l = 1; l < e.length; l++) {
             var h = e[l];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, l = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, i = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
-        var a = i(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(u(e, t, a, n)), d(e[t][a])
+    }, i = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+        var a = u(e, t);
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(i(e, t, a, n)), d(e[t][a])
     }, s = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
     })(((e, r, t, n) => (l(e, t), f(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && s(r, t, n);
         return o ? d(o) : a()
-    })), b = {}, v = {
-        29: () => c("default", "react", [1, 18, 2, 0]),
-        144: () => c("default", "@lumino/widgets", [1, 2, 0, 0]),
-        281: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
-        530: () => c("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 0]),
-        551: () => c("default", "@jupyterlab/mainmenu", [1, 4, 0, 0, , "beta", 0]),
+    })), v = {}, b = {
+        33: () => c("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        38: () => c("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        123: () => c("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        142: () => c("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        271: () => c("default", "react", [1, 17, 0, 1]),
+        344: () => c("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
-        598: () => c("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "beta", 0]),
-        678: () => c("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "beta", 0])
-    }, y = {
-        56: [29, 144, 281, 530, 551, 569, 598, 678]
+        820: () => c("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        832: () => c("default", "@lumino/widgets", [1, 1, 37, 2])
+    }, g = {
+        56: [33, 38, 123, 142, 271, 344, 569, 820, 832]
     }, w.f.consumes = (e, r) => {
-        w.o(y, e) && y[e].forEach((e => {
-            if (w.o(b, e)) return r.push(b[e]);
+        w.o(g, e) && g[e].forEach((e => {
+            if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, w.m[e] = t => {
+                    v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], w.m[e] = t => {
+                    delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var a = b[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             567: 0
@@ -267,21 +264,21 @@
                                 o = t && t.target && t.target.src;
                             l.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", l.name = "ChunkLoadError", l.type = a, l.request = o, n[1](l)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, l, i] = t,
-                    u = 0;
+                var n, a, [o, l, u] = t,
+                    i = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (n in l) w.o(l, n) && (w.m[n] = l[n]);
-                    i && i(w)
+                    u && u(w)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); i < o.length; i++) a = o[i], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_jupyterlab_nbgallery_gallerymenu = self.webpackChunk_jupyterlab_nbgallery_gallerymenu || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), w.nc = void 0;
-    var j = w(421);
+    })();
+    var j = w(70);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab-nbgallery/gallerymenu"] = j
 })();
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/gallerymenu/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8806985294117646%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/coreutils': '>=5.2.0', 'ts-md5': '^1.2.9'}",*

 * * "'description'": "'Track cell execution Metrics'",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'files'": "{insert: [(2, 'schema/**/*.json')]}",*

 * * "'jupyterlab'": "{'outputDir': '../labextension/instrumentation', '_build': {'load': "*

 * *                 "'static/remoteEntry.52d0d8f58cd3e55540ee.js'}}",*

 * * "'name'": "'@jupyterlab-nbgallery/instrumentation'",*

 * * "'version'": "'2.1. […]*

```diff
@@ -1,54 +1,55 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
+        "@jupyterlab/coreutils": ">=5.2.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0"
+        "jquery": "^3.5.0",
+        "ts-md5": "^1.2.9"
     },
-    "description": "Inject the notebook UUID into the kernel.",
+    "description": "Track cell execution Metrics",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6def7b207d91856938f3.js"
+            "load": "static/remoteEntry.52d0d8f58cd3e55540ee.js"
         },
         "extension": true,
-        "outputDir": "../labextension/inject-uuid",
+        "outputDir": "../labextension/instrumentation",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/inject-uuid",
+    "name": "@jupyterlab-nbgallery/instrumentation",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -67,9 +68,9 @@
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.1.0"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/schemas/@jupyterlab-nbgallery/inject-uuid/package.json.orig`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9564479638009051%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/notebook': '>=3.6.0'}",*

 * * "'devDependencies'": "{'prettier': '>=1.13.0', delete: ['@typescript-eslint/eslint-plugin', "*

 * *                      "'@typescript-eslint/parser']}",*

 * * "'version'": "'2.0.1'"}*

```diff
@@ -1,29 +1,29 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
+        "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
         "jquery": "^3.5.0"
     },
     "description": "Inject the notebook UUID into the kernel.",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
+        "prettier": ">=1.13.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
@@ -63,9 +63,9 @@
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/inject-uuid/static/remoteEntry.6def7b207d91856938f3.js` & `jupyterlab_nbgallery-2.0.2/labextension/inject-uuid/static/remoteEntry.f32354aac49e7b8ba738.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, d, f, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v = {
             711: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -40,44 +40,44 @@
             a: r
         }), r
     }, g.d = (e, r) => {
         for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".0616ffe42e5ee3230288.js?v=0616ffe42e5ee3230288", g.g = function() {
+    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".bde16f9395a112a349ee.js?v=bde16f9395a112a349ee", g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/inject-uuid:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -98,15 +98,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => g.e(568).then((() => () => g(568))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab-nbgallery/inject-uuid", "2.0.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@jupyterlab-nbgallery/inject-uuid", "2.0.1"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         g.g.importScripts && (e = g.g.location + "");
         var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -155,33 +155,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != o) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -192,22 +192,22 @@
         if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
-    }, d = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var a = g.I(r);
         return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
-        598: () => f("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "beta", 0])
+        123: () => d("default", "@jupyterlab/notebook", [1, 3, 6, 3])
     }, h = {
-        568: [598]
+        568: [123]
     }, g.f.consumes = (e, r) => {
         g.o(h, e) && h[e].forEach((e => {
             if (g.o(p, e)) return r.push(p[e]);
             var t = r => {
                     p[e] = 0, g.m[e] = t => {
                         delete g.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/schemas/@jupyterlab-nbgallery/environment-life/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8217592592592592%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/coreutils': '>=5.6.0', '@jupyterlab/services': '>=6.6.0', "*

 * *                   "'@jupyterlab/statusbar': '>=3.6.0', delete: ['ts-md5']}",*

 * * "'description'": "'Allow an expiration data to be displayed in the bottom right corner when "*

 * *                  "operating in an environment where jupyter instances have a defined lifetime.'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '>=3.6.0', delete: "*

 * *                      "['@typescript-eslint/eslint-plugin', '@typescript-eslin […]*

```diff
@@ -1,57 +1,51 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
-        "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/coreutils": ">=5.6.0",
+        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0",
-        "ts-md5": "^1.2.9"
+        "@jupyterlab/statusbar": ">=3.6.0",
+        "jquery": "^3.5.0"
     },
-    "description": "Track cell execution Metrics",
+    "description": "Allow an expiration data to be displayed in the bottom right corner when operating in an environment where jupyter instances have a defined lifetime.",
     "devDependencies": {
-        "@jupyterlab/builder": ">=3.3.2",
+        "@jupyterlab/builder": ">=3.6.0",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/**/*.json"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.ae4d1ce402e6ac0dddb5.js"
-        },
         "extension": true,
-        "outputDir": "../labextension/instrumentation",
+        "outputDir": "../labextension/environment-life",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/instrumentation",
+    "name": "@jupyterlab-nbgallery/environment-life",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -69,10 +63,11 @@
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
+    "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "0.2.4"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/schemas/@jupyterlab-nbgallery/instrumentation/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/gallerymenu/package.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8189775910364145%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/mainmenu': '>=3.6.0', '@jupyterlab/notebook': '>=3.6.0', delete: "*

 * *                   "['@jupyterlab/coreutils', 'ts-md5']}",*

 * * "'description'": "'All the menu capabilities needed for saving/forking notebooks and submitting "*

 * *                  "change request to Notebook Gallery'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '>=3.6.0', delete: "*

 * *                      "['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}",*

 * * "'jupyterlab'": "{'outputDir': '../ […]*

```diff
@@ -1,25 +1,23 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
-        "@jupyterlab/coreutils": ">=5.2.0",
+        "@jupyterlab/mainmenu": ">=3.6.0",
+        "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "jquery": "^3.5.0",
-        "ts-md5": "^1.2.9"
+        "jquery": "^3.5.0"
     },
-    "description": "Track cell execution Metrics",
+    "description": "All the menu capabilities needed for saving/forking notebooks and submitting change request to Notebook Gallery",
     "devDependencies": {
-        "@jupyterlab/builder": ">=3.3.2",
+        "@jupyterlab/builder": ">=3.6.0",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
@@ -28,26 +26,30 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/**/*.json"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.fadc9f3eb62fb570716e.js"
+        },
         "extension": true,
-        "outputDir": "../labextension/instrumentation",
+        "outputDir": "../labextension/gallerymenu",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/instrumentation",
+    "name": "@jupyterlab-nbgallery/gallerymenu",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -62,13 +64,10 @@
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "eslint": "eslint . --ext .ts,.tsx --fix",
         "eslint:check": "eslint . --ext .ts,.tsx",
         "install-ext": "jlpm run build",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "sideEffects": [
-        "style/*.css"
-    ],
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.2"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/568.7f1ab65a55b54297cd7b.js` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/568.274dc29b6aea1cf48d74.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,79 +1,81 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_instrumentation = self.webpackChunk_jupyterlab_nbgallery_instrumentation || []).push([
     [568], {
         568: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => u
+                default: () => d
             });
-            var l = n(225),
-                o = n(281),
-                i = n(598),
-                a = n(941),
-                s = n(24),
-                c = n(569),
-                r = n.n(c);
-            const u = {
+            var l = n(38),
+                o = n(142),
+                i = n(123),
+                a = n(191),
+                r = n(24),
+                s = n(569),
+                c = n.n(s);
+            let u = null;
+            const d = {
                 id: "@juptyerlab-nbgallery/instrumentation",
                 autoStart: !0,
                 requires: [l.ISettingRegistry],
                 activate: async (e, t) => {
                     let n = {},
                         l = !1;
                     i.NotebookActions.executionScheduled.connect(((e, t) => {
                         if (l) {
                             let e, l;
                             l = t.notebook, e = t.cell;
                             const o = new Date;
                             n[e.id] = new Object, n[e.id].startTime = o.getTime(), n[e.id].cellIndex = l.activeCellIndex, console.log(e)
                         }
-                    })), i.NotebookActions.executed.connect(((e, t) => {
+                    })), i.NotebookActions.executed.connect(((o, i) => {
                         const {
-                            cell: o,
-                            notebook: i,
-                            success: c
-                        } = t;
-                        if (l && o instanceof a.CodeCell) {
-                            const e = new Date;
-                            console.log("Post execution"),
-                                function(e, t, n, l) {
-                                    let o;
-                                    if (o = e.model.sharedModel.metadata.gallery, o) {
-                                        let i = new Object;
-                                        i.success = n, i.md5 = s.Md5.hashStr(t.model.sharedModel.source), i.runtime = l, i.uuid = o.uuid || o.link || o.clone;
-                                        let a = o.gallery_url;
-                                        console.log(a), a.length > 0 && i.uuid.length > 0 && r().ajax({
+                            cell: s,
+                            notebook: d,
+                            success: g
+                        } = i;
+                        if (l && s instanceof a.CodeCell) {
+                            const l = new Date;
+                            console.log("Post execution"), Promise.all([e.restored, t.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
+                                ! function(e, t, n, l, o) {
+                                    let i;
+                                    if (i = e.model.sharedModel.metadata.gallery, i) {
+                                        let a = new Object;
+                                        a.success = n, a.md5 = r.Md5.hashStr(t.model.sharedModel.source), a.runtime = l, a.uuid = i.uuid || i.link || i.clone;
+                                        let s = i.gallery_url;
+                                        s || (s = o.get("nbgallery_url").composite), s || (s = u), console.log(s), s.length > 0 && a.uuid.length > 0 && c().ajax({
                                             method: "POST",
                                             headers: {
                                                 Accept: "application/json"
                                             },
-                                            url: a + "/executions",
-                                            data: i,
+                                            url: s + "/executions",
+                                            data: a,
                                             xhrFields: {
                                                 withCredentials: !0
                                             }
-                                        }), console.log("Made it here" + e + t + n + l), console.log(o.uuid)
+                                        }), console.log("Made it here" + e + t + n + l), console.log(i.uuid)
                                     }
-                                }(i, o, c, e.getTime() - n[o.id].startTime)
+                                }(d, s, g, l.getTime() - n[s.id].startTime, e)
+                            }))
                         }
                     })), Promise.all([e.restored, t.load("@jupyterlab-nbgallery/instrumentation:instrumentation")]).then((([, e]) => {
                         try {
                             ! function(e) {
-                                r().ajax({
+                                c().ajax({
                                     method: "GET",
                                     headers: {
                                         Accept: "application/json"
                                     },
                                     url: o.PageConfig.getBaseUrl() + "jupyterlab_nbgallery/instrumentation",
                                     cache: !1,
                                     xhrFields: {
                                         withCredentials: !0
                                     },
                                     success: function(t) {
-                                        1 == t.NBGALLERY_ENABLE_INSTRUMENTATION || e.get("enabled").composite ? (e.set("enabled", !0), l = !0) : l = !1
+                                        u = t.NBGALLERY_URL, 1 == t.NBGALLERY_ENABLE_INSTRUMENTATION || e.get("enabled").composite ? (e.set("enabled", !0), l = !0) : l = !1
                                     }
                                 })
                             }(e)
                         } catch (e) {
                             console.error(`Problem initializing instrumentation \n ${e}`)
                         }
                     }))
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/638.b95125ed695cee42aae4.js` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/638.b95125ed695cee42aae4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/701.d81800f5926ab62cc8b2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/remoteEntry.ae4d1ce402e6ac0dddb5.js` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/remoteEntry.52d0d8f58cd3e55540ee.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, d, f, c, p, h, v, b, y, g, m, w, j, S = {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, b, v, y, g, m, w, j, S = {
             250: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         k = {};
 
     function E(e) {
         var r = k[e];
@@ -41,81 +41,81 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        568: "7f1ab65a55b54297cd7b",
+        568: "274dc29b6aea1cf48d74",
         638: "b95125ed695cee42aae4",
         701: "d81800f5926ab62cc8b2"
     } [e] + ".js?v=" + {
-        568: "7f1ab65a55b54297cd7b",
+        568: "274dc29b6aea1cf48d74",
         638: "b95125ed695cee42aae4",
         701: "d81800f5926ab62cc8b2"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/instrumentation:", E.l = (t, n, a, o) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab-nbgallery/instrumentation:", E.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
+            if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         E.S = {};
         var e = {},
             r = {};
         E.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var o = E.S[t],
+                var a = E.S[t],
                     i = "@jupyterlab-nbgallery/instrumentation",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@jupyterlab-nbgallery/instrumentation", "2.0.0", (() => E.e(568).then((() => () => E(568))))), u("jquery", "3.6.4", (() => E.e(638).then((() => () => E(638))))), u("ts-md5", "1.3.1", (() => E.e(701).then((() => () => E(701)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupyterlab-nbgallery/instrumentation", "2.1.0", (() => E.e(568).then((() => () => E(568))))), u("jquery", "3.6.4", (() => E.e(638).then((() => () => E(638))))), u("ts-md5", "1.3.1", (() => E.e(701).then((() => () => E(701)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -129,163 +129,163 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
+                            if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || u <= n) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != a) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(s(e, t, a, n)), h(e[t][a])
-    }, f = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+    }, s = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        var o = l(e, t);
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(s(e, t, o, n)), h(e[t][o])
+    }, d = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
     }, c = (e, r, t, n) => {
-        var o = e[t];
-        return "No satisfying version (" + a(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
+        var a = e[t];
+        return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
     }, p = (e, r, t, n) => {
         "undefined" != typeof console && console.warn && console.warn(c(e, r, t, n))
-    }, h = e => (e.loaded = 1, e.get()), b = (v = e => function(r, t, n, a) {
-        var o = E.I(r);
-        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), h(f(r, t, n) || p(r, e, t, n) || u(r, t))))), y = v(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), g = v(((e, r, t, n, a) => {
-        var o = r && E.o(r, t) && f(r, t, n);
-        return o ? h(o) : a()
+    }, h = e => (e.loaded = 1, e.get()), v = (b = e => function(r, t, n, o) {
+        var a = E.I(r);
+        return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), h(d(r, t, n) || p(r, e, t, n) || u(r, t))))), y = b(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), g = b(((e, r, t, n, o) => {
+        var a = r && E.o(r, t) && d(r, t, n);
+        return a ? h(a) : o()
     })), m = {}, w = {
         24: () => g("default", "ts-md5", [1, 1, 2, 9], (() => E.e(701).then((() => () => E(701))))),
-        225: () => y("default", "@jupyterlab/settingregistry", [1, 4, 0, 0, , "beta", 0]),
-        281: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
-        569: () => g("default", "jquery", [1, 3, 5, 0], (() => E.e(638).then((() => () => E(638))))),
-        598: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "beta", 0]),
-        941: () => b("default", "@jupyterlab/cells", [1, 4, 0, 0, , "beta", 0])
+        38: () => y("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        123: () => y("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
+        142: () => y("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        191: () => v("default", "@jupyterlab/cells", [1, 3, 6, 3]),
+        569: () => g("default", "jquery", [1, 3, 5, 0], (() => E.e(638).then((() => () => E(638)))))
     }, j = {
-        568: [24, 225, 281, 569, 598, 941]
+        568: [24, 38, 123, 142, 191, 569]
     }, E.f.consumes = (e, r) => {
         E.o(j, e) && j[e].forEach((e => {
             if (E.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete m[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
             try {
-                var a = w[e]();
-                a.then ? r.push(m[e] = a.then(t).catch(n)) : t(a)
+                var o = w[e]();
+                o.then ? r.push(m[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             723: 0
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = E.p + E.u(r),
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = E.p + E.u(r),
                         i = new Error;
-                    E.l(o, (t => {
+                    E.l(a, (t => {
                         if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     u && u(E)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyterlab_nbgallery_instrumentation = self.webpackChunk_jupyterlab_nbgallery_instrumentation || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var _ = E(250);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab-nbgallery/instrumentation"] = _
 })();
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/instrumentation/static/third-party-licenses.json` & `jupyterlab_nbgallery-2.0.2/labextension/instrumentation/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/package.json` & `jupyterlab_nbgallery-2.0.2/labextension/environment-life/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8790509259259259%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/coreutils': '>=5.6.0', '@jupyterlab/services': '>=6.6.0', "*

 * *                   "'@jupyterlab/statusbar': '>=3.6.0', delete: ['@jupyterlab/mainmenu', "*

 * *                   "'@jupyterlab/notebook', 'fa-icons']}",*

 * * "'description'": "'Allow an expiration data to be displayed in the bottom right corner when "*

 * *                  "operating in an environment where jupyter instances have a defined lifetime.'",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '>=3.6.0', delete: "*

 * *       […]*

```diff
@@ -1,59 +1,56 @@
 {
     "author": "Team@NBG",
     "bugs": {
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
-        "@jupyterlab/mainmenu": ">=3.6.0 ||",
-        "@jupyterlab/notebook": ">=3.6.0",
+        "@jupyterlab/coreutils": ">=5.6.0",
+        "@jupyterlab/services": ">=6.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "fa-icons": "^0.2.0",
+        "@jupyterlab/statusbar": ">=3.6.0",
         "jquery": "^3.5.0"
     },
-    "description": "All the menu capabilities needed for saving/forking notebooks and submitting change request to Notebook Gallery",
+    "description": "Allow an expiration data to be displayed in the bottom right corner when operating in an environment where jupyter instances have a defined lifetime.",
     "devDependencies": {
-        "@jupyterlab/builder": ">=3.3.2",
+        "@jupyterlab/builder": ">=3.6.0",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/**/*.json"
+        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/nbgallery/lab-extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3f8d9d3f425bc3ff0a80.js",
+            "load": "static/remoteEntry.fe9e40141faed985c15b.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "../labextension/userpreferences",
+        "outputDir": "../labextension/environment-life",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "MIT",
     "main": "lib/index.js",
-    "name": "@jupyterlab-nbgallery/userpreferences",
+    "name": "@jupyterlab-nbgallery/environment-life",
     "repository": {
         "type": "git",
         "url": "https://github.com/nbgallery/lab-extensions"
     },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:all": "jlpm run build:prod",
@@ -73,9 +70,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "1.0.2"
+    "version": "0.2.4"
 }
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/schemas/@jupyterlab-nbgallery/userpreferences/package.json.orig`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407407%*

 * *Differences: {"'dependencies'": "{delete: ['fa-icons']}",*

 * * "'devDependencies'": "{delete: ['@typescript-eslint/eslint-plugin', '@typescript-eslint/parser']}"}*

```diff
@@ -4,23 +4,20 @@
         "url": "https://github.com/nbgallery/lab-extensions/issues"
     },
     "dependencies": {
         "@jupyterlab/application": ">=3.6.0",
         "@jupyterlab/mainmenu": ">=3.6.0 ||",
         "@jupyterlab/notebook": ">=3.6.0",
         "@jupyterlab/settingregistry": ">=3.6.0",
-        "fa-icons": "^0.2.0",
         "jquery": "^3.5.0"
     },
     "description": "All the menu capabilities needed for saving/forking notebooks and submitting change request to Notebook Gallery",
     "devDependencies": {
         "@jupyterlab/builder": ">=3.3.2",
         "@types/jquery": "^3.5.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^8.0.0",
         "eslint-config-prettier": "^6.15.0",
         "eslint-plugin-jsdoc": "^39.0.0",
         "eslint-plugin-prettier": "^3.1.4",
         "eslint-plugin-react": "^7.18.3",
         "npm-run-all": "^4.1.5",
         "rimraf": "^3.0.2",
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/568.0ac7cbac0996e718a0d9.js` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/568.eab1414ad9e7f57f8e93.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,50 +1,58 @@
 "use strict";
 (self.webpackChunk_jupyterlab_nbgallery_userpreferences = self.webpackChunk_jupyterlab_nbgallery_userpreferences || []).push([
     [568], {
         568: (e, r, t) => {
             t.r(r), t.d(r, {
-                default: () => p
+                default: () => h
             });
-            var a = t(551),
-                s = t(678),
-                n = t(144),
-                l = t(530),
-                o = t(281),
-                i = t(569),
-                c = t.n(i);
-            const u = {
+            var a = t(344),
+                s = t(33),
+                n = t(832),
+                l = t(820),
+                i = t(38),
+                o = t(142),
+                c = t(569),
+                u = t.n(c);
+            const d = {
                 id: "@jupyterlab-nbgallery/userpreferences",
                 autoStart: !0,
-                requires: [a.IMainMenu],
-                activate: function(e, r) {
-                    new d(e, r).startup()
+                requires: [a.IMainMenu, i.ISettingRegistry],
+                activate: function(e, r, t) {
+                    new p(e, r, t)
                 }
             };
-            class d {
-                constructor(e, r) {
-                    this.app = e, this.mainMenu = r, this.settings = l.ServerConnection.makeSettings()
+            class p {
+                constructor(e, r, t) {
+                    this.app = e, this.mainMenu = r, this.server_settings = l.ServerConnection.makeSettings(), this.settingRegistry = t, Promise.all([this.app.restored, this.settingRegistry.load("@jupyterlab-nbgallery/environment-registration:environment-registration")]).then((([, e]) => {
+                        this.settings = e, this.startup()
+                    }))
                 }
                 async startup() {
-                    const e = o.URLExt.join(this.settings.baseUrl, "jupyterlab_nbgallery", "environment");
-                    let r = this;
-                    await c().ajax({
-                        method: "GET",
-                        headers: {
-                            Accept: "application/json"
-                        },
-                        url: e,
-                        cache: !1,
-                        xhrFields: {
-                            withCredentials: !0
-                        },
-                        success: function(e) {
-                            r.gallery_url = new URL(e.NBGALLERY_URL)
-                        }
-                    }), this.gallery_preferences_url = o.URLExt.join(this.gallery_url.origin, "preferences"), this.jupyter_preferences_url = o.URLExt.join(this.settings.baseUrl, "jupyterlab_nbgallery", "preferences"), this.gallery_menu = this.buildMenus(), this.mainMenu.addMenu(this.gallery_menu, {
+                    try {
+                        this.gallery_url = new URL(this.settings.get("nbgallery_url").composite)
+                    } catch (e) {
+                        const r = o.URLExt.join(this.server_settings.baseUrl, "jupyterlab_nbgallery", "environment");
+                        let t = this;
+                        await u().ajax({
+                            method: "GET",
+                            headers: {
+                                Accept: "application/json"
+                            },
+                            url: r,
+                            cache: !1,
+                            xhrFields: {
+                                withCredentials: !0
+                            },
+                            success: function(e) {
+                                t.gallery_url = new URL(e.NBGALLERY_URL)
+                            }
+                        })
+                    }
+                    this.gallery_preferences_url = o.URLExt.join(this.gallery_url.origin, "preferences"), this.jupyter_preferences_url = o.URLExt.join(this.server_settings.baseUrl, "jupyterlab_nbgallery", "preferences"), this.gallery_menu = this.buildMenus(), this.mainMenu.addMenu(this.gallery_menu, {
                         rank: 50
                     })
                 }
                 buildMenus() {
                     console.log("Building Menus");
                     const {
                         commands: e
@@ -88,26 +96,26 @@
                         type: "separator"
                     }), r.addItem({
                         type: "submenu",
                         submenu: t
                     }), r
                 }
                 async uploadPreferences() {
-                    let e = await c().ajax({
+                    let e = await u().ajax({
                         method: "GET",
                         url: this.jupyter_preferences_url,
                         cache: !1,
                         headers: {
                             Accept: "application/json"
                         },
                         xhrFields: {
                             withCredentials: !0
                         }
                     });
-                    await c().ajax({
+                    await u().ajax({
                         method: "POST",
                         url: this.gallery_preferences_url,
                         data: {
                             lab_preferences: JSON.stringify(e)
                         },
                         headers: {
                             Accept: "application/json"
@@ -117,26 +125,26 @@
                         },
                         error: function() {
                             (0, s.showErrorMessage)("Error Uploading Preferences", "An error occured saving your preferences to NBGallery.  Please try again later or contact the site adminsitrators.")
                         }
                     })
                 }
                 async downloadPreferences() {
-                    let e = await c().ajax({
+                    let e = await u().ajax({
                         method: "GET",
                         url: this.gallery_preferences_url,
                         cache: !1,
                         headers: {
                             Accept: "application/json"
                         },
                         xhrFields: {
                             withCredentials: !0
                         }
                     });
-                    c().ajax({
+                    u().ajax({
                         method: "POST",
                         url: this.jupyter_preferences_url,
                         data: e.lab_preferences,
                         xhrFields: {
                             withCredentials: !0
                         },
                         cache: !1,
@@ -152,15 +160,15 @@
                 async resetPreferences() {
                     let e = this;
                     (0, s.showDialog)({
                         title: "Reset User Preferences?",
                         body: "This will delete ALL local preferences you have customized in your image restoring JupyterLab to the defaults.  Your preferences saved to the gallery will not be impacted.  Proceed?",
                         buttons: [s.Dialog.cancelButton(), s.Dialog.warnButton()]
                     }).then((r => {
-                        r.button.accept && c().ajax({
+                        r.button.accept && u().ajax({
                             method: "DELETE",
                             url: e.jupyter_preferences_url,
                             xhrFields: {
                                 withCredentials: !0
                             },
                             cache: !1,
                             complete: function(e, r) {
@@ -170,11 +178,11 @@
                                     buttons: [s.Dialog.okButton()]
                                 }) : (0, s.showErrorMessage)("Error Resetting Preferences", "An error occured while attempting to reset your preferences in Jupyter.  Please try again later.")
                             }
                         })
                     }))
                 }
             }
-            const p = u
+            const h = d
         }
     }
 ]);
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/638.e5080f99954048969f76.js` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/638.e5080f99954048969f76.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbgallery-2.0.0a4/labextension/userpreferences/static/remoteEntry.3f8d9d3f425bc3ff0a80.js` & `jupyterlab_nbgallery-2.0.2/labextension/userpreferences/static/remoteEntry.0c562dfea5f20371ffe8.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, f, d, p, c, h, b, v, g, y = {
+    var e, r, t, n, a, o, i, u, l, s, f, p, c, d, h, v, b, g, y = {
             130: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568))),
                         "./style": () => t.e(542).then((() => () => t(542)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,19 +44,19 @@
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         542: "d1718a50e23f3808ba62",
-        568: "0ac7cbac0996e718a0d9",
+        568: "eab1414ad9e7f57f8e93",
         638: "e5080f99954048969f76"
     } [e] + ".js?v=" + {
         542: "d1718a50e23f3808ba62",
-        568: "0ac7cbac0996e718a0d9",
+        568: "eab1414ad9e7f57f8e93",
         638: "e5080f99954048969f76"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -70,24 +70,24 @@
                     var f = l[s];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
                         i = f;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var p = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(p.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -166,86 +166,87 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
+                var s, f, p = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == p ? u > n && !a : "" == p != a);
                 if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                    if (!l || "u" != p) return !1
                 } else if (l)
-                    if (d == f)
+                    if (p == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
                             if (a ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != p && "n" != p) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != a) return !1;
+                    if (u <= n || f < p != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            d = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? o(h, r) : !d())
         }
-        return !!c()
+        return !!d()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), d(e[t][a])
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), p(e[t][a])
     }, f = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
+    }, p = e => (e.loaded = 1, e.get()), d = (c = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
         var o = r && w.o(r, t) && f(r, t, n);
-        return o ? d(o) : a()
-    })), b = {}, v = {
-        144: () => c("default", "@lumino/widgets", [1, 2, 0, 0]),
-        281: () => c("default", "@jupyterlab/coreutils", [1, 6, 0, 0, , "beta", 0]),
-        530: () => c("default", "@jupyterlab/services", [1, 7, 0, 0, , "beta", 0]),
-        551: () => c("default", "@jupyterlab/mainmenu", [1, 4, 0, 0, , "beta", 0]),
+        return o ? p(o) : a()
+    })), v = {}, b = {
+        33: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
+        38: () => d("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
+        142: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        344: () => d("default", "@jupyterlab/mainmenu", [1, 3, 6, 3]),
         569: () => h("default", "jquery", [1, 3, 5, 0], (() => w.e(638).then((() => () => w(638))))),
-        678: () => c("default", "@jupyterlab/apputils", [1, 4, 0, 0, , "beta", 0])
+        820: () => d("default", "@jupyterlab/services", [1, 6, 6, 3]),
+        832: () => d("default", "@lumino/widgets", [1, 1, 37, 2])
     }, g = {
-        568: [144, 281, 530, 551, 569, 678]
+        568: [33, 38, 142, 344, 569, 820, 832]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
-            if (w.o(b, e)) return r.push(b[e]);
+            if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, w.m[e] = t => {
+                    v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], w.m[e] = t => {
+                    delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var a = b[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             480: 0
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/package.json` & `jupyterlab_nbgallery-2.0.2/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9763888888888889%*

 * *Differences: {"'devDependencies'": "{'embedme': '^1.22.1', 'husky': '^8.0.0'}",*

 * * "'scripts'": "{'prepare': 'husky install'}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "devDependencies": {
-        "embedme": "^1.17.1",
-        "husky": "^3.0.9",
+        "embedme": "^1.22.1",
+        "husky": "^8.0.0",
         "lerna": "^3.18.4",
         "lint-staged": "^9.4.3",
         "prettier": "^1.19.1"
     },
     "husky": {
         "hooks": {
             "pre-commit": "lint-staged"
@@ -19,14 +19,15 @@
         "build-jlab": "jupyter lab build --debug",
         "clean-ext": "lerna run clean",
         "embedme": "embedme \"[!n]*/**/README.md\"",
         "install": "lerna bootstrap",
         "install-ext": "lerna run install-ext",
         "lint": "jlpm && jlpm run prettier",
         "lint:check": "jlpm run embedme --verify && jlpm run prettier:check",
+        "prepare": "husky install",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\""
     },
     "workspaces": {
         "packages": [
             "environment-registration",
             "environment-life",
```

### Comparing `jupyterlab_nbgallery-2.0.0a4/setup.py` & `jupyterlab_nbgallery-2.0.2/setup.py`

 * *Files identical despite different names*

