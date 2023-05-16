# Comparing `tmp/moftransformer-2.0.1.tar.gz` & `tmp/moftransformer-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-2.0.1.tar", last modified: Fri May  5 08:01:44 2023, max compression
+gzip compressed data, was "moftransformer-2.1.0.tar", last modified: Tue May 16 04:19:12 2023, max compression
```

## Comparing `moftransformer-2.0.1.tar` & `moftransformer-2.1.0.tar`

### file list

```diff
@@ -1,154 +1,277 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-05 08:01:44.805183 moftransformer-2.0.1/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8612 2023-05-05 06:56:57.000000 moftransformer-2.0.1/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      398 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      576 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3425 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.801183 moftransformer-2.0.1/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/Vector.hpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11518 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7374 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8004 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10096 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/run.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3567 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.805183 moftransformer-2.0.1/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.0.1/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-05 08:01:44.797183 moftransformer-2.0.1/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     6064 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-05-05 08:01:44.000000 moftransformer-2.0.1/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-05-05 08:01:44.805183 moftransformer-2.0.1/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.0.1/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-16 04:19:12.888613 moftransformer-2.1.0/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8612 2023-05-10 05:12:24.000000 moftransformer-2.1.0/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      458 2023-05-11 02:34:27.000000 moftransformer-2.1.0/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      571 2023-05-11 05:33:02.000000 moftransformer-2.1.0/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3431 2023-05-10 06:19:20.000000 moftransformer-2.1.0/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/dataset/test/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.868613 moftransformer-2.1.0/moftransformer/examples/dataset/total/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/dataset/train/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/dataset/val/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.880613 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.880613 moftransformer-2.1.0/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.884613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2023-05-11 05:04:23.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2023-05-11 05:04:24.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2023-05-11 05:04:25.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.o
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.884613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2023-05-11 05:04:26.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2023-05-11 05:04:26.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2023-05-11 05:04:27.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2023-05-11 05:04:27.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2023-05-11 05:04:28.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2023-05-11 05:04:28.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2023-05-11 05:04:29.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2023-05-11 05:04:29.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Vector.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/libgriday.a
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:33.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2COTA
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2023-05-11 05:04:33.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2props
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:31.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2visit
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2023-05-11 05:04:31.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid_gen
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12893 2023-05-11 05:46:03.000000 moftransformer-2.1.0/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7522 2023-05-11 02:40:22.000000 moftransformer-2.1.0/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8487 2023-05-11 02:35:20.000000 moftransformer-2.1.0/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11569 2023-05-11 05:23:53.000000 moftransformer-2.1.0/moftransformer/predict.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10348 2023-05-11 05:08:37.000000 moftransformer-2.1.0/moftransformer/run.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3900 2023-05-10 06:19:25.000000 moftransformer-2.1.0/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12799 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-05-16 04:19:12.888613 moftransformer-2.1.0/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.1.0/setup.py
```

### Comparing `moftransformer-2.0.1/PKG-INFO` & `moftransformer-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.0.1
+Version: 2.1.0
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.0 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
```

### Comparing `moftransformer-2.0.1/README.md` & `moftransformer-2.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

### Comparing `moftransformer-2.0.1/moftransformer/assets/bbs.json` & `moftransformer-2.1.0/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/assets/colors.py` & `moftransformer-2.1.0/moftransformer/assets/colors.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/assets/topology.json` & `moftransformer-2.1.0/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/cli/download.py` & `moftransformer-2.1.0/moftransformer/cli/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/cli/main.py` & `moftransformer-2.1.0/moftransformer/cli/main.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/cli/run.py` & `moftransformer-2.1.0/moftransformer/cli/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     @staticmethod
     def run(args):
         from moftransformer import __root_dir__
 
         run_path = Path(__root_dir__) / "run.py"
         config = args.args
         print(config)
-        os.system(f"python {run_path} with {' '.join(config)}")
+        os.system(f"python {run_path} {' '.join(config)}")
```

### Comparing `moftransformer-2.0.1/moftransformer/config.py` & `moftransformer-2.1.0/moftransformer/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.0.1
+# MOFTransformer version 2.1.0
 import os
 from sacred import Experiment
 from moftransformer import __root_dir__
 from moftransformer.utils.validation import _set_load_path, _loss_names
 
 ex = Experiment("pretrained_mof", save_git_info=False)
 
@@ -67,16 +67,16 @@
     test_only = False
 
     # below params varies with the environment
     root_dataset = os.path.join(__root_dir__, "examples/dataset")
     log_dir = "logs/"
     batch_size = 32  # desired batch size; for gradient accumulation
     per_gpu_batchsize = 8  # you should define this manually with per_gpu_batch_size
-    accelerator = "gpu"
-    devices = 1
+    accelerator = "auto"
+    devices = "auto"
     num_nodes = 1
 
     load_path = _set_load_path('pmtransformer')
 
     num_workers = 16  # the number of cpu's core
     precision = 16
```

### Comparing `moftransformer-2.0.1/moftransformer/config_ex.py` & `moftransformer-2.1.0/moftransformer/config_ex.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/database/__init__.py` & `moftransformer-2.1.0/moftransformer/database/__init__.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/datamodules/datamodule.py` & `moftransformer-2.1.0/moftransformer/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/datamodules/dataset.py` & `moftransformer-2.1.0/moftransformer/datamodules/dataset.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/smm+N577+E166.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/ukg+N387+E203.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-2.1.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/gadgets/my_metrics.py` & `moftransformer-2.1.0/moftransformer/gadgets/my_metrics.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/modules/cgcnn.py` & `moftransformer-2.1.0/moftransformer/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/modules/heads.py` & `moftransformer-2.1.0/moftransformer/modules/heads.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/modules/module.py` & `moftransformer-2.1.0/moftransformer/modules/module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.1.0
+from typing import Any, List
 import torch
 import torch.nn as nn
+import pytorch_lightning as pl
 from pytorch_lightning import LightningModule
 
 from moftransformer.modules import objectives, heads, module_utils
 from moftransformer.modules.cgcnn import GraphEmbeddings
 from moftransformer.modules.vision_transformer_3d import VisionTransformer3D
 
 from moftransformer.modules.module_utils import Normalizer
@@ -108,14 +110,19 @@
 
         if config["load_path"] != "" and config["test_only"]:
             ckpt = torch.load(config["load_path"], map_location="cpu")
             state_dict = ckpt["state_dict"]
             self.load_state_dict(state_dict, strict=False)
             print(f"load model : {config['load_path']}")
 
+        self.test_logits = []
+        self.test_labels = []
+        self.test_cifid = []
+        self.write_log = True
+
     def infer(
         self,
         batch,
         mask_grid=False,
     ):
         cif_id = batch["cif_id"]
         atom_num = batch["atom_num"]  # [N']
@@ -260,51 +267,91 @@
             ret.update(objectives.compute_regression(self, batch, normalizer))
 
         # classification
         if "classification" in self.current_tasks:
             ret.update(objectives.compute_classification(self, batch))
         return ret
 
-    def training_step(self, batch, batch_idx):
+    
+    def on_train_start(self):
         module_utils.set_task(self)
+        self.write_log = True
+
+    def training_step(self, batch, batch_idx):
         output = self(batch)
         total_loss = sum([v for k, v in output.items() if "loss" in k])
         return total_loss
 
-    def training_epoch_end(self, outputs):
+    def on_train_epoch_end(self):
         module_utils.epoch_wrapup(self)
 
-    def validation_step(self, batch, batch_idx):
+    def on_validation_start(self):
         module_utils.set_task(self)
+        self.write_log = True
+
+    def validation_step(self, batch, batch_idx):
         output = self(batch)
 
-    def validation_epoch_end(self, outputs):
+    def on_validation_epoch_end(self) -> None:
         module_utils.epoch_wrapup(self)
 
-    def test_step(self, batch, batch_idx):
+    def on_test_start(self,):
         module_utils.set_task(self)
+    
+    def test_step(self, batch, batch_idx):
         output = self(batch)
         output = {
             k: (v.cpu() if torch.is_tensor(v) else v) for k, v in output.items()
         }  # update cpu for memory
+
+        if 'regression_logits' in output.keys():
+            self.test_logits += output["regression_logits"].tolist()
+            self.test_labels += output["regression_labels"].tolist()
         return output
 
-    def test_epoch_end(self, outputs):
+    def on_test_epoch_end(self):
         module_utils.epoch_wrapup(self)
 
         # calculate r2 score when regression
-        if "regression_logits" in outputs[0].keys():
-            logits = []
-            labels = []
-            for out in outputs:
-                logits += out["regression_logits"].tolist()
-                labels += out["regression_labels"].tolist()
-
-            if len(logits) > 1:
-                r2 = r2_score(np.array(labels), np.array(logits))
-                self.log(f"test/r2_score", r2)
+        if len(self.test_logits) > 1:
+            r2 = r2_score(
+                np.array(self.test_labels), np.array(self.test_logits)
+            )
+            self.log(f"test/r2_score", r2, sync_dist=True)
+            self.test_labels.clear()
+            self.test_logits.clear()
 
     def configure_optimizers(self):
         return module_utils.set_schedule(self)
+    
+    def on_predict_start(self):
+        self.write_log = False
+        module_utils.set_task(self)
 
-    def lr_scheduler_step(self, scheduler, optimizer_idx, metric):
-        scheduler.step()
+    def predict_step(self, batch, batch_idx, dataloader_idx=0):
+        output = self(batch)
+        output = {
+            k: (v.cpu().tolist() if torch.is_tensor(v) else v)
+            for k, v in output.items()
+            if ('logits' in k) or ('labels' in k) or 'cif_id' == k
+        }
+        return output
+    
+    def on_predict_epoch_end(self, *args):
+        self.test_labels.clear()
+        self.test_logits.clear()
+
+    def on_predict_end(self, ):
+        self.write_log = True
+
+    def lr_scheduler_step(self, scheduler, *args):
+        if len(args) == 2:
+            optimizer_idx, metric = args
+        elif len(args) == 1:
+            metric, = args
+        else:
+            raise ValueError('lr_scheduler_step must have metric and optimizer_idx(optional)')
+
+        if pl.__version__ >= '2.0.0':
+            scheduler.step(epoch=self.current_epoch)
+        else:
+            scheduler.step()
```

### Comparing `moftransformer-2.0.1/moftransformer/modules/module_utils.py` & `moftransformer-2.1.0/moftransformer/modules/module_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.1.0
 import torch
 
 from torch.optim import AdamW
 from transformers import (
     get_polynomial_decay_schedule_with_warmup,
     get_cosine_schedule_with_warmup,
     get_constant_schedule,
@@ -43,44 +43,48 @@
 
         if loss_name == "regression" or loss_name == "vfp":
             # mse loss
             pl_module.log(
                 f"{loss_name}/{phase}/loss_epoch",
                 getattr(pl_module, f"{phase}_{loss_name}_loss").compute(),
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
+                sync_dist=True,
             )
             getattr(pl_module, f"{phase}_{loss_name}_loss").reset()
             # mae loss
             value = getattr(pl_module, f"{phase}_{loss_name}_mae").compute()
             pl_module.log(
                 f"{loss_name}/{phase}/mae_epoch",
                 value,
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
+                sync_dist=True,
             )
             getattr(pl_module, f"{phase}_{loss_name}_mae").reset()
 
             value = -value
         else:
             value = getattr(pl_module, f"{phase}_{loss_name}_accuracy").compute()
             pl_module.log(
                 f"{loss_name}/{phase}/accuracy_epoch",
                 value,
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
+                sync_dist=True,
             )
             getattr(pl_module, f"{phase}_{loss_name}_accuracy").reset()
             pl_module.log(
                 f"{loss_name}/{phase}/loss_epoch",
                 getattr(pl_module, f"{phase}_{loss_name}_loss").compute(),
                 batch_size=pl_module.hparams["config"]["per_gpu_batchsize"],
+                sync_dist=True,
             )
             getattr(pl_module, f"{phase}_{loss_name}_loss").reset()
 
         the_metric += value
 
-    pl_module.log(f"{phase}/the_metric", the_metric)
+    pl_module.log(f"{phase}/the_metric", the_metric, sync_dist=True)
 
 
 def set_schedule(pl_module):
     lr = pl_module.hparams.config["learning_rate"]
     wd = pl_module.hparams.config["weight_decay"]
 
     no_decay = [
```

### Comparing `moftransformer-2.0.1/moftransformer/modules/objectives.py` & `moftransformer-2.1.0/moftransformer/modules/objectives.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.1.0
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torchmetrics.functional import mean_absolute_error
 
 
 def init_weights(module):
@@ -37,16 +37,17 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_regression_loss")(ret["regression_loss"])
     mae = getattr(pl_module, f"{phase}_regression_mae")(
         mean_absolute_error(ret["regression_logits"], ret["regression_labels"])
     )
 
-    pl_module.log(f"regression/{phase}/loss", loss)
-    pl_module.log(f"regression/{phase}/mae", mae)
+    if pl_module.write_log:
+        pl_module.log(f"regression/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"regression/{phase}/mae", mae, sync_dist=True)
 
     return ret
 
 
 def compute_classification(pl_module, batch):
     infer = pl_module.infer(batch)
 
@@ -74,16 +75,17 @@
     loss = getattr(pl_module, f"{phase}_classification_loss")(
         ret["classification_loss"]
     )
     acc = getattr(pl_module, f"{phase}_classification_accuracy")(
         ret["classification_logits"], ret["classification_labels"]
     )
 
-    pl_module.log(f"classification/{phase}/loss", loss)
-    pl_module.log(f"classification/{phase}/accuracy", acc)
+    if pl_module.write_log:
+        pl_module.log(f"classification/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"classification/{phase}/accuracy", acc, sync_dist=True)
 
     return ret
 
 
 def compute_mpp(pl_module, batch):
     infer = pl_module.infer(batch, mask_grid=True)
 
@@ -110,16 +112,17 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_mpp_loss")(ret["mpp_loss"])
     acc = getattr(pl_module, f"{phase}_mpp_accuracy")(
         ret["mpp_logits"], ret["mpp_labels"]
     )
 
-    pl_module.log(f"mpp/{phase}/loss", loss)
-    pl_module.log(f"mpp/{phase}/accuracy", acc)
+    if pl_module.write_log:
+        pl_module.log(f"mpp/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"mpp/{phase}/accuracy", acc, sync_dist=True)
 
     return ret
 
 
 def compute_mtp(pl_module, batch):
     infer = pl_module.infer(batch)
     mtp_logits = pl_module.mtp_head(infer["cls_feats"])  # [B, hid_dim]
@@ -136,16 +139,17 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_mtp_loss")(ret["mtp_loss"])
     acc = getattr(pl_module, f"{phase}_mtp_accuracy")(
         ret["mtp_logits"], ret["mtp_labels"]
     )
 
-    pl_module.log(f"mtp/{phase}/loss", loss)
-    pl_module.log(f"mtp/{phase}/accuracy", acc)
+    if pl_module.write_log:
+        pl_module.log(f"mtp/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"mtp/{phase}/accuracy", acc, sync_dist=True)
 
     return ret
 
 
 def compute_vfp(pl_module, batch):
     infer = pl_module.infer(batch)
 
@@ -164,16 +168,17 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_vfp_loss")(ret["vfp_loss"])
     mae = getattr(pl_module, f"{phase}_vfp_mae")(
         mean_absolute_error(ret["vfp_logits"], ret["vfp_labels"])
     )
 
-    pl_module.log(f"vfp/{phase}/loss", loss)
-    pl_module.log(f"vfp/{phase}/mae", mae)
+    if pl_module.write_log:
+        pl_module.log(f"vfp/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"vfp/{phase}/mae", mae, sync_dist=True)
 
     return ret
 
 
 def compute_ggm(pl_module, batch):
     pos_len = len(batch["grid"]) // 2
     neg_len = len(batch["grid"]) - pos_len
@@ -206,16 +211,17 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_ggm_loss")(ret["ggm_loss"])
     acc = getattr(pl_module, f"{phase}_ggm_accuracy")(
         ret["ggm_logits"], ret["ggm_labels"]
     )
 
-    pl_module.log(f"ggm/{phase}/loss", loss)
-    pl_module.log(f"ggm/{phase}/accuracy", acc)
+    if pl_module.write_log:
+        pl_module.log(f"ggm/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"ggm/{phase}/accuracy", acc, sync_dist=True)
 
     return ret
 
 
 def compute_moc(pl_module, batch):
     if "bbc" in batch.keys():
         task = "bbc"
@@ -244,11 +250,12 @@
     # call update() loss and acc
     phase = "train" if pl_module.training else "val"
     loss = getattr(pl_module, f"{phase}_{task}_loss")(ret["moc_loss"])
     acc = getattr(pl_module, f"{phase}_{task}_accuracy")(
         nn.Sigmoid()(ret["moc_logits"]), ret["moc_labels"].long()
     )
 
-    pl_module.log(f"{task}/{phase}/loss", loss)
-    pl_module.log(f"{task}/{phase}/accuracy", acc)
+    if pl_module.write_log:
+        pl_module.log(f"{task}/{phase}/loss", loss, sync_dist=True)
+        pl_module.log(f"{task}/{phase}/accuracy", acc, sync_dist=True)
 
     return ret
```

### Comparing `moftransformer-2.0.1/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-2.1.0/moftransformer/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/run.py` & `moftransformer-2.1.0/moftransformer/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.1.0
 import sys
 import os
 import copy
 import warnings
 
 import pytorch_lightning as pl
 
@@ -30,15 +30,15 @@
 
     Call signatures::
         run(root_dataset, downstream, [test_only], **kwargs)
 
     The basic usage of the code is as follows:
 
     >>> run(root_dataset, downstream)  # train MOFTransformer from [root_dataset] with train_{downstream}.json
-    >>> run(root_dataset, downstream, log_dir, test_only=True, load_path=model_path) # predict MOFTransformer from trained-model path
+    >>> run(root_dataset, downstream, log_dir, test_only=True, load_path=model_path) # test MOFTransformer from trained-model path
 
     Dataset preperation is necessary for learning
     (url: https://hspark1212.github.io/MOFTransformer/dataset.html)
 
     Parameters
     __________
     :param root_dataset: A folder containing graph data, grid data, and json of MOFs that you want to train or test.
@@ -83,15 +83,15 @@
 
     loss_names: str or list, or dict, default: "regression"
         One or more of the following loss : 'regression', 'classification', 'mpt', 'moc', and 'vfp'
 
     n_classes: int, default: 0
         Number of classes when your loss is 'classification'
 
-    batch_size: int, default: 1024
+    batch_size: int, default: 32
         desired batch size; for gradient accumulation
 
     per_gpu_batchsize: int, default: 8
         you should define this manually with per_gpu_batch_size
 
     accelerator: str, default: 'auto'
         Supports passing different accelerator types ("cpu", "gpu", "tpu", "ipu", "hpu", "mps, "auto")
@@ -108,15 +108,15 @@
         the number of cpu's core
 
     precision: int or str, default: 16
         MOFTransformer supports either double (64), float (32), bfloat16 (bf16), or half (16) precision training.
         Half precision, or mixed precision, is the combined use of 32 and 16 bit floating points to reduce memory footprint during model training.
         This can result in improved performance, achieving +3X speedups on modern GPUs.
 
-    max_epochs: int, default: 100
+    max_epochs: int, default: 20
         Stop training once this number of epochs is reached.
 
     seed: int, default: 0
         The random seed for pytorch_lightning.
 
 
     Normalization parameters:
@@ -192,15 +192,15 @@
     ____________________________________
     resume_from = None
     val_check_interval = 1.0
     dataset_size = False  # experiments for dataset size with 100 [k] or 500 [k]
 
     """
 
-    config = _config()
+    config = copy.deepcopy(_config())
     for key in kwargs.keys():
         if key not in config:
             raise ConfigurationError(f"{key} is not in configuration.")
 
     config.update(kwargs)
     config["root_dataset"] = root_dataset
     config["downstream"] = downstream
@@ -225,17 +225,22 @@
         save_top_k=1,
         verbose=True,
         monitor="val/the_metric",
         mode="max",
         save_last=True,
     )
 
+    if _config["test_only"]:
+        name = f'test_{exp_name}_seed{_config["seed"]}_from_{str(_config["load_path"]).split("/")[-1][:-5]}'
+    else:
+        name = f'{exp_name}_seed{_config["seed"]}_from_{str(_config["load_path"]).split("/")[-1][:-5]}'
+
     logger = pl.loggers.TensorBoardLogger(
         _config["log_dir"],
-        name=f'{exp_name}_seed{_config["seed"]}_from_{str(_config["load_path"]).split("/")[-1][:-5]}',
+        name=name,
     )
 
     lr_callback = pl.callbacks.LearningRateMonitor(logging_interval="step")
     callbacks = [checkpoint_callback, lr_callback]
 
     num_device = get_num_devices(_config)
     print("num_device", num_device)
@@ -250,14 +255,16 @@
             _config["per_gpu_batchsize"] * num_device * _config["num_nodes"]
         )
 
     max_steps = _config["max_steps"] if _config["max_steps"] is not None else None
 
     if _IS_INTERACTIVE:
         strategy = None
+    elif pl.__version__ >= '2.0.0':
+        strategy = "ddp_find_unused_parameters_true"
     else:
         strategy = "ddp"
 
     log_every_n_steps = 10
 
     trainer = pl.Trainer(
         accelerator=_config["accelerator"],
@@ -268,16 +275,15 @@
         benchmark=True,
         max_epochs=_config["max_epochs"],
         max_steps=max_steps,
         callbacks=callbacks,
         logger=logger,
         accumulate_grad_batches=accumulate_grad_batches,
         log_every_n_steps=log_every_n_steps,
-        resume_from_checkpoint=_config["resume_from"],
         val_check_interval=_config["val_check_interval"],
         deterministic=True,
     )
 
     if not _config["test_only"]:
-        trainer.fit(model, datamodule=dm)
+        trainer.fit(model, datamodule=dm, ckpt_path=_config["resume_from"])
     else:
         trainer.test(model, datamodule=dm)
```

### Comparing `moftransformer-2.0.1/moftransformer/utils/download.py` & `moftransformer-2.1.0/moftransformer/utils/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/utils/install_griday.py` & `moftransformer-2.1.0/moftransformer/utils/install_griday.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/utils/prepare_data.py` & `moftransformer-2.1.0/moftransformer/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/utils/validation.py` & `moftransformer-2.1.0/moftransformer/utils/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,18 @@
-# MOFTransformer version 2.0.0
+# MOFTransformer version 2.1.0
 import sys
 import warnings
+import pytorch_lightning as pl
 from moftransformer.database import DEFAULT_PMTRANSFORMER_PATH, DEFAULT_MOFTRANSFORMER_PATH
 
+if pl.__version__ >= '2.0.0':
+    from pytorch_lightning.trainer.connectors.accelerator_connector import _AcceleratorConnector as AC
+else:
+    from pytorch_lightning.trainer.connectors.accelerator_connector import AcceleratorConnector as AC
+
 
 _IS_INTERACTIVE = hasattr(sys, "ps1")
 
 
 class ConfigurationError(Exception):
     pass
 
@@ -45,16 +51,20 @@
 def _set_load_path(path):
     if path == 'pmtransformer':
         return DEFAULT_PMTRANSFORMER_PATH
     if path == 'moftransformer':
         return DEFAULT_MOFTRANSFORMER_PATH
     elif not path:
         return ""
-    else:
+    elif str(path)[-4:] == 'ckpt':
         return path
+    else:
+        raise ConfigurationError(
+            "path must be 'pmtransformer', 'moftransformer', None, or *.ckpt, not {path}"
+        )
 
 
 def get_num_devices(_config):
     if isinstance(devices := _config["devices"], list):
         devices = len(devices)
     elif isinstance(devices, int):
         pass
@@ -64,60 +74,56 @@
         raise ConfigurationError(
             f'devices must be int, list, and "auto", not {devices}'
         )
     return devices
 
 
 def _get_auto_device(_config):
-    
-    from pytorch_lightning.trainer.connectors.accelerator_connector import (
-        AcceleratorConnector,
-    )
-    accelerator = AcceleratorConnector(accelerator=_config["accelerator"]).accelerator
+    accelerator = AC(accelerator=_config["accelerator"]).accelerator
     devices = accelerator.auto_device_count()
     
     return devices
 
 
-def _set_valid_batchsize(_config):
-    devices = get_num_devices(_config)
-
+def _set_valid_batchsize(_config, devices):
     per_gpu_batchsize = _config["batch_size"] // devices
 
     _config["per_gpu_batchsize"] = per_gpu_batchsize
     warnings.warn(
         "'Per_gpu_batchsize' is larger than 'batch_size'.\n"
         f" Adjusted to per_gpu_batchsize to {per_gpu_batchsize}"
     )
 
 
 def _check_valid_num_gpus(_config):
     devices = get_num_devices(_config)
 
     if devices > _config["batch_size"]:
         raise ConfigurationError(
-            "Number of devices must be smaller than batch_size. "
+            "Number of devices must be smaller than batch_size."
             f'num_gpus : {devices}, batch_size : {_config["batch_size"]}'
         )
 
     if _IS_INTERACTIVE and devices > 1:
         raise ConfigurationError(
             "The interactive environment (ex. jupyter notebook) does not supports multi-devices environment."
             "If you want to use multi-devices, make *.py file and run."
         )
+    
+    return devices
 
 
 def get_valid_config(_config):
     # set loss_name to dictionary
     _config["loss_names"] = _set_loss_names(_config["loss_names"])
 
     # set load_path to directory
     _config["load_path"] = _set_load_path(_config["load_path"])
 
     # check_valid_num_gpus
-    _check_valid_num_gpus(_config)
+    devices = _check_valid_num_gpus(_config)
 
     # Batch size must be larger than gpu_per_batch
-    if _config["batch_size"] < _config["per_gpu_batchsize"]:
-        _set_valid_batchsize(_config)
+    if _config["batch_size"] < _config["per_gpu_batchsize"] * devices:
+        _set_valid_batchsize(_config, devices)
 
     return _config
```

### Comparing `moftransformer-2.0.1/moftransformer/visualize/drawer.py` & `moftransformer-2.1.0/moftransformer/visualize/drawer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/visualize/setting.py` & `moftransformer-2.1.0/moftransformer/visualize/setting.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/visualize/utils.py` & `moftransformer-2.1.0/moftransformer/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer/visualize/visualizer.py` & `moftransformer-2.1.0/moftransformer/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.0.1/moftransformer.egg-info/PKG-INFO` & `moftransformer-2.1.0/moftransformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.0.1
+Version: 2.1.0
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.0.1-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.0.1-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.0 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
```

### Comparing `moftransformer-2.0.1/setup.py` & `moftransformer-2.1.0/setup.py`

 * *Files identical despite different names*

