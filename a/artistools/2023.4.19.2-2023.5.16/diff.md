# Comparing `tmp/artistools-2023.4.19.2.tar.gz` & `tmp/artistools-2023.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistools-2023.4.19.2.tar", last modified: Wed Apr 19 13:19:18 2023, max compression
+gzip compressed data, was "artistools-2023.5.16.tar", last modified: Tue May 16 13:13:43 2023, max compression
```

## Comparing `artistools-2023.4.19.2.tar` & `artistools-2023.5.16.tar`

### file list

```diff
@@ -1,383 +1,387 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.202411 artistools-2023.4.19.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.202411 artistools-2023.4.19.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.github/workflows/deploypypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.github/workflows/deploytestpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.162409 artistools-2023.4.19.2/artistools/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.162409 artistools-2023.4.19.2/artistools/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/atomic/_atomic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/codecomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.166409 artistools-2023.4.19.2/artistools/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/ElBiEn_2007.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/atomic_properties.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/betaminusdecays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/binding_energies.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.170409 artistools-2023.4.19.2/artistools/data/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/400.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/520.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.174409 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/ASIAGO/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/FUV.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/H.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/H_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/J.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/J_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/K.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/K_ab.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.174409 artistools-2023.4.19.2/artistools/data/filters/LCOGT/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LCOGT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.174409 artistools-2023.4.19.2/artistools/data/filters/LSQ/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LSQ/rs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.178409 artistools-2023.4.19.2/artistools/data/filters/LT/
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/LT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.178409 artistools-2023.4.19.2/artistools/data/filters/NOT/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NOT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.182410 artistools-2023.4.19.2/artistools/data/filters/NTT/
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NTT/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/NUV.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.182410 artistools-2023.4.19.2/artistools/data/filters/OGLE/
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/OGLE/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/OGLE/V.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.182410 artistools-2023.4.19.2/artistools/data/filters/PS1/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/PS1/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/PS1/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/PS1/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/PS1/ws.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/PS1/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/R.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.182410 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvm2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvm2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvw1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvw1_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/uvw2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/filters/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.214411 artistools-2023.4.19.2/artistools/data/lightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN1991T.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN1999by.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN1999dq.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2005cf.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2011fe.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2012cg.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2012dn.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2012fr.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2014J.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2015F.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/SN2018byg.dat.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.214411 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.242412 artistools-2023.4.19.2/artistools/data/refspectra/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2010lp_20110928_fors2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/nero-nebspec.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/solar_r_abundance_pattern.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/data/splitmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5389 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.190410 artistools-2023.4.19.2/artistools/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18917 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/estimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/exportmassfractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/plot3destimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42661 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/estimators/plotestimators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25083 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/gsinetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/hesma_scripts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14443 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/initial_composition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.194410 artistools-2023.4.19.2/artistools/inputmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6383 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/1dslicefrom3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/botyanski2017.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5470 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/describeinputmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/downscale3dgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/energyinputfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.194410 artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10757 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/fullymixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/inputmodel_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/lapuente.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3232 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/makeartismodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3975 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/maketardismodelfromartis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/map_1d_to_3d_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14485 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/maptogrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16451 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/modelfromhydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/opacityinputfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2799 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/plotdensity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/recombinationenergy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24801 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/rprocess_from_trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5532 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/rprocess_solar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2597 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/scalevelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3492 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/shen2018.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8395 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/slice1Dfromconein3dmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/inputmodel/test_inputmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.198410 artistools-2023.4.19.2/artistools/lightcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    64422 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/plotlightcurve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    31967 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/viewingangleanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/lightcurve/writebollightcurvedata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36580 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/linefluxes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5002 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/logfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5882 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/macroatom.py
--rw-r--r--   0 runner    (1001) docker     (123)    40230 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)    46889 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.198410 artistools-2023.4.19.2/artistools/nltepops/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nltepops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nltepops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nltepops/nltepops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33072 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nltepops/plotnltepops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.198410 artistools-2023.4.19.2/artistools/nonthermal/
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58909 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/_nonthermal_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/leptontransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11821 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/plotnonthermal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14258 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/nonthermal/solvespencerfanocmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.198410 artistools-2023.4.19.2/artistools/packets/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28527 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/packets/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/packets/packetsplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/plottools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42451 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/radfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.202411 artistools-2023.4.19.2/artistools/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51607 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/plotspectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/sampleblackbodyfrompacketTR.py
--rw-r--r--   0 runner    (1001) docker     (123)    54240 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4274 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/test_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/spectra/test_vspectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2452 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3305 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/test_artistools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20317 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7374 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/viewing_angles_visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10828 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistools/writecomparisondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.202411 artistools-2023.4.19.2/artistools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-19 13:19:17.000000 artistools-2023.4.19.2/artistools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-04-19 13:19:18.000000 artistools-2023.4.19.2/artistools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:19:17.000000 artistools-2023.4.19.2/artistools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-19 13:19:17.000000 artistools-2023.4.19.2/artistools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 13:19:17.000000 artistools-2023.4.19.2/artistools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-19 13:19:17.000000 artistools-2023.4.19.2/artistools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/artistoolscompletions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-emission.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-emission.png
--rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-estimators.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-estimators.png
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-nlte-Ni.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/images/fig-nlte-Ni.png
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/tests/data/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/tests/data/setuptestdata.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:18.250413 artistools-2023.4.19.2/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/tests/output/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-04-19 13:17:43.000000 artistools-2023.4.19.2/tests/plottransitions_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 13:12:34.000000 artistools-2023.5.16/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 13:12:34.000000 artistools-2023.5.16/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 13:12:34.000000 artistools-2023.5.16/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 13:12:34.000000 artistools-2023.5.16/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 13:12:34.000000 artistools-2023.5.16/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 13:12:34.000000 artistools-2023.5.16/.github/workflows/deploypypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-16 13:12:34.000000 artistools-2023.5.16/.github/workflows/deploytestpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 13:12:34.000000 artistools-2023.5.16/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 13:12:34.000000 artistools-2023.5.16/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-16 13:12:34.000000 artistools-2023.5.16/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 13:12:34.000000 artistools-2023.5.16/.landscape.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 13:12:34.000000 artistools-2023.5.16/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 13:12:34.000000 artistools-2023.5.16/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 13:12:34.000000 artistools-2023.5.16/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 13:12:34.000000 artistools-2023.5.16/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 13:12:34.000000 artistools-2023.5.16/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-16 13:13:43.271188 artistools-2023.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 13:12:34.000000 artistools-2023.5.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.223188 artistools-2023.5.16/artistools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.223188 artistools-2023.5.16/artistools/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/atomic/_atomic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/codecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.223188 artistools-2023.5.16/artistools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/ElBiEn_2007.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/atomic_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/betaminusdecays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/binding_energies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.227188 artistools-2023.5.16/artistools/data/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/400.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/520.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.227188 artistools-2023.5.16/artistools/data/filters/ASIAGO/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/ASIAGO/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/FUV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/H_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/J.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/J_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/K_ab.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.227188 artistools-2023.5.16/artistools/data/filters/LCOGT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LCOGT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.227188 artistools-2023.5.16/artistools/data/filters/LSQ/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LSQ/rs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/LT/
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/LT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/NOT/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NOT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/NTT/
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NTT/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/NUV.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/OGLE/
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/OGLE/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/OGLE/V.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/PS1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/PS1/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/PS1/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/PS1/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/PS1/ws.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/PS1/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/R.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.231188 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/SKYMAPPER/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvm2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvm2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvw1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvw1_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvw2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/uvw2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/filters/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.251188 artistools-2023.5.16/artistools/data/lightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN1991T.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN1999by.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN1999dq.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2005cf.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2011fe.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2012cg.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2012dn.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2012fr.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2014J.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2015F.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/SN2018byg.dat.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.251188 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.267188 artistools-2023.5.16/artistools/data/refspectra/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2010lp_20110928_fors2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/nero-nebspec.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/solar_r_abundance_pattern.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/data/splitmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/deposition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.235188 artistools-2023.5.16/artistools/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19625 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/estimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/exportmassfractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/plot3destimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42569 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/estimators/plotestimators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25084 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/gsinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/hesma_scripts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/initial_composition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.239188 artistools-2023.5.16/artistools/inputmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6390 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/1dslicefrom3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/botyanski2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5478 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/describeinputmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/downscale3dgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/energyinputfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.239188 artistools-2023.5.16/artistools/inputmodel/fromcmfgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/fromcmfgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10742 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/fullymixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44349 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/inputmodel_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/lapuente.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/makeartismodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/maketardismodelfromartis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/map_1d_to_3d_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/maptogrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16453 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/modelfromhydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/opacityinputfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/plotdensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/recombinationenergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24896 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/rprocess_from_trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/rprocess_solar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/scalevelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/shen2018.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/slice1Dfromconein3dmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/inputmodel/test_inputmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.239188 artistools-2023.5.16/artistools/lightcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64689 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/plotlightcurve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31958 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/viewingangleanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/lightcurve/writebollightcurvedata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36660 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/linefluxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4936 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/logfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5822 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/macroatom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)    48179 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.239188 artistools-2023.5.16/artistools/nltepops/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nltepops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nltepops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nltepops/nltepops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33086 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nltepops/plotnltepops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/artistools/nonthermal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58909 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/_nonthermal_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/leptontransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11706 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/plotnonthermal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14234 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/nonthermal/solvespencerfanocmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/artistools/packets/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32364 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/packets/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/packets/packetsplots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13422 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/plotspherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/plottools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42385 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/radfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/artistools/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51706 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/plotspectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/sampleblackbodyfrompacketTR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/test_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/spectra/test_vspectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4325 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/test_artistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20279 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6887 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/viewing_angles_visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistools/writecomparisondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.243188 artistools-2023.5.16/artistools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 13:13:43.000000 artistools-2023.5.16/artistools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 13:12:34.000000 artistools-2023.5.16/artistoolscompletions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-emission.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-emission.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-estimators.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-estimators.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-nlte-Ni.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-05-16 13:12:34.000000 artistools-2023.5.16/images/fig-nlte-Ni.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-16 13:12:34.000000 artistools-2023.5.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 13:12:34.000000 artistools-2023.5.16/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 13:13:43.271188 artistools-2023.5.16/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-05-16 13:12:34.000000 artistools-2023.5.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/data/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/data/setuptestdata.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/tests/data/testmodel_3d_10^3/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/data/testmodel_3d_10^3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    76456 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/data/testmodel_3d_10^3/abundances.txt.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/data/testmodel_3d_10^3/model.txt.xz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:13:43.271188 artistools-2023.5.16/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/output/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-05-16 13:12:34.000000 artistools-2023.5.16/tests/plottransitions_example.sh
```

### Comparing `artistools-2023.4.19.2/.codecov.yml` & `artistools-2023.5.16/.codecov.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/.github/workflows/deploypypi.yml` & `artistools-2023.5.16/.github/workflows/deploypypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/.github/workflows/deploytestpypi.yml` & `artistools-2023.5.16/.github/workflows/deploytestpypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/.github/workflows/linter.yml` & `artistools-2023.5.16/.github/workflows/linter.yml`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,14 @@
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v3
             - uses: psf/black@stable
               with:
                   options: --check --verbose
 
-    flake8:
-        runs-on: ubuntu-latest
-        steps:
-            - name: Checkout Code
-              uses: actions/checkout@v3
-
-            - name: Set up Python
-              uses: actions/setup-python@v4
-              with:
-                  cache: pip
-                  python-version-file: .python-version
-
-            - name: Install dependencies
-              run: |
-                  python3 -m pip install --upgrade pip wheel flake8
-                  # python3 -m pip install -r requirements.txt
-
-            - name: Lint with flake8
-              run: |
-                  # stop the build if there are Python syntax errors or undefined names
-                  flake8 . --count --show-source --statistics
-
     mypy:
         runs-on: ubuntu-latest
         steps:
             - name: Checkout Code
               uses: actions/checkout@v3
 
             - name: Set up Python
```

### Comparing `artistools-2023.4.19.2/.github/workflows/pytest.yml` & `artistools-2023.5.16/.github/workflows/pytest.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 on:
     push:
     merge_group:
 
 jobs:
     pytest:
+        timeout-minutes: 10
         runs-on: ${{ matrix.os }}
         strategy:
             matrix:
                 # os: [ubuntu-latest, macos-latest]
                 os: [ubuntu-latest]
                 python-version: ['3.9', '3.10', '3.11']
         env:
@@ -46,16 +47,18 @@
                   key: testdata20230417
 
             - name: Download/extract test data
               working-directory: tests/data/
               run: source ./setuptestdata.sh
 
             - name: Test with pytest
-              run: |
-                  pytest --cov=./ --cov-report=xml --durations=0
+              run: pytest --cov=./ --cov-report=xml --durations=0
+
+            - name: Report coverage
+              run: coverage report
 
             - name: Upload coverage to Codecov
               uses: codecov/codecov-action@v3
               with:
                   token: ${{ secrets.CODECOV_TOKEN }}
                   files: ./coverage.xml
                   # directory: ./coverage/reports/
```

### Comparing `artistools-2023.4.19.2/.gitignore` & `artistools-2023.5.16/.gitignore`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/.pre-commit-config.yaml` & `artistools-2023.5.16/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,26 @@
           - id: forbid-new-submodules
           - id: mixed-line-ending
             args: [--fix=lf]
           - id: name-tests-test
           - id: requirements-txt-fixer
           - id: trailing-whitespace
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
     - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.261
+      rev: v0.0.267
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
-    - repo: https://github.com/asottile/reorder_python_imports
-      rev: v3.9.0
-      hooks:
-          - id: reorder-python-imports
-            types: [python]
-            args: [--py39-plus, --exit-zero-even-if-changed]
     - repo: https://github.com/psf/black
       rev: 23.3.0
       hooks:
           - id: black
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.2.0
+      rev: v1.3.0
       hooks:
           - id: mypy
             additional_dependencies: [numpy, types-PyYAML, types-psutil]
             types: [python]
             require_serial: true
```

### Comparing `artistools-2023.4.19.2/CODEOWNERS` & `artistools-2023.5.16/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/LICENSE.txt` & `artistools-2023.5.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/PKG-INFO` & `artistools-2023.5.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2023.4.19.2
+Version: 2023.5.16
 Summary: Plotting and analysis tools for the ARTIS 3D supernova radiative transfer code.
 Home-page: https://www.github.com/artis-mcrt/artistools/
 Author: ARTIS Collaboration
 Author-email: ARTIS Collaboration <luke.shingles@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `artistools-2023.4.19.2/README.md` & `artistools-2023.5.16/README.md`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/__init__.py` & `artistools-2023.5.16/artistools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 import artistools.estimators
 import artistools.inputmodel
 import artistools.lightcurve
 import artistools.macroatom
 import artistools.nltepops
 import artistools.nonthermal
 import artistools.packets
+import artistools.plotspherical
 import artistools.radfield
 import artistools.spectra
 import artistools.transitions
+import artistools.writecomparisondata
+
 from .__main__ import addargs
 from .__main__ import main
 from .configuration import get_config
 from .configuration import set_config
 from .inputmodel import add_derived_cols_to_modeldata
 from .inputmodel import get_2d_modeldata
 from .inputmodel import get_cell_angle
@@ -39,32 +42,35 @@
 from .misc import firstexisting
 from .misc import flatten_list
 from .misc import get_atomic_number
 from .misc import get_bflist
 from .misc import get_cellsofmpirank
 from .misc import get_composition_data
 from .misc import get_composition_data_from_outputfile
+from .misc import get_costheta_bins
 from .misc import get_costhetabin_phibin_labels
 from .misc import get_deposition
 from .misc import get_dirbin_labels
 from .misc import get_elsymbol
 from .misc import get_elsymbolslist
 from .misc import get_escaped_arrivalrange
 from .misc import get_file_metadata
 from .misc import get_filterfunc
 from .misc import get_grid_mapping
 from .misc import get_inputparams
 from .misc import get_ionstring
 from .misc import get_linelist_dataframe
 from .misc import get_linelist_dict
+from .misc import get_linelist_pldf
 from .misc import get_model_name
 from .misc import get_mpiranklist
 from .misc import get_mpirankofcell
 from .misc import get_nprocs
 from .misc import get_nu_grid
+from .misc import get_phi_bins
 from .misc import get_runfolders
 from .misc import get_syn_dir
 from .misc import get_time_range
 from .misc import get_timestep_of_timedays
 from .misc import get_timestep_time
 from .misc import get_timestep_times_float
 from .misc import get_viewingdirection_costhetabincount
```

### Comparing `artistools-2023.4.19.2/artistools/__main__.py` & `artistools-2023.5.16/artistools/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import importlib
-import multiprocessing
+from typing import Optional
 
 import argcomplete
 
+from .commands import dictcommands as atdictcommands
+from .misc import CustomArgHelpFormatter
 
-def addargs(parser=None) -> None:
+
+def addargs(parser: argparse.ArgumentParser) -> None:
     pass
 
 
-dictcommands = {
-    "inputmodel": {
-        "describe": ("inputmodel.describeinputmodel", "main"),
-        "maptogrid": ("inputmodel.maptogrid", "main"),
-        "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
-        "makeartismodel": ("inputmodel.makeartismodel", "main"),
-    },
-    "estimators": {
-        "plot": ("estimators.plotestimators", "main"),
-    },
-    "lightcurves": {
-        "plot": ("lightcurve.plotlightcurve", "main"),
-    },
-    "spectra": {
-        "plot": ("spectra.plotspectra", "main"),
-    },
-    "comparetogsinetwork": ("gsinetwork", "main"),
-}
+def addsubparsers(parser, parentcommand, dictcommands, depth: int = 1) -> None:
+    def func(args) -> None:
+        parser.print_help()
 
+    parser.set_defaults(func=func)
+    subparsers = parser.add_subparsers(dest=f"{parentcommand} command", required=False)
 
-def addsubparsers(parser, parentcommand, dictcommands, depth: int = 1) -> None:
-    subparsers = parser.add_subparsers(dest=f"{parentcommand} command", required=True)
     for subcommand, subcommands in dictcommands.items():
-        subparser = subparsers.add_parser(subcommand, help=subcommand)
+        strhelp: Optional[str]
         if isinstance(subcommands, dict):
-            addsubparsers(subparser, subcommand, subcommands, depth=depth + 1)
+            strhelp = "command group"
+            submodule = None
         else:
             submodulename, funcname = subcommands
-            submodule = importlib.import_module(
-                f"artistools.{submodulename.removeprefix('artistools.')}", package="artistools"
-            )
+            namestr = f"artistools.{submodulename.removeprefix('artistools.')}" if submodulename else "artistools"
+            submodule = importlib.import_module(namestr, package="artistools")
+            func = getattr(submodule, funcname)
+            strhelp = func.__doc__
+
+        subparser = subparsers.add_parser(subcommand, help=strhelp, formatter_class=CustomArgHelpFormatter)
+
+        if submodule:
             submodule.addargs(subparser)
-            subparser.set_defaults(func=getattr(submodule, funcname))
+            subparser.set_defaults(func=func)
+        else:
+            addsubparsers(parser=subparser, parentcommand=subcommand, dictcommands=subcommands, depth=depth + 1)
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
     """Parse and run artistools commands."""
-
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(
+        formatter_class=CustomArgHelpFormatter,
+        description="Artistools base command.",
+    )
     parser.set_defaults(func=None)
 
-    addsubparsers(parser, "artistools", dictcommands)
+    addsubparsers(parser, "artistools", atdictcommands)
 
     argcomplete.autocomplete(parser)
     args = parser.parse_args(argsraw)
     args.func(args=args)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/atomic/_atomic_core.py` & `artistools-2023.5.16/artistools/atomic/_atomic_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/codecomparison.py` & `artistools-2023.5.16/artistools/codecomparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-"""
-File readers for Blondin et al. code comparison file formats
+"""File readers for Blondin et al. code comparison file formats
 The model paths are not real file system paths, but take a form like this:
-codecomparison/[modelname]/[codename]
+codecomparison/[modelname]/[codename].
 
 e.g., codecomparison/DDC10/artisnebular
 """
 import math
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any
@@ -45,24 +44,24 @@
         return tstarts
     if loc == "end":
         return tends
     if loc == "delta":
         tdeltas = tends - tstarts
         return tdeltas
 
-    raise ValueError("loc must be one of 'mid', 'start', 'end', or 'delta'")
+    msg = "loc must be one of 'mid', 'start', 'end', or 'delta'"
+    raise ValueError(msg)
 
 
 def read_reference_estimators(
     modelpath: Union[str, Path],
     modelgridindex: Union[None, int, Sequence[int]] = None,
     timestep: Union[None, int, Sequence[int]] = None,
 ) -> dict[tuple[int, int], Any]:
     """Read estimators from code comparison workshop file."""
-
     virtualfolder, inputmodel, codename = Path(modelpath).parts
     assert virtualfolder == "codecomparison"
 
     inputmodelfolder = Path(at.get_config()["codecomparisondata1path"], inputmodel)
 
     physfilepath = Path(inputmodelfolder, f"phys_{inputmodel}_{codename}.txt")
 
@@ -198,21 +197,19 @@
     return dfspectra, arr_timedays
 
 
 def plot_spectrum(
     modelpath: Union[str, Path], timedays: Union[str, float], axis: matplotlib.axes.Axes, **plotkwargs
 ) -> None:
     dfspectra, arr_timedays = get_spectra(modelpath)
-    # print(dfspectra)
     timeindex = (np.abs(arr_timedays - float(timedays))).argmin()
     timedays_found = dfspectra.columns[timeindex + 1]
 
     print(f"{modelpath}: requested spectrum at {timedays} days. Closest matching spectrum is at {timedays_found} days")
     assert np.isclose(arr_timedays[timeindex], float(timedays_found), rtol=0.01)  # check columns match
     assert np.isclose(float(timedays), float(timedays_found), rtol=0.1)  # found a detect match to requested time
-    # print(dfspectra[['lambda', timedays_found]])
     label = str(modelpath).lstrip("_") + f" {timedays_found}d"
 
     megaparsec_to_cm = 3.085677581491367e24
     arr_flux = dfspectra[dfspectra.columns[timeindex + 1]] / 4 / math.pi / (megaparsec_to_cm**2)
 
     axis.plot(dfspectra["lambda"], arr_flux, label=label, **plotkwargs)
```

### Comparing `artistools-2023.4.19.2/artistools/commands.py` & `artistools-2023.5.16/artistools/commands.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,62 @@
+import argparse
 import subprocess
 from pathlib import Path
+from typing import Any
+from typing import Union
+
+try:
+    from typing_extensions import TypeAlias
+except ImportError:
+    from typing import TypeAlias
+
+cmdtype: TypeAlias = dict[str, Union[tuple[str, str], "cmdtype"]]
+
+dictcommands: cmdtype = {
+    "comparetogsinetwork": ("gsinetwork", "main"),
+    "deposition": ("deposition", "main_analytical"),
+    "describeinputmodel": ("inputmodel.describeinputmodel", "main"),
+    "exportmassfractions": ("estimators.exportmassfractions", "main"),
+    "listtimesteps": ("", "showtimesteptimes"),
+    "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
+    "maketardismodelfromartis": ("inputmodel.maketardismodelfromartis", "main"),
+    "maptogrid": ("inputmodel.maptogrid", "main"),
+    "plotestimators": ("estimators.plotestimators", "main"),
+    "plotinitialcomposition": ("initial_composition", "main"),
+    "plotlightcurves": ("lightcurve.plotlightcurve", "main"),
+    "plotlinefluxes": ("linefluxes", "main"),
+    "plotmodeldensity": ("inputmodel.plotdensity", "main"),
+    "plotmodeldeposition": ("deposition", "main"),
+    "plotmacroatom": ("macroatom", "main"),
+    "plotnltepops": ("nltepops.plotnltepops", "main"),
+    "plotnonthermal": ("nonthermal", "main"),
+    "plotradfield": ("radfield", "main"),
+    "plotspectra": ("spectra.plotspectra", "main"),
+    "plotspherical": ("plotspherical", "main"),
+    "plottransitions": ("transitions", "main"),
+    "plotviewingangles": ("viewing_angles_visualization", "main"),
+    "setupcompletions": ("commands", "setup_completions"),
+    "spencerfano": ("nonthermal.solvespencerfanocmd", "main"),
+    "writecodecomparisondata": ("writecomparisondata", "main"),
+    "inputmodel": {
+        "describe": ("inputmodel.describeinputmodel", "main"),
+        "maptogrid": ("inputmodel.maptogrid", "main"),
+        "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
+        "makeartismodel": ("inputmodel.makeartismodel", "main"),
+        "artistools-make1dslicefrom3dmodel": ("inputmodel.1dslicefrom3d", "main"),
+        "makeartismodel1dslicefromcone": ("inputmodel.slice1Dfromconein3dmodel", "main"),
+        "makeartismodelbotyanski2017": ("inputmodel.botyanski2017", "main"),
+        "makeartismodelfromshen2018": ("inputmodel.shen2018", "main"),
+        "makeartismodelfromlapuente": ("inputmodel.lapuente", "main"),
+        "makeartismodelscalevelocity": ("inputmodel.scalevelocity", "main"),
+        "makeartismodelfullymixed": ("inputmodel.fullymixed", "main"),
+        "makeartismodelsolar_rprocess": ("inputmodel.rprocess_solar", "main"),
+        "makeartismodelfromsingletrajectory": ("inputmodel.rprocess_from_trajectory", "main"),
+    },
+}
 
 
 def get_commandlist() -> dict[str, tuple[str, str]]:
     commandlist = {
         "at": ("artistools", "main"),
         "artistools": ("artistools", "main"),
         "artistools-comparetogsinetwork": ("artistools.gsinetwork", "main"),
@@ -49,29 +102,29 @@
         "artistools-spectrum": ("artistools.spectra", "main"),
         "plotartistransitions": ("artistools.transitions", "main"),
         "artistools-transitions": ("artistools.transitions", "main"),
         "plotartisinitialcomposition": ("artistools.initial_composition", "main"),
         "artistools-initialcomposition": ("artistools.initial_composition", "main"),
         "artistools-writecodecomparisondata": ("artistools.writecomparisondata", "main"),
         "artistools-setup_completions": ("artistools.commands", "setup_completions"),
-        "artistools-viewingangles": ("artistools.viewing_angles_visualization", "cli"),
-        "plotartisviewingangles": ("artistools.viewing_angles_visualization", "cli"),
+        "artistools-viewingangles": ("artistools.viewing_angles_visualization", "main"),
+        "plotartisviewingangles": ("artistools.viewing_angles_visualization", "main"),
     }
 
     return commandlist
 
 
 def get_console_scripts() -> list[str]:
     console_scripts = [
         f"{command} = {submodulename}:{funcname}" for command, (submodulename, funcname) in get_commandlist().items()
     ]
     return console_scripts
 
 
-def setup_completions() -> None:
+def setup_completions(*args: Any, **kwargs: Any) -> None:
     # Add the following lines to your .zshrc file to get command completion:
     # autoload -U bashcompinit
     # bashcompinit
     # source artistoolscompletions.sh
     path_repo = Path(__file__).absolute().parent.parent
     with open(path_repo / "artistoolscompletions.sh", "w", encoding="utf-8") as f:
         f.write("#!/usr/bin/env zsh\n")
@@ -93,9 +146,9 @@
             completecommand = strcommandregister.replace("__MY_COMMAND__", command)
             f.write(completecommand + "\n")
 
     print("To enable completions, add this line to your .zshrc/.bashrc")
     print("source artistoolscompletions.sh")
 
 
-def addargs(parser=None) -> None:
+def addargs(parser: argparse.ArgumentParser) -> None:
     pass
```

### Comparing `artistools-2023.4.19.2/artistools/configuration.py` & `artistools-2023.5.16/artistools/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import multiprocessing as mp
 import subprocess
 from pathlib import Path
 from typing import Any
 from typing import Optional
 
 import psutil
 
 config: dict[str, Any] = {}
 
 
 def setup_config():
-    mp.set_start_method("fork")
     # count the cores (excluding the efficiency cores on ARM)
     try:
         num_processes = int(
             subprocess.run(
                 ["sysctl", "-n", "hw.perflevel0.logicalcpu"], capture_output=True, text=True, check=True
             ).stdout
         )
```

### Comparing `artistools-2023.4.19.2/artistools/data/ElBiEn_2007.txt` & `artistools-2023.5.16/artistools/data/ElBiEn_2007.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/atomic_properties.txt` & `artistools-2023.5.16/artistools/data/atomic_properties.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/betaminusdecays.txt` & `artistools-2023.5.16/artistools/data/betaminusdecays.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/binding_energies.txt` & `artistools-2023.5.16/artistools/data/binding_energies.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/collion-AR1985.txt` & `artistools-2023.5.16/artistools/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/collion-reference.txt` & `artistools-2023.5.16/artistools/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/collion.txt` & `artistools-2023.5.16/artistools/data/collion.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/elements.csv` & `artistools-2023.5.16/artistools/data/elements.csv`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/400.txt` & `artistools-2023.5.16/artistools/data/filters/400.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/520.txt` & `artistools-2023.5.16/artistools/data/filters/520.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/B.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/U.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/V.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/gs.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/is.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/rs.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/ASIAGO/zs.txt` & `artistools-2023.5.16/artistools/data/filters/ASIAGO/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/B.txt` & `artistools-2023.5.16/artistools/data/filters/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/FUV.txt` & `artistools-2023.5.16/artistools/data/filters/FUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/H.txt` & `artistools-2023.5.16/artistools/data/filters/H.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/H_ab.txt` & `artistools-2023.5.16/artistools/data/filters/H_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/I.txt` & `artistools-2023.5.16/artistools/data/filters/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/J.txt` & `artistools-2023.5.16/artistools/data/filters/J.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/J_ab.txt` & `artistools-2023.5.16/artistools/data/filters/J_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/K.txt` & `artistools-2023.5.16/artistools/data/filters/K.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/K_ab.txt` & `artistools-2023.5.16/artistools/data/filters/K_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/B.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/I.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/R.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/U.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/V.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/gs.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/is.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/rs.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/us.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LCOGT/zs.txt` & `artistools-2023.5.16/artistools/data/filters/LCOGT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LSQ/rs.txt` & `artistools-2023.5.16/artistools/data/filters/LSQ/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LT/gs.txt` & `artistools-2023.5.16/artistools/data/filters/LT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LT/is.txt` & `artistools-2023.5.16/artistools/data/filters/LT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LT/rs.txt` & `artistools-2023.5.16/artistools/data/filters/LT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LT/us.txt` & `artistools-2023.5.16/artistools/data/filters/LT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/LT/zs.txt` & `artistools-2023.5.16/artistools/data/filters/LT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/B.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/I.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/R.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/U.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/V.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/gs.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/is.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/rs.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/us.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NOT/zs.txt` & `artistools-2023.5.16/artistools/data/filters/NOT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/B.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/I.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/R.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/U.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/V.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/gs.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/rs.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NTT/zs.txt` & `artistools-2023.5.16/artistools/data/filters/NTT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/NUV.txt` & `artistools-2023.5.16/artistools/data/filters/NUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/OGLE/I.txt` & `artistools-2023.5.16/artistools/data/filters/OGLE/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/OGLE/V.txt` & `artistools-2023.5.16/artistools/data/filters/OGLE/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/PS1/gs.txt` & `artistools-2023.5.16/artistools/data/filters/PS1/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/PS1/is.txt` & `artistools-2023.5.16/artistools/data/filters/PS1/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/PS1/rs.txt` & `artistools-2023.5.16/artistools/data/filters/PS1/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/PS1/ws.txt` & `artistools-2023.5.16/artistools/data/filters/PS1/ws.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/PS1/zs.txt` & `artistools-2023.5.16/artistools/data/filters/PS1/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/R.txt` & `artistools-2023.5.16/artistools/data/filters/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/gs.txt` & `artistools-2023.5.16/artistools/data/filters/SKYMAPPER/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/is.txt` & `artistools-2023.5.16/artistools/data/filters/SKYMAPPER/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/rs.txt` & `artistools-2023.5.16/artistools/data/filters/SKYMAPPER/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/us.txt` & `artistools-2023.5.16/artistools/data/filters/SKYMAPPER/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/SKYMAPPER/zs.txt` & `artistools-2023.5.16/artistools/data/filters/SKYMAPPER/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/U.txt` & `artistools-2023.5.16/artistools/data/filters/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/V.txt` & `artistools-2023.5.16/artistools/data/filters/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/gs.txt` & `artistools-2023.5.16/artistools/data/filters/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/is.txt` & `artistools-2023.5.16/artistools/data/filters/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/rs.txt` & `artistools-2023.5.16/artistools/data/filters/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/us.txt` & `artistools-2023.5.16/artistools/data/filters/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvm2.txt` & `artistools-2023.5.16/artistools/data/filters/uvm2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvm2_ab.txt` & `artistools-2023.5.16/artistools/data/filters/uvm2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvw1.txt` & `artistools-2023.5.16/artistools/data/filters/uvw1.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvw1_ab.txt` & `artistools-2023.5.16/artistools/data/filters/uvw1_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvw2.txt` & `artistools-2023.5.16/artistools/data/filters/uvw2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/uvw2_ab.txt` & `artistools-2023.5.16/artistools/data/filters/uvw2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/filters/zs.txt` & `artistools-2023.5.16/artistools/data/filters/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt` & `artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt` & `artistools-2023.5.16/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt` & `artistools-2023.5.16/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2010lp_20110928_fors2.txt` & `artistools-2023.5.16/artistools/data/refspectra/2010lp_20110928_fors2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii` & `artistools-2023.5.16/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz` & `artistools-2023.5.16/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt` & `artistools-2023.5.16/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt` & `artistools-2023.5.16/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt` & `artistools-2023.5.16/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt` & `artistools-2023.5.16/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt` & `artistools-2023.5.16/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt` & `artistools-2023.5.16/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt` & `artistools-2023.5.16/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt` & `artistools-2023.5.16/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt` & `artistools-2023.5.16/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/data/solar_r_abundance_pattern.txt` & `artistools-2023.5.16/artistools/data/solar_r_abundance_pattern.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/deposition.py` & `artistools-2023.5.16/artistools/deposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,20 +42,17 @@
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=".", help="Path to ARTIS folder")
 
     parser.add_argument("-timedays", "-t", default=330, type=float, help="Time in days")
 
 
 def main_analytical(args: Optional[argparse.Namespace] = None, argsraw: Optional[list[str]] = None, **kwargs) -> None:
-    """Use the model initial conditions to calculate the deposition rates"""
-
+    """Use the model initial conditions to calculate the deposition rates."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot deposition rate of a model at time t (days)."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
     dfmodel, t_model_init, _ = at.inputmodel.get_modeldata_tuple(args.modelpath)
 
     t_init = t_model_init * u.day
 
@@ -113,20 +110,19 @@
         #     nnlevel = dfnltepops_cell.query('level == 0', inplace=False).iloc[0]['n_NLTE']
         #     width = ((v_outer - v_inner) * t_now).to('cm').value
         #     tau = width * phixs * nnlevel
         #     print(f'width: {width:.3e} cm, phixs: {phixs:.3e} cm^2, nnlevel: {nnlevel:.3e} cm^-3, tau: {tau:.3e}')
     print(f'Global posdep: {global_posdep.to("solLum"):.3e}')
 
 
-def main(args: Optional[argparse.Namespace] = None, argsraw: Optional[list[str]] = None, **kwargs):
+def main(args: Optional[argparse.Namespace] = None, argsraw: Optional[list[str]] = None, **kwargs) -> None:
+    """Plot deposition rate of a model at time t (days)."""
     main_analytical(args=args, argsraw=argsraw, **kwargs)
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot deposition rate of a model at time t (days)."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
         # TODO: plot deposition.out file!
```

### Comparing `artistools-2023.4.19.2/artistools/estimators/__init__.py` & `artistools-2023.5.16/artistools/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/estimators/estimators.py` & `artistools-2023.5.16/artistools/estimators/estimators.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import math
 import multiprocessing
 import sys
 from collections import namedtuple
 from collections.abc import Collection
 from collections.abc import Iterator
 from collections.abc import Sequence
-from functools import lru_cache
 from functools import partial
 from functools import reduce
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
 
@@ -124,30 +123,33 @@
 
 
 def parse_estimfile(
     estfilepath: Path,
     modelpath: Path,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
+    skip_emptycells: bool = False,
 ) -> Iterator[tuple[int, int, dict]]:  # pylint: disable=unused-argument
     """Generate timestep, modelgridindex, dict from estimator file."""
-    # itstep = at.get_inputparams(modelpath)['itstep']
-
     with at.zopen(estfilepath) as estimfile:
         timestep: int = -1
         modelgridindex: int = -1
         estimblock: dict[Any, Any] = {}
         for line in estimfile:
             row: list[str] = line.split()
             if not row:
                 continue
 
             if row[0] == "timestep":
                 # yield the previous block before starting a new one
-                if timestep >= 0 and modelgridindex >= 0:
+                if (
+                    timestep >= 0
+                    and modelgridindex >= 0
+                    and not (skip_emptycells and estimblock.get("emptycell", True))
+                ):
                     yield timestep, modelgridindex, estimblock
 
                 timestep = int(row[1])
                 # if timestep > itstep:
                 #     print(f"Dropping estimator data from timestep {timestep} and later (> itstep {itstep})")
                 #     # itstep in input.txt is updated by ARTIS at every timestep, so the data beyond here
                 #     # could be half-written to disk and cause parsing errors
@@ -227,26 +229,27 @@
                     estimblock["total_dep"] = estimblock["heating_dep"] / estimblock["heating_dep/total_dep"]
 
             elif row[0] == "cooling:" and get_heatingcooling:
                 for coolingtype, value in zip(row[1::2], row[2::2]):
                     estimblock["cooling_" + coolingtype] = float(value)
 
     # reached the end of file
-    if timestep >= 0 and modelgridindex >= 0:
+    if timestep >= 0 and modelgridindex >= 0 and not (skip_emptycells and estimblock.get("emptycell", True)):
         yield timestep, modelgridindex, estimblock
 
 
 def read_estimators_from_file(
     folderpath: Union[Path, str],
     modelpath: Path,
     arr_velocity_outer: Optional[Sequence[float]],
     mpirank: int,
     printfilename: bool = False,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
+    skip_emptycells: bool = False,
 ) -> dict[tuple[int, int], Any]:
     estimators_thisfile = {}
     estimfilename = f"estimators_{mpirank:04d}.out"
     try:
         estfilepath = at.firstexisting(estimfilename, folder=folderpath, tryzipped=True)
     except FileNotFoundError:
         # not worth printing an error, because ranks with no cells to update do not produce an estimator file
@@ -254,38 +257,45 @@
         return {}
 
     if printfilename:
         filesize = Path(estfilepath).stat().st_size / 1024 / 1024
         print(f"Reading {estfilepath.relative_to(modelpath.parent)} ({filesize:.2f} MiB)")
 
     for fileblock_timestep, fileblock_modelgridindex, file_estimblock in parse_estimfile(
-        estfilepath, modelpath, get_ion_values=get_ion_values, get_heatingcooling=get_heatingcooling
+        estfilepath,
+        modelpath,
+        get_ion_values=get_ion_values,
+        get_heatingcooling=get_heatingcooling,
+        skip_emptycells=skip_emptycells,
     ):
         if arr_velocity_outer is not None:
             file_estimblock["velocity_outer"] = arr_velocity_outer[fileblock_modelgridindex]
             file_estimblock["velocity"] = file_estimblock["velocity_outer"]
 
         estimators_thisfile[(fileblock_timestep, fileblock_modelgridindex)] = file_estimblock
 
     return estimators_thisfile
 
 
-@lru_cache(maxsize=16)
 def read_estimators(
-    modelpath: Union[Path, str],
+    modelpath: Union[Path, str] = Path(),
     modelgridindex: Union[None, int, Sequence[int]] = None,
     timestep: Union[None, int, Sequence[int]] = None,
+    mpirank: Optional[int] = None,
+    runfolder: Union[None, str, Path] = None,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
+    skip_emptycells: bool = False,
+    add_velocity: bool = True,
 ) -> dict[tuple[int, int], dict]:
     """Read estimator files into a nested dictionary structure.
 
     Speed it up by only retrieving estimators for a particular timestep(s) or modelgrid cells.
     """
-
+    modelpath = Path(modelpath)
     match_modelgridindex: Collection[int]
     if modelgridindex is None:
         match_modelgridindex = []
     elif isinstance(modelgridindex, int):
         match_modelgridindex = (modelgridindex,)
     else:
         match_modelgridindex = tuple(modelgridindex)
@@ -304,41 +314,51 @@
     if not Path(modelpath).exists() and Path(modelpath).parts[0] == "codecomparison":
         return artistools.codecomparison.read_reference_estimators(
             modelpath, timestep=timestep, modelgridindex=modelgridindex
         )
 
     # print(f" matching cells {match_modelgridindex} and timesteps {match_timestep}")
 
-    modeldata, _ = at.inputmodel.get_modeldata(modelpath, getheadersonly=True)
-    if "velocity_outer" in modeldata.columns:
-        modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-        arr_velocity_outer = tuple([float(v) for v in modeldata["velocity_outer"].to_numpy()])
-    else:
-        arr_velocity_outer = None
+    arr_velocity_outer = None
+    if add_velocity:
+        modeldata, _ = at.inputmodel.get_modeldata(modelpath, getheadersonly=True)
+        if "velocity_outer" in modeldata.columns:
+            modeldata, _ = at.inputmodel.get_modeldata(modelpath)
+            arr_velocity_outer = tuple([float(v) for v in modeldata["velocity_outer"].to_numpy()])
+
+    mpiranklist = (
+        at.get_mpiranklist(modelpath, modelgridindex=match_modelgridindex, only_ranks_withgridcells=True)
+        if mpirank is None
+        else [mpirank]
+    )
 
-    mpiranklist = at.get_mpiranklist(modelpath, modelgridindex=match_modelgridindex, only_ranks_withgridcells=True)
+    runfolders = at.get_runfolders(modelpath, timesteps=match_timestep) if runfolder is None else [Path(runfolder)]
 
     printfilename = len(mpiranklist) < 10
 
     estimators = {}
-    for folderpath in at.get_runfolders(modelpath, timesteps=match_timestep):
-        print(f"Reading {len(list(mpiranklist))} estimator files in {folderpath.relative_to(Path(modelpath).parent)}")
+    for folderpath in runfolders:
+        if not printfilename:
+            print(
+                f"Reading {len(list(mpiranklist))} estimator files in {folderpath.relative_to(Path(modelpath).parent)}"
+            )
 
         processfile = partial(
             read_estimators_from_file,
             folderpath,
             modelpath,
             arr_velocity_outer,
             get_ion_values=get_ion_values,
             get_heatingcooling=get_heatingcooling,
             printfilename=printfilename,
+            skip_emptycells=skip_emptycells,
         )
 
         if at.get_config()["num_processes"] > 1:
-            with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+            with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
                 arr_rankestimators = pool.map(processfile, mpiranklist)
                 pool.close()
                 pool.join()
                 pool.terminate()
         else:
             arr_rankestimators = [processfile(rank) for rank in mpiranklist]
 
@@ -464,17 +484,16 @@
         # no superlevel
         pass
 
     return energypopsum / ionpopsum
 
 
 def get_partiallycompletetimesteps(estimators: dict[Any, Any]) -> list[int]:
-    """
-    During a simulation, some estimator files can contain information for some cells but not others
-    for the current timestep
+    """During a simulation, some estimator files can contain information for some cells but not others
+    for the current timestep.
     """
     timestepcells: dict[int, list[int]] = {}
     all_mgis = set()
     for nts, mgi in estimators:
         if nts not in timestepcells:
             timestepcells[nts] = []
         timestepcells[nts].append(mgi)
```

### Comparing `artistools-2023.4.19.2/artistools/estimators/estimators_classic.py` & `artistools-2023.5.16/artistools/estimators/estimators_classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 from pathlib import Path
 
 import artistools as at
 
 
 def get_atomic_composition(modelpath):
-    """Read ion list from output file"""
+    """Read ion list from output file."""
     atomic_composition = {}
 
-    output = open(modelpath / "output_0-0.txt").read().splitlines()
-    ioncount = 0
-    for row in output:
-        if row.split()[0] == "[input.c]":
-            split_row = row.split()
-            if split_row[1] == "element":
-                Z = int(split_row[4])
-                ioncount = 0
-            elif split_row[1] == "ion":
-                ioncount += 1
-                atomic_composition[Z] = ioncount
+    with open(modelpath / "output_0-0.txt") as foutput:
+        ioncount = 0
+        for row in foutput:
+            if row.split()[0] == "[input.c]":
+                split_row = row.split()
+                if split_row[1] == "element":
+                    Z = int(split_row[4])
+                    ioncount = 0
+                elif split_row[1] == "ion":
+                    ioncount += 1
+                    atomic_composition[Z] = ioncount
     return atomic_composition
 
 
 def parse_ion_row_classic(row, outdict, atomic_composition):
     outdict["populations"] = {}
 
     elements = atomic_composition.keys()
```

### Comparing `artistools-2023.4.19.2/artistools/estimators/exportmassfractions.py` & `artistools-2023.5.16/artistools/estimators/exportmassfractions.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/estimators/plot3destimators_classic.py` & `artistools-2023.5.16/artistools/estimators/plot3destimators_classic.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/estimators/plotestimators.py` & `artistools-2023.5.16/artistools/estimators/plotestimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # PYTHON_ARGCOMPLETE_OK
 """Functions for plotting artis estimators and internal structure.
 
 Examples are temperatures, populations, heating/cooling rates.
 """
 import argparse
 import math
-import multiprocessing
-import os
 import sys
 from pathlib import Path
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -736,16 +734,16 @@
             **plotkwargs,
         )
 
     if len(set(mgilist)) == 1 and len(timestepslist[0]) > 1:  # single grid cell versus time plot
         figure_title = f"{modelname}\nCell {mgilist[0]}"
 
         defaultoutputfile = Path("plotestimators_cell{modelgridindex:03d}.pdf")
-        if os.path.isdir(args.outputfile):
-            args.outputfile = os.path.join(args.outputfile, defaultoutputfile)
+        if Path(args.outputfile).is_dir():
+            args.outputfile = str(Path(args.outputfile, defaultoutputfile))
 
         outfilename = str(args.outputfile).format(modelgridindex=mgilist[0])
 
     else:
         timeavg = (args.timemin + args.timemax) / 2.0
         if args.multiplot and not args.classicartis:
             tdays = estimators[(timestepslist[0][0], mgilist[0])]["tdays"]
@@ -753,16 +751,16 @@
         elif args.multiplot and args.classicartis:
             timedays = float(at.get_timestep_time(modelpath, timestepslist[0]))
             figure_title = f"{modelname}\nTimestep {timestepslist[0]} ({timedays:.2f}d)"
         else:
             figure_title = f"{modelname}\nTimestep {timestepslist[0]} ({timeavg:.2f}d)"
 
         defaultoutputfile = Path("plotestimators_ts{timestep:02d}_{timeavg:.0f}d.pdf")
-        if os.path.isdir(args.outputfile):
-            args.outputfile = os.path.join(args.outputfile, defaultoutputfile)
+        if Path(args.outputfile).is_dir():
+            args.outputfile = str(Path(args.outputfile, defaultoutputfile))
 
         outfilename = str(args.outputfile).format(timestep=timestepslist[0][0], timeavg=timeavg)
 
     if not args.notitle:
         axes[0].set_title(figure_title, fontsize=11)
     # plt.suptitle(figure_title, fontsize=11, verticalalignment='top')
 
@@ -815,15 +813,14 @@
 
         if not list_rrc:
             continue
 
         # sort the pairs by temperature ascending
         listT_e, list_rrc, list_rrc2 = zip(*sorted(zip(listT_e, list_rrc, list_rrc2), key=lambda x: x[0]))
 
-        # markersize=4, marker='s',
         ax.plot(listT_e, list_rrc, linewidth=2, label=f"{ionstr} ARTIS RRC_LTE_Nahar", **plotkwargs)
         ax.plot(listT_e, list_rrc2, linewidth=2, label=f"{ionstr} ARTIS Alpha_R", **plotkwargs)
 
         try:
             dfrates = recombcalibrationdata[(atomic_number, ion_stage)].query(
                 "T_e > @T_e_min & T_e < @T_e_max", local_dict={"T_e_min": min(listT_e), "T_e_max": max(listT_e)}
             )
@@ -943,18 +940,17 @@
 
     parser.add_argument(
         "--classicartis", action="store_true", help="Flag to show using output from classic ARTIS branch"
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Plot ARTIS estimators."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS estimators."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     modelpath = Path(args.modelpath)
 
@@ -1043,15 +1039,16 @@
         if args.modelgridindex > -1 or args.x in ["time", "timestep"]:
             # plot time evolution in specific cell
             if not args.x:
                 args.x = "time"
             mgilist = [args.modelgridindex] * len(timesteps_included)
             timesteplist_unfiltered = [(ts,) for ts in timesteps_included]
             if estimators[(args.modelgridindex, timesteps_included[0])]["emptycell"]:
-                raise ValueError(f"cell {args.modelgridindex} is empty. no estimators available")
+                msg = f"cell {args.modelgridindex} is empty. no estimators available"
+                raise ValueError(msg)
             make_plot(modelpath, timesteplist_unfiltered, mgilist, estimators, args.x, plotlist, args)
         else:
             # plot a range of cells in a time snapshot showing internal structure
 
             if not args.x:
                 args.x = "velocity_outer"
 
@@ -1088,9 +1085,8 @@
 
             else:
                 timesteplist_unfiltered = [timesteps_included] * len(allnonemptymgilist)
                 make_plot(modelpath, timesteplist_unfiltered, allnonemptymgilist, estimators, args.x, plotlist, args)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/gsinetwork.py` & `artistools-2023.5.16/artistools/gsinetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,16 +311,15 @@
 
 def get_particledata(
     arr_time_s: Sequence[float],
     arr_strnuc: list[str],
     traj_root: Path,
     particleid: int,
 ) -> tuple[int, dict[str, np.ndarray]]:
-    """
-    for an array of times (NSM time including time before merger), interpolate the heating rates of various decay channels
+    """For an array of times (NSM time including time before merger), interpolate the heating rates of various decay channels
     and (if arr_strnuc is not empty) the nuclear mass fractions.
     """
     try:
         nts_min = at.inputmodel.rprocess_from_trajectory.get_closest_network_timestep(
             traj_root, particleid, timesec=min(arr_time_s), cond="lessthan"
         )
         nts_max = at.inputmodel.rprocess_from_trajectory.get_closest_network_timestep(
@@ -479,15 +478,14 @@
             if nts in partiallycomplete_timesteps:
                 continue
             if mgi not in mgiplotlist and not get_global_Ye or estimators[(nts, mgi)]["emptycell"]:
                 continue
 
             if first_mgi is None:
                 first_mgi = mgi
-            # time_days = float(estimators[(nts, mgi)]['tdays'])
             time_days = tmids[nts]
 
             if mgi == first_mgi:
                 arr_time_artis_days.append(time_days)
 
             rho_init_cgs = 10 ** dfmodel.iloc[mgi].logrho
             rho_cgs = rho_init_cgs * (t_model_init_days / time_days) ** 3
@@ -565,29 +563,29 @@
     list_particleids_getabund = dfpartcontrib.query("(cellindex - 1) in @mgiplotlist").particleid.unique()
     fworkerwithabund = partial(get_particledata, arr_time_gsi_s_incpremerger, arr_strnuc, traj_root)
 
     print(f"Reading trajectories from {traj_root}")
     print(f"  Reading Qdot/thermo and abundance data for {len(list_particleids_getabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_withabund = pool.map(fworkerwithabund, list_particleids_getabund)
             pool.close()
             pool.join()
     else:
         list_particledata_withabund = [fworkerwithabund(particleid) for particleid in list_particleids_getabund]
 
     list_particleids_noabund = [
         pid for pid in dfpartcontrib.particleid.unique() if pid not in list_particleids_getabund
     ]
     fworkernoabund = partial(get_particledata, arr_time_gsi_s_incpremerger, [], traj_root)
     print(f"  Reading for Qdot/thermo data (no abundances needed) for {len(list_particleids_noabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_noabund = pool.map(fworkernoabund, list_particleids_noabund)
             pool.close()
             pool.join()
     else:
         list_particledata_noabund = [fworkernoabund(particleid) for particleid in list_particleids_noabund]
 
     allparticledata = dict(list_particledata_withabund + list_particledata_noabund)
@@ -630,18 +628,17 @@
         "-mgi",
         default=None,
         help="Modelgridindex (zero-indexed) to plot or list such as 4,5,6",
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Compare the energy release and abundances from ARTIS to the GSI Network calculation."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Create solar r-process pattern in ARTIS format."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     arr_el_a = [
```

### Comparing `artistools-2023.4.19.2/artistools/hesma_scripts.py` & `artistools-2023.5.16/artistools/hesma_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def plot_hesma_spectrum(timeavg, axes):
     hesma_file = Path("/Users/ccollins/Downloads/hesma_files/M2a/hesma_specseq.dat")
     hesma_spec = pd.read_csv(hesma_file, comment="#", delim_whitespace=True, dtype=float)
     # print(hesma_spec)
 
     def match_closest_time(reftime):
-        return str("{}".format(min([float(x) for x in hesma_spec.keys()[1:]], key=lambda x: abs(x - reftime))))
+        return str(f"{min([float(x) for x in hesma_spec.keys()[1:]], key=lambda x: abs(x - reftime))}")
 
     closest_time = match_closest_time(timeavg)
     closest_time = f"{closest_time:.2f}"
     print(closest_time)
 
     # Scale distance to 1 Mpc
     dist_mpc = 1e-5  # HESMA specta at 10 pc
@@ -105,16 +105,15 @@
             " \n# Spectra are at a distance of 10 pc."
             "\n"
             + content
         )
 
 
 def make_hesma_bol_lightcurve(modelpath, outpath, timemin, timemax):
-    """UVOIR bolometric light curve (angle-averaged)"""
-
+    """UVOIR bolometric light curve (angle-averaged)."""
     lightcurvedataframe = at.lightcurve.writebollightcurvedata.get_bol_lc_from_lightcurveout(modelpath)
     print(lightcurvedataframe)
     lightcurvedataframe = lightcurvedataframe.query("time > @timemin and time < @timemax")
 
     modelname = at.get_model_name(modelpath)
     outfilename = f"doubledet_2021_{modelname}.dat"
```

### Comparing `artistools-2023.4.19.2/artistools/initial_composition.py` & `artistools-2023.5.16/artistools/initial_composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,62 +77,59 @@
 
     if modelmeta is not None and plotaxis1 is not None and plotaxis2 is not None:
         assert slicedf.shape[0] == modelmeta[f"ncoordgrid{plotaxis1}"] * modelmeta[f"ncoordgrid{plotaxis2}"]
 
     return slicedf
 
 
-def plot_slice_modelcol(ax, plotvals, modelmeta, colname, plotaxis1, plotaxis2, t_model_d, args):
-    print(colname)
-    colorscale = plotvals[colname] * plotvals["rho"] if colname.startswith("X_") else plotvals[colname]
+def plot_slice_modelcol(ax, dfmodelslice, modelmeta, colname, plotaxis1, plotaxis2, t_model_d, args):
+    print(f"plotting {colname}")
+    colorscale = (
+        dfmodelslice[colname] * dfmodelslice["rho"] if colname.startswith("X_") else dfmodelslice[colname]
+    ).to_numpy()
 
     if args.hideemptycells:
         # Don't plot empty cells:
         colorscale = np.ma.masked_where(colorscale == 0.0, colorscale)
 
     if args.logcolorscale:
         # logscale for colormap
-        colorscale = np.log10(colorscale)
-    colorscale = colorscale.to_numpy()
+        with np.errstate(divide="ignore"):
+            colorscale = np.log10(colorscale)
 
     normalise_between_0_and_1 = False
     if normalise_between_0_and_1:
         norm = mpl.colors.Normalize(vmin=0, vmax=1)
         scaledmap = mpl.cm.ScalarMappable(cmap="viridis", norm=norm)
         scaledmap.set_array([])
         colorscale = scaledmap.to_rgba(colorscale)  # colorscale fixed between 0 and 1
     else:
         scaledmap = None
 
-    arr_x = plotvals[f"pos_{plotaxis1}_min"] / t_model_d / 86400 / 2.99792458e10
-    arr_y = plotvals[f"pos_{plotaxis2}_min"] / t_model_d / 86400 / 2.99792458e10
+    cmps_to_kmps = 1e-5
+    cmps_to_beta = 1.0 / (2.99792458e10)
+    unitfactor = cmps_to_beta
+    t_model_s = t_model_d * 86400.0
 
-    # x = plotvals[f'pos_{plotaxis1}'] / t_model * (u.cm/u.day).to('m/s') / 2.99792458e+8
-    # y = plotvals[f'pos_{plotaxis2}'] / t_model * (u.cm/u.day).to('m/s') / 2.99792458e+8
-
-    # im = ax.scatter(x, y, c=colorscale, marker="s", s=30, rasterized=False)  # cmap=plt.get_cmap('PuOr')
-    ncoordgrid1 = modelmeta[f"ncoordgrid{plotaxis1}"]
-    ncoordgrid2 = modelmeta[f"ncoordgrid{plotaxis2}"]
-    grid = np.zeros((ncoordgrid1, ncoordgrid2))
-
-    for i in range(0, ncoordgrid1):
-        for j in range(0, ncoordgrid2):
-            grid[j, i] = colorscale[j * ncoordgrid1 + i]
+    # take flat array and turn in into 2D array
+    grid = colorscale.reshape((modelmeta[f"ncoordgrid{plotaxis1}"], modelmeta[f"ncoordgrid{plotaxis2}"]))
 
     im = ax.imshow(
         grid,
         cmap="viridis",
         interpolation="nearest",
-        extent=(arr_x.min(), arr_x.max(), arr_y.min(), arr_y.max()),
+        extent=(
+            dfmodelslice[f"pos_{plotaxis1}_min"].min() / t_model_s * unitfactor,
+            dfmodelslice[f"pos_{plotaxis1}_max"].max() / t_model_s * unitfactor,
+            dfmodelslice[f"pos_{plotaxis2}_min"].min() / t_model_s * unitfactor,
+            dfmodelslice[f"pos_{plotaxis2}_max"].max() / t_model_s * unitfactor,
+        ),
         origin="lower",
         # vmin=0.0,
         # vmax=1.0,
-        # vmax=-9.5,
-        # vmin=-11,
-        # vmin=1e-11,
     )
 
     plot_vmax = 0.2
     ax.set_ylim(bottom=-plot_vmax, top=plot_vmax)
     ax.set_xlim(left=-plot_vmax, right=plot_vmax)
     if "_" in colname:
         ax.annotate(
@@ -152,15 +149,20 @@
     font = {
         # 'weight': 'bold',
         "size": 18
     }
     mpl.rc("font", **font)
 
     dfmodel, modelmeta = at.get_modeldata(
-        modelpath, skipnuclidemassfraccolumns=True, get_elemabundances=True, dtype_backend="pyarrow"
+        modelpath,
+        skipnuclidemassfraccolumns=True,
+        get_elemabundances=True,
+        dtype_backend="pyarrow",
+        derived_cols=["pos_max"],
+        use_polars=False,
     )
 
     targetmodeltime_days = None
     if targetmodeltime_days is not None:
         print(
             f"Scaling modeldata to {targetmodeltime_days} days. \nWARNING: abundances not scaled for radioactive decays"
         )
@@ -180,19 +182,15 @@
     )
 
     subplots = False
     if len(args.plotvars) > 1:
         subplots = True
 
     if not subplots:
-        fig = plt.figure(
-            figsize=(8, 7),
-            tight_layout={"pad": 0.4, "w_pad": 0.0, "h_pad": 0.0},
-        )
-        ax = plt.subplot(111, aspect="equal")
+        fig, ax = plt.subplots(1, 1, figsize=(8, 7), tight_layout={"pad": 0.4, "w_pad": 0.0, "h_pad": 0.0})
     else:
         rows = 1
         cols = len(args.plotvars)
 
         fig, axes = plt.subplots(
             nrows=rows,
             ncols=cols,
@@ -377,32 +375,31 @@
     parser.add_argument("--opacity", action="store_true", help="Plot opacity from opacity.txt (if available for model)")
 
     parser.add_argument("--plot3d", action="store_true", help="Make 3D plot")
 
     parser.add_argument("-surfaces3d", type=float, nargs="+", help="define positions of surfaces for 3D plots")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Plot ARTIS input model composition."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS input model composition"
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = ["."]
 
     if args.plot3d:
         make_3d_plot(Path(args.modelpath), args)
         return
 
-    _, modelmeta = at.get_modeldata(getheadersonly=True, printwarningsonly=True)
+    _, modelmeta = at.get_modeldata(modelpath=args.modelpath, getheadersonly=True, printwarningsonly=True)
 
     if modelmeta["dimensions"] == 2:
         plot_2d_initial_abundances(args.modelpath, args)
 
     elif modelmeta["dimensions"] == 3:
         plot_3d_initial_abundances(args.modelpath, args)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/1dslicefrom3d.py` & `artistools-2023.5.16/artistools/inputmodel/1dslicefrom3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import argparse
 import math
 import os
 import sys
+from pathlib import Path
 
 import matplotlib.pyplot as plt
 
 from artistools import CustomArgHelpFormatter
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
@@ -29,20 +30,20 @@
             formatter_class=CustomArgHelpFormatter,
             description="Covert abundances.txt and model.txt from 3D to a one dimensional slice.",
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args()
 
-    if not os.path.exists(args.outputfolder):
-        os.makedirs(args.outputfolder)
-    elif os.path.exists(os.path.join(args.outputfolder, "model.txt")):
+    if not Path(args.outputfolder).exists():
+        Path(args.outputfolder).mkdir(parents=True)
+    elif Path(args.outputfolder, "model.txt").exists():
         print("ABORT: model.txt already exists")
         sys.exit()
-    elif os.path.exists(os.path.join(args.outputfolder, "abundances.txt")):
+    elif Path(args.outputfolder, "abundances.txt").exists():
         print("ABORT: abundances.txt already exists")
         sys.exit()
 
     dict3dcellidto1dcellid, xlist, ylists = slice_3dmodel(args.inputfolder, args.outputfolder, args.chosenaxis)
 
     slice_abundance_file(args.inputfolder, args.outputfolder, dict3dcellidto1dcellid)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/__init__.py` & `artistools-2023.5.16/artistools/inputmodel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import artistools.inputmodel.botyanski2017
 import artistools.inputmodel.describeinputmodel
+import artistools.inputmodel.downscale3dgrid
 import artistools.inputmodel.energyinputfiles
 import artistools.inputmodel.makeartismodel
+import artistools.inputmodel.maketardismodelfromartis
 import artistools.inputmodel.modelfromhydro
 import artistools.inputmodel.opacityinputfile
 import artistools.inputmodel.rprocess_from_trajectory
+
 from .inputmodel_misc import add_derived_cols_to_modeldata
 from .inputmodel_misc import get_2d_modeldata
 from .inputmodel_misc import get_3d_model_data_merged_model_and_abundances_minimal
 from .inputmodel_misc import get_3d_modeldata_minimal
 from .inputmodel_misc import get_cell_angle
 from .inputmodel_misc import get_dfmodel_dimensions
 from .inputmodel_misc import get_initelemabundances
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/botyanski2017.py` & `artistools-2023.5.16/artistools/inputmodel/botyanski2017.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Create Botyanski et al. 2017 model."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Create Botyanski et al. 2017 ."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     e_k = 1.2  # in units of 10^51 erg
     m_ej = 1.4  # in solar masses
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/describeinputmodel.py` & `artistools-2023.5.16/artistools/inputmodel/describeinputmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,19 @@
         help="Give element abundances only, no isotope abundances (implies --getelemabundances)",
     )
 
     parser.add_argument("--getelemabundances", action="store_true", help="Get elemental abundance masses")
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Describe an ARTIS input model, such as the mass, velocity structure, and abundances."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Scale the velocity of an ARTIS model, keeping mass constant and saving back to ARTIS format.",
+            description=__doc__,
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/energyinputfiles.py` & `artistools-2023.5.16/artistools/inputmodel/energyinputfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     print("Writing energyrate.txt")
     with open(Path(outputfilepath) / "energyrate.txt", "w") as fmodel:
         fmodel.write(f'{len(energy_rate_data["times"])}\n')  # write number of points
         energy_rate_data.to_csv(fmodel, sep="\t", index=False, header=False, float_format="%.10f")
 
 
 def rprocess_const_and_powerlaw():
-    """Following eqn 4 Korobkin 2012"""
+    """Following eqn 4 Korobkin 2012."""
 
     def integrand(t_days, t0, epsilon0, sigma, alpha, thermalisation_factor):
         return (epsilon0 * ((1 / 2) - (1 / np.pi * np.arctan((t_days - t0) / sigma))) ** alpha) * (
             thermalisation_factor / 0.5
         )
 
     from scipy.integrate import quad
@@ -99,24 +99,24 @@
     E_tot = E_tot * scale_factor_energy_diff
     # print(f"E_tot after integrated line scaled to match energy of power law: {E_tot}")
 
     dE = np.diff(times_and_rate["rate"] * E_tot)
     dt = np.diff(times * 24 * 60 * 60)
 
     # check energy rate is on top of power law line
-    plt.plot(times_and_rate["times"][1:], (dE / dt) * 0.01 * MSUN)
-    plt.plot(times_and_rate["times"], qdot * 0.01 * MSUN)
-    plt.yscale("log")
-    plt.xscale("log")
-
-    plt.xlabel("Time [days]")
-    plt.ylabel("Q [erg/g/s]")
-    # plt.xlim(0.1, 20)
-    # plt.ylim(5e39, 2e41)
-    plt.show()
+    # plt.plot(times_and_rate["times"][1:], (dE / dt) * 0.01 * MSUN)
+    # plt.plot(times_and_rate["times"], qdot * 0.01 * MSUN)
+    # plt.yscale("log")
+    # plt.xscale("log")
+
+    # plt.xlabel("Time [days]")
+    # plt.ylabel("Q [erg/g/s]")
+    # # plt.xlim(0.1, 20)
+    # # plt.ylim(5e39, 2e41)
+    # plt.show()
 
     return times_and_rate, E_tot
 
 
 def energy_from_rprocess_calculation(energy_thermo_data, get_rate=True):
     index_time_greaterthan = energy_thermo_data[energy_thermo_data["time/s"] > 1e7].index  # 1e7 seconds = 116 days
     energy_thermo_data = energy_thermo_data.drop(index_time_greaterthan)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py` & `artistools-2023.5.16/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python3
-"""
-    Convert a CMFGEN model file to ARTIS format. Original script possibly by Markus Kromer?
-"""
+"""Convert a CMFGEN model file to ARTIS format. Original script possibly by Markus Kromer?."""
 # from rd_cmfgen import rd_nuc_decay_data
 from math import exp
 
 import numpy as np
 
 from .rd_cmfgen import rd_sn_hydro_data
 
@@ -71,15 +69,15 @@
 
             if iso2fract0[s] < 0.0:
                 iso1fract0[s] += iso2fract0[s]
                 iso2fract0[s] = 0.0
                 print(
                     "shell",
                     s,
-                    " goes fully to top isotope Z={} A={} of the chain at time zero".format(zparent, numnucleons),
+                    f" goes fully to top isotope Z={zparent} A={numnucleons} of the chain at time zero",
                 )
             else:
                 print(
                     "shell",
                     s,
                     " has none of the last isotope Z={} A={} of the chain at time zero".format(
                         zparent - 2, numnucleons
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/fromcmfgen/rd_cmfgen.py` & `artistools-2023.5.16/artistools/inputmodel/fromcmfgen/rd_cmfgen.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/fullymixed.py` & `artistools-2023.5.16/artistools/inputmodel/fullymixed.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/inputmodel_misc.py` & `artistools-2023.5.16/artistools/inputmodel/inputmodel_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,29 @@
 from typing import Callable
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
+import polars as pl
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 import artistools as at
 
 
 def read_modelfile_text(
     filename: Union[Path, str],
     printwarningsonly: bool = False,
     getheadersonly: bool = False,
     skipnuclidemassfraccolumns: bool = False,
     dtype_backend: Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
 ) -> tuple[pd.DataFrame, dict[str, Any]]:
-    """
-    Read an artis model.txt file containing cell velocities, density, and abundances of radioactive nuclides.
-    """
-
+    """Read an artis model.txt file containing cell velocities, density, and abundances of radioactive nuclides."""
     onelinepercellformat = None
 
     modelmeta: dict[str, Any] = {"headercommentlines": []}
 
     modelpath = Path(filename).parent
     if not printwarningsonly:
         print(f"Reading {filename}")
@@ -47,89 +45,105 @@
         while line.startswith("#"):
             line = fmodel.readline()
             if line.startswith("#"):
                 modelmeta["headercommentlines"].append(line.removeprefix("#").removeprefix(" ").removesuffix("\n"))
                 numheaderrows += 1
 
         if len(line.strip().split(" ")) == 2:
-            print("  detected 2D model file")
             modelmeta["dimensions"] = 2
             ncoordgrid_r, ncoordgrid_z = (int(n) for n in line.strip().split(" "))
             modelmeta["ncoordgrid_r"] = ncoordgrid_r
             modelmeta["ncoordgrid_z"] = ncoordgrid_z
             modelcellcount = ncoordgrid_r * ncoordgrid_z
+            print(f"  detected 2D model file with {ncoordgrid_r}x{ncoordgrid_z}={modelcellcount} cells")
         else:
             modelcellcount = int(line)
 
         modelmeta["npts_model"] = modelcellcount
         modelmeta["t_model_init_days"] = float(fmodel.readline())
         numheaderrows += 2
         t_model_init_seconds = modelmeta["t_model_init_days"] * 24 * 60 * 60
 
         filepos = fmodel.tell()
         # if the next line is a single float then the model is 2D or 3D (vmax)
         try:
             modelmeta["vmax_cmps"] = float(fmodel.readline())  # velocity max in cm/s
             xmax_tmodel = modelmeta["vmax_cmps"] * t_model_init_seconds  # xmax = ymax = zmax
             numheaderrows += 1
-            if "dimensions" not in modelmeta:
-                if not printwarningsonly:
-                    print("  detected 3D model file")
+            if "dimensions" not in modelmeta:  # not already detected as 2D
                 modelmeta["dimensions"] = 3
+                # number of grid cell steps along an axis (currently the same for xyz)
+                ncoordgridx = int(round(modelcellcount ** (1.0 / 3.0)))
+                ncoordgridy = int(round(modelcellcount ** (1.0 / 3.0)))
+                ncoordgridz = int(round(modelcellcount ** (1.0 / 3.0)))
+                assert (ncoordgridx * ncoordgridy * ncoordgridz) == modelcellcount
+                modelmeta["ncoordgridx"] = ncoordgridx
+                modelmeta["ncoordgridy"] = ncoordgridy
+                modelmeta["ncoordgridz"] = ncoordgridz
+                if ncoordgridx == ncoordgridy == ncoordgridz:
+                    modelmeta["ncoordgrid"] = ncoordgridx
+
+                if not printwarningsonly:
+                    print(
+                        "  detected 3D model file with"
+                        f" {ncoordgridx}x{ncoordgridy}x{ncoordgridz}={modelcellcount} cells"
+                    )
 
         except ValueError:
             assert modelmeta.get("dimensions", -1) != 2  # 2D model should have vmax line here
             if "dimensions" not in modelmeta:
                 if not printwarningsonly:
-                    print("  detected 1D model file")
+                    print(f"  detected 1D model file with {modelcellcount} radial zones")
                 modelmeta["dimensions"] = 1
+                getheadersonly = False
 
             fmodel.seek(filepos)  # undo the readline() and go back
 
         columns = None
         filepos = fmodel.tell()
         line = fmodel.readline()
         if line.startswith("#"):
             numheaderrows += 1
             columns = line.lstrip("#").split()
         else:
             fmodel.seek(filepos)  # undo the readline() and go back
 
         data_line_even = fmodel.readline().split()
         ncols_line_even = len(data_line_even)
+        ncols_line_odd = len(fmodel.readline().split())
 
         if columns is None:
             if modelmeta["dimensions"] == 1:
                 columns = [
                     "inputcellid",
                     "velocity_outer",
                     "logrho",
                     "X_Fegroup",
                     "X_Ni56",
                     "X_Co56",
                     "X_Fe52",
                     "X_Cr48",
                     "X_Ni57",
                     "X_Co57",
-                ][:ncols_line_even]
+                ]
 
             elif modelmeta["dimensions"] == 2:
                 columns = [
                     "inputcellid",
                     "pos_r_mid",
                     "pos_z_mid",
                     "rho",
                     "X_Fegroup",
                     "X_Ni56",
                     "X_Co56",
                     "X_Fe52",
                     "X_Cr48",
                     "X_Ni57",
                     "X_Co57",
-                ][:ncols_line_even]
+                ]
 
             elif modelmeta["dimensions"] == 3:
                 columns = [
                     "inputcellid",
                     "inputpos_a",
                     "inputpos_b",
                     "inputpos_c",
@@ -137,55 +151,46 @@
                     "X_Fegroup",
                     "X_Ni56",
                     "X_Co56",
                     "X_Fe52",
                     "X_Cr48",
                     "X_Ni57",
                     "X_Co57",
-                ][:ncols_line_even]
+                ]
+            # last two abundances are optional
+            assert columns is not None
+            assert len(columns) == (ncols_line_even + ncols_line_odd) or len(columns) == (
+                ncols_line_even + ncols_line_odd + 2
+            )
+            columns = columns[: ncols_line_even + ncols_line_odd]
 
         assert columns is not None
-
         if ncols_line_even == len(columns):
             if not printwarningsonly:
                 print("  model file is one line per cell")
             ncols_line_odd = 0
             onelinepercellformat = True
         else:
             if not printwarningsonly:
                 print("  model file format is two lines per cell")
             # columns split over two lines
-            ncols_line_odd = len(fmodel.readline().split())
             assert (ncols_line_even + ncols_line_odd) == len(columns)
             onelinepercellformat = False
 
     if skipnuclidemassfraccolumns:
         if not printwarningsonly:
             print("  skipping nuclide abundance columns in model")
         if modelmeta["dimensions"] == 1:
             ncols_line_even = 3
         elif modelmeta["dimensions"] == 2:
             ncols_line_even = 4
         elif modelmeta["dimensions"] == 3:
             ncols_line_even = 5
         ncols_line_odd = 0
 
-    if modelmeta["dimensions"] == 3:
-        # number of grid cell steps along an axis (same for xyz)
-        ncoordgridx = int(round(modelcellcount ** (1.0 / 3.0)))
-        ncoordgridy = int(round(modelcellcount ** (1.0 / 3.0)))
-        ncoordgridz = int(round(modelcellcount ** (1.0 / 3.0)))
-        modelmeta["ncoordgridx"] = ncoordgridx
-        modelmeta["ncoordgridy"] = ncoordgridy
-        modelmeta["ncoordgridz"] = ncoordgridz
-        if ncoordgridx == ncoordgridy == ncoordgridz:
-            modelmeta["ncoordgrid"] = ncoordgridx
-
-        assert (ncoordgridx * ncoordgridy * ncoordgridz) == modelcellcount
-
     nrows_read = 1 if getheadersonly else modelcellcount
 
     skiprows: Union[list, int, None]
 
     skiprows = (
         numheaderrows
         if onelinepercellformat
@@ -321,36 +326,38 @@
 
     modelmeta["modelcellcount"] = modelcellcount
 
     return dfmodel, modelmeta
 
 
 def get_modeldata(
-    inputpath: Union[Path, str] = Path(),
+    modelpath: Union[Path, str] = Path(),
     get_elemabundances: bool = False,
     derived_cols: Optional[Sequence[str]] = None,
     printwarningsonly: bool = False,
     getheadersonly: bool = False,
     skipnuclidemassfraccolumns: bool = False,
     dtype_backend: Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
+    use_polars: bool = False,
 ) -> tuple[pd.DataFrame, dict[str, Any]]:
-    """
-    Read an artis model.txt file containing cell velocities, densities, and mass fraction abundances of radioactive nuclides.
+    """Read an artis model.txt file containing cell velocities, densities, and mass fraction abundances of radioactive nuclides.
 
-    Parameters:
+    Parameters
+    ----------
         - inputpath: either a path to model.txt file, or a folder containing model.txt
         - get_elemabundances: also read elemental abundances (abundances.txt) and
             merge with the output DataFrame
 
     return dfmodel, modelmeta
         - dfmodel: a pandas DataFrame with a row for each model grid cell
         - modelmeta: a dictionary of input model parameters, with keys such as t_model_init_days, vmax_cmps, dimensions, etc.
     """
-
-    inputpath = Path(inputpath)
+    inputpath = Path(modelpath)
+    if use_polars:
+        dtype_backend = "pyarrow"
 
     if inputpath.is_dir():
         modelpath = inputpath
         filename = at.firstexisting("model.txt", folder=inputpath, tryzipped=True)
     elif inputpath.is_file():  # passed in a filename instead of the modelpath
         filename = inputpath
         modelpath = Path(inputpath).parent
@@ -360,14 +367,18 @@
         filename = Path(at.get_config()["codecomparisonmodelartismodelpath"], inputmodel, "model.txt")
     else:
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), inputpath)
 
     dfmodel = None
     filenameparquet = at.stripallsuffixes(Path(filename)).with_suffix(".txt.parquet")
 
+    if filenameparquet.exists() and Path(filename).stat().st_mtime > filenameparquet.stat().st_mtime:
+        print(f"{filename} has been modified after {filenameparquet}. Deleting out of date parquet file.")
+        filenameparquet.unlink()
+
     source_textfile_details = {"st_size": filename.stat().st_size, "st_mtime": filename.stat().st_mtime}
 
     if filenameparquet.is_file() and not getheadersonly:
         if not printwarningsonly:
             print(f"  reading data table from {filenameparquet}")
 
         pqmetadata = pq.read_metadata(filenameparquet)
@@ -387,14 +398,15 @@
                 else None
             )
             dfmodel = pd.read_parquet(
                 filenameparquet,
                 columns=columns,
                 dtype_backend=dtype_backend,
             )
+            print(f"  model is {modelmeta['dimensions']}D with {modelmeta['npts_model']} cells")
 
     if dfmodel is None:
         skipnuclidemassfraccolumns = False
         dfmodel, modelmeta = read_modelfile_text(
             filename=filename,
             printwarningsonly=printwarningsonly,
             getheadersonly=getheadersonly,
@@ -412,104 +424,122 @@
             }
             merged_metadata = {**custom_metadata, **(patable.schema.metadata or {})}
             patable = patable.replace_schema_metadata(merged_metadata)
             pq.write_table(patable, filenameparquet, compression="ZSTD")
             # dfmodel.to_parquet(filenameparquet, compression="zstd")
             print("  Done.")
 
+    dfmodel = pl.from_pandas(dfmodel).lazy()
+
     if get_elemabundances:
-        abundancedata = get_initelemabundances(
-            modelpath, dtype_backend=dtype_backend, printwarningsonly=printwarningsonly
-        )
-        dfmodel = dfmodel.merge(abundancedata, how="inner", on="inputcellid")
+        abundancedata = pl.from_pandas(
+            get_initelemabundances(modelpath, dtype_backend=dtype_backend, printwarningsonly=printwarningsonly)
+        ).lazy()
+        dfmodel = dfmodel.join(abundancedata, how="inner", on="inputcellid")
 
     if derived_cols:
         dfmodel = add_derived_cols_to_modeldata(
             dfmodel=dfmodel,
             derived_cols=derived_cols,
             dimensions=modelmeta["dimensions"],
             t_model_init_seconds=modelmeta["t_model_init_days"] * 86400.0,
             wid_init=modelmeta.get("wid_init", None),
             modelpath=modelpath,
         )
 
-    if len(dfmodel) > 100000:
-        dfmodel.info(verbose=False, memory_usage="deep")
+    if not use_polars:
+        dfmodel = dfmodel.collect().to_pandas(use_pyarrow_extension_array=(dtype_backend == "pyarrow"))
+        if modelmeta["npts_model"] > 100000 and not getheadersonly:
+            dfmodel.info(verbose=False, memory_usage="deep")
 
     return dfmodel, modelmeta
 
 
 def get_modeldata_tuple(*args, **kwargs) -> tuple[pd.DataFrame, float, float]:
-    """
-    Deprecated but included for compatibility with fixed length tuple return type
-    Use get_modeldata() instead!
+    """Deprecated but included for compatibility with fixed length tuple return type
+    Use get_modeldata() instead!.
     """
     dfmodel, modelmeta = get_modeldata(*args, **kwargs)
 
     return dfmodel, modelmeta["t_model_init_days"], modelmeta["vmax_cmps"]
 
 
 def add_derived_cols_to_modeldata(
-    dfmodel: pd.DataFrame,
+    dfmodel: Union[pl.DataFrame, pl.LazyFrame],
     derived_cols: Sequence[str],
     dimensions: Optional[int] = None,
     t_model_init_seconds: Optional[float] = None,
     wid_init: Optional[float] = None,
     modelpath: Optional[Path] = None,
-) -> pd.DataFrame:
-    """add columns to modeldata using e.g. derived_cols = ('velocity', 'Ye')"""
+) -> pl.LazyFrame:
+    """Add columns to modeldata using e.g. derived_cols = ('velocity', 'Ye')."""
     if dimensions is None:
         dimensions = get_dfmodel_dimensions(dfmodel)
 
+    dfmodel = dfmodel.lazy()
+    newcols = []
+
     if dimensions == 3:
+        axes = ["x", "y", "z"]
         if "velocity" in derived_cols or "vel_min" in derived_cols:
             assert t_model_init_seconds is not None
-            for ax in ["x", "y", "z"]:
-                dfmodel[f"vel_{ax}_min"] = dfmodel[f"pos_{ax}_min"] / t_model_init_seconds
+            newcols += [(pl.col(f"pos_{ax}_min") / t_model_init_seconds).alias(f"vel_{ax}_min") for ax in axes]
 
         if "velocity" in derived_cols or "vel_max" in derived_cols:
             assert t_model_init_seconds is not None
-            for ax in ["x", "y", "z"]:
-                dfmodel[f"vel_{ax}_max"] = (dfmodel[f"pos_{ax}_min"] + wid_init) / t_model_init_seconds
+            newcols += [
+                ((pl.col(f"pos_{ax}_min") + wid_init) / t_model_init_seconds).alias(f"vel_{ax}_max") for ax in axes
+            ]
 
         if any(col in derived_cols for col in ["velocity", "vel_mid", "vel_r_mid"]):
             assert wid_init is not None
             assert t_model_init_seconds is not None
-            for ax in ["x", "y", "z"]:
-                dfmodel[f"vel_{ax}_mid"] = (dfmodel[f"pos_{ax}_min"] + (0.5 * wid_init)) / t_model_init_seconds
+            dfmodel = dfmodel.with_columns(
+                [
+                    ((pl.col(f"pos_{ax}_min") + (0.5 * wid_init)) / t_model_init_seconds).alias(f"vel_{ax}_mid")
+                    for ax in axes
+                ]
+            )
 
-            dfmodel["vel_r_mid"] = np.sqrt(
-                dfmodel["vel_x_mid"] ** 2 + dfmodel["vel_y_mid"] ** 2 + dfmodel["vel_z_mid"] ** 2
+            newcols.append(
+                (pl.col("vel_x_mid").pow(2) + pl.col("vel_y_mid").pow(2) + pl.col("vel_z_mid").pow(2))
+                .sqrt()
+                .alias("vel_r_mid")
             )
 
     if dimensions == 3 and "pos_mid" in derived_cols or "angle_bin" in derived_cols:
         assert wid_init is not None
-        for ax in ["x", "y", "z"]:
-            dfmodel[f"pos_{ax}_mid"] = dfmodel[f"pos_{ax}_min"] + (0.5 * wid_init)
+        newcols += [(pl.col(f"pos_{ax}_min") + 0.5 * wid_init).alias(f"pos_{ax}_mid") for ax in axes]
+
+    if dimensions == 3 and "pos_max" in derived_cols:
+        assert wid_init is not None
+        newcols += [(pl.col(f"pos_{ax}_min") + wid_init).alias(f"pos_{ax}_max") for ax in axes]
 
     if "logrho" in derived_cols and "logrho" not in dfmodel.columns:
-        dfmodel["logrho"] = np.log10(dfmodel["rho"])
+        newcols.append(pl.col("rho").log10().alias("logrho"))
 
     if "rho" in derived_cols and "rho" not in dfmodel.columns:
-        dfmodel["rho"] = 10 ** dfmodel["logrho"]
+        newcols.append((10 ** pl.col("logrho")).alias("rho"))
+
+    dfmodel = dfmodel.with_columns(newcols)
 
     if "angle_bin" in derived_cols:
         assert modelpath is not None
-        dfmodel = get_cell_angle(dfmodel, modelpath)
+        dfmodel = pl.from_pandas(get_cell_angle(dfmodel.collect().to_pandas(), modelpath)).lazy()
 
     # if "Ye" in derived_cols and os.path.isfile(modelpath / "Ye.txt"):
     #     dfmodel["Ye"] = at.inputmodel.opacityinputfile.get_Ye_from_file(modelpath)
     # if "Q" in derived_cols and os.path.isfile(modelpath / "Q_energy.txt"):
     #     dfmodel["Q"] = at.inputmodel.energyinputfiles.get_Q_energy_from_file(modelpath)
 
     return dfmodel
 
 
 def get_cell_angle(dfmodel: pd.DataFrame, modelpath: Path) -> pd.DataFrame:
-    """get angle between origin to cell midpoint and the syn_dir axis"""
+    """Get angle between origin to cell midpoint and the syn_dir axis."""
     syn_dir = at.get_syn_dir(modelpath)
 
     cos_theta = np.zeros(len(dfmodel))
     i = 0
     for _, cell in dfmodel.iterrows():
         mid_point = [cell["pos_x_mid"], cell["pos_y_mid"], cell["pos_z_mid"]]
         cos_theta[i] = (np.dot(mid_point, syn_dir)) / (at.vec_len(mid_point) * at.vec_len(syn_dir))
@@ -573,15 +603,16 @@
                 mean_bin_properties[bin_number]["mean_Q"][binindex] += mean_Q
 
     return mean_bin_properties
 
 
 def get_2d_modeldata(modelpath):
     filepath = os.path.join(modelpath, "model.txt")
-    num_lines = sum(1 for line in open(filepath))
+    with open(filepath) as f:
+        num_lines = sum(1 for _ in f)
     skiprowlist = [0, 1, 2]
     skiprowlistodds = skiprowlist + [i for i in range(3, num_lines) if i % 2 == 1]
     skiprowlistevens = skiprowlist + [i for i in range(3, num_lines) if i % 2 == 0]
 
     model1stlines = pd.read_csv(filepath, delim_whitespace=True, header=None, skiprows=skiprowlistevens)
     model2ndlines = pd.read_csv(filepath, delim_whitespace=True, header=None, skiprows=skiprowlistodds)
 
@@ -599,15 +630,16 @@
     ]
     model.columns = column_names
     return model
 
 
 def get_3d_model_data_merged_model_and_abundances_minimal(args):
     """Get 3D data without generating all the extra columns in standard routine.
-    Needed for large (eg. 200^3) models"""
+    Needed for large (eg. 200^3) models.
+    """
     model = get_3d_modeldata_minimal(args.modelpath)
     abundances = get_initelemabundances(args.modelpath[0])
 
     with open(os.path.join(args.modelpath[0], "model.txt")) as fmodelin:
         fmodelin.readline()  # npts_model3d
         args.t_model = float(fmodelin.readline())  # days
         args.vmax = float(fmodelin.readline())  # v_max in [cm/s]
@@ -623,15 +655,16 @@
     merge_dfs.info(verbose=False, memory_usage="deep")
 
     return merge_dfs
 
 
 def get_3d_modeldata_minimal(modelpath) -> pd.DataFrame:
     """Read 3D model without generating all the extra columns in standard routine.
-    Needed for large (eg. 200^3) models"""
+    Needed for large (eg. 200^3) models.
+    """
     model = pd.read_csv(
         os.path.join(modelpath[0], "model.txt"), delim_whitespace=True, header=None, skiprows=3, dtype=np.float64
     )
     columns = [
         "inputcellid",
         "cellpos_in[z]",
         "cellpos_in[y]",
@@ -659,15 +692,15 @@
     vmax: Optional[float] = None,
     dimensions: Optional[int] = None,
     headercommentlines: Optional[list[str]] = None,
     modelmeta: Optional[dict[str, Any]] = None,
     twolinespercell: bool = False,
     float_format: str = ".4e",
 ) -> None:
-    """Save a pandas DataFrame and snapshot time into ARTIS model.txt"""
+    """Save a pandas DataFrame and snapshot time into ARTIS model.txt."""
     if modelmeta:
         if "headercommentlines" in modelmeta:
             assert headercommentlines is None
             headercommentlines = modelmeta["headercommentlines"]
 
         if "vmax_cmps" in modelmeta:
             assert vmax is None
@@ -777,15 +810,16 @@
                 fmodel.write("\n")
 
     print(f"Saved {modelfilepath} (took {time.perf_counter() - timestart:.1f} seconds)")
 
 
 def get_mgi_of_velocity_kms(modelpath: Path, velocity: float, mgilist=None) -> Union[int, float]:
     """Return the modelgridindex of the cell whose outer velocity is closest to velocity.
-    If mgilist is given, then chose from these cells only"""
+    If mgilist is given, then chose from these cells only.
+    """
     modeldata, _, _ = get_modeldata_tuple(modelpath)
 
     velocity = float(velocity)
 
     if not mgilist:
         mgilist = list(modeldata.index)
         arr_vouter = modeldata["velocity_outer"].to_numpy()
@@ -863,15 +897,15 @@
     dfelabundances: pd.DataFrame,
     abundancefilename: Union[Path, str],
     headercommentlines: Optional[Sequence[str]] = None,
 ) -> None:
     """Save a DataFrame (same format as get_initelemabundances) to abundances.txt.
     columns must be:
         - inputcellid: integer index to match model.txt (starting from 1)
-        - X_El: mass fraction of element with two-letter code 'El' (e.g., X_H, X_He, H_Li, ...)
+        - X_El: mass fraction of element with two-letter code 'El' (e.g., X_H, X_He, H_Li, ...).
     """
     timestart = time.perf_counter()
     if Path(abundancefilename).is_dir():
         abundancefilename = Path(abundancefilename) / "abundances.txt"
     dfelabundances["inputcellid"] = dfelabundances["inputcellid"].astype(int)
     atomic_numbers = [
         at.get_atomic_number(colname[2:]) for colname in dfelabundances.columns if colname.startswith("X_")
@@ -891,15 +925,15 @@
             fabund.write(" ".join([f"{getattr(row, colname, 0.):.6e}" for colname in elcolnames]))
             fabund.write("\n")
 
     print(f"Saved {abundancefilename} (took {time.perf_counter() - timestart:.1f} seconds)")
 
 
 def save_empty_abundance_file(ngrid: int, outputfilepath=Path()) -> None:
-    """Dummy abundance file with only zeros"""
+    """Dummy abundance file with only zeros."""
     if Path(outputfilepath).is_dir():
         outputfilepath = Path(outputfilepath) / "abundances.txt"
 
     Z_atomic = np.arange(1, 31)
 
     abundancedata: dict[str, Any] = {"cellid": range(1, ngrid + 1)}
     for atomic_number in Z_atomic:
@@ -907,46 +941,50 @@
 
     # abundancedata['Z=28'] = np.ones(ngrid)
 
     dfabundances = pd.DataFrame(data=abundancedata).round(decimals=5)
     dfabundances.to_csv(outputfilepath, header=False, sep=" ", index=False)
 
 
-def get_dfmodel_dimensions(dfmodel: pd.DataFrame) -> int:
+def get_dfmodel_dimensions(dfmodel: Union[pd.DataFrame, pl.DataFrame, pl.LazyFrame]) -> int:
     if "pos_x_min" in dfmodel.columns:
         return 3
 
+    if "pos_z_mid" in dfmodel.columns:
+        return 2
+
     return 1
 
 
 def sphericalaverage(
     dfmodel: pd.DataFrame,
     t_model_init_days: float,
     vmax: float,
     dfelabundances: Optional[pd.DataFrame] = None,
     dfgridcontributions: Optional[pd.DataFrame] = None,
     nradialbins: Optional[int] = None,
 ) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
-    """Convert 3D Cartesian grid model to 1D spherical"""
+    """Convert 3D Cartesian grid model to 1D spherical."""
     t_model_init_seconds = t_model_init_days * 24 * 60 * 60
     xmax = vmax * t_model_init_seconds
     ngridpoints = len(dfmodel)
     ncoordgridx = round(ngridpoints ** (1.0 / 3.0))
     wid_init = 2 * xmax / ncoordgridx
 
     print(f"Spherically averaging 3D model with {ngridpoints} cells...")
     timestart = time.perf_counter()
 
     # dfmodel = dfmodel.query('rho > 0.').copy()
     dfmodel = dfmodel.copy()
     celldensity = dict(dfmodel[["inputcellid", "rho"]].itertuples(index=False))
 
-    dfmodel = add_derived_cols_to_modeldata(
-        dfmodel, ["velocity"], dimensions=3, t_model_init_seconds=t_model_init_seconds, wid_init=wid_init
-    )
+    for ax in ["x", "y", "z"]:
+        dfmodel[f"vel_{ax}_mid"] = (dfmodel[f"pos_{ax}_min"] + (0.5 * wid_init)) / t_model_init_seconds
+
+    dfmodel["vel_r_mid"] = np.sqrt(dfmodel["vel_x_mid"] ** 2 + dfmodel["vel_y_mid"] ** 2 + dfmodel["vel_z_mid"] ** 2)
     # print(dfmodel)
     # print(dfelabundances)
     km_to_cm = 1e5
     if nradialbins is None:
         nradialbins = int(ncoordgridx / 2.0)
     velocity_bins = [vmax * n / nradialbins for n in range(nradialbins + 1)]  # cm/s
     outcells = []
@@ -1051,16 +1089,15 @@
 
 def scale_model_to_time(
     dfmodel: pd.DataFrame,
     targetmodeltime_days: float,
     t_model_days: Optional[float] = None,
     modelmeta: Optional[dict[str, Any]] = None,
 ) -> tuple[pd.DataFrame, Optional[dict[str, Any]]]:
-    """Homologously expand model to targetmodeltime_days, reducing density and adjusting position columns to match"""
-
+    """Homologously expand model to targetmodeltime_days, reducing density and adjusting position columns to match."""
     if t_model_days is None:
         assert modelmeta is not None
         t_model_days = modelmeta["t_model_days"]
 
     timefactor = targetmodeltime_days / t_model_days
 
     print(
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/lapuente.py` & `artistools-2023.5.16/artistools/inputmodel/lapuente.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/makeartismodel.py` & `artistools-2023.5.16/artistools/inputmodel/makeartismodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=[], nargs="*", action=at.AppendPath, help="Path to initial model file")
 
     parser.add_argument(
         "--downscale3dgrid", action="store_true", help="Downscale a 3D ARTIS model to smaller grid size"
     )
 
-    parser.add_argument("-inputgridsize", default=200, help="Size of big model grid for downscale script")
+    parser.add_argument("-inputgridsize", default=200, type=int, help="Size of big model grid for downscale script")
 
-    parser.add_argument("-outputgridsize", default=50, help="Size of small model grid for downscale script")
+    parser.add_argument("-outputgridsize", default=50, type=int, help="Size of small model grid for downscale script")
 
     parser.add_argument(
         "--makemodelfromgriddata", action="store_true", help="Make ARTIS model files from arepo grid.dat file"
     )
 
     parser.add_argument("-pathtogriddata", default=".", help="Path to arepo grid.dat file")
 
@@ -43,52 +43,46 @@
         "-modeldim", type=int, default=None, help="Choose how many dimensions input model has. 1, 2 or 3"
     )
 
     parser.add_argument("-outputpath", "-o", default=".", help="Folder for output")
 
 
 def main(args=None, argsraw=None, **kwargs):
-    """Called with makeartismodel. Tools to create an ARTIS input model"""
+    """Tools to create an ARTIS input model."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Make ARTIS input model"
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = [Path(".")]
     elif isinstance(args.modelpath, (str, Path)):
         args.modelpath = [args.modelpath]
 
     args.modelpath = at.flatten_list(args.modelpath)
 
     if args.downscale3dgrid:
         at.inputmodel.downscale3dgrid.make_downscaled_3d_grid(
-            modelpath=Path(args.modelpath[0]), inputgridsize=args.inputgridsize, outputgridsize=args.outputgridsize
+            modelpath=Path(args.modelpath[0]), outputgridsize=args.outputgridsize
         )
         return
 
     if args.makemodelfromgriddata:
         print(args)
         at.inputmodel.modelfromhydro.makemodelfromgriddata(
             gridfolderpath=args.pathtogriddata, outputpath=args.modelpath[0], args=args
         )
 
     if args.makeenergyinputfiles:
-        model, t_model, vmax = at.inputmodel.get_modeldata_tuple(args.modelpath[0])
-        if args.modeldim == 1:
-            rho = 10 ** model["logrho"]
-            Mtot_grams = model["cellmass_grams"].sum()
-
-        else:
-            rho = model["rho"]
-            Mtot_grams = model["cellmass_grams"].sum()
-        print(f"total mass { Mtot_grams / 1.989e33} Msun")
+        model, _ = at.inputmodel.get_modeldata(args.modelpath[0])
+        rho = 10 ** model["logrho"] if args.modeldim == 1 else model["rho"]
+        Mtot_grams = model["cellmass_grams"].sum()
+
+        print(f"total mass {Mtot_grams / 1.989e33} Msun")
 
         at.inputmodel.energyinputfiles.make_energy_files(rho, Mtot_grams, outputpath=args.outputpath)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/maketardismodelfromartis.py` & `artistools-2023.5.16/artistools/inputmodel/maketardismodelfromartis.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 
     parser.add_argument("-maxatomicnumber", default=92, help="Maximum atomic number for elemental abundances")
 
     parser.add_argument("-outputpath", "-o", default=".", help="Path of output TARDIS model file")
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Convert an ARTIS format model to TARDIS format."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Convert an ARTIS format model to TARDIS format."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     temperature = args.temperature
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/map_1d_to_3d_grid.py` & `artistools-2023.5.16/artistools/inputmodel/map_1d_to_3d_grid.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/maptogrid.py` & `artistools-2023.5.16/artistools/inputmodel/maptogrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,18 +431,19 @@
         default=1,
         help="Randomly sample particles, reducing the number by this factor (e.g. 2 will ignore half of the particles)",
     )
     parser.add_argument("-outputfolderpath", "-o", default=".", help="Path for output files")
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Map tracer particle trajectories to a Cartesian grid."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Map tracer particle trajectories to a Cartesian grid.",
+            description=__doc__,
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/modelfromhydro.py` & `artistools-2023.5.16/artistools/inputmodel/modelfromhydro.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,19 +423,18 @@
     )
     parser.add_argument(
         "-targetmodeltime_days", "-t", type=float, default=1.0, help="Time in days for the output model snapshot"
     )
     parser.add_argument("-outputpath", "-o", default=None, help="Path for output model files")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Create ARTIS format model from grid.dat."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Create ARTIS format model from grid.dat."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     pd.options.mode.copy_on_write = True
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/opacityinputfile.py` & `artistools-2023.5.16/artistools/inputmodel/opacityinputfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         fopacity.write(f"{ngrid}\n")
 
         for cellid, opacity in enumerate(cell_opacities):
             fopacity.write(f"{cellid+1}    {opacity}\n")
 
 
 def opacity_by_Ye(outputfilepath, griddata):
-    """Opacities from Table 1 Tanaka 2020"""
+    """Opacities from Table 1 Tanaka 2020."""
     griddata = pd.DataFrame(griddata)
     print("Getting opacity kappa from Ye")
 
     cell_opacities = np.zeros_like(griddata["cellYe"])
 
     for index, Ye in enumerate(griddata["cellYe"]):
         if Ye == 0.0 and griddata["rho"][index] == 0:
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/plotdensity.py` & `artistools-2023.5.16/artistools/inputmodel/plotdensity.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,20 @@
         nargs="*",
         action=at.AppendPath,
         help="Path(s) to model.txt file(s) or folders containing model.txt)",
     )
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Plot the radial density profile of an ARTIS model."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Plot the radial density profile of an ARTIS model",
+            description=__doc__,
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/recombinationenergy.py` & `artistools-2023.5.16/artistools/inputmodel/recombinationenergy.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/rprocess_from_trajectory.py` & `artistools-2023.5.16/artistools/inputmodel/rprocess_from_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     if not tarfilepath.is_file():
         tarfilepath = Path(traj_root, f"{particleid}.tar.xz")
 
     if memberfilename.endswith(".dat") and not path_extracted_file.is_file():
         tarfile.open(tarfilepath, "r:*").extract(path=Path(traj_root, str(particleid)), member=memberfilename)
 
     if path_extracted_file.is_file():
-        return open(path_extracted_file, encoding="utf-8")
+        return open(path_extracted_file, encoding="utf-8")  # noqa: SIM115
 
     if not tarfilepath.is_file():
         print(f"No network data found for particle {particleid} (so can't access {memberfilename})")
         raise FileNotFoundError
 
     # print(f"using {tarfilepath} for {memberfilename}")
     # return tarfile.open(tarfilepath, "r:*").extractfile(member=memberfilename)
@@ -81,51 +81,50 @@
 
     return dfevol
 
 
 def get_closest_network_timestep(
     traj_root: Path, particleid: int, timesec: float, cond: Literal["lessthan", "greaterthan", "nearest"] = "nearest"
 ) -> int:
+    """cond:
+    'lessthan': find highest timestep less than time_sec
+    'greaterthan': find lowest timestep greater than time_sec.
     """
-    cond:
-        'lessthan': find highest timestep less than time_sec
-        'greaterthan': find lowest timestep greater than time_sec
-    """
-    dfevol: pd.DataFrame = get_dfevol(traj_root, particleid)
+    dfevol = get_dfevol(traj_root, particleid)
 
     if cond == "nearest":
         idx = np.abs(dfevol.timesec.to_numpy() - timesec).argmin()
 
     elif cond == "greaterthan":
-        return dfevol.query("timesec > @timesec").nstep.min()
+        return dfevol.query("timesec > @timesec")["nstep"].min()
 
     elif cond == "lessthan":
-        return dfevol.query("timesec < @timesec").nstep.max()
+        return dfevol.query("timesec < @timesec")["nstep"].max()
 
     else:
         raise AssertionError
 
-    nts: int = dfevol.nstep.to_numpy()[idx]
+    nts: int = dfevol["nstep"].to_numpy()[idx]
 
     return nts
 
 
 def get_trajectory_timestepfile_nuc_abund(
     traj_root: Path, particleid: int, memberfilename: str
 ) -> tuple[pd.DataFrame, float]:
-    """
-    get the nuclear abundances for a particular trajectory id number and time
-    memberfilename should be something like "./Run_rprocess/tday_nz-plane"
+    """Get the nuclear abundances for a particular trajectory id number and time
+    memberfilename should be something like "./Run_rprocess/tday_nz-plane".
     """
     with open_tar_file_or_extracted(traj_root, particleid, memberfilename) as trajfile:
         try:
             _, str_t_model_init_seconds, _, rho, _, _ = trajfile.readline().split()
         except ValueError as exc:
             print(f"Problem with {memberfilename}")
-            raise ValueError(f"Problem with {memberfilename}") from exc
+            msg = f"Problem with {memberfilename}"
+            raise ValueError(msg) from exc
 
         trajfile.seek(0)
         t_model_init_seconds = float(str_t_model_init_seconds)
 
         dfnucabund = pd.read_fwf(
             trajfile,
             skip_blank_lines=True,
@@ -208,15 +207,16 @@
         if nts is not None:
             memberfilename = f"./Run_rprocess/nz-plane{nts:05d}"
         elif t_model_s is not None:
             # find the closest timestep to the required time
             nts = get_closest_network_timestep(traj_root, particleid, t_model_s)
             memberfilename = f"./Run_rprocess/nz-plane{nts:05d}"
         else:
-            raise ValueError("Either t_model_s or nts must be specified")
+            msg = "Either t_model_s or nts must be specified"
+            raise ValueError(msg)
 
         dftrajnucabund, traj_time_s = get_trajectory_timestepfile_nuc_abund(traj_root, particleid, memberfilename)
 
         if t_model_s is None:
             t_model_s = traj_time_s
 
     except FileNotFoundError:
@@ -417,15 +417,15 @@
 
     listcellnucabundances = []
     print("Reading trajectory abundances...")
     timestart = time.perf_counter()
     trajworker = partial(get_trajectory_abund_q, t_model_s=t_model_s, traj_root=traj_root, getqdotintegral=True)
 
     if at.get_config()["num_processes"] > 1:
-        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             list_traj_nuc_abund = pool.map(trajworker, dfcontribs_particlegroups.groups)
             pool.close()
             pool.join()
     else:
         list_traj_nuc_abund = [trajworker(particleid) for particleid in dfcontribs_particlegroups.groups]
 
     n_missing_particles = len([d for d in list_traj_nuc_abund if not d])
@@ -443,15 +443,15 @@
     print("Generating cell abundances...")
     timestart = time.perf_counter()
     dfcontribs_cellgroups = dfcontribs.groupby("cellindex")
     cellabundworker = partial(get_modelcellabundance, dict_traj_nuc_abund, minparticlespercell)
 
     if at.get_config()["num_processes"] > 1:
         chunksize = math.ceil(len(dfcontribs_cellgroups) / at.get_config()["num_processes"])
-        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             listcellnucabundances = pool.map(cellabundworker, dfcontribs_cellgroups, chunksize=chunksize)
             pool.close()
             pool.join()
     else:
         listcellnucabundances = [cellabundworker(cellgroup) for cellgroup in dfcontribs_cellgroups]
 
     listcellnucabundances = [x for x in listcellnucabundances if x is not None]
@@ -517,18 +517,19 @@
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Create ARTIS model from single trajectory abundances."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Create ARTIS model from single trajectory abundances.",
+            description=__doc__,
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/rprocess_solar.py` & `artistools-2023.5.16/artistools/inputmodel/rprocess_solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import artistools as at
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Create solar r-process pattern in ARTIS format."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Create solar r-process pattern in ARTIS format."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     dfsolarabund = pd.read_csv(
         at.get_config()["path_datadir"] / "solar_r_abundance_pattern.txt", delim_whitespace=True, comment="#"
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/scalevelocity.py` & `artistools-2023.5.16/artistools/inputmodel/scalevelocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,19 @@
             "cellmass_grams = 10 ** logrho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
             "* (1e5 * @t_model_init_seconds) ** 3"
         ),
     )
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Scale the velocity of an ARTIS model, keeping mass constant and saving back to ARTIS format."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Scale the velocity of an ARTIS model, keeping mass constant and saving back to ARTIS format.",
+            description=__doc__,
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     dfmodel, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(args.inputfile)
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/shen2018.py` & `artistools-2023.5.16/artistools/inputmodel/shen2018.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-inputpath", "-i", default="1.00_5050.dat", help="Path of input file")
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
+    """Convert Shen et al. 2018 models to ARTIS format."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Convert Shen et al. 2018 models to ARTIS format."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     with open(args.inputpath) as infile:
         columns = infile.readline().split()
```

### Comparing `artistools-2023.4.19.2/artistools/inputmodel/slice1Dfromconein3dmodel.py` & `artistools-2023.5.16/artistools/inputmodel/slice1Dfromconein3dmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,19 @@
         action="store",
         default=True,
         help="Make 1D model from cone around axis. Default is True.If False uses points along axis.",
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Make 1D model from cone in 3D model."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description='Make 1D model from cone in 3D model. Call with "makeartismodel1dslicefromcone"',
+            description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = [Path(".")]
@@ -221,14 +222,15 @@
     args.other_axis2 = None
     axes = ["x", "y", "z"]
     for ax in axes:
         if args.other_axis1 is None and ax != args.sliceaxis:
             args.other_axis1 = ax
         elif args.other_axis2 is None and ax != args.sliceaxis:
             args.other_axis2 = ax
+
     # remember: models before scaling down to artis input have x and z axis swapped compared to artis input files
 
     make_1D_model_files(args)
 
     # make_plot(args) # Uncomment to make 3D plot todo: add command line option
```

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/__init__.py` & `artistools-2023.5.16/artistools/lightcurve/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/lightcurve.py` & `artistools-2023.5.16/artistools/lightcurve/lightcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import artistools as at
 
 
 def readfile(
     filepath: Union[str, Path],
 ) -> dict[int, pd.DataFrame]:
-    """Read an ARTIS light curve file"""
+    """Read an ARTIS light curve file."""
     print(f"Reading {filepath}")
     lcdata: dict[int, pd.DataFrame] = {}
     if "_res" in str(filepath):
         # get a dict of dfs with light curves at each viewing direction bin
         lcdata_res = pl.read_csv(
             at.zopen(filepath, "rb").read(), separator=" ", has_header=False, new_columns=["time", "lum", "lum_cmf"]
         )
@@ -60,21 +60,22 @@
     return res_data
 
 
 def get_from_packets(
     modelpath: Union[str, Path],
     escape_type: Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
     maxpacketfiles: Optional[int] = None,
-    directionbins: Collection[int] = [-1],
+    directionbins: Optional[Collection[int]] = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     get_cmf_column: bool = True,
 ) -> dict[int, pl.DataFrame]:
-    """Get ARTIS luminosity vs time from packets files"""
-
+    """Get ARTIS luminosity vs time from packets files."""
+    if directionbins is None:
+        directionbins = [-1]
     tmidarray = at.get_timestep_times_float(modelpath=modelpath, loc="mid")
     timearray = at.get_timestep_times_float(modelpath=modelpath, loc="start")
     arr_timedelta = at.get_timestep_times_float(modelpath=modelpath, loc="delta")
     # timearray = np.arange(250, 350, 0.1)
     if get_cmf_column:
         _, modelmeta = at.inputmodel.get_modeldata(modelpath, getheadersonly=True, printwarningsonly=True)
         escapesurfacegamma = math.sqrt(1 - (modelmeta["vmax_cmps"] / 29979245800) ** 2)
@@ -104,14 +105,15 @@
     if directionbins != [-1]:
         if average_over_phi:
             getcols.append("costhetabin")
         elif average_over_theta:
             getcols.append("phibin")
         else:
             getcols.append("dirbin")
+
     dfpackets = dfpackets.select(getcols).collect(streaming=True).lazy()
 
     lcdata = {}
     for dirbin in directionbins:
         if dirbin == -1:
             solidanglefactor = 1.0
             pldfpackets_dirbin = dfpackets
@@ -129,19 +131,23 @@
         dftimebinned = at.packets.bin_and_sum(
             pldfpackets_dirbin,
             bincol="t_arrive_d",
             bins=list(timearrayplusend),
             sumcols=["e_rf"],
         )
 
-        arr_lum = (
-            dftimebinned["e_rf_sum"] / nprocs_read * solidanglefactor * (u.erg / u.day).to("solLum")
-        ) / arr_timedelta
+        unitfactor = float((u.erg / u.day).to("solLum"))
+        dftimebinned = dftimebinned.with_columns(
+            [
+                pl.Series(name="time", values=tmidarray),
+                ((pl.col("e_rf_sum") / nprocs_read * solidanglefactor * unitfactor) / arr_timedelta).alias("lum"),
+            ]
+        ).drop(["e_rf_sum", "t_arrive_d_bin"])
 
-        lcdata[dirbin] = pl.DataFrame({"time": tmidarray, "lum": arr_lum})
+        lcdata[dirbin] = dftimebinned
 
         if get_cmf_column:
             dftimebinned_cmf = at.packets.bin_and_sum(
                 pldfpackets_dirbin,
                 bincol="t_arrive_cmf_d",
                 bins=list(timearrayplusend),
                 sumcols=["e_cmf"],
@@ -164,18 +170,18 @@
 
 def generate_band_lightcurve_data(
     modelpath: Path,
     args: argparse.Namespace,
     angle: int = -1,
     modelnumber: Optional[int] = None,
 ) -> dict:
-    """Method adapted from https://github.com/cinserra/S3/blob/master/src/s3/SMS.py"""
+    """Method adapted from https://github.com/cinserra/S3/blob/master/src/s3/SMS.py."""
     from scipy.interpolate import interp1d
 
-    if args.plotvspecpol and os.path.isfile(modelpath / "vpkt.txt"):
+    if args.plotvspecpol and (modelpath / "vpkt.txt").is_file():
         print("Found vpkt.txt, using virtual packets")
         stokes_params = (
             at.spectra.get_vspecpol_data(vspecangle=angle, modelpath=modelpath)
             if angle >= 0
             else at.spectra.get_specpol_data(angle=angle, modelpath=modelpath)
         )
         vspecdata = stokes_params["I"]
@@ -312,16 +318,15 @@
 
     return times, magnitudes
 
 
 def get_filter_data(
     filterdir: Union[Path, str], filter_name: str
 ) -> tuple[float, np.ndarray, np.ndarray, float, float]:
-    """Filter data in 'data/filters' taken from https://github.com/cinserra/S3/tree/master/src/s3/metadata"""
-
+    """Filter data in 'data/filters' taken from https://github.com/cinserra/S3/tree/master/src/s3/metadata."""
     with Path(filterdir, filter_name + ".txt").open("r") as filter_metadata:  # defintion of the file
         line_in_filter_metadata = filter_metadata.readlines()  # list of lines
 
     zeropointenergyflux = float(line_in_filter_metadata[0])
     # zero point in energy flux (erg/cm^2/s)
 
     wavefilter, transmission = [], []
```

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/plotlightcurve.py` & `artistools-2023.5.16/artistools/lightcurve/plotlightcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # PYTHON_ARGCOMPLETE_OK
 import argparse
 import math
-import multiprocessing
 import os
 import sys
 from collections.abc import Iterable
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any
 from typing import Literal
@@ -24,15 +23,21 @@
 
 import artistools as at
 
 color_list = list(plt.get_cmap("tab20")(np.linspace(0, 1.0, 20)))
 
 
 def plot_deposition_thermalisation(axis, axistherm, modelpath, modelname, plotkwargs, args) -> None:
-    axistherm.set_xscale("log")
+    if args.logscalex:
+        axistherm.set_xscale("log")
+
+    # if args.logscaley:
+    #     axistherm.set_yscale("log")
+    #     axistherm.set_ylim(bottom=0.1, top=1.0)
+
     if args.plotthermalisation:
         dfmodel, modelmeta = at.inputmodel.get_modeldata(
             modelpath, skipnuclidemassfraccolumns=True, derived_cols=["vel_r_mid"], dtype_backend="pyarrow"
         )
 
         t_model_init_days = modelmeta["t_model_init_days"]
         vmax_cmps = modelmeta["vmax_cmps"]
@@ -63,23 +68,24 @@
     #         plotkwargs, **{
     #             'label': plotkwargs['label'] + r' $\dot{E}_{dep}/\dot{E}_{rad}$',
     #             'linestyle': 'solid',
     #             'color': color_total,
     #         }))
 
     color_gamma = next(axis._get_lines.prop_cycler)["color"]
+    color_gamma = next(axis._get_lines.prop_cycler)["color"]
 
     # axis.plot(depdata['tmid_days'], depdata['eps_gamma_Lsun'] * 3.826e33, **dict(
     #     plotkwargs, **{
     #         'label': plotkwargs['label'] + r' $\dot{E}_{rad,\gamma}$',
     #         'linestyle': 'dashed',
     #         'color': color_gamma,
     #     }))
 
-    gammadep_lsun = depdata["gammadeppathint_Lsun"] if "gammadeppathint_Lsun" in depdata else depdata["gammadep_Lsun"]
+    gammadep_lsun = depdata["gammadep_Lsun"]
 
     axis.plot(
         depdata["tmid_days"],
         gammadep_lsun * 3.826e33,
         **{
             **plotkwargs,
             "label": plotkwargs["label"] + r" $\dot{E}_{dep,\gamma}$",
@@ -112,15 +118,15 @@
                 "linestyle": "dashed",
                 "color": color_beta,
             },
         )
 
     c23modelpath = Path(
         "/Users/luke/Library/CloudStorage/GoogleDrive-luke@lukeshingles.com/Shared"
-        " drives/ARTIS/artis_runs_published/Collinsetal2023-KN/sfho_long_1-35-135Msun"
+        " drives/ARTIS/artis_runs_published/Collinsetal2023/sfho_long_1-35-135Msun"
     )
 
     c23energyrate = at.inputmodel.energyinputfiles.get_energy_rate_fromfile(c23modelpath)
     c23etot, c23energydistribution_data = at.inputmodel.energyinputfiles.get_etot_fromfile(c23modelpath)
 
     dE = np.diff(c23energyrate["rate"] * c23etot)
     dt = np.diff(c23energyrate["times"] * 24 * 60 * 60)
@@ -158,15 +164,15 @@
     #         'label': plotkwargs['label'] + r' $\dot{E}_{dep,\alpha}$',
     #         'linestyle': 'dotted',
     #         'color': color_alpha,
     #     }))
     if args.plotthermalisation:
         axistherm.plot(
             depdata["tmid_days"],
-            depdata["gammadeppathint_Lsun"] / depdata["eps_gamma_Lsun"],
+            depdata["gammadep_Lsun"] / depdata["eps_gamma_Lsun"],
             **{**plotkwargs, "label": modelname + r" $f_\gamma$", "linestyle": "solid", "color": color_gamma},
         )
 
         axistherm.plot(
             depdata["tmid_days"],
             depdata["elecdep_Lsun"] / depdata["eps_elec_Lsun"],
             **{
@@ -174,18 +180,17 @@
                 "label": modelname + r" $f_\beta$",
                 "linestyle": "solid",
                 "color": color_beta,
             },
         )
 
         f_alpha = depdata["alphadep_Lsun"] / depdata["eps_alpha_Lsun"]
-        kernel_size = 5
-        if len(f_alpha) > kernel_size:
-            kernel = np.ones(kernel_size) / kernel_size
-            f_alpha = np.convolve(f_alpha, kernel, mode="same")
+        import scipy.signal
+
+        f_alpha = scipy.signal.savgol_filter(f_alpha, 9, 3, mode="interp")
         axistherm.plot(
             depdata["tmid_days"],
             f_alpha,
             **{**plotkwargs, "label": modelname + r" $f_\alpha$", "linestyle": "solid", "color": color_alpha},
         )
 
         ejecta_ke: float
@@ -200,41 +205,45 @@
 
         # velocity derived from ejecta kinetic energy to match Barnes et al. (2016) Section 2.1
         ejecta_v = np.sqrt(2 * ejecta_ke / (model_mass_grams * 1e-3))
         v2 = ejecta_v / (0.2 * 299792458)
         print(f"  Barnes average ejecta velocity: {ejecta_v / 299792458:.2f}c")
         m5 = model_mass_grams / (5e-3 * 1.989e33)  # M / (5e-3 Msun)
 
-        t_ineff_gamma = 0.5 * np.sqrt(m5) / v2
-        barnes_f_gamma = [1 - math.exp(-((t / t_ineff_gamma) ** -2)) for t in depdata["tmid_days"].to_numpy()]
+        # Barnes et al (2016) scaling form from equation 17, with fiducial t_ineff_gamma of 1.4 days
+        t_ineff_gamma = 1.4 * np.sqrt(m5) / v2
+        # Barnes et al (2016) equation 33
+        barnes_f_gamma = [1 - math.exp(-((t / t_ineff_gamma) ** -2)) for t in depdata["tmid_days"]]
 
         axistherm.plot(
             depdata["tmid_days"],
             barnes_f_gamma,
             **{**plotkwargs, "label": r"Barnes+16 $f_\gamma$", "linestyle": "dashed", "color": color_gamma},
         )
 
         e0_beta_mev = 0.5
+        # Barnes et al (2016) equation 20
         t_ineff_beta = 7.4 * (e0_beta_mev / 0.5) ** -0.5 * m5**0.5 * (v2 ** (-3.0 / 2))
+        # Barnes et al (2016) equation 32
         barnes_f_beta = [
-            math.log(1 + 2 * (t / t_ineff_beta) ** 2) / (2 * (t / t_ineff_beta) ** 2)
-            for t in depdata["tmid_days"].to_numpy()
+            math.log(1 + 2 * (t / t_ineff_beta) ** 2) / (2 * (t / t_ineff_beta) ** 2) for t in depdata["tmid_days"]
         ]
 
         axistherm.plot(
             depdata["tmid_days"],
             barnes_f_beta,
             **{**plotkwargs, "label": r"Barnes+16 $f_\beta$", "linestyle": "dashed", "color": color_beta},
         )
 
         e0_alpha_mev = 6.0
+        # Barnes et al (2016) equation 25 times equation 16 for t_peak
         t_ineff_alpha = 4.3 * 1.8 * (e0_alpha_mev / 6.0) ** -0.5 * m5**0.5 * (v2 ** (-3.0 / 2))
+        # Barnes et al (2016) equation 32
         barnes_f_alpha = [
-            math.log(1 + 2 * (t / t_ineff_alpha) ** 2) / (2 * (t / t_ineff_alpha) ** 2)
-            for t in depdata["tmid_days"].to_numpy()
+            math.log(1 + 2 * (t / t_ineff_alpha) ** 2) / (2 * (t / t_ineff_alpha) ** 2) for t in depdata["tmid_days"]
         ]
 
         axistherm.plot(
             depdata["tmid_days"],
             barnes_f_alpha,
             **{**plotkwargs, "label": r"Barnes+16 $f_\alpha$", "linestyle": "dashed", "color": color_alpha},
         )
@@ -245,15 +254,15 @@
     axis,
     lcindex: int = 0,
     label: Optional[str] = None,
     escape_type: Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
     frompackets: bool = False,
     maxpacketfiles: Optional[int] = None,
     axistherm=None,
-    directionbins: Sequence[int] = [-1],
+    directionbins: Optional[Sequence[int]] = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     args=None,
 ) -> Optional[pd.DataFrame]:
     lcfilename = None
     modelpath = Path(modelpath)
     if Path(modelpath).is_file():  # handle e.g. modelpath = 'modelpath/light_curve.out'
@@ -457,15 +466,15 @@
     )
 
     if args.plotthermalisation:
         figtherm, axistherm = plt.subplots(
             nrows=1,
             ncols=1,
             sharex=True,
-            figsize=(args.figscale * at.get_config()["figwidth"] * 1.4, args.figscale * at.get_config()["figwidth"]),
+            figsize=(args.figscale * at.get_config()["figwidth"] * 1.6, args.figscale * at.get_config()["figwidth"]),
             tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
         )
     else:
         axistherm = None
 
     # take any assigned colours our of the cycle
     colors = [
@@ -1523,18 +1532,17 @@
 
     parser.add_argument("-ncolslegend", type=int, default=1, help="Number of columns in legend")
 
     parser.add_argument("--legendframeon", action="store_true", help="Frame on in legend")
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Plot ARTIS light curve."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS light curve."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
         if args.average_every_tenth_viewing_angle:
             print("WARNING: --average_every_tenth_viewing_angle is deprecated. use --average_over_phi_angle instead")
             args.average_over_phi_angle = True
@@ -1626,9 +1634,8 @@
             escape_type=args.escape_type,
             maxpacketfiles=args.maxpacketfiles,
             args=args,
         )
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/test_lightcurve.py` & `artistools-2023.5.16/artistools/lightcurve/test_lightcurve.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 @mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
 def test_lightcurve_plot(mockplot) -> None:
     at.lightcurve.plot(argsraw=[], modelpath=[modelpath], outputfile=outputpath, frompackets=False)
 
     arr_time_d = np.array(mockplot.call_args[0][1])
     arr_lum = np.array(mockplot.call_args[0][2])
 
-    assert np.isclose(arr_time_d.min(), 250.421, rtol=1e-4)
-    assert np.isclose(arr_time_d.max(), 349.412, rtol=1e-4)
+    assert np.isclose(arr_time_d.min(), 257.253, rtol=1e-4)
+    assert np.isclose(arr_time_d.max(), 333.334, rtol=1e-4)
 
-    assert np.isclose(arr_time_d.mean(), 297.20121, rtol=1e-4)
-    assert np.isclose(arr_time_d.std(), 28.83886, rtol=1e-4)
+    assert np.isclose(arr_time_d.mean(), 293.67411, rtol=1e-4)
+    assert np.isclose(arr_time_d.std(), 22.2348791, rtol=1e-4)
 
     integral = np.trapz(arr_lum, arr_time_d)
-    assert np.isclose(integral, 2.7955e42, rtol=1e-2)
+    assert np.isclose(integral, 2.4189054554e42, rtol=1e-2)
 
-    assert np.isclose(arr_lum.mean(), 2.8993e40, rtol=1e-4)
-    assert np.isclose(arr_lum.std(), 1.1244e40, rtol=1e-4)
+    assert np.isclose(arr_lum.mean(), 3.231155e40, rtol=1e-4)
+    assert np.isclose(arr_lum.std(), 7.2115e39, rtol=1e-4)
 
 
 @mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
 def test_lightcurve_plot_frompackets(mockplot) -> None:
     at.lightcurve.plot(
         argsraw=[],
         modelpath=modelpath,
         frompackets=True,
         outputfile=Path(outputpath, "lightcurve_from_packets.pdf"),
     )
 
     arr_time_d = np.array(mockplot.call_args[0][1])
     arr_lum = np.array(mockplot.call_args[0][2])
 
-    assert np.isclose(arr_time_d.min(), 250.421, rtol=1e-4)
-    assert np.isclose(arr_time_d.max(), 349.412, rtol=1e-4)
+    assert np.isclose(arr_time_d.min(), 257.253, rtol=1e-4)
+    assert np.isclose(arr_time_d.max(), 333.33389, rtol=1e-4)
 
-    assert np.isclose(arr_time_d.mean(), 297.20121, rtol=1e-4)
-    assert np.isclose(arr_time_d.std(), 28.83886, rtol=1e-4)
+    assert np.isclose(arr_time_d.mean(), 293.67411, rtol=1e-4)
+    assert np.isclose(arr_time_d.std(), 22.23483, rtol=1e-4)
 
     integral = np.trapz(arr_lum, arr_time_d)
 
-    assert np.isclose(integral, 1.0795078026708302e41, rtol=1e-2)
+    assert np.isclose(integral, 9.0323767e40, rtol=1e-2)
 
-    assert np.isclose(arr_lum.mean(), 1.1176e39, rtol=1e-4)
-    assert np.isclose(arr_lum.std(), 4.4820e38, rtol=1e-4)
+    assert np.isclose(arr_lum.mean(), 1.2033423e39, rtol=1e-4)
+    assert np.isclose(arr_lum.std(), 3.6121162e38, rtol=1e-4)
 
 
 def test_band_lightcurve_plot() -> None:
     at.lightcurve.plot(argsraw=[], modelpath=modelpath, filter=["B"], outputfile=outputpath)
 
 
 def test_band_lightcurve_subplots() -> None:
```

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/viewingangleanalysis.py` & `artistools-2023.5.16/artistools/lightcurve/viewingangleanalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
             + str(band_name)
             + "_band_deltam15 ",
             comments="",
         )
 
 
 def calculate_peak_time_mag_deltam15(time, magnitude, modelname, angle, key, args, filternames_conversion_dict=None):
-    """Calculating band peak time, peak magnitude and delta m15"""
+    """Calculate band peak time, peak magnitude and delta m15."""
     if args.timemin is None or args.timemax is None:
         print(
             "Trying to calculate peak time / dm15 / rise time with no time range. "
             "This will give a stupid result. Specify args.timemin and args.timemax"
         )
         sys.exit(1)
     print(
@@ -283,15 +283,15 @@
         "The --test_viewing_angle_fit flag will allow you to check the fitting is "
         "behaving as expected. In general fitting over a smaller region of the    "
         "light curve tends to produce better fits."
     )
     fxfit, xfit = lightcurve_polyfit(time, magnitude, args)
 
     def match_closest_time_polyfit(reftime_polyfit):
-        return str("{}".format(min([float(x) for x in xfit], key=lambda x: abs(x - reftime_polyfit))))
+        return str(f"{min([float(x) for x in xfit], key=lambda x: abs(x - reftime_polyfit))}")
 
     index_min = np.argmin(fxfit)
     tmax_polyfit = xfit[index_min]
     time_after15days_polyfit = match_closest_time_polyfit(tmax_polyfit + 15)
     if args.include_delta_m40:
         time_after40days_polyfit = match_closest_time_polyfit(tmax_polyfit + 40)
     for ii, xfits in enumerate(xfit):
```

### Comparing `artistools-2023.4.19.2/artistools/lightcurve/writebollightcurvedata.py` & `artistools-2023.5.16/artistools/lightcurve/writebollightcurvedata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from astropy import units as u
 
 import artistools as at
 
 
 def get_bol_lc_from_spec(modelpath):
     res_specdata = at.spectra.read_spec_res(modelpath)
-    # print(res_specdata)
     timearray = res_specdata[0].columns.to_numpy()[1:]
     times = [time for time in timearray if 5 < float(time) < 80]
     lightcurvedata = {"time": times}
 
     for angle in range(len(res_specdata)):
         bol_luminosity = []
         for timestep, time in enumerate(timearray):
```

### Comparing `artistools-2023.4.19.2/artistools/linefluxes.py` & `artistools-2023.5.16/artistools/linefluxes.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import argparse
 import json
 import math
 import multiprocessing
 from collections import namedtuple
 from functools import partial
 from pathlib import Path
+from typing import Optional
+from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import units as u
 
@@ -35,15 +37,15 @@
     assert nprocs_read > 0
 
     model, _ = at.inputmodel.get_modeldata(modelpath)
     # vmax = model.iloc[-1].velocity_outer * u.km / u.s
     processfile = partial(get_packets_with_emtype_onefile, emtypecolumn, lineindices)
     if at.get_config()["num_processes"] > 1:
         print(f"Reading packets files with {at.get_config()['num_processes']} processes")
-        with multiprocessing.Pool(processes=at.get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             arr_dfmatchingpackets = pool.map(processfile, packetsfiles)
             pool.close()
             pool.join()
             # pool.terminate()
     else:
         arr_dfmatchingpackets = [processfile(f) for f in packetsfiles]
 
@@ -189,46 +191,46 @@
 
     lcdata = pd.DataFrame(dictlcdata)
     return lcdata
 
 
 def get_closelines(
     modelpath,
-    atomic_number,
-    ion_stage,
-    approxlambda,
-    lambdamin=-1,
-    lambdamax=-1,
-    lowerlevelindex=-1,
-    upperlevelindex=-1,
+    atomic_number: int,
+    ion_stage: int,
+    approxlambdalabel: Union[str, int],
+    lambdamin: Optional[float] = None,
+    lambdamax: Optional[float] = None,
+    lowerlevelindex: Optional[int] = None,
+    upperlevelindex: Optional[int] = None,
 ):
     dflinelist = at.get_linelist_dataframe(modelpath)
     dflinelistclosematches = dflinelist.query("atomic_number == @atomic_number and ionstage == @ion_stage").copy()
-    if lambdamin > 0:
+    if lambdamin is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamin < lambda_angstroms")
-    if lambdamax > 0:
+    if lambdamax is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamax > lambda_angstroms")
-    if lowerlevelindex >= 0:
+    if lowerlevelindex is not None:
         dflinelistclosematches = dflinelistclosematches.query("lowerlevelindex==@lowerlevelindex")
-    if upperlevelindex >= 0:
+    if upperlevelindex is not None:
         dflinelistclosematches = dflinelistclosematches.query("upperlevelindex==@upperlevelindex")
     # print(dflinelistclosematches)
 
     linelistindices = tuple(dflinelistclosematches.index.to_numpy())
     upperlevelindicies = tuple(dflinelistclosematches.upperlevelindex.to_numpy())
     lowerlevelindicies = tuple(dflinelistclosematches.lowerlevelindex.to_numpy())
     lowestlambda = dflinelistclosematches.lambda_angstroms.min()
     highestlamba = dflinelistclosematches.lambda_angstroms.max()
-    colname = f"flux_{at.get_ionstring(atomic_number, ion_stage, nospace=True)}_{approxlambda}"
-    featurelabel = f"{at.get_ionstring(atomic_number, ion_stage)} {approxlambda} Å"
+    colname = f"flux_{at.get_ionstring(atomic_number, ion_stage, nospace=True)}_{approxlambdalabel}"
+    featurelabel = f"{at.get_ionstring(atomic_number, ion_stage)} {approxlambdalabel} Å"
 
     return (
         colname,
         featurelabel,
-        approxlambda,
+        approxlambdalabel,
         linelistindices,
         lowestlambda,
         highestlamba,
         atomic_number,
         ion_stage,
         upperlevelindicies,
         lowerlevelindicies,
@@ -843,21 +845,19 @@
 
     parser.add_argument(
         "-outputfile", "-o", action="store", dest="outputfile", type=Path, help="path/filename for PDF file"
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
-    """Plot spectra from ARTIS and reference data."""
+    """Plot line fluxe ratios for comparisons to Floers."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description=(
-                "Plot ARTIS model spectra by finding spec.out files in the current directory or subdirectories."
-            ),
+            description=(__doc__),
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = [Path(".")]
@@ -877,9 +877,8 @@
     if args.plotemittingregions:
         make_emitting_regions_plot(args)
     else:
         make_flux_ratio_plot(args)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/logfiles.py` & `artistools-2023.5.16/artistools/logfiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 import argparse
-import multiprocessing
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 
 import artistools as at
 
 
@@ -127,22 +126,21 @@
         help="Path to ARTIS model folders with model.txt and abundances.txt",
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
     if args is None:
         parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Make 1D model from cone in 3D model."
+            formatter_class=at.CustomArgHelpFormatter, description="Plot durations from log files."
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = [Path(".")]
 
     # make_plot(logfiledict)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/macroatom.py` & `artistools-2023.5.16/artistools/macroatom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 import argparse
 import glob
-import multiprocessing
 import os.path
 import sys
 
 import matplotlib.pyplot as plt
 import pandas as pd
 
 import artistools as at
@@ -164,9 +163,8 @@
         if dfall is None or len(dfall) == 0:
             print("No data found")
 
     return dfall
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     sys.exit(main())
```

### Comparing `artistools-2023.4.19.2/artistools/matplotlibrc` & `artistools-2023.5.16/artistools/matplotlibrc`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pdf.fonttype: 42
 font.family: sans-serif
-font.sans-serif: Tahoma
+font.sans-serif: Tahoma, 'DejaVu Sans', 'Lucida Grande', Verdana
 #figure.constrained_layout.use: True
 # figure.figsize: 4.5, 4.
 
 savefig.format:    pdf
 
 
 #axes.formatter.useoffset: False
```

### Comparing `artistools-2023.4.19.2/artistools/misc.py` & `artistools-2023.5.16/artistools/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import gzip
 import io
 import math
 import os
 from collections import namedtuple
-from collections.abc import Collection
 from collections.abc import Iterable
 from collections.abc import Iterator
 from collections.abc import Sequence
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 from typing import Any
@@ -48,18 +47,23 @@
     "XVIII",
     "XIX",
     "XX",
 )
 
 
 class CustomArgHelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        kwargs["max_help_position"] = 39
+        super().__init__(*args, **kwargs)
+
     def add_arguments(self, actions: Iterable[argparse.Action]) -> None:
-        def my_sort(arg: Any) -> str:
-            opstr: str = arg.option_strings[0] if len(arg.option_strings) > 0 else ""
-            # chars = 'abcdefghijklmnopqrstuvwxyz-'
+        getinvocation = super()._format_action_invocation
+
+        def my_sort(action: argparse.Action) -> str:
+            opstr = getinvocation(action)
             opstr = opstr.upper().replace("-", "z")  # push dash chars below alphabet
 
             return opstr
 
         actions = sorted(actions, key=my_sort)
         super().add_arguments(actions)
 
@@ -70,15 +74,14 @@
         #     setattr(args, self.dest, [])
         if isinstance(values, Iterable):
             pathlist = getattr(args, self.dest)
             # not pathlist avoids repeated appending of the same items when called from Python
             # instead of from the command line
             if not pathlist:
                 for pathstr in values:
-                    # print(f"pathstr {pathstr}")
                     # if Path(pathstr) not in pathlist:
                     pathlist.append(Path(pathstr))
         else:
             setattr(args, self.dest, Path(values))
 
 
 def showtimesteptimes(modelpath: Optional[Path] = None, numberofcolumns: int = 5) -> None:
@@ -126,44 +129,44 @@
 
     compdf = pd.concat(rowdfs, ignore_index=True)
 
     return compdf
 
 
 def get_composition_data_from_outputfile(modelpath: Path) -> pd.DataFrame:
-    """Read ion list from output file"""
+    """Read ion list from output file."""
     atomic_composition = {}
 
-    output = open(modelpath / "output_0-0.txt").read().splitlines()
-    Z: Optional[int] = None
-    ioncount = 0
-    for row in output:
-        if row.split()[0] == "[input.c]":
-            split_row = row.split()
-            if split_row[1] == "element":
-                Z = int(split_row[4])
-                ioncount = 0
-            elif split_row[1] == "ion":
-                ioncount += 1
-                assert Z is not None
-                atomic_composition[Z] = ioncount
+    with open(modelpath / "output_0-0.txt") as foutput:
+        Z: Optional[int] = None
+        ioncount = 0
+        for row in foutput:
+            if row.split()[0] == "[input.c]":
+                split_row = row.split()
+                if split_row[1] == "element":
+                    Z = int(split_row[4])
+                    ioncount = 0
+                elif split_row[1] == "ion":
+                    ioncount += 1
+                    assert Z is not None
+                    atomic_composition[Z] = ioncount
 
     composition_df = pd.DataFrame([(Z, atomic_composition[Z]) for Z in atomic_composition], columns=["Z", "nions"])
     composition_df["lowermost_ionstage"] = [1] * composition_df.shape[0]
     composition_df["uppermost_ionstage"] = composition_df["nions"]
     return composition_df
 
 
 def split_dataframe_dirbins(
     res_df: Union[pl.DataFrame, pd.DataFrame], index_of_repeated_value: int = 0, output_polarsdf: bool = False
 ) -> dict[int, Union[pd.DataFrame, pl.DataFrame]]:
-    """res files repeat output for each angle.
+    """Res files repeat output for each angle.
     index_of_repeated_value is the column index to look for repeating eg. time of ts 0.
-    In spec_res files it's 1 , but in lc_res file it's 0"""
-
+    In spec_res files it's 1 , but in lc_res file it's 0.
+    """
     if isinstance(res_df, pd.DataFrame):
         res_df = pl.from_pandas(res_df)
 
     indexes_to_split = pl.arg_where(
         res_df[:, index_of_repeated_value] == res_df[0, index_of_repeated_value], eager=True
     )
 
@@ -186,15 +189,15 @@
     return res_data
 
 
 def average_direction_bins(
     dirbindataframes: dict[int, pl.DataFrame],
     overangle: Literal["phi", "theta"],
 ) -> dict[int, pl.DataFrame]:
-    """Will average dict of direction-binned polars DataFrames according to the phi or theta angle"""
+    """Will average dict of direction-binned polars DataFrames according to the phi or theta angle."""
     dirbincount = at.get_viewingdirectionbincount()
     nphibins = at.get_viewingdirection_phibincount()
 
     assert overangle in ["phi", "theta"]
     if overangle == "phi":
         start_bin_range = range(0, dirbincount, nphibins)
     elif overangle == "theta":
@@ -220,16 +223,16 @@
         dirbindataframesout[start_bin] /= 1 + len(contribbins)  # every nth bin is the average of n bins
         print(f"bin number {start_bin} = the average of bins {[start_bin, *list(contribbins)]}")
 
     return dirbindataframesout
 
 
 def match_closest_time(reftime: float, searchtimes: list[Any]) -> str:
-    """Get time closest to reftime in list of times (searchtimes)"""
-    return str("{}".format(min([float(x) for x in searchtimes], key=lambda x: abs(x - reftime))))
+    """Get time closest to reftime in list of times (searchtimes)."""
+    return str(f"{min([float(x) for x in searchtimes], key=lambda x: abs(x - reftime))}")
 
 
 def get_vpkt_config(modelpath: Union[Path, str]) -> dict[str, Any]:
     filename = Path(modelpath, "vpkt.txt")
     vpkt_config: dict[str, Any] = {}
     with open(filename) as vpkt_txt:
         vpkt_config["nobsdirections"] = int(vpkt_txt.readline())
@@ -250,16 +253,16 @@
 
     return vpkt_config
 
 
 @lru_cache(maxsize=8)
 def get_grid_mapping(modelpath: Union[Path, str]) -> tuple[dict[int, list[int]], dict[int, int]]:
     """Return dict with the associated propagation cells for each model grid cell and
-    a dict with the associated model grid cell of each propagration cell."""
-
+    a dict with the associated model grid cell of each propagration cell.
+    """
     modelpath = Path(modelpath)
     filename = firstexisting("grid.out", tryzipped=True, folder=modelpath) if modelpath.is_dir() else Path(modelpath)
 
     assoc_cells: dict[int, list[int]] = {}
     mgi_of_propcells: dict[int, int] = {}
     with open(filename) as fgrid:
         for line in fgrid:
@@ -305,21 +308,22 @@
 
     assert xmax is not None
     wid_init = 2.0 * xmax / ncoordgridx
 
     return wid_init
 
 
-def get_syn_dir(modelpath: Path) -> Sequence[int]:
+def get_syn_dir(modelpath: Path) -> tuple[float, float, float]:
     if not (modelpath / "syn_dir.txt").is_file():
         print(f"{modelpath / 'syn_dir.txt'} does not exist. using x,y,z = 0,0,1")
-        return (0, 0, 1)
+        return (0.0, 0.0, 1.0)
 
     with open(modelpath / "syn_dir.txt") as syn_dir_file:
-        syn_dir = [int(x) for x in syn_dir_file.readline().split()]
+        x, y, z = (float(i) for i in syn_dir_file.readline().split())
+        syn_dir = (x, y, z)
 
     return syn_dir
 
 
 def vec_len(vec: Union[Sequence[float], np.ndarray[Any, np.dtype[np.float64]]]) -> float:
     return float(np.sqrt(np.dot(vec, vec)))
 
@@ -328,15 +332,15 @@
 def get_nu_grid(modelpath: Path) -> np.ndarray[Any, np.dtype[np.float64]]:
     """Get an array of frequencies at which the ARTIS spectra are binned by exspec."""
     specfilename = firstexisting(["spec.out", "specpol.out"], folder=modelpath, tryzipped=True)
     specdata = pd.read_csv(specfilename, delim_whitespace=True)
     return specdata.loc[:, "0"].to_numpy()
 
 
-def get_deposition(modelpath: Path) -> pd.DataFrame:
+def get_deposition(modelpath: Union[Path, str] = ".") -> pd.DataFrame:
     if Path(modelpath).is_file():
         depfilepath = modelpath
         modelpath = Path(modelpath).parent
     else:
         depfilepath = Path(modelpath, "deposition.out")
 
     ts_mids = get_timestep_times_float(modelpath, loc="mid")
@@ -363,15 +367,14 @@
 
 
 @lru_cache(maxsize=16)
 def get_timestep_times_float(
     modelpath: Union[Path, str], loc: Literal["mid", "start", "end", "delta"] = "mid"
 ) -> np.ndarray[Any, np.dtype[np.float64]]:
     """Return a list of the time in days of each timestep."""
-
     modelpath = Path(modelpath)
     # virtual path to code comparison workshop models
     if not modelpath.exists() and modelpath.parts[0] == "codecomparison":
         import artistools.codecomparison
 
         return artistools.codecomparison.get_timestep_times_float(modelpath=modelpath, loc=loc)
 
@@ -386,15 +389,16 @@
         if loc == "start":
             return dftimesteps.tstart_days.to_numpy()
         if loc == "end":
             return dftimesteps.tstart_days.to_numpy() + dftimesteps.twidth_days.to_numpy()
         if loc == "delta":
             return dftimesteps.twidth_days.to_numpy()
 
-        raise ValueError("loc must be one of 'mid', 'start', 'end', or 'delta'")
+        msg = "loc must be one of 'mid', 'start', 'end', or 'delta'"
+        raise ValueError(msg)
 
     # older versions of Artis always used logarithmic timesteps and didn't produce a timesteps.out file
     inputparams = get_inputparams(modelpath)
     tmin = inputparams["tmin"]
     dlogt = (math.log(inputparams["tmax"]) - math.log(tmin)) / inputparams["ntstep"]
     timesteps = range(inputparams["ntstep"])
     if loc == "mid":
@@ -406,20 +410,20 @@
     if loc == "end":
         tends = np.array([tmin * math.exp((ts + 1) * dlogt) for ts in timesteps])
         return tends
     if loc == "delta":
         tdeltas = np.array([tmin * (math.exp((ts + 1) * dlogt) - math.exp(ts * dlogt)) for ts in timesteps])
         return tdeltas
 
-    raise ValueError("loc must be one of 'mid', 'start', 'end', or 'delta'")
+    msg = "loc must be one of 'mid', 'start', 'end', or 'delta'"
+    raise ValueError(msg)
 
 
 def get_timestep_of_timedays(modelpath: Path, timedays: Union[str, float]) -> int:
     """Return the timestep containing the given time in days."""
-
     if isinstance(timedays, str):
         # could be a string like '330d'
         timedays = timedays.rstrip("d")
 
     timedays_float = float(timedays)
 
     arr_tstart = get_timestep_times_float(modelpath, loc="start")
@@ -427,15 +431,16 @@
     # to avoid roundoff errors, use the next timestep's tstart at each timestep's tend (t_width is not exact)
     arr_tend[:-1] = arr_tstart[1:]
 
     for ts, (tstart, tend) in enumerate(zip(arr_tstart, arr_tend)):
         if timedays_float >= tstart and timedays_float < tend:
             return ts
 
-    raise ValueError(f"Could not find timestep bracketing time {timedays_float}")
+    msg = f"Could not find timestep bracketing time {timedays_float}"
+    raise ValueError(msg)
 
 
 def get_time_range(
     modelpath: Path,
     timestep_range_str: Optional[str] = None,
     timemin: Optional[float] = None,
     timemax: Optional[float] = None,
@@ -494,32 +499,34 @@
         assert timemax is not None
 
         for timestep, tmid in enumerate(tmids):
             if tmid <= float(timemax):
                 timestepmax = timestep
 
         if timestepmax < timestepmin:
-            raise ValueError("Specified time range does not include any full timesteps.")
+            msg = "Specified time range does not include any full timesteps."
+            raise ValueError(msg)
     else:
-        raise ValueError("Either time or timesteps must be specified.")
+        msg = "Either time or timesteps must be specified."
+        raise ValueError(msg)
 
     timesteplast = len(tmids) - 1
     if timestepmax is not None and timestepmax > timesteplast:
         print(f"Warning timestepmax {timestepmax} > timesteplast {timesteplast}")
         timestepmax = timesteplast
     time_days_lower = float(tstarts[timestepmin])
     time_days_upper = float(tends[timestepmax])
     assert timestepmin is not None
     assert timestepmax is not None
 
     return timestepmin, timestepmax, time_days_lower, time_days_upper
 
 
 def get_timestep_time(modelpath: Union[Path, str], timestep: int) -> float:
-    """Return the time in days of the midpoint of a timestep number"""
+    """Return the time in days of the midpoint of a timestep number."""
     timearray = get_timestep_times_float(modelpath, loc="mid")
     if timearray is not None:
         return timearray[timestep]
 
     return -1
 
 
@@ -534,18 +541,24 @@
     # for 3D models, the box corners can have non-zero density (allowing packet escape from tmin)
     # for 1D and 2D, the largest escape radius at tmin is the box side radius
     vmax_tmin = cornervmax if at.inputmodel.get_dfmodel_dimensions(dfmodel) == 3 else vmax
 
     # earliest completely valid time is tmin plus maximum possible travel time from corner to origin
     validrange_start_days = at.get_timestep_times_float(modelpath, loc="start")[0] * (1 + vmax_tmin / 29979245800)
 
+    t_end = at.get_timestep_times_float(modelpath, loc="end")
     # find the last possible escape time and subtract the largest possible travel time (observer time correction)
-    depdata = at.get_deposition(modelpath=modelpath)  # use this file to find the last computed timestep
-    nts_last = depdata.ts.max() if "ts" in depdata.columns else len(depdata) - 1
-    nts_last_tend = at.get_timestep_times_float(modelpath, loc="end")[nts_last]
+    try:
+        depdata = at.get_deposition(modelpath=modelpath)  # use this file to find the last computed timestep
+        nts_last = depdata.ts.max() if "ts" in depdata.columns else len(depdata) - 1
+    except FileNotFoundError:
+        print("WARNING: No deposition.out file found. Assuming all timesteps have been computed")
+        nts_last = len(t_end) - 1
+
+    nts_last_tend = t_end[nts_last]
 
     # latest possible valid range is the end of the latest computed timestep plus the longest travel time
     validrange_end_days = nts_last_tend * (1 - cornervmax / 29979245800)
 
     if validrange_start_days > validrange_end_days:
         validrange_start_days, validrange_end_days = None, None
 
@@ -554,31 +567,32 @@
 
 @lru_cache(maxsize=8)
 def get_model_name(path: Union[Path, str]) -> str:
     """Get the name of an ARTIS model from the path to any file inside it.
 
     Name will be either from a special plotlabel.txt file if it exists or the enclosing directory name
     """
-
-    if not Path(path).exists() and Path(path).parts[0] == "codecomparison":
+    path = Path(path)
+    if not path.exists() and path.parts[0] == "codecomparison":
         return str(path)
 
-    abspath = os.path.abspath(path)
+    abspath = path.resolve()
 
-    modelpath = abspath if os.path.isdir(abspath) else os.path.dirname(abspath)
+    modelpath = abspath if abspath.is_dir() else abspath.parent
 
     try:
         plotlabelfile = Path(modelpath, "plotlabel.txt")
-        return open(plotlabelfile).readline().strip()
+        with open(plotlabelfile) as f:
+            return f.readline().strip()
     except FileNotFoundError:
         return os.path.basename(modelpath)
 
 
 def get_z_a_nucname(nucname: str) -> tuple[int, int]:
-    """return atomic number and mass number from a string like 'Pb208' (returns 92, 208)"""
+    """Return atomic number and mass number from a string like 'Pb208' (returns 92, 208)."""
     if nucname.startswith("X_"):
         nucname = nucname[2:]
     z = get_atomic_number(nucname.rstrip("0123456789"))
     assert z > 0
     a = int(nucname.lower().lstrip("abcdefghijklmnopqrstuvwxyz"))
     return z, a
 
@@ -638,15 +652,16 @@
 
 # based on code from https://gist.github.com/kgaughan/2491663/b35e9a117b02a3567c8107940ac9b2023ba34ced
 def parse_range(rng: str, dictvars: dict[str, int]) -> Iterable[Any]:
     """Parse a string with an integer range and return a list of numbers, replacing special variables in dictvars."""
     strparts = rng.split("-")
 
     if len(strparts) not in [1, 2]:
-        raise ValueError(f"Bad range: '{rng}'")
+        msg = f"Bad range: '{rng}'"
+        raise ValueError(msg)
 
     parts = [int(i) if i not in dictvars else dictvars[i] for i in strparts]
     start: int = parts[0]
     end: int = start if len(parts) == 1 else parts[1]
 
     if start > end:
         end, start = start, end
@@ -673,15 +688,15 @@
         return []
     if isinstance(x, (str, Path)):
         return [x]
     return list(x)
 
 
 def trim_or_pad(requiredlength: int, *listoflistin: list[list[Any]]) -> Iterator[list[Any]]:
-    """Make lists equal in length to requiredlength either by padding with None or truncating"""
+    """Make lists equal in length to requiredlength either by padding with None or truncating."""
     for listin in listoflistin:
         listin = makelist(listin)
 
         listout = [listin[i] if i < len(listin) else None for i in range(requiredlength)]
 
         assert len(listout) == requiredlength
         yield listout
@@ -694,25 +709,24 @@
             listout.extend(elem)
         else:
             listout.append(elem)
     return listout
 
 
 def zopen(filename: Union[Path, str], mode: str = "rt", encoding: Optional[str] = None) -> Any:
-    """Open filename, filename.gz or filename.xz"""
-
+    """Open filename, filename.gz or filename.xz."""
     ext_fopen = [(".lz4", lz4.frame.open), (".zst", pyzstd.open), (".gz", gzip.open), (".xz", xz.open)]
 
     for ext, fopen in ext_fopen:
         file_ext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
         if Path(file_ext).exists():
             return fopen(file_ext, mode=mode, encoding=encoding)
 
     # open() can raise file not found if this file doesn't exist
-    return open(filename, mode=mode, encoding=encoding)
+    return open(filename, mode=mode, encoding=encoding)  # noqa: SIM115
 
 
 def firstexisting(
     filelist: Union[Sequence[Union[str, Path]], str, Path],
     folder: Union[Path, str] = Path("."),
     tryzipped: bool = True,
 ) -> Path:
@@ -730,44 +744,43 @@
                 if filenameext not in filelist:
                     fullpaths.append(Path(folder) / filenameext)
 
     for fullpath in fullpaths:
         if fullpath.exists():
             return fullpath
 
-    raise FileNotFoundError(f'None of these files exist in {folder}: {", ".join([str(x) for x in fullpaths])}')
+    msg = f"None of these files exist in {folder}: {', '.join([str(x) for x in fullpaths])}"
+    raise FileNotFoundError(msg)
 
 
 def anyexist(
     filelist: Sequence[Union[str, Path]],
     folder: Union[Path, str] = Path("."),
     tryzipped: bool = True,
 ) -> bool:
     """Return true if any files in file list exist."""
-
     try:
         firstexisting(filelist=filelist, folder=folder, tryzipped=tryzipped)
     except FileNotFoundError:
         return False
 
     return True
 
 
 def stripallsuffixes(f: Path) -> Path:
-    """Take a file path (e.g. packets00_0000.out.gz) and return the Path with no suffixes (e.g. packets)"""
+    """Take a file path (e.g. packets00_0000.out.gz) and return the Path with no suffixes (e.g. packets)."""
     f_nosuffixes = Path(f)
     for _ in f.suffixes:
         f_nosuffixes = f_nosuffixes.with_suffix("")  # each call removes only one suffix
 
     return f_nosuffixes
 
 
 def readnoncommentline(file: io.TextIOBase) -> str:
-    """Read a line from the text file, skipping blank and comment lines that begin with #"""
-
+    """Read a line from the text file, skipping blank and comment lines that begin with #."""
     line = ""
 
     while not line.strip() or line.strip().lstrip().startswith("#"):
         line = file.readline()
 
     return line
 
@@ -809,16 +822,15 @@
 
     return {}
 
 
 def get_filterfunc(
     args: argparse.Namespace, mode: str = "interp"
 ) -> Optional[Callable[[Union[list[float], np.ndarray]], np.ndarray]]:
-    """Using command line arguments to determine the appropriate filter function."""
-
+    """Use command line arguments to determine the appropriate filter function."""
     filterfunc: Optional[Callable[[Union[list[float], np.ndarray]], np.ndarray]] = None
     dictargs = vars(args)
 
     if dictargs.get("filtermovingavg", False):
 
         def movavgfilterfunc(ylist: Union[list[float], np.ndarray]) -> np.ndarray:
             n = args.filtermovingavg
@@ -847,16 +859,16 @@
 def join_pdf_files(pdf_list: list[str], modelpath_list: list[Path]) -> None:
     from PyPDF2 import PdfFileMerger
 
     merger = PdfFileMerger()
 
     for pdf, modelpath in zip(pdf_list, modelpath_list):
         fullpath = firstexisting([pdf], folder=modelpath)
-        merger.append(open(fullpath, "rb"))
-        os.remove(fullpath)
+        merger.append(open(fullpath, "rb"))  # noqa: SIM115
+        fullpath.unlink()
 
     resultfilename = f'{pdf_list[0].split(".")[0]}-{pdf_list[-1].split(".")[0]}'
     with open(f"{resultfilename}.pdf", "wb") as resultfile:
         merger.write(resultfile)
 
     print(f"Files merged and saved to {resultfilename}.pdf")
 
@@ -883,17 +895,17 @@
 linetuple = namedtuple("linetuple", "lambda_angstroms atomic_number ionstage upperlevelindex lowerlevelindex")
 
 
 def read_linestatfile(
     filepath: Union[Path, str]
 ) -> tuple[int, list[float], list[int], list[int], list[int], list[int]]:
     """Load linestat.out containing transitions wavelength, element, ion, upper and lower levels."""
-
     print(f"Loading {filepath}")
-    data = np.loadtxt(filepath)
+
+    data = np.loadtxt(zopen(filepath))
     lambda_angstroms = data[0] * 1e8
     nlines = len(lambda_angstroms)
 
     atomic_numbers = data[1].astype(int)
     assert len(atomic_numbers) == nlines
 
     ion_stages = data[2].astype(int)
@@ -905,14 +917,41 @@
 
     lower_levels = data[4].astype(int)
     assert len(lower_levels) == nlines
 
     return nlines, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels
 
 
+def get_linelist_pldf(modelpath: Union[Path, str]) -> pl.LazyFrame:
+    textfile = at.firstexisting("linestat.out", folder=modelpath)
+    parquetfile = Path(modelpath, "linelist.out.parquet")
+    if not parquetfile.is_file() or parquetfile.stat().st_mtime < textfile.stat().st_mtime:
+        _, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels = read_linestatfile(textfile)
+
+        pldf = (
+            pl.DataFrame(
+                {
+                    "lambda_angstroms": lambda_angstroms,
+                    "atomic_number": atomic_numbers,
+                    "ion_stage": ion_stages,
+                    "upper_level": upper_levels,
+                    "lower_level": lower_levels,
+                },
+            )
+            # .with_columns(pl.col(pl.Int64).cast(pl.Int32))
+            .with_row_count(name="lineindex")
+        )
+        pldf.write_parquet(parquetfile, compression="zstd")
+        print(f"Saved {parquetfile}")
+    else:
+        print(f"Reading {parquetfile}")
+
+    return pl.scan_parquet(parquetfile)
+
+
 def get_linelist_dict(modelpath: Union[Path, str]) -> dict[int, linetuple]:
     nlines, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels = read_linestatfile(
         Path(modelpath, "linestat.out")
     )
     linelistdict = {
         index: linetuple(lambda_a, Z, ionstage, upper, lower)
         for index, lambda_a, Z, ionstage, upper, lower in zip(
@@ -1029,18 +1068,19 @@
         pass
 
     return tuple(folder_timesteps)
 
 
 def get_runfolders(
     modelpath: Union[Path, str], timestep: Optional[int] = None, timesteps: Optional[Sequence[int]] = None
-) -> Collection[Path]:
+) -> Sequence[Path]:
     """Get a list of folders containing ARTIS output files from a modelpath, optionally with a timestep restriction.
 
-    The folder list may include non-ARTIS folders if a timestep is not specified."""
+    The folder list may include non-ARTIS folders if a timestep is not specified.
+    """
     folderlist_all = (*sorted([child for child in Path(modelpath).iterdir() if child.is_dir()]), Path(modelpath))
     folder_list_matching = []
     if (timestep is not None and timestep > -1) or (timesteps is not None and len(timesteps) > 0):
         for folderpath in folderlist_all:
             folder_timesteps = get_runfolder_timesteps(folderpath)
             if timesteps is None and timestep is not None and timestep in folder_timesteps:
                 return (folderpath,)
@@ -1053,24 +1093,23 @@
 
 
 def get_mpiranklist(
     modelpath: Union[Path, str],
     modelgridindex: Optional[Union[Iterable[int], int]] = None,
     only_ranks_withgridcells: bool = False,
 ) -> Sequence[int]:
-    """
-    Get a list of rank ids. Parameters:
+    """Get a list of rank ids.
+
     - modelpath:
         pathlib.Path() to ARTIS model folder
     - modelgridindex:
         give a cell number to only return the rank number that updates this cell (and outputs its estimators)
     - only_ranks_withgridcells:
-        set True to skip ranks that only update packets (i.e. that don't update any grid cells/output estimators)
+        set True to skip ranks that only update packets (i.e. that don't update any grid cells/output estimators).
     """
-
     if modelgridindex is None or modelgridindex == []:
         if only_ranks_withgridcells:
             return range(min(get_nprocs(modelpath), get_npts_model(modelpath)))
         return range(get_nprocs(modelpath))
 
     if isinstance(modelgridindex, Iterable):
         mpiranklist = set()
@@ -1151,72 +1190,62 @@
 
     assert modelgridindex in get_cellsofmpirank(mpirank, modelpath)
 
     return mpirank
 
 
 def get_viewingdirectionbincount() -> int:
-    return 100
+    return get_viewingdirection_phibincount() * get_viewingdirection_costhetabincount()
 
 
 def get_viewingdirection_phibincount() -> int:
     return 10
 
 
 def get_viewingdirection_costhetabincount() -> int:
     return 10
 
 
-def get_costhetabin_phibin_labels() -> tuple[list[str], list[str]]:
-    # todo: replace with general code for any bin count:
-    # ncosthetabins = at.get_viewingdirection_costhetabincount()
-    # costhetabins_lower = np.arange(-1., 1., 2. / ncosthetabins)
-    # costhetabins_upper = costhetabins_lower + 2. / ncosthetabins
-
-    costheta_viewing_angle_bins = [
-        "-1.0 ≤ cos θ < -0.8",
-        "-0.8 ≤ cos θ < -0.6",
-        "-0.6 ≤ cos θ < -0.4",
-        "-0.4 ≤ cos θ < -0.2",
-        "-0.2 ≤ cos θ <  0.0",
-        " 0.0 ≤ cos θ <  0.2",
-        " 0.2 ≤ cos θ <  0.4",
-        " 0.4 ≤ cos θ <  0.6",
-        " 0.6 ≤ cos θ <  0.8",
-        " 0.8 ≤ cos θ <  1.0",
-    ]
-    assert len(costheta_viewing_angle_bins) == get_viewingdirection_costhetabincount()
+def get_phi_bins() -> tuple[np.ndarray, np.ndarray, list[str]]:
+    nphibins = at.get_viewingdirection_phibincount()
+    # pi/2 must be an exact boundary because of the change in behaviour there
+    assert nphibins % 2 == 0
 
-    # this is not correct because the phi bins are not in ascending order
-    # nphibins = at.get_viewingdirection_phibincount()
-    # thetabins_lower = np.arange(0, 2 * math.pi, 2 * math.pi / nphibins)
-    # thetabins_upper = thetabins_lower + 2 * math.pi / nphibins
-
-    phi_viewing_angle_bins = [
-        "0 ≤ ϕ < π/5",
-        "π/5 ≤ ϕ < 2π/5",
-        "2π/5 ≤ ϕ < 3π/5",
-        "3π/5 ≤ ϕ < 4π/5",
-        "4π/5 ≤ ϕ < π",
-        "9π/5 < ϕ < 2π",
-        "8π/5 < ϕ ≤ 9π/5",
-        "7π/5 < ϕ ≤ 8π/5",
-        "6π/5 < ϕ ≤ 7π/5",
-        "π < ϕ ≤ 6π/5",
-    ]
-    assert len(phi_viewing_angle_bins) == get_viewingdirection_phibincount()
-    assert len(costheta_viewing_angle_bins) * len(phi_viewing_angle_bins) == get_viewingdirectionbincount()
+    # for historical reasons, phi bins ordered by ascending phi are
+    # [0, 1, 2, 3, 4, 9, 8, 7, 6, 5] for nphibins == 10
 
-    # label orders changed so that bins are in order. Not used yet.
-    # phi_viewing_angle_bins_reordered = ['0 ≤ ϕ < π/5', 'π/5 ≤ ϕ < 2π/5',
-    #                                     '2π/5 ≤ ϕ < 3π/5', '3π/5 ≤ ϕ < 4π/5',
-    #                                     '4π/5 ≤ ϕ < π', 'π < ϕ ≤ 6π/5',
-    #                                     '6π/5 < ϕ ≤ 7π/5', '7π/5 < ϕ ≤ 8π/5',
-    #                                     '8π/5 < ϕ ≤ 9π/5', '9π/5 < ϕ < 2π']
-    return costheta_viewing_angle_bins, phi_viewing_angle_bins
+    # convert phibin number to what the number would be if things were sane
+    phisteps = list(range(nphibins // 2)) + list(reversed(range(nphibins // 2, nphibins)))
+
+    phi_lower = np.array([step * 2 * math.pi / nphibins for step in phisteps])
+    phi_upper = np.array([(step + 1) * 2 * math.pi / nphibins for step in phisteps])
+
+    binlabels = []
+    for phibin, step in enumerate(phisteps):
+        str_phi_lower = f"{step}π/{nphibins // 2}" if step > 0 else "0"
+        lower_compare = "≤" if phibin < (nphibins // 2) else "<"
+        str_phi_upper = f"{step+1}π/{nphibins // 2}" if step < nphibins - 1 else "2π"
+        upper_compare = "≤" if phibin > (nphibins // 2) else "<"
+        binlabels.append(f"{str_phi_lower} {lower_compare} ϕ {upper_compare} {str_phi_upper}")
+
+    return phi_lower, phi_upper, binlabels
+
+
+def get_costheta_bins() -> tuple[np.ndarray, np.ndarray, list[str]]:
+    ncosthetabins = at.get_viewingdirection_costhetabincount()
+    costhetabins_lower = np.arange(-1.0, 1.0, 2.0 / ncosthetabins)
+    costhetabins_upper = costhetabins_lower + 2.0 / ncosthetabins
+    binlabels = [f"{lower:.1f} ≤ cos θ < {upper:.1f}" for lower, upper in zip(costhetabins_lower, costhetabins_upper)]
+    return costhetabins_lower, costhetabins_upper, binlabels
+
+
+def get_costhetabin_phibin_labels() -> tuple[list[str], list[str]]:
+    _, _, costhetabinlabels = get_costheta_bins()
+    _, _, phibinlabels = get_phi_bins()
+    return costhetabinlabels, phibinlabels
 
 
 def get_vspec_dir_labels(modelpath: Union[str, Path], viewinganglelabelunits: str = "rad") -> dict[int, str]:
     vpkt_config = at.get_vpkt_config(modelpath)
     dirlabels = {}
     for dirindex in range(vpkt_config["nobsdirections"]):
         phi_angle = round(vpkt_config["phi"][dirindex])
@@ -1237,31 +1266,32 @@
     if modelpath:
         modelpath = Path(modelpath)
         MABINS = at.get_viewingdirectionbincount()
         if len(list(Path(modelpath).glob("*_res_00.out*"))) > 0:  # if the first direction bin file exists
             assert len(list(Path(modelpath).glob(f"*_res_{MABINS-1:02d}.out*"))) > 0  # check last bin exists
             assert len(list(Path(modelpath).glob(f"*_res_{MABINS:02d}.out*"))) == 0  # check one beyond does not exist
 
-    strlist_costheta_bins, strlist_phi_bins = at.get_costhetabin_phibin_labels()
+    _, _, costhetabinlabels = get_costheta_bins()
+    _, _, phibinlabels = get_phi_bins()
 
     nphibins = at.get_viewingdirection_phibincount()
 
     angle_definitions: dict[int, str] = {}
     for dirbin in dirbins:
         if dirbin == -1:
             angle_definitions[dirbin] = ""
             continue
 
         costheta_index = dirbin // nphibins
         phi_index = dirbin % nphibins
 
         if average_over_phi:
-            angle_definitions[dirbin] = f"{strlist_costheta_bins[costheta_index]}"
+            angle_definitions[dirbin] = f"{costhetabinlabels[costheta_index]}"
             assert phi_index == 0
             assert not average_over_theta
         elif average_over_theta:
-            angle_definitions[dirbin] = f"{strlist_phi_bins[phi_index]}"
+            angle_definitions[dirbin] = f"{phibinlabels[phi_index]}"
             assert costheta_index == 0
         else:
-            angle_definitions[dirbin] = f"{strlist_costheta_bins[costheta_index]}, {strlist_phi_bins[phi_index]}"
+            angle_definitions[dirbin] = f"{costhetabinlabels[costheta_index]}, {phibinlabels[phi_index]}"
 
     return angle_definitions
```

### Comparing `artistools-2023.4.19.2/artistools/nltepops/nltepops.py` & `artistools-2023.5.16/artistools/nltepops/nltepops.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
             dfpop.loc[masksuperlevel, "level"] = levelnumber_sl + 2
 
     return dfpop
 
 
 def read_file(nltefilepath: Union[str, Path]) -> pd.DataFrame:
     """Read NLTE populations from one file."""
-
     if not Path(nltefilepath).is_file():
         nltefilepathgz = Path(str(nltefilepath) + ".gz")
         nltefilepathxz = Path(str(nltefilepath) + ".xz")
         if nltefilepathxz.is_file():
             nltefilepath = nltefilepathxz
         elif nltefilepathgz.is_file():
             nltefilepath = nltefilepathgz
@@ -180,15 +179,14 @@
 
 
 @lru_cache(maxsize=2)
 def read_files(
     modelpath, timestep=-1, modelgridindex=-1, dfquery=None, dfqueryvars: Optional[dict] = None
 ) -> pd.DataFrame:
     """Read in NLTE populations from a model for a particular timestep and grid cell."""
-
     if dfqueryvars is None:
         dfqueryvars = {}
 
     mpiranklist = at.get_mpiranklist(modelpath, modelgridindex=modelgridindex)
 
     dfpop = pd.DataFrame()
 
@@ -212,15 +210,15 @@
 
     if dfquery:
         if dfquery_full:
             dfquery_full = f"({dfquery_full}) and "
         dfquery_full += f"({dfquery})"
 
     if get_config()["num_processes"] > 1:
-        with multiprocessing.Pool(processes=get_config()["num_processes"]) as pool:
+        with multiprocessing.get_context("fork").Pool(processes=get_config()["num_processes"]) as pool:
             arr_dfnltepop = pool.map(
                 partial(read_file_filtered, strquery=dfquery_full, dfqueryvars=dfqueryvars), nltefilepaths
             )
             pool.close()
             pool.join()
             pool.terminate()
     else:
```

### Comparing `artistools-2023.4.19.2/artistools/nltepops/plotnltepops.py` & `artistools-2023.5.16/artistools/nltepops/plotnltepops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """Artistools - NLTE population related functions."""
 import argparse
 import math
-import multiprocessing
 import os
 import sys
 from pathlib import Path
+from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import constants as const
 from matplotlib import ticker
@@ -734,17 +734,18 @@
     parser.add_argument("-ymin", type=float, default=None, help="Plot range: y-axis")
 
     parser.add_argument("-ymax", type=float, default=None, help="Plot range: y-axis")
 
     parser.add_argument("-outputfile", "-o", type=Path, default=defaultoutputfile, help="path/filename for PDF file")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Plot ARTIS non-LTE populations."""
     if args is None:
-        parser = argparse.ArgumentParser(description="Plot ARTIS non-LTE corrections.")
+        parser = argparse.ArgumentParser(description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     at.set_mpl_style()
 
     if args.x in ["time", "velocity"]:
@@ -788,15 +789,15 @@
 
     if isinstance(args.elements, str):
         args.elements = [args.elements]
 
     if isinstance(args.velocity, (float, int)):
         args.velocity = [args.velocity]
 
-    mgilist = []
+    mgilist: list[Union[int, float]] = []
     for mgi in args.modelgridindex:
         mgilist.append(int(mgi))
 
     for vel in args.velocity:
         mgilist.append(at.inputmodel.get_mgi_of_velocity_kms(modelpath, vel))
 
     if not mgilist:
@@ -816,9 +817,8 @@
             if atomic_number < 1:
                 print(f"Could not find element '{elsymbol}'")
 
         make_plot(modelpath, atomic_number, ionstages_permitted, mgilist, timestep, args)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/nonthermal/__init__.py` & `artistools-2023.5.16/artistools/nonthermal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Artistools - spectra related functions."""
+import artistools.nonthermal.solvespencerfanocmd
+
 from .__main__ import main
 from ._nonthermal_core import analyse_ntspectrum
 from ._nonthermal_core import ar_xs
 from ._nonthermal_core import calculate_frac_heating
 from ._nonthermal_core import calculate_Latom_excitation
 from ._nonthermal_core import calculate_Latom_ionisation
 from ._nonthermal_core import calculate_N_e
```

### Comparing `artistools-2023.4.19.2/artistools/nonthermal/_nonthermal_core.py` & `artistools-2023.5.16/artistools/nonthermal/_nonthermal_core.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/nonthermal/leptontransport.py` & `artistools-2023.5.16/artistools/nonthermal/leptontransport.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/nonthermal/plotnonthermal.py` & `artistools-2023.5.16/artistools/nonthermal/plotnonthermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 import argparse
-import multiprocessing
 import os
 from functools import lru_cache
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -285,19 +284,17 @@
 
     parser.add_argument(
         "-o", action="store", dest="outputfile", type=Path, default=defaultoutputfile, help="Filename for PDF file"
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
-    """Plot the electron energy distribution."""
+    """Plot ARTIS non-thermal electron energy spectrum."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS non-thermal electron energy spectrum."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
         args.modelpath = [Path(".")]
@@ -318,9 +315,8 @@
     if args.listtimesteps:
         at.showtimesteptimes()
     else:
         make_plot(modelpaths, args)
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/nonthermal/solvespencerfanocmd.py` & `artistools-2023.5.16/artistools/nonthermal/solvespencerfanocmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python3
 import argparse
-import multiprocessing
 import sys
 from pathlib import Path
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -139,18 +138,19 @@
         action="store",
         default=None,
         help="Path/filename for NT stats input (no solution, only plotting stat file)",
     )
 
 
 def main(args=None, argsraw=None, **kwargs):
+    """Solve Spencer-Fano equation using data from ARTIS cell at some timestep."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Plot estimated spectra from bound-bound transitions.",
+            description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if args.plotstats:
         make_ntstats_plot(args.plotstats)
@@ -366,9 +366,8 @@
     if args.ostat:
         make_ntstats_plot(args.ostat)
         return None
     return None
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/packets/__init__.py` & `artistools-2023.5.16/artistools/packets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import artistools as at
+
 from .packets import add_derived_columns
+from .packets import add_derived_columns_lazy
 from .packets import bin_and_sum
 from .packets import bin_packet_directions
+from .packets import bin_packet_directions_lazypolars
 from .packets import get_directionbin
 from .packets import get_mean_packet_emission_velocity_per_ts
 from .packets import get_packets_pl
 from .packets import get_packetsfilepaths
 from .packets import make_3d_grid
 from .packets import make_3d_histogram_from_packets
 from .packets import readfile
```

### Comparing `artistools-2023.4.19.2/artistools/packets/packets.py` & `artistools-2023.5.16/artistools/packets/packets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import calendar
 import gzip
 import math
-import os
+import multiprocessing
 from collections.abc import Sequence
 from functools import lru_cache
 from pathlib import Path
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 import polars as pl
 
 import artistools as at
 
 # for the parquet files
-time_lastschemachange = (2023, 4, 2, 22, 13, 0)
+time_parquetschemachange = (2023, 4, 22, 12, 31, 0)
 
 CLIGHT = 2.99792458e10
 DAY = 86400
 
 types = {
     10: "TYPE_GAMMA",
     11: "TYPE_RPKT",
@@ -141,37 +141,41 @@
     dfpackets: pd.DataFrame,
     modelpath: Path,
     colnames: Sequence[str],
     allnonemptymgilist: Optional[Sequence[int]] = None,
 ) -> pd.DataFrame:
     cm_to_km = 1e-5
     day_in_s = 86400
-    if dfpackets.empty:
+    if isinstance(dfpackets, pd.DataFrame) and dfpackets.empty:
         return dfpackets
 
     colnames = at.makelist(colnames)
+    dimensions = at.get_inputparams(modelpath)["n_dimensions"]
 
     def em_modelgridindex(packet) -> Union[int, float]:
+        assert dimensions == 1
+
         return at.inputmodel.get_mgi_of_velocity_kms(
             modelpath, packet.emission_velocity * cm_to_km, mgilist=allnonemptymgilist
         )
 
     def emtrue_modelgridindex(packet) -> Union[int, float]:
+        assert dimensions == 1
+
         return at.inputmodel.get_mgi_of_velocity_kms(
             modelpath, packet.true_emission_velocity * cm_to_km, mgilist=allnonemptymgilist
         )
 
     def em_timestep(packet) -> int:
         return at.get_timestep_of_timedays(modelpath, packet.em_time / day_in_s)
 
     def emtrue_timestep(packet) -> int:
         return at.get_timestep_of_timedays(modelpath, packet.trueem_time / day_in_s)
 
     if "emission_velocity" in colnames:
-        dfpackets = dfpackets.eval("emission_velocity = sqrt(em_posx ** 2 + em_posy ** 2 + em_posz ** 2) / em_time")
         dfpackets["emission_velocity"] = (
             np.sqrt(dfpackets["em_posx"] ** 2 + dfpackets["em_posy"] ** 2 + dfpackets["em_posz"] ** 2)
             / dfpackets["em_time"]
         )
 
         dfpackets["em_velx"] = dfpackets["em_posx"] / dfpackets["em_time"]
         dfpackets["em_vely"] = dfpackets["em_posy"] / dfpackets["em_time"]
@@ -195,14 +199,61 @@
 
     if any(x in colnames for x in ["angle_bin", "dirbin", "costhetabin", "phibin"]):
         dfpackets = bin_packet_directions(modelpath, dfpackets)
 
     return dfpackets
 
 
+def add_derived_columns_lazy(dfpackets: pl.LazyFrame, modelmeta: Optional[dict] = None) -> pl.LazyFrame:
+    # we might as well add everything, since the columns only get calculated when they are actually used
+
+    dfpackets = dfpackets.with_columns(
+        [
+            (
+                (pl.col("em_posx") ** 2 + pl.col("em_posy") ** 2 + pl.col("em_posz") ** 2).sqrt() / pl.col("em_time")
+            ).alias("emission_velocity")
+        ]
+    )
+
+    dfpackets = dfpackets.with_columns(
+        [
+            (
+                (
+                    (pl.col("em_posx") * pl.col("dirx")) ** 2
+                    + (pl.col("em_posy") * pl.col("diry")) ** 2
+                    + (pl.col("em_posz") * pl.col("dirz")) ** 2
+                ).sqrt()
+                / pl.col("em_time")
+            ).alias("emission_velocity_lineofsight")
+        ]
+    )
+
+    if modelmeta is not None and modelmeta["dimensions"] == 3:
+        t_model_s = modelmeta["t_model_init_days"] * 86400.0
+        vmax = modelmeta["vmax_cmps"]
+        vwidth = modelmeta["wid_init"] / t_model_s
+        dfpackets = dfpackets.with_columns(
+            [
+                ((pl.col(f"em_pos{ax}") / pl.col("em_time") + vmax) / vwidth).cast(pl.Int32).alias(f"coordpointnum{ax}")
+                for ax in ["x", "y", "z"]
+            ]
+        )
+        dfpackets = dfpackets.with_columns(
+            [
+                (
+                    pl.col("coordpointnumz") * modelmeta["ncoordgridy"] * modelmeta["ncoordgridx"]
+                    + pl.col("coordpointnumy") * modelmeta["ncoordgridx"]
+                    + pl.col("coordpointnumx")
+                ).alias("em_modelgridindex")
+            ]
+        )
+
+    return dfpackets
+
+
 def readfile_text(packetsfile: Union[Path, str], modelpath: Path = Path(".")) -> pl.DataFrame:
     """Read a packets*.out(.xz) space-separated text file into a polars DataFrame."""
     print(f"Reading {packetsfile}")
     skiprows: int = 0
     column_names: Optional[list[str]] = None
     try:
         fpackets = at.zopen(packetsfile, mode="rb")
@@ -252,272 +303,330 @@
     dfpackets = dfpackets.drop(["next_trans", "last_cross"])
 
     # drop last column of nulls (caused by trailing space on each line)
     if dfpackets[dfpackets.columns[-1]].is_null().all():
         dfpackets = dfpackets.drop(dfpackets.columns[-1])
 
     if "true_emission_velocity" in dfpackets.columns:
+        # some packets don't have this set, which confused read_csv to mark it as str
         dfpackets = dfpackets.with_columns([pl.col("true_emission_velocity").cast(pl.Float32)])
 
-    # cast Int64 to Int32
+    if "originated_from_positron" in dfpackets.columns:
+        dfpackets = dfpackets.with_columns([pl.col("originated_from_positron").cast(pl.Boolean)])
+
+    # Luke: packet energies in ergs can be huge (>1e39) which is too large for Float32
     dfpackets = dfpackets.with_columns(
-        [pl.col(col).cast(pl.Int32) for col in dfpackets.columns if dfpackets[col].dtype == pl.Int64]
+        [pl.col(pl.Int64).cast(pl.Int32), pl.col(pl.Float64).exclude(["e_rf", "e_cmf"]).cast(pl.Float32)]
     )
 
     return dfpackets
 
 
 def readfile(
     packetsfile: Union[Path, str],
     packet_type: Optional[str] = None,
     escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
 ) -> pd.DataFrame:
     """Read a packet file into a Pandas DataFrame."""
     return readfile_pl(packetsfile, packet_type=packet_type, escape_type=escape_type).collect().to_pandas()
 
 
+def convert_text_to_parquet(
+    packetsfiletext: Union[Path, str],
+) -> Path:
+    packetsfiletext = Path(packetsfiletext)
+    packetsfileparquet = at.stripallsuffixes(packetsfiletext).with_suffix(".out.parquet")
+
+    dfpackets = readfile_text(packetsfiletext).lazy()
+    dfpackets = dfpackets.with_columns(
+        [
+            (
+                (
+                    pl.col("escape_time")
+                    - (
+                        pl.col("posx") * pl.col("dirx")
+                        + pl.col("posy") * pl.col("diry")
+                        + pl.col("posz") * pl.col("dirz")
+                    )
+                    / 29979245800.0
+                )
+                / 86400.0
+            )
+            .cast(pl.Float32)
+            .alias("t_arrive_d"),
+        ]
+    )
+
+    syn_dir = (0.0, 0.0, 1.0)
+    for p in packetsfiletext.parents:
+        if Path(p, "syn_dir.txt").is_file():
+            syn_dir = at.get_syn_dir(p)
+            break
+
+    dfpackets = add_packet_directions_lazypolars(dfpackets, syn_dir)
+    dfpackets = bin_packet_directions_lazypolars(dfpackets)
+
+    # print(f"Saving {packetsfileparquet}")
+    dfpackets = dfpackets.sort(by=["type_id", "escape_type_id", "t_arrive_d"])
+    dfpackets.collect().write_parquet(packetsfileparquet, compression="zstd", statistics=True)
+
+    return packetsfileparquet
+
+
 def readfile_pl(
     packetsfile: Union[Path, str],
+    modelpath: Union[None, Path, str] = None,
     packet_type: Optional[str] = None,
     escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
 ) -> pl.LazyFrame:
     """Read a packets file into a Polars LazyFrame from either a parquet file or a text file (and save .parquet)."""
-    packetsfile = Path(packetsfile)
-    packetsfileparquet = at.stripallsuffixes(packetsfile).with_suffix(".out.parquet")
-    packetsfiletext = (
-        packetsfile
-        if packetsfile.suffixes in [[".out"], [".out", ".gz"], [".out", ".xz"], [".out", ".lz4"]]
-        else at.firstexisting([at.stripallsuffixes(packetsfile).with_suffix(".out")], tryzipped=True)
-    )
-
-    write_parquet = True  # will be set False if parquet file is read
-
-    dfpackets = None
-    if packetsfile == packetsfileparquet and os.path.getmtime(packetsfileparquet) > calendar.timegm(
-        time_lastschemachange
-    ):
-        try:
-            dfpackets = pl.scan_parquet(packetsfileparquet)
-            write_parquet = False
-        except Exception as exc:
-            print(exc)
-            print(f"Error occured in file {packetsfile}. Reading from text version.")
-
-    if dfpackets is None:
-        dfpackets = readfile_text(packetsfiletext).lazy()
-
-    if "t_arrive_d" not in dfpackets.columns:
-        dfpackets = dfpackets.with_columns(
-            [
-                (
-                    (
-                        pl.col("escape_time")
-                        - (
-                            pl.col("posx") * pl.col("dirx")
-                            + pl.col("posy") * pl.col("diry")
-                            + pl.col("posz") * pl.col("dirz")
-                        )
-                        / 29979245800.0
-                    )
-                    / 86400.0
-                ).alias("t_arrive_d"),
-            ]
-        )
-
-    if write_parquet:
-        print(f"Saving {packetsfileparquet}")
-        dfpackets = dfpackets.sort(by=["type_id", "escape_type_id", "t_arrive_d"])
-        dfpackets.collect().write_parquet(packetsfileparquet, compression="zstd", statistics=True)
-        dfpackets = pl.scan_parquet(packetsfileparquet)
+    dfpackets = pl.scan_parquet(packetsfile)
 
     if escape_type is not None:
         assert packet_type is None or packet_type == "TYPE_ESCAPE"
         dfpackets = dfpackets.filter(
             (pl.col("type_id") == type_ids["TYPE_ESCAPE"]) & (pl.col("escape_type_id") == type_ids[escape_type])
         )
     elif packet_type is not None and packet_type:
         dfpackets = dfpackets.filter(pl.col("type_id") == type_ids[packet_type])
 
     return dfpackets
 
 
-def get_packetsfilepaths(modelpath: Union[str, Path], maxpacketfiles: Optional[int] = None) -> list[Path]:
+def get_packetsfilepaths(
+    modelpath: Union[str, Path], maxpacketfiles: Optional[int] = None, printwarningsonly: bool = False
+) -> list[Path]:
     nprocs = at.get_nprocs(modelpath)
 
     searchfolders = [Path(modelpath, "packets"), Path(modelpath)]
     # in descending priority (based on speed of reading)
-    suffix_priority = [".out.parquet", ".out.zst", ".out.lz4", ".out.zst", ".out", ".out.gz", ".out.xz"]
-    packetsfiles = []
+    suffix_priority = [".out.zst", ".out.lz4", ".out.zst", ".out", ".out.gz", ".out.xz"]
+    t_lastschemachange = calendar.timegm(time_parquetschemachange)
+
+    parquetpacketsfiles = []
+    parquetrequiredfiles = []
 
     for rank in range(nprocs + 1):
         name_nosuffix = f"packets00_{rank:04d}"
         found_rank = False
-        for suffix in suffix_priority:
-            if found_rank:
-                break
-            for folderpath in searchfolders:
-                if (folderpath / name_nosuffix).with_suffix(suffix).is_file():
-                    packetsfiles.append((folderpath / name_nosuffix).with_suffix(suffix))
+
+        for folderpath in searchfolders:
+            filepath = (folderpath / name_nosuffix).with_suffix(".out.parquet")
+            if filepath.is_file():
+                if filepath.stat().st_mtime < t_lastschemachange:
+                    filepath.unlink(missing_ok=True)
+                    print(f"{filepath} is out of date.")
+                else:
+                    if rank < nprocs:
+                        parquetpacketsfiles.append(filepath)
                     found_rank = True
+
+        if not found_rank:
+            for suffix in suffix_priority:
+                for folderpath in searchfolders:
+                    filepath = (folderpath / name_nosuffix).with_suffix(suffix)
+                    if filepath.is_file():
+                        if rank < nprocs:
+                            parquetrequiredfiles.append(filepath)
+                        found_rank = True
+                        break
+
+                if found_rank:
                     break
 
         if found_rank and rank >= nprocs:
-            print(f"WARNING: nprocs is {nprocs} but file {packetsfiles[-1]} exists")
-            packetsfiles = packetsfiles[:-1]
+            print(f"WARNING: nprocs is {nprocs} but file {filepath} exists")
         elif not found_rank and rank < nprocs:
             print(f"WARNING: packets file for rank {rank} was not found.")
 
-        if maxpacketfiles is not None and len(packetsfiles) >= maxpacketfiles:
+        if maxpacketfiles is not None and (len(parquetpacketsfiles) + len(parquetrequiredfiles)) >= maxpacketfiles:
             break
 
-    if maxpacketfiles is not None and nprocs > maxpacketfiles:
-        print(f"Reading from the first {maxpacketfiles} of {len(packetsfiles)} packets files")
+    if len(parquetrequiredfiles) >= 20:
+        with multiprocessing.get_context("spawn").Pool(processes=at.get_config()["num_processes"]) as pool:
+            convertedparquetpacketsfiles = pool.map(convert_text_to_parquet, parquetrequiredfiles)
+            pool.close()
+            pool.join()
     else:
-        print(f"Reading from {len(packetsfiles)} packets files")
+        convertedparquetpacketsfiles = [convert_text_to_parquet(p) for p in parquetrequiredfiles]
+
+    parquetpacketsfiles += list(convertedparquetpacketsfiles)
+
+    if not printwarningsonly:
+        if maxpacketfiles is not None and nprocs > maxpacketfiles:
+            print(f"Reading from the first {maxpacketfiles} of {nprocs} packets files")
+        else:
+            print(f"Reading from {len(parquetpacketsfiles)} packets files")
 
-    return packetsfiles
+    return parquetpacketsfiles
 
 
 def get_packets_pl(
     modelpath: Union[str, Path],
     maxpacketfiles: Optional[int] = None,
     packet_type: Optional[str] = None,
     escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
 ) -> tuple[int, pl.LazyFrame]:
     if escape_type is not None:
         assert packet_type in [None, "TYPE_ESCAPE"]
         if packet_type is None:
             packet_type = "TYPE_ESCAPE"
 
-    packetsfiles = at.packets.get_packetsfilepaths(modelpath, maxpacketfiles)
+    packetsfiles = get_packetsfilepaths(modelpath, maxpacketfiles)
 
     nprocs_read = len(packetsfiles)
-    allescrpktfile_parquet = Path(modelpath) / "packets_rpkt_escaped.parquet"
+    packetsdatasize_gb = nprocs_read * Path(packetsfiles[0]).stat().st_size / 1024 / 1024 / 1024
+    print(f" data size is {packetsdatasize_gb:.1f} GB ({nprocs_read} * size of {packetsfiles[0].parts[-1]})")
 
-    write_allpkts_parquet = False
-    pldfpackets = None
-    if maxpacketfiles is None and escape_type == "TYPE_RPKT":
-        if allescrpktfile_parquet.is_file() and os.path.getmtime(allescrpktfile_parquet) > calendar.timegm(
-            time_lastschemachange
-        ):
-            print(f"Reading from {allescrpktfile_parquet}")
-            pldfpackets = pl.scan_parquet(allescrpktfile_parquet)
-        else:
-            write_allpkts_parquet = True
+    pldfpackets = pl.concat(
+        (pl.scan_parquet(packetsfile) for packetsfile in packetsfiles),
+        how="vertical",
+    )
 
-    if pldfpackets is None:
-        pldfpackets = pl.concat(
-            [
-                at.packets.readfile_pl(packetsfile, packet_type=packet_type, escape_type=escape_type)
-                for packetsfile in packetsfiles
-            ],
-            how="vertical",
-            rechunk=False,
-        )
-
-        pldfpackets = bin_packet_directions_lazypolars(modelpath, pldfpackets)
-
-    if write_allpkts_parquet:
-        print(f"Saving {allescrpktfile_parquet}")
-        # pldfpackets = pldfpackets.sort(by=["type_id", "escape_type_id", "t_arrive_d"])
-        pldfpackets.collect(streaming=True).write_parquet(
-            allescrpktfile_parquet,
-            compression="zstd",
-            row_group_size=1024 * 1024,
-            statistics=True,
+    if escape_type is not None:
+        assert packet_type is None or packet_type == "TYPE_ESCAPE"
+        pldfpackets = pldfpackets.filter(
+            (pl.col("type_id") == type_ids["TYPE_ESCAPE"]) & (pl.col("escape_type_id") == type_ids[escape_type])
         )
+    elif packet_type is not None and packet_type:
+        pldfpackets = pldfpackets.filter(pl.col("type_id") == type_ids[packet_type])
 
     return nprocs_read, pldfpackets
 
 
 def get_directionbin(
-    dirx: float, diry: float, dirz: float, nphibins: int, ncosthetabins: int, syn_dir: Sequence[float]
+    dirx: float, diry: float, dirz: float, nphibins: int, ncosthetabins: int, syn_dir: tuple[float, float, float]
 ) -> int:
     dirmag = np.sqrt(dirx**2 + diry**2 + dirz**2)
     pkt_dir = [dirx / dirmag, diry / dirmag, dirz / dirmag]
     costheta = np.dot(pkt_dir, syn_dir)
-    thetabin = int((costheta + 1.0) / 2.0 * ncosthetabins)
+    costhetabin = int((costheta + 1.0) / 2.0 * ncosthetabins)
 
     xhat = np.array([1.0, 0.0, 0.0])
     vec1 = np.cross(pkt_dir, syn_dir)
     vec2 = np.cross(xhat, syn_dir)
     cosphi = np.dot(vec1, vec2) / at.vec_len(vec1) / at.vec_len(vec2)
 
     vec3 = np.cross(vec2, syn_dir)
     testphi = np.dot(vec1, vec3)
+    # phi = math.acos(cosphi) if testphi > 0 else (math.acos(-cosphi) + np.pi)
 
     phibin = (
         int(math.acos(cosphi) / 2.0 / np.pi * nphibins)
-        if testphi > 0
+        if testphi >= 0
         else int((math.acos(cosphi) + np.pi) / 2.0 / np.pi * nphibins)
     )
 
-    return (thetabin * nphibins) + phibin
+    return (costhetabin * nphibins) + phibin
 
 
-def bin_packet_directions_lazypolars(modelpath: Union[Path, str], dfpackets: pl.LazyFrame) -> pl.LazyFrame:
-    nphibins = at.get_viewingdirection_phibincount()
-    ncosthetabins = at.get_viewingdirection_costhetabincount()
-
-    syn_dir = at.get_syn_dir(Path(modelpath))
+def add_packet_directions_lazypolars(dfpackets: pl.LazyFrame, syn_dir: tuple[float, float, float]) -> pl.LazyFrame:
+    assert len(syn_dir) == 3
     xhat = np.array([1.0, 0.0, 0.0])
     vec2 = np.cross(xhat, syn_dir)
 
-    dfpackets = dfpackets.with_columns(
-        (pl.col("dirx") ** 2 + pl.col("diry") ** 2 + pl.col("dirz") ** 2).sqrt().alias("dirmag"),
-    )
-    dfpackets = dfpackets.with_columns(
-        (
-            (pl.col("dirx") * syn_dir[0] + pl.col("diry") * syn_dir[1] + pl.col("dirz") * syn_dir[2]) / pl.col("dirmag")
-        ).alias("costheta"),
-    )
-    dfpackets = dfpackets.with_columns(
-        ((pl.col("costheta") + 1) / 2.0 * ncosthetabins).cast(pl.Int64).alias("costhetabin"),
-    )
-    dfpackets = dfpackets.with_columns(
-        ((pl.col("diry") * syn_dir[2] - pl.col("dirz") * syn_dir[1]) / pl.col("dirmag")).alias("vec1_x"),
-        ((pl.col("dirz") * syn_dir[0] - pl.col("dirx") * syn_dir[2]) / pl.col("dirmag")).alias("vec1_y"),
-        ((pl.col("dirx") * syn_dir[1] - pl.col("diry") * syn_dir[0]) / pl.col("dirmag")).alias("vec1_z"),
-    )
+    if "dirmag" not in dfpackets.columns:
+        dfpackets = dfpackets.with_columns(
+            (pl.col("dirx") ** 2 + pl.col("diry") ** 2 + pl.col("dirz") ** 2).sqrt().alias("dirmag"),
+        )
 
-    dfpackets = dfpackets.with_columns(
-        (
-            (pl.col("vec1_x") * vec2[0] + pl.col("vec1_y") * vec2[1] + pl.col("vec1_z") * vec2[2])
-            / (pl.col("vec1_x") ** 2 + pl.col("vec1_y") ** 2 + pl.col("vec1_z") ** 2).sqrt()
-            / float(np.linalg.norm(vec2))
-        ).alias("cosphi"),
-    )
+    if "costheta" not in dfpackets.columns:
+        dfpackets = dfpackets.with_columns(
+            (
+                (pl.col("dirx") * syn_dir[0] + pl.col("diry") * syn_dir[1] + pl.col("dirz") * syn_dir[2])
+                / pl.col("dirmag")
+            )
+            .cast(pl.Float32)
+            .alias("costheta"),
+        )
 
-    # vec1 = dir cross syn_dir
-    dfpackets = dfpackets.with_columns(
-        ((pl.col("diry") * syn_dir[2] - pl.col("dirz") * syn_dir[1]) / pl.col("dirmag")).alias("vec1_x"),
-        ((pl.col("dirz") * syn_dir[0] - pl.col("dirx") * syn_dir[2]) / pl.col("dirmag")).alias("vec1_y"),
-        ((pl.col("dirx") * syn_dir[1] - pl.col("diry") * syn_dir[0]) / pl.col("dirmag")).alias("vec1_z"),
-    )
+    if "phi" not in dfpackets.columns:
+        dfpackets = dfpackets.with_columns(
+            ((pl.col("diry") * syn_dir[2] - pl.col("dirz") * syn_dir[1]) / pl.col("dirmag")).alias("vec1_x"),
+            ((pl.col("dirz") * syn_dir[0] - pl.col("dirx") * syn_dir[2]) / pl.col("dirmag")).alias("vec1_y"),
+            ((pl.col("dirx") * syn_dir[1] - pl.col("diry") * syn_dir[0]) / pl.col("dirmag")).alias("vec1_z"),
+        )
 
-    vec3 = np.cross(vec2, syn_dir)
+        dfpackets = dfpackets.with_columns(
+            (
+                (pl.col("vec1_x") * vec2[0] + pl.col("vec1_y") * vec2[1] + pl.col("vec1_z") * vec2[2])
+                / (pl.col("vec1_x") ** 2 + pl.col("vec1_y") ** 2 + pl.col("vec1_z") ** 2).sqrt()
+                / float(np.linalg.norm(vec2))
+            )
+            .cast(pl.Float32)
+            .alias("cosphi"),
+        )
+
+        # vec1 = dir cross syn_dir
+        dfpackets = dfpackets.with_columns(
+            ((pl.col("diry") * syn_dir[2] - pl.col("dirz") * syn_dir[1]) / pl.col("dirmag")).alias("vec1_x"),
+            ((pl.col("dirz") * syn_dir[0] - pl.col("dirx") * syn_dir[2]) / pl.col("dirmag")).alias("vec1_y"),
+            ((pl.col("dirx") * syn_dir[1] - pl.col("diry") * syn_dir[0]) / pl.col("dirmag")).alias("vec1_z"),
+        )
+
+        vec3 = np.cross(vec2, syn_dir)
+
+        # arr_testphi = np.dot(arr_vec1, vec3)
+        dfpackets = dfpackets.with_columns(
+            ((pl.col("vec1_x") * vec3[0] + pl.col("vec1_y") * vec3[1] + pl.col("vec1_z") * vec3[2]) / pl.col("dirmag"))
+            .cast(pl.Float32)
+            .alias("testphi"),
+        )
+
+        dfpackets = dfpackets.with_columns(
+            (
+                pl.when(pl.col("testphi") >= 0)
+                .then(pl.col("cosphi").arccos())
+                .otherwise(pl.col("cosphi").mul(-1.0).arccos() + np.pi)
+            )
+            .cast(pl.Float32)
+            .alias("phi"),
+        )
+
+    dfpackets = dfpackets.drop(["dirmag", "vec1_x", "vec1_y", "vec1_z"])
+
+    return dfpackets
+
+
+def bin_packet_directions_lazypolars(
+    dfpackets: pl.LazyFrame,
+    nphibins: Optional[int] = None,
+    ncosthetabins: Optional[int] = None,
+    phibintype: Literal["artis_pi_reversal", "monotonic"] = "artis_pi_reversal",
+) -> pl.LazyFrame:
+    if nphibins is None:
+        nphibins = at.get_viewingdirection_phibincount()
+
+    if ncosthetabins is None:
+        ncosthetabins = at.get_viewingdirection_costhetabincount()
 
-    # arr_testphi = np.dot(arr_vec1, vec3)
     dfpackets = dfpackets.with_columns(
-        (
-            (pl.col("vec1_x") * vec3[0] + pl.col("vec1_y") * vec3[1] + pl.col("vec1_z") * vec3[2]) / pl.col("dirmag")
-        ).alias("testphi"),
+        ((pl.col("costheta") + 1) / 2.0 * ncosthetabins).fill_nan(0.0).cast(pl.Int32).alias("costhetabin"),
     )
 
-    dfpackets = dfpackets.with_columns(
-        (
-            pl.when(pl.col("testphi") > 0)
-            .then(pl.col("cosphi").arccos() / 2.0 / np.pi * nphibins)
-            .otherwise((pl.col("cosphi").arccos() + np.pi) / 2.0 / np.pi * nphibins)
+    if phibintype == "monotonic":
+        dfpackets = dfpackets.with_columns(
+            (pl.col("phi") / 2.0 / np.pi * nphibins).fill_nan(0.0).cast(pl.Int32).alias("phibin"),
         )
-        .cast(pl.Int64)
-        .alias("phibin"),
-    )
+    else:
+        # for historical consistency, this binning is not monotonically increasing in phi angle,
+        # but switches to decreasing for phi > pi
+        dfpackets = dfpackets.with_columns(
+            (
+                pl.when(pl.col("testphi") >= 0)
+                .then(pl.col("cosphi").arccos() / 2.0 / np.pi * nphibins)
+                .otherwise((pl.col("cosphi").arccos() + np.pi) / 2.0 / np.pi * nphibins)
+            )
+            .fill_nan(0.0)
+            .cast(pl.Int32)
+            .alias("phibin"),
+        )
+
     dfpackets = dfpackets.with_columns(
-        (pl.col("costhetabin") * nphibins + pl.col("phibin")).alias("dirbin"),
+        (pl.col("costhetabin") * nphibins + pl.col("phibin")).cast(pl.Int32).alias("dirbin"),
     )
 
     return dfpackets
 
 
 def bin_packet_directions(modelpath: Union[Path, str], dfpackets: pd.DataFrame) -> pd.DataFrame:
     nphibins = at.get_viewingdirection_phibincount()
@@ -539,15 +648,15 @@
 
     arr_vec1 = np.cross(pktdirvecs, syn_dir)
     arr_cosphi = np.dot(arr_vec1, vec2) / np.linalg.norm(arr_vec1, axis=1) / np.linalg.norm(vec2)
     vec3 = np.cross(vec2, syn_dir)
     arr_testphi = np.dot(arr_vec1, vec3)
 
     arr_phibin = np.zeros(len(pktdirvecs), dtype=int)
-    filta = arr_testphi > 0
+    filta = arr_testphi >= 0
     arr_phibin[filta] = np.arccos(arr_cosphi[filta]) / 2.0 / np.pi * nphibins
     filtb = np.invert(filta)
     arr_phibin[filtb] = (np.arccos(arr_cosphi[filtb]) + np.pi) / 2.0 / np.pi * nphibins
     dfpackets["phibin"] = arr_phibin
     dfpackets["arccoscosphi"] = np.arccos(arr_cosphi)
 
     dfpackets["dirbin"] = (arr_costhetabin * nphibins) + arr_phibin
@@ -711,46 +820,40 @@
 def bin_and_sum(
     df: Union[pl.DataFrame, pl.LazyFrame],
     bincol: str,
     bins: list[Union[float, int]],
     sumcols: Optional[list[str]] = None,
     getcounts: bool = False,
 ) -> pl.DataFrame:
-    """bins is a list of lower edges, and the final upper edge"""
-
+    """Bins is a list of lower edges, and the final upper edge."""
     # Polars method
-    df = df.with_columns(
-        [
-            (
-                df.select(bincol)
-                .lazy()
-                .collect()[bincol]
-                .cut(
-                    bins=list(bins),
-                    category_label=bincol + "_bin",
-                    maintain_order=True,
-                )
-                .get_column(bincol + "_bin")
-                .cast(pl.Int32)
-                - 1  # subtract 1 because the returned index 0 is the bin below the start of the first supplied bin
-            )
-        ]
+
+    binindex = (
+        df.select(bincol)
+        .lazy()
+        .collect()
+        .get_column(bincol)
+        .cut(bins=list(bins), category_label=bincol + "_bin", maintain_order=True)
+        .get_column(bincol + "_bin")
+        .cast(pl.Int32)
+        - 1  # subtract 1 because the returned index 0 is the bin below the start of the first supplied bin
     )
+    df = df.with_columns([binindex])
 
     if sumcols is not None:
         aggs = [pl.col(col).sum().alias(col + "_sum") for col in sumcols]
 
     if getcounts:
         aggs.append(pl.col(bincol).count().alias("count"))
 
     wlbins = df.groupby(bincol + "_bin").agg(aggs).lazy().collect()
 
     # now we will include the empty bins
-    dfout = pl.DataFrame(pl.Series(bincol + "_bin", np.arange(0, len(bins) - 1), dtype=pl.Int32))
-    dfout = dfout.join(wlbins, how="left", on=bincol + "_bin").fill_null(0.0)
+    dfout = pl.DataFrame(pl.Series(name=bincol + "_bin", values=np.arange(0, len(bins) - 1), dtype=pl.Int32))
+    dfout = dfout.join(wlbins, how="left", on=bincol + "_bin").fill_null(0)
 
     # pandas method
 
     # dfout2 = pd.DataFrame({bincol + "_bin": np.arange(0, len(bins) - 1)})
     # if isinstance(df, pl.DataFrame):
     #     df2 = df.to_pandas(use_pyarrow_extension_array=True)
```

### Comparing `artistools-2023.4.19.2/artistools/packets/packetsplots.py` & `artistools-2023.5.16/artistools/packets/packetsplots.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/plottools.py` & `artistools-2023.5.16/artistools/plottools.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def set_mpl_style() -> None:
     plt.style.use("file://" + str(get_config()["path_artistools_dir"] / "matplotlibrc"))
 
 
 class ExponentLabelFormatter(ticker.ScalarFormatter):
     """Formatter to move the 'x10^x' offset text into the axis label."""
 
-    def __init__(self, labeltemplate, useMathText=True, decimalplaces=None):
+    def __init__(self, labeltemplate, useMathText=True, decimalplaces=None) -> None:
         self.set_labeltemplate(labeltemplate)
         self.decimalplaces = decimalplaces
         super().__init__(useOffset=True, useMathText=useMathText)
         # ticker.ScalarFormatter.__init__(self, useOffset=useOffset, useMathText=useMathText)
 
     def _set_formatted_label_text(self):
         # or use self.orderOfMagnitude
@@ -155,23 +155,23 @@
 
     return data, extent
 
 
 def autoscale(ax=None, axis="y", margin=0.1):
     """Autoscales the x or y axis of a given matplotlib ax object
     to fit the margins set by manually limits of the other axis,
-    with margins in fraction of the width of the plot
+    with margins in fraction of the width of the plot.
 
     Defaults to current axes object if not specified.
     From https://stackoverflow.com/questions/29461608/matplotlib-fixing-x-axis-scale-and-autoscale-y-axis
     """
 
     def calculate_new_limit(fixed, dependent, limit):
         """Calculates the min/max of the dependent axis given
-        a fixed axis with limits
+        a fixed axis with limits.
         """
         if len(fixed) > 2:
             mask = (fixed > limit[0]) & (fixed < limit[1]) & (~np.isnan(dependent)) & (~np.isnan(fixed))
             window = dependent[mask]
             try:
                 low, high = window.min(), window.max()
             except ValueError:  # Will throw ValueError if `window` has zero elements
@@ -182,21 +182,22 @@
             if low == 0.0 and high == 1.0:
                 # This is a axhline in the autoscale direction
                 low = np.inf
                 high = -np.inf
         return low, high
 
     def get_xy(artist):
-        """Gets the xy coordinates of a given artist"""
+        """Get the xy coordinates of a given artist."""
         if "Collection" in str(artist):
             x, y = artist.get_offsets().T
         elif "Line" in str(artist):
             x, y = artist.get_xdata(), artist.get_ydata()
         else:
-            raise ValueError("This type of object isn't implemented yet")
+            msg = "This type of object isn't implemented yet"
+            raise ValueError(msg)
         return x, y
 
     if ax is None:
         ax = plt.gca()
     newlow, newhigh = np.inf, -np.inf
 
     for artist in ax.collections + ax.lines:
```

### Comparing `artistools-2023.4.19.2/artistools/radfield.py` & `artistools-2023.5.16/artistools/radfield.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 import argparse
 import math
-import multiprocessing
-import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Optional
+from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
@@ -228,29 +227,30 @@
         )
 
     return ymax
 
 
 def plot_specout(
     axis,
-    specfilename,
+    specfilename: Union[str, Path],
     timestep: int,
     peak_value: Optional[float] = None,
     scale_factor: Optional[float] = None,
     **plotkwargs,
 ) -> None:
     """Plot the ARTIS spectrum."""
     print(f"Plotting {specfilename}")
 
-    if os.path.isdir(specfilename):
+    specfilename = Path(specfilename)
+    if specfilename.is_dir():
         modelpath = specfilename
-    elif os.path.isfile(specfilename):
+    elif specfilename.is_file():
         modelpath = Path(specfilename).parent
 
-    dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=modelpath)[-1]
+    dfspectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep)[-1]
     label = "Emergent spectrum"
     if scale_factor is not None:
         label += " (scaled)"
         dfspectrum["f_lambda"] = dfspectrum["f_lambda"] * scale_factor
 
     if peak_value is not None:
         label += " (normalised)"
@@ -968,17 +968,15 @@
 
     parser.add_argument("-o", action="store", dest="outputfile", type=Path, help="Filename for PDF file")
 
 
 def main(args=None, argsraw=None, **kwargs):
     """Plot the radiation field estimators."""
     if args is None:
-        parser = argparse.ArgumentParser(
-            formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS internal radiation field estimators."
-        )
+        parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     at.set_mpl_style()
 
     defaultoutputfile = (
@@ -1042,9 +1040,8 @@
         print(pdf_list, modelpath_list)
         at.join_pdf_files(pdf_list, modelpath_list)
 
     return 0
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/spectra/__init__.py` & `artistools-2023.5.16/artistools/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/spectra/plotspectra.py` & `artistools-2023.5.16/artistools/spectra/plotspectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import numpy as np
 import pandas as pd
 from matplotlib import ticker
 from matplotlib.artist import Artist
 
 import artistools as at
 import artistools.packets
+
 from .spectra import get_from_packets
 from .spectra import get_reference_spectrum
 from .spectra import get_specpol_data
 from .spectra import get_spectrum
 from .spectra import get_vspecpol_spectrum
 from .spectra import make_averaged_vspecfiles
 from .spectra import make_virtual_spectra_summed_file
@@ -145,25 +146,25 @@
 
     print(" metadata: " + ", ".join([f"{k}='{v}'" if hasattr(v, "lower") else f"{k}={v}" for k, v in metadata.items()]))
 
     specdata = specdata.query("lambda_angstroms > @xmin and lambda_angstroms < @xmax")
 
     print_integrated_flux(specdata["f_lambda"], specdata["lambda_angstroms"], distance_megaparsec=metadata["dist_mpc"])
 
-    if len(specdata) > 5000:
-        # specdata = scipy.signal.resample(specdata, 10000)
-        # specdata = specdata.iloc[::3, :].copy()
-        print(f" downsampling to {len(specdata)} points")
-        specdata = specdata.query("index % 3 == 0")
+    # if len(specdata) > 5000:
+    #     # specdata = scipy.signal.resample(specdata, 10000)
+    #     # specdata = specdata.iloc[::3, :].copy()
+    #     print(f" downsampling to {len(specdata)} points")
+    #     specdata = specdata.query("index % 3 == 0")
 
     # clamp negative values to zero
     # specdata['f_lambda'] = specdata['f_lambda'].apply(lambda x: max(0, x))
 
     if flambdafilterfunc:
-        specdata["f_lambda"] = flambdafilterfunc(specdata["f_lambda"])
+        specdata.loc[:, "f_lambda"] = flambdafilterfunc(specdata["f_lambda"])
 
     if scale_to_peak:
         specdata["f_lambda_scaled"] = specdata["f_lambda"] / specdata["f_lambda"].max() * scale_to_peak
         ycolumnname = "f_lambda_scaled"
     else:
         ycolumnname = "f_lambda"
 
@@ -203,19 +204,18 @@
     directionbins: Optional[list[int]] = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     maxpacketfiles: Optional[int] = None,
     **plotkwargs,
 ) -> Optional[pd.DataFrame]:
     """Plot an ARTIS output spectrum. The data plotted are also returned as a DataFrame."""
-
     modelpath = Path(modelpath)
     if Path(modelpath).is_file():  # handle e.g. modelpath = 'modelpath/spec.out'
         specfilename = Path(modelpath).parts[-1]
-        print("WARNING: ignoring filename of {specfilename}")
+        print(f"WARNING: ignoring filename of {specfilename}")
         modelpath = Path(modelpath).parent
 
     if not modelpath.is_dir():
         print(f"WARNING: Skipping because {modelpath} does not exist")
         return None
 
     if directionbins is None:
@@ -989,15 +989,24 @@
     # plt.text(6000, (args.ymax * 0.9), f'{round(args.timemin) + 1} days', fontsize='large')
 
     if args.showtime and not args.multispecplot:
         if not args.ymax:
             ymin, ymax = ax.get_ylim()
         else:
             ymax = args.ymax
-        plt.text(5500, (ymax * 0.9), f"{int(round(args.timemin) + 1)} days", fontsize="large")
+
+        timeavg = (args.timemin + args.timemax) / 2.0
+        ax.annotate(
+            f"{timeavg:.2f} days",
+            xy=(0.03, 0.97),
+            xycoords="axes fraction",
+            horizontalalignment="left",
+            verticalalignment="top",
+            fontsize="x-large",
+        )
 
     if args.write_data and not dfalldata.empty:
         print(dfalldata)
         datafilenameout = Path(filenameout).with_suffix(".txt")
         dfalldata.to_csv(datafilenameout)
         print(f"Saved {datafilenameout}")
 
@@ -1264,17 +1273,15 @@
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
     """Plot spectra from ARTIS and reference data."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description=(
-                "Plot ARTIS model spectra by finding spec.out files in the current directory or subdirectories."
-            ),
+            description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
         if args.average_every_tenth_viewing_angle:
             print("WARNING: --average_every_tenth_viewing_angle is deprecated. use --average_over_phi_angle instead")
```

### Comparing `artistools-2023.4.19.2/artistools/spectra/sampleblackbodyfrompacketTR.py` & `artistools-2023.5.16/artistools/spectra/sampleblackbodyfrompacketTR.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/spectra/spectra.py` & `artistools-2023.5.16/artistools/spectra/spectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,16 +65,16 @@
     return array_lambdabinedges, array_lambda, delta_lambda
 
 
 def stackspectra(
     spectra_and_factors: list[tuple[np.ndarray[Any, np.dtype[np.float64]], float]]
 ) -> np.ndarray[Any, np.dtype[np.float64]]:
     """Add spectra using weighting factors, i.e., specout[nu] = spec1[nu] * factor1 + spec2[nu] * factor2 + ...
-    spectra_and_factors should be a list of tuples: spectra[], factor"""
-
+    spectra_and_factors should be a list of tuples: spectra[], factor.
+    """
     factor_sum = sum([factor for _, factor in spectra_and_factors])
 
     stackedspectrum = np.zeros_like(spectra_and_factors[0][0], dtype=float)
     for spectrum, factor in spectra_and_factors:
         stackedspectrum += spectrum * factor / factor_sum
 
     return stackedspectrum
@@ -244,15 +244,15 @@
             dfdict[dirbin]["packetcount"] = dfbinned["count"]
 
     return dfdict
 
 
 @lru_cache(maxsize=16)
 def read_spec_res(modelpath: Path) -> dict[int, pd.DataFrame]:
-    """Return dataframe of time-series spectra for every viewing direction"""
+    """Return dataframe of time-series spectra for every viewing direction."""
     specfilename = (
         modelpath
         if Path(modelpath).is_file()
         else at.firstexisting(["spec_res.out", "specpol_res.out"], folder=modelpath, tryzipped=True)
     )
 
     print(f"Reading {specfilename} (in read_spec_res)")
@@ -511,15 +511,15 @@
 def get_vspecpol_data(
     vspecangle: Optional[int] = None, modelpath: Optional[Path] = None, specdata: Optional[pd.DataFrame] = None
 ) -> dict[str, pd.DataFrame]:
     if specdata is None:
         assert modelpath is not None
         # alternatively use f'vspecpol_averaged-{angle}.out' ?
         vspecpath = modelpath
-        if os.path.isdir(modelpath / "vspecpol"):
+        if (modelpath / "vspecpol").is_dir():
             vspecpath = modelpath / "vspecpol"
 
         try:
             specfilename = at.firstexisting(f"vspecpol_total-{vspecangle}.out", folder=vspecpath, tryzipped=True)
         except FileNotFoundError:
             print(f"vspecpol_total-{vspecangle}.out does not exist. Generating all-rank summed vspec files..")
             specfilename = make_virtual_spectra_summed_file(modelpath=modelpath)
@@ -573,15 +573,15 @@
 
     nu = vspecdata.loc[:, "nu"].to_numpy()
 
     arr_tmid = [float(i) for i in vspecdata.columns.to_numpy()[1:] if i[-2] != "."]
     arr_tdelta = [l1 - l2 for l1, l2 in zip(arr_tmid[1:], arr_tmid[:-1])] + [arr_tmid[-1] - arr_tmid[-2]]
 
     def match_closest_time(reftime: float) -> str:
-        return str("{}".format(min([float(x) for x in arr_tmid], key=lambda x: abs(x - reftime))))
+        return str(f"{min([float(x) for x in arr_tmid], key=lambda x: abs(x - reftime))}")
 
     # if 'timemin' and 'timemax' in args:
     #     timelower = match_closest_time(args.timemin)  # how timemin, timemax are used changed at some point
     #     timeupper = match_closest_time(args.timemax)  # to average over multiple timesteps needs to fix this
     # else:
     timelower = match_closest_time(timeavg)
     timeupper = match_closest_time(timeavg)
@@ -810,20 +810,22 @@
         adata = at.atomic.get_levels(modelpath)
 
     def get_emprocesslabel(
         linelist: dict[int, at.linetuple], bflist: dict[int, tuple[int, int, int, int]], emtype: int
     ) -> str:
         if emtype >= 0:
             line = linelist[emtype]
+
             if groupby == "line":
                 return (
                     f"{at.get_ionstring(line.atomic_number, line.ionstage)} "
                     f"λ{line.lambda_angstroms:.0f} "
                     f"({line.upperlevelindex}-{line.lowerlevelindex})"
                 )
+
             if groupby == "terms":
                 upper_config = (
                     adata.query("Z == @line.atomic_number and ion_stage == @line.ionstage", inplace=False)
                     .iloc[0]
                     .levels.iloc[line.upperlevelindex]
                     .levelname
                 )
@@ -832,33 +834,37 @@
                     adata.query("Z == @line.atomic_number and ion_stage == @line.ionstage", inplace=False)
                     .iloc[0]
                     .levels.iloc[line.lowerlevelindex]
                     .levelname
                 )
                 lower_term_noj = lower_config.split("_")[-1].split("[")[0]
                 return f"{at.get_ionstring(line.atomic_number, line.ionstage)} {upper_term_noj}->{lower_term_noj}"
+
             if groupby == "upperterm":
                 upper_config = (
                     adata.query("Z == @line.atomic_number and ion_stage == @line.ionstage", inplace=False)
                     .iloc[0]
                     .levels.iloc[line.upperlevelindex]
                     .levelname
                 )
                 upper_term_noj = upper_config.split("_")[-1].split("[")[0]
                 return f"{at.get_ionstring(line.atomic_number, line.ionstage)} {upper_term_noj}"
+
             return f"{at.get_ionstring(line.atomic_number, line.ionstage)} bound-bound"
+
         if emtype == -9999999:
             return "free-free"
 
         bfindex = -emtype - 1
         if bfindex in bflist:
             (atomic_number, ionstage, level) = bflist[bfindex][:3]
             if groupby == "line":
                 return f"{at.get_ionstring(atomic_number, ionstage)} bound-free {level}"
             return f"{at.get_ionstring(atomic_number, ionstage)} bound-free"
+
         return f"? bound-free (bfindex={bfindex})"
 
     def get_absprocesslabel(linelist: dict[int, at.linetuple], abstype: int) -> str:
         if abstype >= 0:
             line = linelist[abstype]
             if groupby == "line":
                 return (
@@ -1301,10 +1307,10 @@
                     spec_file, header=False, sep=" ", index=False, columns=["lambda_angstroms", "f_lambda"]
                 )
 
             spectra_list.write(str(outfilepath.absolute()) + "\n")
 
     with open(outdirectory / "time_list.txt", "w+") as time_list:
         for time in arr_tmid:
-            time_list.write(f"{str(time)} \n")
+            time_list.write(f"{time} \n")
 
     print(f"Saved in {outdirectory}")
```

### Comparing `artistools-2023.4.19.2/artistools/spectra/test_spectra.py` & `artistools-2023.5.16/artistools/spectra/test_spectra.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 #!/usr/bin/env python3
 import math
-import os.path
+from pathlib import Path
+from unittest import mock
 
+import matplotlib.axes
 import numpy as np
 import pandas as pd
 from astropy import constants as const
 
 import artistools as at
 
 modelpath = at.get_config()["path_testartismodel"]
 outputpath = at.get_config()["path_testoutput"]
 
 
-def test_spectraplot() -> None:
+@mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
+def test_spectraplot(mockplot) -> None:
     at.spectra.plot(
         argsraw=[],
         specpath=[modelpath, "sn2011fe_PTF11kly_20120822_norm.txt"],
         outputfile=outputpath,
         timemin=290,
         timemax=320,
     )
 
+    arr_lambda = np.array(mockplot.call_args[0][1])
+    arr_f_lambda = np.array(mockplot.call_args[0][2])
 
-def test_spectra_frompackets() -> None:
+    integral = np.trapz(y=arr_f_lambda, x=arr_lambda)
+    assert np.isclose(integral, 5.870730903198916e-11, atol=1e-14)
+
+
+@mock.patch.object(matplotlib.axes.Axes, "plot", side_effect=matplotlib.axes.Axes.plot, autospec=True)
+def test_spectra_frompackets(mockplot) -> None:
     at.spectra.plot(
         argsraw=[],
         specpath=modelpath,
-        outputfile=os.path.join(outputpath, "spectrum_from_packets.pdf"),
+        outputfile=Path(outputpath, "spectrum_from_packets.pdf"),
         timemin=290,
         timemax=320,
         frompackets=True,
     )
 
+    arr_lambda = np.array(mockplot.call_args[0][1])
+    arr_f_lambda = np.array(mockplot.call_args[0][2])
+
+    integral = np.trapz(y=arr_f_lambda, x=arr_lambda)
+
+    assert np.isclose(integral, 6.7118e-12, atol=1e-14)
+
 
 def test_spectra_outputtext() -> None:
     at.spectra.plot(argsraw=[], specpath=modelpath, output_spectra=True)
 
 
 def test_spectraemissionplot() -> None:
     at.spectra.plot(
```

### Comparing `artistools-2023.4.19.2/artistools/spectra/test_vspectra.py` & `artistools-2023.5.16/artistools/spectra/test_vspectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/artistools/stats.py` & `artistools-2023.5.16/artistools/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python3
 import glob
-import multiprocessing
 import sys
 
 import matplotlib.pyplot as plt
 
 xminvalue, xmaxvalue = 3500, 7000
-# xminvalue, xmaxvalue = 10000, 20000
 
 h = 6.62607004e-34  # m^2 kg / s
 c = 299792458  # m / s
 
 
 def main():
     logfiles = glob.glob("output_0-0.txt") + glob.glob("*/output_0-0.txt") + glob.glob("*/*/output_0-0.txt")
@@ -44,30 +42,27 @@
                 if line.startswith("k_stat_"):
                     (key, value) = line.split(" = ")
                     stats[-1][key] = int(value)
 
         linelabel = runfolder
 
         linestyle = ["-", "--"][int(index / 7)]
-        # xvalues = range(len(stats))
         yvalues = [timestepstats["k_stat_to_r_fb"] for timestepstats in stats]
         axes[0].plot(timesteptimes, yvalues, linestyle=linestyle, linewidth=1.5, label=linelabel)
         yvalues = [timestepstats["k_stat_to_ma_collexc"] for timestepstats in stats]
         axes[1].plot(timesteptimes, yvalues, linestyle=linestyle, linewidth=1.5, label=linelabel)
 
     for axis in axes:
         axis.set_xlim(250, 300)
-        # axis.set_ylim(-0.1, 1.3)
 
     axes[0].legend(loc="best", handlelength=2, frameon=False, numpoints=1, prop={"size": 9})
     axes[-1].set_xlabel(r"Time (days)")
     # ax.xaxis.set_minor_locator(ticker.MultipleLocator(base=5))
     axes[0].set_ylabel(r"k_stat_to_r_fb")
     axes[1].set_ylabel(r"k_stat_to_ma_collexc")
 
     fig.savefig("plotartisstats.pdf", format="pdf")
     plt.close()
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/test_artistools.py` & `artistools-2023.5.16/artistools/test_artistools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,119 @@
 #!/usr/bin/env python3
 import hashlib
 import math
+from typing import Any
 
 import numpy as np
 
 import artistools as at
 
 modelpath = at.get_config()["path_testartismodel"]
 outputpath = at.get_config()["path_testoutput"]
 
 
-def test_commands():
+def test_commands() -> None:
     import importlib
 
     # ensure that the commands are pointing to valid submodule.function() targets
     for _command, (submodulename, funcname) in sorted(at.commands.get_commandlist().items()):
         submodule = importlib.import_module(submodulename, package="artistools")
         assert hasattr(submodule, funcname)
 
+    def recursive_check(dictcmd: dict[str, Any]) -> None:
+        for cmdtarget in dictcmd.values():
+            if isinstance(cmdtarget, dict):
+                recursive_check(cmdtarget)
+            else:
+                submodulename, funcname = cmdtarget
+                namestr = f"artistools.{submodulename.removeprefix('artistools.')}" if submodulename else "artistools"
+                submodule = importlib.import_module(namestr, package="artistools")
+                assert hasattr(submodule, funcname)
 
-def test_timestep_times():
+    recursive_check(at.commands.dictcommands)
+
+
+def test_timestep_times() -> None:
     timestartarray = at.get_timestep_times_float(modelpath, loc="start")
     timedeltarray = at.get_timestep_times_float(modelpath, loc="delta")
     timemidarray = at.get_timestep_times_float(modelpath, loc="mid")
     assert len(timestartarray) == 100
     assert math.isclose(float(timemidarray[0]), 250.421, abs_tol=1e-3)
     assert math.isclose(float(timemidarray[-1]), 349.412, abs_tol=1e-3)
 
     assert all(
         tstart < tmid < (tstart + tdelta) for tstart, tdelta, tmid in zip(timestartarray, timedeltarray, timemidarray)
     )
 
 
-def test_deposition():
+def test_deposition() -> None:
     at.deposition.main(argsraw=[], modelpath=modelpath)
 
 
-def test_estimator_snapshot():
+def test_estimator_snapshot() -> None:
     at.estimators.plot(argsraw=[], modelpath=modelpath, outputfile=outputpath, timedays=300)
 
 
-def test_estimator_timeevolution():
+def test_estimator_timeevolution() -> None:
     at.estimators.plot(argsraw=[], modelpath=modelpath, outputfile=outputpath, modelgridindex=0, x="time")
 
 
-def test_get_inputparams():
+def test_get_inputparams() -> None:
     inputparams = at.get_inputparams(modelpath)
     dicthash = hashlib.sha256(str(sorted(inputparams.items())).encode("utf-8")).hexdigest()
     assert dicthash == "ce7d04d6944207673a105cba8d2430055d0b53b7f3e92db3964d2dca285a3adb"
 
 
-def test_get_levels():
+def test_get_levels() -> None:
     at.atomic.get_levels(modelpath, get_transitions=True, get_photoionisations=True)
 
 
-def test_get_modeldata_tuple():
+def test_get_modeldata_tuple() -> None:
     dfmodel, t_model_init_days, vmax_cmps = at.inputmodel.get_modeldata_tuple(modelpath, get_elemabundances=True)
     assert np.isclose(t_model_init_days, 0.00115740740741, rtol=0.0001)
     assert np.isclose(vmax_cmps, 800000000.0, rtol=0.0001)
 
     # assert (
     #     hashlib.sha256(pd.util.hash_pandas_object(dfmodel, index=True).values).hexdigest() ==
     #     '40a02dfa933f6b28671d42f3cf69a182955a5a89dc93bbcd22c894192375fe9b')
 
 
-def test_macroatom():
+def test_macroatom() -> None:
     at.macroatom.main(argsraw=[], modelpath=modelpath, outputfile=outputpath, timestep=10)
 
 
-def test_nltepops():
+def test_nltepops() -> None:
     # at.nltepops.plot(modelpath=modelpath, outputfile=outputpath, timedays=300),
     #                    **benchargs)
     at.nltepops.plot(argsraw=[], modelpath=modelpath, outputfile=outputpath, timestep=40)
 
 
-def test_nonthermal():
+def test_nonthermal() -> None:
     at.nonthermal.plot(argsraw=[], modelpath=modelpath, outputfile=outputpath, timestep=70)
 
 
-def test_radfield():
+def test_radfield() -> None:
     at.radfield.main(argsraw=[], modelpath=modelpath, modelgridindex=0, outputfile=outputpath)
 
 
-def test_get_ionrecombratecalibration():
+def test_get_ionrecombratecalibration() -> None:
     at.atomic.get_ionrecombratecalibration(modelpath=modelpath)
 
 
-def test_spencerfano():
+def test_plotspherical() -> None:
+    at.plotspherical.main(argsraw=[], modelpath=modelpath, interpolate=True, outputfile=outputpath)
+
+
+def test_spencerfano() -> None:
     at.nonthermal.solvespencerfanocmd.main(
         argsraw=[], modelpath=modelpath, timedays=300, makeplot=True, npts=200, noexcitation=True, outputfile=outputpath
     )
 
 
-def test_transitions():
+def test_transitions() -> None:
     at.transitions.main(argsraw=[], modelpath=modelpath, outputfile=outputpath, timedays=300)
+
+
+def test_write_comparisondata() -> None:
+    at.writecomparisondata.main(
+        argsraw=[], modelpath=modelpath, outputpath=outputpath, selected_timesteps=list(range(99))
+    )
```

### Comparing `artistools-2023.4.19.2/artistools/transitions.py` & `artistools-2023.5.16/artistools/transitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 import argparse
 import math
-import multiprocessing
 import sys
 from collections import namedtuple
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
@@ -220,19 +219,20 @@
     )
 
     parser.add_argument(
         "-o", action="store", dest="outputfile", default=defaultoutputfile, help="path/filename for PDF file"
     )
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
+    """Plot estimated spectra from bound-bound transitions."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Plot estimated spectra from bound-bound transitions.",
+            description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if Path(args.outputfile).is_dir():
         args.outputfile = Path(args.outputfile, defaultoutputfile)
@@ -325,15 +325,15 @@
         # -1 means use NLTE populations
         temperature_list = ["Te", "TR", "-1"]
         temperature_list = ["-1"]
         vardict = {"Te": Te, "TR": TR}
     else:
         if not args.T:
             args.T = [2000]
-        figure_title = f"Te = {args.T[0]:.1f}" if len(args.T) == 1 else None
+        figure_title = f"Te = {args.T[0]:.1f}" if len(args.T) == 1 else ""
 
         temperature_list = []
         vardict = {}
         for index, temperature in enumerate(args.T):
             tlabel = "Te"
             if index > 0:
                 tlabel += f"_{index + 1}"
@@ -506,9 +506,8 @@
         args.xmax,
         figure_title,
         outputfilename,
     )
 
 
 if __name__ == "__main__":
-    multiprocessing.freeze_support()
     main()
```

### Comparing `artistools-2023.4.19.2/artistools/viewing_angles_visualization.py` & `artistools-2023.5.16/artistools/viewing_angles_visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 #!/usr/bin/env python3
 import argparse
 import sys
 
 import numpy as np
 import pandas as pd
 
-
-def load_artis_model(modelfile):
-    with open(modelfile) as f:
-        n = f.readline()
-        res = int(np.cbrt(int(n)))
-        rho = np.zeros([res, res, res])
-        x = np.zeros([res, res, res])
-        y = np.zeros([res, res, res])
-        z = np.zeros([res, res, res])
-
-        t_model = f.readline()
-        _ = f.readline()
-
-        for l in range(0, res):
-            for k in range(0, res):
-                for i in range(0, res):
-                    _, dum2, dum3, dum4, rhoread = f.readline().split()
-                    _, _, _, _, _ = f.readline().split()
-                    rho[i, k, l] = rhoread
-                    x[i, k, l] = dum2
-                    y[i, k, l] = dum3
-                    z[i, k, l] = dum4
-
-    return x, y, z, rho, t_model, res
+import artistools as at
 
 
 def get_theta_phi(anglebin):
     assert isinstance(anglebin, int), "Anglebin has to be int"
     cos_theta = [
         -0.9,
         -0.7,
@@ -103,27 +80,26 @@
         viewing_angles["x_coord"].append(x_c)
         viewing_angles["y_coord"].append(y_c)
         viewing_angles["z_coord"].append(z_c)
 
     return pd.DataFrame(viewing_angles)
 
 
-def main(
+def viewing_angles_visualisation(
     modelfile,
     outfile=None,
     isomin=None,
     isomax=None,
     opacity=2.5,
     surface_count=20,
     linewidth=2.5,
     linelength=1.0,
     show_plot=False,
 ):
-    """
-    Tool to generate a 3D visualization of an ARTIS model.
+    """Tool to generate a 3D visualization of an ARTIS model.
     Viewing angle bins will get overplottet with an animation.
 
     Parameters
     ----------
     modelfile : str
         File where ARTIS  model is stored.
     outfile : str
@@ -154,16 +130,18 @@
         import plotly.express as px
         import plotly.graph_objects as go
     except ModuleNotFoundError:
         print("Cannot run visualization without plotly...")
         sys.exit()
 
     # Load model contents
-    x, y, z, rho, _, res = load_artis_model(modelfile)
-    print("Found model with %d cubed resolution" % res)
+    dfmodel, modelmeta = at.get_modeldata(modelfile, derived_cols=["pos_mid"], dtype_backend="pyarrow")
+    x, y, z = (dfmodel[f"pos_{ax}_mid"].to_numpy() for ax in ("x", "y", "z"))
+    rho = dfmodel["rho"].to_numpy()
+    res = modelmeta["ncoordgrid"]
 
     if isomin is None:
         isomin = min(rho.flatten())
     if isomax is None:
         isomax = max(rho.flatten())
 
     # Generate viewing angle vectory
@@ -269,29 +247,30 @@
     parser.add_argument(
         "--show_plot",
         action="store_true",
         help="If flag is given, plot will be shown after saving.",
     )
 
 
-def cli():
+def main() -> None:
+    """Tool to generate a 3D visualization of an ARTIS model."""
     parser = argparse.ArgumentParser()
 
     addargs(parser)
 
     args = parser.parse_args()
 
-    main(
+    viewing_angles_visualisation(
         modelfile=args.modelfile,
         outfile=args.outfile,
         isomin=args.isomin,
         isomax=args.isomax,
         opacity=args.opacity,
         surface_count=args.surface_count,
         linewidth=args.linewidth,
         linelength=args.linelength,
         show_plot=args.show_plot,
     )
 
 
 if __name__ == "__main__":
-    cli()
+    main()
```

### Comparing `artistools-2023.4.19.2/artistools/writecomparisondata.py` & `artistools-2023.5.16/artistools/writecomparisondata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+"""Tools to get artis output in the required format for the code comparison workshop."""
 import argparse
 from pathlib import Path
 
 import numpy as np
 
 import artistools as at
 
@@ -26,40 +27,36 @@
 
     # convert flux to power by multiplying by area
     for n in range(1000):
         # 2.99792458e18 is c in Angstrom / second
         lum_lambda[n, :] = fluxes_nu[n, :] * 2.99792458e18 / lambdas[n] / lambdas[n] * area
 
     with open(outfile, "w") as f:
-        f.write("#NTIMES: {}\n".format(len(selected_timesteps)))
-        f.write("#NWAVE: {}\n".format(len(lambdas)))
-        f.write("#TIMES[d]: {}\n".format(" ".join(["{:.2f}".format(times[ts]) for ts in selected_timesteps])))
+        f.write(f"#NTIMES: {len(selected_timesteps)}\n")
+        f.write(f"#NWAVE: {len(lambdas)}\n")
+        f.write("#TIMES[d]: {}\n".format(" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])))
         f.write("#wavelength[Ang] flux_t0[erg/s/Ang] flux_t1[erg/s/Ang] ... flux_tn[erg/s/Ang]\n")
 
         for n in reversed(range(len(lambdas))):
-            f.write(
-                "{:.2f} ".format(lambdas[n])
-                + " ".join(["{:.2e}".format(lum_lambda[n, ts]) for ts in selected_timesteps])
-                + "\n"
-            )
+            f.write(f"{lambdas[n]:.2f} " + " ".join([f"{lum_lambda[n, ts]:.2e}" for ts in selected_timesteps]) + "\n")
 
         f.close()
 
 
 def write_ntimes_nvel(f, selected_timesteps, modelpath):
     times = at.get_timestep_times_float(modelpath)
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
     f.write(f"#NTIMES: {len(selected_timesteps)}\n")
     f.write(f"#NVEL: {len(modeldata)}\n")
     f.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
 
 
-def write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist, outfile, keyname):
+def write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist, outfile, keyname) -> None:
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
-    with open(outfile, "w") as f:
+    with Path(outfile).open("w") as f:
         write_ntimes_nvel(f, selected_timesteps, modelpath)
         if keyname == "total_dep":
             f.write("#vel_mid[km/s] Edep_t0[erg/s/cm^3] Edep_t1[erg/s/cm^3] ... Edep_tn[erg/s/cm^3]\n")
         elif keyname == "nne":
             f.write("#vel_mid[km/s] ne_t0[/cm^3] ne_t1[/cm^3] … ne_tn[/cm^3]\n")
         elif keyname == "Te":
             f.write("#vel_mid[km/s] Tgas_t0[K] Tgas_t1[K] ... Tgas_tn[K]\n")
@@ -109,22 +106,22 @@
                         ion_stage = ion + elementlist.lowermost_ionstage[element]
                         ionabund = estimators[(timestep, modelgridindex)]["populations"].get(
                             (atomic_number, ion_stage), 0
                         )
                         ionfrac = ionabund / elabund if elabund > 0 else 0
                         if ionfrac > 0.0:
                             fileisallzeros = False
-                        f.write(" {:.4e}".format(ionfrac))
+                        f.write(f" {ionfrac:.4e}")
                     f.write("\n")
         if fileisallzeros:
             print(f"Deleting {pathfileout} because it is all zeros")
             pathfileout.unlink()
 
 
-def write_phys(modelpath, model_id, selected_timesteps, estimators, allnonemptymgilist, outputpath):
+def write_phys(modelpath, model_id, selected_timesteps, estimators, allnonemptymgilist, outputpath) -> None:
     times = at.get_timestep_times_float(modelpath)
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
     with open(Path(outputpath, f"phys_{model_id}_artisnebular.txt"), "w") as f:
         f.write(f"#NTIMES: {len(selected_timesteps)}\n")
         f.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
         f.write("#\n")
         for timestep in selected_timesteps:
@@ -143,15 +140,15 @@
                     "total"
                 ]
 
                 v_mid = (cell.velocity_inner + cell.velocity_outer) / 2.0
                 f.write(f"{v_mid:.2f}")
                 for keyname in ("Te", "rho", "nne", "nntot"):
                     estvalue = estimators[(timestep, modelgridindex)][keyname]
-                    f.write(" {:.4e}".format(estvalue))
+                    f.write(f" {estvalue:.4e}")
                 f.write("\n")
 
 
 def write_lbol_edep(modelpath, model_id, selected_timesteps, estimators, outputpath):
     # times = at.get_timestep_times_float(modelpath)
     dflightcurve = at.lightcurve.readfile(Path(modelpath, "light_curve.out"))[-1]
     dfdep = at.get_deposition(modelpath)
@@ -169,60 +166,62 @@
 
     f.close()
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=[], nargs="*", action=at.AppendPath, help="Paths to ARTIS folders")
 
-    parser.add_argument(
-        "-selected_timesteps", default=[], nargs="*", action=at.AppendPath, help="Selected ARTIS timesteps"
-    )
+    parser.add_argument("-selected_timesteps", default=[], nargs="*", type=int, help="Selected ARTIS timesteps")
 
     parser.add_argument("-outputpath", "-o", action="store", type=Path, default=Path(), help="path for output files")
 
 
 def main(args=None, argsraw=None, **kwargs):
-    """Plot spectra from ARTIS and reference data."""
+    """Write ARTIS model data out in code comparison workshop format."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
-            description="Write ARTIS model data out in code comparison workshop format.",
+            description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
-    if not args.modelpath and not args.specpath:
+    if not args.modelpath:
         args.modelpath = [Path(".")]
     elif isinstance(args.modelpath, (str, Path)):
         args.modelpath = [args.modelpath]
 
     modelpathlist = args.modelpath
     selected_timesteps = args.selected_timesteps
 
     args.outputpath.mkdir(parents=True, exist_ok=True)
 
     for modelpath in modelpathlist:
         model_id = str(modelpath.name).split("_")[0]
+        print(f"{model_id=}")
 
         modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
         estimators = at.estimators.read_estimators(modelpath=modelpath)
         allnonemptymgilist = [
             modelgridindex
             for modelgridindex in modeldata.index
             if not estimators[(selected_timesteps[0], modelgridindex)]["emptycell"]
         ]
 
-        write_lbol_edep(
-            modelpath,
-            model_id,
-            selected_timesteps,
-            estimators,
-            Path(args.outputpath, "lbol_edep_" + model_id + "_artisnebular.txt"),
-        )
+        try:
+            write_lbol_edep(
+                modelpath,
+                model_id,
+                selected_timesteps,
+                estimators,
+                Path(args.outputpath, "lbol_edep_" + model_id + "_artisnebular.txt"),
+            )
+        except FileNotFoundError:
+            print("Can't write deposition because files are missing")
 
         write_spectra(
             modelpath, model_id, selected_timesteps, Path(args.outputpath, "spectra_" + model_id + "_artisnebular.txt")
         )
 
         # write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist,
         #                        Path(args.outputpath, "eden_" + model_id + "_artisnebular.txt"), keyname='nne')
```

### Comparing `artistools-2023.4.19.2/artistools.egg-info/PKG-INFO` & `artistools-2023.5.16/artistools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artistools
-Version: 2023.4.19.2
+Version: 2023.5.16
 Summary: Plotting and analysis tools for the ARTIS 3D supernova radiative transfer code.
 Home-page: https://www.github.com/artis-mcrt/artistools/
 Author: ARTIS Collaboration
 Author-email: ARTIS Collaboration <luke.shingles@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `artistools-2023.4.19.2/artistools.egg-info/SOURCES.txt` & `artistools-2023.5.16/artistools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .codeclimate.yml
 .codecov.yml
-.flake8
 .git-blame-ignore-revs
 .gitattributes
 .gitignore
 .landscape.yml
 .pre-commit-config.yaml
 .python-version
 CODEOWNERS
@@ -26,14 +25,15 @@
 ./artistools/hesma_scripts.py
 ./artistools/initial_composition.py
 ./artistools/linefluxes.py
 ./artistools/logfiles.py
 ./artistools/macroatom.py
 ./artistools/matplotlibrc
 ./artistools/misc.py
+./artistools/plotspherical.py
 ./artistools/plottools.py
 ./artistools/radfield.py
 ./artistools/stats.py
 ./artistools/test_artistools.py
 ./artistools/transitions.py
 ./artistools/viewing_angles_visualization.py
 ./artistools/writecomparisondata.py
@@ -218,14 +218,15 @@
 artistools/hesma_scripts.py
 artistools/initial_composition.py
 artistools/linefluxes.py
 artistools/logfiles.py
 artistools/macroatom.py
 artistools/matplotlibrc
 artistools/misc.py
+artistools/plotspherical.py
 artistools/plottools.py
 artistools/radfield.py
 artistools/stats.py
 artistools/test_artistools.py
 artistools/transitions.py
 artistools/viewing_angles_visualization.py
 artistools/writecomparisondata.py
@@ -530,8 +531,11 @@
 images/fig-estimators.png
 images/fig-nlte-Ni.pdf
 images/fig-nlte-Ni.png
 tests/__init__.py
 tests/plottransitions_example.sh
 tests/data/.gitignore
 tests/data/setuptestdata.sh
+tests/data/testmodel_3d_10^3/.gitignore
+tests/data/testmodel_3d_10^3/abundances.txt.xz
+tests/data/testmodel_3d_10^3/model.txt.xz
 tests/output/.gitignore
```

### Comparing `artistools-2023.4.19.2/artistools.egg-info/entry_points.txt` & `artistools-2023.5.16/artistools.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 artistools-plotdensity = artistools.inputmodel.plotdensity:main
 artistools-radfield = artistools.radfield:main
 artistools-setup_completions = artistools.commands:setup_completions
 artistools-spectrum = artistools.spectra:main
 artistools-spencerfano = artistools.nonthermal.solvespencerfanocmd:main
 artistools-timesteptimes = artistools:showtimesteptimes
 artistools-transitions = artistools.transitions:main
-artistools-viewingangles = artistools.viewing_angles_visualization:cli
+artistools-viewingangles = artistools.viewing_angles_visualization:main
 artistools-writecodecomparisondata = artistools.writecomparisondata:main
 at = artistools:main
 getartisspencerfano = artistools.nonthermal.solvespencerfanocmd:main
 listartistimesteps = artistools:showtimesteptimes
 makeartismodel = artistools.inputmodel.makeartismodel:main
 makeartismodel1dslicefromcone = artistools.inputmodel.slice1Dfromconein3dmodel:main
 makeartismodelbotyanski2017 = artistools.inputmodel.botyanski2017:main
@@ -45,8 +45,8 @@
 plotartismodeldensity = artistools.inputmodel.plotdensity:main
 plotartismodeldeposition = artistools.deposition:main
 plotartisnltepops = artistools.nltepops.plotnltepops:main
 plotartisnonthermal = artistools.nonthermal:main
 plotartisradfield = artistools.radfield:main
 plotartisspectrum = artistools.spectra.plotspectra:main
 plotartistransitions = artistools.transitions:main
-plotartisviewingangles = artistools.viewing_angles_visualization:cli
+plotartisviewingangles = artistools.viewing_angles_visualization:main
```

### Comparing `artistools-2023.4.19.2/artistoolscompletions.sh` & `artistools-2023.5.16/artistoolscompletions.sh`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-emission.pdf` & `artistools-2023.5.16/images/fig-emission.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-emission.png` & `artistools-2023.5.16/images/fig-emission.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-estimators.pdf` & `artistools-2023.5.16/images/fig-estimators.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-estimators.png` & `artistools-2023.5.16/images/fig-estimators.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-nlte-Ni.pdf` & `artistools-2023.5.16/images/fig-nlte-Ni.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/images/fig-nlte-Ni.png` & `artistools-2023.5.16/images/fig-nlte-Ni.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.4.19.2/pyproject.toml` & `artistools-2023.5.16/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -62,41 +62,41 @@
   "redundant-expr",
   "truthy-bool",
   "ignore-without-code",
 ]
 
 [[tool.mypy.overrides]]
 module = [
-    "artistools.estimators.estimators",
+    "artistools",
+    "artistools.estimators",
+    "artistools.commands",
     "artistools.inputmodel",
     "artistools.lightcurve",
     "artistools.misc",
-#    "artistools.packets",
-    "artistools.spectra.spectra",
+    "artistools.packets",
+    "artistools.spectra",
 ]
 check_untyped_defs = true
 disallow_untyped_defs = true
 warn_return_any = false
 #strict = true
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
 disable = """
     broad-exception-caught,
-    dangerous-default-value,
     eval-used,
     fixme,
     global-statement,
     missing-function-docstring,
     missing-module-docstring,
     import-outside-toplevel,
     invalid-name,
     line-too-long,
     protected-access,
-    redefined-builtin,
     redefined-outer-name,
     too-many-arguments,
     too-many-branches,
     too-many-lines,
     too-many-locals,
     too-many-statements,
     unused-argument,
@@ -105,62 +105,66 @@
     C,
     R,
 """
 [tool.pylint.typecheck]
 ignored-modules = ["astropy", "extinction"]
 
 [tool.ruff]
-select = [
-    #"ALL",
-    "A", "B", "C", "E", "F", "G", "N", "Q", "W", "ARG", "BLE", "DJ", "DTZ", "EM", "ERA", "EXE",
-    "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PYI", "RET", "RSE", "RUF",
-    "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"
-]
+select = ["ALL"]
 ignore = [
     "ARG001", # ignored because variables in df.eval() are not detected
+    "ANN",
     "B005",
     "B007", # variable not used in loop body (but sometimes it is with eval)
     "BLE001",
-    "C9",
-    "D211", "D213",
+    "C901",
+    "COM812",
+    "D100", "D101", "D102", "D103", "D104", "D107", "D203", "D205", "D213", "D401", "D417",
     "E501", "E741",
-    "EM101","EM102",
     "ERA001",
     "F841", # ignored because variables in df.eval() are not detected
+    "FBT",
     "N802", "N803", "N806", "N999",
     "PD901",
     "PGH001",
     "PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004",
+    "PTH112",
+    "PTH113",
+    "PTH123",
+    "PTH118",
+    "PTH119",
+    "PTH120",
     "PLW2901",
-    "PT011",
     "RET504",
-    "SIM115",
+    "S",
     "SLF001",
-    "TRY003",
+    "T201",
     "TRY301",
-    "UP032",
-]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = [
-    "A", "B", "C", "E", "G", "N", "Q", "W", "ARG", "BLE", "DJ", "DTZ", "EM", "ERA", "EXE",
-    "FBT", "ICN", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PLR", "PT", "PTH", "PYI", "RET", "RSE",
-    "RUF", "SIM", "SLF", "TCH", "TID", "UP", "YTT"
 ]
+fixable = ["ALL"]
 unfixable = [
+    "COM812",
     "ERA001",  # commented out code (will just delete it!)
-    "F841",
-    "F401",
-    "PD002"
+    "F841",  # Local variable {name} is assigned to but never used
 ]
+line-length = 120
+target-version = "py39"
+fix = true
+show-fixes = true
+ignore-init-module-imports = true
 
-# larger than black's limit. Let black handle this
-line-length = 200
+[tool.ruff.flake8-annotations]
+ignore-fully-untyped = true
 
-target-version = "py39"
+[tool.ruff.flake8-import-conventions.extend-aliases]
+"artistools" = "at"
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
+[tool.ruff.isort]
+force-single-line = true
+order-by-type = false
+
 [tool.setuptools_scm]
 write_to = "_version.py"
 local_scheme = "no-local-version"
```

### Comparing `artistools-2023.4.19.2/setup.py` & `artistools-2023.5.16/setup.py`

 * *Files identical despite different names*

