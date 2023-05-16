# Comparing `tmp/yadism-0.9.1.tar.gz` & `tmp/yadism-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadism-0.9.1.tar", max compression
+gzip compressed data, was "yadism-0.9.2.tar", max compression
```

## Comparing `yadism-0.9.1.tar` & `yadism-0.9.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    35149 2021-10-19 10:37:51.506383 yadism-0.9.1/LICENSE
--rw-r--r--   0        0        0     2965 2021-10-19 10:37:51.506383 yadism-0.9.1/README.md
--rw-r--r--   0        0        0     3447 2021-10-19 10:39:24.245462 yadism-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      318 2021-10-19 10:39:24.245462 yadism-0.9.1/src/yadism/__init__.py
--rw-r--r--   0        0        0     8742 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/__init__.py
--rw-r--r--   0        0        0    13396 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/coupling_constants.py
--rw-r--r--   0        0        0       46 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/__init__.py
--rw-r--r--   0        0        0     1152 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/f2_cc.py
--rw-r--r--   0        0        0     2508 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/f2_nc.py
--rw-r--r--   0        0        0      912 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/f3_cc.py
--rw-r--r--   0        0        0      656 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/f3_nc.py
--rw-r--r--   0        0        0      883 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/fl_cc.py
--rw-r--r--   0        0        0     1778 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/fl_nc.py
--rw-r--r--   0        0        0     7867 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/kernels.py
--rw-r--r--   0        0        0     7045 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/partonic_channel.py
--rw-r--r--   0        0        0    12326 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/fonll/raw_nc.py
--rw-r--r--   0        0        0      162 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/__init__.py
--rw-r--r--   0        0        0     1249 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/f2_cc.py
--rw-r--r--   0        0        0     4117 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/f2_nc.py
--rw-r--r--   0        0        0     1350 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/f3_cc.py
--rw-r--r--   0        0        0      627 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/f3_nc.py
--rw-r--r--   0        0        0     1525 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/fl_cc.py
--rw-r--r--   0        0        0     3864 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/fl_nc.py
--rw-r--r--   0        0        0     3137 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/kernels.py
--rw-r--r--   0        0        0     6887 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/heavy/partonic_channel.py
--rw-r--r--   0        0        0       46 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/__init__.py
--rw-r--r--   0        0        0      780 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f2_cc.py
--rw-r--r--   0        0        0      402 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f2_nc.py
--rw-r--r--   0        0        0      765 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f3_cc.py
--rw-r--r--   0        0        0      405 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f3_nc.py
--rw-r--r--   0        0        0      775 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/fl_cc.py
--rw-r--r--   0        0        0      588 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/fl_nc.py
--rw-r--r--   0        0        0     1926 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/kernels.py
--rw-r--r--   0        0        0     2423 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/partonic_channel.py
--rw-r--r--   0        0        0     4024 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/raw_cc.py
--rw-r--r--   0        0        0     8896 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/raw_nc.py
--rw-r--r--   0        0        0     5742 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/kernels.py
--rw-r--r--   0        0        0      574 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/light/__init__.py
--rw-r--r--   0        0        0      420 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/light/f2_cc.py
--rw-r--r--   0        0        0     1643 2021-10-19 10:37:51.666381 yadism-0.9.1/src/yadism/coefficient_functions/light/f2_nc.py
--rw-r--r--   0        0        0      480 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/f3_cc.py
--rw-r--r--   0        0        0      727 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/f3_nc.py
--rw-r--r--   0        0        0      418 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/fl_cc.py
--rw-r--r--   0        0        0     1043 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/fl_nc.py
--rw-r--r--   0        0        0     2577 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/kernels.py
--rw-r--r--   0        0        0       25 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nlo/__init__.py
--rw-r--r--   0        0        0      649 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nlo/f2.py
--rw-r--r--   0        0        0      175 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nlo/f3.py
--rw-r--r--   0        0        0      275 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nlo/fl.py
--rw-r--r--   0        0        0       92 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/__init__.py
--rw-r--r--   0        0        0     1862 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc2ns2p.py
--rw-r--r--   0        0        0      890 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc2sg2p.py
--rw-r--r--   0        0        0     1808 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc3ns2p.py
--rw-r--r--   0        0        0      947 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xclns2p.py
--rw-r--r--   0        0        0      708 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xclsg2p.py
--rw-r--r--   0        0        0     1244 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xk3cnvp.py
--rw-r--r--   0        0        0      156 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/light/partonic_channel.py
--rw-r--r--   0        0        0     3975 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/partonic_channel.py
--rw-r--r--   0        0        0     2343 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/special/__init__.py
--rw-r--r--   0        0        0    12103 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/special/nielsen.py
--rw-r--r--   0        0        0       64 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/special/zeta.py
--rw-r--r--   0        0        0     2554 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/__init__.py
--rw-r--r--   0        0        0     3393 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/lo.py
--rw-r--r--   0        0        0     2532 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/__init__.py
--rw-r--r--   0        0        0     1173 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/convolutions.py
--rw-r--r--   0        0        0     4780 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/non_singlet.py
--rw-r--r--   0        0        0     4714 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/singlet.py
--rw-r--r--   0        0        0       24 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/__init__.py
--rw-r--r--   0        0        0     6726 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/conv.py
--rw-r--r--   0        0        0     6582 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/esf.py
--rw-r--r--   0        0        0     2832 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/exs.py
--rw-r--r--   0        0        0     4715 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/result.py
--rw-r--r--   0        0        0     7272 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/scale_variations.py
--rw-r--r--   0        0        0    16776 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/esf/tmc.py
--rw-r--r--   0        0        0      841 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/__init__.py
--rw-r--r--   0        0        0     3207 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/compatibility.py
--rw-r--r--   0        0        0     5283 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/constraints.py
--rw-r--r--   0        0        0     4686 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/cross_constraints.yaml
--rw-r--r--   0        0        0     7452 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/domains.yaml
--rw-r--r--   0        0        0     2592 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/errors.py
--rw-r--r--   0        0        0     3251 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/input/inspector.py
--rw-r--r--   0        0        0     1127 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/log.py
--rw-r--r--   0        0        0     6125 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/observable_name.py
--rw-r--r--   0        0        0    12464 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/output.py
--rw-r--r--   0        0        0     8523 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/runner.py
--rw-r--r--   0        0        0     4169 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/sf.py
--rw-r--r--   0        0        0     1682 2021-10-19 10:37:51.670381 yadism-0.9.1/src/yadism/xs.py
--rw-r--r--   0        0        0     4748 2021-10-19 10:39:24.498860 yadism-0.9.1/setup.py
--rw-r--r--   0        0        0     4759 2021-10-19 10:39:24.499314 yadism-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-10-21 12:57:45.314742 yadism-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2965 2021-10-21 12:57:45.314742 yadism-0.9.2/README.md
+-rw-r--r--   0        0        0     3447 2021-10-21 12:59:33.207237 yadism-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      318 2021-10-21 12:59:33.207237 yadism-0.9.2/src/yadism/__init__.py
+-rw-r--r--   0        0        0     8803 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/__init__.py
+-rw-r--r--   0        0        0    13396 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/coupling_constants.py
+-rw-r--r--   0        0        0       46 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/__init__.py
+-rw-r--r--   0        0        0     1160 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/f2_cc.py
+-rw-r--r--   0        0        0     2561 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/f2_nc.py
+-rw-r--r--   0        0        0      920 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/f3_cc.py
+-rw-r--r--   0        0        0      667 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/f3_nc.py
+-rw-r--r--   0        0        0      964 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/fl_cc.py
+-rw-r--r--   0        0        0     1792 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/fl_nc.py
+-rw-r--r--   0        0        0     7867 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/kernels.py
+-rw-r--r--   0        0        0     7045 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/partonic_channel.py
+-rw-r--r--   0        0        0    12326 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/fonll/raw_nc.py
+-rw-r--r--   0        0        0      162 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/__init__.py
+-rw-r--r--   0        0        0     1249 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/f2_cc.py
+-rw-r--r--   0        0        0     4117 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/f2_nc.py
+-rw-r--r--   0        0        0     1350 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/f3_cc.py
+-rw-r--r--   0        0        0      627 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/f3_nc.py
+-rw-r--r--   0        0        0     1525 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/fl_cc.py
+-rw-r--r--   0        0        0     3864 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/fl_nc.py
+-rw-r--r--   0        0        0     3137 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/kernels.py
+-rw-r--r--   0        0        0     6887 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/heavy/partonic_channel.py
+-rw-r--r--   0        0        0       46 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/__init__.py
+-rw-r--r--   0        0        0      780 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f2_cc.py
+-rw-r--r--   0        0        0      402 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f2_nc.py
+-rw-r--r--   0        0        0      765 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f3_cc.py
+-rw-r--r--   0        0        0      405 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f3_nc.py
+-rw-r--r--   0        0        0      775 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/fl_cc.py
+-rw-r--r--   0        0        0      588 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/fl_nc.py
+-rw-r--r--   0        0        0     1926 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/kernels.py
+-rw-r--r--   0        0        0     2423 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/partonic_channel.py
+-rw-r--r--   0        0        0     4024 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/raw_cc.py
+-rw-r--r--   0        0        0     8896 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/raw_nc.py
+-rw-r--r--   0        0        0     9144 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/kernels.py
+-rw-r--r--   0        0        0      574 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/__init__.py
+-rw-r--r--   0        0        0      474 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/f2_cc.py
+-rw-r--r--   0        0        0     1643 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/f2_nc.py
+-rw-r--r--   0        0        0      534 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/f3_cc.py
+-rw-r--r--   0        0        0      727 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/f3_nc.py
+-rw-r--r--   0        0        0      472 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/fl_cc.py
+-rw-r--r--   0        0        0     1043 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/fl_nc.py
+-rw-r--r--   0        0        0     3041 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/kernels.py
+-rw-r--r--   0        0        0       25 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nlo/__init__.py
+-rw-r--r--   0        0        0      649 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nlo/f2.py
+-rw-r--r--   0        0        0      175 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nlo/f3.py
+-rw-r--r--   0        0        0      275 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nlo/fl.py
+-rw-r--r--   0        0        0       92 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/__init__.py
+-rw-r--r--   0        0        0     1862 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc2ns2p.py
+-rw-r--r--   0        0        0      890 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc2sg2p.py
+-rw-r--r--   0        0        0     1808 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc3ns2p.py
+-rw-r--r--   0        0        0      947 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xclns2p.py
+-rw-r--r--   0        0        0      708 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xclsg2p.py
+-rw-r--r--   0        0        0     1244 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xk3cnvp.py
+-rw-r--r--   0        0        0      156 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/light/partonic_channel.py
+-rw-r--r--   0        0        0     3975 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/partonic_channel.py
+-rw-r--r--   0        0        0     2343 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/special/__init__.py
+-rw-r--r--   0        0        0    12103 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/special/nielsen.py
+-rw-r--r--   0        0        0       64 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/special/zeta.py
+-rw-r--r--   0        0        0     2554 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/__init__.py
+-rw-r--r--   0        0        0     3393 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/lo.py
+-rw-r--r--   0        0        0     2532 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/__init__.py
+-rw-r--r--   0        0        0     1173 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/convolutions.py
+-rw-r--r--   0        0        0     4780 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/non_singlet.py
+-rw-r--r--   0        0        0     4714 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/singlet.py
+-rw-r--r--   0        0        0       24 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/__init__.py
+-rw-r--r--   0        0        0     6726 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/conv.py
+-rw-r--r--   0        0        0     6582 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/esf.py
+-rw-r--r--   0        0        0     2832 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/exs.py
+-rw-r--r--   0        0        0     4715 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/result.py
+-rw-r--r--   0        0        0     7272 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/scale_variations.py
+-rw-r--r--   0        0        0    16776 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/esf/tmc.py
+-rw-r--r--   0        0        0      841 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/__init__.py
+-rw-r--r--   0        0        0     3204 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/compatibility.py
+-rw-r--r--   0        0        0     5283 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/constraints.py
+-rw-r--r--   0        0        0     4686 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/cross_constraints.yaml
+-rw-r--r--   0        0        0     7452 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/domains.yaml
+-rw-r--r--   0        0        0     2592 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/errors.py
+-rw-r--r--   0        0        0     3251 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/input/inspector.py
+-rw-r--r--   0        0        0     1127 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/log.py
+-rw-r--r--   0        0        0     6125 2021-10-21 12:57:45.474743 yadism-0.9.2/src/yadism/observable_name.py
+-rw-r--r--   0        0        0    12464 2021-10-21 12:57:45.478744 yadism-0.9.2/src/yadism/output.py
+-rw-r--r--   0        0        0     8523 2021-10-21 12:57:45.478744 yadism-0.9.2/src/yadism/runner.py
+-rw-r--r--   0        0        0     4169 2021-10-21 12:57:45.478744 yadism-0.9.2/src/yadism/sf.py
+-rw-r--r--   0        0        0     1682 2021-10-21 12:57:45.478744 yadism-0.9.2/src/yadism/xs.py
+-rw-r--r--   0        0        0     4748 2021-10-21 12:59:33.508624 yadism-0.9.2/setup.py
+-rw-r--r--   0        0        0     4759 2021-10-21 12:59:33.509326 yadism-0.9.2/PKG-INFO
```

### Comparing `yadism-0.9.1/LICENSE` & `yadism-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/README.md` & `yadism-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/pyproject.toml` & `yadism-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yadism"
-version = "0.9.1"
+version = "0.9.2"
 description = "Yet Another Deep-Inelastic Scattering Module"
 authors = [
   "Alessandro Candido <alessandro.candido@mi.infn.it>",
   "Felix Hekhorn <felix.hekhorn@mi.infn.it>",
   "Giacomo Magni <gmagni@nikhef.nl>"
 ]
 license = "GPL-3.0-only"
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/__init__.py` & `yadism-0.9.2/src/yadism/coefficient_functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,22 @@
             elems.extend(
                 self.damp_elems(nl, fonll.kernels.generate_light_diff(self.esf, nl))
             )
         if self.obs_name.flavor_family in ["heavy", "total"]:
             ihq = nl + 1
             if self.obs_name.is_raw_heavy and self.obs_name.hqnumber < ihq:
                 raise NotImplementedError(
-                    f"We're not providing {self.obs_name} in FONLL with {nl} light flavors yet"
+                    f"We're not providing {self.obs_name} in FONLL with {nl} light flavors"
+                    f"(Q2={self.esf.Q2}) yet"
                 )
             # F2b is not avaible in FONLL@c
             if self.obs_name.is_raw_heavy and self.obs_name.hqnumber > ihq:
                 raise ValueError(
-                    f"{self.obs_name} is not available in FONLL with {nl} light flavors "
-                    "since we're not providing two masses corrections"
+                    f"{self.obs_name} is not available in FONLL with {nl} light flavors"
+                    f"(Q2={self.esf.Q2}) since we're not providing two masses corrections"
                 )
 
             # FFNSlow
             elems.extend(heavy.kernels.generate(self.esf, nl))
             # add F^d
             if ihq in self.esf.sf.intrinsic_range:
                 elems.extend(intrinsic.kernels.generate(self.esf, ihq))
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/coupling_constants.py` & `yadism-0.9.2/src/yadism/coefficient_functions/coupling_constants.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/f2_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/f2_cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .. import splitting_functions as split
 from ..intrinsic import f2_cc as intrinsic
 from ..light import f2_cc as light
 from ..partonic_channel import RSL, EmptyPartonicChannel
 from . import partonic_channel as pc
 
 
-class AsyQuark(pc.PartonicChannelAsy, light.NonSinglet):
+class AsyQuark(pc.PartonicChannelAsy, light.NonSingletEven):
     def NNLO(self):
         # silence NNLO since heavy NNLO still not available
         return RSL()
 
 
 class AsyGluon(pc.PartonicChannelAsy):
     def NLO(self):
@@ -35,16 +35,16 @@
     pass
 
 
 class LightNonSingletShifted(EmptyPartonicChannel):
     pass
 
 
-class AsyNonSingletMissing(EmptyPartonicChannel):
-    pass
+# class AsyNonSingletMissing(EmptyPartonicChannel):
+#     pass
 
 
 class MatchingIntrinsicSplus(pc.FMatchingQuarkCC):
     ffns = intrinsic.Splus
 
 
 class MatchingGluonSplus(pc.FMatchingGluonCC):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/f2_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/f2_nc.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,56 +52,55 @@
         return RSL(cps_NNLO, args=[self.L])
 
 
 class AsySingletAA(AsySingletVV):
     pass
 
 
-@nb.njit("f8(f8,f8[:])", cache=True)
-def cns_NNLO_reg(z, args):
-    L = args[0]
-    return (
-        raw_nc.c2ns2am0_aq2(z) * L ** 2
-        + raw_nc.c2ns2am0_aq(z) * L
-        + raw_nc.c2ns2am0_a0(z)
-    )
-
-
-@nb.njit("f8(f8,f8[:])", cache=True)
-def cns_NNLO_sing(z, args):
-    L = args[0]
-    return (
-        raw_nc.c2ns2bm0_aq2(z) * L ** 2
-        + raw_nc.c2ns2bm0_aq(z) * L
-        + raw_nc.c2ns2bm0_a0(z)
-    )
-
-
-@nb.njit("f8(f8,f8[:])", cache=True)
-def cns_NNLO_loc(z, args):
-    L = args[0]
-    return (
-        raw_nc.c2ns2cm0_aq2(z) * L ** 2
-        + raw_nc.c2ns2cm0_aq(z) * L
-        + raw_nc.c2ns2cm0_a0(z)
-    )
-
-
 class LightNonSingletShifted(pc.PartonicChannelAsy):
     def NNLO(self):
         return light.NonSinglet(self.ESF, self.nf).NLO()
 
 
 class PdfMatchingNonSinglet(pc.PdfMatchingNonSinglet):
     pass
 
 
-class AsyNonSingletMissing(pc.PartonicChannelAsy):
-    def NNLO(self):
-        return RSL(cns_NNLO_reg, cns_NNLO_sing, cns_NNLO_loc, args=[self.L])
+# @nb.njit("f8(f8,f8[:])", cache=True)
+# def cns_NNLO_reg(z, args):
+#     L = args[0]
+#     return (
+#         raw_nc.c2ns2am0_aq2(z) * L ** 2
+#         + raw_nc.c2ns2am0_aq(z) * L
+#         + raw_nc.c2ns2am0_a0(z)
+#     )
+
+
+# @nb.njit("f8(f8,f8[:])", cache=True)
+# def cns_NNLO_sing(z, args):
+#     L = args[0]
+#     return (
+#         raw_nc.c2ns2bm0_aq2(z) * L ** 2
+#         + raw_nc.c2ns2bm0_aq(z) * L
+#         + raw_nc.c2ns2bm0_a0(z)
+#     )
+
+
+# @nb.njit("f8(f8,f8[:])", cache=True)
+# def cns_NNLO_loc(z, args):
+#     L = args[0]
+#     return (
+#         raw_nc.c2ns2cm0_aq2(z) * L ** 2
+#         + raw_nc.c2ns2cm0_aq(z) * L
+#         + raw_nc.c2ns2cm0_a0(z)
+#     )
+
+# class AsyNonSingletMissing(pc.PartonicChannelAsy):
+#     def NNLO(self):
+#         return RSL(cns_NNLO_reg, cns_NNLO_sing, cns_NNLO_loc, args=[self.L])
 
 
 class MatchingIntrinsicSplus(pc.FMatchingQuark):
     ffns = intrinsic.Splus
 
 
 class MatchingIntrinsicSminus(pc.FMatchingQuark):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/f3_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/f3_cc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .. import splitting_functions as split
 from ..intrinsic import f3_cc as intrinsic
 from ..light import f3_cc as light
 from ..partonic_channel import RSL, EmptyPartonicChannel
 from . import partonic_channel as pc
 
 
-class AsyQuark(pc.PartonicChannelAsy, light.NonSinglet):
+class AsyQuark(pc.PartonicChannelAsy, light.NonSingletEven):
     def NNLO(self):
         # silence NNLO since heavy NNLO still not available
         return RSL()
 
 
 class AsyGluon(pc.PartonicChannelAsy):
     def NLO(self):
@@ -25,16 +25,16 @@
     pass
 
 
 class LightNonSingletShifted(EmptyPartonicChannel):
     pass
 
 
-class AsyNonSingletMissing(EmptyPartonicChannel):
-    pass
+# class AsyNonSingletMissing(EmptyPartonicChannel):
+#     pass
 
 
 class MatchingIntrinsicRplus(pc.FMatchingQuarkCC):
     ffns = intrinsic.Rplus
 
 
 class MatchingGluonRplus(pc.FMatchingGluonCC):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/f3_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/f3_nc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 from ..intrinsic import f3_nc as intrinsic
 from ..light import f3_nc as light
-from ..partonic_channel import EmptyPartonicChannel
+
+# from ..partonic_channel import EmptyPartonicChannel
 from . import partonic_channel as pc
 
 
 class PdfMatchingNonSinglet(pc.PdfMatchingNonSinglet):
     pass
 
 
 class LightNonSingletShifted(pc.PartonicChannelAsy):
     def NNLO(self):
         return light.NonSinglet(self.ESF, self.nf).NLO()
 
 
-class AsyNonSingletMissing(EmptyPartonicChannel):
-    pass
-    # def NNLO(self):
-    # TODO get F3 from g1
+# class AsyNonSingletMissing(EmptyPartonicChannel):
+#     pass
+#     # def NNLO(self):
+#     # TODO get F3 from g1
 
 
 class MatchingIntrinsicRplus(pc.FMatchingQuark):
     ffns = intrinsic.Rplus
 
 
 class MatchingIntrinsicRminus(pc.FMatchingQuark):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/fl_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/fl_nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,23 @@
 
 
 class LightNonSingletShifted(pc.PartonicChannelAsy):
     def NNLO(self):
         return light.NonSinglet(self.ESF, self.nf).NLO()
 
 
-@nb.njit("f8(f8,f8[:])", cache=True)
-def cns_NNLO(z, args):
-    L = args[0]
-    return raw_nc.clns2am0_aq(z) * L + raw_nc.clns2am0_a0(z)
+# @nb.njit("f8(f8,f8[:])", cache=True)
+# def cns_NNLO(z, args):
+#     L = args[0]
+#     return raw_nc.clns2am0_aq(z) * L + raw_nc.clns2am0_a0(z)
 
 
-class AsyNonSingletMissing(pc.PartonicChannelAsy):
-    def NNLO(self):
-        return RSL(cns_NNLO, args=[self.L])
+# class AsyNonSingletMissing(pc.PartonicChannelAsy):
+#     def NNLO(self):
+#         return RSL(cns_NNLO, args=[self.L])
 
 
 class MatchingIntrinsicSplus(pc.FMatchingQuark):
     ffns = intrinsic.Splus
 
 
 class MatchingIntrinsicSminus(pc.FMatchingQuark):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/kernels.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/kernels.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/partonic_channel.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/partonic_channel.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/fonll/raw_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/fonll/raw_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/f2_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/f2_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/f2_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/f2_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/f3_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/f3_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/f3_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/f3_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/fl_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/fl_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/fl_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/fl_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/kernels.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/kernels.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/heavy/partonic_channel.py` & `yadism-0.9.2/src/yadism/coefficient_functions/heavy/partonic_channel.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f2_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f2_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/f3_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/f3_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/fl_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/fl_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/fl_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/fl_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/kernels.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/kernels.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/partonic_channel.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/partonic_channel.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/raw_cc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/raw_cc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/intrinsic/raw_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/intrinsic/raw_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/kernels.py` & `yadism-0.9.2/src/yadism/coefficient_functions/kernels.py`

 * *Files 27% similar despite different names*

```diff
@@ -131,14 +131,110 @@
     # add singlet
     for q in weights["ns"]:
         weights["s"][q] = tot_ch_sq / norm / 2
         weights["s"][-q] = tot_ch_sq / norm / 2
     return weights
 
 
+def cc_weights_even(coupling_constants, Q2, kind, cc_mask, nf):
+    """
+    Collect the weights of the partons.
+
+    Parameters
+    ----------
+        coupling_constants : CouplingConstants
+            manager for coupling constants
+        Q2 : float
+            W virtuality
+        kind : str
+            structure function kind
+        cc_mask : str
+            participating flavors on the CKM matrix
+        nf : int
+            number of light flavors
+
+    Returns
+    -------
+        weights : dict
+            mapping pid -> weight for q and g channel
+    """
+    weights = {"ns": {}, "g": {}, "s": {}}
+    # determine couplings
+    projectile_pid = coupling_constants.obs_config["projectilePID"]
+    if projectile_pid in [-11, 12]:
+        rest = 1
+    else:
+        rest = 0
+    # quark couplings
+    tot_ch_sq = 0
+    norm = len(cc_mask)
+    # iterate: include the heavy quark itself, since it can run in the singlet sector diagrams
+    for q in range(1, min(nf + 2, 6 + 1)):
+        sign = 1 if q % 2 == rest else -1
+        w = coupling_constants.get_weight(q, Q2, None, cc_mask=cc_mask)
+        # the heavy quark can not be in the input
+        # NOTE: intrinsic abuse this statement with nf -> nf + 1
+        if q <= nf:
+            # @F3-sign@
+            weights["ns"][sign * q] = w / 2 * (1 if kind != "F3" else sign)
+            weights["ns"][-sign * q] = w / 2 * (1 if kind != "F3" else sign)
+        # but it contributes to the average
+        tot_ch_sq += w
+    # gluon coupling = charge sum
+    weights["g"][21] = tot_ch_sq / norm / 2
+    # add singlet
+    for q in weights["ns"]:
+        weights["s"][q] = tot_ch_sq / norm / 2
+        weights["s"][-q] = tot_ch_sq / norm / 2
+    return weights
+
+
+def cc_weights_odd(coupling_constants, Q2, kind, cc_mask, nf):
+    """
+    Collect the weights of the partons.
+
+    Parameters
+    ----------
+        coupling_constants : CouplingConstants
+            manager for coupling constants
+        Q2 : float
+            W virtuality
+        kind : str
+            structure function kind
+        cc_mask : str
+            participating flavors on the CKM matrix
+        nf : int
+            number of light flavors
+
+    Returns
+    -------
+        weights : dict
+            mapping pid -> weight for q and g channel
+    """
+    weights = {"ns": {}}
+    # determine couplings
+    projectile_pid = coupling_constants.obs_config["projectilePID"]
+    if projectile_pid in [-11, 12]:
+        rest = 1
+    else:
+        rest = 0
+    # quark couplings
+    # iterate: include the heavy quark itself, since it can run in the singlet sector diagrams
+    for q in range(1, min(nf + 2, 6 + 1)):
+        sign = 1 if q % 2 == rest else -1
+        w = coupling_constants.get_weight(q, Q2, None, cc_mask=cc_mask)
+        # the heavy quark can not be in the input
+        # NOTE: intrinsic abuse this statement with nf -> nf + 1
+        if q <= nf:
+            # @F3-sign@
+            weights["ns"][sign * q] = w / 2 * (1 if kind != "F3" else sign)
+            weights["ns"][-sign * q] = -w / 2 * (1 if kind != "F3" else sign)
+    return weights
+
+
 def generate_single_flavor_light(esf, nf, ihq):
     """
     Add a light-like contribution for a single quark flavor.
 
     The linear dependency to the electric charge is introduce by mulitplying
     and diving by nf. The multiplication is *implicit* inside the coefficient function,
     the division is *explict* made here.
@@ -161,34 +257,42 @@
     light_cfs = import_local(
         kind, esf.process, ".".join(__name__.split(".")[:-1] + ["light", ""])
     )
     ns_partons = {}
     ch_av = 0
     s_partons = {}
     if esf.process == "CC":
-        w = cc_weights(esf.sf.coupling_constants, esf.Q2, kind, flavors[ihq - 1], nf)
-        ns_partons, ch_av, s_partons = (
-            w["ns"],
-            w["g"][21] / (nf),
-            {k: v / (nf) for k, v in w["s"].items()},
+        w_even = cc_weights_even(
+            esf.sf.coupling_constants, esf.Q2, kind, flavors[ihq - 1], nf
+        )
+        w_odd = cc_weights_odd(
+            esf.sf.coupling_constants, esf.Q2, kind, flavors[ihq - 1], nf
+        )
+        return (
+            Kernel(w_even["ns"], light_cfs.NonSingletEven(esf, nf)),
+            Kernel({21: w_even["g"][21] / (nf)}, light_cfs.Gluon(esf, nf)),
+            Kernel(
+                {k: v / (nf) for k, v in w_even["s"].items()},
+                light_cfs.Singlet(esf, nf),
+            ),
+            Kernel(w_odd["ns"], light_cfs.NonSingletOdd(esf, nf)),
         )
+    if kind != "F3":
+        w = esf.sf.coupling_constants.get_weight(
+            ihq, esf.Q2, "VV"
+        ) + esf.sf.coupling_constants.get_weight(ihq, esf.Q2, "AA")
     else:
-        if kind != "F3":
-            w = esf.sf.coupling_constants.get_weight(
-                ihq, esf.Q2, "VV"
-            ) + esf.sf.coupling_constants.get_weight(ihq, esf.Q2, "AA")
-        else:
-            w = esf.sf.coupling_constants.get_weight(
-                ihq, esf.Q2, "VA"
-            ) + esf.sf.coupling_constants.get_weight(ihq, esf.Q2, "AV")
-
-        ns_partons[ihq] = w
-        ns_partons[-ihq] = w if kind != "F3" else -w
-        ch_av = w / (nf) if kind != "F3" else 0.0
-        for pid in range(1, nf):
-            s_partons[pid] = ch_av
-            s_partons[-pid] = ch_av
+        w = esf.sf.coupling_constants.get_weight(
+            ihq, esf.Q2, "VA"
+        ) + esf.sf.coupling_constants.get_weight(ihq, esf.Q2, "AV")
+
+    ns_partons[ihq] = w
+    ns_partons[-ihq] = w if kind != "F3" else -w
+    ch_av = w / (nf) if kind != "F3" else 0.0
+    for pid in range(1, nf):
+        s_partons[pid] = ch_av
+        s_partons[-pid] = ch_av
     return (
         Kernel(ns_partons, light_cfs.NonSinglet(esf, nf)),
         Kernel({21: ch_av}, light_cfs.Gluon(esf, nf)),
         Kernel(s_partons, light_cfs.Singlet(esf, nf)),
     )
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/__init__.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/__init__.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/f2_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/f2_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/f3_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/f3_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/fl_nc.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/fl_nc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/kernels.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/kernels.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,26 @@
     -------
         elems : list(yadism.kernels.Kernel)
             list of elements
     """
     kind = esf.sf.obs_name.kind
     pcs = import_pc_module(kind, esf.process)
     if esf.process == "CC":
-        weights = kernels.cc_weights(
+        weights_even = kernels.cc_weights_even(
             esf.sf.coupling_constants, esf.Q2, kind, kernels.flavors[:nf], nf
         )
-    else:
-        weights = nc_weights(esf.sf.coupling_constants, esf.Q2, kind, nf)
+        ns_even = kernels.Kernel(weights_even["ns"], pcs.NonSingletEven(esf, nf))
+        g = kernels.Kernel(weights_even["g"], pcs.Gluon(esf, nf))
+        s = kernels.Kernel(weights_even["s"], pcs.Singlet(esf, nf))
+        weights_odd = kernels.cc_weights_odd(
+            esf.sf.coupling_constants, esf.Q2, kind, kernels.flavors[:nf], nf
+        )
+        ns_odd = kernels.Kernel(weights_odd["ns"], pcs.NonSingletOdd(esf, nf))
+        return (ns_even, g, s, ns_odd)
+    weights = nc_weights(esf.sf.coupling_constants, esf.Q2, kind, nf)
     ns = kernels.Kernel(weights["ns"], pcs.NonSinglet(esf, nf))
     g = kernels.Kernel(weights["g"], pcs.Gluon(esf, nf))
     s = kernels.Kernel(weights["s"], pcs.Singlet(esf, nf))
     return (ns, g, s)
 
 
 def nc_weights(coupling_constants, Q2, kind, nf, skip_heavylight=False):
```

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nlo/f2.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nlo/f2.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc2ns2p.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc2ns2p.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc2sg2p.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc2sg2p.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xc3ns2p.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xc3ns2p.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xclns2p.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xclns2p.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xclsg2p.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xclsg2p.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/light/nnlo/xk3cnvp.py` & `yadism-0.9.2/src/yadism/coefficient_functions/light/nnlo/xk3cnvp.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/partonic_channel.py` & `yadism-0.9.2/src/yadism/coefficient_functions/partonic_channel.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/special/__init__.py` & `yadism-0.9.2/src/yadism/coefficient_functions/special/__init__.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/special/nielsen.py` & `yadism-0.9.2/src/yadism/coefficient_functions/special/nielsen.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/__init__.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/lo.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/lo.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/__init__.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/__init__.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/convolutions.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/convolutions.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/non_singlet.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/non_singlet.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/coefficient_functions/splitting_functions/nlo/singlet.py` & `yadism-0.9.2/src/yadism/coefficient_functions/splitting_functions/nlo/singlet.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/conv.py` & `yadism-0.9.2/src/yadism/esf/conv.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/esf.py` & `yadism-0.9.2/src/yadism/esf/esf.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/exs.py` & `yadism-0.9.2/src/yadism/esf/exs.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/result.py` & `yadism-0.9.2/src/yadism/esf/result.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/scale_variations.py` & `yadism-0.9.2/src/yadism/esf/scale_variations.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/esf/tmc.py` & `yadism-0.9.2/src/yadism/esf/tmc.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/__init__.py` & `yadism-0.9.2/src/yadism/input/__init__.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/compatibility.py` & `yadism-0.9.2/src/yadism/input/compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     Parameters
     ----------
         theory : dict
             theory runcard
     """
     fns = theory["FNS"]
     nf = theory["NfFF"]
-    if fns not in ["FONLL-A"]:  # = fns in FFNS or ZM-VFNS
+    if "FONLL" not in fns:  # = fns in FFNS or ZM-VFNS
         # enforce correct settings moving all thresholds to 0 or oo
         if fns == "FFNS":
             ks = [0] * (nf - 3) + [np.inf] * (6 - nf)
             for k, fl in zip(ks, hqfl):
                 theory[f"k{fl}Thr"] = k
         # here there is no difference between DGLAP and DIS
         for fl in hqfl:
@@ -95,15 +95,15 @@
     else:
         # keep the old setup for the ZM-VFNS part (above)
         for pid in range(nf + 1, 6 + 1):
             fl = hqfl[pid - 4]
             theory[f"kDIS{fl}Thr"] = theory[f"k{fl}Thr"]
         # for the actual value - keep it or fallback to evolution
         hfl = hqfl[nf - 4]
-        if "kDIS{hfl}Thr" not in theory:
+        if f"kDIS{hfl}Thr" not in theory:
             theory[f"kDIS{hfl}Thr"] = theory[f"k{hfl}Thr"]
         # erase all lower thresholds, meaning lower than the interesting one (NfFF)
         for pid in range(4, nf + 1):
             fl = hqfl[pid - 4]
             # we actually need to run in the nf-FNS so even kill that one
             theory[f"k{fl}Thr"] = 0
             if pid < nf:
```

### Comparing `yadism-0.9.1/src/yadism/input/constraints.py` & `yadism-0.9.2/src/yadism/input/constraints.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/cross_constraints.yaml` & `yadism-0.9.2/src/yadism/input/cross_constraints.yaml`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/domains.yaml` & `yadism-0.9.2/src/yadism/input/domains.yaml`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/errors.py` & `yadism-0.9.2/src/yadism/input/errors.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/input/inspector.py` & `yadism-0.9.2/src/yadism/input/inspector.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/log.py` & `yadism-0.9.2/src/yadism/log.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/observable_name.py` & `yadism-0.9.2/src/yadism/observable_name.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/output.py` & `yadism-0.9.2/src/yadism/output.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/runner.py` & `yadism-0.9.2/src/yadism/runner.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/sf.py` & `yadism-0.9.2/src/yadism/sf.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/src/yadism/xs.py` & `yadism-0.9.2/src/yadism/xs.py`

 * *Files identical despite different names*

### Comparing `yadism-0.9.1/setup.py` & `yadism-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
           'sphinxcontrib-bibtex>=2.3.0,<3.0.0',
           'sphinxcontrib-details-directive>=0.1.0,<0.2.0',
           'nbsphinx>=0.8.6,<0.9.0'],
  'pineappl': ['pineappl==0.5.0_beta.1']}
 
 setup_kwargs = {
     'name': 'yadism',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Yet Another Deep-Inelastic Scattering Module',
     'long_description': '<p align="center">\n  <a href="https://n3pdf.github.io/yadism/"><img alt="Yadism" src="https://raw.githubusercontent.com/N3PDF/yadism/master/docs/_assets/logo/logo.png" width=600></a>\n</p>\n\n<p align="center">\n  <a href="https://github.com/N3PDF/yadism/actions?query=workflow%3A%22yadism%22"><img alt="Tests" src="https://github.com/N3PDF/yadism/workflows/yadism/badge.svg"></a>\n  <a href=\'https://yadism.readthedocs.io/en/latest/?badge=latest\'><img src=\'https://readthedocs.org/projects/yadism/badge/?version=latest\' alt=\'Documentation Status\' /></a>\n  <a href="https://pypi.org/project/yadism/"><img alt="PyPI" src="https://img.shields.io/pypi/v/yadism"/></a>\n  <a href="https://codecov.io/gh/N3PDF/yadism"><img src="https://codecov.io/gh/N3PDF/yadism/branch/master/graph/badge.svg?token=qgCFyUQ6oG" /></a>\n  <a href="https://www.codefactor.io/repository/github/n3pdf/yadism"><img src="https://www.codefactor.io/repository/github/n3pdf/yadism/badge?s=e5a00668b58574b5b056e1aca01c7b25d2c203f8" alt="CodeFactor" /></a>\n  <a href="https://zenodo.org/badge/latestdoi/219968694"><img src="https://zenodo.org/badge/219968694.svg" alt="DOI"></a>\n</p>\n\n<!--Future Badges\n/github/workflow/status/N3PDF/dis/yadism\n\nuse the ones provided by shields.io:\n- example: https://img.shields.io/github/workflow/status/N3PDF/yadism\n\nnote: in order to make shields.io the repo must be public (or accessible to it in some way)\n\noptional:\n- Release-date (github):\n  - /github/release-date/:user/:repo\n- Downloads:\n  - github: /github/downloads/:user/:repo/total\n  - pypi: /pypi/:period/:packageName\n- License:\n  - pypi-license: /pypi/l/:packageName\n  - github-license: /github/license/:user/:repo\n- Activity:\n  - open-issues (github): /github/issues/:user/:repo\n  - open-pull-requests (github): /github/issues-pr/:user/:repo\n- Code size:\n  - github: /github/languages/code-size/:user/:repo\n-->\n\n## Scope of the project\n\nProvide all necessary tools to compute the DIS structure functions and related objects. This project is linked closely to [EKO](https://github.com/N3PDF/eko).\n\n## Installation\n\nAs a user please use [the released version on PyPI](https://pypi.org/project/yadism/),\nthrough your python package manager, e.g. with `pip`:\n\n```sh\npip install yadism\n```\n\n### Dev\n\nFor development just use the install script and poetry (provided by install\nscript):\n\n```sh\npython install.py\npoetry install\n```\n\n## Development\n\nMembers of the development team should always follow the [contribution\nguidelines](.github/contributing.md), to have a uniform strategy in code\ndevelopment and improve collaboration.\n\n## Contributing or contacting the authors\n\nFor any kind of interaction consider before to read [external contribution\nguidelines](.github/contributing.md#external-contributions), otherwise just send\nan email to the authors:\n\n- [Alessandro Candido](mailto:alessandro.candido@mi.infn.it)\n- [Felix Hekhorn](mailto:felix.hekhorn@mi.infn.it)\n- [Giacomo Magni](mailto:gmagni@nikhef.nl)\n',
     'author': 'Alessandro Candido',
     'author_email': 'alessandro.candido@mi.infn.it',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://n3pdf.github.io/yadism/',
```

#### html2text {}

```diff
@@ -10,15 +10,15 @@
 'yadism.input'] package_data = \ {'': ['*']} install_requires = \
 ['LeProHQ>=0.2.0,<0.3.0', 'eko>=0.7.1,<0.8.0', 'numba>=0.53.1,<0.54.0',
 'numpy>=1.21.0,<2.0.0', 'pandas>=1.3.0,<2.0.0', 'rich>=10.6.0,<11.0.0',
 'scipy>=1.7.0,<2.0.0'] extras_require = \ {'docs': ['Sphinx>=4.1.1,<5.0.0',
 'sphinx-rtd-theme>=0.5.2,<0.6.0', 'recommonmark>=0.7.1,<0.8.0', 'sphinxcontrib-
 bibtex>=2.3.0,<3.0.0', 'sphinxcontrib-details-directive>=0.1.0,<0.2.0',
 'nbsphinx>=0.8.6,<0.9.0'], 'pineappl': ['pineappl==0.5.0_beta.1']} setup_kwargs
-= { 'name': 'yadism', 'version': '0.9.1', 'description': 'Yet Another Deep-
+= { 'name': 'yadism', 'version': '0.9.2', 'description': 'Yet Another Deep-
 Inelastic Scattering Module', 'long_description': '
                                  \n [Yadism]\n
 \n\n
                                \n [Tests]\n ' />
 \n [PyPI]\n [https://codecov.io/gh/N3PDF/yadism/branch/master/graph/
 badge.svg?token=qgCFyUQ6oG]\n [CodeFactor]\n [DOI]\n
 \n\n\n\n## Scope of the project\n\nProvide all necessary tools to compute the
```

### Comparing `yadism-0.9.1/PKG-INFO` & `yadism-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadism
-Version: 0.9.1
+Version: 0.9.2
 Summary: Yet Another Deep-Inelastic Scattering Module
 Home-page: https://n3pdf.github.io/yadism/
 License: GPL-3.0-only
 Author: Alessandro Candido
 Author-email: alessandro.candido@mi.infn.it
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yadism Version: 0.9.1 Summary: Yet Another Deep-
+Metadata-Version: 2.1 Name: yadism Version: 0.9.2 Summary: Yet Another Deep-
 Inelastic Scattering Module Home-page: https://n3pdf.github.io/yadism/ License:
 GPL-3.0-only Author: Alessandro Candido Author-email:
 alessandro.candido@mi.infn.it Requires-Python: >=3.8,<3.10 Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: Unix Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic ::
```

