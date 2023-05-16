# Comparing `tmp/cemba-data-1.6.8.tar.gz` & `tmp/cemba-data-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemba-data-1.6.8.tar", last modified: Thu Nov  3 17:31:08 2022, max compression
+gzip compressed data, was "cemba-data-1.6.9.tar", last modified: Tue May 16 19:52:15 2023, max compression
```

## Comparing `cemba-data-1.6.8.tar` & `cemba-data-1.6.9.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.420819 cemba-data-1.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.392819 cemba-data-1.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-11-03 17:30:52.000000 cemba-data-1.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-11-03 17:30:52.000000 cemba-data-1.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-11-03 17:30:52.000000 cemba-data-1.6.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-03 17:30:52.000000 cemba-data-1.6.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-03 17:30:52.000000 cemba-data-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-11-03 17:30:52.000000 cemba-data-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-03 17:31:08.420819 cemba-data-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-11-03 17:30:52.000000 cemba-data-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/cemba_data/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24378 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    18861 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/_yap_internal_cli_.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/cemba_data/bulk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/cemba_data/bulk/Snakefile_template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/Snakefile_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/Snakefile_template/mc_bulk.Snakefile
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7192 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/atac_bulk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4224 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/mc_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     3702 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/bulk/mct_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18391 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/demultiplex/demultiplex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4547 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/demultiplex/fastq_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)    15660 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/demultiplex/plateinfo_and_samplesheet.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/dmr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/dmr/dmrseq/
--rw-r--r--   0 runner    (1001) docker     (121)   135950 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dmrseq/DMRseq.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6793 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dmrseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/dmr/dss/
--rw-r--r--   0 runner    (1001) docker     (121)    29015 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dss/DSS.MultiGroup.SingleRegionDML.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6515 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dss/DSS.TwoGroup.SingleRegionDML.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dss/MultiGroup.py
--rw-r--r--   0 runner    (1001) docker     (121)     8794 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dss/TwoGroup.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/dmr/dss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/files/
--rw-r--r--   0 runner    (1001) docker     (121)    27539 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/V1_i7_i5_index.tsv
--rw-r--r--   0 runner    (1001) docker     (121)    15413 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/V2_i7_i5_index.tsv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/files/default_config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4579 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_4m.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_m3c.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mc.ini
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mct-nome.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mct.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_nome.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.400819 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/
--rw-r--r--   0 runner    (1001) docker     (121)    23374 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/4m_template.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21968 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/m3c_template.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    23468 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/mc_template.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    22027 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/mapping_summary_template/mct_template.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4875 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/plate_info_template_v1.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4749 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/plate_info_template_v2.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v1.fa
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/files/random_index_v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5616 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.fa
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_1.fa
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_2.fa
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_3.fa
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_4.fa
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_5.fa
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_6.fa
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/sample_sheet_header.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2570 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/sbatch_template_schicluster.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3148 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/files/sbatch_template_yap.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/hisat3n/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/hisat3n/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/config/gcp.md
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/config/hisat-3n-build.sh
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/config/hisat3n_mapping_env.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/config/vm_init.sh
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_general.py
--rw-r--r--   0 runner    (1001) docker     (121)    30275 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_m3c.py
--rw-r--r--   0 runner    (1001) docker     (121)     7836 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_mct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14152 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/m3c.smk
--rw-r--r--   0 runner    (1001) docker     (121)    10073 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc-multi.smk
--rw-r--r--   0 runner    (1001) docker     (121)    10053 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc-multi_sort_input.smk
--rw-r--r--   0 runner    (1001) docker     (121)     7924 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc.smk
--rw-r--r--   0 runner    (1001) docker     (121)    16516 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mct-multi.smk
--rw-r--r--   0 runner    (1001) docker     (121)    13447 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mct.smk
--rw-r--r--   0 runner    (1001) docker     (121)     5738 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/stats_col_names.py
--rw-r--r--   0 runner    (1001) docker     (121)    13794 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/stats_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5268 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/hisat3n/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/mapping/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/
--rw-r--r--   0 runner    (1001) docker     (121)    15552 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/4m.Snakefile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9351 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/m3c.Snakefile
--rw-r--r--   0 runner    (1001) docker     (121)     6301 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/mc.Snakefile
--rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/mct.Snakefile
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/mapping/m3c/
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/m3c/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/mapping/mct/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/mct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5843 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/mct/mct_bismark_bam_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/mct/mct_star_bam_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.404819 cemba-data-1.6.8/cemba_data/mapping/pipelines/
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/pipelines/_4m.py
--rw-r--r--   0 runner    (1001) docker     (121)    14951 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/pipelines/m3c.py
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/pipelines/mc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3569 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/pipelines/mct.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.408819 cemba-data-1.6.8/cemba_data/mapping/stats/
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/_4m.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/m3c.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/mc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/mct.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/plate_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     5179 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8774 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/stats/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/mapping/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    28276 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/qsub.py
--rw-r--r--   0 runner    (1001) docker     (121)    15752 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.408819 cemba-data-1.6.8/cemba_data/snm3C/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/snm3C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/snm3C/prepare_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    14528 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/snm3C/prepare_impute.py
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-11-03 17:30:52.000000 cemba-data-1.6.8/cemba_data/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.396818 cemba-data-1.6.8/cemba_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-03 17:31:08.000000 cemba-data-1.6.8/cemba_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.416819 cemba-data-1.6.8/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    10397 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/Mapping.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  7567692 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/MappingSummary.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    10152 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/PipelineInput.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27407 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/PlateInfoAndSampleSheet.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/TODO_GenerateMCDS.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/TODO_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4656 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/TechBasic.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.416819 cemba-data-1.6.8/doc/archive/
--rw-r--r--   0 runner    (1001) docker     (121)     7554 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/archive/MakeFastqDataframe.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4112 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/demultiplex.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 17:31:08.416819 cemba-data-1.6.8/doc/files/
--rw-r--r--   0 runner    (1001) docker     (121)    98979 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/files/MappingPipeline.png
--rw-r--r--   0 runner    (1001) docker     (121)   207618 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/files/molecularsteps.png
--rw-r--r--   0 runner    (1001) docker     (121)   425565 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/files/primerstructure.png
--rw-r--r--   0 runner    (1001) docker     (121)   238633 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/files/v1barcode.png
--rw-r--r--   0 runner    (1001) docker     (121)   294693 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/files/v2barcode.png
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/installation.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-03 17:30:52.000000 cemba-data-1.6.8/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-03 17:30:52.000000 cemba-data-1.6.8/env.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-11-03 17:30:52.000000 cemba-data-1.6.8/hisat3n_env.yml
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-03 17:30:52.000000 cemba-data-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-03 17:30:52.000000 cemba-data-1.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 17:31:08.420819 cemba-data-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-11-03 17:30:52.000000 cemba-data-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.828202 cemba-data-1.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.800202 cemba-data-1.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.804202 cemba-data-1.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 19:51:58.000000 cemba-data-1.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 19:51:58.000000 cemba-data-1.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-16 19:51:58.000000 cemba-data-1.6.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-16 19:51:58.000000 cemba-data-1.6.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 19:51:58.000000 cemba-data-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 19:51:58.000000 cemba-data-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-16 19:52:15.828202 cemba-data-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-16 19:51:58.000000 cemba-data-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.804202 cemba-data-1.6.9/cemba_data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24378 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/_yap_internal_cli_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/bulk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/bulk/Snakefile_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/Snakefile_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/Snakefile_template/mc_bulk.Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/atac_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/mc_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/bulk/mct_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/demultiplex/demultiplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/demultiplex/fastq_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/demultiplex/plateinfo_and_samplesheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/dmr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/dmr/dmrseq/
+-rw-r--r--   0 runner    (1001) docker     (123)   135950 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dmrseq/DMRseq.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dmrseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/dmr/dss/
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dss/DSS.MultiGroup.SingleRegionDML.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dss/DSS.TwoGroup.SingleRegionDML.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dss/MultiGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dss/TwoGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/dmr/dss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.808202 cemba-data-1.6.9/cemba_data/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    27539 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/V1_i7_i5_index.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    15413 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/V2_i7_i5_index.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.812202 cemba-data-1.6.9/cemba_data/files/default_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_4m.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_m3c.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mc.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mct-nome.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mct.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_nome.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.812202 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    23374 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/4m_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/m3c_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23468 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/mc_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22027 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/mapping_summary_template/mct_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/plate_info_template_v1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/plate_info_template_v2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v1.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.812202 cemba-data-1.6.9/cemba_data/files/random_index_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_1.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_2.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_3.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_4.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_5.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/sample_sheet_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/sbatch_template_schicluster.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/files/sbatch_template_yap.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.812202 cemba-data-1.6.9/cemba_data/hisat3n/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.812202 cemba-data-1.6.9/cemba_data/hisat3n/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/config/gcp.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/config/hisat-3n-build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/config/hisat3n_mapping_env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/config/vm_init.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30423 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_m3c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_mct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/m3c.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc-multi.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc-multi_sort_input.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mct-multi.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mct.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/stats_col_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/stats_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/hisat3n/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/4m.Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/m3c.Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/mc.Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)    11025 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/mct.Snakefile
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/m3c/
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/m3c/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/mct/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/mct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/mct/mct_bismark_bam_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/mct/mct_star_bam_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/pipelines/_4m.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/pipelines/m3c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/pipelines/mc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/pipelines/mct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/mapping/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/_4m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/m3c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/mc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/mct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/plate_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/stats/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/mapping/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/qsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.816202 cemba-data-1.6.9/cemba_data/snm3C/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/snm3C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/snm3C/prepare_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/snm3C/prepare_impute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-16 19:51:58.000000 cemba-data-1.6.9/cemba_data/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.804202 cemba-data-1.6.9/cemba_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 19:52:15.000000 cemba-data-1.6.9/cemba_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.828202 cemba-data-1.6.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/Mapping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  7567692 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/MappingSummary.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/PipelineInput.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27407 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/PlateInfoAndSampleSheet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/TODO_GenerateMCDS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/TODO_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/TechBasic.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.828202 cemba-data-1.6.9/doc/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/archive/MakeFastqDataframe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/demultiplex.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:52:15.828202 cemba-data-1.6.9/doc/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    98979 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/files/MappingPipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   207618 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/files/molecularsteps.png
+-rw-r--r--   0 runner    (1001) docker     (123)   425565 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/files/primerstructure.png
+-rw-r--r--   0 runner    (1001) docker     (123)   238633 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/files/v1barcode.png
+-rw-r--r--   0 runner    (1001) docker     (123)   294693 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/files/v2barcode.png
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/installation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-16 19:51:58.000000 cemba-data-1.6.9/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 19:51:58.000000 cemba-data-1.6.9/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 19:51:58.000000 cemba-data-1.6.9/hisat3n_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 19:51:58.000000 cemba-data-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 19:51:58.000000 cemba-data-1.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:52:15.828202 cemba-data-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-16 19:51:58.000000 cemba-data-1.6.9/setup.py
```

### Comparing `cemba-data-1.6.8/.github/workflows/publish.yaml` & `cemba-data-1.6.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/.gitignore` & `cemba-data-1.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/.travis.yml` & `cemba-data-1.6.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/Dockerfile` & `cemba-data-1.6.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/LICENSE` & `cemba-data-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/PKG-INFO` & `cemba-data-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemba-data
-Version: 1.6.8
+Version: 1.6.9
 Summary: Pipelines for single nucleus methylome and multi-omic dataset.
 Home-page: https://github.com/lhqing/cemba_data
 Author: Hanqing Liu
 Author-email: hanliu@salk.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cemba-data-1.6.8/README.md` & `cemba-data-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/__main__.py` & `cemba-data-1.6.9/cemba_data/__main__.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/_yap_internal_cli_.py` & `cemba-data-1.6.9/cemba_data/_yap_internal_cli_.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/Snakefile_template/mc_bulk.Snakefile` & `cemba-data-1.6.9/cemba_data/bulk/Snakefile_template/mc_bulk.Snakefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/atac_bulk.py` & `cemba-data-1.6.9/cemba_data/bulk/atac_bulk.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/mc_bulk.py` & `cemba-data-1.6.9/cemba_data/bulk/mc_bulk.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup.py` & `cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup_template.py` & `cemba-data-1.6.9/cemba_data/bulk/mc_bulk_multigroup/mc_bulk_multigroup_template.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/bulk/mct_bulk.py` & `cemba-data-1.6.9/cemba_data/bulk/mct_bulk.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/demultiplex/demultiplex.py` & `cemba-data-1.6.9/cemba_data/demultiplex/demultiplex.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/demultiplex/fastq_dataframe.py` & `cemba-data-1.6.9/cemba_data/demultiplex/fastq_dataframe.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/demultiplex/plateinfo_and_samplesheet.py` & `cemba-data-1.6.9/cemba_data/demultiplex/plateinfo_and_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dmrseq/DMRseq.ipynb` & `cemba-data-1.6.9/cemba_data/dmr/dmrseq/DMRseq.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dmrseq/__init__.py` & `cemba-data-1.6.9/cemba_data/dmr/dmrseq/__init__.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dss/DSS.MultiGroup.SingleRegionDML.ipynb` & `cemba-data-1.6.9/cemba_data/dmr/dss/DSS.MultiGroup.SingleRegionDML.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dss/DSS.TwoGroup.SingleRegionDML.ipynb` & `cemba-data-1.6.9/cemba_data/dmr/dss/DSS.TwoGroup.SingleRegionDML.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dss/MultiGroup.py` & `cemba-data-1.6.9/cemba_data/dmr/dss/MultiGroup.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/dmr/dss/TwoGroup.py` & `cemba-data-1.6.9/cemba_data/dmr/dss/TwoGroup.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/V1_i7_i5_index.tsv` & `cemba-data-1.6.9/cemba_data/files/V1_i7_i5_index.tsv`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/V2_i7_i5_index.tsv` & `cemba-data-1.6.9/cemba_data/files/V2_i7_i5_index.tsv`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_4m.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_4m.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_m3c.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_m3c.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mc.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mc.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mct-nome.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mct-nome.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_mct.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_mct.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/default_config/mapping_config_nome.ini` & `cemba-data-1.6.9/cemba_data/files/default_config/mapping_config_nome.ini`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/mapping_summary_template/4m_template.ipynb` & `cemba-data-1.6.9/cemba_data/files/mapping_summary_template/4m_template.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/mapping_summary_template/m3c_template.ipynb` & `cemba-data-1.6.9/cemba_data/files/mapping_summary_template/m3c_template.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/mapping_summary_template/mc_template.ipynb` & `cemba-data-1.6.9/cemba_data/files/mapping_summary_template/mc_template.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/mapping_summary_template/mct_template.ipynb` & `cemba-data-1.6.9/cemba_data/files/mapping_summary_template/mct_template.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/plate_info_template_v1.txt` & `cemba-data-1.6.9/cemba_data/files/plate_info_template_v1.txt`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/plate_info_template_v2.txt` & `cemba-data-1.6.9/cemba_data/files/plate_info_template_v2.txt`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_1.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_1.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_2.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_2.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_3.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_3.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_4.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_4.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_5.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_5.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_6.fa` & `cemba-data-1.6.9/cemba_data/files/random_index_v2/random_index_v2.multiplex_group_6.fa`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/sbatch_template_schicluster.txt` & `cemba-data-1.6.9/cemba_data/files/sbatch_template_schicluster.txt`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/files/sbatch_template_yap.txt` & `cemba-data-1.6.9/cemba_data/files/sbatch_template_yap.txt`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/config/gcp.md` & `cemba-data-1.6.9/cemba_data/hisat3n/config/gcp.md`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_general.py` & `cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_general.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_m3c.py` & `cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_m3c.py`

 * *Files 1% similar despite different names*

```diff
@@ -631,22 +631,26 @@
     contacts = contacts.sort_values(
         by=['chrom1', 'chrom2', 'start1', 'start2', 'end1', 'end2'])
     input_contacts = contacts.shape[0]
 
     total_dedup = []
     for _, chrom_df in contacts.groupby(['chrom1', 'chrom2']):
         total_dedup.append(_dedup_chrom_df(chrom_df))
-    total_dedup = pd.concat(total_dedup)
+    try:
+        total_dedup = pd.concat(total_dedup)
+    except ValueError:
+        # no dataframes in total_dedup
+        total_dedup = pd.DataFrame(columns=contacts.columns)
     total_dedup.to_csv(output_path, sep='\t', index=False)
 
     if not save_raw:
         subprocess.run(shlex.split(f'rm -f {input_path}'), check=True)
 
     dedup_contacts = total_dedup.shape[0]
-    dup_rate = (input_contacts - dedup_contacts) / input_contacts
+    dup_rate = (input_contacts - dedup_contacts) / (input_contacts + 0.00001)
     return dedup_contacts, dup_rate
 
 
 def _contact_to_hic_format(output_prefix):
     contact_df = pd.read_csv(f'{output_prefix}.dedup_contacts.tsv.gz', sep='\t')
     # some columns used in hic format
     contact_df['hic0'] = 0
```

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/hisat3n_mct.py` & `cemba-data-1.6.9/cemba_data/hisat3n/hisat3n_mct.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/m3c.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/m3c.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc-multi.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc-multi.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc-multi_sort_input.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc-multi_sort_input.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mc.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mc.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mct-multi.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mct-multi.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/snakefile/mct.smk` & `cemba-data-1.6.9/cemba_data/hisat3n/snakefile/mct.smk`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/stats_col_names.py` & `cemba-data-1.6.9/cemba_data/hisat3n/stats_col_names.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/stats_parser.py` & `cemba-data-1.6.9/cemba_data/hisat3n/stats_parser.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/summary.py` & `cemba-data-1.6.9/cemba_data/hisat3n/summary.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/hisat3n/utilities.py` & `cemba-data-1.6.9/cemba_data/hisat3n/utilities.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/4m.Snakefile` & `cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/4m.Snakefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/m3c.Snakefile` & `cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/m3c.Snakefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/mc.Snakefile` & `cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/mc.Snakefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/Snakefile_template/mct.Snakefile` & `cemba-data-1.6.9/cemba_data/mapping/Snakefile_template/mct.Snakefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/config.py` & `cemba-data-1.6.9/cemba_data/mapping/config.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/m3c/__init__.py` & `cemba-data-1.6.9/cemba_data/mapping/m3c/__init__.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/mct/mct_bismark_bam_filter.py` & `cemba-data-1.6.9/cemba_data/mapping/mct/mct_bismark_bam_filter.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/mct/mct_star_bam_filter.py` & `cemba-data-1.6.9/cemba_data/mapping/mct/mct_star_bam_filter.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/pipelines/_4m.py` & `cemba-data-1.6.9/cemba_data/mapping/pipelines/_4m.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/pipelines/__init__.py` & `cemba-data-1.6.9/cemba_data/mapping/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/pipelines/m3c.py` & `cemba-data-1.6.9/cemba_data/mapping/pipelines/m3c.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/pipelines/mc.py` & `cemba-data-1.6.9/cemba_data/mapping/pipelines/mc.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/pipelines/mct.py` & `cemba-data-1.6.9/cemba_data/mapping/pipelines/mct.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/_4m.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/_4m.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/__init__.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/m3c.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/m3c.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/mc.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/mc.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/mct.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/mct.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/plate_info.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/plate_info.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/plot.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/plot.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/stats/utilities.py` & `cemba-data-1.6.9/cemba_data/mapping/stats/utilities.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/mapping/test_environment.py` & `cemba-data-1.6.9/cemba_data/mapping/test_environment.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/qsub.py` & `cemba-data-1.6.9/cemba_data/qsub.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/sbatch.py` & `cemba-data-1.6.9/cemba_data/sbatch.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/snm3C/prepare_dataset.py` & `cemba-data-1.6.9/cemba_data/snm3C/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/snm3C/prepare_impute.py` & `cemba-data-1.6.9/cemba_data/snm3C/prepare_impute.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data/utilities.py` & `cemba-data-1.6.9/cemba_data/utilities.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/cemba_data.egg-info/PKG-INFO` & `cemba-data-1.6.9/cemba_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cemba-data
-Version: 1.6.8
+Version: 1.6.9
 Summary: Pipelines for single nucleus methylome and multi-omic dataset.
 Home-page: https://github.com/lhqing/cemba_data
 Author: Hanqing Liu
 Author-email: hanliu@salk.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cemba-data-1.6.8/cemba_data.egg-info/SOURCES.txt` & `cemba-data-1.6.9/cemba_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/Makefile` & `cemba-data-1.6.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/Mapping.ipynb` & `cemba-data-1.6.9/doc/Mapping.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/MappingSummary.ipynb` & `cemba-data-1.6.9/doc/MappingSummary.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/PipelineInput.ipynb` & `cemba-data-1.6.9/doc/PipelineInput.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/PlateInfoAndSampleSheet.ipynb` & `cemba-data-1.6.9/doc/PlateInfoAndSampleSheet.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/TODO_GenerateMCDS.ipynb` & `cemba-data-1.6.9/doc/TODO_GenerateMCDS.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/TODO_overview.ipynb` & `cemba-data-1.6.9/doc/TODO_overview.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/TechBasic.ipynb` & `cemba-data-1.6.9/doc/TechBasic.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/archive/MakeFastqDataframe.ipynb` & `cemba-data-1.6.9/doc/archive/MakeFastqDataframe.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/conf.py` & `cemba-data-1.6.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/demultiplex.ipynb` & `cemba-data-1.6.9/doc/demultiplex.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/files/MappingPipeline.png` & `cemba-data-1.6.9/doc/files/MappingPipeline.png`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/files/molecularsteps.png` & `cemba-data-1.6.9/doc/files/molecularsteps.png`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/files/primerstructure.png` & `cemba-data-1.6.9/doc/files/primerstructure.png`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/files/v1barcode.png` & `cemba-data-1.6.9/doc/files/v1barcode.png`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/files/v2barcode.png` & `cemba-data-1.6.9/doc/files/v2barcode.png`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/installation.ipynb` & `cemba-data-1.6.9/doc/installation.ipynb`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/doc/make.bat` & `cemba-data-1.6.9/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/env.yaml` & `cemba-data-1.6.9/env.yaml`

 * *Files identical despite different names*

### Comparing `cemba-data-1.6.8/setup.py` & `cemba-data-1.6.9/setup.py`

 * *Files identical despite different names*

