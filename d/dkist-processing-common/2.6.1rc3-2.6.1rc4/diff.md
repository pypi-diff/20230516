# Comparing `tmp/dkist-processing-common-2.6.1rc3.tar.gz` & `tmp/dkist-processing-common-2.6.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.6.1rc3.tar", last modified: Tue May  9 22:03:30 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.6.1rc4.tar", last modified: Tue May 16 19:56:45 2023, max compression
```

## Comparing `dkist-processing-common-2.6.1rc3.tar` & `dkist-processing-common-2.6.1rc4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13093 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.916435 dkist-processing-common-2.6.1rc3/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/changelog/137.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.920435 dkist-processing-common-2.6.1rc3/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.920435 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.920435 dkist-processing-common-2.6.1rc3/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.920435 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.924435 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.924435 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.924435 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.924435 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8367 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10502 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.920435 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-09 22:03:30.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4211 2023-05-09 22:03:30.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 22:03:30.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-09 22:03:30.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-09 22:03:30.000000 dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-09 22:03:30.928435 dkist-processing-common-2.6.1rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-09 22:03:25.000000 dkist-processing-common-2.6.1rc3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13093 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/changelog/137.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.646141 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.646141 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.646141 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.646141 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.642141 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-05-16 19:56:45.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-05-16 19:56:45.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 19:56:45.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-16 19:56:45.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-16 19:56:45.000000 dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-16 19:56:45.650141 dkist-processing-common-2.6.1rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-16 19:56:39.000000 dkist-processing-common-2.6.1rc4/setup.py
```

### Comparing `dkist-processing-common-2.6.1rc3/.gitignore` & `dkist-processing-common-2.6.1rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/.pre-commit-config.yaml` & `dkist-processing-common-2.6.1rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/CHANGELOG.rst` & `dkist-processing-common-2.6.1rc4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/PKG-INFO` & `dkist-processing-common-2.6.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.6.1rc3
+Version: 2.6.1rc4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.6.1rc3/README.rst` & `dkist-processing-common-2.6.1rc4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/bitbucket-pipelines.yml` & `dkist-processing-common-2.6.1rc4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/check_changelog_updated.sh` & `dkist-processing-common-2.6.1rc4/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/manual.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     variance_cadence = "VARIANCE_CADENCE"
     num_dsps_repeats = "NUM_DSPS_REPEATS"
     dark_exposure_times = "DARK_EXPOSURE_TIMES"
 
 
 class ConstantsBase:
     """
-    Aggregate (from the constant flowers flower pot) in a single property on task classes.
+    Aggregate (from the constant buds flower pot) in a single property on task classes.
 
     It also provides some default constants, but is intended to be subclassed by instruments.
 
     To subclass:
 
     1. Create the actual subclass. All you need to do is add more @properties for the constants you want
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/flower_pot.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 from typing import List
 
 
 class FlowerPot:
     """Base class to hold multiple sets (stems) of key, value pairs."""
 
     def __init__(self):
-        self.flowers: List[Stem] = list()
+        self.stems: List[Stem] = list()
 
     def __iter__(self):
-        return self.flowers.__iter__()
+        return self.stems.__iter__()
 
     def __len__(self):
-        return self.flowers.__len__()
+        return self.stems.__len__()
 
     def __getitem__(self, item):
-        return self.flowers.__getitem__(item)
+        return self.stems.__getitem__(item)
 
     def add_dirt(self, key: Hashable, value: Any) -> None:
         """
-        Send key and value through all Flowers.
+        Send key and value through all Stems.
 
         Parameters
         ----------
         key
             The key
         value
             The value
@@ -47,16 +47,16 @@
         Returns
         -------
         None
         """
         if not isinstance(key, Hashable):
             raise TypeError(f"Type of key ({type(key)}) is not hashable")
 
-        for flower in self.flowers:
-            flower.update(key, value)
+        for stem in self.stems:
+            stem.update(key, value)
 
 
 class SpilledDirt:
     """
     A custom class for when a Flower wants the FlowerPot to skip that particular key/value.
 
     Exists because None, False, [], (), etc. etc. are all valid Flower return values
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/message.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,16 @@
         with self.apm_task_step("Tag files"):
             self.tag_petals(tag_pot)
 
     def make_flower_pots(self) -> tuple[FlowerPot, FlowerPot]:
         """Ingest all headers."""
         tag_pot = FlowerPot()
         constant_pot = FlowerPot()
-        tag_pot.flowers += self.tag_flowers
-        constant_pot.flowers += self.constant_buds
+        tag_pot.stems += self.tag_flowers
+        constant_pot.stems += self.constant_buds
 
         for fits_obj in self.input_frames:
             filepath = fits_obj.name
             tag_pot.add_dirt(filepath, fits_obj)
             constant_pot.add_dirt(filepath, fits_obj)
 
         return tag_pot, constant_pot
@@ -149,29 +149,29 @@
         ----------
         constant_pot
             The flower pot to be updated
         Returns
         -------
         None
         """
-        for flower in constant_pot:
-            with self.apm_processing_step(f"Setting value of constant {flower.stem_name}"):
-                logger.info(f"Setting value of constant {flower.stem_name}")
+        for stem in constant_pot:
+            with self.apm_processing_step(f"Setting value of constant {stem.stem_name}"):
+                logger.info(f"Setting value of constant {stem.stem_name}")
                 try:
-                    if flower.bud.value is Thorn:
+                    if stem.bud.value is Thorn:
                         # Must've been a picky bud that passed. We don't want to pick it because it has no value
                         continue
                     # If the value is a set, sort it before storing in redis
-                    if isinstance(flower.bud.value, set):
-                        sorted_value = json.dumps(sorted(flower.bud.value))
-                        self.constants._update({flower.stem_name: sorted_value})
-                        logger.info(f"Value of {flower.stem_name} set to {sorted_value}")
+                    if isinstance(stem.bud.value, set):
+                        sorted_value = json.dumps(sorted(stem.bud.value))
+                        self.constants._update({stem.stem_name: sorted_value})
+                        logger.info(f"Value of {stem.stem_name} set to {sorted_value}")
                     else:
-                        self.constants._update({flower.stem_name: flower.bud.value})
-                        logger.info(f"Value of {flower.stem_name} set to {flower.bud.value}")
+                        self.constants._update({stem.stem_name: stem.bud.value})
+                        logger.info(f"Value of {stem.stem_name} set to {stem.bud.value}")
                 except StopIteration:
                     # There are no petals
                     pass
 
     def tag_petals(self, tag_pot: FlowerPot):
         """
         Apply tags to file paths.
@@ -180,19 +180,19 @@
         ----------
         tag_pot
             The flower pot to be tagged
         Returns
         -------
         None
         """
-        for flower in tag_pot:
-            with self.apm_processing_step(f"Applying {flower.stem_name} tag to files"):
-                logger.info(f"Applying {flower.stem_name} tag to files")
-                for petal in flower.petals:
-                    tag = Tag.format_tag(flower.stem_name, petal.value)
+        for stem in tag_pot:
+            with self.apm_processing_step(f"Applying {stem.stem_name} tag to files"):
+                logger.info(f"Applying {stem.stem_name} tag to files")
+                for petal in stem.petals:
+                    tag = Tag.format_tag(stem.stem_name, petal.value)
                     for path in petal.keys:
                         self.tag(path, tag)
 
 
 class ParseL0InputDataBase(ParseDataBase, ABC):
     """
     Common task to populate pipeline Constants and group files with tags by scanning headers.
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,8 +368,8 @@
     petal = list(bud.petals)
     assert len(petal) == 1
 
     # Because there are 3 observe frames in `basic_header_objs` spaced 1, and 2 seconds apart.
     assert petal[0].value == 0.25
 
 
-# TODO: test new flowers that have been added to parse_l0_input_data
+# TODO: test new stems that have been added to parse_l0_input_data
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_flower_pot.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     return Flower(stem_name="simple_flower")
 
 
 @pytest.fixture()
 def simple_flower_pot(simple_flower):
     flower_pot = FlowerPot()
-    flower_pot.flowers += [simple_flower]
+    flower_pot.stems += [simple_flower]
 
     return flower_pot
 
 
 @pytest.fixture()
 def simple_key_values():
     return {f"thing{i}": i for i in range(5)}
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,35 +226,35 @@
     Given: ParseInputData task with constant and tag Flowers
     When: Constructing constant and tag FlowerPots
     Then: The Flowers associated with the Task are correctly placed in either FlowerPot
     """
 
     tag_pot, constant_pot = parse_inputs_task.make_flower_pots()
 
-    assert len(tag_pot.flowers) == 2
-    assert len(constant_pot.flowers) == 3
-    assert tag_pot.flowers[0].stem_name == StemName.modstate.value
-    assert tag_pot.flowers[1].stem_name == "EMPTY_FLOWER"
-    assert constant_pot.flowers[0].stem_name == BudName.num_modstates.value
-    assert constant_pot.flowers[1].stem_name == "EMPTY_BUD"
-    assert constant_pot.flowers[2].stem_name == "PICKY_BUD"
+    assert len(tag_pot.stems) == 2
+    assert len(constant_pot.stems) == 3
+    assert tag_pot.stems[0].stem_name == StemName.modstate.value
+    assert tag_pot.stems[1].stem_name == "EMPTY_FLOWER"
+    assert constant_pot.stems[0].stem_name == BudName.num_modstates.value
+    assert constant_pot.stems[1].stem_name == "EMPTY_BUD"
+    assert constant_pot.stems[2].stem_name == "PICKY_BUD"
 
 
 def test_subclass_flowers(visp_parse_inputs_task, mocker, max_cs_step_time_sec):
     """
-    Given: ParseInputData child class with custom flowers
+    Given: ParseInputData child class with custom stems
     When: Making the flower pots
-    Then: Both the base and custom flowers are placed in the correct FlowerPots
+    Then: Both the base and custom stems are placed in the correct FlowerPots
     """
     tag_pot, constant_pot = visp_parse_inputs_task.make_flower_pots()
 
-    assert len(tag_pot.flowers) == 1
-    assert len(constant_pot.flowers) == 11
-    assert sorted([f.stem_name for f in tag_pot.flowers]) == sorted([StemName.modstate.value])
-    assert sorted([f.stem_name for f in constant_pot.flowers]) == sorted(
+    assert len(tag_pot.stems) == 1
+    assert len(constant_pot.stems) == 11
+    assert sorted([f.stem_name for f in tag_pot.stems]) == sorted([StemName.modstate.value])
+    assert sorted([f.stem_name for f in constant_pot.stems]) == sorted(
         [
             BudName.instrument.value,
             BudName.num_modstates.value,
             BudName.proposal_id.value,
             BudName.contributing_proposal_ids.value,
             BudName.average_cadence.value,
             BudName.maximum_cadence.value,
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.6.1rc4/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.6.1rc3
+Version: 2.6.1rc4
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.6.1rc4/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/docs/Makefile` & `dkist-processing-common-2.6.1rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/docs/conf.py` & `dkist-processing-common-2.6.1rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/docs/make.bat` & `dkist-processing-common-2.6.1rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/licenses/LICENSE.rst` & `dkist-processing-common-2.6.1rc4/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/pyproject.toml` & `dkist-processing-common-2.6.1rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.6.1rc3/setup.cfg` & `dkist-processing-common-2.6.1rc4/setup.cfg`

 * *Files identical despite different names*

