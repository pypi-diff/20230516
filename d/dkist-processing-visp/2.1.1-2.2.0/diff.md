# Comparing `tmp/dkist_processing_visp-2.1.1.tar.gz` & `tmp/dkist_processing_visp-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.1.1.tar", last modified: Fri May  5 18:27:01 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.2.0.tar", last modified: Tue May 16 16:34:41 2023, max compression
```

## Comparing `dkist_processing_visp-2.1.1.tar` & `dkist_processing_visp-2.2.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.804837 dkist_processing_visp-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    19968 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-05 18:27:01.804837 dkist_processing_visp-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.788837 dkist_processing_visp-2.1.1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.788837 dkist_processing_visp-2.1.1/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.792837 dkist_processing_visp-2.1.1/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.792837 dkist_processing_visp-2.1.1/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10418 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.792837 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.796837 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14365 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    38179 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20011 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.796837 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10422 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4499 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27922 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.800837 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16212 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17553 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    13876 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11821 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.800837 dkist_processing_visp-2.1.1/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.792837 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-05 18:27:01.000000 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3605 2023-05-05 18:27:01.000000 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 18:27:01.000000 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-05 18:27:01.000000 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-05 18:27:01.000000 dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.804837 dkist_processing_visp-2.1.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-05 18:27:01.804837 dkist_processing_visp-2.1.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-05-05 18:27:01.804837 dkist_processing_visp-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-05 18:26:55.000000 dkist_processing_visp-2.1.1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    20303 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.596091 dkist_processing_visp-2.2.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.596091 dkist_processing_visp-2.2.0/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.596091 dkist_processing_visp-2.2.0/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.596091 dkist_processing_visp-2.2.0/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11585 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.600091 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.600091 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14365 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    40378 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20011 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.600091 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10422 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4499 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    27922 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16389 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    17553 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11821 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/dkist_processing_visp/workflows/single_task_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.596091 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-16 16:34:41.000000 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-05-16 16:34:41.000000 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 16:34:41.000000 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-16 16:34:41.000000 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-16 16:34:41.000000 dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-05-16 16:34:41.604091 dkist_processing_visp-2.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-16 16:34:35.000000 dkist_processing_visp-2.2.0/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.1.1/.gitignore` & `dkist_processing_visp-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/.pre-commit-config.yaml` & `dkist_processing_visp-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/CHANGELOG.rst` & `dkist_processing_visp-2.2.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.2.0 (2023-05-16)
+===================
+
+Bugfixes
+--------
+
+- Lots of small updates to harden the beam angle calculation against pathological data. We are now resistant to lamp data with large gradients and/or data with a high density of bad pixels. (`#114 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/114>`__)
+
+
 v2.1.1 (2023-05-05)
 ===================
 
 Misc
 ----
 
 - Update dkist-processing-common to 2.6.0 which includes an upgrade to airflow 2.6.0
```

### Comparing `dkist_processing_visp-2.1.1/PKG-INFO` & `dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist_processing_visp
-Version: 2.1.1
+Name: dkist-processing-visp
+Version: 2.2.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.1.1/README.rst` & `dkist_processing_visp-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.2.0/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/bitbucket-pipelines.yml` & `dkist_processing_visp-2.2.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/check_changelog_updated.sh` & `dkist_processing_visp-2.2.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.2.0/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/models/parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,24 +87,47 @@
 
         This ensures that very very small values way out in the wings are not included in the mask. For example, if
         this value is 0.01 then any mask points less than 1% of the maximum will be ignored.
         """
         return self._find_most_recent_past_value("visp_hairline_mask_gaussian_peak_cutoff_fraction")
 
     @property
-    def geo_max_num_otsu(self):
-        """Max number of Otsu iterations to consider when looking for the ideal separation of hairlines."""
-        return self._find_most_recent_past_value("visp_geo_max_num_otsu")
+    def geo_binary_opening_diameter(self) -> int:
+        """
+        Diameter threshold of morphological opening performed on binary image prior to spatial smoothing.
+
+        The opening removes dot-like feautres that are smaller than the given diameter. Because the hairlines are long
+        and thin it is hard to set this value too high.
+        """
+        return self._find_most_recent_past_value("visp_geo_binary_opening_diameter")
+
+    @property
+    def geo_hairline_flat_id_threshold(self) -> float:
+        """Minimum fraction of binary pixels in a single spatial column for that column to be considered a hairline."""
+        return self._find_most_recent_past_value("visp_geo_hairline_flat_id_threshold")
 
     @property
     def geo_hairline_fit_width_px(self) -> int:
         """Plus/minus distance around initial guess to look at when fitting a Gaussian to the hairline signal."""
         return self._find_most_recent_past_value("visp_geo_hairline_fit_width_px")
 
     @property
+    def geo_hairline_angle_fit_sig_clip(self) -> float:
+        """Plus/minus number of standard deviations away from the median used to clip bad hairline center fits.
+
+        Clipping deviant values can greatly improve the fit to the slope and thus the beam angle.
+        """
+        return self._find_most_recent_past_value("visp_geo_hairline_angle_fit_sig_clip")
+
+    @property
+    def geo_hairline_angle_fit_min_samples(self) -> float:
+        """Return fractional number of samples required for the RANSAC regressor used to fit hairline angles."""
+        return self._find_most_recent_past_value("visp_geo_hairline_angle_fit_min_samples")
+
+    @property
     def geo_max_beam_2_angle_refinement(self) -> float:
         """Maximum allowable refinement to the beam 2 spectral tilt angle, in radians."""
         return self._find_most_recent_past_value("visp_geo_max_beam_2_angle_refinement")
 
     @property
     def geo_upsample_factor(self):
         """Pixel precision (1/upsample_factor) to use during phase matching of beam/modulator images."""
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 from typing import Generator
 
 import numpy as np
 import peakutils as pku
 import scipy.ndimage as spnd
 import scipy.optimize as spo
 import skimage.metrics as skim
+import skimage.morphology as skimo
 import skimage.registration as skir
+from astropy.modeling import fitting
+from astropy.modeling import models
+from astropy.stats import sigma_clip
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
-from dkist_processing_math.transform import make_binary
 from logging42 import logger
 from scipy.fft import fftn
 from scipy.optimize import minimize
 from skimage.registration._phase_cross_correlation import _upsampled_dft
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
@@ -98,15 +101,15 @@
                         angle_corr_array = self.remove_beam_angle(
                             angle=angle, beam=beam, modstate=modstate
                         )
 
                     with self.apm_processing_step(
                         f"Computing state offset for {beam = } and {modstate = }"
                     ):
-                        logger.info(f"Computing state offset for {beam=} and {modstate = }")
+                        logger.info(f"Computing state offset for {beam = } and {modstate = }")
                         state_offset = self.compute_modstate_offset(
                             array=angle_corr_array, beam=beam, modstate=modstate
                         )
                         self.write_state_offset(offset=state_offset, beam=beam, modstate=modstate)
 
                     with self.apm_processing_step(
                         f"Removing state offset for {beam = } and {modstate = }"
@@ -254,86 +257,88 @@
         """
         array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
             beam=beam, task="GC_OFFSET"
         )
         return array_generator
 
     def do_basic_corrections(self):
-        """
-        Apply dark correction to all data that will be used for Geometric Calibration.
+        """Apply dark correction to all data that will be used for Geometric Calibration."""
+        self._prep_lamp_gain()
+        self._prep_input_solar_gain()
 
-        Lamp correction is not applied because it was found to reduce contrast between the spectra and the hairlines
-        that are used to find the rotation angle.
-        """
-        # SOLAR
-        #######
-        for exp_time in self.constants.solar_exposure_times:
+    def _prep_lamp_gain(self):
+        """Apply dark corrections fo INPUT lamp frames."""
+        for exp_time in self.constants.lamp_exposure_times:
             for beam in range(1, self.constants.num_beams + 1):
-                logger.info(f"Starting basic reductions for {exp_time = } and {beam = }")
+                logger.info(f"Starting basic lamp reductions for {exp_time = } and {beam = }")
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
                         beam=beam, exposure_time=exp_time
                     )
                 except StopIteration:
                     raise ValueError(f"No matching dark found for {exp_time = } s")
 
                 for modstate in range(1, self.constants.num_modstates + 1):
-                    input_solar_arrays = self.input_frame_loaders_solar_gain_array_generator(
+                    input_lamp_arrays = self.input_frame_loaders_lamp_gain_array_generator(
                         beam=beam,
                         modstate=modstate,
                         exposure_time=exp_time,
                     )
-                    avg_solar_array = average_numpy_arrays(input_solar_arrays)
+                    avg_lamp_array = average_numpy_arrays(input_lamp_arrays)
 
-                    dark_corrected_solar_array = next(
+                    dark_corrected_lamp_array = next(
                         subtract_array_from_arrays(
-                            arrays=avg_solar_array, array_to_subtract=dark_array
+                            arrays=avg_lamp_array, array_to_subtract=dark_array
                         )
                     )
 
-                    logger.info(f"Writing dark corrected data for {beam=}, {modstate=}")
+                    logger.info(f"Writing dark corrected lamp data for {beam=}, {modstate=}")
                     self.intermediate_frame_helpers_write_arrays(
-                        arrays=dark_corrected_solar_array,
+                        arrays=dark_corrected_lamp_array,
                         beam=beam,
                         modstate=modstate,
-                        task="GC_SOLAR_BASIC",
+                        task="GC_LAMP_BASIC",
                     )
 
-        # LAMP
-        ######
-        for exp_time in self.constants.lamp_exposure_times:
+    def _prep_input_solar_gain(self):
+        """
+        Apply dark correction to INPUT solar gain images.
+
+        Lamp correction is not applied because it was found to reduce contrast between the spectra and the hairlines.
+        """
+        for exp_time in self.constants.solar_exposure_times:
             for beam in range(1, self.constants.num_beams + 1):
-                logger.info(f"Starting basic lamp reductions for {exp_time = } and {beam = }")
+                logger.info(f"Starting basic reductions for {exp_time = } and {beam = }")
                 try:
                     dark_array = self.intermediate_frame_helpers_load_dark_array(
                         beam=beam, exposure_time=exp_time
                     )
                 except StopIteration:
                     raise ValueError(f"No matching dark found for {exp_time = } s")
 
                 for modstate in range(1, self.constants.num_modstates + 1):
-                    input_lamp_arrays = self.input_frame_loaders_lamp_gain_array_generator(
+                    input_solar_arrays = self.input_frame_loaders_solar_gain_array_generator(
                         beam=beam,
                         modstate=modstate,
                         exposure_time=exp_time,
                     )
-                    avg_lamp_array = average_numpy_arrays(input_lamp_arrays)
+                    avg_solar_array = average_numpy_arrays(input_solar_arrays)
 
-                    dark_corrected_lamp_array = next(
+                    dark_corrected_solar_array = next(
                         subtract_array_from_arrays(
-                            arrays=avg_lamp_array, array_to_subtract=dark_array
+                            arrays=avg_solar_array, array_to_subtract=dark_array
                         )
                     )
 
-                    logger.info(f"Writing dark corrected lamp data for {beam=}, {modstate=}")
+                    logger.info(f"Writing dark corrected data for {beam=}, {modstate=}")
                     self.intermediate_frame_helpers_write_arrays(
-                        arrays=dark_corrected_lamp_array,
+                        arrays=dark_corrected_solar_array,
                         beam=beam,
                         modstate=modstate,
-                        task="GC_LAMP_BASIC",
+                        task="GC_SOLAR_BASIC",
                     )
 
     def compute_beam_angle(self, beam: int) -> float:
         """
         Find the angle between the slit hairlines and the pixel axes for a single beam.
 
         Generally, the algorithm is:
@@ -353,69 +358,125 @@
         -------
         float
             Beam angle in radians
         """
         angle_list = []
         for modstate in range(1, self.constants.num_modstates + 1):
             data = self.basic_corrected_lamp_data(beam=beam, modstate=modstate)
-            angle = self._compute_single_modstate_angle(data)
-            logger.info(f"Angle for {beam = } and {modstate = } = {np.rad2deg(angle):0.4f} deg")
+            angle = self._compute_single_modstate_angles(data)
+            logger.info(f"Angles for {beam = } and {modstate = } = {np.rad2deg(angle)} deg")
             angle_list.append(angle)
 
         theta = float(np.nanmedian(angle_list))
         logger.info(f"Beam angle for {beam = }: {np.rad2deg(theta):0.4f} deg")
         return theta
 
-    def _compute_single_modstate_angle(self, array: np.ndarray) -> float:
+    def _identify_hairlines_and_bad_pixels(
+        self, input_array: np.ndarray
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """
+        Return pixel coordinates corresponding to hairlines and a map of non-hairline bad pixels.
+
+        This is almost exactly the same algorithm as `dkist_processing_visp.tasks.mixin.corrections._find_hairline_pixels`,
+        but it adds an extra step of doing a morphological opening prior to smoothing in the spatial dimension. This
+        opening helps to remove small point/dot-like pixels that are not part of the hairline.
+
+        The difference between the opened result and the original deviant pixel map shows the locations of non-hairline
+        "bad" (i.e., deviant) pixels. This map is also returned.
         """
-        Compute the angle of a single array.
+        filtered_array = spnd.median_filter(
+            input_array, size=(1, self.parameters.hairline_median_spatial_smoothing_width_px)
+        )
+        diff = (input_array - filtered_array) / filtered_array
+        hairline_locations = np.abs(diff) > self.parameters.hairline_fraction
+
+        # dtype kwarg necessary here to avoid endianness issues
+        mask_array = np.zeros_like(input_array, dtype=int)
+        mask_array[hairline_locations] = 1
+
+        # These lines are what's different between this function and
+        # `dkist_processing_visp.tasks.mixin.corrections._find_hairline_pixels`
+        cleaned_mask_array = skimo.diameter_opening(
+            mask_array, diameter_threshold=self.parameters.geo_binary_opening_diameter
+        )
+        bad_pixel_map = (mask_array - cleaned_mask_array).astype(bool)
+
+        # Now smooth the hairline mask in the spatial dimension to capture the higher-flux wings
+        smoothed_mask_array = spnd.gaussian_filter1d(
+            cleaned_mask_array.astype(float),
+            self.parameters.hairline_mask_spatial_smoothing_width_px,
+            axis=1,
+        )
+
+        hairline_locations = np.where(
+            smoothed_mask_array
+            > smoothed_mask_array.max()
+            * self.parameters.hairline_mask_gaussian_peak_cutoff_fraction
+        )
+
+        return hairline_locations, bad_pixel_map
+
+    def _make_hairline_binary_and_bad_pixel_map(
+        self, array: np.ndarray
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """
+        Return two maps showing hairline pixels and bad pixels, respectively.
 
-        The angle is computed by simply looking at the slope of the two hairlines. The hairlines are identified
+        The hairline map is type `int` because it is treated as a binary image.
+        The bad pixel map is type `bool` because it will be used to index the source array.
+        """
+        hairline_locations, bad_pixel_map = self._identify_hairlines_and_bad_pixels(array)
+        map = np.zeros_like(array)
+        map[hairline_locations] = 1
+
+        return map, bad_pixel_map
+
+    def _compute_single_modstate_angles(self, array: np.ndarray) -> np.ndarray:
+        """
+        Compute the angles of a single array.
+
+        The angles are computed by simply looking at the slope of the two hairlines. The hairlines are identified
         by fitting a Gaussian to each spectral pixel based on an initial guess from the center of mass of a binarized
         image.
         """
-        # Compute the optimal number of Otsu iterations on the full array (instead of each individual hairline region)
-        # so that the signals of the strong, but narrow hairlines combine to increase hairline SNR.
-        ideal_num_otsu = self._compute_ideal_num_otsu(
-            array, max_num_otsu=self.parameters.geo_max_num_otsu
-        )
-        logger.info(f"Ideal number of Otsu iterations is {ideal_num_otsu} ")
-
-        # The 2 hairlines aren't exactly centered in these regions, but we don't care because we'll find the rough
-        # locations with a center of mass below.
-        half_idx = array.shape[1] // 2
-        hairline_1_region = array[:, :half_idx]
-        hairline_2_region = array[:, half_idx:]
+        full_binary, bad_pixel_map = self._make_hairline_binary_and_bad_pixel_map(array)
+
+        # Roughly remove any non-hairline bad pxiels. We don't need this to be perfect.
+        array[bad_pixel_map.astype(bool)] = np.nanmedian(array)
+
+        hairline_regions = self._find_hairline_regions(full_binary)
 
         angles = []
-        for h, data in enumerate([hairline_1_region, hairline_2_region], start=1):
-            # binary will be 1 on the hairlines and 0 elsewhere
-            binary = make_binary(data, ideal_num_otsu)
+        for h, hairline_idx in enumerate(hairline_regions, start=1):
+            data = array[:, hairline_idx]
+            binary = full_binary[:, hairline_idx]
             wave_size, spatial_size = data.shape
             wave_x = np.arange(wave_size)
             spatial_x = np.arange(spatial_size)
 
-            # Calculate the center of mass (COM) of the hairline for each spectral pixel. These will be the initial
-            # guesses. (The [None, :] and axis=1 allow us to compute the COM for all spectral pixels at once, so
-            # hailine_COM will have shape (wave_size, )).
-            hairline_COM = np.sum(spatial_x[None, :] * binary, axis=1) / np.sum(binary, axis=1)
+            # Compute the median spatial pixel location of all non-zero pixels in the map. This gives use a rought
+            # guess of where the hairline center is for each spectral pixel. (The [None, :] and axis=1 allow us to
+            # compute the COM for all spectral pixels at once, so hailine_centers_init_guess will have shape (wave_size, )).
+            # Set the 0s to NaN so a nanmedian will only consider non-zero pixels.
+            binary[binary == 0] = np.nan
+            hairline_centers_init_guess = np.nanmedian(spatial_x[None, :] * binary, axis=1)
 
             # Now refine hairline center with a gaussian fit at each spectral pixel
             #
             # Initialize gaussian fit centers with NaN so any bad pixels can easily be ignored during the line fit.
-            hairline_centers = np.zeros(wave_size) * np.nan
+            hairline_fit_centers = np.zeros(wave_size) * np.nan
             for i in range(wave_size):
-                if np.isnan(hairline_COM[i]):
+                if np.isnan(hairline_centers_init_guess[i]):
                     # NaNs happen when there's no identified hairline pixels at all for a particular spectral pixel.
                     logger.info(
                         f"Hairline region {h} and spectral pixel {i} has a NaN initial guess. Ignoring pixel in line fit."
                     )
                     continue
 
-                x0 = int(hairline_COM[i])
+                x0 = int(hairline_centers_init_guess[i])
                 fit_slice = slice(
                     x0 - self.parameters.geo_hairline_fit_width_px,
                     x0 + self.parameters.geo_hairline_fit_width_px,
                 )
                 hairline_profile = data[i, fit_slice]
                 abscissa = spatial_x[fit_slice]
 
@@ -435,55 +496,85 @@
                     fit_center = fit_pars[1]
                 except RuntimeError:
                     logger.info(
                         f"Hairline fit in hairline region {h} and pixel {i} failed. Ignoring pixel in line fit."
                     )
                     continue
 
-                hairline_centers[i] = fit_center
+                hairline_fit_centers[i] = fit_center
 
-            # Fit the hairlines with a simple line
-            non_nan_idx = ~np.isnan(hairline_centers)
-            coeffs = np.polyfit(wave_x[non_nan_idx], hairline_centers[non_nan_idx], 1)
+            slope = self._fit_line_to_hairline_centers(wave_x, hairline_fit_centers)
 
             # The angle is just the arctan of the slope
-            angles.append(np.arctan(coeffs[0]))
+            angles.append(np.arctan(slope))
 
-        return float(np.mean(angles))
+        return np.array(angles)
 
-    @staticmethod
-    def _compute_ideal_num_otsu(data: np.ndarray, max_num_otsu: int) -> int:
+    def _find_hairline_regions(self, binary: np.ndarray) -> list[np.ndarray]:
+        """
+        Identify spatial regions around each hairline.
+
+        This function exists because some ViSP frames show reflections of the hairlines as well as the actual hairlines.
+        Rather than ignore these we can use them to further refine the beam angle.
+
+        Regions are constrained to be within the bounds of the input array.
+
+        Returns
+        -------
+        A list of indices corresponding to each hairline
+        """
+        collapsed_binary = np.nanmean(binary, axis=0)
+        hairline_idx = pku.indexes(
+            collapsed_binary, thres=self.parameters.geo_hairline_flat_id_threshold
+        )
+        logger.info(f"Hairline centers at {hairline_idx}")
+        hairline_regions = []
+
+        region_width = self.parameters.geo_hairline_fit_width_px * 4
+        lower_limit = 0
+        upper_limit = binary.shape[1]
+        for idx in hairline_idx:
+            region = np.arange(
+                max(idx - region_width, lower_limit), min(idx + region_width, upper_limit)
+            )
+            hairline_regions.append(region)
+
+        return hairline_regions
+
+    def _fit_line_to_hairline_centers(
+        self, abscissa: np.ndarray, hairline_centers: np.ndarray
+    ) -> float:
+        """
+        Fit a 1-degree polynomial (i.e., a line) to the hairline centers.
+
+        Outliers are iteratively removed using a sigma clipping algorithm as detailed here:
+        https://docs.astropy.org/en/stable/modeling/example-fitting-line.html#iterative-fitting-using-sigma-clipping
+
+        Returns
+        -------
+        The slope of the fit line
         """
-        Determine how many iterations of Otsu's method will yield the best identification/separation of hairlines.
+        non_nan_idx = ~np.isnan(hairline_centers)
 
-        First, the fraction of pixels below the derived threshold is computed for a range of number of Otsu iterations;
-        call this function `Frac(num_otsu)`. Then we examine the 2nd derivative of `Frac`; where the slope changes
-        the most is where we stop removing non-hairline pixels with the threshold. Therefore, the location of the max
-        value in the 2nd derivative is the first Otsu iteration where the separation was not improved.
-        """
-        total_num_px = data.size
-
-        fraction_list = []
-        for num_otsu in np.arange(1, max_num_otsu):
-            binary = make_binary(data, num_otsu)
-            fraction_list.append(np.sum(binary) / total_num_px)
-
-        dd_fraction = np.diff(fraction_list, 2)
-        # Max of the 2nd derivative of the fraction as a function of num_otsu tells us where further iteration does not
-        # segment out more non-hairline pixels.
-        max_slope_change_idx = np.argmax(dd_fraction)
-
-        # We start at 3 because we took the 2nd derivative
-        otsu_dd_values = np.arange(3, max_num_otsu)
-
-        # Subtract one here because the max change in slope is where the first iteration didn't improve things. We want
-        # *last* iteration where the separation was improved because this represents the most complete hairline
-        # identification (further iterations have been shown to slightly degrade the hairline signal).
-        best_otsu = otsu_dd_values[max_slope_change_idx] - 1
-        return best_otsu
+        line_fitter = fitting.LinearLSQFitter()
+        outlier_rejection_fitter = fitting.FittingWithOutlierRemoval(
+            fitter=line_fitter,
+            outlier_func=sigma_clip,
+            sigma=self.parameters.geo_hairline_angle_fit_sig_clip,
+            niter=10,
+            cenfunc="median",
+            stdfunc="std",
+        )
+        linear_model = models.Linear1D()
+
+        fit_line, _ = outlier_rejection_fitter(
+            model=linear_model, x=abscissa[non_nan_idx], y=hairline_centers[non_nan_idx]
+        )
+
+        return fit_line.slope.value
 
     @staticmethod
     def _gaussian_with_background(x, a, x0, sigma, background_level, slope):
         """Compute a gaussian with a baseline offset and slope."""
         gaussian = a * np.exp(-((x - x0) ** 2) / (2 * sigma**2))
         return gaussian + background_level + slope * (x - x0)
 
@@ -839,37 +930,14 @@
         logger.info(f"Found {zones = }")
         mask = np.zeros(array.shape).astype(bool)
         for z in zones:
             mask[z[0] : z[1], :] = True
 
         return mask
 
-    def find_brightest_modstate(self, beam: int) -> np.ndarray:
-        """
-        Return the array for the modstate with the largest median value.
-
-        The idea here is that the brightest array will have the highest contrast between the spectra and the slit
-        hairlines, which helps in the latter's identification. It's very possible that this function doesn't make
-        any meaningful difference.
-        """
-        brightest_array = None
-        brightest_modstate = np.nan
-        median = -np.inf
-        for m in range(1, self.constants.num_modstates + 1):
-            array = self.basic_corrected_lamp_data(beam=beam, modstate=m)
-            new_median = np.median(array)
-            logger.info(f"Modstate {m} has median {new_median}")
-            if new_median > median:
-                median = new_median
-                brightest_array = array
-                brightest_modstate = m
-
-        logger.info(f"Brightest modstate is {brightest_modstate}")
-        return brightest_array
-
     @staticmethod
     def high_pass_filter_array(array: np.ndarray) -> np.ndarray:
         """Perform a simple high-pass filter to accentuate narrow features (hairlines and spectra)."""
         return array / spnd.gaussian_filter(array, sigma=5)
 
     @staticmethod
     def shift_chisq(par: np.ndarray, ref_spec: np.ndarray, spec: np.ndarray) -> float:
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,30 +89,54 @@
         The hairlines will be replaced with data from a median-filtered version of the input array.
 
         Hairlines are identified by first subtracting a spatially smoothed copy of the array and then looking for pixels
         that have large differences. This works because the hairlines are the only features that are sharp in the
         spatial dimension. The identified hairlines are then slightly smoothed spatially to ensure that their
         higher-flux wings are correctly masked.
         """
+        filtered_array = self._median_filter_array_for_hairline_identification(array)
+        hairline_locations = self._find_hairline_pixels(
+            input_array=array, filtered_array=filtered_array
+        )
+
+        # Replace hairline pixels with data from the spatially-filtered array
+        array[hairline_locations] = filtered_array[hairline_locations]
+
+        return array
+
+    def _median_filter_array_for_hairline_identification(self, array: np.ndarray) -> np.ndarray:
+        """
+        Small helper to separate out the median filter step of hairline identification.
+
+        It has been factored out so that functions that need the filtered array for further processing can avoid
+        repeating this expensive step.
+        """
         # The size=(1, X) means we only smooth in the spatial dimension (1st axis)
         filtered_array = spnd.median_filter(
             array, size=(1, self.parameters.hairline_median_spatial_smoothing_width_px)
         )
-        diff = (array - filtered_array) / filtered_array
+        return filtered_array
+
+    def _find_hairline_pixels(
+        self, input_array: np.ndarray, filtered_array: np.ndarray
+    ) -> np.ndarray:
+        """
+        Find pixels that likely correspond to hairlines.
+
+        This also slightly smooths the identified pixels so that high-flux wings of the hairlines are included.
+        """
+        diff = (input_array - filtered_array) / filtered_array
         hairline_locations = np.abs(diff) > self.parameters.hairline_fraction
 
         # Now smooth the hairline mask in the spatial dimension to capture the higher-flux wings
-        mask_array = np.zeros_like(array)
+        mask_array = np.zeros_like(input_array)
         mask_array[hairline_locations] = 1.0
         mask_array = spnd.gaussian_filter1d(
             mask_array, self.parameters.hairline_mask_spatial_smoothing_width_px, axis=1
         )
 
         hairline_locations = np.where(
             mask_array
             > mask_array.max() * self.parameters.hairline_mask_gaussian_peak_cutoff_fraction
         )
 
-        # Replace hairline pixels with data from the spatially-smoothed array
-        array[hairline_locations] = filtered_array[hairline_locations]
-
-        return array
+        return hairline_locations
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,16 +371,19 @@
     visp_background_continuum_index: WavelengthParameter = WavelengthParameter(
         values=(list(range(190)), list(range(190)), list(range(190)), list(range(190)))
     )
     visp_hairline_median_spatial_smoothing_width_px: int = 30
     visp_hairline_fraction: float = 0.11
     visp_hairline_mask_spatial_smoothing_width_px: float = 1.0
     visp_hairline_mask_gaussian_peak_cutoff_fraction: float = 0.02
-    visp_geo_max_num_otsu: int = 6
+    visp_geo_binary_opening_diameter: int = 21
+    visp_geo_hairline_flat_id_threshold: float = 0.9
     visp_geo_hairline_fit_width_px: int = 10
+    visp_geo_hairline_angle_fit_sig_clip: float = 3.0
+    visp_geo_hairline_angle_fit_min_samples: float = 0.9
     visp_geo_max_beam_2_angle_refinement: float = np.deg2rad(0.1)
     visp_geo_upsample_factor: float = 10.0
     visp_geo_max_shift: float = 40.0
     visp_geo_poly_fit_order: int = 3
     visp_solar_spectral_avg_window: WavelengthParameter = WavelengthParameter(
         values=(800, 800, 800, 800)
     )
@@ -390,15 +393,15 @@
     )
     visp_solar_zone_width: WavelengthParameter = WavelengthParameter(values=(7, 2, 3, 2))
     visp_solar_zone_bg_order: WavelengthParameter = WavelengthParameter(values=(21, 22, 11, 22))
     visp_solar_zone_normalization_percentile: WavelengthParameter = WavelengthParameter(
         values=(90, 99, 90, 90)
     )
     visp_solar_zone_rel_height: float = 0.97
-    visp_max_cs_step_time_sec: float = 20.0
+    visp_max_cs_step_time_sec: float = 180.0
     visp_polcal_spatial_median_filter_width_px: int = 10
     visp_polcal_num_spatial_bins: int = 5
     visp_polcal_demod_spatial_smooth_fit_order: int = 17
     visp_polcal_demod_spatial_smooth_min_samples: float = 0.9
     visp_polcal_demod_upsample_order: int = 3
     visp_pac_remove_linear_I_trend: bool = True
     visp_pac_fit_mode: str = "use_M12_I_sys_per_step"
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_geometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from dataclasses import dataclass
 
 import numpy as np
 import pytest
+from astropy.io import fits
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_math import transform
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.geometric import GeometricCalibration
@@ -48,15 +49,15 @@
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
             assign_input_dataset_doc_to_task(task, VispGeoTestingParameters30())
-            task.angles = np.array([0.0, 0.0])
+            task.angles = np.array([0.01, -0.01])
             task.offsets = np.zeros((number_of_beams, number_of_modstates, 2))
             task.shifts = np.zeros(intermediate_shape[0])
             for beam in range(1, number_of_beams + 1):
 
                 dark_cal = np.ones(intermediate_shape) * 3.0
                 task.intermediate_frame_helpers_write_arrays(
                     arrays=dark_cal, beam=beam, task="DARK", exposure_time=solar_exp_time
@@ -123,15 +124,16 @@
                         )
                     )
                     translated_lamp[translated_lamp == 0] = 10 * (modstate + beam + 1)
 
                     # Hairlines
                     translated_lamp[:, 30] = 5.0
                     translated_lamp[:, 70] = 5.0
-                    translated_lamp[5:15, 70] = 10 * (modstate + beam + 1)
+                    # Chop out part of the second hairline so the fitter has to skip over these pixels
+                    translated_lamp[5:9, 70] = 10 * (modstate + beam + 1)
                     distorted_lamp = next(
                         transform.rotate_arrays_about_point(
                             arrays=translated_lamp, angle=task.angles[beam - 1]
                         )
                     )
                     raw_lamp = distorted_lamp + raw_dark
                     lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.2.0/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist-processing-visp
-Version: 2.1.1
+Name: dkist_processing_visp
+Version: 2.2.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.2.0/dkist_processing_visp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/Makefile` & `dkist_processing_visp-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/background_light.rst` & `dkist_processing_visp-2.2.0/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/conf.py` & `dkist_processing_visp-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/gain_correction.rst` & `dkist_processing_visp-2.2.0/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.2.0/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/make.bat` & `dkist_processing_visp-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/polarization_calibration.rst` & `dkist_processing_visp-2.2.0/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/docs/science_calibration.rst` & `dkist_processing_visp-2.2.0/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/licenses/LICENSE.rst` & `dkist_processing_visp-2.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/pyproject.toml` & `dkist_processing_visp-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.1.1/setup.cfg` & `dkist_processing_visp-2.2.0/setup.cfg`

 * *Files identical despite different names*

