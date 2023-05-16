# Comparing `tmp/mwrpy-0.1.8.tar.gz` & `tmp/mwrpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.8.tar", last modified: Fri May 12 11:13:06 2023, max compression
+gzip compressed data, was "mwrpy-0.2.0.tar", last modified: Tue May 16 13:55:09 2023, max compression
```

## Comparing `mwrpy-0.1.8.tar` & `mwrpy-0.2.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.137483 mwrpy-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-12 11:12:51.000000 mwrpy-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 11:12:51.000000 mwrpy-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-12 11:13:06.137483 mwrpy-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-12 11:12:51.000000 mwrpy-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20186 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.129483 mwrpy-0.1.8/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rwxr-xr-x   0 runner    (1001) docker     (123)  1208422 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.133484 mwrpy-0.1.8/mwrpy/site_config/lindenberg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.137483 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/HZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TEL_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/site_config/lindenberg/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 11:12:51.000000 mwrpy-0.1.8/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:13:06.125483 mwrpy-0.1.8/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-12 11:13:06.000000 mwrpy-0.1.8/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 11:13:05.000000 mwrpy-0.1.8/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:13:06.137483 mwrpy-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-12 11:12:51.000000 mwrpy-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 13:54:56.000000 mwrpy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 13:54:56.000000 mwrpy-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-16 13:55:09.427990 mwrpy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-16 13:54:56.000000 mwrpy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14642 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20148 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)  1208422 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.423990 mwrpy-0.2.0/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/juelich/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/lindenberg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.427990 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    47201 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)   209789 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    63954 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    41482 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/site_config/lindenberg/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15747 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 13:54:56.000000 mwrpy-0.2.0/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:09.419990 mwrpy-0.2.0/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 13:55:09.000000 mwrpy-0.2.0/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:55:09.427990 mwrpy-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 13:54:56.000000 mwrpy-0.2.0/setup.py
```

### Comparing `mwrpy-0.1.8/LICENSE` & `mwrpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/PKG-INFO` & `mwrpy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.8
+Version: 0.2.0
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.8/README.md` & `mwrpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/atmos.py` & `mwrpy-0.2.0/mwrpy/atmos.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,50 +146,48 @@
     if vdir < 180.0:
         Dv = vdir + 180.0
     elif vdir > 180.0:
         Dv = vdir - 180
     return Dv
 
 
-def find_lwcl_free(lev1: dict, ix: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
+def find_lwcl_free(lev1: dict) -> tuple[np.ndarray, np.ndarray]:
     """Identifying liquid water cloud free periods using 31.4 GHz TB variability + IRT.
     Uses pre-defined time index and additionally returns status of IRT availability"""
 
     if "elevation_angle" in lev1:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
-    index = np.ones(len(ix)) * np.nan
-    status = np.ones(len(ix), dtype=np.int32)
+    index = np.ones(len(lev1["time"]), dtype=np.float32) * np.nan
+    status = np.ones(len(lev1["time"]), dtype=np.int32)
     freq_31 = np.where(np.round(lev1["frequency"][:], 1) == 31.4)[0]
     if len(freq_31) == 1:
-        tb = np.squeeze(lev1["tb"][ix, freq_31])
-        tb[(lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)] = np.nan
-        ind = utils.time_to_datetime_index(lev1["time"][ix])
+        tb = np.squeeze(lev1["tb"][:, freq_31])
+        tb[(lev1["pointing_flag"][:] == 1) | (elevation_angle[:] < 89.0)] = np.nan
+        ind = utils.time_to_datetime_index(lev1["time"][:])
         tb_df = pd.DataFrame({"Tb": tb}, index=ind)
         tb_std = tb_df.rolling("2min", center=True, min_periods=10).std()
         tb_mx = tb_std.rolling("20min", center=True, min_periods=100).max()
 
         if "irt" in lev1:
             tb_thres = 0.1
-            irt = lev1["irt"][ix, :]
+            irt = lev1["irt"][:, :]
             irt[irt == -999.0] = np.nan
             irt = np.nanmean(irt, axis=1)
-            irt[
-                (lev1["pointing_flag"][ix] == 1) | (elevation_angle[ix] < 89.0)
-            ] = np.nan
+            irt[(lev1["pointing_flag"][:] == 1) | (elevation_angle[:] < 89.0)] = np.nan
             irt_df = pd.DataFrame({"Irt": irt[:]}, index=ind)
             irt_mx = irt_df.rolling("20min", center=True, min_periods=100).max()
-            index[(irt_mx["Irt"] > 263.15) & (tb_mx["Tb"] > tb_thres)] = 1
+            index[(irt_mx["Irt"] > 263.15) & (tb_mx["Tb"] > tb_thres)] = 1.0
             status[:] = 0
 
         tb_thres = 0.2
-        index[(tb_mx["Tb"] > tb_thres)] = 1
+        index[(tb_mx["Tb"] > tb_thres)] = 1.0
         df = pd.DataFrame({"index": index}, index=ind)
         df = df.fillna(method="bfill", limit=120)
         df = df.fillna(method="ffill", limit=120)
         index = np.array(df["index"])
         index[(tb_mx["Tb"] < tb_thres) & (index != 1.0)] = 0.0
-        index[(elevation_angle[ix] < 89.0) & (index != 1.0)] = 2.0
+        index[(elevation_angle[:] < 89.0) & (index != 1.0)] = 2.0
 
     return np.nan_to_num(index, nan=2).astype(int), status
```

### Comparing `mwrpy-0.1.8/mwrpy/cli.py` & `mwrpy-0.2.0/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.2.0/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/level1/met_quality_control.py` & `mwrpy-0.2.0/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/level1/quality_control.py` & `mwrpy-0.2.0/mwrpy/level1/quality_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,16 +294,22 @@
                 _, freq_ind, coeff_ind = np.intersect1d(
                     data["frequency"],
                     cfile["freq"],
                     assume_unique=False,
                     return_indices=True,
                 )
                 ele_ind = np.where(
-                    (data["ele"][:] > cfile["elevation_predictand"][:] - 0.5)
-                    & (data["ele"][:] < cfile["elevation_predictand"][:] + 0.5)
+                    (
+                        data["elevation_angle"][:]
+                        > cfile["elevation_predictand"][:] - 0.5
+                    )
+                    & (
+                        data["elevation_angle"][:]
+                        < cfile["elevation_predictand"][:] + 0.5
+                    )
                     & (data["pointing_flag"][:] == 0)
                 )[0]
 
                 if (ele_ind.size > 0) & (freq_ind.size > 0):
                     rpg_dat["tb_spectrum"][ele_ind, ifreq] = (
                         cfile["offset_mvr"][:]
                         + np.sum(
```

### Comparing `mwrpy-0.1.8/mwrpy/level1/rpg_bin.py` & `mwrpy-0.2.0/mwrpy/level1/rpg_bin.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,30 +71,22 @@
 
     def _init_data(self):
         for key, data in self.raw_data.items():
             self.data[key] = data
 
     def _get_date(self):
         time_median = float(np.ma.median(self.raw_data["time"]))
-        date = (
-            datetime.datetime.utcfromtimestamp(
-                utils.epoch2unix(time_median, self.header["_time_ref"])
-            )
-            .strftime("%Y-%m-%d")
-        )
+        date = datetime.datetime.utcfromtimestamp(
+            utils.epoch2unix(time_median, self.header["_time_ref"])
+        ).strftime("%Y-%m-%d")
         today = float(datetime.datetime.today().strftime("%Y"))
         if float(date[0:4]) > today:
-            date = (
-                datetime.datetime.utcfromtimestamp(
-                    utils.epoch2unix(
-                        time_median, self.header["_time_ref"], (1970, 1, 1)
-                    )
-                )
-                .strftime("%Y-%m-%d")
-            )
+            date = datetime.datetime.utcfromtimestamp(
+                utils.epoch2unix(time_median, self.header["_time_ref"], (1970, 1, 1))
+            ).strftime("%Y-%m-%d")
         return date
 
     def find_valid_times(self):
         # sort timestamps
         time = self.data["time"]
         ind = time.argsort()
         self._screen(ind)
```

### Comparing `mwrpy-0.1.8/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.2.0/mwrpy/level1/write_lev1_nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                         rpg_irt.data["time"],
                         "ir_azimuth_angle",
                     )
 
             (
                 rpg_bin.data["liquid_cloud_flag"],
                 rpg_bin.data["liquid_cloud_flag_status"],
-            ) = atmos.find_lwcl_free(rpg_bin.data, np.arange(len(rpg_bin.data["time"])))
+            ) = atmos.find_lwcl_free(rpg_bin.data)
 
             try:
                 file_list_met = get_file_list(path_to_files, "MET")
             except RuntimeError as err:
                 print(err)
             rpg_met = RpgBin(file_list_met)
             add_interpol1d(
```

### Comparing `mwrpy-0.1.8/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.2.0/mwrpy/level2/get_ret_coeff.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,14 @@
         coeff["FR_BL"] = coeff["FR"]
 
     elif (str(c_list[0][-2:]).lower() == "nc") & (len(c_list) > 0):
         coeff["RT"] = Fill_Value_Int
         N = len(c_list)
 
         if prefix in ("lwp", "iwv"):
-
             coeff["AG"] = np.ones(N) * Fill_Value_Float
             coeff["FR"] = np.ones([len(freq), N]) * Fill_Value_Float
             coeff["TL"] = np.zeros([N, len(freq)])
             coeff["TQ"] = np.zeros([N, len(freq)])
             coeff["OS"] = np.zeros(N)
             coeff["AL"] = [0]
 
@@ -221,15 +220,14 @@
                 if c_file.regression_type == "quadratic":
                     coeff["TQ"][i_file, freq_ind] = c_file["coefficient_mvr"][
                         freq_coeff + len(freq_coeff)
                     ]
                 coeff["OS"][i_file] = c_file["offset_mvr"][0]
 
         elif prefix in ("tpt", "hpt"):
-
             c_file = nc.Dataset(c_list[0])
             n_height_grid = c_file.dimensions["n_height_grid"].size
 
             coeff["AG"] = np.ones(N) * Fill_Value_Float
             coeff["FR"] = np.ones([len(freq), N]) * Fill_Value_Float
             coeff["TL"] = np.zeros([N, n_height_grid, len(freq)])
             coeff["TQ"] = np.zeros([N, n_height_grid, len(freq)])
@@ -255,15 +253,14 @@
                 if c_file.regression_type == "quadratic":
                     coeff["TQ"][i_file, :, freq_ind] = c_file["coefficient_mvr"][
                         freq_coeff + len(freq_coeff), :
                     ]
                 coeff["OS"][:, i_file] = c_file["offset_mvr"][:]
 
         elif prefix == "tpb":
-
             c_file = nc.Dataset(c_list[0])
             _, freq_ind, freq_coeff = np.intersect1d(
                 freq[:], c_file["freq"][:], assume_unique=False, return_indices=True
             )
             if len(freq_coeff) < len(c_file["freq"][:]):
                 raise RuntimeError(
                     ["Instrument and retrieval frequencies do not match."]
```

### Comparing `mwrpy-0.1.8/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.2.0/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/level2/lwp_offset.py` & `mwrpy-0.2.0/mwrpy/level2/lwp_offset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Module for LWP offset correction"""
 import numpy as np
 import pandas as pd
 
 from mwrpy import utils
-from mwrpy.atmos import find_lwcl_free
-
-Fill_Value_Float = -999.0
 
 
 def correct_lwp_offset(
     lev1: dict, lwp_org: np.ndarray, index: np.ndarray
 ) -> tuple[np.ndarray, np.ndarray]:
     """This function corrects Lwp offset using the
     2min standard deviation of the 31.4 GHz channel and IR temperature
@@ -21,23 +18,25 @@
     """
 
     if "elevation_angle" in lev1:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
-    lwcl_i, _ = find_lwcl_free(lev1, index)
+    lwcl_i = lev1["liquid_cloud_flag"][index]
     lwp = np.copy(lwp_org)
     lwp[(lwcl_i != 0) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
     ind = utils.time_to_datetime_index(lev1["time"][index])
     lwp_df = pd.DataFrame({"Lwp": lwp}, index=ind)
     lwp_std = lwp_df.rolling("2min", center=True, min_periods=10).std()
     lwp_max = lwp_std.rolling("20min", center=True, min_periods=100).max()
     lwp_df[lwp_max > 0.002] = np.nan
     lwp_offset = lwp_df.rolling("20min", center=True, min_periods=100).mean()
 
+    if np.isnan(lwp_offset["Lwp"][-1]):
+        lwp_offset["Lwp"][-1] = 0.0
     lwp_offset = lwp_offset.interpolate(method="linear")
     lwp_offset = lwp_offset.fillna(method="bfill")
-    lwp_offset["Lwp"][np.isnan(lwp_offset["Lwp"])] = 0
+    lwp_offset["Lwp"][np.isnan(lwp_offset["Lwp"])] = 0.0
     lwp_org -= lwp_offset["Lwp"].values
 
     return lwp_org, lwp_offset["Lwp"].values
```

### Comparing `mwrpy-0.1.8/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.2.0/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/plots/generate_plots.py` & `mwrpy-0.2.0/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/plots/plot_meta.py` & `mwrpy-0.2.0/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/plots/plot_utils.py` & `mwrpy-0.2.0/mwrpy/plots/plot_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module containing additional helper functions for plotting"""
 import locale
 from datetime import datetime, timezone
 
-from matplotlib import ticker
 import netCDF4
 import numpy as np
+from matplotlib import ticker
 from numpy import ma, ndarray
 
 from mwrpy.utils import (
     convolve2DFFT,
     get_ret_freq,
     isbit,
     read_nc_fields,
```

### Comparing `mwrpy-0.1.8/mwrpy/process_mwrpy.py` & `mwrpy-0.2.0/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/rpg_mwr.py` & `mwrpy-0.2.0/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.2.0/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.2.0/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.2.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/HZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TEL_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/coefficients/TZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.8/mwrpy/site_config/lindenberg/config.yaml` & `mwrpy-0.2.0/mwrpy/site_config/lindenberg/config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Site config file
 
 type: hatpro
 
 params:
-    station_altitude: 104.
-    station_longitude: 14.118
-    station_latitude: 52.208
-    
+    altitude: 104.
+    longitude: 14.118
+    latitude: 52.208
+
     # path to level1 data and path for processed files
     data_in: /data/obs/site/lin/linhat/l1/
     data_out: /data/obs/site/lin/linhat/actris/
-    
+
     # path to ABSCAL.HIS file
     path_to_cal: /data/obs/site/lin/linhat/
 
-    # integration time for BL scans in seconds 
+    # integration time for BL scans in seconds
     scan_time: 100.
 
     # integration time of measurements in seconds
     int_time: 1
 
     # Azimuth angle is transformed to geographical coordinates (E=90 and W=270), currently only for RPG scanners.
     # If you do not want to transform the coordinates set azi_cor to -999.
@@ -33,72 +33,72 @@
     # Bit 3: tb_above_threshold
     # Bit 4: spectral_consistency_above_threshold
     # Bit 5: receiver_sanity_failed
     # Bit 6: rain_detected
     # Bit 7: sun_moon_in_beam
     # Bit 8: tb_offset_above_threshold
     flag_status: [0, 0, 0, 0, 0, 0, 0, 1]
-    
+
     # availability of IR
     ir_flag: True
 
 
 global_specs:
     # A succinct description of what is in the dataset, composed of instrument type and site name
     title: HATPRO G5 MWR at Lindenberg, Germany
-    
+
     # Versioning of the datasets (containing date and software version)
     history:
-    
+
     # Where the original data was produced
     institution: DWD
-    
+
     # Miscellaneous Information about the dataset or methods used to produce it
     comment:
-    
+
     # References that describe the data or methods used to produce it
     references:
-    
+
     # Name of measurement station
     site_location: lindenberg
-    
+
     # E-PROFILE instrument identifier. “A” if there is only one instrument on the station. Additional instruments are identified with the letters B, C, etc.
     instrument_id: A
-    
+
     # WIGOS Station identifier acording to WIGOS convention
     wigos_station_id: 0-20000-0-10393
-    
+
     # Department responsible for the instrument
     principal_investigator:
-    
+
     # Instrument generation
-    instrument_generation: G5    
-    
+    instrument_generation: G5
+
     # Specific to mainboard
     instrument_hw_id:
-    
+
     # Name of network(s) that instrument may be part of
     network_name: ACTRIS
-    
+
     # Name of campaign instrument may collect data for
     campaign_name:
-    
+
     # List of files the data set is depending on
     dependencies:
-    
+
     # Data license
-    license:  
-    
+    license:
+
     # Logbook repair/replacement work performed
     instrument_history:
-    
+
     # Fabrication year of the infrared radiometer
     ir_instrument_fabrication_year:
-    
+
     # Logbook repair/replacement work performed
     ir_instrument_history:
-    
+
     # Fabrication year of the weather station
     met_instrument_fabrication_year:
-    
+
     # Logbook repair/replacement work performed
     met_instrument_history:
```

### Comparing `mwrpy-0.1.8/mwrpy/utils.py` & `mwrpy-0.2.0/mwrpy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,36 +263,31 @@
             ]
         )
     return f_list
 
 
 def read_yaml_config(site: str) -> tuple[dict, dict]:
     """Reads config yaml files."""
+    dir_name = os.path.dirname(__file__)
+    site_config_file = os.path.join(dir_name, "site_config", site, "config.yaml")
+    if not os.path.exists(site_config_file):
+        raise NotImplementedError(
+            f"Site config file {site_config_file} does not exist."
+        )
 
-    params = {
-        "altitude": 108.0,
-        "longitude": 6.407,
-        "latitude": 50.906,
-        "scan_time": 50.0,
-        "int_time": 1,
-        "azi_cor": -999.0,
-        "const_azi": -999.0,
-        "flag_status": [0, 0, 0, 1, 0, 0, 0, 0],
-        "ir_flag": True,
-        "site_name": site,
-    }
+    with open(site_config_file, "r", encoding="utf8") as f:
+        params = yaml.load(f, Loader=SafeLoader)["params"]
 
     global_specs = {
         "title": "HATPRO Level 1B data",
     }
     site_config = {
         "global_specs": global_specs,
         "params": params,
     }
-    dir_name = os.path.dirname(__file__)
     inst_file = os.path.join(dir_name, "site_config/hatpro.yaml")
     with open(inst_file, "r", encoding="utf8") as f:
         inst_config = yaml.load(f, Loader=SafeLoader)
     inst_config["global_specs"].update(site_config["global_specs"])
     for name in inst_config["params"].keys():
         site_config["params"][name] = inst_config["params"][name]
```

### Comparing `mwrpy-0.1.8/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.2.0/mwrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.8
+Version: 0.2.0
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.8/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.2.0/mwrpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 mwrpy/site_config/hyytiala/config.yaml
 mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+mwrpy/site_config/juelich/config.yaml
 mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
@@ -55,13 +56,13 @@
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
 mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
 mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
 mwrpy/site_config/lindenberg/config.yaml
-mwrpy/site_config/lindenberg/coefficients/HZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
 mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
 mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
 mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
-mwrpy/site_config/lindenberg/coefficients/TEL_NN_DE_Lindenberg_HATPRO_G5_v121.ret
-mwrpy/site_config/lindenberg/coefficients/TZE_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
```

### Comparing `mwrpy-0.1.8/setup.py` & `mwrpy-0.2.0/setup.py`

 * *Files identical despite different names*

