# Comparing `tmp/emmet-api-0.55.1.tar.gz` & `tmp/emmet-api-0.55.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.55.1.tar", last modified: Mon May 15 19:45:40 2023, max compression
+gzip compressed data, was "emmet-api-0.55.2.tar", last modified: Tue May 16 21:41:50 2023, max compression
```

## Comparing `emmet-api-0.55.1.tar` & `emmet-api-0.55.2.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.676993 emmet-api-0.55.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-15 19:45:35.000000 emmet-api-0.55.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 19:45:40.676993 emmet-api-0.55.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 19:45:35.000000 emmet-api-0.55.1/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.648993 emmet-api-0.55.1/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.656993 emmet-api-0.55.1/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.660993 emmet-api-0.55.1/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-15 19:45:35.000000 emmet-api-0.55.1/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.664993 emmet-api-0.55.1/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 19:45:40.000000 emmet-api-0.55.1/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 19:45:35.000000 emmet-api-0.55.1/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-15 19:45:35.000000 emmet-api-0.55.1/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-15 19:45:35.000000 emmet-api-0.55.1/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-15 19:45:35.000000 emmet-api-0.55.1/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:45:40.676993 emmet-api-0.55.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-15 19:45:35.000000 emmet-api-0.55.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 19:45:35.000000 emmet-api-0.55.1/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.648993 emmet-api-0.55.1/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.652993 emmet-api-0.55.1/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.668993 emmet-api-0.55.1/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.672993 emmet-api-0.55.1/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.676993 emmet-api-0.55.1/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.676993 emmet-api-0.55.1/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:40.676993 emmet-api-0.55.1/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 19:45:35.000000 emmet-api-0.55.1/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-16 21:41:40.000000 emmet-api-0.55.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 21:41:50.237911 emmet-api-0.55.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 21:41:40.000000 emmet-api-0.55.2/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.205911 emmet-api-0.55.2/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-16 21:41:50.000000 emmet-api-0.55.2/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-16 21:41:40.000000 emmet-api-0.55.2/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-16 21:41:40.000000 emmet-api-0.55.2/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-16 21:41:40.000000 emmet-api-0.55.2/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:41:50.237911 emmet-api-0.55.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 21:41:40.000000 emmet-api-0.55.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 21:41:40.000000 emmet-api-0.55.2/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.209911 emmet-api-0.55.2/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.209911 emmet-api-0.55.2/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.55.1/Dockerfile` & `emmet-api-0.55.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/app.py` & `emmet-api-0.55.2/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/api.py` & `emmet-api-0.55.2/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.55.2/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.55.2/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/documentation.py` & `emmet-api-0.55.2/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/global_header.py` & `emmet-api-0.55.2/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/core/settings.py` & `emmet-api-0.55.2/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.55.2/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.55.2/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.55.2/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.55.2/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/dois/resources.py` & `emmet-api-0.55.2/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.55.2/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.55.2/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.55.2/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.55.2/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.55.2/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/utils.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.55.2/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/legacy_resources.py` & `emmet-api-0.55.2/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/material_resources.py` & `emmet-api-0.55.2/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/molecule_resources.py` & `emmet-api-0.55.2/molecule_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,85 +38,85 @@
     if len(db_uri.split("://", 1)) < 2:
         db_uri = "mongodb+srv://" + db_uri
 
     task_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="task_id",
-        collection_name="mpcules_tasks",
+        collection_name="molecules_tasks",
     )
 
     assoc_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="molecule_id",
-        collection_name="mpcules_assoc",
+        collection_name="molecules_assoc",
     )
 
     mol_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="molecule_id",
-        collection_name="mpcules_molecules",
+        collection_name="molecules_molecules",
     )
 
     charges_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_charges",
+        collection_name="molecules_charges",
     )
 
     spins_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_spins",
+        collection_name="molecules_spins",
     )
 
     bonds_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_bonds",
+        collection_name="molecules_bonds",
     )
 
     orbitals_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_orbitals",
+        collection_name="molecules_orbitals",
     )
 
     redox_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_redox",
+        collection_name="molecules_redox",
     )
 
     thermo_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_thermo",
+        collection_name="molecules_thermo",
     )
 
     vibes_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="property_id",
-        collection_name="mpcules_vibes",
+        collection_name="molecules_vibes",
     )
 
     summary_store = MongoURIStore(
         uri=db_uri,
         database="mp_molecules",
         key="molecule_id",
-        collection_name="mpcules_summary",
+        collection_name="molecules_summary",
     )
 
 else:
     raise RuntimeError("Must specify MongoDB URI containing inputs.")
 
 
 mp_molecules_resources = list()
```

### Comparing `emmet-api-0.55.1/requirements/deployment.txt` & `emmet-api-0.55.2/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.10.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.11.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.8.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.9.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.55.2/requirements/macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.55.2/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/setup.py` & `emmet-api-0.55.2/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/_consumer/test_query_operators.py` & `emmet-api-0.55.2/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/_general_store/test_query_operators.py` & `emmet-api-0.55.2/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/core/test_mapi.py` & `emmet-api-0.55.2/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.55.2/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/electrodes/test_utils.py` & `emmet-api-0.55.2/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/materials/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/materials/test_utils.py` & `emmet-api-0.55.2/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/summary/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.55.2/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.55.2/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/synthesis/test_utils.py` & `emmet-api-0.55.2/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/tasks/test_utils.py` & `emmet-api-0.55.2/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/materials/xas/test_query_operators.py` & `emmet-api-0.55.2/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.1/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.55.2/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

