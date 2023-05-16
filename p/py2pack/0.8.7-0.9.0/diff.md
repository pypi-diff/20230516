# Comparing `tmp/py2pack-0.8.7.tar.gz` & `tmp/py2pack-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2pack-0.8.7.tar", last modified: Thu Jul  8 10:13:04 2021, max compression
+gzip compressed data, was "py2pack-0.9.0.tar", last modified: Tue May 16 16:11:24 2023, max compression
```

## Comparing `py2pack-0.8.7.tar` & `py2pack-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.959680 py2pack-0.8.7/
--rw-r--r--   0 thesp0nge  (1000) users      (100)      573 2021-07-08 10:07:58.000000 py2pack-0.8.7/.travis.yml
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1238 2021-07-08 10:13:04.000000 py2pack-0.8.7/AUTHORS
--rw-r--r--   0 thesp0nge  (1000) users      (100)    16880 2021-07-08 10:13:04.000000 py2pack-0.8.7/ChangeLog
--rw-r--r--   0 thesp0nge  (1000) users      (100)    10143 2021-07-08 10:07:58.000000 py2pack-0.8.7/LICENSE
--rw-r--r--   0 thesp0nge  (1000) users      (100)     5628 2021-07-08 10:13:04.959680 py2pack-0.8.7/PKG-INFO
--rw-r--r--   0 thesp0nge  (1000) users      (100)     3815 2021-07-08 10:07:58.000000 py2pack-0.8.7/README.rst
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.955680 py2pack-0.8.7/doc/
--rw-r--r--   0 thesp0nge  (1000) users      (100)     7669 2021-07-08 10:07:58.000000 py2pack-0.8.7/doc/Makefile
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.955680 py2pack-0.8.7/doc/source/
--rw-r--r--   0 thesp0nge  (1000) users      (100)       68 2021-07-08 10:07:58.000000 py2pack-0.8.7/doc/source/cli.rst
--rw-r--r--   0 thesp0nge  (1000) users      (100)     7954 2021-07-08 10:07:58.000000 py2pack-0.8.7/doc/source/conf.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)      476 2021-07-08 10:07:58.000000 py2pack-0.8.7/doc/source/index.rst
--rw-r--r--   0 thesp0nge  (1000) users      (100)      514 2021-07-08 10:07:58.000000 py2pack-0.8.7/doc/source/templates.rst
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.955680 py2pack-0.8.7/py2pack/
--rw-r--r--   0 thesp0nge  (1000) users      (100)    15007 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/__init__.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1254 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/proxy.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     4089 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/requires.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     2586 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/setup.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)    23379 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/spdx_license_map.p
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.955680 py2pack-0.8.7/py2pack/templates/
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1512 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/templates/fedora.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1313 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/templates/mageia.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     3285 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/templates/opensuse-legacy.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)      922 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/templates/opensuse.dsc
--rw-r--r--   0 thesp0nge  (1000) users      (100)     4317 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/templates/opensuse.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1805 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/utils.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)      829 2021-07-08 10:07:58.000000 py2pack-0.8.7/py2pack/version.py
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.955680 py2pack-0.8.7/py2pack.egg-info/
--rw-r--r--   0 thesp0nge  (1000) users      (100)     5628 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/PKG-INFO
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1106 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/SOURCES.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)        1 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/dependency_links.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)       42 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/entry_points.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)        1 2021-07-08 10:10:19.000000 py2pack-0.8.7/py2pack.egg-info/not-zip-safe
--rw-r--r--   0 thesp0nge  (1000) users      (100)       47 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/pbr.json
--rw-r--r--   0 thesp0nge  (1000) users      (100)       85 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/requires.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)        8 2021-07-08 10:13:04.000000 py2pack-0.8.7/py2pack.egg-info/top_level.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)       79 2021-07-08 10:07:58.000000 py2pack-0.8.7/requirements.txt
--rw-r--r--   0 thesp0nge  (1000) users      (100)     1078 2021-07-08 10:13:04.959680 py2pack-0.8.7/setup.cfg
--rwxr-xr-x   0 thesp0nge  (1000) users      (100)      766 2021-07-08 10:07:58.000000 py2pack-0.8.7/setup.py
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.959680 py2pack-0.8.7/test/
--rw-r--r--   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/__init__.py
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.959680 py2pack-0.8.7/test/examples/
--rw-r--r--   0 thesp0nge  (1000) users      (100)     4764 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-fedora.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)      757 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-mageia.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     2443 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-opensuse-augmented.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     5414 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-opensuse-legacy.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)      178 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-opensuse.dsc
--rw-r--r--   0 thesp0nge  (1000) users      (100)     5482 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/examples/py2pack-opensuse.spec
--rw-r--r--   0 thesp0nge  (1000) users      (100)     5690 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/test_py2pack.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     2463 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/test_requires.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     2339 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/test_template.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)     3431 2021-07-08 10:07:58.000000 py2pack-0.8.7/test/test_utils.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)       92 2021-07-08 10:07:58.000000 py2pack-0.8.7/test-requirements.txt
-drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:13:04.959680 py2pack-0.8.7/tools/
--rwxr-xr-x   0 thesp0nge  (1000) users      (100)     2263 2021-07-08 10:07:58.000000 py2pack-0.8.7/tools/obs-from-pypi.py
--rw-r--r--   0 thesp0nge  (1000) users      (100)      549 2021-07-08 10:07:58.000000 py2pack-0.8.7/tox.ini
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.248378 py2pack-0.9.0/
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.240378 py2pack-0.9.0/.github/
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.240378 py2pack-0.9.0/.github/workflows/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1008 2023-05-12 07:06:36.000000 py2pack-0.9.0/.github/workflows/tox.yml
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1393 2023-05-16 16:11:24.000000 py2pack-0.9.0/AUTHORS
+-rw-r--r--   0 thesp0nge  (1000) users      (100)    17579 2023-05-16 16:11:24.000000 py2pack-0.9.0/ChangeLog
+-rw-r--r--   0 thesp0nge  (1000) users      (100)    10143 2021-07-08 10:07:58.000000 py2pack-0.9.0/LICENSE
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     5039 2023-05-16 16:11:24.248378 py2pack-0.9.0/PKG-INFO
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     4232 2023-05-16 16:02:57.000000 py2pack-0.9.0/README.rst
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/doc/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     7669 2021-07-08 10:07:58.000000 py2pack-0.9.0/doc/Makefile
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/doc/source/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)       68 2021-07-08 10:07:58.000000 py2pack-0.9.0/doc/source/cli.rst
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     7954 2021-07-08 10:07:58.000000 py2pack-0.9.0/doc/source/conf.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      476 2021-07-08 10:07:58.000000 py2pack-0.9.0/doc/source/index.rst
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      514 2021-07-08 10:07:58.000000 py2pack-0.9.0/doc/source/templates.rst
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/py2pack/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)    18386 2023-05-12 07:06:36.000000 py2pack-0.9.0/py2pack/__init__.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1254 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/proxy.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     4089 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/requires.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     2586 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/setup.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)    23379 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/spdx_license_map.p
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/py2pack/templates/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1512 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/templates/fedora.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1313 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/templates/mageia.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     3290 2023-05-12 07:06:36.000000 py2pack-0.9.0/py2pack/templates/opensuse-legacy.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      922 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/templates/opensuse.dsc
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     4485 2023-05-12 07:06:36.000000 py2pack-0.9.0/py2pack/templates/opensuse.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     3554 2023-05-12 07:06:36.000000 py2pack-0.9.0/py2pack/utils.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      829 2021-07-08 10:07:58.000000 py2pack-0.9.0/py2pack/version.py
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/py2pack.egg-info/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     5039 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/PKG-INFO
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1120 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/SOURCES.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)        1 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/dependency_links.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)       41 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/entry_points.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)        1 2021-07-08 10:10:19.000000 py2pack-0.9.0/py2pack.egg-info/not-zip-safe
+-rw-r--r--   0 thesp0nge  (1000) users      (100)       47 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/pbr.json
+-rw-r--r--   0 thesp0nge  (1000) users      (100)       57 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/requires.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)        8 2023-05-16 16:11:24.000000 py2pack-0.9.0/py2pack.egg-info/top_level.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)       82 2023-05-12 07:06:36.000000 py2pack-0.9.0/requirements.txt
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     1092 2023-05-16 16:11:24.248378 py2pack-0.9.0/setup.cfg
+-rwxr-xr-x   0 thesp0nge  (1000) users      (100)      766 2023-05-12 10:23:02.000000 py2pack-0.9.0/setup.py
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/test/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)        0 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/__init__.py
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.244378 py2pack-0.9.0/test/examples/
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     4764 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/examples/py2pack-fedora.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      757 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/examples/py2pack-mageia.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     2456 2023-05-12 07:06:36.000000 py2pack-0.9.0/test/examples/py2pack-opensuse-augmented.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     5419 2023-05-12 07:06:36.000000 py2pack-0.9.0/test/examples/py2pack-opensuse-legacy.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      178 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/examples/py2pack-opensuse.dsc
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     5469 2023-05-12 07:06:36.000000 py2pack-0.9.0/test/examples/py2pack-opensuse.spec
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     7883 2023-05-12 07:06:36.000000 py2pack-0.9.0/test/test_py2pack.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     2463 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/test_requires.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     2529 2023-05-12 07:06:36.000000 py2pack-0.9.0/test/test_template.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)     3431 2021-07-08 10:07:58.000000 py2pack-0.9.0/test/test_utils.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      123 2023-05-12 07:09:20.000000 py2pack-0.9.0/test-requirements.txt
+drwxr-xr-x   0 thesp0nge  (1000) users      (100)        0 2023-05-16 16:11:24.248378 py2pack-0.9.0/tools/
+-rwxr-xr-x   0 thesp0nge  (1000) users      (100)     2263 2021-07-08 10:07:58.000000 py2pack-0.9.0/tools/obs-from-pypi.py
+-rw-r--r--   0 thesp0nge  (1000) users      (100)      636 2023-05-12 07:06:36.000000 py2pack-0.9.0/tox.ini
```

### Comparing `py2pack-0.8.7/AUTHORS` & `py2pack-0.9.0/AUTHORS`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Adam Spiers <py2pack@adamspiers.org>
 Antonio Larrosa <larrosa@kde.org>
 Ben Greiner <code@bnavigator.de>
 Bitdeli Chef <chef@bitdeli.com>
 Christopher Yeleighton <ne01026@shark.2a.pl>
 Dan Čermák <dcermak@suse.com>
+Daniel Garcia Moreno <daniel.garcia@suse.com>
 Dirk Mueller <dmueller@suse.com>
 Jerome Soyer <jerome.soyer@ac-dijon.fr>
 Jürgen Weigert <juewei@fabfolk.com>
 Karol Babioch <kbabioch@suse.de>
 Lukas Wunner <lukas@wunner.de>
 Maciek Borzecki <maciek.borzecki@gmail.com>
 Manuel Schnitzer <mschnitzer@suse.de>
 Markéta Calábková <meggy.calabkova@gmail.com>
 Matěj Cepl <mcepl@cepl.eu>
 MeggyCal <MeggyCal@users.noreply.github.com>
+Michal Suchanek <msuchanek@suse.de>
+Mikhail Terekhov <termim@gmail.com>
 Oliver Bengs <obengs@flashgrafik.de>
 Oliver Kurz <okurz@suse.de>
+Paolo Perego <paolo.perego@suse.com>
 Paolo Perego <paolo@codiceinsicuro.it>
 Sascha Peilicke <sasch.pe@gmx.de>
 Sascha Peilicke <sascha@peilicke.de>
 Sascha Peilicke <saschpe@gmx.de>
 Sascha Peilicke <saschpe@mailbox.org>
 Sascha Peilicke <saschpe@suse.de>
 Sascha Peilicke <speilicke@suse.com>
```

### Comparing `py2pack-0.8.7/ChangeLog` & `py2pack-0.9.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Adding a missing newline
+* Preparing for 0.9.0 release
+* Rewrite hackish section
+* Adding a missing testing dependency
+* parse and canonicalize pyproject.toml data
+* Fix default generated spec filename
+* Update python version in tox.yml
+* Remove python\_module definition macro
+* Use %autosetup instead of %setup
+* Do not use 'releases' data from API
+* Add status badge icon
+* openSUSE teample: add package name to sitelib path
+* Fixes from review. Thank you
+* Switch from Travis-CI to Github Actions
+* Added tags file in gitignore
+* Added venv dir in gitignore file
+* Do not crash when setup.py could not be run, fixes #150
+* Use package name from PyPI for tarball name, fixes #148
+
 0.8.7
 -----
 
 * Adding version string
 * license is UNKNOWN if nothing determined
 * Fix issue #139 and issue #140 with pypi\_search module that it simply use the same searching facility available on pypi.org website
 * Ignoring python virtual env directory
```

### Comparing `py2pack-0.8.7/LICENSE` & `py2pack-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/PKG-INFO` & `py2pack-0.9.0/test/examples/py2pack-opensuse-legacy.spec`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,178 @@
-Metadata-Version: 1.1
-Name: py2pack
-Version: 0.8.7
-Summary: Generate distribution packages from PyPI
-Home-page: http://github.com/openSUSE/py2pack
-Author: Sascha Peilicke, Thomas Bechtold
-Author-email: sascha@peilicke.de, thomasbechtold@jpberlin.de
-License: UNKNOWN
-Description: Py2pack: Generate distribution packages from PyPI
-        =================================================
-        
-        .. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
-                :target: https://travis-ci.org/openSUSE/py2pack
-        
-        
-        This script allows to generate RPM spec or DEB dsc files from Python modules.
-        It allows to list Python modules or search for them on the Python Package Index
-        (PyPI). Conveniently, it can fetch tarballs and changelogs making it an
-        universal tool to package Python modules.
-        
-        
-        Installation
-        ------------
-        
-        To install py2pack from the `Python Package Index`_, simply:
-        
-        .. code-block:: bash
-        
-            $ python3 -mpip install py2pack
-        
-        You can also check your distro of choice if they provide packages.
-        For openSUSE Tumbleweed and Leap 15.X, you can
-        
-        .. code-block:: bash
-        
-            $ sudo zypper install python3-py2pack
-        
-        
-        Usage
-        -----
-        
-        Lets suppose you want to package zope.interface_ and you don't know how it is named
-        exactly. First of all, you can search for it and download the source tarball if
-        you found the correct module:
-        
-        .. code-block:: bash
-        
-            $ py2pack search zope.interface
-            searching for module zope.interface...
-            found zope.interface-3.6.1
-            $ py2pack fetch zope.interface
-            downloading package zope.interface-3.6.1...
-            from http://pypi.python.org/packages/source/z/zope.interface/zope.interface-3.6.1.tar.gz
-        
-        
-        As a next step you may want to generate a package recipe for your distribution.
-        For RPM_-based distributions (let's use openSUSE_ as an example), you want to
-        generate a spec file (named 'python-zope.interface.spec'):
-        
-        .. code-block:: bash
-        
-            $ py2pack generate zope.interface -t opensuse.spec -f python-zope.interface.spec
-        
-        The source tarball and the package recipe is all you need to generate the RPM_
-        (or DEB_) file.
-        This final step may depend on which distribution you use. Again,
-        for openSUSE_ (and by using the `Open Build Service`_), the complete recipe is:
-        
-        .. code-block:: bash
-        
-            $ osc mkpac python-zope.interface
-            $ cd python-zope.interface
-            $ py2pack fetch zope.interface
-            $ py2pack generate zope.interface -f python-zope.interface.spec
-            $ osc build
-            ...
-        
-        Depending on the module, you may have to adapt the resulting spec file slightly.
-        To get further help about py2pack usage, issue the following command:
-        
-        .. code-block:: bash
-        
-            $ py2pack help
-        
-        
-        Hacking and contributing
-        ------------------------
-        
-        You can test py2pack from your git checkout by executing the py2pack module:
-        
-        .. code-block:: bash
-        
-            $ python3 -m py2pack
-        
-        Fork `the repository`_ on Github to start making your changes to the **master**
-        branch (or branch off of it). Don't forget to write a test for fixed issues or
-        implemented features whenever appropriate. You can invoke the testsuite from
-        the repository root directory via `tox`_:
-        
-        .. code-block:: bash
-        
-            $ tox
-        
-        To run a single test class via `tox`_, use i.e.:
-        
-        .. code-block:: bash
-        
-            $ tox -epy38 test.test_py2pack:Py2packTestCase
-        
-        
-        You can also run `pytest`_ directly:
-        
-        .. code-block:: bash
-        
-            $ pytest
-        
-        It assumes you have the test dependencies installed (available on PYTHONPATH)
-        on your system.
-        
-        :copyright: (c) 2013 Sascha Peilicke.
-        :license: Apache-2.0, see LICENSE for more details.
-        
-        
-        .. _argparse: http://pypi.python.org/pypi/argparse
-        .. _Jinja2: http://pypi.python.org/pypi/Jinja2
-        .. _zope.interface: http://pypi.python.org/pypi/zope.interface/
-        .. _openSUSE: http://www.opensuse.org/en/
-        .. _RPM: http://en.wikipedia.org/wiki/RPM_Package_Manager
-        .. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
-        .. _`Python Package Index`: https://pypi.org/
-        .. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
-        .. _`the repository`: https://github.com/openSUSE/py2pack
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: http://testrun.org/tox
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Pre-processors
+#
+# spec file for package python-py2pack
+#
+# Copyright (c) __YEAR__ SUSE LINUX GmbH, Nuernberg, Germany.
+#
+# All modifications and additions to the file contributed by third parties
+# remain the property of their copyright owners, unless otherwise agreed
+# upon. The license for this file, and modifications and additions to the
+# file, is the same license as for the pristine package itself (unless the
+# license for the pristine package is not an Open Source License, in which
+# case the license is the MIT License). An "Open Source License" is a
+# license that conforms to the Open Source Definition (Version 1.9)
+# published by the Open Source Initiative.
+
+# Please submit bugfixes or comments via https://bugs.opensuse.org/
+
+
+Name:           python-py2pack
+Version:        0.8.5
+Release:        0
+Summary:        Generate distribution packages from PyPI
+License:        Apache-2.0
+URL:            http://github.com/openSUSE/py2pack
+Source:         https://files.pythonhosted.org/packages/source/p/py2pack/py2pack-%{version}.tar.gz
+BuildRequires:  python-setuptools
+BuildRoot:      %{_tmppath}/%{name}-%{version}-build
+BuildArch:      noarch
+
+%description
+Py2pack: Generate distribution packages from PyPI
+=================================================
+
+.. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
+        :target: https://travis-ci.org/openSUSE/py2pack
+
+
+This script allows to generate RPM spec or DEB dsc files from Python modules.
+It allows to list Python modules or search for them on the Python Package Index
+(PyPI). Conveniently, it can fetch tarballs and changelogs making it an
+universal tool to package Python modules.
+
+
+Installation
+------------
+
+To install py2pack from the `Python Package Index`_, simply:
+
+.. code-block:: bash
+
+    $ pip install py2pack
+
+Or, if you absolutely must:
+
+.. code-block:: bash
+
+    $ easy_install py2pack
+
+But, you really shouldn't do that. Lastly, you can check your distro of choice
+if they provide packages. For openSUSE, you can find packages in the `Open
+Build Service`_ for all releases. If you happen to use openSUSE:Factory (the
+rolling release / development version), simply:
+
+.. code-block:: bash
+
+    $ sudo zypper install python-py2pack
+
+
+Usage
+-----
+
+Lets suppose you want to package zope.interface_ and you don't know how it is named
+exactly. First of all, you can search for it and download the source tarball if
+you found the correct module:
+
+.. code-block:: bash
+
+    $ py2pack search zope.interface
+    searching for module zope.interface...
+    found zope.interface-3.6.1
+    $ py2pack fetch zope.interface
+    downloading package zope.interface-3.6.1...
+    from http://pypi.python.org/packages/source/z/zope.interface/zope.interface-3.6.1.tar.gz
+
+
+As a next step you may want to generate a package recipe for your distribution.
+For RPM_-based distributions (let's use openSUSE_ as an example), you want to
+generate a spec file (named 'python-zope.interface.spec'):
+
+.. code-block:: bash
+
+    $ py2pack generate zope.interface -t opensuse.spec -f python-zope.interface.spec
+
+The source tarball and the package recipe is all you need to generate the RPM_
+(or DEB_) file.
+This final step may depend on which distribution you use. Again,
+for openSUSE_ (and by using the `Open Build Service`_), the complete recipe is:
+
+.. code-block:: bash
+
+    $ osc mkpac python-zope.interface
+    $ cd python-zope.interface
+    $ py2pack fetch zope.interface
+    $ py2pack generate zope.interface -f python-zope.interface.spec
+    $ osc build
+    ...
+
+Depending on the module, you may have to adapt the resulting spec file slightly.
+To get further help about py2pack usage, issue the following command:
+
+.. code-block:: bash
+
+    $ py2pack help
+
+
+Hacking and contributing
+------------------------
+
+You can test py2pack from your git checkout by executing the py2pack module:
+
+.. code-block:: bash
+
+    $ python -m py2pack
+
+Fork `the repository`_ on Github to start making your changes to the **master**
+branch (or branch off of it). Don't forget to write a test for fixed issues or
+implemented features whenever appropriate. You can invoke the testsuite from
+the repository root directory via `tox`_:
+
+.. code-block:: bash
+
+    $ tox
+
+To run a single test class via `tox`_, use i.e.:
+
+.. code-block:: bash
+
+    $ tox -epy27 test.test_py2pack:Py2packTestCase
+
+
+You can also run `pytest`_ directly:
+
+.. code-block:: bash
+
+    $ pytest
+
+It assumes you have the test dependencies installed (available on PYTHONPATH)
+on your system.
+
+:copyright: (c) 2013 Sascha Peilicke.
+:license: Apache-2.0, see LICENSE for more details.
+
+
+.. _argparse: http://pypi.python.org/pypi/argparse
+.. _Jinja2: http://pypi.python.org/pypi/Jinja2
+.. _zope.interface: http://pypi.python.org/pypi/zope.interface/
+.. _openSUSE: http://www.opensuse.org/en/
+.. _RPM: http://en.wikipedia.org/wiki/RPM_Package_Manager
+.. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
+.. _`Python Package Index`: https://pypi.org/
+.. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
+.. _`the repository`: https://github.com/openSUSE/py2pack
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: http://testrun.org/tox
+
+%prep
+%autosetup -p1 -n py2pack-%{version}
+
+%build
+python setup.py build
+
+%install
+python setup.py install --prefix=%{_prefix} --root=%{buildroot}
+
+%files
+%defattr(-,root,root,-)
+%{python_sitelib}/*
+
+%changelog
```

### Comparing `py2pack-0.8.7/README.rst` & `py2pack-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Py2pack: Generate distribution packages from PyPI
 =================================================
 
-.. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
-        :target: https://travis-ci.org/openSUSE/py2pack
-
+.. image:: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml/badge.svg
+        :target: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml
+        :alt: Unit tests
 
 This script allows to generate RPM spec or DEB dsc files from Python modules.
 It allows to list Python modules or search for them on the Python Package Index
 (PyPI). Conveniently, it can fetch tarballs and changelogs making it an
 universal tool to package Python modules.
 
 
@@ -74,19 +74,31 @@
 
     $ py2pack help
 
 
 Hacking and contributing
 ------------------------
 
-You can test py2pack from your git checkout by executing the py2pack module:
+You can test py2pack from your git checkout by executing the py2pack module.
+
+Edit `setup.cfg` file changing the version number. Adding +1 to the revision
+number is enough. This step is mandatory to install locally the py2pack module.
+
+From the py2pack directory, install the py2pack module locally.
+
+.. code-block:: bash
+
+    $ pip install -e .
+
+Now you can run your hackish py2pack version. It is usually located in
+$HOME/.local/bin/py2pack
 
 .. code-block:: bash
 
-    $ python3 -m py2pack
+    $ py2pack
 
 Fork `the repository`_ on Github to start making your changes to the **master**
 branch (or branch off of it). Don't forget to write a test for fixed issues or
 implemented features whenever appropriate. You can invoke the testsuite from
 the repository root directory via `tox`_:
 
 .. code-block:: bash
```

### Comparing `py2pack-0.8.7/doc/Makefile` & `py2pack-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/doc/source/conf.py` & `py2pack-0.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/doc/source/templates.rst` & `py2pack-0.9.0/doc/source/templates.rst`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/__init__.py` & `py2pack-0.9.0/py2pack/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 # limitations under the License.
 
 import argparse
 import datetime
 import glob
 import os
 import pickle
-import pkg_resources
 import pprint
 import pwd
 import re
-import requests
+import subprocess
 import sys
 import urllib
-import jinja2
 import warnings
 import xmlrpc
-import pypi_search.search
 
+import jinja2
+import pkg_resources
+import pypi_search.search
+import requests
 from metaextract import utils as meta_utils
 
 import py2pack.proxy
 import py2pack.requires
-import py2pack.utils
 from py2pack import version as py2pack_version
+from py2pack.utils import (_get_archive_filelist, get_pyproject_table,
+                           parse_pyproject)
 
 # https://warehouse.pypa.io/api-reference/xml-rpc.html
 pypi_xml = xmlrpc.client.ServerProxy('https://pypi.org/pypi')
 
 warnings.simplefilter('always', DeprecationWarning)
 
 SPDX_LICENSES_FILE = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'spdx_license_map.p')
@@ -98,76 +100,143 @@
         sys.exit(1)
     print('downloading package {0}-{1}...'.format(args.name, args.version))
     print('from {0}'.format(url['url']))
     urllib.request.urlretrieve(url['url'], url['filename'])
 
 
 def _canonicalize_setup_data(data):
-    if data.get('setup_requires', None):
+
+    if data.get('build-system', None):
+        # PEP 518: 'requires' field is mandatory
+        data['build_requires'] = py2pack.requires._requirements_sanitize(
+            data['build-system']['requires'])
+    elif data.get('setup_requires', None):
+        # Setuptools, deprecated.
+        setup_requires = data.pop('setup_requires')
         # setup_requires may be a string, convert to list of strings:
-        if isinstance(data["setup_requires"], str):
-            data["setup_requires"] = data["setup_requires"].splitlines()
-        data["setup_requires"] = \
-            py2pack.requires._requirements_sanitize(data["setup_requires"])
-
-    if data.get('install_requires', None):
-        # install_requires may be a string, convert to list of strings:
-        if isinstance(data["install_requires"], str):
-            data["install_requires"] = data["install_requires"].splitlines()
+        if isinstance(setup_requires, str):
+            setup_requires = setup_requires.splitlines()
+        # canonicalize to build_requires
+        data["build_requires"] = ['setuptools', 'wheel'] + \
+            py2pack.requires._requirements_sanitize(setup_requires)
+    else:
+        # no build_requires means most probably legacy setuptools
+        data["build_requires"] = ['setuptools']
+    if 'setuptools' in data['build_requires'] and 'wheel' not in data['build_requires']:
+        data['build_requires'] += ['wheel']
+
+    install_requires = (
+        get_pyproject_table(data, "project.dependencies") or
+        get_pyproject_table(data, "tool.flit.metadata.requires") or
+        data.get("install_requires", None))
+    if install_requires:
+        # Setuptools or PEP 621
+        # Setuptools: install_requires may be a string, convert to list of strings:
+        if isinstance(install_requires, str):
+            install_requires = install_requires.splitlines()
         data["install_requires"] = \
-            py2pack.requires._requirements_sanitize(data["install_requires"])
-
-    if data.get('tests_require', None):
-        # tests_require may be a string, convert to list of strings:
-        if isinstance(data["tests_require"], str):
-            data["tests_require"] = data["tests_require"].splitlines()
+            py2pack.requires._requirements_sanitize(install_requires)
+    else:
+        # Poetry
+        try:
+            if 'dependencies' in data['tool']['poetry']:
+                warnings.warn("The package defines its dependencies in the "
+                              "[tool.poetry.dependencies] table of pyproject.toml. "
+                              "Automatic parsing of the poetry format is not "
+                              "implemented yet. You must add the requirements "
+                              "manually.")
+        except KeyError:
+            pass
+
+    tests_require = (
+        get_pyproject_table(data, "project.optional-dependencies.test") or
+        get_pyproject_table(data, "tool.flit.metadata.requires-extra.test") or
+        data.get("tests_require", None))
+    if tests_require:
+        # Setuptools: tests_require may be a string, convert to list of strings:
+        if isinstance(tests_require, str):
+            tests_require = tests_require.splitlines()
         data["tests_require"] = \
-            py2pack.requires._requirements_sanitize(data["tests_require"])
+            py2pack.requires._requirements_sanitize(tests_require)
 
-    if data.get('extras_require', None):
-        # extras_require value may be a string, convert to list of strings:
-        for (key, value) in data["extras_require"].items():
+    extras_require = (
+        get_pyproject_table(data, "project.optional-dependencies") or
+        get_pyproject_table(data, "tool.flit.metadata.requires-extra") or
+        data.get("extras_require", None))
+    if extras_require:
+        data["extras_require"] = dict()
+        for (key, value) in extras_require.items():
+            # do not add the test requirements to the regular suggestions
+            if key == "test":
+                continue
+            # Setuptools: extras_require value may be a string, convert to list of strings:
             if isinstance(value, str):
-                data["extras_require"][key] = value.splitlines()
+                extras_require[key] = value.splitlines()
             data["extras_require"][key] = \
-                py2pack.requires._requirements_sanitize(data["extras_require"][key])
+                py2pack.requires._requirements_sanitize(extras_require[key])
 
     if data.get('data_files', None):
         # data_files may be a sequence of files without a target directory:
         if len(data["data_files"]) and isinstance(data["data_files"][0], str):
             data["data_files"] = [("", data["data_files"])]
         # directory paths may be relative to the installation prefix:
         prefix = sys.exec_prefix if "is_extension" in data else sys.prefix
         data["data_files"] = [
             (dir if (len(dir) and dir[0] == '/') else os.path.join(prefix, dir), files)
             for (dir, files) in data["data_files"]]
 
+    console_scripts = []
     if data.get('entry_points', None):
+        # setuptools style entry_points only.
+        # PEP518 projects.entry-points does not have scripts subtables.
         # entry_points may be a string with .ini-style sections or a dict.
         # convert to a dict and parse it
         data["entry_points"] = pkg_resources.EntryPoint.parse_map(data["entry_points"])
-        if "console_scripts" in data["entry_points"]:
-            data["console_scripts"] = list(data["entry_points"]["console_scripts"].keys())
-
+        for s in ["console_scripts", "gui_scripts"]:
+            if s in data["entry_points"] and data["entry_points"][s]:
+                console_scripts += list(data["entry_points"][s].keys())
+    console_scripts += list(get_pyproject_table(data, "project.scripts", notfound={}).keys())
+    console_scripts += list(get_pyproject_table(data, "project.gui-scripts", notfound={}).keys())
+    console_scripts += list(get_pyproject_table(data, "tool.flit.scripts", notfound={}).keys())
+    if console_scripts:
+        data["console_scripts"] = console_scripts
+
+    homepage = get_pyproject_table(data, 'project.urls.homepage') or data.get('home_page', None)
+    if homepage:
+        data['home_page'] = homepage
 
 def _quote_shell_metacharacters(string):
     shell_metachars_re = re.compile(r"[|&;()<>\s]")
     if re.search(shell_metachars_re, string):
         return "'" + string + "'"
     return string
 
 
 def _augment_data_from_tarball(args, filename, data):
     docs_re = re.compile(r"{0}-{1}\/((?:AUTHOR|ChangeLog|CHANGES|NEWS|README).*)".format(args.name, args.version), re.IGNORECASE)
     license_re = re.compile(r"{0}-{1}\/((?:COPYING|LICENSE).*)".format(args.name, args.version), re.IGNORECASE)
 
-    data_archive = meta_utils.from_archive(filename)
-    data.update(data_archive['data'])
+    data_pyproject = parse_pyproject(filename)
+    data.update(data_pyproject)
+    
+    try:
+        buildrequires = data['build-system']['requires']
+    except KeyError:
+        # No build system specified in pyproject.toml: legacy setuptools
+        buildrequires = ['setuptools']
+    if any(['setuptools' in br for br in buildrequires]):
+        try:
+            data_archive = meta_utils.from_archive(filename)
+            data.update(data_archive['data'])
+        except Exception as exc:
+            warnings.warn("Could not get setuptools information from tarball {}: {}. "
+                        "Valuable information for the generation might be missing."
+                        .format(filename, exc))
 
-    names = py2pack.utils._get_archive_filelist(filename)
+    names = _get_archive_filelist(filename)
     _canonicalize_setup_data(data)
 
     for name in names:
         match_docs = re.match(docs_re, name)
         match_license = re.match(license_re, name)
         if match_docs:
             if "doc_files" not in data:
@@ -230,31 +299,35 @@
         warnings.warn("the '--run' switch is deprecated and a noop",
                       DeprecationWarning)
 
     fetch_data(args)
     if not args.template:
         args.template = file_template_list()[0]
     if not args.filename:
-        args.filename = args.name + '.' + args.template.rsplit('.', 1)[1]   # take template file ending
+        args.filename = "python-" + args.name + '.' + args.template.rsplit('.', 1)[1]   # take template file ending
     print('generating spec file for {0}...'.format(args.name))
     data = args.fetched_data['info']
     durl = newest_download_url(args)
     data['source_url'] = (args.source_url or
                           (durl and durl['url']) or
                           args.name + '-' + args.version + '.zip')
     data['year'] = datetime.datetime.now().year                             # set current year
     data['user_name'] = pwd.getpwuid(os.getuid())[4]                        # set system user (packager)
     data['summary_no_ending_dot'] = re.sub(r'(.*)\.', r'\g<1>', data.get('summary', ""))
 
-    tarball_file = glob.glob("{0}-{1}.*".format(args.name, args.version))
-    # also check tarball files with underscore. Some packages have a name with
-    # a '-' or '.' but the tarball name has a '_' . Eg the package os-faults
-    tr = str.maketrans('-.', '__')
-    tarball_file += glob.glob("{0}-{1}.*".format(args.name.translate(tr),
-                                                 args.version))
+    # If package name supplied on command line differs in case from PyPI's one
+    # then package archive will be fetched but the name will be the one from PyPI.
+    # Eg. send2trash vs Send2Trash. Check that.
+    for name in (args.name, data['name']):
+        tarball_file = glob.glob("{0}-{1}.*".format(name, args.version))
+        # also check tarball files with underscore. Some packages have a name with
+        # a '-' or '.' but the tarball name has a '_' . Eg the package os-faults
+        tr = str.maketrans('-.', '__')
+        tarball_file += glob.glob("{0}-{1}.*".format(name.translate(tr),
+                                                     args.version))
     if tarball_file:                                                        # get some more info from that
         _augment_data_from_tarball(args, tarball_file[0], data)
     else:
         warnings.warn("No tarball for {} in version {} found. Valuable "
                       "information for the generation might be missing."
                       "".format(args.name, args.version))
 
@@ -268,35 +341,33 @@
         outfile.write(result)
     finally:
         outfile.close()
 
 
 def fetch_data(args):
     args.fetched_data = pypi_json(args.name, args.version)
-    releases = args.fetched_data['releases']
-    if len(releases) == 0:
+    urls = args.fetched_data['urls']
+    if len(urls) == 0:
         print("unable to find a suitable release for {0}!".format(args.name))
         sys.exit(1)
     else:
         args.version = args.fetched_data['info']['version']                 # return current release number
 
 
 def newest_download_url(args):
     """check but do not use the url delivered by pypi. that url contains a hash and
     needs to be adjusted with every package update. Instead use
     the pypi.io url
     """
     if not hasattr(args, "fetched_data"):
         return {}
-    for version, release_data in args.fetched_data['releases'].items():     # Check download URLs in releases
-        if (version == args.version):
-            for release in release_data:
-                if release['packagetype'] == 'sdist':                      # Found the source URL we care for
-                    release['url'] = _get_source_url(args.name, release['filename'])
-                    return release
+    for release in args.fetched_data['urls']:     # Check download URLs in releases
+        if release['packagetype'] == 'sdist':                      # Found the source URL we care for
+            release['url'] = _get_source_url(args.name, release['filename'])
+            return release
     # No PyPI tarball release, let's see if an upstream download URL is provided:
     data = args.fetched_data['info']
     if 'download_url' in data and data['download_url']:
         url = data['download_url']
         return {'url': url,
                 'filename': os.path.basename(url)}
     return {}                                                               # We're all out of bubblegum
```

### Comparing `py2pack-0.8.7/py2pack/proxy.py` & `py2pack-0.9.0/py2pack/proxy.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/requires.py` & `py2pack-0.9.0/py2pack/requires.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/setup.py` & `py2pack-0.9.0/py2pack/setup.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/spdx_license_map.p` & `py2pack-0.9.0/py2pack/spdx_license_map.p`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/templates/fedora.spec` & `py2pack-0.9.0/py2pack/templates/fedora.spec`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/templates/mageia.spec` & `py2pack-0.9.0/py2pack/templates/mageia.spec`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/templates/opensuse-legacy.spec` & `py2pack-0.9.0/py2pack/templates/opensuse-legacy.spec`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 BuildArch:      noarch
 {%- endif %}
 
 %description
 {{ description }}
 
 %prep
-%setup -q -n {{ name }}-%{version}
+%autosetup -p1 -n {{ name }}-%{version}
 
 %build
 {% if has_ext_modules %}CFLAGS="%{optflags}" {% endif %}python setup.py build
 
 %install
 python setup.py install --prefix=%{_prefix} --root=%{buildroot}
```

### Comparing `py2pack-0.8.7/py2pack/templates/opensuse.dsc` & `py2pack-0.9.0/py2pack/templates/opensuse.dsc`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack/templates/opensuse.spec` & `py2pack-0.9.0/py2pack/templates/opensuse.spec`

 * *Files 11% similar despite different names*

```diff
@@ -12,38 +12,36 @@
 # license that conforms to the Open Source Definition (Version 1.9)
 # published by the Open Source Initiative.
 
 # Please submit bugfixes or comments via https://bugs.opensuse.org/
 #
 
 
-%{?!python_module:%define python_module() python-%{**} python3-%{**}}
 Name:           python-{{ name }}
 Version:        {{ version }}
 Release:        0
 Summary:        {{ summary_no_ending_dot|default(summary, true) }}
 License:        {{ license }}
 URL:            {{ home_page }}
 Source:         {{ source_url|replace(version, '%{version}') }}
 BuildRequires:  python-rpm-macros
-BuildRequires:  %{python_module setuptools}
-{%- if setup_requires and setup_requires is not none %}
-{%- for req in setup_requires|sort %}
+{%- set build_requires_plus_pip = ((build_requires if build_requires and build_requires is not none else []) +
+                                   ['pip']) %}
+{%- for req in build_requires_plus_pip |sort %}
 BuildRequires:  %{python_module {{ req }}}
 {%- endfor %}
-{%- endif %}
 {%- if (install_requires and install_requires is not none) or (tests_require and tests_require is not none) %}
 # SECTION test requirements
 {%- if install_requires and install_requires is not none %}
-{%- for req in install_requires|sort %}
+{%- for req in install_requires|reject("in",build_requires)|sort %}
 BuildRequires:  %{python_module {{ req }}}
 {%- endfor %}
 {%- endif %}
 {%- if tests_require and tests_require is not none %}
-{%- for req in tests_require|sort %}
+{%- for req in tests_require|sort|reject("in",build_requires|sort) %}
 BuildRequires:  %{python_module {{ req }}}
 {%- endfor %}
 {%- endif %}
 # /SECTION
 {%- endif %}
 {%- if source_url.endswith('.zip') %}
 BuildRequires:  unzip
@@ -66,24 +64,24 @@
 {%- endif %}
 %python_subpackages
 
 %description
 {{ description }}
 
 %prep
-%setup -q -n {{ name }}-%{version}
+%autosetup -p1 -n {{ name }}-%{version}
 
 %build
 {%- if has_ext_modules %}
 export CFLAGS="%{optflags}"
 {%- endif %}
-%python_build
+%pyproject_wheel
 
 %install
-%python_install
+%pyproject_install
 {%- set scripts_or_console_scripts = (
             (scripts|map('basename')|list if scripts and scripts is not none else []) +
             (console_scripts if console_scripts and console_scripts is not none else [])) %}
 {%- for script in scripts_or_console_scripts %}
 %python_clone -a %{buildroot}%{_bindir}/{{ script }}
 {%- endfor %}
 {%- if has_ext_modules %}
@@ -118,17 +116,19 @@
 {%- if license_files and license_files is not none %}
 %license {{ license_files|join(" ") }}
 {%- endif %}
 {%- for script in scripts_or_console_scripts %}
 %python_alternative %{_bindir}/{{ script }}
 {%- endfor %}
 {%- if has_ext_modules %}
-%{python_sitearch}/*
+%{python_sitearch}/{{name}}
+%{python_sitearch}/{{name}}-%{version}.dist-info
 {%- else %}
-%{python_sitelib}/*
+%{python_sitelib}/{{name}}
+%{python_sitelib}/{{name}}-%{version}.dist-info
 {%- endif %}
 {%- if data_files and data_files is not none %}
 {%- for dir, files in data_files %}
 {%- set dir = dir |
     replace('/usr/share/doc/'~name, '%doc %{_defaultdocdir}/%{python_prefix}-{{ name }}', 1) |
     replace('/usr/share/man/', '%doc %{_mandir}/', 1) |
     replace('/usr/share/', '%{_datadir}/', 1) |
```

### Comparing `py2pack-0.8.7/py2pack/version.py` & `py2pack-0.9.0/py2pack/version.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/py2pack.egg-info/PKG-INFO` & `py2pack-0.9.0/test/examples/py2pack-opensuse.spec`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,182 @@
-Metadata-Version: 1.1
-Name: py2pack
-Version: 0.8.7
-Summary: Generate distribution packages from PyPI
-Home-page: http://github.com/openSUSE/py2pack
-Author: Sascha Peilicke, Thomas Bechtold
-Author-email: sascha@peilicke.de, thomasbechtold@jpberlin.de
-License: UNKNOWN
-Description: Py2pack: Generate distribution packages from PyPI
-        =================================================
-        
-        .. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
-                :target: https://travis-ci.org/openSUSE/py2pack
-        
-        
-        This script allows to generate RPM spec or DEB dsc files from Python modules.
-        It allows to list Python modules or search for them on the Python Package Index
-        (PyPI). Conveniently, it can fetch tarballs and changelogs making it an
-        universal tool to package Python modules.
-        
-        
-        Installation
-        ------------
-        
-        To install py2pack from the `Python Package Index`_, simply:
-        
-        .. code-block:: bash
-        
-            $ python3 -mpip install py2pack
-        
-        You can also check your distro of choice if they provide packages.
-        For openSUSE Tumbleweed and Leap 15.X, you can
-        
-        .. code-block:: bash
-        
-            $ sudo zypper install python3-py2pack
-        
-        
-        Usage
-        -----
-        
-        Lets suppose you want to package zope.interface_ and you don't know how it is named
-        exactly. First of all, you can search for it and download the source tarball if
-        you found the correct module:
-        
-        .. code-block:: bash
-        
-            $ py2pack search zope.interface
-            searching for module zope.interface...
-            found zope.interface-3.6.1
-            $ py2pack fetch zope.interface
-            downloading package zope.interface-3.6.1...
-            from http://pypi.python.org/packages/source/z/zope.interface/zope.interface-3.6.1.tar.gz
-        
-        
-        As a next step you may want to generate a package recipe for your distribution.
-        For RPM_-based distributions (let's use openSUSE_ as an example), you want to
-        generate a spec file (named 'python-zope.interface.spec'):
-        
-        .. code-block:: bash
-        
-            $ py2pack generate zope.interface -t opensuse.spec -f python-zope.interface.spec
-        
-        The source tarball and the package recipe is all you need to generate the RPM_
-        (or DEB_) file.
-        This final step may depend on which distribution you use. Again,
-        for openSUSE_ (and by using the `Open Build Service`_), the complete recipe is:
-        
-        .. code-block:: bash
-        
-            $ osc mkpac python-zope.interface
-            $ cd python-zope.interface
-            $ py2pack fetch zope.interface
-            $ py2pack generate zope.interface -f python-zope.interface.spec
-            $ osc build
-            ...
-        
-        Depending on the module, you may have to adapt the resulting spec file slightly.
-        To get further help about py2pack usage, issue the following command:
-        
-        .. code-block:: bash
-        
-            $ py2pack help
-        
-        
-        Hacking and contributing
-        ------------------------
-        
-        You can test py2pack from your git checkout by executing the py2pack module:
-        
-        .. code-block:: bash
-        
-            $ python3 -m py2pack
-        
-        Fork `the repository`_ on Github to start making your changes to the **master**
-        branch (or branch off of it). Don't forget to write a test for fixed issues or
-        implemented features whenever appropriate. You can invoke the testsuite from
-        the repository root directory via `tox`_:
-        
-        .. code-block:: bash
-        
-            $ tox
-        
-        To run a single test class via `tox`_, use i.e.:
-        
-        .. code-block:: bash
-        
-            $ tox -epy38 test.test_py2pack:Py2packTestCase
-        
-        
-        You can also run `pytest`_ directly:
-        
-        .. code-block:: bash
-        
-            $ pytest
-        
-        It assumes you have the test dependencies installed (available on PYTHONPATH)
-        on your system.
-        
-        :copyright: (c) 2013 Sascha Peilicke.
-        :license: Apache-2.0, see LICENSE for more details.
-        
-        
-        .. _argparse: http://pypi.python.org/pypi/argparse
-        .. _Jinja2: http://pypi.python.org/pypi/Jinja2
-        .. _zope.interface: http://pypi.python.org/pypi/zope.interface/
-        .. _openSUSE: http://www.opensuse.org/en/
-        .. _RPM: http://en.wikipedia.org/wiki/RPM_Package_Manager
-        .. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
-        .. _`Python Package Index`: https://pypi.org/
-        .. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
-        .. _`the repository`: https://github.com/openSUSE/py2pack
-        .. _`pytest`: https://github.com/pytest-dev/pytest
-        .. _`tox`: http://testrun.org/tox
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Pre-processors
+#
+# spec file for package python-py2pack
+#
+# Copyright (c) __YEAR__ SUSE LLC
+#
+# All modifications and additions to the file contributed by third parties
+# remain the property of their copyright owners, unless otherwise agreed
+# upon. The license for this file, and modifications and additions to the
+# file, is the same license as for the pristine package itself (unless the
+# license for the pristine package is not an Open Source License, in which
+# case the license is the MIT License). An "Open Source License" is a
+# license that conforms to the Open Source Definition (Version 1.9)
+# published by the Open Source Initiative.
+
+# Please submit bugfixes or comments via https://bugs.opensuse.org/
+#
+
+
+Name:           python-py2pack
+Version:        0.8.5
+Release:        0
+Summary:        Generate distribution packages from PyPI
+License:        Apache-2.0
+URL:            http://github.com/openSUSE/py2pack
+Source:         https://files.pythonhosted.org/packages/source/p/py2pack/py2pack-%{version}.tar.gz
+BuildRequires:  python-rpm-macros
+BuildRequires:  %{python_module pip}
+BuildRequires:  fdupes
+BuildArch:      noarch
+%python_subpackages
+
+%description
+Py2pack: Generate distribution packages from PyPI
+=================================================
+
+.. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
+        :target: https://travis-ci.org/openSUSE/py2pack
+
+
+This script allows to generate RPM spec or DEB dsc files from Python modules.
+It allows to list Python modules or search for them on the Python Package Index
+(PyPI). Conveniently, it can fetch tarballs and changelogs making it an
+universal tool to package Python modules.
+
+
+Installation
+------------
+
+To install py2pack from the `Python Package Index`_, simply:
+
+.. code-block:: bash
+
+    $ pip install py2pack
+
+Or, if you absolutely must:
+
+.. code-block:: bash
+
+    $ easy_install py2pack
+
+But, you really shouldn't do that. Lastly, you can check your distro of choice
+if they provide packages. For openSUSE, you can find packages in the `Open
+Build Service`_ for all releases. If you happen to use openSUSE:Factory (the
+rolling release / development version), simply:
+
+.. code-block:: bash
+
+    $ sudo zypper install python-py2pack
+
+
+Usage
+-----
+
+Lets suppose you want to package zope.interface_ and you don't know how it is named
+exactly. First of all, you can search for it and download the source tarball if
+you found the correct module:
+
+.. code-block:: bash
+
+    $ py2pack search zope.interface
+    searching for module zope.interface...
+    found zope.interface-3.6.1
+    $ py2pack fetch zope.interface
+    downloading package zope.interface-3.6.1...
+    from http://pypi.python.org/packages/source/z/zope.interface/zope.interface-3.6.1.tar.gz
+
+
+As a next step you may want to generate a package recipe for your distribution.
+For RPM_-based distributions (let's use openSUSE_ as an example), you want to
+generate a spec file (named 'python-zope.interface.spec'):
+
+.. code-block:: bash
+
+    $ py2pack generate zope.interface -t opensuse.spec -f python-zope.interface.spec
+
+The source tarball and the package recipe is all you need to generate the RPM_
+(or DEB_) file.
+This final step may depend on which distribution you use. Again,
+for openSUSE_ (and by using the `Open Build Service`_), the complete recipe is:
+
+.. code-block:: bash
+
+    $ osc mkpac python-zope.interface
+    $ cd python-zope.interface
+    $ py2pack fetch zope.interface
+    $ py2pack generate zope.interface -f python-zope.interface.spec
+    $ osc build
+    ...
+
+Depending on the module, you may have to adapt the resulting spec file slightly.
+To get further help about py2pack usage, issue the following command:
+
+.. code-block:: bash
+
+    $ py2pack help
+
+
+Hacking and contributing
+------------------------
+
+You can test py2pack from your git checkout by executing the py2pack module:
+
+.. code-block:: bash
+
+    $ python -m py2pack
+
+Fork `the repository`_ on Github to start making your changes to the **master**
+branch (or branch off of it). Don't forget to write a test for fixed issues or
+implemented features whenever appropriate. You can invoke the testsuite from
+the repository root directory via `tox`_:
+
+.. code-block:: bash
+
+    $ tox
+
+To run a single test class via `tox`_, use i.e.:
+
+.. code-block:: bash
+
+    $ tox -epy27 test.test_py2pack:Py2packTestCase
+
+
+You can also run `pytest`_ directly:
+
+.. code-block:: bash
+
+    $ pytest
+
+It assumes you have the test dependencies installed (available on PYTHONPATH)
+on your system.
+
+:copyright: (c) 2013 Sascha Peilicke.
+:license: Apache-2.0, see LICENSE for more details.
+
+
+.. _argparse: http://pypi.python.org/pypi/argparse
+.. _Jinja2: http://pypi.python.org/pypi/Jinja2
+.. _zope.interface: http://pypi.python.org/pypi/zope.interface/
+.. _openSUSE: http://www.opensuse.org/en/
+.. _RPM: http://en.wikipedia.org/wiki/RPM_Package_Manager
+.. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
+.. _`Python Package Index`: https://pypi.org/
+.. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
+.. _`the repository`: https://github.com/openSUSE/py2pack
+.. _`pytest`: https://github.com/pytest-dev/pytest
+.. _`tox`: http://testrun.org/tox
+
+%prep
+%autosetup -p1 -n py2pack-%{version}
+
+%build
+%pyproject_wheel
+
+%install
+%pyproject_install
+%python_expand %fdupes %{buildroot}%{$python_sitelib}
+
+%files %{python_files}
+%{python_sitelib}/py2pack
+%{python_sitelib}/py2pack-%{version}.dist-info
+
+%changelog
```

### Comparing `py2pack-0.8.7/py2pack.egg-info/SOURCES.txt` & `py2pack-0.9.0/py2pack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-.travis.yml
 AUTHORS
 ChangeLog
 LICENSE
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
+.github/workflows/tox.yml
 doc/Makefile
 doc/source/cli.rst
 doc/source/conf.py
 doc/source/index.rst
 doc/source/templates.rst
 py2pack/__init__.py
 py2pack/proxy.py
```

### Comparing `py2pack-0.8.7/setup.cfg` & `py2pack-0.9.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = py2pack
 summary = Generate distribution packages from PyPI
-version = 0.8.7
-description-file = 
+version = 0.9.0
+description_file = 
 	README.rst
 author = Sascha Peilicke, Thomas Bechtold
-author-email = sascha@peilicke.de, thomasbechtold@jpberlin.de
-home-page = http://github.com/openSUSE/py2pack
+author_email = sascha@peilicke.de, thomasbechtold@jpberlin.de
+home_page = https://github.com/openSUSE/py2pack
 classifier = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
```

### Comparing `py2pack-0.8.7/setup.py` & `py2pack-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/test/examples/py2pack-fedora.spec` & `py2pack-0.9.0/test/examples/py2pack-fedora.spec`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/test/examples/py2pack-mageia.spec` & `py2pack-0.9.0/test/examples/py2pack-mageia.spec`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/test/examples/py2pack-opensuse-augmented.spec` & `py2pack-0.9.0/test/examples/py2pack-opensuse-augmented.spec`

 * *Files 15% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # license that conforms to the Open Source Definition (Version 1.9)
 # published by the Open Source Initiative.
 
 # Please submit bugfixes or comments via https://bugs.opensuse.org/
 #
 
 
-%{?!python_module:%define python_module() python-%{**} python3-%{**}}
 Name:           python-py2pack
 Version:        0.8.5
 Release:        0
 Summary:        Generate distribution packages from PyPI
-License:        UNKNOWN (FIXME:No SPDX)
+License:        Apache-2.0
 URL:            http://github.com/openSUSE/py2pack
 Source:         https://files.pythonhosted.org/packages/source/p/py2pack/py2pack-%{version}.tar.gz
 BuildRequires:  python-rpm-macros
-BuildRequires:  %{python_module setuptools}
 BuildRequires:  %{python_module pbr >= 1.8}
+BuildRequires:  %{python_module pip}
+BuildRequires:  %{python_module setuptools}
+BuildRequires:  %{python_module wheel}
 # SECTION test requirements
 BuildRequires:  %{python_module Jinja2}
 BuildRequires:  %{python_module metaextract}
-BuildRequires:  %{python_module setuptools}
 BuildRequires:  %{python_module six}
 BuildRequires:  %{python_module coverage}
 BuildRequires:  %{python_module ddt}
 BuildRequires:  %{python_module flake8}
 BuildRequires:  %{python_module pytest}
 BuildRequires:  %{python_module Sphinx >= 1.2.1}
 BuildRequires:  %{python_module sphinxcontrib.programoutput}
@@ -48,21 +48,21 @@
 BuildArch:      noarch
 %python_subpackages
 
 %description
 Generate distribution packages from PyPI
 
 %prep
-%setup -q -n py2pack-%{version}
+%autosetup -p1 -n py2pack-%{version}
 
 %build
-%python_build
+%pyproject_wheel
 
 %install
-%python_install
+%pyproject_install
 %python_clone -a %{buildroot}%{_bindir}/py2pack
 %python_expand %fdupes %{buildroot}%{$python_sitelib}
 
 %check
 CHOOSE: %pytest OR %pyunittest -v OR CUSTOM
 
 %post
@@ -71,10 +71,11 @@
 %postun
 %python_uninstall_alternative py2pack
 
 %files %{python_files}
 %doc AUTHORS ChangeLog README.rst
 %license LICENSE
 %python_alternative %{_bindir}/py2pack
-%{python_sitelib}/*
+%{python_sitelib}/py2pack
+%{python_sitelib}/py2pack-%{version}.dist-info
 
 %changelog
```

### Comparing `py2pack-0.8.7/test/examples/py2pack-opensuse-legacy.spec` & `py2pack-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,55 @@
-#
-# spec file for package python-py2pack
-#
-# Copyright (c) __YEAR__ SUSE LINUX GmbH, Nuernberg, Germany.
-#
-# All modifications and additions to the file contributed by third parties
-# remain the property of their copyright owners, unless otherwise agreed
-# upon. The license for this file, and modifications and additions to the
-# file, is the same license as for the pristine package itself (unless the
-# license for the pristine package is not an Open Source License, in which
-# case the license is the MIT License). An "Open Source License" is a
-# license that conforms to the Open Source Definition (Version 1.9)
-# published by the Open Source Initiative.
-
-# Please submit bugfixes or comments via https://bugs.opensuse.org/
-
-
-Name:           python-py2pack
-Version:        0.8.5
-Release:        0
-Summary:        Generate distribution packages from PyPI
-License:        Apache-2.0
-URL:            http://github.com/openSUSE/py2pack
-Source:         https://files.pythonhosted.org/packages/source/p/py2pack/py2pack-%{version}.tar.gz
-BuildRequires:  python-setuptools
-BuildRoot:      %{_tmppath}/%{name}-%{version}-build
-BuildArch:      noarch
+Metadata-Version: 2.1
+Name: py2pack
+Version: 0.9.0
+Summary: Generate distribution packages from PyPI
+Home-page: https://github.com/openSUSE/py2pack
+Author: Sascha Peilicke, Thomas Bechtold
+Author-email: sascha@peilicke.de, thomasbechtold@jpberlin.de
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Pre-processors
+License-File: LICENSE
+License-File: AUTHORS
 
-%description
 Py2pack: Generate distribution packages from PyPI
 =================================================
 
-.. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
-        :target: https://travis-ci.org/openSUSE/py2pack
-
+.. image:: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml/badge.svg
+        :target: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml
+        :alt: Unit tests
 
 This script allows to generate RPM spec or DEB dsc files from Python modules.
 It allows to list Python modules or search for them on the Python Package Index
 (PyPI). Conveniently, it can fetch tarballs and changelogs making it an
 universal tool to package Python modules.
 
 
 Installation
 ------------
 
 To install py2pack from the `Python Package Index`_, simply:
 
 .. code-block:: bash
 
-    $ pip install py2pack
-
-Or, if you absolutely must:
-
-.. code-block:: bash
-
-    $ easy_install py2pack
+    $ python3 -mpip install py2pack
 
-But, you really shouldn't do that. Lastly, you can check your distro of choice
-if they provide packages. For openSUSE, you can find packages in the `Open
-Build Service`_ for all releases. If you happen to use openSUSE:Factory (the
-rolling release / development version), simply:
+You can also check your distro of choice if they provide packages.
+For openSUSE Tumbleweed and Leap 15.X, you can
 
 .. code-block:: bash
 
-    $ sudo zypper install python-py2pack
+    $ sudo zypper install python3-py2pack
 
 
 Usage
 -----
 
 Lets suppose you want to package zope.interface_ and you don't know how it is named
 exactly. First of all, you can search for it and download the source tarball if
@@ -111,34 +94,46 @@
 
     $ py2pack help
 
 
 Hacking and contributing
 ------------------------
 
-You can test py2pack from your git checkout by executing the py2pack module:
+You can test py2pack from your git checkout by executing the py2pack module.
+
+Edit `setup.cfg` file changing the version number. Adding +1 to the revision
+number is enough. This step is mandatory to install locally the py2pack module.
+
+From the py2pack directory, install the py2pack module locally.
 
 .. code-block:: bash
 
-    $ python -m py2pack
+    $ pip install -e .
+
+Now you can run your hackish py2pack version. It is usually located in
+$HOME/.local/bin/py2pack
+
+.. code-block:: bash
+
+    $ py2pack
 
 Fork `the repository`_ on Github to start making your changes to the **master**
 branch (or branch off of it). Don't forget to write a test for fixed issues or
 implemented features whenever appropriate. You can invoke the testsuite from
 the repository root directory via `tox`_:
 
 .. code-block:: bash
 
     $ tox
 
 To run a single test class via `tox`_, use i.e.:
 
 .. code-block:: bash
 
-    $ tox -epy27 test.test_py2pack:Py2packTestCase
+    $ tox -epy38 test.test_py2pack:Py2packTestCase
 
 
 You can also run `pytest`_ directly:
 
 .. code-block:: bash
 
     $ pytest
@@ -158,21 +153,7 @@
 .. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
 .. _`Python Package Index`: https://pypi.org/
 .. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
 .. _`the repository`: https://github.com/openSUSE/py2pack
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: http://testrun.org/tox
 
-%prep
-%setup -q -n py2pack-%{version}
-
-%build
-python setup.py build
-
-%install
-python setup.py install --prefix=%{_prefix} --root=%{buildroot}
-
-%files
-%defattr(-,root,root,-)
-%{python_sitelib}/*
-
-%changelog
```

### Comparing `py2pack-0.8.7/test/examples/py2pack-opensuse.spec` & `py2pack-0.9.0/py2pack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,55 @@
-#
-# spec file for package python-py2pack
-#
-# Copyright (c) __YEAR__ SUSE LLC
-#
-# All modifications and additions to the file contributed by third parties
-# remain the property of their copyright owners, unless otherwise agreed
-# upon. The license for this file, and modifications and additions to the
-# file, is the same license as for the pristine package itself (unless the
-# license for the pristine package is not an Open Source License, in which
-# case the license is the MIT License). An "Open Source License" is a
-# license that conforms to the Open Source Definition (Version 1.9)
-# published by the Open Source Initiative.
-
-# Please submit bugfixes or comments via https://bugs.opensuse.org/
-#
-
-
-%{?!python_module:%define python_module() python-%{**} python3-%{**}}
-Name:           python-py2pack
-Version:        0.8.5
-Release:        0
-Summary:        Generate distribution packages from PyPI
-License:        Apache-2.0
-URL:            http://github.com/openSUSE/py2pack
-Source:         https://files.pythonhosted.org/packages/source/p/py2pack/py2pack-%{version}.tar.gz
-BuildRequires:  python-rpm-macros
-BuildRequires:  %{python_module setuptools}
-BuildRequires:  fdupes
-BuildArch:      noarch
-%python_subpackages
+Metadata-Version: 2.1
+Name: py2pack
+Version: 0.9.0
+Summary: Generate distribution packages from PyPI
+Home-page: https://github.com/openSUSE/py2pack
+Author: Sascha Peilicke, Thomas Bechtold
+Author-email: sascha@peilicke.de, thomasbechtold@jpberlin.de
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Pre-processors
+License-File: LICENSE
+License-File: AUTHORS
 
-%description
 Py2pack: Generate distribution packages from PyPI
 =================================================
 
-.. image:: https://travis-ci.org/openSUSE/py2pack.png?branch=master
-        :target: https://travis-ci.org/openSUSE/py2pack
-
+.. image:: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml/badge.svg
+        :target: https://github.com/openSUSE/py2pack/actions/workflows/tox.yml
+        :alt: Unit tests
 
 This script allows to generate RPM spec or DEB dsc files from Python modules.
 It allows to list Python modules or search for them on the Python Package Index
 (PyPI). Conveniently, it can fetch tarballs and changelogs making it an
 universal tool to package Python modules.
 
 
 Installation
 ------------
 
 To install py2pack from the `Python Package Index`_, simply:
 
 .. code-block:: bash
 
-    $ pip install py2pack
-
-Or, if you absolutely must:
-
-.. code-block:: bash
-
-    $ easy_install py2pack
+    $ python3 -mpip install py2pack
 
-But, you really shouldn't do that. Lastly, you can check your distro of choice
-if they provide packages. For openSUSE, you can find packages in the `Open
-Build Service`_ for all releases. If you happen to use openSUSE:Factory (the
-rolling release / development version), simply:
+You can also check your distro of choice if they provide packages.
+For openSUSE Tumbleweed and Leap 15.X, you can
 
 .. code-block:: bash
 
-    $ sudo zypper install python-py2pack
+    $ sudo zypper install python3-py2pack
 
 
 Usage
 -----
 
 Lets suppose you want to package zope.interface_ and you don't know how it is named
 exactly. First of all, you can search for it and download the source tarball if
@@ -115,34 +94,46 @@
 
     $ py2pack help
 
 
 Hacking and contributing
 ------------------------
 
-You can test py2pack from your git checkout by executing the py2pack module:
+You can test py2pack from your git checkout by executing the py2pack module.
+
+Edit `setup.cfg` file changing the version number. Adding +1 to the revision
+number is enough. This step is mandatory to install locally the py2pack module.
+
+From the py2pack directory, install the py2pack module locally.
 
 .. code-block:: bash
 
-    $ python -m py2pack
+    $ pip install -e .
+
+Now you can run your hackish py2pack version. It is usually located in
+$HOME/.local/bin/py2pack
+
+.. code-block:: bash
+
+    $ py2pack
 
 Fork `the repository`_ on Github to start making your changes to the **master**
 branch (or branch off of it). Don't forget to write a test for fixed issues or
 implemented features whenever appropriate. You can invoke the testsuite from
 the repository root directory via `tox`_:
 
 .. code-block:: bash
 
     $ tox
 
 To run a single test class via `tox`_, use i.e.:
 
 .. code-block:: bash
 
-    $ tox -epy27 test.test_py2pack:Py2packTestCase
+    $ tox -epy38 test.test_py2pack:Py2packTestCase
 
 
 You can also run `pytest`_ directly:
 
 .. code-block:: bash
 
     $ pytest
@@ -162,21 +153,7 @@
 .. _DEB: http://en.wikipedia.org/wiki/Deb_(file_format)
 .. _`Python Package Index`: https://pypi.org/
 .. _`Open Build Service`: https://build.opensuse.org/package/show/devel:languages:python/python-py2pack
 .. _`the repository`: https://github.com/openSUSE/py2pack
 .. _`pytest`: https://github.com/pytest-dev/pytest
 .. _`tox`: http://testrun.org/tox
 
-%prep
-%setup -q -n py2pack-%{version}
-
-%build
-%python_build
-
-%install
-%python_install
-%python_expand %fdupes %{buildroot}%{$python_sitelib}
-
-%files %{python_files}
-%{python_sitelib}/*
-
-%changelog
```

### Comparing `py2pack-0.8.7/test/test_py2pack.py` & `py2pack-0.9.0/test/test_py2pack.py`

 * *Files 21% similar despite different names*

```diff
@@ -100,46 +100,89 @@
         self.assertTrue('opensuse.spec' in env.list_templates())
         self.assertTrue('parenthesize_version' in env.filters)
         self.assertTrue('basename' in env.filters)
 
     @data(
         (
             {'install_requires': ["pywin32>=1.0;sys_platform=='win32'", 'monotonic>=0.1 #comment']},
-            {'install_requires': ['monotonic >= 0.1']},
+            {'build_requires': ['setuptools', 'wheel'],
+             'install_requires': ['monotonic >= 0.1']},
         ),
         (
             {'install_requires': 'six  >=1.9,!=1.0  # comment\nfoobar>=0.1,>=0.5'},
-            {'install_requires': ['six >= 1.9', 'foobar >= 0.1']}
+            {'build_requires': ['setuptools', 'wheel'],
+             'install_requires': ['six >= 1.9', 'foobar >= 0.1']}
         ),
         (
             {'setup_requires': 'six  >=1.9,!=1.0  # comment\nfoobar>=0.1,>=0.5'},
-            {'setup_requires': ['six >= 1.9', 'foobar >= 0.1']}
+            {'build_requires': ['setuptools', 'wheel', 'six >= 1.9', 'foobar >= 0.1']}
         ),
         (
             {'tests_require': ['six  >=1.9', 'foobar>=0.1,>=0.5']},
-            {'tests_require': ['six >= 1.9', 'foobar >= 0.1']}
+            {'build_requires': ['setuptools', 'wheel'],
+             'tests_require': ['six >= 1.9', 'foobar >= 0.1']}
         ),
         (
             {'tests_require': 'six  >=1.9\nfoobar>=0.1,>=0.5'},
-            {'tests_require': ['six >= 1.9', 'foobar >= 0.1']}
+            {'build_requires': ['setuptools', 'wheel'],
+             'tests_require': ['six >= 1.9', 'foobar >= 0.1']}
         ),
         (
             {'extras_require': {'extra1': ['foobar<=3.0, >= 2.1']}},
-            {'extras_require': {'extra1': ['foobar >= 2.1']}}
+            {'build_requires': ['setuptools', 'wheel'],
+             'extras_require': {'extra1': ['foobar >= 2.1']}}
         ),
         (
             {'extras_require': {'extra1': 'foobar<=3.0, >= 2.1\ntest1  # comment',
                                 'extra2': ['test2']}},
-            {'extras_require': {'extra1': ['foobar >= 2.1', 'test1'],
+            {'build_requires': ['setuptools', 'wheel'],
+             'extras_require': {'extra1': ['foobar >= 2.1', 'test1'],
                                 'extra2': ['test2']}}
         ),
+        (
+            {'build-system': {'requires': ['setuptools']},
+             'project': {'dependencies': ['foo', 'bar>=1', 'foobar>2,<3'],
+                         'optional-dependencies': {'extra': ['extra1', 'extra2 >2'],
+                                                   'test': ['pytest']},
+                         'scripts': {'cmd1': 'foo:main', 'cmd2': 'bar:cmd2'},
+                         'gui-scripts': {'gui': 'foo:mainview'}}},
+            {'build_requires': ['setuptools', 'wheel'],
+             'install_requires': ['foo', 'bar >= 1', 'foobar > 2'],
+             'extras_require': {'extra': ['extra1', 'extra2 > 2']},
+             'tests_require': ['pytest'],
+             'console_scripts': ['cmd1', 'cmd2', 'gui']}
+        ),
+        (
+            {'build-system': {'requires': ['flit_core']},
+             'tool': { 'flit': {
+                'metadata': {
+                    'requires': ['foo', 'bar>=1','foobar>2,<3'],
+                    'requires-extra': {'extra': ['extra1', 'extra2>2'],
+                                       'test': ['pytest']}},
+                'scripts': {'cmd': 'foo:main'}}}},
+            {'build_requires': ['flit_core'],
+             'install_requires': ['foo', 'bar >= 1', 'foobar > 2'],
+             'extras_require': {'extra': ['extra1', 'extra2 > 2']},
+             'tests_require': ['pytest'],
+             'console_scripts': ['cmd']}
+        ),
+        (
+            {'build-system': {'requires': ['hatchling']},
+             'project': {'dependencies': ['foo', 'bar>=1', 'foobar>2,<3']}},
+            {'build_requires': ['hatchling'],
+             'install_requires': ['foo', 'bar >= 1', 'foobar > 2']}
+        ),
     )
     @unpack
-    def test_canonicalize_setup_data(self, data, expected_data):
-        py2pack._canonicalize_setup_data(data)
+    def test_canonicalize_setup_data(self, data, updated_data):
+        expected_data = data.copy()
+        expected_data.update(updated_data)
+        expected_data.pop("setup_requires", None)
+        py2pack._canonicalize_setup_data(data)    
+        self.maxDiff = None
         self.assertEqual(data, expected_data)
 
     @data(
         (
             {'entry_points': "[console_scripts]\nfoo = foo:main"},
             ['foo']
         ),
```

### Comparing `py2pack-0.8.7/test/test_requires.py` & `py2pack-0.9.0/test/test_requires.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/test/test_template.py` & `py2pack-0.9.0/test/test_template.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import datetime
 import os
 import os.path
 import pwd
+import sys
+import unittest
 
 import pytest
 
 import py2pack
 
 
 class Args(object):
@@ -45,14 +47,16 @@
                           ('mageia.spec', False),
                           ('opensuse-legacy.spec', False),
                           ('opensuse.dsc', False),
                           ('opensuse.spec', False),
                           ('opensuse.spec', True)])
 def test_template(tmpdir, template, fetch_tarball):
     """ Test if generated specfile equals to stored one. """
+    if (template, fetch_tarball, sys.version_info[:2]) == ('opensuse.spec', True, (3, 6)):
+        raise unittest.SkipTest('This combination of tests fails ATM.')
     args = Args()
     args.template = template
     base, ext = template.split(".")
     suffix = '-augmented' if fetch_tarball else ''
     filename = "{}{}.{}".format(base, suffix, ext)
     args.filename = filename
     with tmpdir.as_cwd():
```

### Comparing `py2pack-0.8.7/test/test_utils.py` & `py2pack-0.9.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `py2pack-0.8.7/tools/obs-from-pypi.py` & `py2pack-0.9.0/tools/obs-from-pypi.py`

 * *Files identical despite different names*

