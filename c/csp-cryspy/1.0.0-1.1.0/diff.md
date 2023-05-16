# Comparing `tmp/csp-cryspy-1.0.0.tar.gz` & `tmp/csp-cryspy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp-cryspy-1.0.0.tar", last modified: Thu Mar 16 13:18:46 2023, max compression
+gzip compressed data, was "csp-cryspy-1.1.0.tar", last modified: Tue May 16 08:22:18 2023, max compression
```

## Comparing `csp-cryspy-1.0.0.tar` & `csp-cryspy-1.1.0.tar`

### file list

```diff
@@ -1,112 +1,117 @@
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.272158 csp-cryspy-1.0.0/
--rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.0.0/LICENSE
--rw-r--r--   0 yamashita06   (501) staff       (20)     4972 2023-03-16 13:18:46.271760 csp-cryspy-1.0.0/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     3066 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/README.md
--rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.0.0/pyproject.toml
--rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-03-16 13:18:46.272205 csp-cryspy-1.0.0/setup.cfg
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.248398 csp-cryspy-1.0.0/src/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.249041 csp-cryspy-1.0.0/src/cryspy/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.250425 csp-cryspy-1.0.0/src/cryspy/BO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2580 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/bo_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6772 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/bo_next_select.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/bo_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4804 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/combo_cryspy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      688 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/BO/select_descriptor.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.251264 csp-cryspy-1.0.0/src/cryspy/EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3995 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/ea_append.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4870 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/ea_child.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2262 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/ea_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4765 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/ea_next_gen.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.252700 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    29426 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/crossover.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8526 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/ea_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8533 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/permutation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2858 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/rotation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9434 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/select_parents.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6434 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/strain.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.253704 csp-cryspy-1.0.0/src/cryspy/IO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/change_input.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1825 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/io_stat.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/out_results.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/pkl_data.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    69226 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/IO/read_input.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.254680 csp-cryspy-1.0.0/src/cryspy/LAQA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/LAQA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      455 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/LAQA/calc_score.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1394 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1862 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_next_selection.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1049 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.255299 csp-cryspy-1.0.0/src/cryspy/RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.255920 csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    28668 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    19283 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/random_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/rs_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/RS/rs_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.256165 csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.256663 csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/FP/
--rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/FP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3401 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/FP/calc_FP.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.257037 csp-cryspy-1.0.0/src/cryspy/interface/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.265018 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      855 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1442 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/collect_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2112 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.265796 csp-cryspy-1.0.0/src/cryspy/interface/OMX/
--rw-r--r--   0 yamashita06   (501) staff       (20)      752 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/OMX/calc_files_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2679 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/OMX/collect_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3954 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/OMX/ctrl_job_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/OMX/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.266610 csp-cryspy-1.0.0/src/cryspy/interface/QE/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/QE/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      703 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/QE/calc_files_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    11215 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/QE/collect_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3856 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/QE/ctrl_job_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2884 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/QE/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.267302 csp-cryspy-1.0.0/src/cryspy/interface/VASP/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/VASP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      661 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/VASP/calc_files_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9167 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/VASP/collect_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3603 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/VASP/ctrl_job_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.267639 csp-cryspy-1.0.0/src/cryspy/interface/ext/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/ext/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      428 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/ext/collect_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6603 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/select_code.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.268685 csp-cryspy-1.0.0/src/cryspy/interface/soiap/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/soiap/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      705 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/soiap/calc_files_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7477 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/soiap/collect_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2173 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/soiap/ctrl_job_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/interface/soiap/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.269162 csp-cryspy-1.0.0/src/cryspy/job/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/job/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    12290 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/job/ctrl_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    30737 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/job/ctrl_job.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.269519 csp-cryspy-1.0.0/src/cryspy/scripts/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/scripts/__init__.py
--rwxr-xr-x   0 yamashita06   (501) staff       (20)     3184 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/scripts/cryspy.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.270003 csp-cryspy-1.0.0/src/cryspy/start/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/start/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5786 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/start/cryspy_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5494 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/start/cryspy_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.270580 csp-cryspy-1.0.0/src/cryspy/util/
--rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/util/constants.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    15469 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/util/struc_util.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2555 2023-03-16 12:21:45.000000 csp-cryspy-1.0.0/src/cryspy/util/utility.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-03-16 13:18:46.271544 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/
--rw-r--r--   0 yamashita06   (501) staff       (20)     4972 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     2947 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/SOURCES.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/dependency_links.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       54 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/entry_points.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       14 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/requires.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        7 2023-03-16 13:18:46.000000 csp-cryspy-1.0.0/src/csp_cryspy.egg-info/top_level.txt
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.084537 csp-cryspy-1.1.0/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp-cryspy-1.1.0/LICENSE
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5562 2023-05-16 08:22:18.084063 csp-cryspy-1.1.0/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3656 2023-05-16 07:49:41.000000 csp-cryspy-1.1.0/README.md
+-rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp-cryspy-1.1.0/pyproject.toml
+-rw-r--r--   0 yamashita06   (501) staff       (20)       38 2023-05-16 08:22:18.084663 csp-cryspy-1.1.0/setup.cfg
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.031596 csp-cryspy-1.1.0/src/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.032798 csp-cryspy-1.1.0/src/cryspy/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.037816 csp-cryspy-1.1.0/src/cryspy/BO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2580 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6772 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_next_select.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/bo_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4804 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/combo_cryspy.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      688 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/BO/select_descriptor.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.040631 csp-cryspy-1.1.0/src/cryspy/EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3995 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_append.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4870 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_child.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2262 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4765 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/ea_next_gen.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.045247 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    29426 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/crossover.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8526 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/ea_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8533 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/permutation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2858 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/rotation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/select_parents.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6434 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/strain.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.048476 csp-cryspy-1.1.0/src/cryspy/IO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/change_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1825 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/io_stat.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5567 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/out_results.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4842 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/IO/pkl_data.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    70193 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/IO/read_input.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.050866 csp-cryspy-1.1.0/src/cryspy/LAQA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/calc_score.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1394 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1872 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_next_selection.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1049 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.052849 csp-cryspy-1.1.0/src/cryspy/RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.054808 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    28668 2023-04-20 07:19:24.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    19060 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/random_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/rs_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/RS/rs_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.055387 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.056737 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3401 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/calc_FP.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.058093 csp-cryspy-1.1.0/src/cryspy/interface/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.059373 csp-cryspy-1.1.0/src/cryspy/interface/ASE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      684 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/calc_files_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1065 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/collect_ase.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1915 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/ASE/ctrl_job_ase.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.061995 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      855 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1442 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/collect_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2112 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2859 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.064739 csp-cryspy-1.1.0/src/cryspy/interface/OMX/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      752 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/calc_files_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2679 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/collect_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3954 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/ctrl_job_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3119 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/OMX/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.067875 csp-cryspy-1.1.0/src/cryspy/interface/QE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      703 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/calc_files_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    11215 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/collect_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3856 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/ctrl_job_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2884 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/QE/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.070543 csp-cryspy-1.1.0/src/cryspy/interface/VASP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      661 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/calc_files_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9063 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/collect_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3603 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/VASP/ctrl_job_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.071927 csp-cryspy-1.1.0/src/cryspy/interface/ext/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/ext/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      428 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/ext/collect_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7127 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/interface/select_code.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.075159 csp-cryspy-1.1.0/src/cryspy/interface/soiap/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      705 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/calc_files_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7477 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/collect_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2173 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/ctrl_job_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2415 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/interface/soiap/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.076857 csp-cryspy-1.1.0/src/cryspy/job/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/job/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    12290 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/job/ctrl_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    30848 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/job/ctrl_job.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.077736 csp-cryspy-1.1.0/src/cryspy/scripts/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/scripts/__init__.py
+-rwxr-xr-x   0 yamashita06   (501) staff       (20)     4166 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/scripts/cryspy.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.079384 csp-cryspy-1.1.0/src/cryspy/start/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/start/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5317 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/cryspy_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4565 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/cryspy_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6664 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/start/gen_init_struc.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.080781 csp-cryspy-1.1.0/src/cryspy/util/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp-cryspy-1.1.0/src/cryspy/util/constants.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    15584 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/util/struc_util.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2581 2023-05-16 07:40:54.000000 csp-cryspy-1.1.0/src/cryspy/util/utility.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2023-05-16 08:22:18.083496 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5562 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3106 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/SOURCES.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/dependency_links.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       54 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/entry_points.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)       14 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/requires.txt
+-rw-r--r--   0 yamashita06   (501) staff       (20)        7 2023-05-16 08:22:18.000000 csp-cryspy-1.1.0/src/csp_cryspy.egg-info/top_level.txt
```

### Comparing `csp-cryspy-1.0.0/LICENSE` & `csp-cryspy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/PKG-INFO` & `csp-cryspy-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.0.0
+Version: 1.1.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -31,36 +31,45 @@
 Project-URL: changelog, https://github.com/Tomoki-YAMASHITA/CrySPY/blob/master/CHANGELOG.md
 Keywords: CSP
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![cryspy_logo](./logo/cryspy_fix-03.png)
+![cryspy_logo](https://github.com/Tomoki-YAMASHITA/CrySPY/blob/master/logo/cryspy_fix-03.png)
+
+[![PyPI version](https://badge.fury.io/py/csp-cryspy.svg)](https://badge.fury.io/py/csp-cryspy)
+[![Downloads](https://static.pepy.tech/badge/csp-cryspy)](https://pepy.tech/project/csp-cryspy)
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
-Document: https://tomoki-yamashita.github.io/CrySPY_doc/
+Document: https://tomoki-yamashita.github.io/CrySPY_doc  
+Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.0.0 (2023 March 16)
+version 1.1.0 (2023 May 16)
 
 ## News
+- [2023 May 16] CrySPY 1.1.0 released
+    + MPI parallelization (optional)
+    + New score of LAQA
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
-    + CrySPY is available in PyPI, so you can install by pip.
+    + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
 - [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
+- mpi4py
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
```

### Comparing `csp-cryspy-1.0.0/README.md` & `csp-cryspy-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-![cryspy_logo](./logo/cryspy_fix-03.png)
+![cryspy_logo](https://github.com/Tomoki-YAMASHITA/CrySPY/blob/master/logo/cryspy_fix-03.png)
+
+[![PyPI version](https://badge.fury.io/py/csp-cryspy.svg)](https://badge.fury.io/py/csp-cryspy)
+[![Downloads](https://static.pepy.tech/badge/csp-cryspy)](https://pepy.tech/project/csp-cryspy)
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
-Document: https://tomoki-yamashita.github.io/CrySPY_doc/
+Document: https://tomoki-yamashita.github.io/CrySPY_doc  
+Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.0.0 (2023 March 16)
+version 1.1.0 (2023 May 16)
 
 ## News
+- [2023 May 16] CrySPY 1.1.0 released
+    + MPI parallelization (optional)
+    + New score of LAQA
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
-    + CrySPY is available in PyPI, so you can install by pip.
+    + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
 - [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
+- mpi4py
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
```

### Comparing `csp-cryspy-1.0.0/pyproject.toml` & `csp-cryspy-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/BO/bo_init.py` & `csp-cryspy-1.1.0/src/cryspy/BO/bo_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/BO/bo_next_select.py` & `csp-cryspy-1.1.0/src/cryspy/BO/bo_next_select.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/BO/bo_restart.py` & `csp-cryspy-1.1.0/src/cryspy/BO/bo_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/BO/combo_cryspy.py` & `csp-cryspy-1.1.0/src/cryspy/BO/combo_cryspy.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/BO/select_descriptor.py` & `csp-cryspy-1.1.0/src/cryspy/BO/select_descriptor.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/ea_append.py` & `csp-cryspy-1.1.0/src/cryspy/EA/ea_append.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/ea_child.py` & `csp-cryspy-1.1.0/src/cryspy/EA/ea_child.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/ea_init.py` & `csp-cryspy-1.1.0/src/cryspy/EA/ea_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/ea_next_gen.py` & `csp-cryspy-1.1.0/src/cryspy/EA/ea_next_gen.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/crossover.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/crossover.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/ea_generation.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/ea_generation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/permutation.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/permutation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/rotation.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/rotation.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/select_parents.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/select_parents.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/EA/gen_struc_EA/strain.py` & `csp-cryspy-1.1.0/src/cryspy/EA/gen_struc_EA/strain.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/IO/io_stat.py` & `csp-cryspy-1.1.0/src/cryspy/IO/io_stat.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/IO/out_results.py` & `csp-cryspy-1.1.0/src/cryspy/IO/out_results.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/IO/pkl_data.py` & `csp-cryspy-1.1.0/src/cryspy/IO/pkl_data.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/IO/read_input.py` & `csp-cryspy-1.1.0/src/cryspy/IO/read_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
     # ---------- basic
     # ------ global declaration
     global algo, calc_code, tot_struc
     global nstage, njob, jobcmd, jobfile
     # ------ read intput variables
     calc_code = config.get('basic', 'calc_code')
-    if calc_code not in ['VASP', 'QE', 'soiap', 'LAMMPS', 'OMX', 'ext']:
+    if calc_code not in ['VASP', 'QE', 'soiap', 'LAMMPS', 'OMX', 'ASE', 'ext']:
         raise NotImplementedError(
-            'calc_code must be VASP, QE, OMX, soiap, LAMMPS, or ext')
+            'calc_code must be VASP, QE, OMX, soiap, LAMMPS, ASE, or ext')
     algo = config.get('basic', 'algo')
     if algo not in ['RS', 'BO', 'LAQA', 'EA']:
         raise NotImplementedError('algo must be RS, BO, LAQA, or EA')
     if algo == 'LAQA':
         if calc_code not in ['VASP', 'QE', 'soiap']:
             raise NotImplementedError('LAQA: only VASP, QE, and soiap for now')
     tot_struc = config.getint('basic', 'tot_struc')
@@ -290,35 +290,35 @@
                                  ' and less than tot_struc')
     try:
         append_struc_ea = config.getboolean('option', 'append_struc_ea')
     except (configparser.NoOptionError, configparser.NoSectionError):
         append_struc_ea = False
     try:
         energy_step_flag = config.getboolean('option', 'energy_step_flag')
-        if calc_code in ['LAMMPS', 'OMX', 'ext']:
+        if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
             raise NotImplementedError('energy_step_flag: only VASP, QE, and soiap for now')
     except (configparser.NoOptionError, configparser.NoSectionError):
         energy_step_flag = False
     try:
         struc_step_flag = config.getboolean('option', 'struc_step_flag')
-        if calc_code in ['LAMMPS', 'OMX', 'ext']:
+        if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
             raise NotImplementedError('struc_step_flag: only VASP, QE, and soiap for now')
     except (configparser.NoOptionError, configparser.NoSectionError):
         struc_step_flag = False
     try:
         force_step_flag = config.getboolean('option', 'force_step_flag')
-        if calc_code in ['LAMMPS', 'OMX', 'ext']:
+        if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
             raise NotImplementedError('force_step_flag: only VASP, QE, and soiap for now')
     except (configparser.NoOptionError, configparser.NoSectionError):
         force_step_flag = False
     if algo == 'LAQA':
         force_step_flag = True
     try:
         stress_step_flag = config.getboolean('option', 'stress_step_flag')
-        if calc_code in ['LAMMPS', 'OMX', 'ext']:
+        if calc_code in ['LAMMPS', 'OMX', 'ASE', 'ext']:
             raise NotImplementedError('stress_step_flag: only VASP, QE, and soiap for now')
     except (configparser.NoOptionError, configparser.NoSectionError):
         stress_step_flag = False
     if algo == 'LAQA':
         stress_step_flag = True
 
     # ---------- BO
@@ -410,21 +410,25 @@
         if emax_bo is not None and emin_bo is not None:
             if emin_bo > emax_bo:
                 raise ValueError('emax_bo < emin_bo, check emax_bo and emin_bo')
 
     # ---------- LAQA
     if algo == 'LAQA':
         # ------ global declaration
-        global nselect_laqa, weight_laqa
+        global nselect_laqa, wf, ws
         # ------ read intput variables
         nselect_laqa = config.getint('LAQA', 'nselect_laqa')
         try:
-            weight_laqa = config.getfloat('LAQA', 'weight_laqa')
+            wf = config.getfloat('LAQA', 'wf')
         except configparser.NoOptionError:
-            weight_laqa = 1.0
+            wf = 0.1
+        try:
+            ws = config.getfloat('LAQA', 'ws')
+        except configparser.NoOptionError:
+            ws = 10.0
 
     # ---------- EA
     if algo == 'EA' or append_struc_ea:
         # ------ global declaration
         global n_pop, n_crsov, n_perm, n_strain, n_rand, n_elite
         global fit_reverse, n_fittest
         global slct_func, t_size, a_rlt, b_rlt
@@ -669,14 +673,24 @@
             lammps_potential = lammps_potential.split()
         except configparser.NoOptionError:
             lammps_potential = None
         lammps_data = config.get('LAMMPS', 'lammps_data')
         kpt_flag = False
         force_gamma = False
 
+    # ---------- ase
+    elif calc_code == 'ASE':
+        # ------ global declaration
+        global ase_python
+        # ------ read input variables
+        try:
+            ase_python = config.get('ASE', 'ase_python')
+        except configparser.NoOptionError:
+            ase_python = 'ase.py'
+
     # ---------- ext
     elif calc_code == 'ext':
         kpt_flag = False
 
 
 def _spglist(spgnum):
     tmpspg = []
@@ -777,15 +791,16 @@
             ' '.join(str(x) for x in manual_select_bo)))
         stat.set('BO', 'emax_bo', '{}'.format(emax_bo))
         stat.set('BO', 'emin_bo', '{}'.format(emin_bo))
 
     # ---------- LAQA
     if algo == 'LAQA':
         stat.set('LAQA', 'nselect_laqa', '{}'.format(nselect_laqa))
-        stat.set('LAQA', 'weight_laqa', '{}'.format(weight_laqa))
+        stat.set('LAQA', 'wf', '{}'.format(wf))
+        stat.set('LAQA', 'ws', '{}'.format(ws))
 
     # ---------- EA
     elif algo == 'EA' or append_struc_ea:
         stat.set('EA', 'n_pop', '{}'.format(n_pop))
         stat.set('EA', 'n_crsov', '{}'.format(n_crsov))
         stat.set('EA', 'n_perm', '{}'.format(n_perm))
         stat.set('EA', 'n_strain', '{}'.format(n_strain))
@@ -852,14 +867,18 @@
             stat.set('LAMMPS', 'lammps_potential',
                      '{}'.format(lammps_potential))
         else:
             stat.set('LAMMPS', 'lammps_potential',
                      '{}'.format(' '.join(lammps_potential)))
         stat.set('LAMMPS', 'lammps_data', '{}'.format(lammps_data))
 
+    # ---------- ASE
+    if calc_code == 'ASE':
+        stat.set('ASE', 'ase_python', '{}'.format(ase_python))
+    
     # ---------- option
     stat.set('option', 'stop_chkpt', '{}'.format(stop_chkpt))
     stat.set('option', 'load_struc_flag', '{}'.format(load_struc_flag))
     stat.set('option', 'stop_next_struc', '{}'.format(stop_next_struc))
     stat.set('option', 'recalc', '{}'.format(' '.join(str(x) for x in recalc)))
     stat.set('option', 'append_struc_ea', '{}'.format(append_struc_ea))
     stat.set('option', 'energy_step_flag', '{}'.format(energy_step_flag))
@@ -999,15 +1018,17 @@
             old_emin_bo = None    # char --> None
         else:
             old_emin_bo = float(old_emin_bo)    # char --> float
 
     # ------ LAQA
     if old_algo == 'LAQA':
         old_nselect_laqa = stat.getint('LAQA', 'nselect_laqa')
-        old_weight_laqa = stat.getfloat('LAQA', 'weight_laqa')
+        old_wf = stat.getfloat('LAQA', 'wf')
+        old_ws = stat.getfloat('LAQA', 'ws')
+
 
     # ------ EA
     if old_algo == 'EA':
         old_n_pop = stat.getint('EA', 'n_pop')
         old_n_crsov = stat.getint('EA', 'n_crsov')
         old_n_perm = stat.getint('EA', 'n_perm')
         old_n_strain = stat.getint('EA', 'n_strain')
@@ -1083,14 +1104,18 @@
         old_lammps_potential = stat.get('LAMMPS', 'lammps_potential')
         if old_lammps_potential == 'None':    # 'None' is just character here
             old_lammps_potential = None
         else:
             old_lammps_potential = old_lammps_potential.split()    # str --> list
         old_lammps_data = stat.get('LAMMPS', 'lammps_data')
 
+    # ------ ASE
+    if old_calc_code == 'ASE':
+        old_ase_python = stat.get('ASE', 'ase_python')
+
     # ------ option
     old_stop_chkpt = stat.getint('option', 'stop_chkpt')
     old_load_struc_flag = stat.getboolean('option', 'load_struc_flag')
     old_stop_next_struc = stat.getboolean('option', 'stop_next_struc')
     old_recalc = stat.get('option', 'recalc')
     old_recalc = [int(x) for x in old_recalc.split()]    # int list
     old_append_struc_ea = stat.getboolean('option', 'append_struc_ea')
@@ -1324,17 +1349,21 @@
     # ------ LAQA
     sec = 'LAQA'
     if algo == 'LAQA':
         if not old_nselect_laqa == nselect_laqa:
             diff_out('nselect_laqa', old_nselect_laqa, nselect_laqa)
             io_stat.set_input_common(stat, sec, 'nselect_laqa', nselect_laqa)
             logic_change = True
-        if not old_weight_laqa == weight_laqa:
-            diff_out('weight_laqa', old_weight_laqa, weight_laqa)
-            io_stat.set_input_common(stat, sec, 'weight_laqa', weight_laqa)
+        if not old_wf == wf:
+            diff_out('wf', old_wf, wf)
+            io_stat.set_input_common(stat, sec, 'wf', wf)
+            logic_change = True
+        if not old_ws == ws:
+            diff_out('ws', old_ws, ws)
+            io_stat.set_input_common(stat, sec, 'ws', ws)
             logic_change = True
 
     # ------ EA
     sec = 'EA'
     if algo == 'EA':
         if not old_n_pop == n_pop:
             diff_out('n_pop', old_n_pop, n_pop)
@@ -1501,14 +1530,20 @@
         if not old_lammps_outfile == lammps_outfile:
             raise ValueError('Do not change lammps_outfile')
         if not old_lammps_potential == lammps_potential:
             raise ValueError('Do not change lammps_potential')
         if not old_lammps_data == lammps_data:
             raise ValueError('Do not change lammps_data')
 
+    # ------ ASE
+    sec = 'ASE'
+    if calc_code == 'ASE':
+        if not old_ase_python == ase_python:
+            raise ValueError('Do not change ase_python')
+
     # ------ option
     sec = 'option'
     if not old_stop_chkpt == stop_chkpt:
         diff_out('stop_chkpt', old_stop_chkpt, stop_chkpt)
         io_stat.set_input_common(stat, sec, 'stop_chkpt', stop_chkpt)
         logic_change = True
     if not old_load_struc_flag == load_struc_flag:
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_init.py` & `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_init.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_next_selection.py` & `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_next_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         else:
             id_queueing.append(k)
             if len(id_queueing) == rin.nselect_laqa:
                 break
 
     # ---------- done LAQA
     if len(id_queueing) == 0:
-        print('\nDone LAQA!')
+        print('\nDone all structures!')
         os.remove('lock_cryspy')
         raise SystemExit()
 
     # ---------- append id_select_hist and out
     id_select_hist.append(id_queueing[:])    # append shallow copy
     out_laqa_id_hist(id_select_hist)
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/LAQA/laqa_restart.py` & `csp-cryspy-1.1.0/src/cryspy/LAQA/laqa_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py` & `csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/RS/gen_struc_RS/random_generation.py` & `csp-cryspy-1.1.0/src/cryspy/RS/gen_struc_RS/random_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                       ' Space group: {1:>3} {2}'.format(cid, spg_num, spg_sym), flush=True)
                 # ------ save poscar
                 if init_pos_path is not None:
                     out_poscar(tmp_struc, cid, init_pos_path)
         self.init_struc_data = init_struc_data
 
     def gen_with_find_wy(self, nstruc, id_offset=0,
-                         init_pos_path=None, fwpath='find_wy'):
+                         init_pos_path=None, fwpath='find_wy', mpi_rank=0):
         '''
         Generate random structures with space gruop information
         using find_wy program
 
         # ---------- args
         nstruc (int): number of generated structures
 
@@ -105,17 +105,16 @@
 
         # ---------- comment
         generated init_struc_data is saved in self.init_struc_data
         '''
         # ---------- initialize
         init_struc_data = {}
         # ---------- cd tmp_gen_struc
-        if not os.path.isdir('tmp_gen_struc'):
-            os.mkdir('tmp_gen_struc')
-        os.chdir('tmp_gen_struc')
+        os.makedirs(f'tmp_gen_struc/rank_{mpi_rank}', exist_ok=True)
+        os.chdir(f'tmp_gen_struc/rank_{mpi_rank}')
 
         # ---------- generate structures
         while len(init_struc_data) < nstruc:
             # ------ get spg, a, b, c, alpha, beta, gamma in self.*
             self._gen_lattice()
             # ------ get cosa, cosb, and cosg in self.*
             self._calc_cos()
@@ -165,23 +164,18 @@
                 spg_sym = None
             # ------ register the structure in pymatgen format
             cid = len(init_struc_data) + id_offset
             init_struc_data[cid] = tmp_struc
             print('Structure ID {0:>6} was generated.'
                   ' Space group: {1:>3} --> {2:>3} {3}'.format(
                    cid, self.spg, spg_num, spg_sym), flush=True)
-            # ------ save poscar
-            if init_pos_path is not None:
-                os.chdir('../')    # temporarily go back to ../
-                out_poscar(tmp_struc, cid, init_pos_path)
-                os.chdir('tmp_gen_struc')
             # ------ clean
             self._rm_files()
         # ---------- go back to ..
-        os.chdir('../')
+        os.chdir('../../')
         # ---------- init_struc_data
         self.init_struc_data = init_struc_data
 
     def _get_atomlist(self):
         '''
         e.g. Na2Cl2
             atomlist = ['Na', 'Na', 'Cl', 'Cl']
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/RS/rs_restart.py` & `csp-cryspy-1.1.0/src/cryspy/RS/rs_restart.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/calc_dscrpt/FP/calc_FP.py` & `csp-cryspy-1.1.0/src/cryspy/calc_dscrpt/FP/calc_FP.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py` & `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/calc_files_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/collect_lammps.py` & `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/collect_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py` & `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/LAMMPS/structure.py` & `csp-cryspy-1.1.0/src/cryspy/interface/LAMMPS/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/OMX/calc_files_OMX.py` & `csp-cryspy-1.1.0/src/cryspy/interface/OMX/calc_files_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/OMX/collect_OMX.py` & `csp-cryspy-1.1.0/src/cryspy/interface/OMX/collect_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/OMX/ctrl_job_OMX.py` & `csp-cryspy-1.1.0/src/cryspy/interface/OMX/ctrl_job_OMX.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/OMX/structure.py` & `csp-cryspy-1.1.0/src/cryspy/interface/OMX/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/QE/calc_files_qe.py` & `csp-cryspy-1.1.0/src/cryspy/interface/QE/calc_files_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/QE/collect_qe.py` & `csp-cryspy-1.1.0/src/cryspy/interface/QE/collect_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/QE/ctrl_job_qe.py` & `csp-cryspy-1.1.0/src/cryspy/interface/QE/ctrl_job_qe.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/QE/structure.py` & `csp-cryspy-1.1.0/src/cryspy/interface/QE/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/VASP/calc_files_vasp.py` & `csp-cryspy-1.1.0/src/cryspy/interface/VASP/calc_files_vasp.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/VASP/collect_vasp.py` & `csp-cryspy-1.1.0/src/cryspy/interface/VASP/collect_vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     check_opt = check_opt_vasp(work_path+'OUTCAR')
     # ---------- obtain energy and magmom
     energy, magmom = get_energy_magmom_vasp(work_path)
     if np.isnan(energy):
         print('    Structure ID {0},'
               ' could not obtain energy from OSZICAR'.format(current_id))
     # ---------- collect CONTCAR
-    opt_struc = get_opt_struc_vasp(work_path+'CONTCAR')
+    try:
+        opt_struc = Structure.from_file(work_path+'CONTCAR')
+    except Exception:
+        opt_struc = None
     # ---------- check
     if np.isnan(energy):
         opt_struc = None
     if opt_struc is None:
         energy = np.nan
         magmom = np.nan
     # ---------- remove STOPCAR
@@ -64,22 +67,14 @@
                 magmom = float(oszi[-1].split()[-1])    # total magnetic moment
     except Exception:
         pass
     # ---------- return
     return energy, magmom
 
 
-def get_opt_struc_vasp(file_name):
-    try:
-        opt_struc = Structure.from_file(file_name)
-    except Exception:
-        opt_struc = None
-    return opt_struc
-
-
 def get_energy_step_vasp(energy_step_data, current_id, work_path):
     '''
     get energy step data in eV/atom
 
     energy_step_data[ID][stage][step]
     energy_step_data[ID][0] <-- stage 1
     energy_step_data[ID][1] <-- stage 2
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/VASP/ctrl_job_vasp.py` & `csp-cryspy-1.1.0/src/cryspy/interface/VASP/ctrl_job_vasp.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/select_code.py` & `csp-cryspy-1.1.0/src/cryspy/interface/select_code.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 '''
 Select an optimizer
     - VASP
     - QE
     - OMX
     - soiap
     - LAMMPS
+    - ASE
 '''
 
 from .VASP import calc_files_vasp, ctrl_job_vasp, collect_vasp
 from .QE import calc_files_qe, ctrl_job_qe, collect_qe
 from .soiap import calc_files_soiap, ctrl_job_soiap, collect_soiap
 from .LAMMPS import calc_files_lammps, ctrl_job_lammps, collect_lammps
 from .OMX import calc_files_OMX, ctrl_job_OMX, collect_OMX
+from .ASE import calc_files_ase, ctrl_job_ase, collect_ase
 from .ext import collect_ext
 
 from ..IO import read_input as rin
 
 
 def check_calc_files():
     if rin.calc_code == 'VASP':
@@ -24,23 +26,25 @@
         calc_files_qe.check_input_qe()
     elif rin.calc_code == 'OMX':
         calc_files_OMX.check_input_OMX()
     elif rin.calc_code == 'soiap':
         calc_files_soiap.check_input_soiap()
     elif rin.calc_code == 'LAMMPS':
         calc_files_lammps.check_input_lammps()
+    elif rin.calc_code == 'ASE':
+        calc_files_ase.check_input_ase()
     elif rin.calc_code == 'ext':
         pass
     else:
         raise NotImplementedError()
 
 
 def next_stage(stage, work_path, *args):
     # args[0] <-- kpt_data
-    # args[1] <-- current_id
+    # args[1] <-- current_id for kpt_data
     if rin.calc_code == 'VASP':
         skip_flag, kpt_data = ctrl_job_vasp.next_stage_vasp(stage, work_path,
                                                             args[0], args[1])
         return skip_flag, kpt_data
     elif rin.calc_code == 'QE':
         skip_flag, kpt_data = ctrl_job_qe.next_stage_qe(stage, work_path,
                                                         args[0], args[1])
@@ -51,14 +55,17 @@
         return skip_flag, kpt_data
     elif rin.calc_code == 'soiap':
         skip_flag = ctrl_job_soiap.next_stage_soiap(stage, work_path)
         return skip_flag
     elif rin.calc_code == 'LAMMPS':
         skip_flag = ctrl_job_lammps.next_stage_lammps(stage, work_path)
         return skip_flag
+    elif rin.calc_code == 'ASE':
+        skip_flag = ctrl_job_ase.next_stage_ase(stage, work_path)
+        return skip_flag
     else:
         raise NotImplementedError()
 
 
 def collect(current_id, work_path):
     if rin.calc_code == 'VASP':
         opt_struc, energy, magmom, check_opt = \
@@ -71,14 +78,17 @@
             collect_OMX.collect_OMX(current_id, work_path)
     elif rin.calc_code == 'soiap':
         opt_struc, energy, magmom, check_opt = \
             collect_soiap.collect_soiap(current_id, work_path)
     elif rin.calc_code == 'LAMMPS':
         opt_struc, energy, magmom, check_opt = \
             collect_lammps.collect_lammps(current_id, work_path)
+    elif rin.calc_code == 'ASE':
+        opt_struc, energy, magmom, check_opt = \
+            collect_ase.collect_ase(current_id, work_path)
     elif rin.calc_code == 'ext':
         ext_opt_struc_data, ext_energy_data = collect_ext.collect_ext()
         return ext_opt_struc_data, ext_energy_data
     else:
         raise NotImplementedError()
 
     # ---------- return
@@ -99,14 +109,16 @@
         kpt_data = ctrl_job_OMX.next_struc_OMX(structure, current_id,
                                                work_path, args[0])
         return kpt_data
     elif rin.calc_code == 'soiap':
         ctrl_job_soiap.next_struc_soiap(structure, current_id, work_path)
     elif rin.calc_code == 'LAMMPS':
         ctrl_job_lammps.next_struc_lammps(structure, current_id, work_path)
+    elif rin.calc_code == 'ASE':
+        ctrl_job_ase.next_struc_ase(structure, current_id, work_path)
     else:
         raise NotImplementedError()
 
 
 def get_energy_step(energy_step_data, current_id, work_path):
     if rin.calc_code == 'VASP':
         energy_step_data = collect_vasp.get_energy_step_vasp(
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/soiap/calc_files_soiap.py` & `csp-cryspy-1.1.0/src/cryspy/interface/soiap/calc_files_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/soiap/collect_soiap.py` & `csp-cryspy-1.1.0/src/cryspy/interface/soiap/collect_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/soiap/ctrl_job_soiap.py` & `csp-cryspy-1.1.0/src/cryspy/interface/soiap/ctrl_job_soiap.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/interface/soiap/structure.py` & `csp-cryspy-1.1.0/src/cryspy/interface/soiap/structure.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/job/ctrl_ext.py` & `csp-cryspy-1.1.0/src/cryspy/job/ctrl_ext.py`

 * *Files identical despite different names*

### Comparing `csp-cryspy-1.0.0/src/cryspy/job/ctrl_job.py` & `csp-cryspy-1.1.0/src/cryspy/job/ctrl_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
     def ctrl_collect_laqa(self):
         # ---------- flag for finish
         self.fin_laqa = False
         # ---------- get opt data
         opt_struc, energy, magmom, check_opt = \
             select_code.collect(self.current_id, self.work_path)
         # ---------- total step and laqa_step
-        #     force_step_data[key][stage][step][atom]
+        #     force_step_data[ID][stage][step][atom]
         if self.force_step_data[self.current_id][-1] is None:
             self.laqa_step[self.current_id].append(0)
         else:
             self.tot_step_select[-1] += len(
                 self.force_step_data[self.current_id][-1])
             self.laqa_step[self.current_id].append(
                 len(self.force_step_data[self.current_id][-1]))
@@ -331,17 +331,20 @@
         io_stat.set_common(self.stat, 'total_step', sum(self.tot_step_select))
         io_stat.write_stat(self.stat)
         # ---------- append laqa struc
         self.laqa_struc[self.current_id].append(opt_struc)
         # ---------- append laqa energy
         self.laqa_energy[self.current_id].append(energy)
         # ---------- append laqa bias
-        #     force_step_data[key][stage][step][atom]
+        #     force_step_data[ID][stage][step][atom]
+        #     stress_step_data[ID][stage][step][atom]
         tmp_laqa_bias = calc_laqa_bias(
-            self.force_step_data[self.current_id][-1], c=rin.weight_laqa)
+            self.force_step_data[self.current_id][-1],
+            self.stress_step_data[self.current_id][-1],
+            wf=rin.wf, ws=rin.ws)
         self.laqa_bias[self.current_id].append(tmp_laqa_bias)
         # ---------- append laqa score
         if check_opt == 'done' or np.isnan(energy) or np.isnan(tmp_laqa_bias):
             self.laqa_score[self.current_id].append(-float('inf'))
         else:
             self.laqa_score[self.current_id].append(-energy + tmp_laqa_bias)
         # ---------- save and out laqa data
@@ -618,20 +621,20 @@
         # ---------- done all structures
         if len(self.rslt_data) == rin.tot_struc:
             print('Done all structures!')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nBO is ready\n')
+            print('\nBO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('Stop at check point 3: BO is ready\n')
+            print('Stop at check point 3: BO is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- max_select_bo
         if 0 < rin.max_select_bo <= self.n_selection:
             print('Reached max_select_bo: {}\n'.format(rin.max_select_bo))
             os.remove('lock_cryspy')
             raise SystemExit()
@@ -643,20 +646,20 @@
                       self.id_running, self.id_select_hist)
         bo_next_select.next_select(self.stat, self.rslt_data,
                                    bo_id_data, bo_data)
 
     def next_select_LAQA(self):
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nLAQA is ready\n')
+            print('\nLAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('\nStop at check point 3: LAQA is ready\n')
+            print('\nStop at check point 3: LAQA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- selection of LAQA
         backup_cryspy()
         laqa_id_data = (self.id_queueing, self.id_running,
                         self.id_select_hist)
         laqa_data = (self.tot_step_select, self.laqa_step, self.laqa_struc,
@@ -664,20 +667,20 @@
         laqa_next_selection.next_selection(self.stat, laqa_id_data, laqa_data)
 
     def next_gen_EA(self):
         # ---------- log
         print('\nDone generation {}\n'.format(self.gen))
         # ---------- flag for next selection or generation
         if not self.go_next_sg:
-            print('\nEA is ready\n')
+            print('\nEA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- check point 3
         if rin.stop_chkpt == 3:
-            print('\nStop at check point 3: EA is ready\n')
+            print('\nStop at check point 3: EA is ready')
             os.remove('lock_cryspy')
             raise SystemExit()
         # ---------- maxgen_ea
         if 0 < rin.maxgen_ea <= self.gen:
             print('\nReached maxgen_ea: {}\n'.format(rin.maxgen_ea))
             os.remove('lock_cryspy')
             raise SystemExit()
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/start/cryspy_init.py` & `csp-cryspy-1.1.0/src/cryspy/start/cryspy_init.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,143 @@
 '''
 Initialize CrySPY
 '''
 
+from datetime import datetime
 import os
 
 import pandas as pd
 
+from .gen_init_struc import gen_init_struc
 from ..IO import pkl_data, io_stat
 from ..IO import read_input as rin
-from ..util.utility import get_date, get_version, check_fwpath
-from ..util.struc_util import set_mindist
+from ..util.utility import get_date, get_version
+from ..util.struc_util import out_poscar
 
 # ---------- import later
 #from ..RS import rs_init
 #from ..BO import bo_init
 #from ..LAQA import laqa_init
 #from ..EA import ea_init
 #from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
 #from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
 
 
-def initialize():
-    # ---------- start
-    print(get_date())
-    print('CrySPY ' + get_version())
-    print('Start cryspy.py\n', flush=True)
+def initialize(comm, mpi_rank, mpi_size):
+    if mpi_rank == 0:
+        # ---------- start
+        print(get_date())
+        print('CrySPY ' + get_version())
+        print('Start cryspy.py', flush=True)
+        print(f'Number of MPI processes: {mpi_size}\n')
 
     # ---------- read input
-    print('Read input file, cryspy.in')
+    if mpi_rank == 0:
+        print('Read input file, cryspy.in')
+    # ########## MPI start
+    if mpi_size > 1:
+        comm.barrier()
     rin.readin()          # read input data, cryspy,in
-    stat = io_stat.stat_init()    # initialize stat
-    rin.save_stat(stat)   # save input variables in cryspy.stat
+    # ########## MPI end
+    if mpi_rank == 0:
+        stat = io_stat.stat_init()    # initialize stat
+        rin.save_stat(stat)   # save input variables in cryspy.stat
 
-    # ---------- make data directory
-    os.makedirs('data/pkl_data', exist_ok=True)
+        # ---------- make data directory
+        os.makedirs('data/pkl_data', exist_ok=True)
 
     # ---------- generate initial structures
     if not rin.load_struc_flag:
+        if mpi_rank == 0:
+            print('\n# --------- Generate initial structures')
+        if mpi_size > 1:
+            comm.barrier()
+        if mpi_rank == 0:
+            # ------ time
+            time_start = datetime.today()
+        # ########## MPI start
         # ------ from scratch
-        print('\n# --------- Generate initial structures')
-        # ------ mindist
-        print('# ------ mindist')
-        mindist = set_mindist(rin.mindist, rin.mindist_factor)
-        # ------ pyxtal
-        if not (rin.spgnum == 0 or rin.use_find_wy):
-            from ..RS.gen_struc_RS.gen_pyxtal import Rnd_struc_gen_pyxtal
-            rsgx = Rnd_struc_gen_pyxtal(mindist=mindist)
-            # ------ crystal
-            if rin.struc_mode == 'crystal':
-                rsgx.gen_struc(nstruc=rin.tot_struc, id_offset=0,
-                               init_pos_path='./data/init_POSCARS')
-            # ------ molecular crystal
-            elif rin.struc_mode == 'mol':
-                rsgx.set_mol()
-                rsgx.gen_struc_mol(nstruc=rin.tot_struc, id_offset=0,
-                                   init_pos_path='./data/init_POSCARS')
-            # ------ molecular crystal breaking symmetry
-            elif rin.struc_mode == 'mol_bs':
-                print('# -- mindist_mol_bs')
-                mindist_dummy = set_mindist(rin.mindist_mol_bs, rin.mindist_mol_bs_factor, dummy=True)
-                rsgx.set_mol()
-                rsgx.gen_struc_mol_break_sym(nstruc=rin.tot_struc,
-                                             mindist_dummy=mindist_dummy,
-                                             id_offset=0,
-                                             init_pos_path='./data/init_POSCARS')
-            # ------ init_struc_data
-            init_struc_data = rsgx.init_struc_data
-            if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
-                struc_mol_id = rsgx.struc_mol_id
-        # ------ w/o pyxtal
-        else:
-            from ..RS.gen_struc_RS.random_generation import Rnd_struc_gen
-            rsg = Rnd_struc_gen(mindist=mindist)
-            if rin.spgnum == 0:
-                rsg.gen_wo_spg(nstruc=rin.tot_struc, id_offset=0,
-                               init_pos_path='./data/init_POSCARS')
-                init_struc_data = rsg.init_struc_data
-            else:
-                fwpath = check_fwpath(rin.fwpath)
-                rsg.gen_with_find_wy(nstruc=rin.tot_struc,
-                                     id_offset=0, init_pos_path='./data/init_POSCARS',
-                                     fwpath=fwpath)
-                init_struc_data = rsg.init_struc_data
-        # ------ save
-        pkl_data.save_init_struc(init_struc_data)
+        init_struc_data = {}
+        if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
+            struc_mol_id = {}
+        # ------ gen_init_struc()
+        # only init_struc_data in rank0 is important
         if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
-            pkl_data.save_struc_mol_id(struc_mol_id)
+            init_struc_data, struc_mol_id = gen_init_struc(init_struc_data, struc_mol_id,
+                                                           comm, mpi_rank, mpi_size)
+        else:
+            init_struc_data = gen_init_struc(init_struc_data, None,
+                                             comm, mpi_rank, mpi_size)
+        # ########## MPI end
+        if mpi_rank == 0:
+            # ------ save
+            pkl_data.save_init_struc(init_struc_data)
+            if rin.algo == 'EA' and rin.struc_mode in ['mol', 'mol_bs']:
+                pkl_data.save_struc_mol_id(struc_mol_id)
+            # ------ time
+            time_end = datetime.today()
+            etime = time_end - time_start
+            print(f'\nElapsed time for structure generation: {etime}\n')
     else:
         # ------ load initial structure
-        print('\n# --------- Load initial structure data')
-        print('Load ./data/pkl_data/init_struc_data.pkl\n')
-        init_struc_data = pkl_data.load_init_struc()
-        # -- check
-        if not rin.tot_struc == len(init_struc_data):
-            raise ValueError('rin.tot_struc = {0},'
-                             ' len(init_struc_data) = {1}'.format(
-                                 rin.tot_struc, len(init_struc_data)))
-
-    # ---------- initialize opt_struc_data
-    opt_struc_data = {}
-    pkl_data.save_opt_struc(opt_struc_data)
-
-    # ---------- initialize rslt_data
-    rslt_data = pd.DataFrame(columns=['Spg_num', 'Spg_sym',
-                                      'Spg_num_opt', 'Spg_sym_opt',
-                                      'E_eV_atom', 'Magmom', 'Opt'])
-    rslt_data[['Spg_num', 'Spg_num_opt']] = rslt_data[
-                                   ['Spg_num', 'Spg_num_opt']].astype(int)
-    pkl_data.save_rslt(rslt_data)
-
-    # ---------- initialize for each algorithm
-    if rin.algo == 'RS':
-        from ..RS import rs_init
-        rs_init.initialize(stat)
-    elif rin.algo == 'BO':
-        from ..BO import bo_init
-        bo_init.initialize(stat, init_struc_data, rslt_data)
-    elif rin.algo == 'LAQA':
-        from ..LAQA import laqa_init
-        laqa_init.initialize(stat)
-    elif rin.algo == "EA":
-        from ..EA import ea_init
-        ea_init.initialize(stat, rslt_data)
-
-    # ---------- initialize etc
-    if rin.kpt_flag:
-        kpt_data = {}
-        pkl_data.save_kpt(kpt_data)
-    if rin.energy_step_flag:
-        energy_step_data = {}
-        pkl_data.save_energy_step(energy_step_data)
-    if rin.struc_step_flag:
-        struc_step_data = {}
-        pkl_data.save_struc_step(struc_step_data)
-    if rin.force_step_flag:
-        force_step_data = {}
-        pkl_data.save_force_step(force_step_data)
-    if rin.stress_step_flag:
-        stress_step_data = {}
-        pkl_data.save_stress_step(stress_step_data)
-
-    # ---------- for ext
-    if rin.calc_code == 'ext':
-        os.makedirs('ext', exist_ok=True)
-        with open('ext/stat_job', 'w') as fstat:
-            fstat.write('out\n')
+        if mpi_rank == 0:
+            print('\n# --------- Load initial structure data')
+            print('Load ./data/pkl_data/init_struc_data.pkl\n')
+            init_struc_data = pkl_data.load_init_struc()
+            # -- check
+            if not rin.tot_struc == len(init_struc_data):
+                raise ValueError('rin.tot_struc = {0},'
+                                ' len(init_struc_data) = {1}'.format(
+                                    rin.tot_struc, len(init_struc_data)))
+            # -- init_POSCARS
+            for cid, struc in init_struc_data.items():
+                out_poscar(struc, cid, './data/init_POSCARS')
+
+    if mpi_rank == 0:
+        # ---------- initialize opt_struc_data
+        opt_struc_data = {}
+        pkl_data.save_opt_struc(opt_struc_data)
+
+        # ---------- initialize rslt_data
+        rslt_data = pd.DataFrame(columns=['Spg_num', 'Spg_sym',
+                                        'Spg_num_opt', 'Spg_sym_opt',
+                                        'E_eV_atom', 'Magmom', 'Opt'])
+        rslt_data[['Spg_num', 'Spg_num_opt']] = rslt_data[
+                                    ['Spg_num', 'Spg_num_opt']].astype(int)
+        pkl_data.save_rslt(rslt_data)
+
+        # ---------- initialize for each algorithm
+        if rin.algo == 'RS':
+            from ..RS import rs_init
+            rs_init.initialize(stat)
+        elif rin.algo == 'BO':
+            from ..BO import bo_init
+            bo_init.initialize(stat, init_struc_data, rslt_data)
+        elif rin.algo == 'LAQA':
+            from ..LAQA import laqa_init
+            laqa_init.initialize(stat)
+        elif rin.algo == "EA":
+            from ..EA import ea_init
+            ea_init.initialize(stat, rslt_data)
+
+        # ---------- initialize etc
+        if rin.kpt_flag:
+            kpt_data = {}
+            pkl_data.save_kpt(kpt_data)
+        if rin.energy_step_flag:
+            energy_step_data = {}
+            pkl_data.save_energy_step(energy_step_data)
+        if rin.struc_step_flag:
+            struc_step_data = {}
+            pkl_data.save_struc_step(struc_step_data)
+        if rin.force_step_flag:
+            force_step_data = {}
+            pkl_data.save_force_step(force_step_data)
+        if rin.stress_step_flag:
+            stress_step_data = {}
+            pkl_data.save_stress_step(stress_step_data)
+
+        # ---------- for ext
+        if rin.calc_code == 'ext':
+            os.makedirs('ext', exist_ok=True)
+            with open('ext/stat_job', 'w') as fstat:
+                fstat.write('out\n')
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/util/struc_util.py` & `csp-cryspy-1.1.0/src/cryspy/util/struc_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pymatgen.core import Structure
 from pymatgen.io.cif import CifWriter
 from pyxtal.tolerance import Tol_matrix
 
 from ..IO import read_input as rin
 
 
-def set_mindist(mindist_in, factor, dummy=False):
+def set_mindist(mindist_in, factor, dummy=False, mpi_rank=0):
     # ---------- dummy atom in mol_bs
     if dummy:
         atype = get_atype_dummy()
     else:
         atype = rin.atype
 
     # ---------- mindist
@@ -37,25 +37,26 @@
                 tmp.append(tolmat.get_tol(itype, jtype))
             mindist.append(tmp)
     else:
         tmp_array = factor * np.array(mindist_in)
         mindist = tmp_array.tolist()
 
     # ---------- print
-    for i, itype in enumerate(atype):
-        for j, jtype in enumerate(atype):
-            if i <= j:
-                if dummy:
-                    print(rin.mol_file[i], '-', rin.mol_file[j], mindist[i][j])
-                else:
-                    print(itype, '-', jtype, mindist[i][j])
-    if rin.struc_mode == 'mol':
-        print('When struc_mode is mol (only random structure, not EA part),')
-        print('- tolerance between monoatomic molecules is multiplied by 0.8 inside pyxtal (not printed above)')
-        print('- H-N, H-O, or H-F tolerance is multiplied by 0.9 inside pyxtal (not printed above)')
+    if mpi_rank == 0:
+        for i, itype in enumerate(atype):
+            for j, jtype in enumerate(atype):
+                if i <= j:
+                    if dummy:
+                        print(rin.mol_file[i], '-', rin.mol_file[j], mindist[i][j], flush=True)
+                    else:
+                        print(itype, '-', jtype, mindist[i][j], flush=True)
+        if rin.struc_mode == 'mol':
+            print('When struc_mode is mol (only random structure, not EA part),')
+            print('- tolerance between monoatomic molecules is multiplied by 0.8 inside pyxtal (not printed above)')
+            print('- H-N, H-O, or H-F tolerance is multiplied by 0.9 inside pyxtal (not printed above)',  flush=True)
 
     # ---------- return
     return mindist
 
 
 def get_atype_dummy():
     noble_gas = ['Rn', 'Xe', 'Kr', 'Ar', 'Ne', 'He']
```

### Comparing `csp-cryspy-1.0.0/src/cryspy/util/utility.py` & `csp-cryspy-1.1.0/src/cryspy/util/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import shutil
 import subprocess
 
 
 # ---------- functions
 def get_version():
-    return '1.0.0'
+    return '1.1.0'
 
 
 def get_date():
     return datetime.now().strftime("%Y/%m/%d %H:%M:%S")
 
 
 def check_fwpath(fwpath):
@@ -43,30 +43,29 @@
         if not os.path.isfile(fppath):
             raise IOError('There is no cal_fingerprint program in {}'.format(fppath))
     return fppath
 
 
 def backup_cryspy():
     # ---------- make directory
-    dst = 'backup'
-    if os.path.isdir(dst):
-        shutil.rmtree(dst)
-    os.mkdir(dst)
+    dname = datetime.now().strftime("%Y%m%d_%H%M%S")
+    dst = 'backup/' + dname + '/'
+    os.makedirs(dst, exist_ok=True)
 
     # ---------- file/directory list
     flist = ['cryspy.in', 'cryspy.stat', 'err_cryspy', 'log_cryspy']
     dlist = ['calc_in', 'data', 'ext']
 
     # ---------- backup
     for f in flist:
         if os.path.isfile(f):
             shutil.copy2(f, dst)
     for d in dlist:
         if os.path.isdir(d):
-            shutil.copytree(d, dst + '/' + d)
+            shutil.copytree(d, dst + d)
 
     # ---------- print
     print('\nBackup data')
 
 
 def clean_cryspy():
     # ---------- yes/no
```

### Comparing `csp-cryspy-1.0.0/src/csp_cryspy.egg-info/PKG-INFO` & `csp-cryspy-1.1.0/src/csp_cryspy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.0.0
+Version: 1.1.0
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -31,36 +31,45 @@
 Project-URL: changelog, https://github.com/Tomoki-YAMASHITA/CrySPY/blob/master/CHANGELOG.md
 Keywords: CSP
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![cryspy_logo](./logo/cryspy_fix-03.png)
+![cryspy_logo](https://github.com/Tomoki-YAMASHITA/CrySPY/blob/master/logo/cryspy_fix-03.png)
+
+[![PyPI version](https://badge.fury.io/py/csp-cryspy.svg)](https://badge.fury.io/py/csp-cryspy)
+[![Downloads](https://static.pepy.tech/badge/csp-cryspy)](https://pepy.tech/project/csp-cryspy)
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
-Document: https://tomoki-yamashita.github.io/CrySPY_doc/
+Document: https://tomoki-yamashita.github.io/CrySPY_doc  
+Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.0.0 (2023 March 16)
+version 1.1.0 (2023 May 16)
 
 ## News
+- [2023 May 16] CrySPY 1.1.0 released
+    + MPI parallelization (optional)
+    + New score of LAQA
+    + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 - [2023 March 16] CrySPY 1.0.0 released
-    + CrySPY is available in PyPI, so you can install by pip.
+    + CrySPY is available in PyPI, so you can install by pip (project name is csp-cryspy).
     + See also [Version information](https://tomoki-yamashita.github.io/CrySPY_doc/version_info) and [Changelog](./CHANGELOG.md)
 
 
 ## System requirements
 ### Python
 - Python >= 3.8
 - [PyXtal >= 0.5.3](https://pyxtal.readthedocs.io/en/latest "PyXtal")
 
 (optional)
 - [COMBO](https://github.com/Tomoki-YAMASHITA/combo3 "COMBO") (required if algo is BO)
+- mpi4py
 
 
 See [CrySPY document](https://tomoki-yamashita.github.io/CrySPY_doc/installation/requirements/ "CrySPY document") in detail.
 
 ### Structure optimizer
 At least one optimizer is required.
```

### Comparing `csp-cryspy-1.0.0/src/csp_cryspy.egg-info/SOURCES.txt` & `csp-cryspy-1.1.0/src/csp_cryspy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
 src/cryspy/RS/gen_struc_RS/random_generation.py
 src/cryspy/calc_dscrpt/__init__.py
 src/cryspy/calc_dscrpt/FP/__init__.py
 src/cryspy/calc_dscrpt/FP/calc_FP.py
 src/cryspy/interface/__init__.py
 src/cryspy/interface/select_code.py
+src/cryspy/interface/ASE/calc_files_ase.py
+src/cryspy/interface/ASE/collect_ase.py
+src/cryspy/interface/ASE/ctrl_job_ase.py
 src/cryspy/interface/LAMMPS/__init__.py
 src/cryspy/interface/LAMMPS/calc_files_lammps.py
 src/cryspy/interface/LAMMPS/collect_lammps.py
 src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
 src/cryspy/interface/LAMMPS/structure.py
 src/cryspy/interface/OMX/calc_files_OMX.py
 src/cryspy/interface/OMX/collect_OMX.py
@@ -71,14 +74,15 @@
 src/cryspy/job/ctrl_ext.py
 src/cryspy/job/ctrl_job.py
 src/cryspy/scripts/__init__.py
 src/cryspy/scripts/cryspy.py
 src/cryspy/start/__init__.py
 src/cryspy/start/cryspy_init.py
 src/cryspy/start/cryspy_restart.py
+src/cryspy/start/gen_init_struc.py
 src/cryspy/util/constants.py
 src/cryspy/util/struc_util.py
 src/cryspy/util/utility.py
 src/csp_cryspy.egg-info/PKG-INFO
 src/csp_cryspy.egg-info/SOURCES.txt
 src/csp_cryspy.egg-info/dependency_links.txt
 src/csp_cryspy.egg-info/entry_points.txt
```

