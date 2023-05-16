# Comparing `tmp/artistools-2023.5.16.2.tar.gz` & `tmp/artistools-2023.5.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistools-2023.5.16.2.tar", last modified: Tue May 16 19:57:53 2023, max compression
+gzip compressed data, was "artistools-2023.5.16.3.tar", last modified: Tue May 16 20:40:06 2023, max compression
```

## Comparing `artistools-2023.5.16.2.tar` & `artistools-2023.5.16.3.tar`

### file list

```diff
@@ -1,387 +1,387 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.485103 artistools-2023.5.16.2/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.449103 artistools-2023.5.16.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.449103 artistools-2023.5.16.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.github/workflows/deploypypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.github/workflows/deploytestpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 19:57:53.485103 artistools-2023.5.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.425102 artistools-2023.5.16.2/artistools/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.425102 artistools-2023.5.16.2/artistools/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/atomic/_atomic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/codecomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.425102 artistools-2023.5.16.2/artistools/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/ElBiEn_2007.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/atomic_properties.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/betaminusdecays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/binding_energies.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.429103 artistools-2023.5.16.2/artistools/data/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/400.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/520.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.429103 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/ASIAGO/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/FUV.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/H.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/H_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/J.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/J_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/K.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/K_ab.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.429103 artistools-2023.5.16.2/artistools/data/filters/LCOGT/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LCOGT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.429103 artistools-2023.5.16.2/artistools/data/filters/LSQ/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LSQ/rs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.429103 artistools-2023.5.16.2/artistools/data/filters/LT/
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/LT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.433102 artistools-2023.5.16.2/artistools/data/filters/NOT/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NOT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.433102 artistools-2023.5.16.2/artistools/data/filters/NTT/
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NTT/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/NUV.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.433102 artistools-2023.5.16.2/artistools/data/filters/OGLE/
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/OGLE/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/OGLE/V.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.433102 artistools-2023.5.16.2/artistools/data/filters/PS1/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/PS1/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/PS1/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/PS1/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/PS1/ws.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/PS1/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/R.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.433102 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvm2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvm2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvw1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvw1_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/uvw2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/filters/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.457103 artistools-2023.5.16.2/artistools/data/lightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN1991T.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN1999by.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN1999dq.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2005cf.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2011fe.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2012cg.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2012dn.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2012fr.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2014J.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2015F.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/SN2018byg.dat.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.457103 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.481103 artistools-2023.5.16.2/artistools/data/refspectra/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2010lp_20110928_fors2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/nero-nebspec.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/solar_r_abundance_pattern.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/data/splitmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.441103 artistools-2023.5.16.2/artistools/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19625 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/estimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/exportmassfractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/plot3destimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42569 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/estimators/plotestimators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25084 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/gsinetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/hesma_scripts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/initial_composition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.445103 artistools-2023.5.16.2/artistools/inputmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6390 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/1dslicefrom3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/botyanski2017.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5478 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/describeinputmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/downscale3dgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/energyinputfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.445103 artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10742 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/fullymixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    44349 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/inputmodel_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/lapuente.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/makeartismodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/maketardismodelfromartis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/map_1d_to_3d_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/maptogrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16453 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/modelfromhydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/opacityinputfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/plotdensity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/recombinationenergy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24896 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/rprocess_from_trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/rprocess_solar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/scalevelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/shen2018.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/slice1Dfromconein3dmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/inputmodel/test_inputmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.445103 artistools-2023.5.16.2/artistools/lightcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    64689 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/plotlightcurve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    31958 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/viewingangleanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/lightcurve/writebollightcurvedata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36660 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/linefluxes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4936 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/logfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5822 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/macroatom.py
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)    48179 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.445103 artistools-2023.5.16.2/artistools/nltepops/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nltepops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nltepops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nltepops/nltepops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33086 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nltepops/plotnltepops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.445103 artistools-2023.5.16.2/artistools/nonthermal/
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58909 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/_nonthermal_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/leptontransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11706 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/plotnonthermal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14234 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/nonthermal/solvespencerfanocmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.449103 artistools-2023.5.16.2/artistools/packets/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32364 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/packets/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/packets/packetsplots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13422 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/plotspherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/plottools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42385 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/radfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.449103 artistools-2023.5.16.2/artistools/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51706 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/plotspectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/sampleblackbodyfrompacketTR.py
--rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/test_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/spectra/test_vspectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4325 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/test_artistools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20279 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6887 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/viewing_angles_visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistools/writecomparisondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.449103 artistools-2023.5.16.2/artistools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 19:57:53.000000 artistools-2023.5.16.2/artistools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/artistoolscompletions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.481103 artistools-2023.5.16.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-emission.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-emission.png
--rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-estimators.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-estimators.png
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-nlte-Ni.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/images/fig-nlte-Ni.png
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 19:57:53.485103 artistools-2023.5.16.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.481103 artistools-2023.5.16.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.481103 artistools-2023.5.16.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/data/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/data/setuptestdata.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.485103 artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    76456 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/abundances.txt.xz
--rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/model.txt.xz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:57:53.485103 artistools-2023.5.16.2/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/output/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-05-16 19:56:47.000000 artistools-2023.5.16.2/tests/plottransitions_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/deploypypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/deploytestpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.landscape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/atomic/_atomic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/codecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/ElBiEn_2007.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/atomic_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/betaminusdecays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/binding_energies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/400.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/520.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/FUV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/H_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/J.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/J_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/K_ab.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/LCOGT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/LSQ/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LSQ/rs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/LT/
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/NOT/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/NTT/
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NUV.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/OGLE/
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/OGLE/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/OGLE/V.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/PS1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/ws.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/R.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvm2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvm2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw1_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.650305 artistools-2023.5.16.3/artistools/data/lightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1991T.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1999by.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1999dq.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2005cf.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2011fe.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012cg.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012dn.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012fr.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2014J.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2015F.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2018byg.dat.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.650305 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.670305 artistools-2023.5.16.3/artistools/data/refspectra/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/nero-nebspec.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/solar_r_abundance_pattern.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/splitmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/deposition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19625 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/estimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/exportmassfractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/plot3destimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42569 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/plotestimators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25084 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/gsinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/hesma_scripts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/initial_composition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/inputmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6390 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/1dslicefrom3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/botyanski2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5478 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/describeinputmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/downscale3dgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/energyinputfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10742 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fullymixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44529 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/inputmodel_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/lapuente.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/makeartismodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/maketardismodelfromartis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/map_1d_to_3d_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/maptogrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16453 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/modelfromhydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/opacityinputfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/plotdensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/recombinationenergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24896 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/rprocess_from_trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/rprocess_solar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/scalevelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/shen2018.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/slice1Dfromconein3dmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/test_inputmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/lightcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64689 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/plotlightcurve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31958 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/viewingangleanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/writebollightcurvedata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36660 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/linefluxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4936 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/logfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5822 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/macroatom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)    48179 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/nltepops/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/nltepops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33086 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/plotnltepops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/nonthermal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58909 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/_nonthermal_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/leptontransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11706 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/plotnonthermal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14234 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/solvespencerfanocmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/packets/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32364 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/packetsplots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13422 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/plotspherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/plottools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42385 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/radfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51706 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/plotspectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/sampleblackbodyfrompacketTR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/test_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/test_vspectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4325 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/test_artistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20279 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6887 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/viewing_angles_visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/writecomparisondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.646304 artistools-2023.5.16.3/artistools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistoolscompletions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-emission.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-emission.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-estimators.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-estimators.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-nlte-Ni.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-nlte-Ni.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/setuptestdata.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    76456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/abundances.txt.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/model.txt.xz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/output/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/plottransitions_example.sh
```

### Comparing `artistools-2023.5.16.2/.codecov.yml` & `artistools-2023.5.16.3/.codecov.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.github/workflows/deploypypi.yml` & `artistools-2023.5.16.3/.github/workflows/deploypypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.github/workflows/deploytestpypi.yml` & `artistools-2023.5.16.3/.github/workflows/deploytestpypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.github/workflows/linter.yml` & `artistools-2023.5.16.3/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.github/workflows/pytest.yml` & `artistools-2023.5.16.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.gitignore` & `artistools-2023.5.16.3/.gitignore`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/.pre-commit-config.yaml` & `artistools-2023.5.16.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/CODEOWNERS` & `artistools-2023.5.16.3/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/LICENSE.txt` & `artistools-2023.5.16.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/PKG-INFO` & `artistools-2023.5.16.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2023.5.16.2
+Version: 2023.5.16.3
 Summary: Plotting and analysis tools for the ARTIS 3D supernova radiative transfer code.
 Home-page: https://www.github.com/artis-mcrt/artistools/
 Author: ARTIS Collaboration
 Author-email: ARTIS Collaboration <luke.shingles@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `artistools-2023.5.16.2/README.md` & `artistools-2023.5.16.3/README.md`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/__init__.py` & `artistools-2023.5.16.3/artistools/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/__main__.py` & `artistools-2023.5.16.3/artistools/__main__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/atomic/_atomic_core.py` & `artistools-2023.5.16.3/artistools/atomic/_atomic_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/codecomparison.py` & `artistools-2023.5.16.3/artistools/codecomparison.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/commands.py` & `artistools-2023.5.16.3/artistools/commands.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/configuration.py` & `artistools-2023.5.16.3/artistools/configuration.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/ElBiEn_2007.txt` & `artistools-2023.5.16.3/artistools/data/ElBiEn_2007.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/atomic_properties.txt` & `artistools-2023.5.16.3/artistools/data/atomic_properties.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/betaminusdecays.txt` & `artistools-2023.5.16.3/artistools/data/betaminusdecays.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/binding_energies.txt` & `artistools-2023.5.16.3/artistools/data/binding_energies.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/collion-AR1985.txt` & `artistools-2023.5.16.3/artistools/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/collion-reference.txt` & `artistools-2023.5.16.3/artistools/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/collion.txt` & `artistools-2023.5.16.3/artistools/data/collion.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/elements.csv` & `artistools-2023.5.16.3/artistools/data/elements.csv`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/400.txt` & `artistools-2023.5.16.3/artistools/data/filters/400.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/520.txt` & `artistools-2023.5.16.3/artistools/data/filters/520.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/B.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/U.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/ASIAGO/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/B.txt` & `artistools-2023.5.16.3/artistools/data/filters/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/FUV.txt` & `artistools-2023.5.16.3/artistools/data/filters/FUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/H.txt` & `artistools-2023.5.16.3/artistools/data/filters/H.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/H_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/H_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/I.txt` & `artistools-2023.5.16.3/artistools/data/filters/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/J.txt` & `artistools-2023.5.16.3/artistools/data/filters/J.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/J_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/J_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/K.txt` & `artistools-2023.5.16.3/artistools/data/filters/K.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/K_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/K_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/B.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/I.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/R.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/U.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/us.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LCOGT/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LCOGT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LSQ/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LSQ/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LT/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LT/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/LT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LT/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LT/us.txt` & `artistools-2023.5.16.3/artistools/data/filters/LT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/LT/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/LT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/B.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/I.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/R.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/U.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/us.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NOT/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NOT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/B.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/I.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/R.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/U.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NTT/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/NTT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/NUV.txt` & `artistools-2023.5.16.3/artistools/data/filters/NUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/OGLE/I.txt` & `artistools-2023.5.16.3/artistools/data/filters/OGLE/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/OGLE/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/OGLE/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/PS1/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/PS1/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/PS1/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/PS1/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/PS1/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/PS1/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/PS1/ws.txt` & `artistools-2023.5.16.3/artistools/data/filters/PS1/ws.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/PS1/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/PS1/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/R.txt` & `artistools-2023.5.16.3/artistools/data/filters/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/us.txt` & `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/SKYMAPPER/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/U.txt` & `artistools-2023.5.16.3/artistools/data/filters/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/V.txt` & `artistools-2023.5.16.3/artistools/data/filters/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/gs.txt` & `artistools-2023.5.16.3/artistools/data/filters/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/is.txt` & `artistools-2023.5.16.3/artistools/data/filters/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/rs.txt` & `artistools-2023.5.16.3/artistools/data/filters/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/us.txt` & `artistools-2023.5.16.3/artistools/data/filters/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvm2.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvm2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvm2_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvm2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvw1.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvw1.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvw1_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvw1_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvw2.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvw2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/uvw2_ab.txt` & `artistools-2023.5.16.3/artistools/data/filters/uvw2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/filters/zs.txt` & `artistools-2023.5.16.3/artistools/data/filters/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt` & `artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt` & `artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2010lp_20110928_fors2.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii` & `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz` & `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt` & `artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/data/solar_r_abundance_pattern.txt` & `artistools-2023.5.16.3/artistools/data/solar_r_abundance_pattern.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/deposition.py` & `artistools-2023.5.16.3/artistools/deposition.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/__init__.py` & `artistools-2023.5.16.3/artistools/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/estimators.py` & `artistools-2023.5.16.3/artistools/estimators/estimators.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/estimators_classic.py` & `artistools-2023.5.16.3/artistools/estimators/estimators_classic.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/exportmassfractions.py` & `artistools-2023.5.16.3/artistools/estimators/exportmassfractions.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/plot3destimators_classic.py` & `artistools-2023.5.16.3/artistools/estimators/plot3destimators_classic.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/estimators/plotestimators.py` & `artistools-2023.5.16.3/artistools/estimators/plotestimators.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/gsinetwork.py` & `artistools-2023.5.16.3/artistools/gsinetwork.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/hesma_scripts.py` & `artistools-2023.5.16.3/artistools/hesma_scripts.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/initial_composition.py` & `artistools-2023.5.16.3/artistools/initial_composition.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/1dslicefrom3d.py` & `artistools-2023.5.16.3/artistools/inputmodel/1dslicefrom3d.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/__init__.py` & `artistools-2023.5.16.3/artistools/inputmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/botyanski2017.py` & `artistools-2023.5.16.3/artistools/inputmodel/botyanski2017.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/describeinputmodel.py` & `artistools-2023.5.16.3/artistools/inputmodel/describeinputmodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/downscale3dgrid.py` & `artistools-2023.5.16.3/artistools/inputmodel/downscale3dgrid.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/energyinputfiles.py` & `artistools-2023.5.16.3/artistools/inputmodel/energyinputfiles.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py` & `artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py` & `artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/rd_cmfgen.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/fullymixed.py` & `artistools-2023.5.16.3/artistools/inputmodel/fullymixed.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/inputmodel_misc.py` & `artistools-2023.5.16.3/artistools/inputmodel/inputmodel_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,22 @@
                     "X_Fe52",
                     "X_Cr48",
                     "X_Ni57",
                     "X_Co57",
                 ]
             # last two abundances are optional
             assert columns is not None
-            assert len(columns) == (ncols_line_even + ncols_line_odd) or len(columns) == (
-                ncols_line_even + ncols_line_odd + 2
-            )
+            if ncols_line_even == ncols_line_odd and (ncols_line_even + ncols_line_odd) > len(columns):
+                # one line per cell format
+                ncols_line_odd = 0
+
+            assert len(columns) in [
+                ncols_line_even + ncols_line_odd,
+                ncols_line_even + ncols_line_odd + 2,
+            ]
             columns = columns[: ncols_line_even + ncols_line_odd]
 
         assert columns is not None
         if ncols_line_even == len(columns):
             if not printwarningsonly:
                 print("  model file is one line per cell")
             ncols_line_odd = 0
```

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/lapuente.py` & `artistools-2023.5.16.3/artistools/inputmodel/lapuente.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/makeartismodel.py` & `artistools-2023.5.16.3/artistools/inputmodel/makeartismodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/maketardismodelfromartis.py` & `artistools-2023.5.16.3/artistools/inputmodel/maketardismodelfromartis.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/map_1d_to_3d_grid.py` & `artistools-2023.5.16.3/artistools/inputmodel/map_1d_to_3d_grid.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/maptogrid.py` & `artistools-2023.5.16.3/artistools/inputmodel/maptogrid.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/modelfromhydro.py` & `artistools-2023.5.16.3/artistools/inputmodel/modelfromhydro.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/opacityinputfile.py` & `artistools-2023.5.16.3/artistools/inputmodel/opacityinputfile.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/plotdensity.py` & `artistools-2023.5.16.3/artistools/inputmodel/plotdensity.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/recombinationenergy.py` & `artistools-2023.5.16.3/artistools/inputmodel/recombinationenergy.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/rprocess_from_trajectory.py` & `artistools-2023.5.16.3/artistools/inputmodel/rprocess_from_trajectory.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/rprocess_solar.py` & `artistools-2023.5.16.3/artistools/inputmodel/rprocess_solar.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/scalevelocity.py` & `artistools-2023.5.16.3/artistools/inputmodel/scalevelocity.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/shen2018.py` & `artistools-2023.5.16.3/artistools/inputmodel/shen2018.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/slice1Dfromconein3dmodel.py` & `artistools-2023.5.16.3/artistools/inputmodel/slice1Dfromconein3dmodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/inputmodel/test_inputmodel.py` & `artistools-2023.5.16.3/artistools/inputmodel/test_inputmodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/__init__.py` & `artistools-2023.5.16.3/artistools/lightcurve/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/lightcurve.py` & `artistools-2023.5.16.3/artistools/lightcurve/lightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/plotlightcurve.py` & `artistools-2023.5.16.3/artistools/lightcurve/plotlightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/test_lightcurve.py` & `artistools-2023.5.16.3/artistools/lightcurve/test_lightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/viewingangleanalysis.py` & `artistools-2023.5.16.3/artistools/lightcurve/viewingangleanalysis.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/lightcurve/writebollightcurvedata.py` & `artistools-2023.5.16.3/artistools/lightcurve/writebollightcurvedata.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/linefluxes.py` & `artistools-2023.5.16.3/artistools/linefluxes.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/logfiles.py` & `artistools-2023.5.16.3/artistools/logfiles.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/macroatom.py` & `artistools-2023.5.16.3/artistools/macroatom.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/matplotlibrc` & `artistools-2023.5.16.3/artistools/matplotlibrc`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/misc.py` & `artistools-2023.5.16.3/artistools/misc.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nltepops/nltepops.py` & `artistools-2023.5.16.3/artistools/nltepops/nltepops.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nltepops/plotnltepops.py` & `artistools-2023.5.16.3/artistools/nltepops/plotnltepops.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nonthermal/__init__.py` & `artistools-2023.5.16.3/artistools/nonthermal/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nonthermal/_nonthermal_core.py` & `artistools-2023.5.16.3/artistools/nonthermal/_nonthermal_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nonthermal/leptontransport.py` & `artistools-2023.5.16.3/artistools/nonthermal/leptontransport.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nonthermal/plotnonthermal.py` & `artistools-2023.5.16.3/artistools/nonthermal/plotnonthermal.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/nonthermal/solvespencerfanocmd.py` & `artistools-2023.5.16.3/artistools/nonthermal/solvespencerfanocmd.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/packets/__init__.py` & `artistools-2023.5.16.3/artistools/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/packets/packets.py` & `artistools-2023.5.16.3/artistools/packets/packets.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/packets/packetsplots.py` & `artistools-2023.5.16.3/artistools/packets/packetsplots.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/plotspherical.py` & `artistools-2023.5.16.3/artistools/plotspherical.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/plottools.py` & `artistools-2023.5.16.3/artistools/plottools.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/radfield.py` & `artistools-2023.5.16.3/artistools/radfield.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/__init__.py` & `artistools-2023.5.16.3/artistools/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/plotspectra.py` & `artistools-2023.5.16.3/artistools/spectra/plotspectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/sampleblackbodyfrompacketTR.py` & `artistools-2023.5.16.3/artistools/spectra/sampleblackbodyfrompacketTR.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/spectra.py` & `artistools-2023.5.16.3/artistools/spectra/spectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/test_spectra.py` & `artistools-2023.5.16.3/artistools/spectra/test_spectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/spectra/test_vspectra.py` & `artistools-2023.5.16.3/artistools/spectra/test_vspectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/stats.py` & `artistools-2023.5.16.3/artistools/stats.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/test_artistools.py` & `artistools-2023.5.16.3/artistools/test_artistools.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/transitions.py` & `artistools-2023.5.16.3/artistools/transitions.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/viewing_angles_visualization.py` & `artistools-2023.5.16.3/artistools/viewing_angles_visualization.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools/writecomparisondata.py` & `artistools-2023.5.16.3/artistools/writecomparisondata.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools.egg-info/PKG-INFO` & `artistools-2023.5.16.3/artistools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2023.5.16.2
+Version: 2023.5.16.3
 Summary: Plotting and analysis tools for the ARTIS 3D supernova radiative transfer code.
 Home-page: https://www.github.com/artis-mcrt/artistools/
 Author: ARTIS Collaboration
 Author-email: ARTIS Collaboration <luke.shingles@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `artistools-2023.5.16.2/artistools.egg-info/SOURCES.txt` & `artistools-2023.5.16.3/artistools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistools.egg-info/entry_points.txt` & `artistools-2023.5.16.3/artistools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/artistoolscompletions.sh` & `artistools-2023.5.16.3/artistoolscompletions.sh`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-emission.pdf` & `artistools-2023.5.16.3/images/fig-emission.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-emission.png` & `artistools-2023.5.16.3/images/fig-emission.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-estimators.pdf` & `artistools-2023.5.16.3/images/fig-estimators.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-estimators.png` & `artistools-2023.5.16.3/images/fig-estimators.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-nlte-Ni.pdf` & `artistools-2023.5.16.3/images/fig-nlte-Ni.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/images/fig-nlte-Ni.png` & `artistools-2023.5.16.3/images/fig-nlte-Ni.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/pyproject.toml` & `artistools-2023.5.16.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/setup.py` & `artistools-2023.5.16.3/setup.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/abundances.txt.xz` & `artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/abundances.txt.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.2/tests/data/testmodel_3d_10^3/model.txt.xz` & `artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/model.txt.xz`

 * *Files identical despite different names*

