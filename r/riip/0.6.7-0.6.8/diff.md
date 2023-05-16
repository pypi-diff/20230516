# Comparing `tmp/riip-0.6.7.tar.gz` & `tmp/riip-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riip-0.6.7.tar", last modified: Mon Feb 28 09:34:52 2022, max compression
+gzip compressed data, was "riip-0.6.8.tar", last modified: Mon Feb 28 13:09:50 2022, max compression
```

## Comparing `riip-0.6.7.tar` & `riip-0.6.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.634441 riip-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-02-28 09:34:32.000000 riip-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-28 09:34:32.000000 riip-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-02-28 09:34:52.634441 riip-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-02-28 09:34:32.000000 riip-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-28 09:34:32.000000 riip-0.6.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-02-28 09:34:32.000000 riip-0.6.7/docs/conda_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-02-28 09:34:32.000000 riip-0.6.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-02-28 09:34:32.000000 riip-0.6.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-02-28 09:34:32.000000 riip-0.6.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-28 09:34:32.000000 riip-0.6.7/docs/markdown.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-02-28 09:34:32.000000 riip-0.6.7/docs/notebooks/00_Installation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   130028 2022-02-28 09:34:32.000000 riip-0.6.7/docs/notebooks/01_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   115094 2022-02-28 09:34:32.000000 riip-0.6.7/docs/notebooks/02_RiiDataFrame.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   108872 2022-02-28 09:34:32.000000 riip-0.6.7/docs/notebooks/03_Material.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   566399 2022-02-28 09:34:32.000000 riip-0.6.7/docs/notebooks/04_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-28 09:34:32.000000 riip-0.6.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-02-28 09:34:32.000000 riip-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-02-28 09:34:32.000000 riip-0.6.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-02-28 09:34:52.634441 riip-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-02-28 09:34:32.000000 riip-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/src/riip/data/my_database/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/src/riip/data/my_database/data/BB/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Ag/
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Ag/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Al/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Al/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Au/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Au/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Be/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Be/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Cr/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Cr/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Cu/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Cu/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Ni/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Ni/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Pd/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Pd/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Pt/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Pt/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/Ti/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/Ti/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/BB/W/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/BB/W/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.626441 riip-0.6.7/src/riip/data/my_database/data/DL/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Ag/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Ag/Lee.yml
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Ag/Rakic.yml
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Ag/Vial.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Al/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Al/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Au/
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Au/Rakic.yml
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Au/Stewart.yml
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Au/Vial_d.yml
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Au/Vial_dl.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Be/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Be/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Cr/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Cr/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Cu/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Cu/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Ni/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Ni/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Pd/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Pd/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Pt/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Pt/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/Ti/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/Ti/Rakic.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip/data/my_database/data/DL/W/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/data/DL/W/Rakic.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/my_database/library.yml
--rw-r--r--   0 runner    (1001) docker     (121)      827 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/data/riid.patch
--rw-r--r--   0 runner    (1001) docker     (121)    25361 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/formulas.py
--rw-r--r--   0 runner    (1001) docker     (121)    16436 2022-02-28 09:34:32.000000 riip-0.6.7/src/riip/material.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/riip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-28 09:34:52.000000 riip-0.6.7/src/riip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:52.630441 riip-0.6.7/src/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 09:34:32.000000 riip-0.6.7/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-02-28 09:34:32.000000 riip-0.6.7/src/utils/formulas_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-02-28 13:09:29.000000 riip-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-28 13:09:29.000000 riip-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-02-28 13:09:50.690676 riip-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3577 2022-02-28 13:09:29.000000 riip-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.682676 riip-0.6.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-28 13:09:29.000000 riip-0.6.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-02-28 13:09:29.000000 riip-0.6.8/docs/conda_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-02-28 13:09:29.000000 riip-0.6.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-02-28 13:09:29.000000 riip-0.6.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-02-28 13:09:29.000000 riip-0.6.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-28 13:09:29.000000 riip-0.6.8/docs/markdown.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.682676 riip-0.6.8/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-02-28 13:09:29.000000 riip-0.6.8/docs/notebooks/00_Installation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   130028 2022-02-28 13:09:29.000000 riip-0.6.8/docs/notebooks/01_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   115094 2022-02-28 13:09:29.000000 riip-0.6.8/docs/notebooks/02_RiiDataFrame.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   108872 2022-02-28 13:09:29.000000 riip-0.6.8/docs/notebooks/03_Material.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   566399 2022-02-28 13:09:29.000000 riip-0.6.8/docs/notebooks/04_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-28 13:09:29.000000 riip-0.6.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-02-28 13:09:29.000000 riip-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-02-28 13:09:29.000000 riip-0.6.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-02-28 13:09:50.690676 riip-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-02-28 13:09:29.000000 riip-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.682676 riip-0.6.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.678676 riip-0.6.8/src/riip/data/my_database/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.678676 riip-0.6.8/src/riip/data/my_database/data/BB/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Ag/
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Ag/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Al/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Al/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Au/
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Au/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Be/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Be/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Cr/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Cr/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Cu/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Cu/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Ni/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Ni/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Pd/
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Pd/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Pt/
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Pt/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/Ti/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/Ti/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip/data/my_database/data/BB/W/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/BB/W/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.682676 riip-0.6.8/src/riip/data/my_database/data/DL/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Ag/
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Ag/Lee.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Ag/Rakic.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Ag/Vial.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Al/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Al/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Au/
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Au/Rakic.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      573 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Au/Stewart.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Au/Vial_d.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      535 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Au/Vial_dl.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Be/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Be/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Cr/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Cr/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Cu/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Cu/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Ni/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Ni/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Pd/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Pd/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Pt/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Pt/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/Ti/
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/Ti/Rakic.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/riip/data/my_database/data/DL/W/
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/data/DL/W/Rakic.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/my_database/library.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      827 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/data/riid.patch
+-rw-r--r--   0 runner    (1001) docker     (121)    25361 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4993 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/formulas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16436 2022-02-28 13:09:29.000000 riip-0.6.8/src/riip/material.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.686676 riip-0.6.8/src/riip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-28 13:09:50.000000 riip-0.6.8/src/riip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:50.690676 riip-0.6.8/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-28 13:09:29.000000 riip-0.6.8/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-02-28 13:09:29.000000 riip-0.6.8/src/utils/formulas_cython.pyx
```

### Comparing `riip-0.6.7/LICENSE` & `riip-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/PKG-INFO` & `riip-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riip
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python 3 + Pandas wrapper for the refractiveindex.info database
 Home-page: https://github.com/mnishida/RII_Pandas
 Author: Munehiro Nishida
 Author-email: mnishida@hiroshima-u.ac.jp
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -108,10 +108,10 @@
 - numpy
 - scipy
 - pandas
 - pyyaml
 - gitpython
 
 ## Version
-0.6.7
+0.6.8
```

### Comparing `riip-0.6.7/README.md` & `riip-0.6.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,8 @@
 - numpy
 - scipy
 - pandas
 - pyyaml
 - gitpython
 
 ## Version
-0.6.7
+0.6.8
```

### Comparing `riip-0.6.7/docs/Makefile` & `riip-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/conf.py` & `riip-0.6.8/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from recommonmark.transform import AutoStructify
 
 project = "RII_Pandas"
-version = "0.6.7"
+version = "0.6.8"
 copyright = "2021, Munehiro Nishida"
 author = "Munehiro Nishida"
 
 master_doc = "index"
 html_theme = "sphinx_rtd_theme"
 
 source_suffix = {
```

### Comparing `riip-0.6.7/docs/index.rst` & `riip-0.6.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/make.bat` & `riip-0.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/notebooks/00_Installation.ipynb` & `riip-0.6.8/docs/notebooks/00_Installation.ipynb`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/notebooks/01_tutorial.ipynb` & `riip-0.6.8/docs/notebooks/01_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/notebooks/02_RiiDataFrame.ipynb` & `riip-0.6.8/docs/notebooks/02_RiiDataFrame.ipynb`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/notebooks/03_Material.ipynb` & `riip-0.6.8/docs/notebooks/03_Material.ipynb`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/docs/notebooks/04_examples.ipynb` & `riip-0.6.8/docs/notebooks/04_examples.ipynb`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/setup.py` & `riip-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     language="c++",
 )
 e.cython_directives = {"language_level": "3"}
 ext_modules.append(e)
 
 setup(
     name="riip",
-    version="0.6.7",
+    version="0.6.8",
     url="https://github.com/mnishida/RII_Pandas",
     license="MIT",
     author="Munehiro Nishida",
     author_email="mnishida@hiroshima-u.ac.jp",
     description="Python 3 + Pandas wrapper for the refractiveindex.info database",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Ag/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Ag/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Al/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Al/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Au/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Au/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Be/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Be/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Cr/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Cr/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Cu/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Cu/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Ni/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Ni/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Pd/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Pd/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Pt/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Pt/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/Ti/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/Ti/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/BB/W/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/BB/W/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Ag/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Ag/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Ag/Vial.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Ag/Vial.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Al/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Al/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Au/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Au/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Au/Stewart.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Au/Stewart.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Au/Vial_dl.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Au/Vial_dl.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Be/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Be/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Cr/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Cr/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Cu/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Cu/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Ni/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Ni/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Pd/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Pd/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Pt/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Pt/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/Ti/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/Ti/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/data/DL/W/Rakic.yml` & `riip-0.6.8/src/riip/data/my_database/data/DL/W/Rakic.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/my_database/library.yml` & `riip-0.6.8/src/riip/data/my_database/library.yml`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/data/riid.patch` & `riip-0.6.8/src/riip/data/riid.patch`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/dataframe.py` & `riip-0.6.8/src/riip/dataframe.py`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/formulas.py` & `riip-0.6.8/src/riip/formulas.py`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip/material.py` & `riip-0.6.8/src/riip/material.py`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/riip.egg-info/PKG-INFO` & `riip-0.6.8/src/riip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riip
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python 3 + Pandas wrapper for the refractiveindex.info database
 Home-page: https://github.com/mnishida/RII_Pandas
 Author: Munehiro Nishida
 Author-email: mnishida@hiroshima-u.ac.jp
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -108,10 +108,10 @@
 - numpy
 - scipy
 - pandas
 - pyyaml
 - gitpython
 
 ## Version
-0.6.7
+0.6.8
```

### Comparing `riip-0.6.7/src/riip.egg-info/SOURCES.txt` & `riip-0.6.8/src/riip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riip-0.6.7/src/utils/formulas_cython.pyx` & `riip-0.6.8/src/utils/formulas_cython.pyx`

 * *Files identical despite different names*

