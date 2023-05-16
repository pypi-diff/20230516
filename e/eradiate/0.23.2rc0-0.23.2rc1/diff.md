# Comparing `tmp/eradiate-0.23.2rc0.tar.gz` & `tmp/eradiate-0.23.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eradiate-0.23.2rc0.tar", last modified: Tue May  9 16:07:24 2023, max compression
+gzip compressed data, was "eradiate-0.23.2rc1.tar", last modified: Tue May 16 13:35:25 2023, max compression
```

## Comparing `eradiate-0.23.2rc0.tar` & `eradiate-0.23.2rc1.tar`

### file list

```diff
@@ -1,625 +1,604 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.349281 eradiate-0.23.2rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.349281 eradiate-0.23.2rc0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.349281 eradiate-0.23.2rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    17880 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.353281 eradiate-0.23.2rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.353281 eradiate-0.23.2rc0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_ext/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_ext/pluginparameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.353281 eradiate-0.23.2rc0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-darkgrey.png
--rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-darkgrey.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_static/theme_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.337280 eradiate-0.23.2rc0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.357281 eradiate-0.23.2rc0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.357281 eradiate-0.23.2rc0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/_templates/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/convert_figures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.365281 eradiate-0.23.2rc0/docs/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/atmosphere_attributes.png
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/atmosphere_attributes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-east_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-east_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-east_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-east_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-north_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-north_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-north_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-north_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-south_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-south_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-south_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-south_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-west_left.png
--rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-west_left.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-west_right.png
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/azimuth-west_right.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/cartesian-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/cartesian-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/cuboid_leaf_cloud_params.png
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/cuboid_leaf_cloud_params.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.365281 eradiate-0.23.2rc0/docs/fig/diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/diagrams/class_diagram_biosphere.drawio
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/diagrams/package.drawio
--rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/eradiate-logo-typo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/eradiate-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/icon_eradiate.png
--rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/package.png
--rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/package.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/radiancemeter_hsphere.png
--rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/radiancemeter_hsphere.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/radiancemeter_plane.png
--rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/radiancemeter_plane.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/requirement_layers.png
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/requirement_layers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/solid_2017.png
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_noatm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_atm_interval.png
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_atm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_interval1.png
--rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_interval2.png
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_isolated.png
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spherical-coordinate-system.png
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/spherical-coordinate-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/fig/thuillier_2003.png
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/generate_md_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/generate_rst_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/generate_rst_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/index_latex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.369281 eradiate-0.23.2rc0/docs/rst/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/dependencies.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.369281 eradiate-0.23.2rc0/docs/rst/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/design_atmosphere.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/factory_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/lazy_loading.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/radiometric_kernel_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/developer_guide/scene_generator.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.369281 eradiate-0.23.2rc0/docs/rst/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/getting_started/update.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/maintainer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.377281 eradiate-0.23.2rc0/docs/rst/reference_api/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/attrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/constants.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/contexts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/converters.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/eradiate_core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/kernel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/mode.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/notebook.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/pipelines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/quad.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/rng.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/scenes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/srf_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/test_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/util.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/warp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_api/xarray.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.377281 eradiate-0.23.2rc0/docs/rst/reference_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/reference_plugins/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.377281 eradiate-0.23.2rc0/docs/rst/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.377281 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/absorption.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.377281 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/good_resolution.png
--rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/line.png
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/heterogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/homogeneous.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/molecular.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/particle_layer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/basic_concepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.381281 eradiate-0.23.2rc0/docs/rst/user_guide/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/absorption.rst
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/atmosphere_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/atmosphere_thermoprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/ckd.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.381281 eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
--rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/pt_points.png
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/particle_radprops.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/solar_irradiance.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/spectra-us76_u86_4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/data/srf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/onedim_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/package_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/spectral_discretization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/rst/user_guide/unit_guide_user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.381281 eradiate-0.23.2rc0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (123)    17880 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/src/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/docs/src/reference_cli.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.381281 eradiate-0.23.2rc0/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/ext/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.389281 eradiate-0.23.2rc0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/check_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/copy_envvars.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-minimal.yml
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-optional.yml
--rw-r--r--   0 runner    (1001) docker     (123)    30957 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-production.yml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment-recommended.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/environment.in
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/layered.yml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/make_conda_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/make_pip_in_files.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/optional.in
--rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/production.in
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/recommended.in
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/tests.in
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/requirements/tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.389281 eradiate-0.23.2rc0/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/resources/downloads.yml
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/setpath.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.341281 eradiate-0.23.2rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.393281 eradiate-0.23.2rc0/src/eradiate/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/attrs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.393281 eradiate-0.23.2rc0/src/eradiate/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/cli/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/cli/srf.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.397281 eradiate-0.23.2rc0/src/eradiate/data/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_safe_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/data/_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.397281 eradiate-0.23.2rc0/src/eradiate/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/experiments/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.401281 eradiate-0.23.2rc0/src/eradiate/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/_bitmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/_bsdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/kernel/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.401281 eradiate-0.23.2rc0/src/eradiate/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/notebook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/notebook/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.401281 eradiate-0.23.2rc0/src/eradiate/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/pipelines/_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.405281 eradiate-0.23.2rc0/src/eradiate/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/_util_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/radprops/rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/rng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.405281 eradiate-0.23.2rc0/src/eradiate/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.405281 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.409281 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.409281 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_black.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.409281 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.413281 eradiate-0.23.2rc0/src/eradiate/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/integrators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/integrators/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/integrators/_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.413281 eradiate-0.23.2rc0/src/eradiate/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/measure/_radiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.417281 eradiate-0.23.2rc0/src/eradiate/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/phase/_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.421281 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.421281 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_multi_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.425281 eradiate-0.23.2rc0/src/eradiate/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/scenes/surface/_dem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.425281 eradiate-0.23.2rc0/src/eradiate/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/spectral/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/spectral/ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/spectral/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/spectral/mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.425281 eradiate-0.23.2rc0/src/eradiate/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/test_tools/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/test_tools/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/test_tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/test_tools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.429282 eradiate-0.23.2rc0/src/eradiate/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/thermoprops/afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/thermoprops/us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/thermoprops/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.429282 eradiate-0.23.2rc0/src/eradiate/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/util/numpydoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/util/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.433282 eradiate-0.23.2rc0/src/eradiate/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/xarray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/xarray/_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/xarray/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/src/eradiate/xarray/interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.393281 eradiate-0.23.2rc0/src/eradiate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:07:23.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 16:07:24.000000 eradiate-0.23.2rc0/src/eradiate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.433282 eradiate-0.23.2rc0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.433282 eradiate-0.23.2rc0/tests/01_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.433282 eradiate-0.23.2rc0/tests/01_plugins/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/bsdfs/test_bilambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/bsdfs/test_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.433282 eradiate-0.23.2rc0/tests/01_plugins/phase/
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/phase/test_tabphase_irregular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.437282 eradiate-0.23.2rc0/tests/01_plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/sensors/test_distantflux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/sensors/test_hdistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/sensors/test_mdistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/sensors/test_mradiancemeter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.437282 eradiate-0.23.2rc0/tests/01_plugins/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/01_plugins/volumes/test_spherical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.437282 eradiate-0.23.2rc0/tests/02_eradiate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.441282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.441282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_blind_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_blind_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_safe_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_safe_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.445282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_canopy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.445282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_gridvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_kernel_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.449282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_gather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.449282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_afgl_1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_rayleigh_scattering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_us76_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_zgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.449282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.453282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.453282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.457282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_black.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_rpv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.457282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_directional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_spot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.457282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/integrators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.461282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_distant_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_multi_distant.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_radiancemeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.461282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_blend.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_isotropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_rayleigh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_tabulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.465282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_buffermesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_cuboid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_filemesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.465282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_interpolated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.469282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_central_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_dem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.469282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_ckd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_srf_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.469282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_tools/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.469282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_us76.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.473282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.473282 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/xarray/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/01_unit/xarray/test_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.477282 eradiate-0.23.2rc0/tests/02_eradiate/02_system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_albedo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_atmosphere_rpv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_ckd_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_compare_canopy_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_irradiance_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_kernel_render_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_maximum_scene_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_mdistant_insitu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_lambertian_brf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_spectral_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/rami4atm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/rami4atm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:24.481282 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het04.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het06.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/02_eradiate/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-09 16:07:09.000000 eradiate-0.23.2rc0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.883456 eradiate-0.23.2rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_ext/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_ext/pluginparameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25531 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34059 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.879456 eradiate-0.23.2rc1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.887456 eradiate-0.23.2rc1/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/_templates/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/convert_figures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    20540 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28149 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35278 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-east_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    30666 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32862 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28115 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-north_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28153 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32939 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28118 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32455 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-south_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28178 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32935 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28067 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/azimuth-west_right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15939 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25301 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/fig/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/diagrams/package.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)    40438 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/eradiate-logo-typo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/eradiate-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/icon_eradiate.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38873 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/package.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57417 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/package.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32384 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.png
+-rw-r--r--   0 runner    (1001) docker     (123)    43351 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36773 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31853 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/requirement_layers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/requirement_layers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21451 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/solid_2017.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16459 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28519 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14036 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/fig/thuillier_2003.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_md_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_rst_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/generate_rst_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/index_latex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/dependencies.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/design_atmosphere.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/factory_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/lazy_loading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/developer_guide/scene_generator.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.895456 eradiate-0.23.2rc1/docs/rst/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/getting_started/update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/maintainer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/reference_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/attrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/constants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/contexts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/converters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/eradiate_core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/mode.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/notebook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/pipelines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/quad.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/rng.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/scenes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/srf_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/test_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/validators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/warp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_api/xarray.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/reference_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/reference_plugins/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.899456 eradiate-0.23.2rc1/docs/rst/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/absorption.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    25171 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24938 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/line.png
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/homogeneous.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/molecular.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/particle_layer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/basic_concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/absorption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/ckd.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    30117 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59107 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/pt_points.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/particle_radprops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/solar_irradiance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/spectra-us76_u86_4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/data/srf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/onedim_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/package_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/spectral_discretization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/rst/user_guide/unit_guide_user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.903456 eradiate-0.23.2rc1/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18002 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/src/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/docs/src/reference_cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.907456 eradiate-0.23.2rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/check_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/copy_envvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    39893 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-minimal.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-optional.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    30957 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-production.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment-recommended.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/environment.in
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/layered.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/make_conda_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/make_pip_in_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/optional.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20920 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/production.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/recommended.in
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/tests.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/setpath.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.879456 eradiate-0.23.2rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/attrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/cli/srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_safe_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/downloads.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/data/downloads_development.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20760 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/experiments/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_bitmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_bsdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/kernel/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/notebook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/notebook/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/pipelines/_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/_util_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/radprops/rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/rng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.915456 eradiate-0.23.2rc1/src/eradiate/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38992 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.919456 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/measure/_radiancemeter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/phase/_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_multi_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.923456 eradiate-0.23.2rc1/src/eradiate/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/scenes/surface/_dem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/spectral/mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26485 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/test_tools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42061 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/thermoprops/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/numpydoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/util/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/src/eradiate/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/src/eradiate/xarray/interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.911456 eradiate-0.23.2rc1/src/eradiate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21002 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 13:35:25.000000 eradiate-0.23.2rc1/src/eradiate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/01_eradiate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.927456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_gather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.931456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.935456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_us76.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.939456 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/02_system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_albedo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25312 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:25.943456 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/01_eradiate/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-16 13:35:14.000000 eradiate-0.23.2rc1/tests/conftest.py
```

### Comparing `eradiate-0.23.2rc0/.clang-format` & `eradiate-0.23.2rc1/.clang-format`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.github/ISSUE_TEMPLATE/feature_request.md` & `eradiate-0.23.2rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.github/pull_request_template.md` & `eradiate-0.23.2rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.github/workflows/cd.yml` & `eradiate-0.23.2rc1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.github/workflows/ci.yml` & `eradiate-0.23.2rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.pre-commit-config.yaml` & `eradiate-0.23.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/.readthedocs.yml` & `eradiate-0.23.2rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/CHANGELOG.md` & `eradiate-0.23.2rc1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
 * Exposed the ``eradiate.spectral.*`` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
+* Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
+* Provide an Eradiate Pypi package ({ghpr}`328`)
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
```

### Comparing `eradiate-0.23.2rc0/CONTRIBUTING.md` & `eradiate-0.23.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/LICENSE` & `eradiate-0.23.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/Makefile` & `eradiate-0.23.2rc1/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,21 @@
 	python3 requirements/copy_envvars.py
 	pip install --editable . --no-deps
 
 conda-update: conda-lock-all conda-init
 
 .PHONY: conda-env conda-lock conda-lock-all conda-init conda-update
 
+# -- Build the Eradiate Mitsuba kernel -----------------------------------------
+
+kernel:
+	cmake -S ext/mitsuba -B ext/mitsuba/build -DCMAKE_BUILD_TYPE=Release -GNinja --preset eradiate
+	ninja -C ext/mitsuba/build
+
+
 # -- Build Wheel for Eradiate --------------------------------------------------
 
 wheel:
 	python3 -m build
 
 # -- Documentation -------------------------------------------------------------
```

### Comparing `eradiate-0.23.2rc0/PKG-INFO` & `eradiate-0.23.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc0
+Version: 0.23.2rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc0/README.md` & `eradiate-0.23.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/Makefile` & `eradiate-0.23.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_ext/exec.py` & `eradiate-0.23.2rc1/docs/_ext/exec.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_ext/pluginparameters.py` & `eradiate-0.23.2rc1/docs/_ext/pluginparameters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-black.svg` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-black.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-darkgrey.png` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-darkgrey.svg` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-darkgrey.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-white.png` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_static/eradiate-logo-typo-white.svg` & `eradiate-0.23.2rc1/docs/_static/eradiate-logo-typo-white.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_templates/autosummary/module.rst` & `eradiate-0.23.2rc1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/_templates/sections/footer-content.html` & `eradiate-0.23.2rc1/docs/_templates/sections/footer-content.html`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/conf.py` & `eradiate-0.23.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/atmosphere_attributes.png` & `eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/atmosphere_attributes.svg` & `eradiate-0.23.2rc1/docs/fig/atmosphere_attributes.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-east_left.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-east_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-east_left.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-east_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-east_right.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-east_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-east_right.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-east_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-north_left.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-north_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-north_left.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-north_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-north_right.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-north_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-north_right.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-north_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-south_left.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-south_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-south_left.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-south_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-south_right.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-south_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-south_right.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-south_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-west_left.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-west_left.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-west_left.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-west_left.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-west_right.png` & `eradiate-0.23.2rc1/docs/fig/azimuth-west_right.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/azimuth-west_right.svg` & `eradiate-0.23.2rc1/docs/fig/azimuth-west_right.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/cartesian-coordinate-system.png` & `eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/cartesian-coordinate-system.svg` & `eradiate-0.23.2rc1/docs/fig/cartesian-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/cuboid_leaf_cloud_params.png` & `eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/cuboid_leaf_cloud_params.svg` & `eradiate-0.23.2rc1/docs/fig/cuboid_leaf_cloud_params.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/diagrams/class_diagram_biosphere.drawio` & `eradiate-0.23.2rc1/docs/fig/diagrams/class_diagram_biosphere.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio` & `eradiate-0.23.2rc1/docs/fig/diagrams/cuboid_leaf_cloud_params.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/diagrams/package.drawio` & `eradiate-0.23.2rc1/docs/fig/diagrams/package.drawio`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/eradiate-logo-typo-black.png` & `eradiate-0.23.2rc1/docs/fig/eradiate-logo-typo-black.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/eradiate-logo.svg` & `eradiate-0.23.2rc1/docs/fig/eradiate-logo.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/icon_eradiate.png` & `eradiate-0.23.2rc1/docs/fig/icon_eradiate.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/package.png` & `eradiate-0.23.2rc1/docs/fig/package.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/package.svg` & `eradiate-0.23.2rc1/docs/fig/package.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/radiancemeter_hsphere.png` & `eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/radiancemeter_hsphere.svg` & `eradiate-0.23.2rc1/docs/fig/radiancemeter_hsphere.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/radiancemeter_plane.png` & `eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/radiancemeter_plane.svg` & `eradiate-0.23.2rc1/docs/fig/radiancemeter_plane.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/requirement_layers.png` & `eradiate-0.23.2rc1/docs/fig/requirement_layers.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/requirement_layers.svg` & `eradiate-0.23.2rc1/docs/fig/requirement_layers.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/solid_2017.png` & `eradiate-0.23.2rc1/docs/fig/solid_2017.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_atm_interval.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_atm_isolated.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_noatm_interval.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_ckd_noatm_isolated.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_ckd_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_atm_interval.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_interval.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_atm_isolated.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_atm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_interval1.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval1.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_interval2.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_interval2.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spectral_discretization_mono_noatm_isolated.png` & `eradiate-0.23.2rc1/docs/fig/spectral_discretization_mono_noatm_isolated.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spherical-coordinate-system.png` & `eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/spherical-coordinate-system.svg` & `eradiate-0.23.2rc1/docs/fig/spherical-coordinate-system.svg`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/fig/thuillier_2003.png` & `eradiate-0.23.2rc1/docs/fig/thuillier_2003.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/generate_md_cli.py` & `eradiate-0.23.2rc1/docs/generate_md_cli.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/generate_rst_api.py` & `eradiate-0.23.2rc1/docs/generate_rst_api.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/generate_rst_plugins.py` & `eradiate-0.23.2rc1/docs/generate_rst_plugins.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/index.rst` & `eradiate-0.23.2rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/make.bat` & `eradiate-0.23.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/references.bib` & `eradiate-0.23.2rc1/docs/references.bib`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/contributing.rst` & `eradiate-0.23.2rc1/docs/rst/contributing.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/dependencies.rst` & `eradiate-0.23.2rc1/docs/rst/dependencies.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/developer_guide/design_atmosphere.rst` & `eradiate-0.23.2rc1/docs/rst/developer_guide/design_atmosphere.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/developer_guide/factory_guide.rst` & `eradiate-0.23.2rc1/docs/rst/developer_guide/factory_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/developer_guide/lazy_loading.rst` & `eradiate-0.23.2rc1/docs/rst/developer_guide/lazy_loading.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/developer_guide/radiometric_kernel_interface.rst` & `eradiate-0.23.2rc1/docs/rst/developer_guide/radiometric_kernel_interface.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/developer_guide/scene_generator.rst` & `eradiate-0.23.2rc1/docs/rst/developer_guide/scene_generator.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/getting_started/index.rst` & `eradiate-0.23.2rc1/docs/rst/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/getting_started/install.rst` & `eradiate-0.23.2rc1/docs/rst/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/getting_started/update.rst` & `eradiate-0.23.2rc1/docs/rst/getting_started/update.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/maintainer_guide.rst` & `eradiate-0.23.2rc1/docs/rst/maintainer_guide.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/data.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/data.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/eradiate_core.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/eradiate_core.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/experiments.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/experiments.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/factory.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/factory.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/index.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/index.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/kernel.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/kernel.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/pipelines.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/pipelines.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/scenes.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/scenes.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/srf_tools.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/srf_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/test_tools.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/test_tools.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/reference_api/xarray.rst` & `eradiate-0.23.2rc1/docs/rst/reference_api/xarray.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/absorption.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/bad_resolution.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/bad_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/good_resolution.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/good_resolution.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/fig/line.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/fig/line.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/heterogeneous.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/heterogeneous.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/intro.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/molecular.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/molecular.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/atmosphere/rayleigh_scattering.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/basic_concepts.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/basic_concepts.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/conventions.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/conventions.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/absorption.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/absorption.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/atmosphere_radprops.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/atmosphere_thermoprops.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/atmosphere_thermoprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/ckd.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/ckd.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/pt_points.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/pt_points.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/intro.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/intro.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/particle_radprops.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/particle_radprops.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/solar_irradiance.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/solar_irradiance.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/spectra-us76_u86_4.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/spectra-us76_u86_4.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/data/srf.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/data/srf.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/onedim_experiment.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/onedim_experiment.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/package_structure.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/package_structure.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/spectral_discretization.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/spectral_discretization.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/rst/user_guide/unit_guide_user.rst` & `eradiate-0.23.2rc1/docs/rst/user_guide/unit_guide_user.rst`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/docs/src/CHANGELOG.md` & `eradiate-0.23.2rc1/docs/src/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
 ### Improvements and fixes
 
 * Added {class}`.MultiDeltaSpectrum` spectrum type ({ghpr}`311`).
 * Exposed several API members in the top-level namespace ({ghpr}`324`).
 * Exposed the ``eradiate.spectral.*`` subpackage members in the
   {mod}`eradiate.spectral` namespace ({ghpr}`324`).
+* Fixed incorrect Mitsuba scene parameter drop and lookup ({ghpr}`329`).
+* Provide an Eradiate Pypi package ({ghpr}`328`)
 
 ### Documentation
 
 * Added a user guide page on spectral discretization.
 
 ### Internal changes
```

### Comparing `eradiate-0.23.2rc0/docs/src/reference_cli.md` & `eradiate-0.23.2rc1/docs/src/reference_cli.md`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/pyproject.toml` & `eradiate-0.23.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 ]
 src = ["src", "tests"]
 
 [tool.ruff.isort]
 relative-imports-order = "closest-to-furthest"
 
 [tool.setuptools]
-zip-safe = false  # Required because of package data
+include-package-data = true # Required because of package data
 
 [tool.setuptools.package-data]
 # Required by PEP 561
 # https://mypy.readthedocs.io/en/stable/installed_packages.html#creating-pep-561-compatible-packages
 eradiate = ["py.typed", "*.pyi"]
 
 [tool.setuptools.packages.find]
```

### Comparing `eradiate-0.23.2rc0/requirements/copy_envvars.py` & `eradiate-0.23.2rc1/requirements/copy_envvars.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/dev.txt` & `eradiate-0.23.2rc1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/docs.txt` & `eradiate-0.23.2rc1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-dev.yml` & `eradiate-0.23.2rc1/requirements/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-linux-64.lock` & `eradiate-0.23.2rc1/requirements/environment-linux-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-optional.yml` & `eradiate-0.23.2rc1/requirements/environment-optional.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-osx-64.lock` & `eradiate-0.23.2rc1/requirements/environment-osx-64.lock`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-production.yml` & `eradiate-0.23.2rc1/requirements/environment-production.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/environment-recommended.yml` & `eradiate-0.23.2rc1/requirements/environment-recommended.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/layered.yml` & `eradiate-0.23.2rc1/requirements/layered.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/main.txt` & `eradiate-0.23.2rc1/requirements/main.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/make_conda_env.py` & `eradiate-0.23.2rc1/requirements/make_conda_env.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/make_pip_in_files.py` & `eradiate-0.23.2rc1/requirements/make_pip_in_files.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/optional.txt` & `eradiate-0.23.2rc1/requirements/optional.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/production.txt` & `eradiate-0.23.2rc1/requirements/production.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/requirements/tests.txt` & `eradiate-0.23.2rc1/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/resources/downloads.yml` & `eradiate-0.23.2rc1/src/eradiate/data/downloads_development.yml`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/setpath.sh` & `eradiate-0.23.2rc1/setpath.sh`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/_config.py` & `eradiate-0.23.2rc1/src/eradiate/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,14 +161,28 @@
                 "using Eradiate directly from the sources, you can alternatively "
                 "source the provided setpath.sh script. If you wish to use Eradiate "
                 "in a production environment, you can install the eradiate-mitsuba "
                 "package using 'pip install eradiate-mitsuba' and unset the "
                 "'ERADIATE_SOURCE_DIR' environment variable."
             ) from FileNotFoundError(eradiate_init)
 
+    #: URL where small data files are located (production use only)
+    small_files_registry_url = var(
+        default="https://raw.githubusercontent.com/eradiate/eradiate-data",
+        converter=str,
+        help="URL where small data files are located (production use only)",
+    )
+
+    #: Revision of the small files registry (production use only)
+    small_files_registry_revision = var(
+        default="master",
+        converter=str,
+        help="Revision of the small files registry (production use only)",
+    )
+
     #: URL where large data files are located.
     data_store_url = var(
         default="http://eradiate.eu/data/store/",
         converter=str,
         help="URL where large data files are located.",
     )
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/_factory.py` & `eradiate-0.23.2rc1/src/eradiate/_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/_mode.py` & `eradiate-0.23.2rc1/src/eradiate/_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/attrs.py` & `eradiate-0.23.2rc1/src/eradiate/attrs.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/cli/__init__.py` & `eradiate-0.23.2rc1/src/eradiate/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/cli/data.py` & `eradiate-0.23.2rc1/src/eradiate/cli/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os.path
 import textwrap
 from pathlib import Path
 from typing import List, Optional
+from importlib_resources import files
 
 import typer
 from rich.console import Console
 from ruamel.yaml import YAML
 from typing_extensions import Annotated
-
 import eradiate
 
 from ..exceptions import DataError
 
 app = typer.Typer()
 console = Console(color_system=None)
 
@@ -108,15 +108,15 @@
             data_store.registry_fetch()
             console.print("  [green]✓ Done[/]")
             continue
 
 
 @app.command()
 def fetch(
-    files: Annotated[
+    file_list: Annotated[
         Optional[List[str]],
         typer.Argument(
             help="An arbitrary number of relative paths to files to be "
             "retrieved from the data store. If unset, the list of "
             "files is read from a YAML file which can be specified by "
             "using the ``--from-file`` option and defaults to "
             "``$ERADIATE_SOURCE_DIR/resources/downloads.yml``."
@@ -131,23 +131,26 @@
             "the FILES argument(s) will be ignored.",
         ),
     ] = None,
 ):
     """
     Fetch files from the Eradiate data store.
     """
-    if not files:
+    if not file_list:
         if from_file is None:
             # TODO: fetch this list from online
-            from_file = eradiate.config.source_dir / "resources/downloads.yml"
+            if eradiate.config.source_dir is None:
+                from_file = files("eradiate") / "data" / "downloads.yml"
+            else:
+                from_file = eradiate.config.source_dir / "data" / "downloads_development.yml"
         console.print(f"Reading file list from '{from_file}'")
         yaml = YAML()
-        files = yaml.load(from_file)
+        file_list = yaml.load(from_file)
 
-    for filename in files:
+    for filename in file_list:
         try:
             console.print(f"[blue]Fetching '{filename}'[/]")
             path = eradiate.data.data_store.fetch(filename)
         except DataError:
             console.print(f"[red]✗[/] not found")
         else:
             console.print(f"[green]✓[/] found \[{path}]")
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/cli/show.py` & `eradiate-0.23.2rc1/src/eradiate/cli/show.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/cli/srf.py` & `eradiate-0.23.2rc1/src/eradiate/cli/srf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/contexts.py` & `eradiate-0.23.2rc1/src/eradiate/contexts.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/converters.py` & `eradiate-0.23.2rc1/src/eradiate/converters.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_access.py` & `eradiate-0.23.2rc1/src/eradiate/data/_access.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_blind_directory.py` & `eradiate-0.23.2rc1/src/eradiate/data/_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_blind_online.py` & `eradiate-0.23.2rc1/src/eradiate/data/_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_core.py` & `eradiate-0.23.2rc1/src/eradiate/data/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_multi.py` & `eradiate-0.23.2rc1/src/eradiate/data/_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_safe_directory.py` & `eradiate-0.23.2rc1/src/eradiate/data/_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_safe_online.py` & `eradiate-0.23.2rc1/src/eradiate/data/_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/data/_store.py` & `eradiate-0.23.2rc1/src/eradiate/data/_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._safe_online import SafeOnlineDataStore
 from .._config import config
 
 #: Global data store.
 data_store: MultiDataStore = None
 
 
-def init_data_store(offline: bool | None = None) -> None:
+def init_data_store(offline: bool | None = None, production: bool | None = None) -> None:
     """
     Initialize the global data store.
 
     Parameters
     ----------
     offline : bool, optional
         If ``True``, replace all online data stores with blind directory data
@@ -29,52 +29,60 @@
     imported.
     """
     global data_store
 
     if offline is None:
         offline = config.offline
 
+    if production is None:
+        production = config.source_dir is None
+
+    if not production:
+        small_files = SafeDirectoryDataStore(
+            path=config.source_dir / "resources" / "data"
+        )
+    else:
+        if offline:
+            small_files = BlindDirectoryDataStore(
+                path=config.download_dir / "resources" / "data"
+            )
+        else:
+            small_files = SafeOnlineDataStore(
+                base_url="/".join([config.small_files_registry_url, config.small_files_registry_revision,]),
+                path=config.download_dir / "resources" / "data",
+            )
+
     if not offline:
         data_store = MultiDataStore(
             stores=OrderedDict(
                 [
-                    (
-                        "small_files",
-                        SafeDirectoryDataStore(
-                            path=config.source_dir / "resources/data/"
-                        ),
-                    ),
+                    ("small_files", small_files),
                     (
                         "large_files_stable",
                         SafeOnlineDataStore(
-                            base_url="http://eradiate.eu/data/store/stable/",
+                            base_url="/".join([config.data_store_url, "stable"]),
                             path=config.download_dir / "stable",
                         ),
                     ),
                     (
                         "large_files_unstable",
                         BlindOnlineDataStore(
-                            base_url="http://eradiate.eu/data/store/unstable/",
+                            base_url="/".join([config.data_store_url, "unstable"]),
                             path=config.download_dir / "unstable",
                         ),
                     ),
                 ]
             )
         )
 
     else:
         data_store = MultiDataStore(
             stores=OrderedDict(
                 [
-                    (
-                        "small_files",
-                        SafeDirectoryDataStore(
-                            path=config.source_dir / "resources/data/"
-                        ),
-                    ),
+                    ("small_files", small_files),
                     (
                         "large_files_stable",
                         BlindDirectoryDataStore(path=config.download_dir / "stable"),
                     ),
                     (
                         "large_files_unstable",
                         BlindDirectoryDataStore(path=config.download_dir / "unstable"),
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/exceptions.py` & `eradiate-0.23.2rc1/src/eradiate/exceptions.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_atmosphere.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_canopy.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_canopy_atmosphere.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_core.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_dem.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/experiments/_helpers.py` & `eradiate-0.23.2rc1/src/eradiate/experiments/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/frame.py` & `eradiate-0.23.2rc1/src/eradiate/frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/__init__.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/_bitmap.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/_bitmap.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/_bsdf.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/_bsdf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/_kernel_dict.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/_render.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/_render.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 import typing as t
+import warnings
 
 import attrs
 import mitsuba as mi
 from tqdm.auto import tqdm
 
 from ._kernel_dict import UpdateMapTemplate
 from .._config import ProgressLevel, config
@@ -110,18 +111,34 @@
         default="None",
     )
 
     def drop_parameters(self) -> None:
         """
         Reduce the size of the scene parameter table :attr:`.parameters` by
         only keeping elements whose keys are listed in the parameter update
-        map template :attr:`.umap_template`.
+        map template :attr:`.umap_template`. For parameters associated with a
+        lookup protocol, the looked up parameter ID is checked and used.
         """
         if self.umap_template is not None:
-            self.parameters.keep(list(self.umap_template.keys()))
+            keys = []
+            for name, param in self.umap_template.items():
+                if param.lookup_strategy is not None:
+                    if param.parameter_id is not None:
+                        keys.append(param.parameter_id)
+                    else:
+                        warnings.warn(
+                            f"Parameter '{name}' has a lookup strategy but the "
+                            "associated parameter ID is undefined; was a "
+                            "parameter lookup performed during the Mitsuba "
+                            "scene traversal?"
+                        )
+                else:
+                    keys.append(name)
+
+            self.parameters.keep(keys)
 
 
 def mi_traverse(
     obj: mi.Object,
     umap_template: UpdateMapTemplate | None = None,
 ) -> MitsubaObjectWrapper:
     """
@@ -187,18 +204,21 @@
             self.name = name
             self.node = node
             self.depth = depth
             self.hierarchy[node] = (parent, depth)
             self.flags = flags
 
             # Try and recover a parameter ID from this node
-            for uparam in list(lookups.values()):
+            for name, uparam in list(lookups.items()):
                 lookup_result = uparam.lookup_strategy(self.node, self.name)
                 if lookup_result is not None:
                     uparam.parameter_id = lookup_result
+                    del lookups[
+                        name
+                    ]  # Remove successful lookups to accelerate future searches
 
         def put_parameter(self, name, ptr, flags, cpptype=None):
             name = name if self.name is None else self.name + "." + name
 
             flags = self.flags | flags
             # Non-differentiable parameters shouldn't be flagged as discontinuous
             if (flags & mi.ParamFlags.NonDifferentiable) != 0:
@@ -220,14 +240,21 @@
                 flags=self.flags | flags,
             )
             node.traverse(cb)
 
     cb = SceneTraversal(obj)
     obj.traverse(cb)
 
+    # Check if there are unsuccessful lookups
+    if lookups:
+        warnings.warn(
+            "There were unsuccessful Mitsuba scene parameter lookups: "
+            f"{list(lookups.keys())}"
+        )
+
     return MitsubaObjectWrapper(
         obj=obj,
         parameters=mi.SceneParameters(cb.properties, cb.hierarchy),
         umap_template=umap_template,
     )
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/gridvolume.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/logging.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/kernel/transform.py` & `eradiate-0.23.2rc1/src/eradiate/kernel/transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/notebook/__init__.py` & `eradiate-0.23.2rc1/src/eradiate/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/notebook/tutorials.py` & `eradiate-0.23.2rc1/src/eradiate/notebook/tutorials.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/_aggregate.py` & `eradiate-0.23.2rc1/src/eradiate/pipelines/_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/_assemble.py` & `eradiate-0.23.2rc1/src/eradiate/pipelines/_assemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         def eval_illumination_spectrum(
             field_name: str, k_units: pint.Unit
         ) -> pint.Quantity:
             # Local helper function to help with illumination spectrum evaluation
 
             spectrum: Spectrum = getattr(illumination, field_name)
             results_wavelengths = to_quantity(x.w)
-            print(f"{results_wavelengths=}")
 
             if eradiate.mode().is_mono:
                 wavelengths = results_wavelengths
                 assert np.allclose(wavelengths, wavelengths_dataset)
                 return spectrum.eval_mono(wavelengths).m_as(k_units)
 
             elif eradiate.mode().is_ckd:
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/_compute.py` & `eradiate-0.23.2rc1/src/eradiate/pipelines/_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/_core.py` & `eradiate-0.23.2rc1/src/eradiate/pipelines/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/pipelines/_gather.py` & `eradiate-0.23.2rc1/src/eradiate/pipelines/_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/plot.py` & `eradiate-0.23.2rc1/src/eradiate/plot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/quad.py` & `eradiate-0.23.2rc1/src/eradiate/quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/_afgl1986.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/_core.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/_us76_approx.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/_util_mono.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/_util_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/absorption.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/radprops/rayleigh.py` & `eradiate-0.23.2rc1/src/eradiate/radprops/rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/rng.py` & `eradiate-0.23.2rc1/src/eradiate/rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_heterogeneous.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_homogeneous.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_molecular_atmosphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             default=None,
             converter=attrs.converters.optional(
                 converters.to_dataset(load_from_id=None)
             ),
             validator=attrs.validators.optional(
                 attrs.validators.instance_of(xr.Dataset)
             ),
+            repr=summary_repr,
         ),
         doc="Absorption coefficient dataset. If ``None``, the absorption "
         "coefficient is set to zero.",
         type="Dataset",
         init_type="PathLike or Dataset",
         default="None",
     )
@@ -352,15 +353,16 @@
         However, this class allows you to rescale the concentrations of each
         individual molecular species to custom concentration values.
         Custom concentrations can be provided in different units.
         """
         if "absorption_dataset" in kwargs:
             raise TypeError(
                 "Cannot pass 'absorption_dataset' keyword argument. The "
-                "'afgl_1986' sets the absorption dataset automatically."
+                "'afgl_1986' constructor sets the absorption dataset "
+                "automatically."
             )
 
         thermoprops = afgl_1986.make_profile(model_id=model)
 
         path = "ckd/absorption"
         if kwargs.get("has_absorption", True):
             if binset == "10nm":
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_particle_dist.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/atmosphere/_particle_layer.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/atmosphere/_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_discrete.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_leaf_cloud.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/biosphere/_tree.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/biosphere/_tree.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_checkerboard.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_checkerboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,17 @@
 
     @property
     def template(self) -> dict:
         # Inherit docstring
 
         result = {"type": "diffuse", "reflectance.type": "checkerboard"}
 
+        if self.id is not None:
+            result["id"] = self.id
+
         for obj_key, obj_values in {
             "color0": traverse(self.reflectance_a)[0],
             "color1": traverse(self.reflectance_b)[0],
         }.items():
             for key, value in obj_values.items():
                 result[f"reflectance.{obj_key}.{key}"] = value
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_lambertian.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_lambertian.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,27 @@
         init_type=".Spectrum or dict or float",
         default="0.5",
     )
 
     @property
     def template(self) -> dict:
         # Inherit docstring
-        return {
+        result = {
             "type": "diffuse",
             **{
                 f"reflectance.{key}": value
                 for key, value in traverse(self.reflectance)[0].items()
             },
         }
 
+        if self.id is not None:
+            result["id"] = self.id
+
+        return result
+
     @property
     def params(self) -> dict[str, UpdateParameter]:
         # Inherit docstring
         params = traverse(self.reflectance)[1].data
 
         result = {}
         for key, param in params.items():
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_mqdiffuse.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_mqdiffuse.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,16 +117,22 @@
             .values
         )
         return mi.VolumeGrid(values.astype(np.float32))
 
     @property
     def template(self) -> dict:
         # Inherit docstring
-        return {
+
+        result = {
             "type": "mqdiffuse",
             "grid": InitParameter(lambda ctx: self._eval_grid_impl(ctx)),
         }
 
+        if self.id is not None:
+            result["id"] = self.id
+
+        return result
+
     @property
     def params(self) -> dict[str, UpdateParameter]:
         # Inherit docstring
         return {}
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/bsdfs/_rpv.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/bsdfs/_rpv.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,14 +118,17 @@
 
         result = {"type": "rpv"}
 
         for obj_key, obj_values in objects.items():
             for key, value in obj_values.items():
                 result[f"{obj_key}.{key}"] = value
 
+        if self.id is not None:
+            result["id"] = self.id
+
         return result
 
     @property
     def params(self) -> dict[str, UpdateParameter]:
         # Inherit docstring
         objects = {
             "rho_0": traverse(self.rho_0)[1],
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/geometry.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/geometry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_constant.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_directional.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/illumination/_spot.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/illumination/_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/integrators/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/integrators/_path_tracers.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/integrators/_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/__init__.pyi` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/__init__.pyi`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_distant.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_distant_flux.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_hemispherical_distant.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_multi_distant.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_multi_radiancemeter.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_perspective.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/measure/_radiancemeter.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/measure/_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/phase/_blend.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/phase/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/phase/_hg.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_hg.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/phase/_rayleigh.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_rayleigh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/phase/_tabulated.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/phase/_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_buffermesh.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_buffermesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,17 @@
         # Inherit docstring
         raise NotImplementedError
 
     @property
     def instance(self) -> mi.Object:
         if self.bsdf is not None:
             template, _ = traverse(self.bsdf)
-            bsdf = mi.load_dict(template.render(ctx=KernelContext()))
+            kdict = template.render(ctx=KernelContext())
+            kdict["id"] = self._bsdf_id  # TODO: Enforce ID control at BSDF level
+            bsdf = mi.load_dict(kdict)
         else:
             bsdf = None
 
         props = mi.Properties()
         props["mesh_bsdf"] = bsdf
 
         mesh = mi.Mesh(
@@ -90,9 +92,9 @@
         return mesh
 
     @property
     def params(self) -> dict[str, UpdateParameter] | None:
         if self.bsdf is None:
             return None
 
-        _, params = traverse(self.bsdf)
+        _, params = traverse(attrs.evolve(self.bsdf, id=self._bsdf_id))
         return {f"bsdf.{k}": v for k, v in params.items()}
```

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_cuboid.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_cuboid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_filemesh.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_rectangle.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/shapes/_sphere.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/shapes/_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_air_scattering_coefficient.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_interpolated.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_multi_delta.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_multi_delta.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_solar_irradiance.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/spectra/_uniform.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/spectra/_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/surface/_basic.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/surface/_central_patch.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/surface/_core.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/scenes/surface/_dem.py` & `eradiate-0.23.2rc1/src/eradiate/scenes/surface/_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/spectral/ckd.py` & `eradiate-0.23.2rc1/src/eradiate/spectral/ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/spectral/index.py` & `eradiate-0.23.2rc1/src/eradiate/spectral/index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/spectral/mono.py` & `eradiate-0.23.2rc1/src/eradiate/spectral/mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/srf_tools.py` & `eradiate-0.23.2rc1/src/eradiate/srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/test_tools/plugin.py` & `eradiate-0.23.2rc1/src/eradiate/test_tools/plugin.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/test_tools/regression.py` & `eradiate-0.23.2rc1/src/eradiate/test_tools/regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/test_tools/types.py` & `eradiate-0.23.2rc1/src/eradiate/test_tools/types.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/test_tools/util.py` & `eradiate-0.23.2rc1/src/eradiate/test_tools/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/thermoprops/afgl_1986.py` & `eradiate-0.23.2rc1/src/eradiate/thermoprops/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/thermoprops/us76.py` & `eradiate-0.23.2rc1/src/eradiate/thermoprops/us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/thermoprops/util.py` & `eradiate-0.23.2rc1/src/eradiate/thermoprops/util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/units.py` & `eradiate-0.23.2rc1/src/eradiate/units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/util/deprecation.py` & `eradiate-0.23.2rc1/src/eradiate/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/util/misc.py` & `eradiate-0.23.2rc1/src/eradiate/util/misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/util/numpydoc.py` & `eradiate-0.23.2rc1/src/eradiate/util/numpydoc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/util/sys_info.py` & `eradiate-0.23.2rc1/src/eradiate/util/sys_info.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/validators.py` & `eradiate-0.23.2rc1/src/eradiate/validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/warp.py` & `eradiate-0.23.2rc1/src/eradiate/warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/xarray/_accessors.py` & `eradiate-0.23.2rc1/src/eradiate/xarray/_accessors.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/xarray/_helpers.py` & `eradiate-0.23.2rc1/src/eradiate/xarray/_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate/xarray/interp.py` & `eradiate-0.23.2rc1/src/eradiate/xarray/interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/src/eradiate.egg-info/PKG-INFO` & `eradiate-0.23.2rc1/src/eradiate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eradiate
-Version: 0.23.2rc0
+Version: 0.23.2rc1
 Summary: A radiative transfer model for the Earth observation community
 Author: The Eradiate Team
 Maintainer: The Eradiate Team
 License: LGPLv3
 Project-URL: changelog, https://github.com/eradiate/eradiate/CHANGELOG.md
 Project-URL: documentation, https://eradiate.readthedocs.io
 Project-URL: repository, https://github.com/eradiate/eradiate
```

### Comparing `eradiate-0.23.2rc0/src/eradiate.egg-info/SOURCES.txt` & `eradiate-0.23.2rc1/src/eradiate.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .gitignore
 .gitmodules
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 setpath.sh
 setup.py
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
@@ -164,15 +165,14 @@
 docs/rst/user_guide/data/spectra-us76_u86_4.rst
 docs/rst/user_guide/data/srf.rst
 docs/rst/user_guide/data/fig/p_interp_rerr_histo_65349.png
 docs/rst/user_guide/data/fig/pt_points.png
 docs/rst/user_guide/data/fig/w_interp_rerr_histo_101325.png
 docs/src/CHANGELOG.md
 docs/src/reference_cli.md
-ext/CMakeLists.txt
 requirements/check_conda_env.py
 requirements/copy_envvars.py
 requirements/dev.in
 requirements/dev.txt
 requirements/docs.in
 requirements/docs.txt
 requirements/environment-dev.yml
@@ -191,15 +191,14 @@
 requirements/optional.in
 requirements/optional.txt
 requirements/production.in
 requirements/production.txt
 requirements/recommended.in
 requirements/tests.in
 requirements/tests.txt
-resources/downloads.yml
 src/eradiate/__init__.py
 src/eradiate/__init__.pyi
 src/eradiate/_config.py
 src/eradiate/_factory.py
 src/eradiate/_mode.py
 src/eradiate/_version.py
 src/eradiate/attrs.py
@@ -217,15 +216,14 @@
 src/eradiate/units.py
 src/eradiate/validators.py
 src/eradiate/warp.py
 src/eradiate.egg-info/PKG-INFO
 src/eradiate.egg-info/SOURCES.txt
 src/eradiate.egg-info/dependency_links.txt
 src/eradiate.egg-info/entry_points.txt
-src/eradiate.egg-info/not-zip-safe
 src/eradiate.egg-info/requires.txt
 src/eradiate.egg-info/top_level.txt
 src/eradiate/cli/__init__.py
 src/eradiate/cli/data.py
 src/eradiate/cli/show.py
 src/eradiate/cli/srf.py
 src/eradiate/data/__init__.py
@@ -234,14 +232,16 @@
 src/eradiate/data/_blind_directory.py
 src/eradiate/data/_blind_online.py
 src/eradiate/data/_core.py
 src/eradiate/data/_multi.py
 src/eradiate/data/_safe_directory.py
 src/eradiate/data/_safe_online.py
 src/eradiate/data/_store.py
+src/eradiate/data/downloads.yml
+src/eradiate/data/downloads_development.yml
 src/eradiate/experiments/__init__.py
 src/eradiate/experiments/__init__.pyi
 src/eradiate/experiments/_atmosphere.py
 src/eradiate/experiments/_canopy.py
 src/eradiate/experiments/_canopy_atmosphere.py
 src/eradiate/experiments/_core.py
 src/eradiate/experiments/_dem.py
@@ -371,168 +371,154 @@
 src/eradiate/xarray/__init__.py
 src/eradiate/xarray/__init__.pyi
 src/eradiate/xarray/_accessors.py
 src/eradiate/xarray/_helpers.py
 src/eradiate/xarray/interp.py
 tests/__init__.py
 tests/conftest.py
-tests/01_plugins/__init__.py
-tests/01_plugins/conftest.py
-tests/01_plugins/bsdfs/__init__.py
-tests/01_plugins/bsdfs/test_bilambertian.py
-tests/01_plugins/bsdfs/test_mqdiffuse.py
-tests/01_plugins/bsdfs/test_rpv.py
-tests/01_plugins/phase/test_tabphase_irregular.py
-tests/01_plugins/sensors/__init__.py
-tests/01_plugins/sensors/test_distantflux.py
-tests/01_plugins/sensors/test_hdistant.py
-tests/01_plugins/sensors/test_mdistant.py
-tests/01_plugins/sensors/test_mradiancemeter.py
-tests/01_plugins/volumes/__init__.py
-tests/01_plugins/volumes/test_spherical.py
-tests/02_eradiate/__init__.py
-tests/02_eradiate/conftest.py
-tests/02_eradiate/01_unit/__init__.py
-tests/02_eradiate/01_unit/test_config.py
-tests/02_eradiate/01_unit/test_factory.py
-tests/02_eradiate/01_unit/test_frame.py
-tests/02_eradiate/01_unit/test_mode.py
-tests/02_eradiate/01_unit/test_quad.py
-tests/02_eradiate/01_unit/test_rng.py
-tests/02_eradiate/01_unit/test_srf_tools.py
-tests/02_eradiate/01_unit/test_units.py
-tests/02_eradiate/01_unit/test_validators.py
-tests/02_eradiate/01_unit/test_warp.py
-tests/02_eradiate/01_unit/data/__init__.py
-tests/02_eradiate/01_unit/data/test_blind_directory.py
-tests/02_eradiate/01_unit/data/test_blind_online.py
-tests/02_eradiate/01_unit/data/test_core.py
-tests/02_eradiate/01_unit/data/test_datasets.py
-tests/02_eradiate/01_unit/data/test_multi.py
-tests/02_eradiate/01_unit/data/test_open.py
-tests/02_eradiate/01_unit/data/test_safe_directory.py
-tests/02_eradiate/01_unit/data/test_safe_online.py
-tests/02_eradiate/01_unit/experiments/__init__.py
-tests/02_eradiate/01_unit/experiments/test_atmosphere.py
-tests/02_eradiate/01_unit/experiments/test_canopy.py
-tests/02_eradiate/01_unit/experiments/test_canopy_atmosphere.py
-tests/02_eradiate/01_unit/experiments/test_core.py
-tests/02_eradiate/01_unit/experiments/test_dem.py
-tests/02_eradiate/01_unit/experiments/test_helpers.py
-tests/02_eradiate/01_unit/kernel/__init__.py
-tests/02_eradiate/01_unit/kernel/test_gridvolume.py
-tests/02_eradiate/01_unit/kernel/test_kernel_dict.py
-tests/02_eradiate/01_unit/kernel/test_logging.py
-tests/02_eradiate/01_unit/kernel/test_render.py
-tests/02_eradiate/01_unit/kernel/test_transform.py
-tests/02_eradiate/01_unit/pipelines/__init__.py
-tests/02_eradiate/01_unit/pipelines/conftest.py
-tests/02_eradiate/01_unit/pipelines/test_aggregate.py
-tests/02_eradiate/01_unit/pipelines/test_assemble.py
-tests/02_eradiate/01_unit/pipelines/test_compute.py
-tests/02_eradiate/01_unit/pipelines/test_core.py
-tests/02_eradiate/01_unit/pipelines/test_gather.py
-tests/02_eradiate/01_unit/radprops/__init__.py
-tests/02_eradiate/01_unit/radprops/test_absorption.py
-tests/02_eradiate/01_unit/radprops/test_afgl_1986.py
-tests/02_eradiate/01_unit/radprops/test_rayleigh_scattering.py
-tests/02_eradiate/01_unit/radprops/test_us76_approx.py
-tests/02_eradiate/01_unit/radprops/test_zgrid.py
-tests/02_eradiate/01_unit/scenes/__init__.py
-tests/02_eradiate/01_unit/scenes/test_core.py
-tests/02_eradiate/01_unit/scenes/atmosphere/__init__.py
-tests/02_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
-tests/02_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
-tests/02_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
-tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
-tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
-tests/02_eradiate/01_unit/scenes/biosphere/__init__.py
-tests/02_eradiate/01_unit/scenes/biosphere/test_core.py
-tests/02_eradiate/01_unit/scenes/biosphere/test_discrete.py
-tests/02_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
-tests/02_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
-tests/02_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
-tests/02_eradiate/01_unit/scenes/bsdfs/__init__.py
-tests/02_eradiate/01_unit/scenes/bsdfs/test_black.py
-tests/02_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
-tests/02_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
-tests/02_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
-tests/02_eradiate/01_unit/scenes/bsdfs/test_rpv.py
-tests/02_eradiate/01_unit/scenes/illumination/__init__.py
-tests/02_eradiate/01_unit/scenes/illumination/test_constant.py
-tests/02_eradiate/01_unit/scenes/illumination/test_directional.py
-tests/02_eradiate/01_unit/scenes/illumination/test_spot.py
-tests/02_eradiate/01_unit/scenes/integrators/__init__.py
-tests/02_eradiate/01_unit/scenes/integrators/test_path_tracers.py
-tests/02_eradiate/01_unit/scenes/measure/__init__.py
-tests/02_eradiate/01_unit/scenes/measure/test_distant_flux.py
-tests/02_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
-tests/02_eradiate/01_unit/scenes/measure/test_multi_distant.py
-tests/02_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
-tests/02_eradiate/01_unit/scenes/measure/test_perspective.py
-tests/02_eradiate/01_unit/scenes/measure/test_radiancemeter.py
-tests/02_eradiate/01_unit/scenes/measure/test_target.py
-tests/02_eradiate/01_unit/scenes/phase/__init__.py
-tests/02_eradiate/01_unit/scenes/phase/test_blend.py
-tests/02_eradiate/01_unit/scenes/phase/test_hg.py
-tests/02_eradiate/01_unit/scenes/phase/test_isotropic.py
-tests/02_eradiate/01_unit/scenes/phase/test_rayleigh.py
-tests/02_eradiate/01_unit/scenes/phase/test_tabulated.py
-tests/02_eradiate/01_unit/scenes/shapes/__init__.py
-tests/02_eradiate/01_unit/scenes/shapes/test_buffermesh.py
-tests/02_eradiate/01_unit/scenes/shapes/test_cuboid.py
-tests/02_eradiate/01_unit/scenes/shapes/test_filemesh.py
-tests/02_eradiate/01_unit/scenes/shapes/test_rectangle.py
-tests/02_eradiate/01_unit/scenes/shapes/test_sphere.py
-tests/02_eradiate/01_unit/scenes/spectra/__init__.py
-tests/02_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
-tests/02_eradiate/01_unit/scenes/spectra/test_core.py
-tests/02_eradiate/01_unit/scenes/spectra/test_interpolated.py
-tests/02_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
-tests/02_eradiate/01_unit/scenes/spectra/test_uniform.py
-tests/02_eradiate/01_unit/scenes/surface/__init__.py
-tests/02_eradiate/01_unit/scenes/surface/test_basic.py
-tests/02_eradiate/01_unit/scenes/surface/test_central_patch.py
-tests/02_eradiate/01_unit/scenes/surface/test_dem.py
-tests/02_eradiate/01_unit/spectral/test_ckd.py
-tests/02_eradiate/01_unit/spectral/test_index.py
-tests/02_eradiate/01_unit/spectral/test_mono.py
-tests/02_eradiate/01_unit/test_tools/__init__.py
-tests/02_eradiate/01_unit/test_tools/test_regression.py
-tests/02_eradiate/01_unit/thermoprops/__init__.py
-tests/02_eradiate/01_unit/thermoprops/test_afgl1986.py
-tests/02_eradiate/01_unit/thermoprops/test_us76.py
-tests/02_eradiate/01_unit/thermoprops/test_util.py
-tests/02_eradiate/01_unit/util/__init__.py
-tests/02_eradiate/01_unit/util/test_deprecation.py
-tests/02_eradiate/01_unit/util/test_misc.py
-tests/02_eradiate/01_unit/xarray/conftest.py
-tests/02_eradiate/01_unit/xarray/test_interp.py
-tests/02_eradiate/02_system/__init__.py
-tests/02_eradiate/02_system/conftest.py
-tests/02_eradiate/02_system/test_albedo.py
-tests/02_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
-tests/02_eradiate/02_system/test_atmosphere_rpv.py
-tests/02_eradiate/02_system/test_basic.py
-tests/02_eradiate/02_system/test_ckd_basic.py
-tests/02_eradiate/02_system/test_compare_canopy_atmosphere.py
-tests/02_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
-tests/02_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
-tests/02_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
-tests/02_eradiate/02_system/test_irradiance_scaling.py
-tests/02_eradiate/02_system/test_kernel_render_benchmark.py
-tests/02_eradiate/02_system/test_maximum_scene_size.py
-tests/02_eradiate/02_system/test_mdistant_insitu.py
-tests/02_eradiate/02_system/test_onedim_lambertian_brf.py
-tests/02_eradiate/02_system/test_onedim_phase.py
-tests/02_eradiate/02_system/test_onedim_symmetry.py
-tests/02_eradiate/02_system/test_spectral_loop.py
-tests/02_eradiate/03_regression/__init__.py
-tests/02_eradiate/03_regression/atmospheres/__init__.py
-tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
-tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
-tests/02_eradiate/03_regression/rami4atm/__init__.py
-tests/02_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
-tests/02_eradiate/03_regression/romc/__init__.py
-tests/02_eradiate/03_regression/romc/test_het01.py
-tests/02_eradiate/03_regression/romc/test_het04.py
-tests/02_eradiate/03_regression/romc/test_het06.py
+tests/01_eradiate/__init__.py
+tests/01_eradiate/conftest.py
+tests/01_eradiate/01_unit/__init__.py
+tests/01_eradiate/01_unit/test_config.py
+tests/01_eradiate/01_unit/test_factory.py
+tests/01_eradiate/01_unit/test_frame.py
+tests/01_eradiate/01_unit/test_mode.py
+tests/01_eradiate/01_unit/test_quad.py
+tests/01_eradiate/01_unit/test_rng.py
+tests/01_eradiate/01_unit/test_srf_tools.py
+tests/01_eradiate/01_unit/test_units.py
+tests/01_eradiate/01_unit/test_validators.py
+tests/01_eradiate/01_unit/test_warp.py
+tests/01_eradiate/01_unit/data/__init__.py
+tests/01_eradiate/01_unit/data/test_blind_directory.py
+tests/01_eradiate/01_unit/data/test_blind_online.py
+tests/01_eradiate/01_unit/data/test_core.py
+tests/01_eradiate/01_unit/data/test_datasets.py
+tests/01_eradiate/01_unit/data/test_multi.py
+tests/01_eradiate/01_unit/data/test_open.py
+tests/01_eradiate/01_unit/data/test_safe_directory.py
+tests/01_eradiate/01_unit/data/test_safe_online.py
+tests/01_eradiate/01_unit/experiments/__init__.py
+tests/01_eradiate/01_unit/experiments/test_atmosphere.py
+tests/01_eradiate/01_unit/experiments/test_canopy.py
+tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py
+tests/01_eradiate/01_unit/experiments/test_core.py
+tests/01_eradiate/01_unit/experiments/test_dem.py
+tests/01_eradiate/01_unit/experiments/test_helpers.py
+tests/01_eradiate/01_unit/kernel/__init__.py
+tests/01_eradiate/01_unit/kernel/test_gridvolume.py
+tests/01_eradiate/01_unit/kernel/test_kernel_dict.py
+tests/01_eradiate/01_unit/kernel/test_logging.py
+tests/01_eradiate/01_unit/kernel/test_render.py
+tests/01_eradiate/01_unit/kernel/test_transform.py
+tests/01_eradiate/01_unit/pipelines/__init__.py
+tests/01_eradiate/01_unit/pipelines/conftest.py
+tests/01_eradiate/01_unit/pipelines/test_aggregate.py
+tests/01_eradiate/01_unit/pipelines/test_assemble.py
+tests/01_eradiate/01_unit/pipelines/test_compute.py
+tests/01_eradiate/01_unit/pipelines/test_core.py
+tests/01_eradiate/01_unit/pipelines/test_gather.py
+tests/01_eradiate/01_unit/radprops/__init__.py
+tests/01_eradiate/01_unit/radprops/test_absorption.py
+tests/01_eradiate/01_unit/radprops/test_afgl_1986.py
+tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py
+tests/01_eradiate/01_unit/radprops/test_us76_approx.py
+tests/01_eradiate/01_unit/radprops/test_zgrid.py
+tests/01_eradiate/01_unit/scenes/__init__.py
+tests/01_eradiate/01_unit/scenes/test_core.py
+tests/01_eradiate/01_unit/scenes/atmosphere/__init__.py
+tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py
+tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py
+tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py
+tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py
+tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py
+tests/01_eradiate/01_unit/scenes/biosphere/__init__.py
+tests/01_eradiate/01_unit/scenes/biosphere/test_core.py
+tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py
+tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py
+tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py
+tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py
+tests/01_eradiate/01_unit/scenes/bsdfs/__init__.py
+tests/01_eradiate/01_unit/scenes/bsdfs/test_black.py
+tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py
+tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py
+tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py
+tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py
+tests/01_eradiate/01_unit/scenes/illumination/__init__.py
+tests/01_eradiate/01_unit/scenes/illumination/test_constant.py
+tests/01_eradiate/01_unit/scenes/illumination/test_directional.py
+tests/01_eradiate/01_unit/scenes/illumination/test_spot.py
+tests/01_eradiate/01_unit/scenes/integrators/__init__.py
+tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py
+tests/01_eradiate/01_unit/scenes/measure/__init__.py
+tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py
+tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py
+tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py
+tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py
+tests/01_eradiate/01_unit/scenes/measure/test_perspective.py
+tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py
+tests/01_eradiate/01_unit/scenes/measure/test_target.py
+tests/01_eradiate/01_unit/scenes/phase/__init__.py
+tests/01_eradiate/01_unit/scenes/phase/test_blend.py
+tests/01_eradiate/01_unit/scenes/phase/test_hg.py
+tests/01_eradiate/01_unit/scenes/phase/test_isotropic.py
+tests/01_eradiate/01_unit/scenes/phase/test_rayleigh.py
+tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py
+tests/01_eradiate/01_unit/scenes/shapes/__init__.py
+tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py
+tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py
+tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py
+tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py
+tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py
+tests/01_eradiate/01_unit/scenes/spectra/__init__.py
+tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py
+tests/01_eradiate/01_unit/scenes/spectra/test_core.py
+tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py
+tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py
+tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py
+tests/01_eradiate/01_unit/scenes/surface/__init__.py
+tests/01_eradiate/01_unit/scenes/surface/test_basic.py
+tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py
+tests/01_eradiate/01_unit/scenes/surface/test_dem.py
+tests/01_eradiate/01_unit/spectral/test_ckd.py
+tests/01_eradiate/01_unit/spectral/test_index.py
+tests/01_eradiate/01_unit/spectral/test_mono.py
+tests/01_eradiate/01_unit/test_tools/__init__.py
+tests/01_eradiate/01_unit/test_tools/test_regression.py
+tests/01_eradiate/01_unit/thermoprops/__init__.py
+tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py
+tests/01_eradiate/01_unit/thermoprops/test_us76.py
+tests/01_eradiate/01_unit/thermoprops/test_util.py
+tests/01_eradiate/01_unit/util/__init__.py
+tests/01_eradiate/01_unit/util/test_deprecation.py
+tests/01_eradiate/01_unit/util/test_misc.py
+tests/01_eradiate/01_unit/xarray/conftest.py
+tests/01_eradiate/01_unit/xarray/test_interp.py
+tests/01_eradiate/02_system/__init__.py
+tests/01_eradiate/02_system/conftest.py
+tests/01_eradiate/02_system/test_albedo.py
+tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py
+tests/01_eradiate/02_system/test_atmosphere_rpv.py
+tests/01_eradiate/02_system/test_basic.py
+tests/01_eradiate/02_system/test_ckd_basic.py
+tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py
+tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py
+tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py
+tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py
+tests/01_eradiate/02_system/test_irradiance_scaling.py
+tests/01_eradiate/02_system/test_kernel_render_benchmark.py
+tests/01_eradiate/02_system/test_maximum_scene_size.py
+tests/01_eradiate/02_system/test_mdistant_insitu.py
+tests/01_eradiate/02_system/test_onedim_lambertian_brf.py
+tests/01_eradiate/02_system/test_onedim_phase.py
+tests/01_eradiate/02_system/test_onedim_symmetry.py
+tests/01_eradiate/02_system/test_spectral_loop.py
+tests/01_eradiate/03_regression/__init__.py
+tests/01_eradiate/03_regression/atmospheres/__init__.py
+tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py
+tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py
+tests/01_eradiate/03_regression/rami4atm/__init__.py
+tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py
+tests/01_eradiate/03_regression/romc/__init__.py
+tests/01_eradiate/03_regression/romc/test_het01.py
+tests/01_eradiate/03_regression/romc/test_het04.py
+tests/01_eradiate/03_regression/romc/test_het06.py
```

### Comparing `eradiate-0.23.2rc0/src/eradiate.egg-info/requires.txt` & `eradiate-0.23.2rc1/src/eradiate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/01_plugins/bsdfs/test_bilambertian.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_cuboid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,92 @@
 import drjit as dr
 import mitsuba as mi
+import numpy as np
 import pytest
 
+from eradiate import KernelContext
+from eradiate import unit_context_config as ucc
+from eradiate import unit_context_kernel as uck
+from eradiate import unit_registry as ureg
+from eradiate.scenes.core import traverse
+from eradiate.scenes.shapes import CuboidShape
+from eradiate.test_tools.types import check_scene_element
 
-def test_instantiation(variant_scalar_rgb):
-    b = mi.load_dict({"type": "bilambertian"})
-    assert b is not None
-    assert b.component_count() == 2
-    expected_flags_reflection = (
-        mi.BSDFFlags.DiffuseReflection | mi.BSDFFlags.FrontSide | mi.BSDFFlags.BackSide
-    )
-    expected_flags_transmission = (
-        mi.BSDFFlags.DiffuseTransmission
-        | mi.BSDFFlags.FrontSide
-        | mi.BSDFFlags.BackSide
-    )
-    assert expected_flags_reflection == b.flags(0)
-    assert expected_flags_transmission == b.flags(1)
 
-
-@pytest.mark.parametrize(
-    "r, t",
-    [
-        (0.2, 0.4),
-        (0.4, 0.2),
-        (0.1, 0.9),
-        (0.9, 0.1),
-        (0.4, 0.6),
-        (0.6, 0.4),
-    ],
-)
 @pytest.mark.parametrize(
-    "wi",
-    [
-        [0, 0, 1],
-        [1, 1, 1],
-        [0, 0, -1],
-        [1, 1, -1],
-    ],
-    ids=["front", "front_oblique", "back", "back_oblique"],
+    "kwargs, expected_reflectance",
+    [({}, None), ({"bsdf": {"type": "black"}}, 0.0)],
+    ids=["noargs", "args"],
 )
-def test_eval_pdf_vector(variant_llvm_ad_rgb, r, t, wi):
-    def sph_to_dir(theta, phi):
-        """Map spherical to Euclidean coordinates"""
-        st, ct = dr.sincos(theta)
-        sp, cp = dr.sincos(phi)
-        return mi.Vector3f(cp * st, sp * st, ct)
-
-    ctx = mi.BSDFContext()
-    bsdf = mi.load_dict({"type": "bilambertian", "reflectance": r, "transmittance": t})
-
-    si = mi.SurfaceInteraction3f()
-    si.p = [0, 0, 0]
-    si.n = [0, 0, 1]
-    si.wi = dr.normalize(mi.ScalarVector3f(wi))
-    si.sh_frame = mi.Frame3f(si.n)
-
-    # Create grid in spherical coordinates and map it onto the sphere
-    res = 300
-    theta_o, phi_o = dr.meshgrid(
-        dr.linspace(mi.Float, 0, dr.pi, res),
-        dr.linspace(mi.Float, 0, 2 * dr.pi, 2 * res),
-    )
-    wo = sph_to_dir(theta_o, phi_o)
+def test_cuboid_construct_kernel_dict(modes_all, kwargs, expected_reflectance):
+    cuboid = CuboidShape(**kwargs)
 
-    # Evaluate BSDF
-    is_reflect = dr.eq(
-        dr.sign(dr.dot(wo, si.n)),
-        dr.sign(dr.dot(si.wi, si.n)),
-    )
-    v_eval = bsdf.eval(ctx, si, wo=wo)
-    eval_expected = dr.select(
-        is_reflect,
-        r * dr.abs(wo[2]) / dr.pi,
-        t * dr.abs(wo[2]) / dr.pi,
-    )
-    assert dr.allclose(v_eval, eval_expected)
+    mi_wrapper = check_scene_element(cuboid, mi.Shape)
 
-    v_pdf = bsdf.pdf(ctx, si, wo=wo)
-    assert dr.allclose(v_pdf, eval_expected / (r + t))
+    if expected_reflectance is not None:
+        assert mi_wrapper.parameters["bsdf.reflectance.value"] == expected_reflectance
 
 
 @pytest.mark.parametrize(
-    "r, t",
+    "kwargs, expected_transform",
     [
-        [0.6, 0.2],
-        [0.2, 0.6],
-        [0.6, 0.4],
-        [0.4, 0.6],
-        [0.9, 0.1],
-        [0.1, 0.9],
-        [1.0, 0.0],
-        [0.0, 1.0],
-        [0.0, 0.0],
+        (
+            {"edges": [2, 4, 8]},
+            [(-1, -2, -4), (1, 2, 4)],
+        ),
+        (
+            {"edges": [2, 2, 2], "center": [1, 1, 1]},
+            [(0, 0, 0), (2, 2, 2)],
+        ),
     ],
+    ids=["edges", "center"],
 )
-def test_chi2(variant_llvm_ad_rgb, r, t):
-    from mitsuba.python.chi2 import BSDFAdapter, ChiSquareTest, SphericalDomain
-
-    xml = f"""
-        <spectrum name="reflectance" value="{r}"/>
-        <spectrum name="transmittance" value="{t}"/>
-    """
-
-    sample_func, pdf_func = BSDFAdapter("bilambertian", xml)
-
-    chi2 = ChiSquareTest(
-        domain=SphericalDomain(),
-        sample_func=sample_func,
-        pdf_func=pdf_func,
-        sample_dim=3,
+def test_cuboid_params(mode_mono_double, kwargs, expected_transform):
+    # Set edges
+    cuboid = CuboidShape(**kwargs)
+    template, _ = traverse(cuboid)
+    kernel_dict = template.render(ctx=KernelContext())
+    to_world = kernel_dict["to_world"]
+    assert dr.allclose(
+        to_world.transform_affine(mi.Point3f(-1, -1, -1)), expected_transform[0]
+    )
+    assert dr.allclose(
+        to_world.transform_affine(mi.Point3f(1, 1, 1)), expected_transform[1]
     )
 
-    assert chi2.run()
+
+def test_cuboid_atmosphere(mode_mono_double):
+    with ucc.override(length="km"):
+        cuboid = CuboidShape.atmosphere(
+            top=1.0,
+            bottom=0.0,
+            bottom_offset=-0.5,
+            width=1.0,
+        )
+        assert np.allclose(cuboid.edges, [1, 1, 1.5] * ureg.km)
+        assert np.allclose(cuboid.center, [0, 0, 0.25] * ureg.km)
+
+    with uck.override(length="m"):
+        template, _ = traverse(cuboid)
+        kernel_dict = template.render(ctx=KernelContext())
+        bbox = mi.load_dict(kernel_dict).bbox()
+        assert dr.allclose(bbox.min, [-500, -500, -500])
+        assert dr.allclose(bbox.max, [500, 500, 1000])
+
+
+def test_cuboid_contains():
+    cuboid = CuboidShape(center=[0.5, 0.5, 0.5], edges=[1, 1, 1])
+
+    # Works with a single point
+    assert cuboid.contains([0.5, 0.5, 0.5])
+    assert not cuboid.contains([0.5, 0.5, -0.5])
+    assert not cuboid.contains([0.5, 0.5, 0.5] * ureg.km)
+
+    # Works with multiple points
+    assert np.all(cuboid.contains([[0.5, 0.5, 0.5], [0.5, -0.5, 0.5]]) == [True, False])
+
+
+def test_cuboid_bbox():
+    cuboid = CuboidShape(center=[0.5, 0.5, 0.5], edges=[1, 1, 1])
+    bbox = cuboid.bbox
+    np.testing.assert_array_equal(bbox.min.m_as(ureg.m), [0, 0, 0])
+    np.testing.assert_array_equal(bbox.max.m_as(ureg.m), [1, 1, 1])
```

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_blind_directory.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_blind_online.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_blind_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_datasets.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_multi.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_multi.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_safe_directory.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_directory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/data/test_safe_online.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/data/test_safe_online.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_atmosphere.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_atmosphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Extra objects can be added to the scene.
     """
     exp = AtmosphereExperiment(
         extra_objects={
             "reference_surface": {
                 "factory": "shape",
                 "type": "rectangle",
+                "id": "reference_surface",
                 "bsdf": {"type": "lambertian"},
             }
         }
     )
     assert isinstance(exp.extra_objects["reference_surface"], RectangleShape)
     mi_wrapper = check_scene_element(exp.scene, mi.Scene, ctx=exp.context_init)
     assert mi_wrapper.obj.shapes()[0].id() == "reference_surface"
```

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_canopy.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_canopy_atmosphere.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_dem.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/experiments/test_helpers.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/experiments/test_helpers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_gridvolume.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_gridvolume.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_kernel_dict.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_kernel_dict.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_logging.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_logging.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_render.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_render.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/kernel/test_transform.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/kernel/test_transform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/conftest.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_aggregate.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_assemble.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_assemble.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_compute.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_compute.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/pipelines/test_gather.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/pipelines/test_gather.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_absorption.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_absorption.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_afgl_1986.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_rayleigh_scattering.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_rayleigh_scattering.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_us76_approx.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_us76_approx.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/radprops/test_zgrid.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/radprops/test_zgrid.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_heterogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_homogeneous.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_molecular_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_dist.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/atmosphere/test_particle_layer.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_discrete.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_discrete.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_leaf_cloud.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_abstract.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/biosphere/test_tree_mesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_checkerboard.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_lambertian.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_lambertian.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_mqdiffuse.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/bsdfs/test_rpv.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/bsdfs/test_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_constant.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_constant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_directional.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_directional.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/illumination/test_spot.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/illumination/test_spot.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/integrators/test_path_tracers.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/integrators/test_path_tracers.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_distant_flux.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_distant_flux.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_hemispherical_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_multi_distant.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_distant.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_multi_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_perspective.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_perspective.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_radiancemeter.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_radiancemeter.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/measure/test_target.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/measure/test_target.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_blend.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_blend.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/phase/test_tabulated.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/phase/test_tabulated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_buffermesh.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_buffermesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_filemesh.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_filemesh.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_rectangle.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/shapes/test_sphere.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/shapes/test_sphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_air_scattering_coefficient.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_interpolated.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_interpolated.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_solar_irradiance.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/spectra/test_uniform.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/spectra/test_uniform.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_basic.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_central_patch.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_central_patch.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/surface/test_dem.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/surface/test_dem.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/scenes/test_core.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/scenes/test_core.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_ckd.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_ckd.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_index.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_index.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/spectral/test_mono.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/spectral/test_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_config.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,75 @@
 from pathlib import Path
 
 import pytest
 from environ.exceptions import ConfigError, MissingEnvValueError
+from importlib.metadata import PackageNotFoundError, version
 
 from eradiate._config import EradiateConfig, ProgressLevel
 from eradiate.exceptions import ConfigWarning
+from environ.exceptions import ConfigError
 
 
-def test_config(tmpdir):
+def eradiate_mitsuba_status(expect_installed=False):
+
+    """
+    Check if eradiate-mitsuba is installed in order to skip tests depending
+    on the setup type (production or development).
+    """
+
+    try:
+        version("eradiate-mitsuba")
+        return expect_installed
+    except PackageNotFoundError:
+        return not expect_installed
+
+
+@pytest.mark.skipif(eradiate_mitsuba_status(True), reason='This is a production environment: eradiate-mitsuba is installed')
+def test_development_config(tmpdir):
     # Create an appropriate file tree for tests
     tmpdir_path = Path(tmpdir)
     (tmpdir_path / "eradiate/src/eradiate").mkdir(parents=True)
     (tmpdir_path / "eradiate/src/eradiate/__init__.py").touch()
 
-    # Raises if ERADIATE_SOURCE_DIR is missing
-    with pytest.raises(MissingEnvValueError):
+    # Raises if ERADIATE_SOURCE_DIR and eradiate_mitsuba are missing
+    with pytest.raises(ConfigError):
         EradiateConfig.from_environ({})
 
     # When ERADIATE_SOURCE_DIR points to a correct path
     # (i.e. contains eradiate.__init__.py), config init succeeds
     assert EradiateConfig.from_environ(
         {"ERADIATE_SOURCE_DIR": tmpdir_path / "eradiate"}
     )
 
     # Otherwise it raises
     with pytest.raises(ConfigError):
         EradiateConfig.from_environ({"ERADIATE_SOURCE_DIR": tmpdir_path})
 
 
+
+@pytest.mark.skipif(eradiate_mitsuba_status(), reason='This is not a production environment: eradiate-mitsuba is not installed')
+def test_production_config():
+    # Create an appropriate file tree for tests
+    tmpdir_path = Path(tmpdir)
+    (tmpdir_path / "eradiate/src/eradiate").mkdir(parents=True)
+    (tmpdir_path / "eradiate/src/eradiate/__init__.py").touch()
+
+
+    # Should not fail, should detect eradiate-mitsuba instead
+    config = EradiateConfig.from_environ({})
+    assert config.source_dir is None
+
+    # When ERADIATE_SOURCE_DIR points to a correct path
+    # (i.e. contains eradiate.__init__.py), config init succeeds
+    # This mixed setup is supported, but should give precedence to ???
+    assert EradiateConfig.from_environ(
+        {"ERADIATE_SOURCE_DIR": tmpdir_path / "eradiate"}
+    )
+
+
 def test_config_progress():
     cfg = EradiateConfig.from_environ()
 
     # We can set progress level using a level
     cfg.progress = ProgressLevel.NONE
     assert cfg.progress is ProgressLevel.NONE
```

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_factory.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_frame.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_mode.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_mode.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_quad.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_quad.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_rng.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_rng.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_srf_tools.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_srf_tools.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_tools/test_regression.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_tools/test_regression.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_units.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_units.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_validators.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_validators.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/test_warp.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/test_warp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_afgl1986.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_us76.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_us76.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/thermoprops/test_util.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/thermoprops/test_util.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/test_deprecation.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/util/test_misc.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/util/test_misc.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/xarray/conftest.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/01_unit/xarray/test_interp.py` & `eradiate-0.23.2rc1/tests/01_eradiate/01_unit/xarray/test_interp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/conftest.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_albedo.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_albedo.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_atmosphere_ckd_vs_mono.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_ckd_vs_mono.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_atmosphere_rpv.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_atmosphere_rpv.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_basic.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_ckd_basic.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_ckd_basic.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_compare_canopy_atmosphere.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_compare_canopy_atmosphere.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_expansion.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_flags.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_flags.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_heterogeneous_atmosphere_parameter_id_lookup.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_irradiance_scaling.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_irradiance_scaling.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_kernel_render_benchmark.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_kernel_render_benchmark.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_maximum_scene_size.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_maximum_scene_size.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_mdistant_insitu.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_mdistant_insitu.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_lambertian_brf.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_lambertian_brf.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_phase.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_phase.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_onedim_symmetry.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_onedim_symmetry.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/02_system/test_spectral_loop.py` & `eradiate-0.23.2rc1/tests/01_eradiate/02_system/test_spectral_loop.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/atmospheres/test_rpv_afgl1986_continental.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/rami4atm/test_rami4atm_hom00_bla_sd2s_m03_z30a000_brfpp.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het01.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het01.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het04.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het04.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/03_regression/romc/test_het06.py` & `eradiate-0.23.2rc1/tests/01_eradiate/03_regression/romc/test_het06.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/02_eradiate/conftest.py` & `eradiate-0.23.2rc1/tests/01_eradiate/conftest.py`

 * *Files identical despite different names*

### Comparing `eradiate-0.23.2rc0/tests/conftest.py` & `eradiate-0.23.2rc1/tests/conftest.py`

 * *Files identical despite different names*

