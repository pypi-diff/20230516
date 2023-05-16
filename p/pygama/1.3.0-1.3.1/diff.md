# Comparing `tmp/pygama-1.3.0.tar.gz` & `tmp/pygama-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygama-1.3.0.tar", last modified: Sun May  7 09:40:56 2023, max compression
+gzip compressed data, was "pygama-1.3.1.tar", last modified: Tue May 16 14:10:23 2023, max compression
```

## Comparing `pygama-1.3.0.tar` & `pygama-1.3.1.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 09:40:47.000000 pygama-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-07 09:40:56.440826 pygama-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-07 09:40:47.000000 pygama-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-07 09:40:47.000000 pygama-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 09:40:56.440826 pygama-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-07 09:40:47.000000 pygama-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.416826 pygama-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    71519 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/evt/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/build_tcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/flow/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60726 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/file_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/hit/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/hit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/hit/build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/lgdo/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/arrayofequalsizedarrays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68140 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/waveform_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/math/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/AoE_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/dsp_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/ecal_th.py
--rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/energy_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    72502 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/energy_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/extract_tau.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/mse_psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/build_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/compass/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/data_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/data_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_digitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33100 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_flashcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_run_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/vis/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/mpl/clint.mpl
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/mpl/root.mpl
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/dsp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/dsp/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/data-loader-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/filedb-config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/configs/nested/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/nested/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/nested/data-loader-config-nested.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_filedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_flow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/functional/test_l200_dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/functional/test_teststand_dataproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/hit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/hit/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/basic-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-a-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-multi-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/test_build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    47033 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_waveform_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/math/test_fwhm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/pargen/test_ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/pargen/test_energy_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)    56908 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/compass/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/fc-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/orca-out-spec-cli.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/orca-out-spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/test_or_run_decoder_for_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/test_orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_build_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_daq_to_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 14:10:15.000000 pygama-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-16 14:10:23.377868 pygama-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-16 14:10:15.000000 pygama-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 14:10:15.000000 pygama-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 14:10:23.377868 pygama-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 14:10:15.000000 pygama-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.349867 pygama-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.353868 pygama-1.3.1/src/pygama/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.357868 pygama-1.3.1/src/pygama/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71519 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/evt/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/build_tcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/tcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60726 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27420 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/hit/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/hit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/hit/build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/arrayofequalsizedarrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68140 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/waveform_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/math/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/AoE_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/dsp_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/ecal_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/energy_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72502 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/energy_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/extract_tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/mse_psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/build_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/data_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/data_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33100 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_flashcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_run_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/vis/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/mpl/clint.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/mpl/root.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.357868 pygama-1.3.1/src/pygama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/data-loader-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/filedb-config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/configs/nested/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/nested/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/nested/data-loader-config-nested.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_filedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_flow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/functional/test_l200_dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/functional/test_teststand_dataproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/hit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/hit/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/basic-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-a-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-multi-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/test_build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47033 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_waveform_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/math/test_fwhm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/pargen/test_ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/pargen/test_energy_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/raw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)    56908 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_lh5_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/fc-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/orca-out-spec-cli.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/orca-out-spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/test_or_run_decoder_for_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/test_orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_daq_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/vis/test_waveform_browser.py
```

### Comparing `pygama-1.3.0/LICENSE` & `pygama-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/PKG-INFO` & `pygama-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.3.0/README.md` & `pygama-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/setup.cfg` & `pygama-1.3.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -72,17 +72,17 @@
 	myst-parser
 	nbsphinx
 	pygama
 	sphinx
 	sphinx-copybutton
 	sphinx-inline-tabs
 test = 
-	legend-testdata>=0.4.2
 	pre-commit
 	pygama
+	pylegendtestdata
 	pytest>=6.0
 	pytest-cov
 
 [options.package_data]
 * = *.json
 
 [flake8]
```

### Comparing `pygama-1.3.0/src/pygama/cli.py` & `pygama-1.3.1/src/pygama/cli.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/__init__.py` & `pygama-1.3.1/src/pygama/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/build_dsp.py` & `pygama-1.3.1/src/pygama/dsp/build_dsp.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/errors.py` & `pygama-1.3.1/src/pygama/dsp/errors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processing_chain.py` & `pygama-1.3.1/src/pygama/dsp/processing_chain.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/__init__.py` & `pygama-1.3.1/src/pygama/dsp/processors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 from .peak_snr_threshold import peak_snr_threshold
 from .pole_zero import double_pole_zero, pole_zero
 from .presum import presum
 from .pulse_injector import inject_exp_pulse, inject_sig_pulse
 from .saturation import saturation
 from .soft_pileup_corr import soft_pileup_corr, soft_pileup_corr_bl
 from .time_over_threshold import time_over_threshold
-from .time_point_thresh import time_point_thresh
+from .time_point_thresh import interpolated_time_point_thresh, time_point_thresh
 from .trap_filters import asym_trap_filter, trap_filter, trap_norm, trap_pickoff
 from .upsampler import interpolating_upsampler, upsampler
 from .wiener_filter import wiener_filter
 from .windower import windower
 
 __all__ = [
     "bl_subtract",
@@ -128,14 +128,15 @@
     "inject_exp_pulse",
     "inject_sig_pulse",
     "saturation",
     "peak_snr_threshold",
     "soft_pileup_corr",
     "soft_pileup_corr_bl",
     "time_point_thresh",
+    "interpolated_time_point_thresh",
     "asym_trap_filter",
     "trap_filter",
     "trap_norm",
     "trap_pickoff",
     "upsampler",
     "interpolating_upsampler",
     "wiener_filter",
```

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/bl_subtract.py` & `pygama-1.3.1/src/pygama/dsp/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/convolutions.py` & `pygama-1.3.1/src/pygama/dsp/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/dplms.py` & `pygama-1.3.1/src/pygama/dsp/processors/dplms.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/dwt.py` & `pygama-1.3.1/src/pygama/dsp/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/fftw.py` & `pygama-1.3.1/src/pygama/dsp/processors/fftw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/fixed_time_pickoff.py` & `pygama-1.3.1/src/pygama/dsp/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/gaussian_filter1d.py` & `pygama-1.3.1/src/pygama/dsp/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/get_multi_local_extrema.py` & `pygama-1.3.1/src/pygama/dsp/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/histogram.py` & `pygama-1.3.1/src/pygama/dsp/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/linear_slope_fit.py` & `pygama-1.3.1/src/pygama/dsp/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/log_check.py` & `pygama-1.3.1/src/pygama/dsp/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/min_max.py` & `pygama-1.3.1/src/pygama/dsp/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/moving_windows.py` & `pygama-1.3.1/src/pygama/dsp/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/multi_a_filter.py` & `pygama-1.3.1/src/pygama/dsp/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/multi_t_filter.py` & `pygama-1.3.1/src/pygama/dsp/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/optimize.py` & `pygama-1.3.1/src/pygama/dsp/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/param_lookup.py` & `pygama-1.3.1/src/pygama/dsp/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/peak_snr_threshold.py` & `pygama-1.3.1/src/pygama/dsp/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/pole_zero.py` & `pygama-1.3.1/src/pygama/dsp/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/presum.py` & `pygama-1.3.1/src/pygama/dsp/processors/presum.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/pulse_injector.py` & `pygama-1.3.1/src/pygama/dsp/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/saturation.py` & `pygama-1.3.1/src/pygama/dsp/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/soft_pileup_corr.py` & `pygama-1.3.1/src/pygama/dsp/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/time_over_threshold.py` & `pygama-1.3.1/src/pygama/dsp/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/time_point_thresh.py` & `pygama-1.3.1/src/pygama/dsp/processors/time_point_thresh.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/trap_filters.py` & `pygama-1.3.1/src/pygama/dsp/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/upsampler.py` & `pygama-1.3.1/src/pygama/dsp/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/wiener_filter.py` & `pygama-1.3.1/src/pygama/dsp/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/processors/windower.py` & `pygama-1.3.1/src/pygama/dsp/processors/windower.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/dsp/utils.py` & `pygama-1.3.1/src/pygama/dsp/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/evt/build_tcm.py` & `pygama-1.3.1/src/pygama/evt/build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/evt/tcm.py` & `pygama-1.3.1/src/pygama/evt/tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/flow/data_loader.py` & `pygama-1.3.1/src/pygama/flow/data_loader.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/flow/file_db.py` & `pygama-1.3.1/src/pygama/flow/file_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,19 +504,34 @@
         for p in path:
             paths += lgdo.lgdo_utils.expand_path(p, list=True)
 
         if not paths:
             raise FileNotFoundError(path)
 
         sto = lh5.LH5Store()
-        # objects that will be used to configure the FileDB at the end
+        # objects/accumulators that will be used to configure the FileDB at the end
         _cfg = None
         _df = None
         _columns = None
 
+        # function needed later in the loop
+        def _replace_idx(row, trans, tier):
+            col = row[f"{tier}_col_idx"]
+            if col is None:
+                return None
+
+            col = np.array(col)
+            new_col = np.copy(col)
+
+            for idx, new_idx in trans.items():
+                new_col[np.where(col == idx)] = new_idx
+
+            return new_col.tolist()
+
+        # loop over the files
         for p in paths:
             cfg, _ = sto.read_object("config", p)
             cfg = json.loads(cfg.value.decode())
 
             # make sure configurations are all the same
             if _cfg is None:
                 _cfg = cfg
@@ -534,39 +549,43 @@
             df = pd.read_hdf(p, key="dataframe")
 
             # first iteration
             if _columns is None:
                 _columns = columns
                 _df = df
                 continue
+
             elif _columns != columns:
                 log.debug("found inconsistent FileDB, trying to merge")
                 # if columns are not the same, need to merge the two dataframes
-                # in the right way
+                # in the right way. loop over new columns
+                idx_trans = {}
                 for idx, cols in enumerate(columns):
+                    new_idx = None
+
+                    # the columns might be a new entry...
                     if cols not in _columns:
                         # add the new column at the end and save its index
                         _columns += [cols]
                         new_idx = len(_columns) - 1
-
-                        def _replace_idx(row, idx, new_idx, tier):
-                            col = row[f"{tier}_col_idx"]
-                            if col is None:
-                                return None
-                            else:
-                                return [new_idx if x == idx else x for x in col]
-
-                        # now go through the new dataframe and update the old index
-                        # everywhere in the {tier}_col_idx columns
-                        for tier in list(_cfg["tier_dirs"].keys()):
-                            df[f"{tier}_col_idx"] = df.apply(
-                                _replace_idx,
-                                args=(idx, new_idx, tier),
-                                axis=1,
-                            )
+                    # ...or just located (at a different index?) in the
+                    # existing column list
+                    else:
+                        new_idx = _columns.index(cols)
+
+                    idx_trans[idx] = new_idx
+
+                # now go through the new dataframe and update the old index
+                # everywhere in the {tier}_col_idx columns
+                for tier in list(_cfg["tier_dirs"].keys()):
+                    df[f"{tier}_col_idx"] = df.apply(
+                        _replace_idx,
+                        args=(idx_trans, tier),
+                        axis=1,
+                    )
 
             # now we can safely concat the dataframes
             _df = pd.concat([_df, df], ignore_index=True, copy=False)
 
         self.set_config(_cfg)
         self.df = _df
         self.columns = _columns
```

### Comparing `pygama-1.3.0/src/pygama/flow/utils.py` & `pygama-1.3.1/src/pygama/flow/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/hit/build_hit.py` & `pygama-1.3.1/src/pygama/hit/build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/__init__.py` & `pygama-1.3.1/src/pygama/lgdo/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/array.py` & `pygama-1.3.1/src/pygama/lgdo/array.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/arrayofequalsizedarrays.py` & `pygama-1.3.1/src/pygama/lgdo/arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/__init__.py` & `pygama-1.3.1/src/pygama/lgdo/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/base.py` & `pygama-1.3.1/src/pygama/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/generic.py` & `pygama-1.3.1/src/pygama/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/radware.py` & `pygama-1.3.1/src/pygama/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/utils.py` & `pygama-1.3.1/src/pygama/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/compression/varlen.py` & `pygama-1.3.1/src/pygama/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/encoded.py` & `pygama-1.3.1/src/pygama/lgdo/encoded.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/fixedsizearray.py` & `pygama-1.3.1/src/pygama/lgdo/fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/lgdo.py` & `pygama-1.3.1/src/pygama/lgdo/lgdo.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/lgdo_utils.py` & `pygama-1.3.1/src/pygama/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/lh5_store.py` & `pygama-1.3.1/src/pygama/lgdo/lh5_store.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/scalar.py` & `pygama-1.3.1/src/pygama/lgdo/scalar.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/struct.py` & `pygama-1.3.1/src/pygama/lgdo/struct.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/table.py` & `pygama-1.3.1/src/pygama/lgdo/table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/vectorofvectors.py` & `pygama-1.3.1/src/pygama/lgdo/vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/lgdo/waveform_table.py` & `pygama-1.3.1/src/pygama/lgdo/waveform_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/logging.py` & `pygama-1.3.1/src/pygama/logging.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/math/histogram.py` & `pygama-1.3.1/src/pygama/math/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/math/peak_fitting.py` & `pygama-1.3.1/src/pygama/math/peak_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/math/utils.py` & `pygama-1.3.1/src/pygama/math/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/AoE_cal.py` & `pygama-1.3.1/src/pygama/pargen/AoE_cal.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/cuts.py` & `pygama-1.3.1/src/pygama/pargen/cuts.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/data_cleaning.py` & `pygama-1.3.1/src/pygama/pargen/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/dsp_optimize.py` & `pygama-1.3.1/src/pygama/pargen/dsp_optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/ecal_th.py` & `pygama-1.3.1/src/pygama/pargen/ecal_th.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/energy_cal.py` & `pygama-1.3.1/src/pygama/pargen/energy_cal.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/energy_optimisation.py` & `pygama-1.3.1/src/pygama/pargen/energy_optimisation.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/extract_tau.py` & `pygama-1.3.1/src/pygama/pargen/extract_tau.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/pargen/mse_psd.py` & `pygama-1.3.1/src/pygama/pargen/mse_psd.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/__init__.py` & `pygama-1.3.1/src/pygama/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/buffer_processor/buffer_processor.py` & `pygama-1.3.1/src/pygama/raw/buffer_processor/buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py` & `pygama-1.3.1/src/pygama/raw/buffer_processor/lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/build_raw.py` & `pygama-1.3.1/src/pygama/raw/build_raw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/compass/compass_config_parser.py` & `pygama-1.3.1/src/pygama/raw/compass/compass_config_parser.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/compass/compass_event_decoder.py` & `pygama-1.3.1/src/pygama/raw/compass/compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/compass/compass_header_decoder.py` & `pygama-1.3.1/src/pygama/raw/compass/compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/compass/compass_streamer.py` & `pygama-1.3.1/src/pygama/raw/compass/compass_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/data_decoder.py` & `pygama-1.3.1/src/pygama/raw/data_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/data_streamer.py` & `pygama-1.3.1/src/pygama/raw/data_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/fc/fc_config_decoder.py` & `pygama-1.3.1/src/pygama/raw/fc/fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/fc/fc_event_decoder.py` & `pygama-1.3.1/src/pygama/raw/fc/fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/fc/fc_status_decoder.py` & `pygama-1.3.1/src/pygama/raw/fc/fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/fc/fc_streamer.py` & `pygama-1.3.1/src/pygama/raw/fc/fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_base.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_base.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_digitizers.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_digitizers.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_flashcam.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_flashcam.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_header.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_header.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_header_decoder.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_packet.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_packet.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_run_decoder.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_run_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/orca/orca_streamer.py` & `pygama-1.3.1/src/pygama/raw/orca/orca_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/raw/raw_buffer.py` & `pygama-1.3.1/src/pygama/raw/raw_buffer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/vis/mpl/clint.mpl` & `pygama-1.3.1/src/pygama/vis/mpl/clint.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/vis/mpl/root.mpl` & `pygama-1.3.1/src/pygama/vis/mpl/root.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama/vis/waveform_browser.py` & `pygama-1.3.1/src/pygama/vis/waveform_browser.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/src/pygama.egg-info/PKG-INFO` & `pygama-1.3.1/src/pygama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.3.0/src/pygama.egg-info/SOURCES.txt` & `pygama-1.3.1/src/pygama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/conftest.py` & `pygama-1.3.1/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 import copy
 import inspect
 import os
 import re
+import shutil
+import uuid
+from getpass import getuser
 from pathlib import Path
+from tempfile import gettempdir
 
 import numpy as np
 import pytest
-from legend_testdata import LegendTestData
+from legendtestdata import LegendTestData
 
 from pygama.dsp import build_dsp
 from pygama.raw import build_raw
 
 config_dir = Path(__file__).parent / "dsp" / "configs"
+_tmptestdir = os.path.join(
+    gettempdir(), "pygama-tests-" + getuser() + str(uuid.uuid4())
+)
+
+
+@pytest.fixture(scope="session")
+def tmptestdir():
+    os.mkdir(_tmptestdir)
+    yield _tmptestdir
+    shutil.rmtree(_tmptestdir)
+
+
+def pytest_sessionfinish(session, exitstatus):
+    if exitstatus is True:
+        os.rmdir(_tmptestdir)
 
 
 @pytest.fixture(scope="session")
 def lgnd_test_data():
     ldata = LegendTestData()
-    ldata.checkout("39f9927")
+    ldata.checkout("c089a59")
     return ldata
 
 
 @pytest.fixture(scope="session")
 def dsp_test_file(lgnd_test_data):
     out_name = "/tmp/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5"
     build_dsp(
```

### Comparing `pygama-1.3.0/tests/dsp/configs/icpc-dsp-config.json` & `pygama-1.3.1/tests/dsp/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/configs/numpy-parsing.json` & `pygama-1.3.1/tests/dsp/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/configs/sipm-dplms-config.json` & `pygama-1.3.1/tests/dsp/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/configs/sipm-dsp-config.json` & `pygama-1.3.1/tests/dsp/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/conftest.py` & `pygama-1.3.1/tests/dsp/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/dplms_noise_mat.dat` & `pygama-1.3.1/tests/dsp/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/test_dplms.py` & `pygama-1.3.1/tests/dsp/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/test_dwt.py` & `pygama-1.3.1/tests/dsp/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/test_fixed_time_pickoff.py` & `pygama-1.3.1/tests/dsp/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/test_get_multi_local_extrema.py` & `pygama-1.3.1/tests/dsp/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/processors/test_histogram.py` & `pygama-1.3.1/tests/dsp/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/test_build_dsp.py` & `pygama-1.3.1/tests/dsp/test_build_dsp.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/test_list_parsing.py` & `pygama-1.3.1/tests/dsp/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/test_numpy_constants_parsing.py` & `pygama-1.3.1/tests/dsp/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/dsp/test_processing_chain.py` & `pygama-1.3.1/tests/dsp/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/flow/configs/filedb-config.json` & `pygama-1.3.1/tests/flow/configs/filedb-config.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'table_format'": "{'raw': 'ch{ch:07d}/raw', 'dsp': 'ch{ch:07d}/dsp', 'hit': 'ch{ch:07d}/hit', "*

 * *                   "'tcm': 'hardware_tcm_1'}"}*

```diff
@@ -4,19 +4,19 @@
         "dsp": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_dsp.lh5",
         "evt": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_evt.lh5",
         "hit": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_hit.lh5",
         "raw": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_raw.lh5",
         "tcm": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_tcm.lh5"
     },
     "table_format": {
-        "dsp": "ch{ch:03d}/dsp",
+        "dsp": "ch{ch:07d}/dsp",
         "evt": "{grp}/evt",
-        "hit": "ch{ch:03d}/hit",
-        "raw": "ch{ch:03d}/raw",
-        "tcm": "hardware_tcm"
+        "hit": "ch{ch:07d}/hit",
+        "raw": "ch{ch:07d}/raw",
+        "tcm": "hardware_tcm_1"
     },
     "tier_dirs": {
         "dsp": "/dsp",
         "evt": "/evt",
         "hit": "/hit",
         "raw": "/raw",
         "tcm": "/tcm"
```

### Comparing `pygama-1.3.0/tests/flow/conftest.py` & `pygama-1.3.1/tests/flow/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/flow/test_data_loader.py` & `pygama-1.3.1/tests/flow/test_data_loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 
+import numpy as np
 import pandas as pd
 import pytest
 
 from pygama import lgdo
 from pygama.flow import DataLoader
 
 config_dir = Path(__file__).parent / "configs"
@@ -73,82 +74,85 @@
 def test_no_merge(test_dl):
     test_dl.set_files("all")
     test_dl.set_output(columns=["timestamp"], merge_files=False)
     data = test_dl.load()
 
     assert isinstance(data, dict)
     assert isinstance(data[0], lgdo.Table)
-    assert len(data) == 2
+    assert len(data) == 4  # 4 files
     assert list(data[0].keys()) == ["hit_table", "hit_idx", "timestamp"]
 
 
 def test_outputs(test_dl):
-    test_dl.set_files("all")
+    test_dl.set_files("type == 'phy'")
+    test_dl.set_datastreams([1057600, 1059201], "ch")
     test_dl.set_output(
-        fmt="pd.DataFrame", columns=["timestamp", "channel", "bl_mean", "hit_par1"]
+        fmt="pd.DataFrame", columns=["timestamp", "channel", "energies", "energy_in_pe"]
     )
     data = test_dl.load()
 
     assert isinstance(data, pd.DataFrame)
     assert list(data.keys()) == [
         "hit_table",
         "hit_idx",
         "file",
         "timestamp",
         "channel",
-        "bl_mean",
-        "hit_par1",
+        "energies",
+        "energy_in_pe",
     ]
 
 
 def test_any_mode(test_dl):
     test_dl.filedb.scan_tables_columns()
-    test_dl.set_files("all")
-    test_dl.set_cuts({"hit": "daqenergy == 634"})
+    test_dl.set_files("type == 'phy'")
+    test_dl.set_cuts({"hit": "daqenergy == 10221"})
     el = test_dl.build_entry_list(tcm_level="tcm", mode="any")
 
-    assert len(el) == 42
+    assert len(el) == 6
 
 
 def test_set_files(test_dl):
-    test_dl.set_files("timestamp == '20220716T104550Z'")
+    test_dl.set_files("timestamp == '20230318T012144Z'")
     test_dl.set_output(columns=["timestamp"], merge_files=False)
     data = test_dl.load()
 
     assert len(data) == 1
 
 
 def test_set_keylist(test_dl):
-    test_dl.set_files(["20220716T104550Z", "20220716T104550Z"])
+    test_dl.set_files(["20230318T012144Z", "20230318T012228Z"])
     test_dl.set_output(columns=["timestamp"], merge_files=False)
     data = test_dl.load()
 
-    assert len(data) == 1
+    assert len(data) == 2
 
 
 def test_set_datastreams(test_dl):
-    test_dl.set_files("all")
-    test_dl.set_datastreams([1, 3, 8], "ch")
-    test_dl.set_output(columns=["channel"], merge_files=False)
+    channels = [1084803, 1084804, 1121600]
+    test_dl.set_files("timestamp == '20230318T012144Z'")
+    test_dl.set_datastreams(channels, "ch")
+    test_dl.set_output(columns=["eventnumber"], fmt="pd.DataFrame", merge_files=False)
     data = test_dl.load()
 
-    assert (data[0]["hit_table"].nda == [1, 3, 8]).all()
-    assert (data[0]["channel"].nda == [1, 3, 8]).all()
+    assert np.array_equal(data[0]["hit_table"].unique(), channels)
 
 
 def test_set_cuts(test_dl):
-    test_dl.set_files("all")
-    test_dl.set_cuts({"hit": "card == 3"})
-    test_dl.set_output(columns=["card"])
+    test_dl.set_files("type == 'cal'")
+    test_dl.set_cuts({"hit": "is_valid_cal == False"})
+    test_dl.set_datastreams([1084803], "ch")
+    test_dl.set_output(columns=["is_valid_cal"], fmt="pd.DataFrame")
     data = test_dl.load()
 
-    assert (data["hit_table"].nda == [12, 13, 12, 13]).all()
+    assert (data.is_valid_cal == False).all()  # noqa: E712
 
 
 def test_browse(test_dl):
-    test_dl.set_files("all")
+    test_dl.set_files("type == 'phy'")
+    test_dl.set_datastreams([1057600, 1059201], "ch")
     test_dl.set_output(
-        fmt="pd.DataFrame", columns=["timestamp", "channel", "bl_mean", "hit_par1"]
+        fmt="pd.DataFrame", columns=["timestamp", "channel", "energies", "energy_in_pe"]
     )
     wb = test_dl.browse()
 
     wb.draw_next()
```

### Comparing `pygama-1.3.0/tests/hit/configs/spms-hit-a-config.json` & `pygama-1.3.1/tests/hit/configs/spms-hit-a-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/hit/test_build_hit.py` & `pygama-1.3.1/tests/hit/test_build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `pygama-1.3.1/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/sigcompress/special-wf-clipped.dat` & `pygama-1.3.1/tests/lgdo/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/test_compression.py` & `pygama-1.3.1/tests/lgdo/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/test_radware_sigcompress.py` & `pygama-1.3.1/tests/lgdo/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/test_str2wfcodec.py` & `pygama-1.3.1/tests/lgdo/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/compression/test_uleb128_zigzag_diff.py` & `pygama-1.3.1/tests/lgdo/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_array.py` & `pygama-1.3.1/tests/lgdo/test_array.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_arrayofequalsizedarrays.py` & `pygama-1.3.1/tests/lgdo/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_encoded.py` & `pygama-1.3.1/tests/lgdo/test_encoded.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_fixedsizearray.py` & `pygama-1.3.1/tests/lgdo/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_lgdo_utils.py` & `pygama-1.3.1/tests/lgdo/test_lgdo_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,23 +60,23 @@
         == "a_random_string/blah"
     )
 
 
 def test_expand_path(lgnd_test_data):
     files = [
         lgnd_test_data.get_path(
-            "lh5/prod-ref-l200/generated/tier/dsp/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_dsp.lh5"
+            "lh5/prod-ref-l200/generated/tier/dsp/cal/p03/r001/l200-p03-r001-cal-20230318T012144Z-tier_dsp.lh5"
         ),
         lgnd_test_data.get_path(
-            "lh5/prod-ref-l200/generated/tier/dsp/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_dsp.lh5"
+            "lh5/prod-ref-l200/generated/tier/dsp/cal/p03/r001/l200-p03-r001-cal-20230318T012228Z-tier_dsp.lh5"
         ),
     ]
     base_dir = os.path.dirname(files[0])
 
-    assert lgdo_utils.expand_path(f"{base_dir}/*20220716T104550Z*") == files[0]
+    assert lgdo_utils.expand_path(f"{base_dir}/*20230318T012144Z*") == files[0]
 
     # Should fail if file not found
     with pytest.raises(FileNotFoundError):
         lgdo_utils.expand_path(f"{base_dir}/not_a_real_file.lh5")
 
     # Should fail if multiple files found
     with pytest.raises(FileNotFoundError):
```

### Comparing `pygama-1.3.0/tests/lgdo/test_lh5_iterator.py` & `pygama-1.3.1/tests/lgdo/test_lh5_iterator.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,44 +75,44 @@
 
 
 @pytest.fixture(scope="module")
 def more_lgnd_files(lgnd_test_data):
     return [
         [
             lgnd_test_data.get_path(
-                "lh5/prod-ref-l200/generated/tier/raw/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_raw.lh5"
+                "lh5/prod-ref-l200/generated/tier/raw/cal/p03/r001/l200-p03-r001-cal-20230318T012144Z-tier_raw.lh5"
             ),
             lgnd_test_data.get_path(
-                "lh5/prod-ref-l200/generated/tier/raw/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_raw.lh5"
+                "lh5/prod-ref-l200/generated/tier/raw/cal/p03/r001/l200-p03-r001-cal-20230318T012228Z-tier_raw.lh5"
             ),
         ],
         [
             lgnd_test_data.get_path(
-                "lh5/prod-ref-l200/generated/tier/hit/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_hit.lh5"
+                "lh5/prod-ref-l200/generated/tier/hit/cal/p03/r001/l200-p03-r001-cal-20230318T012144Z-tier_hit.lh5"
             ),
             lgnd_test_data.get_path(
-                "lh5/prod-ref-l200/generated/tier/hit/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_hit.lh5"
+                "lh5/prod-ref-l200/generated/tier/hit/cal/p03/r001/l200-p03-r001-cal-20230318T012228Z-tier_hit.lh5"
             ),
         ],
     ]
 
 
 def test_friend(more_lgnd_files):
     lh5_raw_it = LH5Iterator(
         more_lgnd_files[0],
-        "ch000/raw",
+        "ch1084803/raw",
         field_mask=["waveform", "baseline"],
         buffer_len=5,
     )
     lh5_it = LH5Iterator(
         more_lgnd_files[1],
-        "ch000/hit",
-        field_mask=["hit_par1"],
+        "ch1084803/hit",
+        field_mask=["is_valid_0vbb"],
         buffer_len=5,
         friend=lh5_raw_it,
     )
 
     lh5_obj, n_rows = lh5_it.read(0)
 
-    assert n_rows == 2
+    assert n_rows == 5
     assert isinstance(lh5_obj, lgdo.Table)
-    assert set(lh5_obj.keys()) == {"waveform", "baseline", "hit_par1"}
+    assert set(lh5_obj.keys()) == {"waveform", "baseline", "is_valid_0vbb"}
```

### Comparing `pygama-1.3.0/tests/lgdo/test_lh5_store.py` & `pygama-1.3.1/tests/lgdo/test_lh5_store.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_representations.py` & `pygama-1.3.1/tests/lgdo/test_representations.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_scalar.py` & `pygama-1.3.1/tests/lgdo/test_scalar.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_struct.py` & `pygama-1.3.1/tests/lgdo/test_struct.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_table.py` & `pygama-1.3.1/tests/lgdo/test_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_table_eval.py` & `pygama-1.3.1/tests/lgdo/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_vectorofvectors.py` & `pygama-1.3.1/tests/lgdo/test_vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/lgdo/test_waveform_table.py` & `pygama-1.3.1/tests/lgdo/test_waveform_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/math/test_fwhm.py` & `pygama-1.3.1/tests/math/test_fwhm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor.py` & `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json` & `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json` & `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py` & `pygama-1.3.1/tests/raw/buffer_processor/test_lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/compass/conftest.py` & `pygama-1.3.1/tests/raw/compass/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/compass/test_compass_event_decoder.py` & `pygama-1.3.1/tests/raw/compass/test_compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/compass/test_compass_header_decoder.py` & `pygama-1.3.1/tests/raw/compass/test_compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/compass/test_compass_streamer.py` & `pygama-1.3.1/tests/raw/compass/test_compass_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/fc/test_fc_config_decoder.py` & `pygama-1.3.1/tests/raw/fc/test_fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/fc/test_fc_event_decoder.py` & `pygama-1.3.1/tests/raw/fc/test_fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/fc/test_fc_status_decoder.py` & `pygama-1.3.1/tests/raw/fc/test_fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/fc/test_fc_streamer.py` & `pygama-1.3.1/tests/raw/fc/test_fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/orca/test_or_run_decoder_for_run.py` & `pygama-1.3.1/tests/raw/orca/test_or_run_decoder_for_run.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/test_build_raw.py` & `pygama-1.3.1/tests/raw/test_build_raw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/test_cli.py` & `pygama-1.3.1/tests/raw/test_cli.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/test_daq_to_raw.py` & `pygama-1.3.1/tests/raw/test_daq_to_raw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/raw/test_raw_buffer.py` & `pygama-1.3.1/tests/raw/test_raw_buffer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/vis/configs/hpge-dsp-config.json` & `pygama-1.3.1/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.0/tests/vis/test_waveform_browser.py` & `pygama-1.3.1/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

