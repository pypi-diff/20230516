# Comparing `tmp/OApackage-2.7.6.tar.gz` & `tmp/OApackage-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\OApackage-2.7.6.tar", last modified: Thu Dec  8 23:01:17 2022, max compression
+gzip compressed data, was "OApackage-2.7.7.tar", last modified: Tue May 16 07:39:37 2023, max compression
```

## Comparing `OApackage-2.7.6.tar` & `OApackage-2.7.7.tar`

### file list

```diff
@@ -1,453 +1,454 @@
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.867607 OApackage-2.7.6/
--rw-rw-rw-   0        0        0       89 2022-12-08 22:55:49.000000 OApackage-2.7.6/CONTRIBUTORS.md
--rw-rw-rw-   0        0        0     2229 2022-12-08 22:55:49.000000 OApackage-2.7.6/LICENSE
--rw-rw-rw-   0        0        0      390 2022-12-08 22:55:49.000000 OApackage-2.7.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.633130 OApackage-2.7.6/OApackage.egg-info/
--rw-rw-rw-   0        0        0     5387 2022-12-08 23:01:17.000000 OApackage-2.7.6/OApackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13640 2022-12-08 23:01:17.000000 OApackage-2.7.6/OApackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-08 23:01:17.000000 OApackage-2.7.6/OApackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-08 22:59:22.000000 OApackage-2.7.6/OApackage.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2022-12-08 23:01:17.000000 OApackage-2.7.6/OApackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2022-12-08 23:01:17.000000 OApackage-2.7.6/OApackage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5387 2022-12-08 23:01:17.867607 OApackage-2.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     3613 2022-12-08 22:55:49.000000 OApackage-2.7.6/README.md
--rw-rw-rw-   0        0        0    34426 2022-12-08 22:55:49.000000 OApackage-2.7.6/doxy2swig.py
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.601881 OApackage-2.7.6/misc/
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.633130 OApackage-2.7.6/misc/scripts/
--rw-rw-rw-   0        0        0      767 2022-12-08 22:55:49.000000 OApackage-2.7.6/misc/scripts/example_oapackage_python.py
--rw-rw-rw-   0        0        0   105735 2022-12-08 22:55:49.000000 OApackage-2.7.6/numpy.i
--rw-rw-rw-   0        0        0       48 2022-12-08 22:55:49.000000 OApackage-2.7.6/oaconfig.txt
--rw-rw-rw-   0        0        0   144029 2022-12-08 22:55:49.000000 OApackage-2.7.6/oadoxy.i
--rw-rw-rw-   0        0        0    16256 2022-12-08 22:55:49.000000 OApackage-2.7.6/oalib.i
--rw-rw-rw-   0        0        0   413738 2022-12-08 22:57:43.000000 OApackage-2.7.6/oalib.py
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.648913 OApackage-2.7.6/oapackage/
--rw-rw-rw-   0        0        0    21031 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/Doptim.py
--rw-rw-rw-   0        0        0      852 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/__init__.py
--rw-rw-rw-   0        0        0     5625 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/_scanf.py
--rw-rw-rw-   0        0        0     3997 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/conference.py
--rw-rw-rw-   0        0        0     3539 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/graphtools.py
--rw-rw-rw-   0        0        0    21023 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/markup.py
--rw-rw-rw-   0        0        0    38421 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/oahelper.py
--rw-rw-rw-   0        0        0      316 2022-12-08 22:55:49.000000 OApackage-2.7.6/oapackage/scanf.py
--rw-rw-rw-   0        0        0      187 2022-12-08 23:01:17.867607 OApackage-2.7.6/setup.cfg
--rw-rw-rw-   0        0        0    12411 2022-12-08 22:55:49.000000 OApackage-2.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.664380 OApackage-2.7.6/src/
--rw-rw-rw-   0        0        0    16020 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Deff.cpp
--rw-rw-rw-   0        0        0     3902 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Deff.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.680011 OApackage-2.7.6/src/Eigen/
--rw-rw-rw-   0        0        0      694 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/CMakeLists.txt
--rw-rw-rw-   0        0        0     1206 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Cholesky
--rw-rw-rw-   0        0        0     1900 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/CholmodSupport
--rw-rw-rw-   0        0        0    17969 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Core
--rw-rw-rw-   0        0        0      122 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Dense
--rw-rw-rw-   0        0        0       35 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Eigen
--rw-rw-rw-   0        0        0     1822 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Eigenvalues
--rw-rw-rw-   0        0        0     2050 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Geometry
--rw-rw-rw-   0        0        0      874 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Householder
--rw-rw-rw-   0        0        0     2083 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/IterativeLinearSolvers
--rw-rw-rw-   0        0        0      939 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Jacobi
--rw-rw-rw-   0        0        0     1433 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/LU
--rw-rw-rw-   0        0        0      991 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/MetisSupport
--rw-rw-rw-   0        0        0     2483 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/OrderingMethods
--rw-rw-rw-   0        0        0     1676 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/PaStiXSupport
--rw-rw-rw-   0        0        0     1116 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/PardisoSupport
--rw-rw-rw-   0        0        0     1317 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/QR
--rw-rw-rw-   0        0        0      945 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/QtAlignedMalloc
--rw-rw-rw-   0        0        0     1162 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SPQRSupport
--rw-rw-rw-   0        0        0     1629 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SVD
--rw-rw-rw-   0        0        0      919 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/Sparse
--rw-rw-rw-   0        0        0     1371 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SparseCholesky
--rw-rw-rw-   0        0        0     2240 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SparseCore
--rw-rw-rw-   0        0        0     1713 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SparseLU
--rw-rw-rw-   0        0        0     1222 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SparseQR
--rw-rw-rw-   0        0        0      797 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/StdDeque
--rw-rw-rw-   0        0        0      726 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/StdList
--rw-rw-rw-   0        0        0      803 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/StdVector
--rw-rw-rw-   0        0        0     2243 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/SuperLUSupport
--rw-rw-rw-   0        0        0     1382 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/UmfPackSupport
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.617507 OApackage-2.7.6/src/Eigen/src/
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.680011 OApackage-2.7.6/src/Eigen/src/Cholesky/
--rw-rw-rw-   0        0        0    24440 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Cholesky/LDLT.h
--rw-rw-rw-   0        0        0    18395 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Cholesky/LLT.h
--rw-rw-rw-   0        0        0     3974 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.695629 OApackage-2.7.6/src/Eigen/src/CholmodSupport/
--rw-rw-rw-   0        0        0    22307 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.726881 OApackage-2.7.6/src/Eigen/src/Core/
--rw-rw-rw-   0        0        0    12218 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Array.h
--rw-rw-rw-   0        0        0     8179 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ArrayBase.h
--rw-rw-rw-   0        0        0     6775 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ArrayWrapper.h
--rw-rw-rw-   0        0        0     2720 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Assign.h
--rw-rw-rw-   0        0        0    38153 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/AssignEvaluator.h
--rw-rw-rw-   0        0        0    12479 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Assign_MKL.h
--rw-rw-rw-   0        0        0    13910 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/BandMatrix.h
--rw-rw-rw-   0        0        0    18064 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Block.h
--rw-rw-rw-   0        0        0     4249 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/BooleanRedux.h
--rw-rw-rw-   0        0        0     5689 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CommaInitializer.h
--rw-rw-rw-   0        0        0     6970 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ConditionEstimator.h
--rw-rw-rw-   0        0        0    62197 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CoreEvaluators.h
--rw-rw-rw-   0        0        0     4525 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CoreIterators.h
--rw-rw-rw-   0        0        0     7593 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-rw-   0        0        0    31424 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-rw-   0        0        0     8256 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-rw-   0        0        0     3877 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-rw-   0        0        0     5282 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-rw-   0        0        0    27420 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/DenseBase.h
--rw-rw-rw-   0        0        0    24212 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-rw-   0        0        0    21959 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/DenseStorage.h
--rw-rw-rw-   0        0        0     9597 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Diagonal.h
--rw-rw-rw-   0        0        0    12666 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-rw-   0        0        0      970 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/DiagonalProduct.h
--rw-rw-rw-   0        0        0    11507 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Dot.h
--rw-rw-rw-   0        0        0     5619 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/EigenBase.h
--rw-rw-rw-   0        0        0     4769 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-rw-   0        0        0     5705 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Fuzzy.h
--rw-rw-rw-   0        0        0    21123 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/GeneralProduct.h
--rw-rw-rw-   0        0        0    22185 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/GenericPacketMath.h
--rw-rw-rw-   0        0        0    10222 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/GlobalFunctions.h
--rw-rw-rw-   0        0        0     7076 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/IO.h
--rw-rw-rw-   0        0        0     3519 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Inverse.h
--rw-rw-rw-   0        0        0     7239 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Map.h
--rw-rw-rw-   0        0        0    10621 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/MapBase.h
--rw-rw-rw-   0        0        0    40402 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/MathFunctions.h
--rw-rw-rw-   0        0        0     3369 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-rw-   0        0        0    19170 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Matrix.h
--rw-rw-rw-   0        0        0    22154 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/MatrixBase.h
--rw-rw-rw-   0        0        0     3400 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/NestByValue.h
--rw-rw-rw-   0        0        0     3582 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/NoAlias.h
--rw-rw-rw-   0        0        0     9234 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/NumTraits.h
--rw-rw-rw-   0        0        0    21646 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/PermutationMatrix.h
--rw-rw-rw-   0        0        0    45180 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/PlainObjectBase.h
--rw-rw-rw-   0        0        0     7235 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Product.h
--rw-rw-rw-   0        0        0    49497 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ProductEvaluators.h
--rw-rw-rw-   0        0        0     6379 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Random.h
--rw-rw-rw-   0        0        0    17852 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Redux.h
--rw-rw-rw-   0        0        0    12800 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Ref.h
--rw-rw-rw-   0        0        0     5595 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Replicate.h
--rw-rw-rw-   0        0        0     4200 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/ReturnByValue.h
--rw-rw-rw-   0        0        0     7073 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Reverse.h
--rw-rw-rw-   0        0        0     6020 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Select.h
--rw-rw-rw-   0        0        0    14245 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/SelfAdjointView.h
--rw-rw-rw-   0        0        0     1697 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     6795 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Solve.h
--rw-rw-rw-   0        0        0     9031 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/SolveTriangular.h
--rw-rw-rw-   0        0        0     4365 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/SolverBase.h
--rw-rw-rw-   0        0        0     7692 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/StableNorm.h
--rw-rw-rw-   0        0        0     3865 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Stride.h
--rw-rw-rw-   0        0        0     2683 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Swap.h
--rw-rw-rw-   0        0        0    14777 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Transpose.h
--rw-rw-rw-   0        0        0    14386 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Transpositions.h
--rw-rw-rw-   0        0        0    37234 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/TriangularMatrix.h
--rw-rw-rw-   0        0        0     3462 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/VectorBlock.h
--rw-rw-rw-   0        0        0    29441 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/VectorwiseOp.h
--rw-rw-rw-   0        0        0     8074 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/Visitor.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.617507 OApackage-2.7.6/src/Eigen/src/Core/arch/
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.726881 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/
--rw-rw-rw-   0        0        0    18037 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-rw-   0        0        0    17776 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-rw-   0        0        0    27787 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-rw-   0        0        0     1194 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.726881 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX512/
--rw-rw-rw-   0        0        0    15733 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-rw-   0        0        0    50936 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.726881 OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/
--rw-rw-rw-   0        0        0    16443 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-rw-   0        0        0    10797 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-rw-   0        0        0    37671 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.742505 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/
--rw-rw-rw-   0        0        0     4240 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/Complex.h
--rw-rw-rw-   0        0        0    22059 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/Half.h
--rw-rw-rw-   0        0        0     2387 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-rw-rw-   0        0        0    10744 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-rw-rw-   0        0        0    35442 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-rw-rw-   0        0        0     5509 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.742505 OApackage-2.7.6/src/Eigen/src/Core/arch/Default/
--rw-rw-rw-   0        0        0     1989 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-rw-   0        0        0     1746 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/Default/Settings.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.742505 OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/
--rw-rw-rw-   0        0        0    17706 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-rw-   0        0        0     2846 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-rw-   0        0        0    28726 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.742505 OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/
--rw-rw-rw-   0        0        0    19426 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-rw-   0        0        0    18888 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-rw-   0        0        0    35825 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-rw-   0        0        0     1759 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.742505 OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/
--rw-rw-rw-   0        0        0    15366 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-rw-   0        0        0     4418 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-rw-rw-   0        0        0    32283 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.758538 OApackage-2.7.6/src/Eigen/src/Core/functors/
--rw-rw-rw-   0        0        0     6284 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-rw-   0        0        0    18263 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-rw-   0        0        0     8229 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-rw-   0        0        0     4400 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-rw-   0        0        0      607 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-rw-   0        0        0    27944 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.758538 OApackage-2.7.6/src/Eigen/src/Core/products/
--rw-rw-rw-   0        0        0    81106 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-rw-   0        0        0    18478 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-rw-   0        0        0    15188 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-rw-   0        0        0     6907 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-rw-   0        0        0     5017 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    26808 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-rw-   0        0        0     6368 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     4905 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/Parallelizer.h
--rw-rw-rw-   0        0        0    19632 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-rw-   0        0        0    11198 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0     9901 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-rw-   0        0        0     5209 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0     6105 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-rw-   0        0        0     4066 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-rw-   0        0        0    20403 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-rw-   0        0        0    13743 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-rw-   0        0        0    14722 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-rw-   0        0        0    10571 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-rw-   0        0        0    13979 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-rw-   0        0        0     6513 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-rw-   0        0        0     5741 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.773756 OApackage-2.7.6/src/Eigen/src/Core/util/
--rw-rw-rw-   0        0        0    15722 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/BlasUtil.h
--rw-rw-rw-   0        0        0    21579 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/Constants.h
--rw-rw-rw-   0        0        0     3564 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-rw-   0        0        0    14150 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-rw-   0        0        0     4026 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/MKL_support.h
--rw-rw-rw-   0        0        0    36570 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/Macros.h
--rw-rw-rw-   0        0        0    40154 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/Memory.h
--rw-rw-rw-   0        0        0    19365 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/Meta.h
--rw-rw-rw-   0        0        0       85 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/NonMPL2.h
--rw-rw-rw-   0        0        0      809 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-rw-   0        0        0    10518 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/StaticAssert.h
--rw-rw-rw-   0        0        0    34198 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Core/util/XprHelper.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.773756 OApackage-2.7.6/src/Eigen/src/Eigenvalues/
--rw-rw-rw-   0        0        0    12558 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-rw-   0        0        0    17021 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-rw-   0        0        0     4178 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    22944 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-rw-   0        0        0    17176 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-rw-   0        0        0     9715 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0    14351 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-rw-   0        0        0     5679 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-rw-   0        0        0    23586 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-rw-   0        0        0    20288 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-rw-   0        0        0     3650 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-rw-   0        0        0    33674 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-rw-   0        0        0     4104 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-rw-   0        0        0    22444 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.789379 OApackage-2.7.6/src/Eigen/src/Geometry/
--rw-rw-rw-   0        0        0    14815 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/AlignedBox.h
--rw-rw-rw-   0        0        0     8423 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/AngleAxis.h
--rw-rw-rw-   0        0        0     3639 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/EulerAngles.h
--rw-rw-rw-   0        0        0    20539 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Homogeneous.h
--rw-rw-rw-   0        0        0    11961 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Hyperplane.h
--rw-rw-rw-   0        0        0     8949 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-rw-   0        0        0     8308 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-rw-   0        0        0    32152 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Quaternion.h
--rw-rw-rw-   0        0        0     6877 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Rotation2D.h
--rw-rw-rw-   0        0        0     8063 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/RotationBase.h
--rw-rw-rw-   0        0        0     6324 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Scaling.h
--rw-rw-rw-   0        0        0    60514 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Transform.h
--rw-rw-rw-   0        0        0     7773 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Translation.h
--rw-rw-rw-   0        0        0     6191 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/Umeyama.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.789379 OApackage-2.7.6/src/Eigen/src/Geometry/arch/
--rw-rw-rw-   0        0        0     5387 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.789379 OApackage-2.7.6/src/Eigen/src/Householder/
--rw-rw-rw-   0        0        0     4481 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-rw-   0        0        0     5345 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Householder/Householder.h
--rw-rw-rw-   0        0        0    20603 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.789379 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/
--rw-rw-rw-   0        0        0     6755 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-rw-   0        0        0     7253 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-rw-   0        0        0     9184 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-rw-   0        0        0    15062 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-rw-   0        0        0    15234 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-rw-   0        0        0    11527 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-rw-   0        0        0     7762 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-rw-   0        0        0     4158 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.789379 OApackage-2.7.6/src/Eigen/src/Jacobi/
--rw-rw-rw-   0        0        0    15957 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/Jacobi/Jacobi.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/LU/
--rw-rw-rw-   0        0        0     3057 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/Determinant.h
--rw-rw-rw-   0        0        0    32803 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/FullPivLU.h
--rw-rw-rw-   0        0        0    15064 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/InverseImpl.h
--rw-rw-rw-   0        0        0    21478 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/PartialPivLU.h
--rw-rw-rw-   0        0        0     3555 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/LU/arch/
--rw-rw-rw-   0        0        0    13669 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/LU/arch/Inverse_SSE.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/MetisSupport/
--rw-rw-rw-   0        0        0     4588 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/OrderingMethods/
--rw-rw-rw-   0        0        0    16396 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/OrderingMethods/Amd.h
--rw-rw-rw-   0        0        0    62266 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-rw-   0        0        0     5229 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/PaStiXSupport/
--rw-rw-rw-   0        0        0    22248 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/PardisoSupport/
--rw-rw-rw-   0        0        0    20032 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/QR/
--rw-rw-rw-   0        0        0    24881 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-rw-   0        0        0     4662 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-rw-   0        0        0    20805 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-rw-   0        0        0    25478 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-rw-   0        0        0    14022 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/HouseholderQR.h
--rw-rw-rw-   0        0        0     2993 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/SPQRSupport/
--rw-rw-rw-   0        0        0    11405 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/SVD/
--rw-rw-rw-   0        0        0    48778 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SVD/BDCSVD.h
--rw-rw-rw-   0        0        0    32949 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SVD/JacobiSVD.h
--rw-rw-rw-   0        0        0     5099 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-rw-   0        0        0    12650 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SVD/SVDBase.h
--rw-rw-rw-   0        0        0    15957 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.805005 OApackage-2.7.6/src/Eigen/src/SparseCholesky/
--rw-rw-rw-   0        0        0    24010 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-rw-   0        0        0     6898 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.836253 OApackage-2.7.6/src/Eigen/src/SparseCore/
--rw-rw-rw-   0        0        0    10537 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-rw-   0        0        0     8164 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-rw-   0        0        0    13178 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-rw-   0        0        0     2191 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-rw-   0        0        0     8080 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-rw-   0        0        0    25592 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-rw-   0        0        0     6485 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-rw-   0        0        0    12720 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-rw-   0        0        0    25840 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-rw-   0        0        0     4711 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-rw-   0        0        0    12487 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-rw-   0        0        0     5808 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-rw-   0        0        0     3080 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDot.h
--rw-rw-rw-   0        0        0     1107 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-rw-   0        0        0    12589 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMap.h
--rw-rw-rw-   0        0        0    52349 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-rw-   0        0        0    17923 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-rw-   0        0        0     7329 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-rw-   0        0        0     7049 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-rw-   0        0        0     1699 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-rw-   0        0        0    15492 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseRef.h
--rw-rw-rw-   0        0        0    25715 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-rw-   0        0        0     4424 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-rw-   0        0        0     8704 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-rw-   0        0        0     3175 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-rw-   0        0        0     6437 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-rw-   0        0        0     6602 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-rw-   0        0        0    14831 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseVector.h
--rw-rw-rw-   0        0        0     8110 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/SparseView.h
--rw-rw-rw-   0        0        0     9657 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.836253 OApackage-2.7.6/src/Eigen/src/SparseLU/
--rw-rw-rw-   0        0        0    27923 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU.h
--rw-rw-rw-   0        0        0     4303 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-rw-   0        0        0     7601 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-rw-   0        0        0     4974 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-rw-   0        0        0    10022 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-rw-   0        0        0     2049 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-rw-   0        0        0     6712 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-rw-   0        0        0     6582 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-rw-   0        0        0     3681 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-rw-   0        0        0    10216 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-rw-   0        0        0     4181 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-rw-   0        0        0     5723 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-rw-   0        0        0     8486 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-rw-   0        0        0     9028 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-rw-   0        0        0     4979 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-rw-   0        0        0     4545 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-rw-   0        0        0     2889 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.836253 OApackage-2.7.6/src/Eigen/src/SparseQR/
--rw-rw-rw-   0        0        0    28373 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SparseQR/SparseQR.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.836253 OApackage-2.7.6/src/Eigen/src/StlSupport/
--rw-rw-rw-   0        0        0     5117 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/StlSupport/StdDeque.h
--rw-rw-rw-   0        0        0     4147 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/StlSupport/StdList.h
--rw-rw-rw-   0        0        0     5330 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/StlSupport/StdVector.h
--rw-rw-rw-   0        0        0     2809 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/StlSupport/details.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.836253 OApackage-2.7.6/src/Eigen/src/SuperLUSupport/
--rw-rw-rw-   0        0        0    34341 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.851884 OApackage-2.7.6/src/Eigen/src/UmfPackSupport/
--rw-rw-rw-   0        0        0    17202 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.851884 OApackage-2.7.6/src/Eigen/src/misc/
--rw-rw-rw-   0        0        0     2913 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/Image.h
--rw-rw-rw-   0        0        0     2742 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/Kernel.h
--rw-rw-rw-   0        0        0     1748 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/RealSvd2x2.h
--rw-rw-rw-   0        0        0    30560 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/blas.h
--rw-rw-rw-   0        0        0     7834 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/lapack.h
--rw-rw-rw-   0        0        0  1058368 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/lapacke.h
--rw-rw-rw-   0        0        0      474 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/misc/lapacke_mangling.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.851884 OApackage-2.7.6/src/Eigen/src/plugins/
--rw-rw-rw-   0        0        0    13132 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-rw-   0        0        0    16929 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-rw-   0        0        0    37403 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/BlockMethods.h
--rw-rw-rw-   0        0        0     4828 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     5621 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-rw-   0        0        0     6375 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-rw-   0        0        0     2937 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-rw-   0        0        0      121 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/InfInt.cpp
--rw-rw-rw-   0        0        0    33528 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/InfInt.h
--rw-rw-rw-   0        0        0    30719 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/anyoption.cpp
--rw-rw-rw-   0        0        0    11552 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/anyoption.h
--rw-rw-rw-   0        0        0    58143 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/arrayproperties.cpp
--rw-rw-rw-   0        0        0    25076 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/arrayproperties.h
--rw-rw-rw-   0        0        0   232511 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/arraytools.cpp
--rw-rw-rw-   0        0        0    63495 2022-12-08 22:55:49.000000 OApackage-2.7.6/src/arraytools.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.851884 OApackage-2.7.6/src/bitarray/
--rw-rw-rw-   0        0        0    15816 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/bitarray/bit_array.cpp
--rw-rw-rw-   0        0        0     4769 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/bitarray/bit_array.h
--rw-rw-rw-   0        0        0     4482 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/bitarray/bit_array_test.cpp
--rw-rw-rw-   0        0        0   125312 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/conference.cpp
--rw-rw-rw-   0        0        0    21130 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/conference.h
--rw-rw-rw-   0        0        0     8792 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/depth_extend.cpp
--rw-rw-rw-   0        0        0     1413 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/depth_extend.h
--rw-rw-rw-   0        0        0    37361 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/evenodd.cpp
--rw-rw-rw-   0        0        0    19179 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/evenodd.h
--rw-rw-rw-   0        0        0    40256 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/extend.cpp
--rw-rw-rw-   0        0        0     9929 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/extend.h
--rw-rw-rw-   0        0        0    15876 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/graphtools.cpp
--rw-rw-rw-   0        0        0     3041 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/graphtools.h
--rw-rw-rw-   0        0        0    91267 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/lmc.cpp
--rw-rw-rw-   0        0        0    20620 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/lmc.h
--rw-rw-rw-   0        0        0     8461 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/mathtools.cpp
--rw-rw-rw-   0        0        0    57619 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/mathtools.h
--rw-rw-rw-   0        0        0    16314 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/md5.cpp
--rw-rw-rw-   0        0        0      274 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/md5.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.851884 OApackage-2.7.6/src/mpitools/
--rw-rw-rw-   0        0        0    10354 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/mpitools/mpitools.cpp
--rw-rw-rw-   0        0        0     3256 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/mpitools/mpitools.h
--rw-rw-rw-   0        0        0     7926 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/msstdint.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.867607 OApackage-2.7.6/src/nauty/
--rw-rw-rw-   0        0        0    47137 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/gtools.c
--rw-rw-rw-   0        0        0     8276 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/gtools.h
--rw-rw-rw-   0        0        0    25673 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naugraph.c
--rw-rw-rw-   0        0        0     9584 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naugroup.c
--rw-rw-rw-   0        0        0     1451 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naugroup.h
--rw-rw-rw-   0        0        0     4681 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naurng.c
--rw-rw-rw-   0        0        0     1143 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naurng.h
--rw-rw-rw-   0        0        0     4542 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nausparse.h
--rw-rw-rw-   0        0        0    28418 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nautil.c
--rw-rw-rw-   0        0        0    65854 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nautinv.c
--rw-rw-rw-   0        0        0     2470 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nautinv.h
--rw-rw-rw-   0        0        0    14184 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/naututil.h
--rw-rw-rw-   0        0        0    46615 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nauty.c
--rw-rw-rw-   0        0        0    53904 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/nauty.h
--rw-rw-rw-   0        0        0    26910 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/schreier.c
--rw-rw-rw-   0        0        0     2741 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/schreier.h
--rw-rw-rw-   0        0        0    10479 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nauty/sorttemplates.c
--rw-rw-rw-   0        0        0    46007 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nonroot.cpp
--rw-rw-rw-   0        0        0     1343 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/nonroot.h
--rw-rw-rw-   0        0        0     5133 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/oaoptions.cpp
--rw-rw-rw-   0        0        0     1761 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/oaoptions.h
--rw-rw-rw-   0        0        0       16 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/pareto.cpp
--rw-rw-rw-   0        0        0    11534 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/pareto.h
--rw-rw-rw-   0        0        0      728 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/printfheader.h
--rw-rw-rw-   0        0        0    26632 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/strength.cpp
--rw-rw-rw-   0        0        0     6070 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/strength.h
--rw-rw-rw-   0        0        0    11896 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/tools.cpp
--rw-rw-rw-   0        0        0    14609 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/tools.h
--rw-rw-rw-   0        0        0     6761 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/unittests.cpp
--rw-rw-rw-   0        0        0      611 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/unittests.h
--rw-rw-rw-   0        0        0       35 2022-12-08 22:55:50.000000 OApackage-2.7.6/src/version.h
-drwxrwxrwx   0        0        0        0 2022-12-08 23:01:17.867607 OApackage-2.7.6/tests/
--rw-rw-rw-   0        0        0        0 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/__init__.py
--rw-rw-rw-   0        0        0     5793 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_Doptim.py
--rw-rw-rw-   0        0        0     4427 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_conference.py
--rw-rw-rw-   0        0        0    34777 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_cpplibrary.py
--rw-rw-rw-   0        0        0     1188 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_cpplibrary_gwlp.py
--rw-rw-rw-   0        0        0      897 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_cpplibrary_macwilliams.py
--rw-rw-rw-   0        0        0     1446 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_nauty.py
--rw-rw-rw-   0        0        0    16691 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_oapackage.py
--rw-rw-rw-   0        0        0      625 2022-12-08 22:55:50.000000 OApackage-2.7.6/tests/test_oapackage_graphtools.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/
+-rw-rw-rw-   0        0        0       89 2023-05-16 07:33:53.000000 OApackage-2.7.7/CONTRIBUTORS.md
+-rw-rw-rw-   0        0        0     2229 2023-05-16 07:33:53.000000 OApackage-2.7.7/LICENSE
+-rw-rw-rw-   0        0        0      390 2023-05-16 07:33:53.000000 OApackage-2.7.7/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.379256 OApackage-2.7.7/OApackage.egg-info/
+-rw-rw-rw-   0        0        0     4638 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13655 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 07:37:48.000000 OApackage-2.7.7/OApackage.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 07:39:37.000000 OApackage-2.7.7/OApackage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4638 2023-05-16 07:39:37.652107 OApackage-2.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3610 2023-05-16 07:33:53.000000 OApackage-2.7.7/README.md
+-rw-rw-rw-   0        0        0    34426 2023-05-16 07:33:54.000000 OApackage-2.7.7/doxy2swig.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/misc/
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.379256 OApackage-2.7.7/misc/scripts/
+-rw-rw-rw-   0        0        0      767 2023-05-16 07:33:54.000000 OApackage-2.7.7/misc/scripts/example_oapackage_python.py
+-rw-rw-rw-   0        0        0   105735 2023-05-16 07:33:54.000000 OApackage-2.7.7/numpy.i
+-rw-rw-rw-   0        0        0       48 2023-05-16 07:33:54.000000 OApackage-2.7.7/oaconfig.txt
+-rw-rw-rw-   0        0        0   144029 2023-05-16 07:33:54.000000 OApackage-2.7.7/oadoxy.i
+-rw-rw-rw-   0        0        0    16256 2023-05-16 07:33:54.000000 OApackage-2.7.7/oalib.i
+-rw-rw-rw-   0        0        0   421148 2023-05-16 07:35:59.000000 OApackage-2.7.7/oalib.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.394565 OApackage-2.7.7/oapackage/
+-rw-rw-rw-   0        0        0    21582 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/Doptim.py
+-rw-rw-rw-   0        0        0     2128 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/__init__.py
+-rw-rw-rw-   0        0        0     5620 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/_scanf.py
+-rw-rw-rw-   0        0        0     4150 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/conference.py
+-rw-rw-rw-   0        0        0     3569 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/graphtools.py
+-rw-rw-rw-   0        0        0    21493 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/markup.py
+-rw-rw-rw-   0        0        0    38474 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/oahelper.py
+-rw-rw-rw-   0        0        0      316 2023-05-16 07:33:54.000000 OApackage-2.7.7/oapackage/scanf.py
+-rw-rw-rw-   0        0        0      839 2023-05-16 07:33:54.000000 OApackage-2.7.7/pyproject.toml
+-rw-rw-rw-   0        0        0      187 2023-05-16 07:39:37.652107 OApackage-2.7.7/setup.cfg
+-rw-rw-rw-   0        0        0    12267 2023-05-16 07:33:54.000000 OApackage-2.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.412303 OApackage-2.7.7/src/
+-rw-rw-rw-   0        0        0    16020 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Deff.cpp
+-rw-rw-rw-   0        0        0     3902 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Deff.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/
+-rw-rw-rw-   0        0        0      694 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1206 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Cholesky
+-rw-rw-rw-   0        0        0     1900 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/CholmodSupport
+-rw-rw-rw-   0        0        0    17969 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Core
+-rw-rw-rw-   0        0        0      122 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Dense
+-rw-rw-rw-   0        0        0       35 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Eigen
+-rw-rw-rw-   0        0        0     1822 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Eigenvalues
+-rw-rw-rw-   0        0        0     2050 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Geometry
+-rw-rw-rw-   0        0        0      874 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Householder
+-rw-rw-rw-   0        0        0     2083 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/IterativeLinearSolvers
+-rw-rw-rw-   0        0        0      939 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Jacobi
+-rw-rw-rw-   0        0        0     1433 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/LU
+-rw-rw-rw-   0        0        0      991 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/MetisSupport
+-rw-rw-rw-   0        0        0     2483 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/OrderingMethods
+-rw-rw-rw-   0        0        0     1676 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/PaStiXSupport
+-rw-rw-rw-   0        0        0     1116 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/PardisoSupport
+-rw-rw-rw-   0        0        0     1317 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/QR
+-rw-rw-rw-   0        0        0      945 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/QtAlignedMalloc
+-rw-rw-rw-   0        0        0     1162 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SPQRSupport
+-rw-rw-rw-   0        0        0     1629 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SVD
+-rw-rw-rw-   0        0        0      919 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/Sparse
+-rw-rw-rw-   0        0        0     1371 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseCholesky
+-rw-rw-rw-   0        0        0     2240 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseCore
+-rw-rw-rw-   0        0        0     1713 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseLU
+-rw-rw-rw-   0        0        0     1222 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SparseQR
+-rw-rw-rw-   0        0        0      797 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdDeque
+-rw-rw-rw-   0        0        0      726 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdList
+-rw-rw-rw-   0        0        0      803 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/StdVector
+-rw-rw-rw-   0        0        0     2243 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/SuperLUSupport
+-rw-rw-rw-   0        0        0     1382 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/UmfPackSupport
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/src/Eigen/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/src/Cholesky/
+-rw-rw-rw-   0        0        0    24440 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LDLT.h
+-rw-rw-rw-   0        0        0    18395 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LLT.h
+-rw-rw-rw-   0        0        0     3974 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.441457 OApackage-2.7.7/src/Eigen/src/CholmodSupport/
+-rw-rw-rw-   0        0        0    22307 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/
+-rw-rw-rw-   0        0        0    12218 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Array.h
+-rw-rw-rw-   0        0        0     8179 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ArrayBase.h
+-rw-rw-rw-   0        0        0     6775 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-rw-   0        0        0     2720 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Assign.h
+-rw-rw-rw-   0        0        0    38153 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/AssignEvaluator.h
+-rw-rw-rw-   0        0        0    12479 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Assign_MKL.h
+-rw-rw-rw-   0        0        0    13910 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/BandMatrix.h
+-rw-rw-rw-   0        0        0    18064 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Block.h
+-rw-rw-rw-   0        0        0     4249 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/BooleanRedux.h
+-rw-rw-rw-   0        0        0     5689 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CommaInitializer.h
+-rw-rw-rw-   0        0        0     6970 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-rw-   0        0        0    62197 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-rw-   0        0        0     4525 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CoreIterators.h
+-rw-rw-rw-   0        0        0     7593 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-rw-   0        0        0    31424 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-rw-   0        0        0     8256 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-rw-   0        0        0     3877 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-rw-   0        0        0     5282 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-rw-   0        0        0    27420 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseBase.h
+-rw-rw-rw-   0        0        0    24212 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-rw-   0        0        0    21959 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DenseStorage.h
+-rw-rw-rw-   0        0        0     9597 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Diagonal.h
+-rw-rw-rw-   0        0        0    12666 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-rw-   0        0        0      970 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-rw-   0        0        0    11507 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Dot.h
+-rw-rw-rw-   0        0        0     5619 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/EigenBase.h
+-rw-rw-rw-   0        0        0     4769 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-rw-   0        0        0     5705 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Fuzzy.h
+-rw-rw-rw-   0        0        0    21123 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GeneralProduct.h
+-rw-rw-rw-   0        0        0    22185 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-rw-   0        0        0    10222 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-rw-   0        0        0     7076 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/IO.h
+-rw-rw-rw-   0        0        0     3519 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Inverse.h
+-rw-rw-rw-   0        0        0     7239 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Map.h
+-rw-rw-rw-   0        0        0    10621 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MapBase.h
+-rw-rw-rw-   0        0        0    40402 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MathFunctions.h
+-rw-rw-rw-   0        0        0     3369 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-rw-   0        0        0    19170 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Matrix.h
+-rw-rw-rw-   0        0        0    22154 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/MatrixBase.h
+-rw-rw-rw-   0        0        0     3400 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NestByValue.h
+-rw-rw-rw-   0        0        0     3582 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NoAlias.h
+-rw-rw-rw-   0        0        0     9234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/NumTraits.h
+-rw-rw-rw-   0        0        0    21646 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-rw-   0        0        0    45180 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-rw-   0        0        0     7235 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Product.h
+-rw-rw-rw-   0        0        0    49497 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-rw-   0        0        0     6379 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Random.h
+-rw-rw-rw-   0        0        0    17852 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Redux.h
+-rw-rw-rw-   0        0        0    12800 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Ref.h
+-rw-rw-rw-   0        0        0     5595 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Replicate.h
+-rw-rw-rw-   0        0        0     4200 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/ReturnByValue.h
+-rw-rw-rw-   0        0        0     7073 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Reverse.h
+-rw-rw-rw-   0        0        0     6020 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Select.h
+-rw-rw-rw-   0        0        0    14245 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-rw-   0        0        0     1697 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     6795 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Solve.h
+-rw-rw-rw-   0        0        0     9031 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SolveTriangular.h
+-rw-rw-rw-   0        0        0     4365 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/SolverBase.h
+-rw-rw-rw-   0        0        0     7692 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/StableNorm.h
+-rw-rw-rw-   0        0        0     3865 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Stride.h
+-rw-rw-rw-   0        0        0     2683 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Swap.h
+-rw-rw-rw-   0        0        0    14777 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Transpose.h
+-rw-rw-rw-   0        0        0    14386 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Transpositions.h
+-rw-rw-rw-   0        0        0    37234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-rw-   0        0        0     3462 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/VectorBlock.h
+-rw-rw-rw-   0        0        0    29441 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-rw-   0        0        0     8074 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/Visitor.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.363316 OApackage-2.7.7/src/Eigen/src/Core/arch/
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/
+-rw-rw-rw-   0        0        0    18037 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-rw-   0        0        0    17776 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-rw-   0        0        0    27787 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-rw-   0        0        0     1194 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/
+-rw-rw-rw-   0        0        0    15733 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-rw-   0        0        0    50936 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/
+-rw-rw-rw-   0        0        0    16443 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-rw-   0        0        0    10797 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-rw-   0        0        0    37671 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/
+-rw-rw-rw-   0        0        0     4240 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-rw-rw-   0        0        0    22059 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Half.h
+-rw-rw-rw-   0        0        0     2387 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-rw-rw-   0        0        0    10744 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-rw-rw-   0        0        0    35442 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-rw-rw-   0        0        0     5509 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.488316 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/
+-rw-rw-rw-   0        0        0     1989 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-rw-   0        0        0     1746 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/Default/Settings.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/
+-rw-rw-rw-   0        0        0    17706 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-rw-   0        0        0     2846 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-rw-   0        0        0    28726 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/
+-rw-rw-rw-   0        0        0    19426 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-rw-   0        0        0    18888 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-rw-rw-   0        0        0    35825 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-rw-   0        0        0     1759 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/
+-rw-rw-rw-   0        0        0    15366 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-rw-   0        0        0     4418 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-rw-rw-   0        0        0    32283 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.503941 OApackage-2.7.7/src/Eigen/src/Core/functors/
+-rw-rw-rw-   0        0        0     6284 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-rw-   0        0        0    18263 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-rw-   0        0        0     8229 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-rw-   0        0        0     4400 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-rw-   0        0        0      607 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-rw-   0        0        0    27944 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.519566 OApackage-2.7.7/src/Eigen/src/Core/products/
+-rw-rw-rw-   0        0        0    81106 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-rw-   0        0        0    18478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-rw-   0        0        0    15188 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-rw-   0        0        0     6907 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-rw-   0        0        0     5017 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    26808 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-rw-   0        0        0     6368 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     4905 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-rw-   0        0        0    19632 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-rw-   0        0        0    11198 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0     9901 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-rw-   0        0        0     5209 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0     6105 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-rw-   0        0        0     4066 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-rw-   0        0        0    20403 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-rw-   0        0        0    13743 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-rw-   0        0        0    14722 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-rw-   0        0        0    10571 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-rw-   0        0        0    13979 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-rw-   0        0        0     6513 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-rw-   0        0        0     5741 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.527083 OApackage-2.7.7/src/Eigen/src/Core/util/
+-rw-rw-rw-   0        0        0    15722 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-rw-   0        0        0    21579 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Constants.h
+-rw-rw-rw-   0        0        0     3564 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-rw-   0        0        0    14150 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-rw-   0        0        0     4026 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/MKL_support.h
+-rw-rw-rw-   0        0        0    36570 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Macros.h
+-rw-rw-rw-   0        0        0    40154 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Memory.h
+-rw-rw-rw-   0        0        0    19365 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/Meta.h
+-rw-rw-rw-   0        0        0       85 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-rw-   0        0        0      809 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-rw-   0        0        0    10518 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-rw-   0        0        0    34198 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Core/util/XprHelper.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.527083 OApackage-2.7.7/src/Eigen/src/Eigenvalues/
+-rw-rw-rw-   0        0        0    12558 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-rw-   0        0        0    17021 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-rw-   0        0        0     4178 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    22944 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-rw-   0        0        0    17176 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-rw-   0        0        0     9715 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0    14351 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-rw-   0        0        0     5679 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-rw-   0        0        0    23586 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-rw-   0        0        0    20288 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-rw-   0        0        0     3650 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-rw-   0        0        0    33674 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-rw-   0        0        0     4104 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-rw-   0        0        0    22444 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Geometry/
+-rw-rw-rw-   0        0        0    14815 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-rw-   0        0        0     8423 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-rw-   0        0        0     3639 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-rw-   0        0        0    20539 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-rw-   0        0        0    11961 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-rw-   0        0        0     8949 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-rw-   0        0        0     8308 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-rw-   0        0        0    32152 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Quaternion.h
+-rw-rw-rw-   0        0        0     6877 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-rw-   0        0        0     8063 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/RotationBase.h
+-rw-rw-rw-   0        0        0     6324 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Scaling.h
+-rw-rw-rw-   0        0        0    60514 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Transform.h
+-rw-rw-rw-   0        0        0     7773 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Translation.h
+-rw-rw-rw-   0        0        0     6191 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/Umeyama.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Geometry/arch/
+-rw-rw-rw-   0        0        0     5387 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Householder/
+-rw-rw-rw-   0        0        0     4481 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-rw-   0        0        0     5345 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/Householder.h
+-rw-rw-rw-   0        0        0    20603 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/
+-rw-rw-rw-   0        0        0     6755 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-rw-   0        0        0     7253 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-rw-   0        0        0     9184 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-rw-   0        0        0    15062 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-rw-   0        0        0    15234 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-rw-   0        0        0    11527 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-rw-   0        0        0     7762 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-rw-   0        0        0     4158 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.542746 OApackage-2.7.7/src/Eigen/src/Jacobi/
+-rw-rw-rw-   0        0        0    15957 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/Jacobi/Jacobi.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/LU/
+-rw-rw-rw-   0        0        0     3057 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/Determinant.h
+-rw-rw-rw-   0        0        0    32803 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/FullPivLU.h
+-rw-rw-rw-   0        0        0    15064 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/InverseImpl.h
+-rw-rw-rw-   0        0        0    21478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU.h
+-rw-rw-rw-   0        0        0     3555 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/LU/arch/
+-rw-rw-rw-   0        0        0    13669 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/LU/arch/Inverse_SSE.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/MetisSupport/
+-rw-rw-rw-   0        0        0     4588 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/OrderingMethods/
+-rw-rw-rw-   0        0        0    16396 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-rw-   0        0        0    62266 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-rw-   0        0        0     5229 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/PaStiXSupport/
+-rw-rw-rw-   0        0        0    22248 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/PardisoSupport/
+-rw-rw-rw-   0        0        0    20032 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/QR/
+-rw-rw-rw-   0        0        0    24881 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-rw-   0        0        0     4662 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-rw-   0        0        0    20805 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-rw-   0        0        0    25478 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-rw-   0        0        0    14022 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR.h
+-rw-rw-rw-   0        0        0     2993 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SPQRSupport/
+-rw-rw-rw-   0        0        0    11405 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SVD/
+-rw-rw-rw-   0        0        0    48778 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/BDCSVD.h
+-rw-rw-rw-   0        0        0    32949 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-rw-   0        0        0     5099 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-rw-   0        0        0    12650 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/SVDBase.h
+-rw-rw-rw-   0        0        0    15957 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.558360 OApackage-2.7.7/src/Eigen/src/SparseCholesky/
+-rw-rw-rw-   0        0        0    24010 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-rw-   0        0        0     6898 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseCore/
+-rw-rw-rw-   0        0        0    10537 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-rw-   0        0        0     8164 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-rw-   0        0        0    13178 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-rw-   0        0        0     2191 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-rw-   0        0        0     8080 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-rw-   0        0        0    25592 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-rw-   0        0        0     6485 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-rw-   0        0        0    12720 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-rw-   0        0        0    25840 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-rw-   0        0        0     4711 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-rw-   0        0        0    12487 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-rw-   0        0        0     5808 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-rw-   0        0        0     3080 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-rw-   0        0        0     1107 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-rw-   0        0        0    12589 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-rw-   0        0        0    52349 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-rw-   0        0        0    17923 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-rw-   0        0        0     7329 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-rw-   0        0        0     7049 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-rw-   0        0        0     1699 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-rw-   0        0        0    15492 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-rw-   0        0        0    25715 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-rw-   0        0        0     4424 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-rw-   0        0        0     8704 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-rw-   0        0        0     3175 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-rw-   0        0        0     6437 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-rw-   0        0        0     6602 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-rw-   0        0        0    14831 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-rw-   0        0        0     8110 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/SparseView.h
+-rw-rw-rw-   0        0        0     9657 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseLU/
+-rw-rw-rw-   0        0        0    27923 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-rw-   0        0        0     4303 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-rw-   0        0        0     7601 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-rw-   0        0        0     4974 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-rw-   0        0        0    10022 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-rw-   0        0        0     2049 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-rw-   0        0        0     6712 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-rw-   0        0        0     6582 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-rw-   0        0        0     3681 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-rw-   0        0        0    10216 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-rw-   0        0        0     4181 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-rw-   0        0        0     5723 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-rw-   0        0        0     8486 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-rw-   0        0        0     9028 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-rw-   0        0        0     4979 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-rw-   0        0        0     4545 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-rw-   0        0        0     2889 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SparseQR/
+-rw-rw-rw-   0        0        0    28373 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SparseQR/SparseQR.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/StlSupport/
+-rw-rw-rw-   0        0        0     5117 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-rw-   0        0        0     4147 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdList.h
+-rw-rw-rw-   0        0        0     5330 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/StdVector.h
+-rw-rw-rw-   0        0        0     2809 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/StlSupport/details.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/SuperLUSupport/
+-rw-rw-rw-   0        0        0    34341 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.589672 OApackage-2.7.7/src/Eigen/src/UmfPackSupport/
+-rw-rw-rw-   0        0        0    17202 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.605246 OApackage-2.7.7/src/Eigen/src/misc/
+-rw-rw-rw-   0        0        0     2913 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/Image.h
+-rw-rw-rw-   0        0        0     2742 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/Kernel.h
+-rw-rw-rw-   0        0        0     1748 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-rw-   0        0        0    30560 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/blas.h
+-rw-rw-rw-   0        0        0     7834 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapack.h
+-rw-rw-rw-   0        0        0  1058368 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapacke.h
+-rw-rw-rw-   0        0        0      474 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/misc/lapacke_mangling.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/Eigen/src/plugins/
+-rw-rw-rw-   0        0        0    13132 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0    16929 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0    37403 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/BlockMethods.h
+-rw-rw-rw-   0        0        0     4828 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     5621 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0     6375 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-rw-   0        0        0     2937 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-rw-   0        0        0      121 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/InfInt.cpp
+-rw-rw-rw-   0        0        0    33528 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/InfInt.h
+-rw-rw-rw-   0        0        0    30719 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/anyoption.cpp
+-rw-rw-rw-   0        0        0    11552 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/anyoption.h
+-rw-rw-rw-   0        0        0    57087 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arrayproperties.cpp
+-rw-rw-rw-   0        0        0    25076 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arrayproperties.h
+-rw-rw-rw-   0        0        0   231991 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arraytools.cpp
+-rw-rw-rw-   0        0        0    63495 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/arraytools.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/bitarray/
+-rw-rw-rw-   0        0        0    15816 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array.cpp
+-rw-rw-rw-   0        0        0     4769 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array.h
+-rw-rw-rw-   0        0        0     4482 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/bitarray/bit_array_test.cpp
+-rw-rw-rw-   0        0        0   125312 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/conference.cpp
+-rw-rw-rw-   0        0        0    21129 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/conference.h
+-rw-rw-rw-   0        0        0     8792 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/depth_extend.cpp
+-rw-rw-rw-   0        0        0     1413 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/depth_extend.h
+-rw-rw-rw-   0        0        0    37361 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/evenodd.cpp
+-rw-rw-rw-   0        0        0    19179 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/evenodd.h
+-rw-rw-rw-   0        0        0    40268 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/extend.cpp
+-rw-rw-rw-   0        0        0     9929 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/extend.h
+-rw-rw-rw-   0        0        0    15876 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/graphtools.cpp
+-rw-rw-rw-   0        0        0     3041 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/graphtools.h
+-rw-rw-rw-   0        0        0    91267 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/lmc.cpp
+-rw-rw-rw-   0        0        0    20620 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/lmc.h
+-rw-rw-rw-   0        0        0     8461 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mathtools.cpp
+-rw-rw-rw-   0        0        0    57619 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mathtools.h
+-rw-rw-rw-   0        0        0    16314 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/md5.cpp
+-rw-rw-rw-   0        0        0      274 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/md5.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.621722 OApackage-2.7.7/src/mpitools/
+-rw-rw-rw-   0        0        0    10354 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mpitools/mpitools.cpp
+-rw-rw-rw-   0        0        0     3256 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/mpitools/mpitools.h
+-rw-rw-rw-   0        0        0     7926 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/msstdint.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/src/nauty/
+-rw-rw-rw-   0        0        0    47137 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/gtools.c
+-rw-rw-rw-   0        0        0     8276 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/gtools.h
+-rw-rw-rw-   0        0        0    25673 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugraph.c
+-rw-rw-rw-   0        0        0     9584 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugroup.c
+-rw-rw-rw-   0        0        0     1451 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naugroup.h
+-rw-rw-rw-   0        0        0     4681 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naurng.c
+-rw-rw-rw-   0        0        0     1143 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naurng.h
+-rw-rw-rw-   0        0        0     4542 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nausparse.h
+-rw-rw-rw-   0        0        0    28418 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautil.c
+-rw-rw-rw-   0        0        0    65854 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautinv.c
+-rw-rw-rw-   0        0        0     2470 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nautinv.h
+-rw-rw-rw-   0        0        0    14184 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/naututil.h
+-rw-rw-rw-   0        0        0    46615 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nauty.c
+-rw-rw-rw-   0        0        0    53904 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/nauty.h
+-rw-rw-rw-   0        0        0    26910 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/schreier.c
+-rw-rw-rw-   0        0        0     2741 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/schreier.h
+-rw-rw-rw-   0        0        0    10479 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nauty/sorttemplates.c
+-rw-rw-rw-   0        0        0    46007 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nonroot.cpp
+-rw-rw-rw-   0        0        0     1343 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/nonroot.h
+-rw-rw-rw-   0        0        0     5133 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/oaoptions.cpp
+-rw-rw-rw-   0        0        0     1761 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/oaoptions.h
+-rw-rw-rw-   0        0        0       16 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/pareto.cpp
+-rw-rw-rw-   0        0        0    11534 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/pareto.h
+-rw-rw-rw-   0        0        0      728 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/printfheader.h
+-rw-rw-rw-   0        0        0    26632 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/strength.cpp
+-rw-rw-rw-   0        0        0     6070 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/strength.h
+-rw-rw-rw-   0        0        0    12014 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/tools.cpp
+-rw-rw-rw-   0        0        0    14609 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/tools.h
+-rw-rw-rw-   0        0        0     6761 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/unittests.cpp
+-rw-rw-rw-   0        0        0      611 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/unittests.h
+-rw-rw-rw-   0        0        0       35 2023-05-16 07:33:54.000000 OApackage-2.7.7/src/version.h
+drwxrwxrwx   0        0        0        0 2023-05-16 07:39:37.636482 OApackage-2.7.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     5904 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_Doptim.py
+-rw-rw-rw-   0        0        0     4427 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_conference.py
+-rw-rw-rw-   0        0        0    34777 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary.py
+-rw-rw-rw-   0        0        0     1188 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary_gwlp.py
+-rw-rw-rw-   0        0        0      897 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_cpplibrary_macwilliams.py
+-rw-rw-rw-   0        0        0     1446 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_nauty.py
+-rw-rw-rw-   0        0        0    16691 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_oapackage.py
+-rw-rw-rw-   0        0        0      625 2023-05-16 07:33:54.000000 OApackage-2.7.7/tests/test_oapackage_graphtools.py
```

### Comparing `OApackage-2.7.6/LICENSE` & `OApackage-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/OApackage.egg-info/PKG-INFO` & `OApackage-2.7.7/OApackage.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 Metadata-Version: 2.1
 Name: OApackage
-Version: 2.7.6
+Version: 2.7.7
 Summary: Package to generate and analyse orthogonal arrays, conference designs and optimal designs
 Home-page: http://www.pietereendebak.nl/oapackage/index.html
 Author: Pieter Eendebak
 Author-email: pieter.eendebak@gmail.com
 License: BSD
-Description: Orthogonal Array Package
-        ========================
-        
-        The Orthogonal Array package contains functionality to generate and analyse orthogonal arrays, optimal designs and conference designs.
-        Features include generation of complete series of orthogonal arrays,
-        reduction of arrays to normal form and calculation of properties such as the strength or D-efficiency of an array.
-        For more information about the package see the
-        documentation at [oapackage.readthedocs.io](https://oapackage.readthedocs.io/en/latest/). A large collection of results generated
-        with the package can be found at <http://pietereendebak.nl/oapackage/>.
-        
-        Usage
-        -------
-        
-        The package can be used from Python:
-        ``` python
-        >>> import oapackage
-        >>> al=oapackage.exampleArray(0)
-        >>> al.showarraycompact()
-        00
-        00
-        01
-        01
-        10
-        10
-        11
-        11
-        >>> print('D-efficiency %f, rank %d' % (al.Defficiency(), al.rank()) )
-        D-efficiency 1.000000, rank 2
-        >>> print('Generalized wordlength pattern: %s' % str(al.GWLP()))
-        Generalized wordlength pattern: (1.0, 0.0, 0.0)
-        ```
-        
-        For more examples see the Jupyter notebooks in the
-        [docs/examples](docs/examples/).
-        
-        Acknowledgements
-        ----------------
-        
-        If you use this code or any of the results, please cite this program as follows:
-        
-        * [OApackage: A Python package for generation and analysis of orthogonal arrays, optimal designs and conference designs](https://doi.org/10.21105/joss.01097), P.T. Eendebak, A.R. Vazquez, Journal of Open Source Software, 2019
-        * [Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays](https://doi.org/10.1002/jcd.20236), E.D. Schoen, P.T. Eendebak, M.V.M. Nguyen, Volume 18, Issue 2, pages 123-140, 2010
-        * [Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions](https://doi.org/10.1080/00401706.2016.1142903), Pieter T. Eendebak, Eric D. Schoen, Technometrics Vol. 59 , Iss. 1, 2017
-        * [A classification criterion for definitive screening designs](https://projecteuclid.org/euclid.aos/1547197252), E.D. Schoen, P.T. Eendebak, P. Goos, Ann. Statist. 47, no. 2, 2019.
-        
-        The code was written by:
-        
-        * Pieter Eendebak <pieter.eendebak@gmail.com>
-        * Alan Vazquez-Alcocer
-        * Vincent Brouerius van Nidek
-        
-        Ideas contributed by:
-        
-        * Eric Schoen <eric.schoen@tno.nl>
-        * Alan Vazquez-Alcocer <alanrvazquez@gmail.com>
-        
-        See the file LICENSE for copyright details.
-        
-        Installation
-        ------------
-        
-        [![PyPI version](https://badge.fury.io/py/OApackage.svg)](https://badge.fury.io/py/OApackage)
-        [![Build status](https://ci.appveyor.com/api/projects/status/f6ia9br95soimf9u/branch/master?svg=true)](https://ci.appveyor.com/project/eendebakpt/oapackage-4lws8)
-        [![Build Status](https://travis-ci.org/eendebakpt/oapackage.svg?branch=master)](https://travis-ci.org/eendebakpt/oapackage)
-        [![Documentation Status](https://readthedocs.org/projects/oapackage/badge/?version=latest)](https://oapackage.readthedocs.io/en/latest/?badge=latest)
-        
-        The Python interface to the package is available on the [Python Package index](https://pypi.python.org/pypi/OApackage/).
-        Installation can be done using the following command:
-        ``` console
-        $ pip install OApackage
-        ```
-        (or `pip install OApackage --user` if you do not have admin rights). To compile the package you need Python, Numpy and Swig 3.x.
-        
-        The command line tools have been tested using Linux, Windows XP/Win7/Win10 and Raspberry Pi.
-        The program uses a `cmake` build system. From the command line type:
-        ```
-        $ mkdir -p build; cd build
-        $ cmake ..
-        $ make
-        $ make install
-        ````
-        
-        Contributing, unit testing and support
-        --------------------------------------
-        
-        See the file [CONTRIBUTING.md](https://github.com/eendebakpt/oapackage/blob/master/CONTRIBUTING.md) on GitHub.
-        
 Keywords: orthogonal arrays, design of experiments, conference designs, isomorphism testing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Requires: numpy
 Requires: matplotlib
 Description-Content-Type: text/markdown
-Provides-Extra: GUI
 Provides-Extra: doc
+License-File: LICENSE
+
+Orthogonal Array Package
+========================
+
+The Orthogonal Array package contains functionality to generate and analyse orthogonal arrays, optimal designs and conference designs.
+Features include generation of complete series of orthogonal arrays,
+reduction of arrays to normal form and calculation of properties such as the strength or D-efficiency of an array.
+For more information about the package see the
+documentation at [oapackage.readthedocs.io](https://oapackage.readthedocs.io/en/latest/). A large collection of results generated
+with the package can be found at <http://pietereendebak.nl/oapackage/>.
+
+Usage
+-------
+
+The package can be used from Python:
+``` python
+>>> import oapackage
+>>> al=oapackage.exampleArray(0)
+>>> al.showarraycompact()
+00
+00
+01
+01
+10
+10
+11
+11
+>>> print('D-efficiency %f, rank %d' % (al.Defficiency(), al.rank()) )
+D-efficiency 1.000000, rank 2
+>>> print('Generalized wordlength pattern: %s' % str(al.GWLP()))
+Generalized wordlength pattern: (1.0, 0.0, 0.0)
+```
+
+For more examples see the Jupyter notebooks in the
+[docs/examples](docs/examples/).
+
+Acknowledgements
+----------------
+
+If you use this code or any of the results, please cite this program as follows:
+
+* [OApackage: A Python package for generation and analysis of orthogonal arrays, optimal designs and conference designs](https://doi.org/10.21105/joss.01097), P.T. Eendebak, A.R. Vazquez, Journal of Open Source Software, 2019
+* [Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays](https://doi.org/10.1002/jcd.20236), E.D. Schoen, P.T. Eendebak, M.V.M. Nguyen, Volume 18, Issue 2, pages 123-140, 2010
+* [Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions](https://doi.org/10.1080/00401706.2016.1142903), Pieter T. Eendebak, Eric D. Schoen, Technometrics Vol. 59 , Iss. 1, 2017
+* [A classification criterion for definitive screening designs](https://projecteuclid.org/euclid.aos/1547197252), E.D. Schoen, P.T. Eendebak, P. Goos, Ann. Statist. 47, no. 2, 2019.
+
+The code was written by:
+
+* Pieter Eendebak <pieter.eendebak@gmail.com>
+* Alan Vazquez-Alcocer
+* Vincent Brouerius van Nidek
+
+Ideas contributed by:
+
+* Eric Schoen <eric.schoen@tno.nl>
+* Alan Vazquez-Alcocer <alanrvazquez@gmail.com>
+
+See the file LICENSE for copyright details.
+
+Installation
+------------
+
+[![PyPI version](https://badge.fury.io/py/OApackage.svg)](https://badge.fury.io/py/OApackage)
+[![Build status](https://ci.appveyor.com/api/projects/status/f6ia9br95soimf9u/branch/master?svg=true)](https://ci.appveyor.com/project/eendebakpt/oapackage-4lws8)
+[![Build Status](https://travis-ci.org/eendebakpt/oapackage.svg?branch=master)](https://travis-ci.org/eendebakpt/oapackage)
+[![Documentation Status](https://readthedocs.org/projects/oapackage/badge/?version=latest)](https://oapackage.readthedocs.io/en/latest/?badge=latest)
+
+The Python interface to the package is available on the [Python Package index](https://pypi.python.org/pypi/OApackage/).
+Installation can be done using the following command:
+``` console
+$ pip install OApackage
+```
+(or `pip install OApackage --user` if you do not have admin rights). To compile the package you need Python, Numpy and Swig 3.x.
+
+The command line tools have been tested using Linux, Windows Win7/Win10 and Raspberry Pi.
+The program uses a `cmake` build system. From the command line type:
+```
+$ mkdir -p build; cd build
+$ cmake ..
+$ make
+$ make install
+````
+
+Contributing, unit testing and support
+--------------------------------------
+
+See the file [CONTRIBUTING.md](https://github.com/eendebakpt/oapackage/blob/master/CONTRIBUTING.md) on GitHub.
+
+
```

### Comparing `OApackage-2.7.6/OApackage.egg-info/SOURCES.txt` & `OApackage-2.7.7/OApackage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 doxy2swig.py
 numpy.i
 oaconfig.txt
 oadoxy.i
 oalib.i
 oalib.py
+pyproject.toml
 setup.cfg
 setup.py
 OApackage.egg-info/PKG-INFO
 OApackage.egg-info/SOURCES.txt
 OApackage.egg-info/dependency_links.txt
 OApackage.egg-info/not-zip-safe
 OApackage.egg-info/requires.txt
```

### Comparing `OApackage-2.7.6/PKG-INFO` & `OApackage-2.7.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,112 @@
 Metadata-Version: 2.1
 Name: OApackage
-Version: 2.7.6
+Version: 2.7.7
 Summary: Package to generate and analyse orthogonal arrays, conference designs and optimal designs
 Home-page: http://www.pietereendebak.nl/oapackage/index.html
 Author: Pieter Eendebak
 Author-email: pieter.eendebak@gmail.com
 License: BSD
-Description: Orthogonal Array Package
-        ========================
-        
-        The Orthogonal Array package contains functionality to generate and analyse orthogonal arrays, optimal designs and conference designs.
-        Features include generation of complete series of orthogonal arrays,
-        reduction of arrays to normal form and calculation of properties such as the strength or D-efficiency of an array.
-        For more information about the package see the
-        documentation at [oapackage.readthedocs.io](https://oapackage.readthedocs.io/en/latest/). A large collection of results generated
-        with the package can be found at <http://pietereendebak.nl/oapackage/>.
-        
-        Usage
-        -------
-        
-        The package can be used from Python:
-        ``` python
-        >>> import oapackage
-        >>> al=oapackage.exampleArray(0)
-        >>> al.showarraycompact()
-        00
-        00
-        01
-        01
-        10
-        10
-        11
-        11
-        >>> print('D-efficiency %f, rank %d' % (al.Defficiency(), al.rank()) )
-        D-efficiency 1.000000, rank 2
-        >>> print('Generalized wordlength pattern: %s' % str(al.GWLP()))
-        Generalized wordlength pattern: (1.0, 0.0, 0.0)
-        ```
-        
-        For more examples see the Jupyter notebooks in the
-        [docs/examples](docs/examples/).
-        
-        Acknowledgements
-        ----------------
-        
-        If you use this code or any of the results, please cite this program as follows:
-        
-        * [OApackage: A Python package for generation and analysis of orthogonal arrays, optimal designs and conference designs](https://doi.org/10.21105/joss.01097), P.T. Eendebak, A.R. Vazquez, Journal of Open Source Software, 2019
-        * [Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays](https://doi.org/10.1002/jcd.20236), E.D. Schoen, P.T. Eendebak, M.V.M. Nguyen, Volume 18, Issue 2, pages 123-140, 2010
-        * [Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions](https://doi.org/10.1080/00401706.2016.1142903), Pieter T. Eendebak, Eric D. Schoen, Technometrics Vol. 59 , Iss. 1, 2017
-        * [A classification criterion for definitive screening designs](https://projecteuclid.org/euclid.aos/1547197252), E.D. Schoen, P.T. Eendebak, P. Goos, Ann. Statist. 47, no. 2, 2019.
-        
-        The code was written by:
-        
-        * Pieter Eendebak <pieter.eendebak@gmail.com>
-        * Alan Vazquez-Alcocer
-        * Vincent Brouerius van Nidek
-        
-        Ideas contributed by:
-        
-        * Eric Schoen <eric.schoen@tno.nl>
-        * Alan Vazquez-Alcocer <alanrvazquez@gmail.com>
-        
-        See the file LICENSE for copyright details.
-        
-        Installation
-        ------------
-        
-        [![PyPI version](https://badge.fury.io/py/OApackage.svg)](https://badge.fury.io/py/OApackage)
-        [![Build status](https://ci.appveyor.com/api/projects/status/f6ia9br95soimf9u/branch/master?svg=true)](https://ci.appveyor.com/project/eendebakpt/oapackage-4lws8)
-        [![Build Status](https://travis-ci.org/eendebakpt/oapackage.svg?branch=master)](https://travis-ci.org/eendebakpt/oapackage)
-        [![Documentation Status](https://readthedocs.org/projects/oapackage/badge/?version=latest)](https://oapackage.readthedocs.io/en/latest/?badge=latest)
-        
-        The Python interface to the package is available on the [Python Package index](https://pypi.python.org/pypi/OApackage/).
-        Installation can be done using the following command:
-        ``` console
-        $ pip install OApackage
-        ```
-        (or `pip install OApackage --user` if you do not have admin rights). To compile the package you need Python, Numpy and Swig 3.x.
-        
-        The command line tools have been tested using Linux, Windows XP/Win7/Win10 and Raspberry Pi.
-        The program uses a `cmake` build system. From the command line type:
-        ```
-        $ mkdir -p build; cd build
-        $ cmake ..
-        $ make
-        $ make install
-        ````
-        
-        Contributing, unit testing and support
-        --------------------------------------
-        
-        See the file [CONTRIBUTING.md](https://github.com/eendebakpt/oapackage/blob/master/CONTRIBUTING.md) on GitHub.
-        
 Keywords: orthogonal arrays, design of experiments, conference designs, isomorphism testing
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Requires: numpy
 Requires: matplotlib
 Description-Content-Type: text/markdown
-Provides-Extra: GUI
 Provides-Extra: doc
+License-File: LICENSE
+
+Orthogonal Array Package
+========================
+
+The Orthogonal Array package contains functionality to generate and analyse orthogonal arrays, optimal designs and conference designs.
+Features include generation of complete series of orthogonal arrays,
+reduction of arrays to normal form and calculation of properties such as the strength or D-efficiency of an array.
+For more information about the package see the
+documentation at [oapackage.readthedocs.io](https://oapackage.readthedocs.io/en/latest/). A large collection of results generated
+with the package can be found at <http://pietereendebak.nl/oapackage/>.
+
+Usage
+-------
+
+The package can be used from Python:
+``` python
+>>> import oapackage
+>>> al=oapackage.exampleArray(0)
+>>> al.showarraycompact()
+00
+00
+01
+01
+10
+10
+11
+11
+>>> print('D-efficiency %f, rank %d' % (al.Defficiency(), al.rank()) )
+D-efficiency 1.000000, rank 2
+>>> print('Generalized wordlength pattern: %s' % str(al.GWLP()))
+Generalized wordlength pattern: (1.0, 0.0, 0.0)
+```
+
+For more examples see the Jupyter notebooks in the
+[docs/examples](docs/examples/).
+
+Acknowledgements
+----------------
+
+If you use this code or any of the results, please cite this program as follows:
+
+* [OApackage: A Python package for generation and analysis of orthogonal arrays, optimal designs and conference designs](https://doi.org/10.21105/joss.01097), P.T. Eendebak, A.R. Vazquez, Journal of Open Source Software, 2019
+* [Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays](https://doi.org/10.1002/jcd.20236), E.D. Schoen, P.T. Eendebak, M.V.M. Nguyen, Volume 18, Issue 2, pages 123-140, 2010
+* [Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions](https://doi.org/10.1080/00401706.2016.1142903), Pieter T. Eendebak, Eric D. Schoen, Technometrics Vol. 59 , Iss. 1, 2017
+* [A classification criterion for definitive screening designs](https://projecteuclid.org/euclid.aos/1547197252), E.D. Schoen, P.T. Eendebak, P. Goos, Ann. Statist. 47, no. 2, 2019.
+
+The code was written by:
+
+* Pieter Eendebak <pieter.eendebak@gmail.com>
+* Alan Vazquez-Alcocer
+* Vincent Brouerius van Nidek
+
+Ideas contributed by:
+
+* Eric Schoen <eric.schoen@tno.nl>
+* Alan Vazquez-Alcocer <alanrvazquez@gmail.com>
+
+See the file LICENSE for copyright details.
+
+Installation
+------------
+
+[![PyPI version](https://badge.fury.io/py/OApackage.svg)](https://badge.fury.io/py/OApackage)
+[![Build status](https://ci.appveyor.com/api/projects/status/f6ia9br95soimf9u/branch/master?svg=true)](https://ci.appveyor.com/project/eendebakpt/oapackage-4lws8)
+[![Build Status](https://travis-ci.org/eendebakpt/oapackage.svg?branch=master)](https://travis-ci.org/eendebakpt/oapackage)
+[![Documentation Status](https://readthedocs.org/projects/oapackage/badge/?version=latest)](https://oapackage.readthedocs.io/en/latest/?badge=latest)
+
+The Python interface to the package is available on the [Python Package index](https://pypi.python.org/pypi/OApackage/).
+Installation can be done using the following command:
+``` console
+$ pip install OApackage
+```
+(or `pip install OApackage --user` if you do not have admin rights). To compile the package you need Python, Numpy and Swig 3.x.
+
+The command line tools have been tested using Linux, Windows Win7/Win10 and Raspberry Pi.
+The program uses a `cmake` build system. From the command line type:
+```
+$ mkdir -p build; cd build
+$ cmake ..
+$ make
+$ make install
+````
+
+Contributing, unit testing and support
+--------------------------------------
+
+See the file [CONTRIBUTING.md](https://github.com/eendebakpt/oapackage/blob/master/CONTRIBUTING.md) on GitHub.
+
+
```

### Comparing `OApackage-2.7.6/README.md` & `OApackage-2.7.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 The Python interface to the package is available on the [Python Package index](https://pypi.python.org/pypi/OApackage/).
 Installation can be done using the following command:
 ``` console
 $ pip install OApackage
 ```
 (or `pip install OApackage --user` if you do not have admin rights). To compile the package you need Python, Numpy and Swig 3.x.
 
-The command line tools have been tested using Linux, Windows XP/Win7/Win10 and Raspberry Pi.
+The command line tools have been tested using Linux, Windows Win7/Win10 and Raspberry Pi.
 The program uses a `cmake` build system. From the command line type:
 ```
 $ mkdir -p build; cd build
 $ cmake ..
 $ make
 $ make install
 ````
```

### Comparing `OApackage-2.7.6/doxy2swig.py` & `OApackage-2.7.7/doxy2swig.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/misc/scripts/example_oapackage_python.py` & `OApackage-2.7.7/misc/scripts/example_oapackage_python.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/numpy.i` & `OApackage-2.7.7/numpy.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/oadoxy.i` & `OApackage-2.7.7/oadoxy.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/oalib.i` & `OApackage-2.7.7/oalib.i`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/oalib.py` & `OApackage-2.7.7/oalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# This file was automatically generated by SWIG (http://www.swig.org).
-# Version 4.0.2
+# This file was automatically generated by SWIG (https://www.swig.org).
+# Version 4.1.1
 #
-# Do not make changes to this file unless you know what you are doing--modify
+# Do not make changes to this file unless you know what you are doing - modify
 # the SWIG interface file instead.
 
 """Python Orthogonal Array interface"""
 
 from sys import version_info as _swig_python_version_info
-if _swig_python_version_info < (2, 7, 0):
-    raise RuntimeError("Python 2.7 or later required")
-
 # Import the low-level C/C++ module
 if __package__ or "." in __name__:
     from . import _oalib
 else:
     import _oalib
 
 try:
@@ -27,18 +24,18 @@
     except __builtin__.Exception:
         strthis = ""
     return "<%s.%s; %s >" % (self.__class__.__module__, self.__class__.__name__, strthis,)
 
 
 def _swig_setattr_nondynamic_instance_variable(set):
     def set_instance_attr(self, name, value):
-        if name == "thisown":
-            self.this.own(value)
-        elif name == "this":
+        if name == "this":
             set(self, name, value)
+        elif name == "thisown":
+            self.this.own(value)
         elif hasattr(self, name) and isinstance(getattr(type(self), name), property):
             set(self, name, value)
         else:
             raise AttributeError("You cannot add instance attributes to %s" % self)
     return set_instance_attr
 
 
@@ -120,15 +117,14 @@
         return _oalib.SwigPyIterator___sub__(self, *args)
     def __iter__(self):
         return self
 
 # Register SwigPyIterator in _oalib:
 _oalib.SwigPyIterator_swigregister(SwigPyIterator)
 
-
 import sys
 import numpy as np
 import copy
 from typing import Optional, List
 
 def reduceGraphNauty(G, colors : Optional[List] = None, verbose : int = 1) -> List:
   """ Return vertex transformation reducing array to normal form
@@ -210,29 +206,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(arraylist_t self, std::deque< array_link >::difference_type i, std::deque< array_link >::difference_type j)"""
         return _oalib.arraylist_t___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(arraylist_t self, std::deque< array_link >::difference_type i)
-        __delitem__(arraylist_t self, PySliceObject * slice)
+        __delitem__(arraylist_t self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.arraylist_t___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(arraylist_t self, PySliceObject * slice) -> arraylist_t
+        __getitem__(arraylist_t self, SWIGPY_SLICEOBJECT * slice) -> arraylist_t
         __getitem__(arraylist_t self, std::deque< array_link >::difference_type i) -> array_link
         """
         return _oalib.arraylist_t___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(arraylist_t self, PySliceObject * slice, arraylist_t v)
-        __setitem__(arraylist_t self, PySliceObject * slice)
+        __setitem__(arraylist_t self, SWIGPY_SLICEOBJECT * slice, arraylist_t v)
+        __setitem__(arraylist_t self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(arraylist_t self, std::deque< array_link >::difference_type i, array_link x)
         """
         return _oalib.arraylist_t___setitem__(self, *args)
 
     def pop(self):
         r"""pop(arraylist_t self) -> array_link"""
         return _oalib.arraylist_t_pop(self)
@@ -338,15 +334,14 @@
     def __repr__(self):
         r"""__repr__(arraylist_t self) -> std::string"""
         return _oalib.arraylist_t___repr__(self)
     __swig_destroy__ = _oalib.delete_arraylist_t
 
 # Register arraylist_t in _oalib:
 _oalib.arraylist_t_swigregister(arraylist_t)
-
 class jstructArray(object):
     r"""Proxy of C++ std::vector< jstruct_t > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -381,29 +376,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(jstructArray self, std::vector< jstruct_t >::difference_type i, std::vector< jstruct_t >::difference_type j)"""
         return _oalib.jstructArray___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(jstructArray self, std::vector< jstruct_t >::difference_type i)
-        __delitem__(jstructArray self, PySliceObject * slice)
+        __delitem__(jstructArray self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.jstructArray___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(jstructArray self, PySliceObject * slice) -> jstructArray
+        __getitem__(jstructArray self, SWIGPY_SLICEOBJECT * slice) -> jstructArray
         __getitem__(jstructArray self, std::vector< jstruct_t >::difference_type i) -> jstruct_t
         """
         return _oalib.jstructArray___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(jstructArray self, PySliceObject * slice, jstructArray v)
-        __setitem__(jstructArray self, PySliceObject * slice)
+        __setitem__(jstructArray self, SWIGPY_SLICEOBJECT * slice, jstructArray v)
+        __setitem__(jstructArray self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(jstructArray self, std::vector< jstruct_t >::difference_type i, jstruct_t x)
         """
         return _oalib.jstructArray___setitem__(self, *args)
 
     def pop(self):
         r"""pop(jstructArray self) -> jstruct_t"""
         return _oalib.jstructArray_pop(self)
@@ -505,15 +500,14 @@
     def capacity(self):
         r"""capacity(jstructArray self) -> std::vector< jstruct_t >::size_type"""
         return _oalib.jstructArray_capacity(self)
     __swig_destroy__ = _oalib.delete_jstructArray
 
 # Register jstructArray in _oalib:
 _oalib.jstructArray_swigregister(jstructArray)
-
 class uint8Vector(object):
     r"""Proxy of C++ std::vector< unsigned char > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -548,29 +542,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(uint8Vector self, std::vector< unsigned char >::difference_type i, std::vector< unsigned char >::difference_type j)"""
         return _oalib.uint8Vector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(uint8Vector self, std::vector< unsigned char >::difference_type i)
-        __delitem__(uint8Vector self, PySliceObject * slice)
+        __delitem__(uint8Vector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.uint8Vector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(uint8Vector self, PySliceObject * slice) -> uint8Vector
+        __getitem__(uint8Vector self, SWIGPY_SLICEOBJECT * slice) -> uint8Vector
         __getitem__(uint8Vector self, std::vector< unsigned char >::difference_type i) -> std::vector< unsigned char >::value_type const &
         """
         return _oalib.uint8Vector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(uint8Vector self, PySliceObject * slice, uint8Vector v)
-        __setitem__(uint8Vector self, PySliceObject * slice)
+        __setitem__(uint8Vector self, SWIGPY_SLICEOBJECT * slice, uint8Vector v)
+        __setitem__(uint8Vector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(uint8Vector self, std::vector< unsigned char >::difference_type i, std::vector< unsigned char >::value_type const & x)
         """
         return _oalib.uint8Vector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(uint8Vector self) -> std::vector< unsigned char >::value_type"""
         return _oalib.uint8Vector_pop(self)
@@ -672,15 +666,14 @@
     def capacity(self):
         r"""capacity(uint8Vector self) -> std::vector< unsigned char >::size_type"""
         return _oalib.uint8Vector_capacity(self)
     __swig_destroy__ = _oalib.delete_uint8Vector
 
 # Register uint8Vector in _oalib:
 _oalib.uint8Vector_swigregister(uint8Vector)
-
 class charVector(object):
     r"""Proxy of C++ std::vector< signed char > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -715,29 +708,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(charVector self, std::vector< signed char >::difference_type i, std::vector< signed char >::difference_type j)"""
         return _oalib.charVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(charVector self, std::vector< signed char >::difference_type i)
-        __delitem__(charVector self, PySliceObject * slice)
+        __delitem__(charVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.charVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(charVector self, PySliceObject * slice) -> charVector
+        __getitem__(charVector self, SWIGPY_SLICEOBJECT * slice) -> charVector
         __getitem__(charVector self, std::vector< signed char >::difference_type i) -> std::vector< signed char >::value_type const &
         """
         return _oalib.charVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(charVector self, PySliceObject * slice, charVector v)
-        __setitem__(charVector self, PySliceObject * slice)
+        __setitem__(charVector self, SWIGPY_SLICEOBJECT * slice, charVector v)
+        __setitem__(charVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(charVector self, std::vector< signed char >::difference_type i, std::vector< signed char >::value_type const & x)
         """
         return _oalib.charVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(charVector self) -> std::vector< signed char >::value_type"""
         return _oalib.charVector_pop(self)
@@ -839,15 +832,14 @@
     def capacity(self):
         r"""capacity(charVector self) -> std::vector< signed char >::size_type"""
         return _oalib.charVector_capacity(self)
     __swig_destroy__ = _oalib.delete_charVector
 
 # Register charVector in _oalib:
 _oalib.charVector_swigregister(charVector)
-
 class intVector(object):
     r"""Proxy of C++ std::vector< int > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -882,29 +874,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(intVector self, std::vector< int >::difference_type i, std::vector< int >::difference_type j)"""
         return _oalib.intVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(intVector self, std::vector< int >::difference_type i)
-        __delitem__(intVector self, PySliceObject * slice)
+        __delitem__(intVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.intVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(intVector self, PySliceObject * slice) -> intVector
+        __getitem__(intVector self, SWIGPY_SLICEOBJECT * slice) -> intVector
         __getitem__(intVector self, std::vector< int >::difference_type i) -> std::vector< int >::value_type const &
         """
         return _oalib.intVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(intVector self, PySliceObject * slice, intVector v)
-        __setitem__(intVector self, PySliceObject * slice)
+        __setitem__(intVector self, SWIGPY_SLICEOBJECT * slice, intVector v)
+        __setitem__(intVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(intVector self, std::vector< int >::difference_type i, std::vector< int >::value_type const & x)
         """
         return _oalib.intVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(intVector self) -> std::vector< int >::value_type"""
         return _oalib.intVector_pop(self)
@@ -1006,15 +998,14 @@
     def capacity(self):
         r"""capacity(intVector self) -> std::vector< int >::size_type"""
         return _oalib.intVector_capacity(self)
     __swig_destroy__ = _oalib.delete_intVector
 
 # Register intVector in _oalib:
 _oalib.intVector_swigregister(intVector)
-
 class longVector(object):
     r"""Proxy of C++ std::vector< long > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -1049,29 +1040,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(longVector self, std::vector< long >::difference_type i, std::vector< long >::difference_type j)"""
         return _oalib.longVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(longVector self, std::vector< long >::difference_type i)
-        __delitem__(longVector self, PySliceObject * slice)
+        __delitem__(longVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.longVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(longVector self, PySliceObject * slice) -> longVector
+        __getitem__(longVector self, SWIGPY_SLICEOBJECT * slice) -> longVector
         __getitem__(longVector self, std::vector< long >::difference_type i) -> std::vector< long >::value_type const &
         """
         return _oalib.longVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(longVector self, PySliceObject * slice, longVector v)
-        __setitem__(longVector self, PySliceObject * slice)
+        __setitem__(longVector self, SWIGPY_SLICEOBJECT * slice, longVector v)
+        __setitem__(longVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(longVector self, std::vector< long >::difference_type i, std::vector< long >::value_type const & x)
         """
         return _oalib.longVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(longVector self) -> std::vector< long >::value_type"""
         return _oalib.longVector_pop(self)
@@ -1173,15 +1164,14 @@
     def capacity(self):
         r"""capacity(longVector self) -> std::vector< long >::size_type"""
         return _oalib.longVector_capacity(self)
     __swig_destroy__ = _oalib.delete_longVector
 
 # Register longVector in _oalib:
 _oalib.longVector_swigregister(longVector)
-
 class longDeque(object):
     r"""Proxy of C++ std::deque< long > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -1216,29 +1206,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(longDeque self, std::deque< long >::difference_type i, std::deque< long >::difference_type j)"""
         return _oalib.longDeque___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(longDeque self, std::deque< long >::difference_type i)
-        __delitem__(longDeque self, PySliceObject * slice)
+        __delitem__(longDeque self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.longDeque___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(longDeque self, PySliceObject * slice) -> longDeque
+        __getitem__(longDeque self, SWIGPY_SLICEOBJECT * slice) -> longDeque
         __getitem__(longDeque self, std::deque< long >::difference_type i) -> std::deque< long >::value_type const &
         """
         return _oalib.longDeque___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(longDeque self, PySliceObject * slice, longDeque v)
-        __setitem__(longDeque self, PySliceObject * slice)
+        __setitem__(longDeque self, SWIGPY_SLICEOBJECT * slice, longDeque v)
+        __setitem__(longDeque self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(longDeque self, std::deque< long >::difference_type i, std::deque< long >::value_type const & x)
         """
         return _oalib.longDeque___setitem__(self, *args)
 
     def pop(self):
         r"""pop(longDeque self) -> std::deque< long >::value_type"""
         return _oalib.longDeque_pop(self)
@@ -1340,15 +1330,14 @@
     def push_front(self, x):
         r"""push_front(longDeque self, std::deque< long >::value_type const & x)"""
         return _oalib.longDeque_push_front(self, x)
     __swig_destroy__ = _oalib.delete_longDeque
 
 # Register longDeque in _oalib:
 _oalib.longDeque_swigregister(longDeque)
-
 class doubleVector(object):
     r"""Proxy of C++ std::vector< double > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -1383,29 +1372,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(doubleVector self, std::vector< double >::difference_type i, std::vector< double >::difference_type j)"""
         return _oalib.doubleVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(doubleVector self, std::vector< double >::difference_type i)
-        __delitem__(doubleVector self, PySliceObject * slice)
+        __delitem__(doubleVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.doubleVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(doubleVector self, PySliceObject * slice) -> doubleVector
+        __getitem__(doubleVector self, SWIGPY_SLICEOBJECT * slice) -> doubleVector
         __getitem__(doubleVector self, std::vector< double >::difference_type i) -> std::vector< double >::value_type const &
         """
         return _oalib.doubleVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(doubleVector self, PySliceObject * slice, doubleVector v)
-        __setitem__(doubleVector self, PySliceObject * slice)
+        __setitem__(doubleVector self, SWIGPY_SLICEOBJECT * slice, doubleVector v)
+        __setitem__(doubleVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(doubleVector self, std::vector< double >::difference_type i, std::vector< double >::value_type const & x)
         """
         return _oalib.doubleVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(doubleVector self) -> std::vector< double >::value_type"""
         return _oalib.doubleVector_pop(self)
@@ -1507,15 +1496,14 @@
     def capacity(self):
         r"""capacity(doubleVector self) -> std::vector< double >::size_type"""
         return _oalib.doubleVector_capacity(self)
     __swig_destroy__ = _oalib.delete_doubleVector
 
 # Register doubleVector in _oalib:
 _oalib.doubleVector_swigregister(doubleVector)
-
 class stringVector(object):
     r"""Proxy of C++ std::vector< std::string > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -1550,29 +1538,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(stringVector self, std::vector< std::string >::difference_type i, std::vector< std::string >::difference_type j)"""
         return _oalib.stringVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(stringVector self, std::vector< std::string >::difference_type i)
-        __delitem__(stringVector self, PySliceObject * slice)
+        __delitem__(stringVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.stringVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(stringVector self, PySliceObject * slice) -> stringVector
+        __getitem__(stringVector self, SWIGPY_SLICEOBJECT * slice) -> stringVector
         __getitem__(stringVector self, std::vector< std::string >::difference_type i) -> std::vector< std::string >::value_type const &
         """
         return _oalib.stringVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(stringVector self, PySliceObject * slice, stringVector v)
-        __setitem__(stringVector self, PySliceObject * slice)
+        __setitem__(stringVector self, SWIGPY_SLICEOBJECT * slice, stringVector v)
+        __setitem__(stringVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(stringVector self, std::vector< std::string >::difference_type i, std::vector< std::string >::value_type const & x)
         """
         return _oalib.stringVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(stringVector self) -> std::vector< std::string >::value_type"""
         return _oalib.stringVector_pop(self)
@@ -1674,15 +1662,14 @@
     def capacity(self):
         r"""capacity(stringVector self) -> std::vector< std::string >::size_type"""
         return _oalib.stringVector_capacity(self)
     __swig_destroy__ = _oalib.delete_stringVector
 
 # Register stringVector in _oalib:
 _oalib.stringVector_swigregister(stringVector)
-
 class map_int_long(object):
     r"""Proxy of C++ std::map< int,long > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -1826,15 +1813,14 @@
         r"""upper_bound(map_int_long self, std::map< int,long >::key_type const & x) -> std::map< int,long >::iterator"""
         return _oalib.map_int_long_upper_bound(self, x)
     __swig_destroy__ = _oalib.delete_map_int_long
 
 # Register map_int_long in _oalib:
 _oalib.map_int_long_swigregister(map_int_long)
 
-
 import numpy
 
 MAXCOLS = _oalib.MAXCOLS
 
 MAXROWS = _oalib.MAXROWS
 
 OACHECK = _oalib.OACHECK
@@ -1977,48 +1963,14 @@
 
         """
         _oalib.Combinations_swiginit(self, _oalib.new_Combinations())
 
 # Register Combinations in _oalib:
 _oalib.Combinations_swigregister(Combinations)
 
-def Combinations_number_combinations_max_n():
-    r"""
-    Combinations_number_combinations_max_n() -> int
-
-
-    return max number of N that can be calculated with number_combinations
-
-    """
-    return _oalib.Combinations_number_combinations_max_n()
-
-def Combinations_initialize_number_combinations(N):
-    r"""
-    Combinations_initialize_number_combinations(int N)
-
-
-    initialize datastructure for number_combinations, this function is not thread
-    safe
-
-    """
-    return _oalib.Combinations_initialize_number_combinations(N)
-
-def Combinations_number_combinations(n, k):
-    r"""
-    Combinations_number_combinations(int n, int k) -> long
-
-
-    Return number of combinations from previously calculated results
-
-    The results should be initialized with initialize_number_combinations
-
-    """
-    return _oalib.Combinations_number_combinations(n, k)
-
-
 def fastrand():
     r"""
     fastrand() -> int
 
 
     """
     return _oalib.fastrand()
@@ -2120,15 +2072,14 @@
 
         """
         return _oalib.indexsort_issorteddescending(self)
     __swig_destroy__ = _oalib.delete_indexsort
 
 # Register indexsort in _oalib:
 _oalib.indexsort_swigregister(indexsort)
-
 class symmetry_group(object):
     r"""
 
     `symmetry_group(vals, ascending=true, verbose=0)`
     `symmetry_group(vals, ascending=true, verbose=0)`
     `symmetry_group(vals, ascending=true, verbose=0)`
     `symmetry_group(vals, ascending=true, verbose=0)`
@@ -2188,19 +2139,19 @@
 
     C++ includes: mathtools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     gidx = property(_oalib.symmetry_group_gidx_get, _oalib.symmetry_group_gidx_set, doc=r"""gidx : std::vector<(int,std::allocator<(int)>)>""")
-    gstart = property(_oalib.symmetry_group_gstart_get, _oalib.symmetry_group_gstart_set, doc=r"""gstart : std::vector<(int,std::allocator<(int)>)>""")
-    gsize = property(_oalib.symmetry_group_gsize_get, _oalib.symmetry_group_gsize_set, doc=r"""gsize : std::vector<(int,std::allocator<(int)>)>""")
-    ngroups = property(_oalib.symmetry_group_ngroups_get, _oalib.symmetry_group_ngroups_set, doc=r"""ngroups : int""")
-    n = property(_oalib.symmetry_group_n_get, _oalib.symmetry_group_n_set, doc=r"""n : int""")
-    ascending = property(_oalib.symmetry_group_ascending_get, _oalib.symmetry_group_ascending_set, doc=r"""ascending : bool""")
+    gstart = property(_oalib.symmetry_group_gstart_get, _oalib.symmetry_group_gstart_set, doc=r""" start of the subgroups""")
+    gsize = property(_oalib.symmetry_group_gsize_get, _oalib.symmetry_group_gsize_set, doc=r""" size of the subgroups""")
+    ngroups = property(_oalib.symmetry_group_ngroups_get, _oalib.symmetry_group_ngroups_set, doc=r""" number of subgroups""")
+    n = property(_oalib.symmetry_group_n_get, _oalib.symmetry_group_n_set, doc=r""" number of elements""")
+    ascending = property(_oalib.symmetry_group_ascending_get, _oalib.symmetry_group_ascending_set, doc=r""" ordering of elements""")
 
     def __init__(self, *args):
         r"""
         __init__(symmetry_group self, intVector vals, bool ascending=True, int verbose=0) -> symmetry_group
         __init__(symmetry_group self, doubleVector vals, bool ascending=True, int verbose=0) -> symmetry_group
         __init__(symmetry_group self, std::vector< float,std::allocator< float > > const & vals, bool ascending=True, int verbose=0) -> symmetry_group
         __init__(symmetry_group self, std::vector< short,std::allocator< short > > const & vals, bool ascending=True, int verbose=0) -> symmetry_group
@@ -2267,15 +2218,14 @@
 
         """
         return _oalib.symmetry_group_show(self, verbose)
     __swig_destroy__ = _oalib.delete_symmetry_group
 
 # Register symmetry_group in _oalib:
 _oalib.symmetry_group_swigregister(symmetry_group)
-
 class symmetry_group_walker(object):
     r"""
 
     `symmetry_group_walker(sg)`
 
     Class to walk over all elements of a symmetry group
 
@@ -2295,16 +2245,16 @@
 
     C++ includes: mathtools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    sg = property(_oalib.symmetry_group_walker_sg_get, _oalib.symmetry_group_walker_sg_set, doc=r"""sg : symmetry_group""")
-    perms = property(_oalib.symmetry_group_walker_perms_get, _oalib.symmetry_group_walker_perms_set, doc=r"""perms : std::vector<(std::vector<(int,std::allocator<(int)>)>,std::allocator<(std::vector<(int,std::allocator<(int)>)>)>)>""")
+    sg = property(_oalib.symmetry_group_walker_sg_get, _oalib.symmetry_group_walker_sg_set, doc=r""" symmetry group""")
+    perms = property(_oalib.symmetry_group_walker_perms_get, _oalib.symmetry_group_walker_perms_set, doc=r""" current element of the symmetry group""")
 
     def __init__(self, sg):
         r"""
         __init__(symmetry_group_walker self, symmetry_group sg) -> symmetry_group_walker
 
 
         """
@@ -2341,15 +2291,14 @@
         """
         return _oalib.symmetry_group_walker_fullperm(self)
     __swig_destroy__ = _oalib.delete_symmetry_group_walker
 
 # Register symmetry_group_walker in _oalib:
 _oalib.symmetry_group_walker_swigregister(symmetry_group_walker)
 
-
 def ipow(*args):
     r"""
     ipow(long x, long y) -> long
     ipow(unsigned int x, unsigned int p) -> unsigned int
 
 
     Power of two unsigned integers.
@@ -2377,48 +2326,67 @@
 
     This exception is caught in the SWIG interface.
 
     """
     return _oalib.throw_runtime_exception(exception_message)
 
 def eigenInfo(*args):
-    r"""eigenInfo(MatrixFloat const m, char const * str="eigen", int verbose=1)"""
+    r"""
+     Print information about an Eigen matrix
+
+    :type m: MatrixFloat
+    :param m: Matrix about which to print information
+    :type str: string, optional
+    :param str: String to prepend in output
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    """
     return _oalib.eigenInfo(*args)
 
 def print_eigen_matrix(matrix):
-    r"""print_eigen_matrix(MatrixFloat const matrix)"""
+    r""" Print Eigen matrix to stdout"""
     return _oalib.print_eigen_matrix(matrix)
 
 def eigen2numpyHelper(pymat1, n, m):
     r"""eigen2numpyHelper(double * pymat1, int n, MatrixFloat const & m)"""
     return _oalib.eigen2numpyHelper(pymat1, n, m)
 
 def sizeof_array_t():
-    r"""sizeof_array_t() -> int"""
+    r""" return size in bytes of array_t type"""
     return _oalib.sizeof_array_t()
 
 def sizeof_double():
-    r"""sizeof_double() -> int"""
+    r""" return size in bytes of double type"""
     return _oalib.sizeof_double()
 
 def possible_F_values(N, strength):
-    r"""possible_F_values(int N, int strength) -> intVector"""
+    r""" possible values for J-values of 2-level design"""
     return _oalib.possible_F_values(N, strength)
 
 def file_exists(*args):
     r"""
-    file_exists(std::string const filename) -> bool
-    file_exists(char const * filename) -> bool
+    *Overload 1:*
+    return true if the specified file exists
+
+    |
+
+    *Overload 2:*
+    return true if the specified file exists
     """
     return _oalib.file_exists(*args)
 
 def oa_file_exists(*args):
     r"""
-    oa_file_exists(char const * filename) -> bool
-    oa_file_exists(std::string const filename) -> bool
+    *Overload 1:*
+    return true if the specified oa file exists
+
+    |
+
+    *Overload 2:*
+    return true if the specified oa file exists
     """
     return _oalib.oa_file_exists(*args)
 ORDER_LEX = _oalib.ORDER_LEX
 r""" lexicograph minimal by columns ordering"""
 ORDER_J5 = _oalib.ORDER_J5
 r""" J5 based ordering"""
 class arraydata_t(object):
@@ -2560,23 +2528,23 @@
         index of the array
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    N = property(_oalib.arraydata_t_N_get, _oalib.arraydata_t_N_set, doc=r"""N : rowindex_t""")
-    ncols = property(_oalib.arraydata_t_ncols_get, _oalib.arraydata_t_ncols_set, doc=r"""ncols : colindex_t""")
-    strength = property(_oalib.arraydata_t_strength_get, _oalib.arraydata_t_strength_set, doc=r"""strength : colindex_t""")
-    s = property(_oalib.arraydata_t_s_get, _oalib.arraydata_t_s_set, doc=r"""s : p.array_t""")
-    order = property(_oalib.arraydata_t_order_get, _oalib.arraydata_t_order_set, doc=r"""order : ordering_t""")
-    ncolgroups = property(_oalib.arraydata_t_ncolgroups_get, _oalib.arraydata_t_ncolgroups_set, doc=r"""ncolgroups : colindex_t""")
-    colgroupindex = property(_oalib.arraydata_t_colgroupindex_get, _oalib.arraydata_t_colgroupindex_set, doc=r"""colgroupindex : p.colindex_t""")
-    colgroupsize = property(_oalib.arraydata_t_colgroupsize_get, _oalib.arraydata_t_colgroupsize_set, doc=r"""colgroupsize : p.colindex_t""")
-    oaindex = property(_oalib.arraydata_t_oaindex_get, _oalib.arraydata_t_oaindex_set, doc=r"""oaindex : int""")
+    N = property(_oalib.arraydata_t_N_get, _oalib.arraydata_t_N_set, doc=r""" number of runs""")
+    ncols = property(_oalib.arraydata_t_ncols_get, _oalib.arraydata_t_ncols_set, doc=r""" total number of columns (factors) in the design""")
+    strength = property(_oalib.arraydata_t_strength_get, _oalib.arraydata_t_strength_set, doc=r""" strength of the design""")
+    s = property(_oalib.arraydata_t_s_get, _oalib.arraydata_t_s_set, doc=r""" pointer to factor levels of the array""")
+    order = property(_oalib.arraydata_t_order_get, _oalib.arraydata_t_order_set, doc=r""" Ordering used for arrays""")
+    ncolgroups = property(_oalib.arraydata_t_ncolgroups_get, _oalib.arraydata_t_ncolgroups_set, doc=r""" number of groups of columns with the same number of levels""")
+    colgroupindex = property(_oalib.arraydata_t_colgroupindex_get, _oalib.arraydata_t_colgroupindex_set, doc=r""" specifies for each column the index of the column group""")
+    colgroupsize = property(_oalib.arraydata_t_colgroupsize_get, _oalib.arraydata_t_colgroupsize_set, doc=r""" specifies for each column the size of the column group""")
+    oaindex = property(_oalib.arraydata_t_oaindex_get, _oalib.arraydata_t_oaindex_set, doc=r""" index of the array""")
 
     def __init__(self, *args):
         r"""
         __init__(arraydata_t self) -> arraydata_t
         __init__(arraydata_t self, array_t s, rowindex_t N, colindex_t strength, colindex_t ncols) -> arraydata_t
         __init__(arraydata_t self, intVector s, rowindex_t N, colindex_t strength, colindex_t ncols) -> arraydata_t
         __init__(arraydata_t self, array_t const * s_, rowindex_t N, colindex_t strength, colindex_t ncols) -> arraydata_t
@@ -2749,15 +2717,15 @@
 
         set column group equal to that of a symmetry group
 
         """
         return _oalib.arraydata_t_set_colgroups(self, *args)
 
     def get_column_groups_sizes(self):
-        r"""get_column_groups_sizes(arraydata_t self) -> intVector"""
+        r""" return sizes of the column groups"""
         return _oalib.arraydata_t_get_column_groups_sizes(self)
 
     def show_colgroups(self):
         r"""
         show_colgroups(arraydata_t self)
 
 
@@ -2814,15 +2782,15 @@
 
         return factor levels
 
         """
         return _oalib.arraydata_t_factor_levels(self)
 
     def factor_levels_column_groups(self):
-        r"""factor_levels_column_groups(arraydata_t self) -> intVector"""
+        r""" return factor levels for the column groups"""
         return _oalib.arraydata_t_factor_levels_column_groups(self)
 
     def reset_strength(self, strength):
         r"""
         reset_strength(arraydata_t self, colindex_t strength)
 
 
@@ -2859,36 +2827,54 @@
     def __repr__(self):
         r"""__repr__(arraydata_t self) -> std::string"""
         return _oalib.arraydata_t___repr__(self)
 
 # Register arraydata_t in _oalib:
 _oalib.arraydata_t_swigregister(arraydata_t)
 
-
 def readConfigFile(file):
-    r"""readConfigFile(char const * file) -> arraydata_t"""
+    r""" Read array configuration from file"""
     return _oalib.readConfigFile(file)
 
 def copy_array(src, dst, nrows, ncols):
-    r"""copy_array(array_t const * src, array_t *const dst, int const nrows, int const ncols)"""
+    r"""Make a copy of an array"""
     return _oalib.copy_array(src, dst, nrows, ncols)
 
 def destroy_array(array):
-    r"""destroy_array(array_t * array) -> int"""
+    r"""
+    Delete an array
+    :type array: int
+    :param array:
+    :rtype: int
+    :return: 
+    """
     return _oalib.destroy_array(array)
 
 def create_array(*args):
     r"""
-    create_array(int const nrows, int const ncols) -> array_t
-    create_array(arraydata_t ad) -> array_t *
+    *Overload 1:*
+
+    Create an array
+    :type nrows: int
+    :param nrows: Number of rows
+    :type ncols: int
+    :param ncols: Number of columns
+    :rtype: int
+    :return: 
+
+    |
+
+    *Overload 2:*
+
+    Create an array from an arraydata_t structure
     """
     return _oalib.create_array(*args)
 
 def clone_array(array, nrows, ncols):
-    r"""clone_array(array_t const *const array, rowindex_t const nrows, colindex_t const ncols) -> array_t *"""
+    r"""Clone an array"""
     return _oalib.clone_array(array, nrows, ncols)
 class array_link(object):
     r"""
 
     `array_link()`
     `array_link(nrows, ncols, index)`
     `array_link(nrows, ncols, index, data)`
@@ -2984,18 +2970,18 @@
     * `INDEX_DEFAULT` : `const int`
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    n_rows = property(_oalib.array_link_n_rows_get, _oalib.array_link_n_rows_set, doc=r"""n_rows : rowindex_t""")
-    n_columns = property(_oalib.array_link_n_columns_get, _oalib.array_link_n_columns_set, doc=r"""n_columns : colindex_t""")
-    index = property(_oalib.array_link_index_get, _oalib.array_link_index_set, doc=r"""index : int""")
-    array = property(_oalib.array_link_array_get, _oalib.array_link_array_set, doc=r"""array : p.array_t""")
+    n_rows = property(_oalib.array_link_n_rows_get, _oalib.array_link_n_rows_set, doc=r""" Number of rows in array""")
+    n_columns = property(_oalib.array_link_n_columns_get, _oalib.array_link_n_columns_set, doc=r""" Number of columns in array""")
+    index = property(_oalib.array_link_index_get, _oalib.array_link_index_set, doc=r""" Index number""")
+    array = property(_oalib.array_link_array_get, _oalib.array_link_array_set, doc=r""" Pointer to array data""")
     INDEX_NONE = _oalib.array_link_INDEX_NONE
     
     INDEX_ERROR = _oalib.array_link_INDEX_ERROR
     
     INDEX_DEFAULT = _oalib.array_link_INDEX_DEFAULT
     
     __swig_destroy__ = _oalib.delete_array_link
@@ -3472,15 +3458,22 @@
         shallowcopy(array_link self, array_link rhs) -> array_link
 
 
         """
         return _oalib.array_link_shallowcopy(self, rhs)
 
     def __eq__(self, rhs):
-        r"""__eq__(array_link self, array_link rhs) -> int"""
+        r"""
+         Return True if both arrays are equal
+
+        :type rhs: :py:class:`array_link`
+        :param rhs: Array to compare to
+        :rtype: int
+        :return: 1 if arrays are equal. 0 otherwise. Returns 0 if arrays have different sizes
+        """
         return _oalib.array_link___eq__(self, rhs)
 
     def __ne__(self, rhs):
         r"""__ne__(array_link self, array_link rhs) -> int"""
         return _oalib.array_link___ne__(self, rhs)
 
     def __lt__(self, rhs):
@@ -3499,16 +3492,21 @@
         return true of two array have the same dimensions
 
         """
         return _oalib.array_link_equalsize(self, rhs)
 
     def __add__(self, *args):
         r"""
-        __add__(array_link self, array_link arg2) -> array_link
-        __add__(array_link self, array_t value) -> array_link
+        *Overload 1:*
+        elementwise addition
+
+        |
+
+        *Overload 2:*
+        elementwise addition
         """
         return _oalib.array_link___add__(self, *args)
 
     def __sub__(self, *args):
         r"""
         __sub__(array_link self, array_link arg2) -> array_link
         __sub__(array_link self, array_t value) -> array_link
@@ -3934,68 +3932,99 @@
     def __repr__(self):
         r"""__repr__(array_link self) -> std::string"""
         return _oalib.array_link___repr__(self)
 
 # Register array_link in _oalib:
 _oalib.array_link_swigregister(array_link)
 
-
 def create_array_link(pymatinput):
-    r"""create_array_link(long * pymatinput) -> array_link"""
+    r""" Create array_link from numpy array"""
     return _oalib.create_array_link(pymatinput)
 
 def update_array_link(al, pymatinput):
-    r"""update_array_link(array_link al, long * pymatinput)"""
+    r""" Update the data of an array_link with the specified data"""
     return _oalib.update_array_link(al, pymatinput)
 
 def compareLMC(lhs, rhs):
-    r"""compareLMC(array_link lhs, array_link rhs) -> int"""
+    r""" Return -1 if the first array is smaller in LMC ordering than the second array, 0 if equal and 1 otherwise *"""
     return _oalib.compareLMC(lhs, rhs)
 
 def exampleArray(idx=0, verbose=0):
-    r"""exampleArray(int idx=0, int verbose=0) -> array_link"""
+    r"""
+     Return example array
+
+    :type idx: int, optional
+    :param idx: Index of example array to return
+    :type verbose: int, optional
+    :param verbose: If True, then print information about the array to stdout
+    """
     return _oalib.exampleArray(idx, verbose)
 
 def Jcharacteristics_conference(array, number_of_columns, verbose=0):
-    r"""Jcharacteristics_conference(array_link array, int number_of_columns, int verbose=0) -> intVector"""
+    r"""
+     Calculate Jk-characteristics for a conference design
+
+    :type array: :py:class:`array_link`
+    :param array: Conference design
+    :type number_of_columns: int
+    :param number_of_columns: Specifies the number of columns to use
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: std::vector< int,std::allocator< int > >
+    :return: A vector of calculated inner products between all combinations of k columns.
+    """
     return _oalib.Jcharacteristics_conference(array, number_of_columns, verbose)
 
 def hstack(*args):
     r"""
-    hstack(array_link array1, array_link array2) -> array_link
-    hstack(array_link array, charVector column) -> array_link
+    *Overload 1:*
+    concatenate 2 arrays in vertical direction
+
+    |
+
+    *Overload 2:*
+    concatenate array and conference_column
     """
     return _oalib.hstack(*args)
 
 def hstacklastcol(A, B):
-    r"""hstacklastcol(array_link A, array_link B) -> array_link"""
+    r""" concatenate the last column of array B to array A"""
     return _oalib.hstacklastcol(A, B)
 
 def vstack(column_top, column_bottom):
-    r"""vstack(charVector column_top, charVector column_bottom) -> charVector"""
+    r""" concatenate two columns"""
     return _oalib.vstack(column_top, column_bottom)
 
 def perform_column_permutation(source, target, perm):
-    r"""perform_column_permutation(array_link source, array_link target, intVector perm)"""
+    r""" perform column permutation for an array"""
     return _oalib.perform_column_permutation(source, target, perm)
 
 def perform_row_permutation(source, target, perm):
-    r"""perform_row_permutation(array_link source, array_link target, intVector perm)"""
+    r""" perform row permutation for an array"""
     return _oalib.perform_row_permutation(source, target, perm)
 
 def arraylink2arraydata(array, extracols=0, strength=2):
-    r"""arraylink2arraydata(array_link array, int extracols=0, int strength=2) -> arraydata_t"""
+    r"""
+     create arraydata_t structure from array
+
+    :type array: :py:class:`array_link`
+    :param array: Array to use as input specifiction for array class
+    :type extracols: int, optional
+    :param extracols: Number of extra columns to add to the number of columns of the array
+    :type strength: int, optional
+    :param strength: Strength to set in the array class. If -1, then use the strength of the array
+    """
     return _oalib.arraylink2arraydata(array, extracols, strength)
 
 def addConstant(lst, value):
-    r"""addConstant(arraylist_t lst, int value) -> arraylist_t"""
+    r""" add a constant value to all arrays in a list"""
     return _oalib.addConstant(lst, value)
 
 def getJcounts(arraylist, N, k, verbose=1):
-    r"""getJcounts(arraylist_t arraylist, int N, int k, int verbose=1) -> intVector"""
+    r""" Return number of arrays with j_{2n+1}=0 for number_of_arrays<m"""
     return _oalib.getJcounts(arraylist, N, k, verbose)
 class jstructbase_t(object):
     r"""
 
 
     struct to hold data of an array, e.g. J-characteristic. Abstract base class
 
@@ -4017,18 +4046,18 @@
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
 
     def __init__(self, *args, **kwargs):
         raise AttributeError("No constructor defined - class is abstract")
     __repr__ = _swig_repr
-    values = property(_oalib.jstructbase_t_values_get, _oalib.jstructbase_t_values_set, doc=r"""values : std::vector<(int,std::allocator<(int)>)>""")
+    values = property(_oalib.jstructbase_t_values_get, _oalib.jstructbase_t_values_set, doc=r""" calculated J-characteristics""")
     jvalues = property(_oalib.jstructbase_t_jvalues_get, _oalib.jstructbase_t_jvalues_set, doc=r"""jvalues : std::vector<(int,std::allocator<(int)>)>""")
-    jvalue2index = property(_oalib.jstructbase_t_jvalue2index_get, _oalib.jstructbase_t_jvalue2index_set, doc=r"""jvalue2index : std::map<(int,int,std::less<(int)>,std::allocator<(std::pair<(q(const).int,int)>)>)>""")
-    jj = property(_oalib.jstructbase_t_jj_get, _oalib.jstructbase_t_jj_set, doc=r"""jj : int""")
+    jvalue2index = property(_oalib.jstructbase_t_jvalue2index_get, _oalib.jstructbase_t_jvalue2index_set, doc=r""" map from Jk-value to index in the jvalues variable""")
+    jj = property(_oalib.jstructbase_t_jj_get, _oalib.jstructbase_t_jj_set, doc=r""" number of columns""")
 
     def maxJ(self):
         r"""
         maxJ(jstructbase_t self) -> int
 
 
         calculate maximum J value
@@ -4106,15 +4135,14 @@
 
         """
         return _oalib.jstructbase_t_allzero(self)
     __swig_destroy__ = _oalib.delete_jstructbase_t
 
 # Register jstructbase_t in _oalib:
 _oalib.jstructbase_t_swigregister(jstructbase_t)
-
 class symmdata(object):
     r"""
 
     `symmdata(al, minlen=1)`
 
     structure containing data related to symmetries of arrays
 
@@ -4165,15 +4193,14 @@
 
         """
         return _oalib.symmdata_checkIdx(self, col)
     __swig_destroy__ = _oalib.delete_symmdata
 
 # Register symmdata in _oalib:
 _oalib.symmdata_swigregister(symmdata)
-
 class jstruct_t(object):
     r"""
 
     `jstruct_t()`
     `jstruct_t(al, jj=4)`
     `jstruct_t(N, K, jj=4)`
     `jstruct_t(js)`
@@ -4223,20 +4250,20 @@
         calculated abberation
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    N = property(_oalib.jstruct_t_N_get, _oalib.jstruct_t_N_set, doc=r"""N : int""")
-    k = property(_oalib.jstruct_t_k_get, _oalib.jstruct_t_k_set, doc=r"""k : int""")
-    jj = property(_oalib.jstruct_t_jj_get, _oalib.jstruct_t_jj_set, doc=r"""jj : int""")
-    nc = property(_oalib.jstruct_t_nc_get, _oalib.jstruct_t_nc_set, doc=r"""nc : int""")
-    values = property(_oalib.jstruct_t_values_get, _oalib.jstruct_t_values_set, doc=r"""values : std::vector<(int,std::allocator<(int)>)>""")
-    abberration = property(_oalib.jstruct_t_abberration_get, _oalib.jstruct_t_abberration_set, doc=r"""abberration : double""")
+    N = property(_oalib.jstruct_t_N_get, _oalib.jstruct_t_N_set, doc=r""" number of rows in array""")
+    k = property(_oalib.jstruct_t_k_get, _oalib.jstruct_t_k_set, doc=r""" number of columns in array""")
+    jj = property(_oalib.jstruct_t_jj_get, _oalib.jstruct_t_jj_set, doc=r""" J-characteristic that is calculated""")
+    nc = property(_oalib.jstruct_t_nc_get, _oalib.jstruct_t_nc_set, doc=r""" number of column combinations possible""")
+    values = property(_oalib.jstruct_t_values_get, _oalib.jstruct_t_values_set, doc=r""" contains calculated J-values""")
+    abberration = property(_oalib.jstruct_t_abberration_get, _oalib.jstruct_t_abberration_set, doc=r""" calculated abberation""")
 
     def __init__(self, *args):
         r"""
         __init__(jstruct_t self) -> jstruct_t
         __init__(jstruct_t self, array_link al, int jj=4) -> jstruct_t
         __init__(jstruct_t self, int const N, int const K, int const jj=4) -> jstruct_t
         __init__(jstruct_t self, jstruct_t js) -> jstruct_t
@@ -4345,24 +4372,23 @@
 
         return 1 if all J values are zero, otherwise return 0
 
         """
         return _oalib.jstruct_t_allzero(self)
 
     def calcj5(self, al):
-        r"""calcj5(jstruct_t self, array_link al)"""
+        r""" calculate J-characteristics of a 2-level array, special function for jj=5"""
         return _oalib.jstruct_t_calcj5(self, al)
 
     def __repr__(self):
         r"""__repr__(jstruct_t self) -> std::string"""
         return _oalib.jstruct_t___repr__(self)
 
 # Register jstruct_t in _oalib:
 _oalib.jstruct_t_swigregister(jstruct_t)
-
 class jstructconference_t(jstructbase_t):
     r"""
 
     `jstructconference_t(N, jj=4)`
     `jstructconference_t(array, jj=4)`
 
     Calculate J-characteristics of conference designs
@@ -4417,40 +4443,48 @@
         r"""__repr__(jstructconference_t self) -> std::string"""
         return _oalib.jstructconference_t___repr__(self)
     __swig_destroy__ = _oalib.delete_jstructconference_t
 
 # Register jstructconference_t in _oalib:
 _oalib.jstructconference_t_swigregister(jstructconference_t)
 
-
 def create_root(*args):
     r"""
-    create_root(array_t * array, arraydata_t arrayclass)
-    create_root(arraydata_t arrayclass, arraylist_t solutions)
+    *Overload 1:*
+    set first columns of an array to root form
+
+    |
+
+    *Overload 2:*
+    Creates the root of an orthogonal array. The root is appended to the list of arrays
     """
     return _oalib.create_root(*args)
 
 def array_diff(A, B, r, c, rpos, cpos):
-    r"""array_diff(carray_p A, carray_p B, rowindex_t const r, colindex_t const c, rowindex_t & rpos, colindex_t & cpos) -> int"""
+    r""" Compare 2 arrays and return position of first difference"""
     return _oalib.array_diff(A, B, r, c, rpos, cpos)
 
 def fastJupdate(array, N, J, column_indices, tmp):
-    r"""fastJupdate(array_t const * array, rowindex_t N, int const J, colindex_t const * column_indices, array_t * tmp)"""
+    r""" helper function to calculate J-values"""
     return _oalib.fastJupdate(array, N, J, column_indices, tmp)
 
 def jvalue(array, J, column_indices):
-    r"""jvalue(array_link array, int const J, int const * column_indices) -> int"""
+    r""" Calculate J-value for a 2-level array"""
     return _oalib.jvalue(array, J, column_indices)
 
 def jvaluefast(array, N, J, column_indices):
-    r"""jvaluefast(array_t const * array, rowindex_t N, int const J, colindex_t const * column_indices) -> int"""
+    r"""
+     Calculate J-value for a column combination of a 2-level array
+
+    We assume the array has values 0 and 1. No boundary checks are performed.
+    """
     return _oalib.jvaluefast(array, N, J, column_indices)
 
 def analyseArrays(arraylist, verbose, jj=4):
-    r"""analyseArrays(arraylist_t arraylist, int const verbose, int const jj=4) -> jstructArray"""
+    r""" Analyse a list of arrays"""
     return _oalib.analyseArrays(arraylist, verbose, jj)
 class array_transformation_t(object):
     r"""
 
     `array_transformation_t(arrayclass)`
     `array_transformation_t(arrayclass)`
     `array_transformation_t()`
@@ -4490,18 +4524,18 @@
         type of array
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    rperm = property(_oalib.array_transformation_t_rperm_get, _oalib.array_transformation_t_rperm_set, doc=r"""rperm : rowperm_t""")
-    cperm = property(_oalib.array_transformation_t_cperm_get, _oalib.array_transformation_t_cperm_set, doc=r"""cperm : colperm_t""")
-    lperms = property(_oalib.array_transformation_t_lperms_get, _oalib.array_transformation_t_lperms_set, doc=r"""lperms : p.levelperm_t""")
-    ad = property(_oalib.array_transformation_t_ad_get, _oalib.array_transformation_t_ad_set, doc=r"""ad : p.q(const).arraydata_t""")
+    rperm = property(_oalib.array_transformation_t_rperm_get, _oalib.array_transformation_t_rperm_set, doc=r""" row permutation""")
+    cperm = property(_oalib.array_transformation_t_cperm_get, _oalib.array_transformation_t_cperm_set, doc=r""" column permutation""")
+    lperms = property(_oalib.array_transformation_t_lperms_get, _oalib.array_transformation_t_lperms_set, doc=r""" level permutations""")
+    ad = property(_oalib.array_transformation_t_ad_get, _oalib.array_transformation_t_ad_set, doc=r""" type of array""")
 
     def __init__(self, *args):
         r"""
         __init__(array_transformation_t self, arraydata_t arrayclass) -> array_transformation_t
         __init__(array_transformation_t self, arraydata_t arrayclass) -> array_transformation_t
         __init__(array_transformation_t self) -> array_transformation_t
         __init__(array_transformation_t self, array_transformation_t transformation) -> array_transformation_t
@@ -4570,19 +4604,19 @@
 
         initialize with a random row permutation
 
         """
         return _oalib.array_transformation_t_randomizerowperm(self)
 
     def __eq__(self, t2):
-        r"""__eq__(array_transformation_t self, array_transformation_t t2) -> int"""
+        r""" Comparison operator"""
         return _oalib.array_transformation_t___eq__(self, t2)
 
     def __mul__(self, b):
-        r"""__mul__(array_transformation_t self, array_transformation_t b) -> array_transformation_t"""
+        r""" composition operator. the transformations are applied from the left"""
         return _oalib.array_transformation_t___mul__(self, b)
 
     def apply(self, *args):
         r"""
         apply(array_transformation_t self, array_link array) -> array_link
         apply(array_transformation_t self, array_t * sourcetarget)
         apply(array_transformation_t self, array_t const * source, array_t * target)
@@ -4674,15 +4708,14 @@
 
     def __repr__(self):
         r"""__repr__(array_transformation_t self) -> std::string"""
         return _oalib.array_transformation_t___repr__(self)
 
 # Register array_transformation_t in _oalib:
 _oalib.array_transformation_t_swigregister(array_transformation_t)
-
 class conference_transformation_t(object):
     r"""
 
     `conference_transformation_t()`
     `conference_transformation_t(nrows, ncols)`
     `conference_transformation_t(al)`
     `conference_transformation_t(T)`
@@ -4729,20 +4762,20 @@
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    rperm = property(_oalib.conference_transformation_t_rperm_get, _oalib.conference_transformation_t_rperm_set, doc=r"""rperm : std::vector<(int,std::allocator<(int)>)>""")
-    cperm = property(_oalib.conference_transformation_t_cperm_get, _oalib.conference_transformation_t_cperm_set, doc=r"""cperm : std::vector<(int,std::allocator<(int)>)>""")
-    cswitch = property(_oalib.conference_transformation_t_cswitch_get, _oalib.conference_transformation_t_cswitch_set, doc=r"""cswitch : std::vector<(int,std::allocator<(int)>)>""")
-    rswitch = property(_oalib.conference_transformation_t_rswitch_get, _oalib.conference_transformation_t_rswitch_set, doc=r"""rswitch : std::vector<(int,std::allocator<(int)>)>""")
-    nrows = property(_oalib.conference_transformation_t_nrows_get, _oalib.conference_transformation_t_nrows_set, doc=r"""nrows : int""")
-    ncols = property(_oalib.conference_transformation_t_ncols_get, _oalib.conference_transformation_t_ncols_set, doc=r"""ncols : int""")
+    rperm = property(_oalib.conference_transformation_t_rperm_get, _oalib.conference_transformation_t_rperm_set, doc=r""" row permutation of the transformation""")
+    cperm = property(_oalib.conference_transformation_t_cperm_get, _oalib.conference_transformation_t_cperm_set, doc=r""" column permutation of the transformation""")
+    cswitch = property(_oalib.conference_transformation_t_cswitch_get, _oalib.conference_transformation_t_cswitch_set, doc=r""" sign flips for the columns""")
+    rswitch = property(_oalib.conference_transformation_t_rswitch_get, _oalib.conference_transformation_t_rswitch_set, doc=r""" sign flips for the rows""")
+    nrows = property(_oalib.conference_transformation_t_nrows_get, _oalib.conference_transformation_t_nrows_set, doc=r""" number of rows""")
+    ncols = property(_oalib.conference_transformation_t_ncols_get, _oalib.conference_transformation_t_ncols_set, doc=r""" number of columns""")
 
     def __init__(self, *args):
         r"""
         __init__(conference_transformation_t self) -> conference_transformation_t
         __init__(conference_transformation_t self, int nrows, int ncols) -> conference_transformation_t
         __init__(conference_transformation_t self, array_link al) -> conference_transformation_t
         __init__(conference_transformation_t self, conference_transformation_t T) -> conference_transformation_t
@@ -4852,15 +4885,19 @@
         return _oalib.conference_transformation_t_apply(self, al)
 
     def __eq__(self, rhs):
         r"""__eq__(conference_transformation_t self, conference_transformation_t rhs) -> int"""
         return _oalib.conference_transformation_t___eq__(self, rhs)
 
     def __mul__(self, rhs):
-        r"""__mul__(conference_transformation_t self, conference_transformation_t rhs) -> conference_transformation_t"""
+        r"""
+         composition operator. the transformations are applied from the left
+
+        E.g. (T1*T2)(x) = T1(T2(x))
+        """
         return _oalib.conference_transformation_t___mul__(self, rhs)
 
     def setrowperm(self, rp):
         r"""
         setrowperm(conference_transformation_t self, intVector rp)
 
 
@@ -4875,17 +4912,16 @@
         """
         return _oalib.conference_transformation_t_setcolperm(self, cp)
     __swig_destroy__ = _oalib.delete_conference_transformation_t
 
 # Register conference_transformation_t in _oalib:
 _oalib.conference_transformation_t_swigregister(conference_transformation_t)
 
-
 def showArrayList(lst):
-    r"""showArrayList(arraylist_t lst)"""
+    r""" print a list of arrays to stdout"""
     return _oalib.showArrayList(lst)
 ATEXT = _oalib.ATEXT
 r""" text based format"""
 ALATEX = _oalib.ALATEX
 r""" write arrays to a text file in a format that can be parsed by LaTeX"""
 ABINARY = _oalib.ABINARY
 r""" binary format"""
@@ -4996,22 +5032,22 @@
         maximum number of arrays in structure
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    filename = property(_oalib.arrayfile_t_filename_get, _oalib.arrayfile_t_filename_set, doc=r"""filename : std::string""")
-    iscompressed = property(_oalib.arrayfile_t_iscompressed_get, _oalib.arrayfile_t_iscompressed_set, doc=r"""iscompressed : int""")
-    nrows = property(_oalib.arrayfile_t_nrows_get, _oalib.arrayfile_t_nrows_set, doc=r"""nrows : int""")
-    ncols = property(_oalib.arrayfile_t_ncols_get, _oalib.arrayfile_t_ncols_set, doc=r"""ncols : int""")
-    nbits = property(_oalib.arrayfile_t_nbits_get, _oalib.arrayfile_t_nbits_set, doc=r"""nbits : int""")
-    mode = property(_oalib.arrayfile_t_mode_get, _oalib.arrayfile_t_mode_set, doc=r"""mode : arrayfile::arrayfilemode_t""")
-    rwmode = property(_oalib.arrayfile_t_rwmode_get, _oalib.arrayfile_t_rwmode_set, doc=r"""rwmode : arrayfile::afilerw_t""")
-    narrays = property(_oalib.arrayfile_t_narrays_get, _oalib.arrayfile_t_narrays_set, doc=r"""narrays : int""")
+    filename = property(_oalib.arrayfile_t_filename_get, _oalib.arrayfile_t_filename_set, doc=r""" location of file on disk""")
+    iscompressed = property(_oalib.arrayfile_t_iscompressed_get, _oalib.arrayfile_t_iscompressed_set, doc=r""" True of the file is compressed with gzip""")
+    nrows = property(_oalib.arrayfile_t_nrows_get, _oalib.arrayfile_t_nrows_set, doc=r""" number of rows of the arrays""")
+    ncols = property(_oalib.arrayfile_t_ncols_get, _oalib.arrayfile_t_ncols_set, doc=r""" number of columns of the arrays""")
+    nbits = property(_oalib.arrayfile_t_nbits_get, _oalib.arrayfile_t_nbits_set, doc=r""" number of bits used when storing an array""")
+    mode = property(_oalib.arrayfile_t_mode_get, _oalib.arrayfile_t_mode_set, doc=r""" file mode, can be ATEXT or ABINARY, ABINARY_DIFF, ABINARY_DIFFZERO""")
+    rwmode = property(_oalib.arrayfile_t_rwmode_get, _oalib.arrayfile_t_rwmode_set, doc=r""" file opened for reading or writing""")
+    narrays = property(_oalib.arrayfile_t_narrays_get, _oalib.arrayfile_t_narrays_set, doc=r""" number of arrays in the file""")
     narraycounter = property(_oalib.arrayfile_t_narraycounter_get, _oalib.arrayfile_t_narraycounter_set, doc=r"""narraycounter : int""")
     NARRAYS_MAX = _oalib.arrayfile_t_NARRAYS_MAX
     r""" maximum number of arrays in structure"""
 
     def __init__(self, *args):
         r"""
         __init__(arrayfile_t self) -> arrayfile_t
@@ -5188,16 +5224,16 @@
 
 
         return true of the file format has random access mode
 
         """
         return _oalib.arrayfile_t_hasrandomaccess(self)
     nfid = property(_oalib.arrayfile_t_nfid_get, _oalib.arrayfile_t_nfid_set, doc=r"""nfid : p.FILE""")
-    gzfid = property(_oalib.arrayfile_t_gzfid_get, _oalib.arrayfile_t_gzfid_set, doc=r"""gzfid : int""")
-    verbose = property(_oalib.arrayfile_t_verbose_get, _oalib.arrayfile_t_verbose_set, doc=r"""verbose : int""")
+    gzfid = property(_oalib.arrayfile_t_gzfid_get, _oalib.arrayfile_t_gzfid_set, doc=r""" pointer to compressed file""")
+    verbose = property(_oalib.arrayfile_t_verbose_get, _oalib.arrayfile_t_verbose_set, doc=r""" verbosity level""")
 
     def updatenumbers(self):
         r"""
         updatenumbers(arrayfile_t self)
 
 
         """
@@ -5266,79 +5302,202 @@
     def __repr__(self):
         r"""__repr__(arrayfile_t self) -> std::string"""
         return _oalib.arrayfile_t___repr__(self)
 
 # Register arrayfile_t in _oalib:
 _oalib.arrayfile_t_swigregister(arrayfile_t)
 
-def arrayfile_t_parseModeString(format):
-    r"""
-    arrayfile_t_parseModeString(std::string const format) -> arrayfile::arrayfilemode_t
-
-
-    parse string to determine the file mode
-
-    """
-    return _oalib.arrayfile_t_parseModeString(format)
-
-def arrayfile_t_arrayNbits(*args):
-    r"""
-    arrayfile_t_arrayNbits(arraydata_t ad) -> int
-    arrayfile_t_arrayNbits(array_link A) -> int
-
-
-    return number of bits necessary to store an array
-
-    """
-    return _oalib.arrayfile_t_arrayNbits(*args)
-
-
 def nArrays(fname):
-    r"""nArrays(char const * fname) -> long"""
+    r""" return number of arrays in an array file"""
     return _oalib.nArrays(fname)
 
 def arrayfileinfo(filename, number_of_arrays, number_of_rows, number_of_columns):
-    r"""arrayfileinfo(char const * filename, int & number_of_arrays, int & number_of_rows, int & number_of_columns)"""
+    r"""
+     return information about file with arrays
+
+    :type filename: string
+    :param filename: Filename of array file
+    :type number_of_arrays: int
+    :param number_of_arrays: Variable is set with number of arrays
+    :type number_of_rows: int
+    :param number_of_rows: Variable is set with number of rows
+    :type number_of_columns: int
+    :param number_of_columns: Variable is set with number of columns
+    """
     return _oalib.arrayfileinfo(filename, number_of_arrays, number_of_rows, number_of_columns)
 
 def readarrayfile(*args):
     r"""
-    readarrayfile(char const * fname, int verbose=0, int * setcols=None) -> arraylist_t
-    readarrayfile(char const * filename, arraylist_t arraylist, int verbose=1, int * setcols=None, int * setrows=None, int * setbits=None) -> int
+    *Overload 1:*
+     Read all arrays in a file and append then to an array list
+
+    :type filename: string
+    :param filename: Filename to read from
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: Pointer to list of arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :type setcols: int, optional
+    :param setcols: Reference that is set with the number of columns from the file
+    :type setrows: int, optional
+    :param setrows: Reference that is set with the number of rows from the file
+    :type setbits: int, optional
+    :param setbits: Reference that is set with the number of bits from the file
+    :rtype: int
+    :return: 
+
+
+    |
+
+    *Overload 2:*
+     Read all arrays in a file and append then to an array list
+
+    :type filename: string
+    :param filename: Filename to read from
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: Pointer to list of arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :type setcols: int, optional
+    :param setcols: Reference that is set with the number of columns from the file
+    :type setrows: int, optional
+    :param setrows: Reference that is set with the number of rows from the file
+    :param setbits: Reference that is set with the number of bits from the file
+    :rtype: int
+    :return: 
+
+
+    |
+
+    *Overload 3:*
+     Read all arrays in a file and append then to an array list
+
+    :type filename: string
+    :param filename: Filename to read from
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: Pointer to list of arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :type setcols: int, optional
+    :param setcols: Reference that is set with the number of columns from the file
+    :param setrows: Reference that is set with the number of rows from the file
+    :param setbits: Reference that is set with the number of bits from the file
+    :rtype: int
+    :return: 
+
+
+    |
+
+    *Overload 4:*
+     Read all arrays in a file and append then to an array list
+
+    :type filename: string
+    :param filename: Filename to read from
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: Pointer to list of arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :param setcols: Reference that is set with the number of columns from the file
+    :param setrows: Reference that is set with the number of rows from the file
+    :param setbits: Reference that is set with the number of bits from the file
+    :rtype: int
+    :return: 
+
+
+    |
+
+    *Overload 5:*
+     Read all arrays in a file and append then to an array list
+
+    :type filename: string
+    :param filename: Filename to read from
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: Pointer to list of arrays
+    :param verbose: Verbosity level
+    :param setcols: Reference that is set with the number of columns from the file
+    :param setrows: Reference that is set with the number of rows from the file
+    :param setbits: Reference that is set with the number of bits from the file
+    :rtype: int
+    :return: 
     """
     return _oalib.readarrayfile(*args)
 
 def writearrayfile(*args):
     r"""
-    writearrayfile(char const * filename, arraylist_t arraylist, arrayfile::arrayfilemode_t mode=ATEXT, int nrows=NRAUTO, int ncols=NRAUTO) -> int
-    writearrayfile(char const * filename, array_link array, arrayfile::arrayfilemode_t mode=ATEXT) -> int
+    *Overload 1:*
+     Write a list of arrays to file on disk
+
+    :type filename: string
+    :param filename: Filename to use
+    :type arraylist: :py:class:`arraylist_t`
+    :param arraylist: List of arrays to write
+    :type mode: int, optional
+    :param mode: Mode for the file with designs
+    :type nrows: int, optional
+    :param nrows: If the list of arrays is empty, use this number of rows for the design file
+    :type ncols: int, optional
+    :param ncols: If the list of arrays is empty, use this number of rows for the design file
+    :rtype: int
+    :return: Value zero if succesfull
+
+
+    |
+
+    *Overload 2:*
+     Write a single array to file
+
+    |
+
+    *Overload 3:*
+     Write a single array to file
     """
     return _oalib.writearrayfile(*args)
 
 def append_arrayfile(filename, array):
-    r"""append_arrayfile(char const * filename, array_link array) -> int"""
+    r""" Append a single array to an array file. creates a new file if no file exists"""
     return _oalib.append_arrayfile(filename, array)
 
 def selectArrays(*args):
     r"""
-    selectArrays(std::string const filename, intVector idx, arraylist_t fl, int verbose=0)
-    selectArrays(std::string filename, int index) -> array_link
-    selectArrays(arraylist_t input_list, intVector idx) -> arraylist_t
-    selectArrays(arraylist_t input_list, longVector idx) -> arraylist_t
-    selectArrays(arraylist_t input_list, intVector idx, arraylist_t output_list)
-    selectArrays(arraylist_t input_list, longVector idx, arraylist_t output_list)
+    *Overload 1:*
+    Make a selection of arrays from binary array file, append to list
+
+    |
+
+    *Overload 2:*
+    Select a single array from a file
+
+    |
+
+    *Overload 3:*
+    Make a selection of arrays
+
+    |
+
+    *Overload 4:*
+    Make a selection of arrays
+
+    |
+
+    *Overload 5:*
+    Make a selection of arrays, append to list
+
+    |
+
+    *Overload 6:*
+    Make a selection of arrays, append to list
     """
     return _oalib.selectArrays(*args)
 
 def appendArrays(arrays_to_append, dst):
-    r"""appendArrays(arraylist_t arrays_to_append, arraylist_t dst)"""
+    r""" Append set of arrays to existing list"""
     return _oalib.appendArrays(arrays_to_append, dst)
 
 def convert_array_file(input_filename, output_filename, output_format, verbose=0):
-    r"""convert_array_file(std::string input_filename, std::string output_filename, arrayfile::arrayfilemode_t output_format, int verbose=0)"""
+    r""" Convert a file with arrays to a different format"""
     return _oalib.convert_array_file(input_filename, output_filename, output_format, verbose)
 class arraywriter_t(object):
     r"""
 
     `arraywriter_t()`
 
     structure to write arrays to disk, thread safe
@@ -5366,18 +5525,22 @@
 
     C++ includes: arraytools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    afiles = property(_oalib.arraywriter_t_afiles_get, _oalib.arraywriter_t_afiles_set, doc=r"""afiles : std::vector<(p.arrayfile::arrayfile_t,std::allocator<(p.arrayfile::arrayfile_t)>)>""")
-    writearrays = property(_oalib.arraywriter_t_writearrays_get, _oalib.arraywriter_t_writearrays_set, doc=r"""writearrays : bool""")
-    nwritten = property(_oalib.arraywriter_t_nwritten_get, _oalib.arraywriter_t_nwritten_set, doc=r"""nwritten : int""")
-    verbose = property(_oalib.arraywriter_t_verbose_get, _oalib.arraywriter_t_verbose_set, doc=r"""verbose : int""")
+    afiles = property(_oalib.arraywriter_t_afiles_get, _oalib.arraywriter_t_afiles_set, doc=r"""
+     Pointers to different data files.
+
+    Since depth_extend is a depth first approach we need to store arrays with a different number of columns
+    """)
+    writearrays = property(_oalib.arraywriter_t_writearrays_get, _oalib.arraywriter_t_writearrays_set, doc=r""" only write arrays if this variable is true""")
+    nwritten = property(_oalib.arraywriter_t_nwritten_get, _oalib.arraywriter_t_nwritten_set, doc=r""" number of arrays written to disk""")
+    verbose = property(_oalib.arraywriter_t_verbose_get, _oalib.arraywriter_t_verbose_set, doc=r""" verbosity level""")
 
     def __init__(self):
         r"""
         __init__(arraywriter_t self) -> arraywriter_t
 
 
         """
@@ -5436,51 +5599,129 @@
 # Register arraywriter_t in _oalib:
 _oalib.arraywriter_t_swigregister(arraywriter_t)
 cvar = _oalib.cvar
 NRAUTO = cvar.NRAUTO
 
 
 def readbinheader(fid, nr, nc):
-    r"""readbinheader(FILE * fid, int & nr, int & nc) -> bool"""
+    r"""
+     Read header for binary data file. Return true if valid header file
+
+    The header consists of 4 integers: 2 magic numbers, then the number of rows and columns
+    """
     return _oalib.readbinheader(fid, nr, nc)
 
 def writebinheader(fid, number_rows, number_columns):
-    r"""writebinheader(FILE * fid, int number_rows, int number_columns)"""
+    r""" Write header for binary data file"""
     return _oalib.writebinheader(fid, number_rows, number_columns)
 
 def vectorvector2binfile(fname, vals, writeheader, na):
-    r"""vectorvector2binfile(std::string const fname, vector_vector_double vals, int writeheader, int na)"""
+    r""" Write a vector of vector elements to binary file"""
     return _oalib.vectorvector2binfile(fname, vals, writeheader, na)
 
 def array2eigenX1(array, intercept=1):
-    r"""array2eigenX1(array_link array, int intercept=1) -> MatrixFloat"""
+    r"""
+     Convert 2-level array to main effects in Eigen format
+
+    :type array: :py:class:`array_link`
+    :param array: Array to convert
+    :type intercept: int, optional
+    :param intercept: If True, then include the intercept
+    :rtype: MatrixFloat
+    :return: The main effects model
+    """
     return _oalib.array2eigenX1(array, intercept)
 
 def array2eigenX2(array):
-    r"""array2eigenX2(array_link array) -> MatrixFloat"""
+    r"""
+     Convert 2-level array to second order interaction matrix in Eigen format
+
+    The intercept and main effects are not included.
+
+    :type array: :py:class:`array_link`
+    :param array: Array to convert
+    :rtype: MatrixFloat
+    :return: The second order interaction model
+    """
     return _oalib.array2eigenX2(array)
 
 def array2eigenModelMatrix(array):
-    r"""array2eigenModelMatrix(array_link array) -> MatrixFloat"""
+    r"""
+     Convert 2-level array to second order interaction model matrix (intercept, main effects, interaction effects)
+
+    :type array: :py:class:`array_link`
+    :param array: Design of which to calculate the model matrix
+    :rtype: MatrixFloat
+    :return: Eigen matrix with the model matrix
+    """
     return _oalib.array2eigenModelMatrix(array)
 
 def array2eigenModelMatrixMixed(array, verbose=1):
-    r"""array2eigenModelMatrixMixed(array_link array, int verbose=1) -> pairEigenMatrix"""
+    r"""
+     Create first and second order model matrix for mixed-level orthogonal array
+
+    :type array: :py:class:`array_link`
+    :param array: Input array
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: std::pair< MatrixFloat,MatrixFloat >
+    :return: Pair with main effects and two-factor interaction model
+
+    For 2-level arrays a direct calculation is used. For mixel-level arrays Helmert contrasts are used.
+    """
     return _oalib.array2eigenModelMatrixMixed(array, verbose)
 
 def numberModelParams(array, order=-1):
-    r"""numberModelParams(array_link array, int order=-1) -> intVector"""
+    r"""
+     Calculate number of parameters in the model matrix
+
+    A list of integers is returned, with the number of columns in:
+
+    - The intercept (always 1)
+    - The main effects
+    - The interaction effects (second order interaction terms without quadratics)
+    - The quadratic effects
+
+    :type array: :py:class:`array_link`
+    :param array: Orthogonal array or conference design
+    :type order: int, optional
+    :param order: Not used any more
+    :rtype: std::vector< int,std::allocator< int > >
+    :return: List of sizes
+    """
     return _oalib.numberModelParams(array, order)
 
 def arrayInFile(array, array_file, verbose=1):
-    r"""arrayInFile(array_link array, char const * array_file, int verbose=1) -> int"""
+    r"""
+     return index of specified array in a file. returns -1 if array is not found
+
+    :type array: :py:class:`array_link`
+    :param array: Array to find
+    :type array_file: string
+    :param array_file: Location if file with arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: int
+    :return: Position of array in list
+    """
     return _oalib.arrayInFile(array, array_file, verbose)
 
 def arrayInList(array, arrays, verbose=1):
-    r"""arrayInList(array_link array, arraylist_t arrays, int verbose=1) -> int"""
+    r"""
+     return index of specified array in a list. returns -1 if array is not found
+
+    :type array: :py:class:`array_link`
+    :param array: Array to find
+    :type arrays: :py:class:`arraylist_t`
+    :param arrays: List of arrays
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: int
+    :return: Position of array in list
+    """
     return _oalib.arrayInList(array, arrays, verbose)
 
 def printfd_handler(*args):
     r"""
     printfd_handler(char const * file, char const * func, int line, char const * message)
 
 
@@ -5657,15 +5898,15 @@
 
     return string describing array
 
     """
     return _oalib.oafilestring(arrayclass)
 
 def warning(*args):
-    r"""warning(char const * message)"""
+    r""" Raise warning. In C++ this is a message to stdout. In Python a runtime warning"""
     return _oalib.warning(*args)
 
 def replaceString(subject, search, replacement):
     r"""
     replaceString(std::string subject, std::string const & search, std::string const & replacement) -> std::string
 
 
@@ -5887,15 +6128,27 @@
     The PICk of a design is the average D-efficiency of estimable second-order
     models in k factors. The vector (PIC1, PIC2, ..., ) is called the PIC sequence.
 
     """
     return _oalib.PICsequence(array, verbose)
 
 def macwilliams_transform_mixed(B, N, factor_levels_for_groups, verbose=0):
-    r"""macwilliams_transform_mixed(ndarray_double B, int N, intVector factor_levels_for_groups, int verbose=0) -> ndarray_double"""
+    r"""
+     Calculate MacWilliams transform
+    :type B: ndarray< double >
+    :param B: Input array
+    :type N: int
+    :param N: Number of rows
+    :type factor_levels_for_groups: std::vector< int,std::allocator< int > >
+    :param factor_levels_for_groups: Factor levels for the groups
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: ndarray< double >
+    :return: MacWilliams transform of the input array
+    """
     return _oalib.macwilliams_transform_mixed(B, N, factor_levels_for_groups, verbose)
 
 def distance_distribution(array):
     r"""
     distance_distribution(array_link array) -> doubleVector
 
 
@@ -5904,19 +6157,37 @@
     The distance distribution is described in "Generalized minimum aberration for
     asymmetrical fractional factorial designs", Wu and Xu, 2001
 
     """
     return _oalib.distance_distribution(array)
 
 def distance_distribution_shape(arrayclass):
-    r"""distance_distribution_shape(arraydata_t arrayclass) -> intVector"""
+    r"""
+     Return shape of distance distribution for mixed level design
+    :type arrayclass: :py:class:`arraydata_t`
+    :param arrayclass: Specification of the array class
+    :rtype: std::vector< int,std::allocator< int > >
+    :return: Shape of the distance distribution
+    """
     return _oalib.distance_distribution_shape(arrayclass)
 
 def distance_distribution_mixed(array, verbose=0):
-    r"""distance_distribution_mixed(array_link array, int verbose=0) -> ndarray_double"""
+    r"""
+     Return the distance distribution of a mixed-level design
+
+    The distance distribution is described in "Generalized minimum aberration for asymmetrical fractional factorial designs", Wu and Xu, 2001.
+    For mixed-level designs more details can be found in "A canonical form for non-regular arrays based on generalized wordlength pattern values of delete-one-factor projections", Eendebak, 2014.
+
+    :type array: :py:class:`array_link`
+    :param array: Array for which to calculate the distribution
+    :type verbose: int, optional
+    :param verbose: Verbosity level
+    :rtype: ndarray< double >
+    :return: Distance distribution
+    """
     return _oalib.distance_distribution_mixed(array, verbose)
 
 def distance_distribution_mixed_inplace(al, B, verbose=0):
     r"""distance_distribution_mixed_inplace(array_link al, ndarray_double B, int verbose=0)"""
     return _oalib.distance_distribution_mixed_inplace(al, B, verbose)
 
 def Jcharacteristics(array, number_of_columns=4, verbose=0):
@@ -6296,18 +6567,18 @@
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     alsub = property(_oalib.rankStructure_alsub_get, _oalib.rankStructure_alsub_set, doc=r"""alsub : array_link""")
     r = property(_oalib.rankStructure_r_get, _oalib.rankStructure_r_set, doc=r"""r : int""")
-    verbose = property(_oalib.rankStructure_verbose_get, _oalib.rankStructure_verbose_set, doc=r"""verbose : int""")
-    ks = property(_oalib.rankStructure_ks_get, _oalib.rankStructure_ks_set, doc=r"""ks : int""")
-    nsub = property(_oalib.rankStructure_nsub_get, _oalib.rankStructure_nsub_set, doc=r"""nsub : int""")
-    id = property(_oalib.rankStructure_id_get, _oalib.rankStructure_id_set, doc=r"""id : int""")
+    verbose = property(_oalib.rankStructure_verbose_get, _oalib.rankStructure_verbose_set, doc=r""" verbosity level""")
+    ks = property(_oalib.rankStructure_ks_get, _oalib.rankStructure_ks_set, doc=r""" number of columns of subarray in cache""")
+    nsub = property(_oalib.rankStructure_nsub_get, _oalib.rankStructure_nsub_set, doc=r""" number of columns to subtract from array when updating cache""")
+    id = property(_oalib.rankStructure_id_get, _oalib.rankStructure_id_set, doc=r""" used for debugging""")
 
     def __init__(self, *args):
         r"""
         __init__(rankStructure self, array_link al, int nsub=3, int verbose=0) -> rankStructure
         __init__(rankStructure self, int nsub=3, int id=-1) -> rankStructure
 
 
@@ -6367,15 +6638,14 @@
         """
         return _oalib.rankStructure_rankxf(self, array)
     __swig_destroy__ = _oalib.delete_rankStructure
 
 # Register rankStructure in _oalib:
 _oalib.rankStructure_swigregister(rankStructure)
 
-
 def conditionNumber(matrix):
     r"""
     conditionNumber(array_link matrix) -> double
 
 
     return the condition number of a matrix
 
@@ -6519,17 +6789,17 @@
 
     C++ includes: Deff.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    dds = property(_oalib.DoptimReturn_dds_get, _oalib.DoptimReturn_dds_set, doc=r"""dds : std::vector<(std::vector<(double,std::allocator<(double)>)>,std::allocator<(std::vector<(double,std::allocator<(double)>)>)>)>""")
-    designs = property(_oalib.DoptimReturn_designs_get, _oalib.DoptimReturn_designs_set, doc=r"""designs : arraylist_t""")
-    nrestarts = property(_oalib.DoptimReturn_nrestarts_get, _oalib.DoptimReturn_nrestarts_set, doc=r"""nrestarts : int""")
+    dds = property(_oalib.DoptimReturn_dds_get, _oalib.DoptimReturn_dds_set, doc=r""" calculated efficiencies for the generated designs""")
+    designs = property(_oalib.DoptimReturn_designs_get, _oalib.DoptimReturn_designs_set, doc=r""" designs generated""")
+    nrestarts = property(_oalib.DoptimReturn_nrestarts_get, _oalib.DoptimReturn_nrestarts_set, doc=r""" number of restarts performed""")
     _nimproved = property(_oalib.DoptimReturn__nimproved_get, _oalib.DoptimReturn__nimproved_set, doc=r"""_nimproved : int""")
 
     def __init__(self):
         r"""
         __init__(DoptimReturn self) -> DoptimReturn
 
 
@@ -6553,15 +6823,14 @@
         """
         _oalib.DoptimReturn_swiginit(self, _oalib.new_DoptimReturn())
     __swig_destroy__ = _oalib.delete_DoptimReturn
 
 # Register DoptimReturn in _oalib:
 _oalib.DoptimReturn_swigregister(DoptimReturn)
 
-
 def Doptimize(arrayclass, nrestarts, alpha, verbose, method=DOPTIM_AUTOMATIC, niter=300000, maxtime=100000, nabort=5000):
     r"""
     Doptimize(arraydata_t arrayclass, int nrestarts, doubleVector alpha, int verbose, coordinate_exchange_method_t method=DOPTIM_AUTOMATIC, int niter=300000, double maxtime=100000, int nabort=5000) -> DoptimReturn
 
 
     Generates optimal designs for the specified class of designs
 
@@ -6700,29 +6969,29 @@
     * `j5structure` : `j5structure_t`
 
     C++ includes: extend.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    singleExtendTime = property(_oalib.OAextend_singleExtendTime_get, _oalib.OAextend_singleExtendTime_set, doc=r"""singleExtendTime : double""")
-    nLMC = property(_oalib.OAextend_nLMC_get, _oalib.OAextend_nLMC_set, doc=r"""nLMC : int""")
-    checkarrays = property(_oalib.OAextend_checkarrays_get, _oalib.OAextend_checkarrays_set, doc=r"""checkarrays : int""")
-    check_maximal = property(_oalib.OAextend_check_maximal_get, _oalib.OAextend_check_maximal_set, doc=r"""check_maximal : int""")
-    use_row_symmetry = property(_oalib.OAextend_use_row_symmetry_get, _oalib.OAextend_use_row_symmetry_set, doc=r"""use_row_symmetry : int""")
-    init_column_previous = property(_oalib.OAextend_init_column_previous_get, _oalib.OAextend_init_column_previous_set, doc=r"""init_column_previous : int""")
+    singleExtendTime = property(_oalib.OAextend_singleExtendTime_get, _oalib.OAextend_singleExtendTime_set, doc=r""" time before printing progress of single extension, [seconds]""")
+    nLMC = property(_oalib.OAextend_nLMC_get, _oalib.OAextend_nLMC_set, doc=r""" number of arrays LMC tested before printing progress of single extension""")
+    checkarrays = property(_oalib.OAextend_checkarrays_get, _oalib.OAextend_checkarrays_set, doc=r""" perform LMC test after generation of array""")
+    check_maximal = property(_oalib.OAextend_check_maximal_get, _oalib.OAextend_check_maximal_set, doc=r""" if true then return at once if a single extension has been found""")
+    use_row_symmetry = property(_oalib.OAextend_use_row_symmetry_get, _oalib.OAextend_use_row_symmetry_set, doc=r""" adds a symmetry check to the extension algorithm based in symmetry of row permutations""")
+    init_column_previous = property(_oalib.OAextend_init_column_previous_get, _oalib.OAextend_init_column_previous_set, doc=r""" init column with previous column in extension (if in the same column group)""")
     extendarray_mode_t_APPENDEXTENSION = _oalib.OAextend_extendarray_mode_t_APPENDEXTENSION
     r""" append extension column to extension list"""
     extendarray_mode_t_APPENDFULL = _oalib.OAextend_extendarray_mode_t_APPENDFULL
     r""" append full array to extension list"""
     extendarray_mode_t_STOREARRAY = _oalib.OAextend_extendarray_mode_t_STOREARRAY
     r""" store extension to disk"""
     extendarray_mode_t_NONE = _oalib.OAextend_extendarray_mode_t_NONE
     r""" do not store generated extensions"""
-    extendarraymode = property(_oalib.OAextend_extendarraymode_get, _oalib.OAextend_extendarraymode_set, doc=r"""extendarraymode : OAextend::extendarray_mode_t""")
+    extendarraymode = property(_oalib.OAextend_extendarraymode_get, _oalib.OAextend_extendarraymode_set, doc=r""" determines how the extension arrays are stored""")
     storefile = property(_oalib.OAextend_storefile_get, _oalib.OAextend_storefile_set, doc=r"""storefile : arrayfile::arrayfile_t""")
     j5structure = property(_oalib.OAextend_j5structure_get, _oalib.OAextend_j5structure_set, doc=r"""j5structure : j5structure_t""")
 
     def __init__(self, *args):
         r"""
         __init__(OAextend self) -> OAextend
         __init__(OAextend self, OAextend o) -> OAextend
@@ -6826,36 +7095,14 @@
         """
         return _oalib.OAextend___repr__(self)
     __swig_destroy__ = _oalib.delete_OAextend
 
 # Register OAextend in _oalib:
 _oalib.OAextend_swigregister(OAextend)
 
-def OAextend_getPreferredAlgorithm(arrayclass, verbose=0):
-    r"""
-    OAextend_getPreferredAlgorithm(arraydata_t arrayclass, int verbose=0) -> algorithm_t
-
-
-    Return preferred extension algorithm
-
-    Parameters
-    ----------
-    * `arrayclass` :
-        Class of designs to extend
-    * `verbose` :
-        Verbosity level
-
-    Returns
-    -------
-    Algorithm selected to be used for this class
-
-    """
-    return _oalib.OAextend_getPreferredAlgorithm(arrayclass, verbose)
-
-
 def extend_arraylist(*args):
     r"""
     extend_arraylist(arraylist_t array_list, arraydata_t array_class, OAextend oaextend_options) -> arraylist_t
     extend_arraylist(arraylist_t array_list, arraydata_t arrayclass) -> arraylist_t
     extend_arraylist(arraylist_t array_list, arraydata_t array_class, OAextend oaextend_options, colindex_t extensioncol, arraylist_t extensions) -> int
 
 
@@ -6993,21 +7240,21 @@
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     NO_VALUE = _oalib.dextend_t_NO_VALUE
     
-    lmctype = property(_oalib.dextend_t_lmctype_get, _oalib.dextend_t_lmctype_set, doc=r"""lmctype : std::vector<(lmc_t,std::allocator<(lmc_t)>)>""")
-    lastcol = property(_oalib.dextend_t_lastcol_get, _oalib.dextend_t_lastcol_set, doc=r"""lastcol : std::vector<(int,std::allocator<(int)>)>""")
-    Deff = property(_oalib.dextend_t_Deff_get, _oalib.dextend_t_Deff_set, doc=r"""Deff : std::vector<(double,std::allocator<(double)>)>""")
-    filter = property(_oalib.dextend_t_filter_get, _oalib.dextend_t_filter_set, doc=r"""filter : std::vector<(int,std::allocator<(int)>)>""")
+    lmctype = property(_oalib.dextend_t_lmctype_get, _oalib.dextend_t_lmctype_set, doc=r""" results of minimal form calculations""")
+    lastcol = property(_oalib.dextend_t_lastcol_get, _oalib.dextend_t_lastcol_set, doc=r""" last column changed in lmc check""")
+    Deff = property(_oalib.dextend_t_Deff_get, _oalib.dextend_t_Deff_set, doc=r""" calculated efficiency values""")
+    filter = property(_oalib.dextend_t_filter_get, _oalib.dextend_t_filter_set, doc=r""" indices of filtered arrays""")
     filtermode = property(_oalib.dextend_t_filtermode_get, _oalib.dextend_t_filtermode_set, doc=r"""filtermode : dfilter_t""")
     Dcheck = property(_oalib.dextend_t_Dcheck_get, _oalib.dextend_t_Dcheck_set, doc=r"""Dcheck : dcalc_mode""")
-    directcheck = property(_oalib.dextend_t_directcheck_get, _oalib.dextend_t_directcheck_set, doc=r"""directcheck : int""")
+    directcheck = property(_oalib.dextend_t_directcheck_get, _oalib.dextend_t_directcheck_set, doc=r""" perform immediate LMC check in extension""")
 
     def __init__(self):
         r"""
         __init__(dextend_t self) -> dextend_t
 
 
         """
@@ -7036,24 +7283,23 @@
         filterArrays(dextend_t self, array_link al, arraylist_t earrays, arraylist_t earraysout, vector_vector_double edata, int verbose=1) -> intVector
 
 
         filter the arrays based on values in filter
 
         """
         return _oalib.dextend_t_filterArrays(self, al, earrays, earraysout, edata, verbose)
-    ntotal = property(_oalib.dextend_t_ntotal_get, _oalib.dextend_t_ntotal_set, doc=r"""ntotal : long""")
-    nlmc = property(_oalib.dextend_t_nlmc_get, _oalib.dextend_t_nlmc_set, doc=r"""nlmc : long""")
-    n = property(_oalib.dextend_t_n_get, _oalib.dextend_t_n_set, doc=r"""n : long""")
+    ntotal = property(_oalib.dextend_t_ntotal_get, _oalib.dextend_t_ntotal_set, doc=r""" total number of arrays found""")
+    nlmc = property(_oalib.dextend_t_nlmc_get, _oalib.dextend_t_nlmc_set, doc=r""" total number of arrays found in LMC form""")
+    n = property(_oalib.dextend_t_n_get, _oalib.dextend_t_n_set, doc=r""" total number of arrays found passing all tests""")
     DmaxDiscard = property(_oalib.dextend_t_DmaxDiscard_get, _oalib.dextend_t_DmaxDiscard_set, doc=r"""DmaxDiscard : double""")
     nmaxrnktotal = property(_oalib.dextend_t_nmaxrnktotal_get, _oalib.dextend_t_nmaxrnktotal_set, doc=r"""nmaxrnktotal : long""")
     __swig_destroy__ = _oalib.delete_dextend_t
 
 # Register dextend_t in _oalib:
 _oalib.dextend_t_swigregister(dextend_t)
-
 LMC_LESS = _oalib.LMC_LESS
 r""" Found a permutation which leads to a lexicographically smaller array"""
 LMC_EQUAL = _oalib.LMC_EQUAL
 r""" Found a permutation which leads to a lexicographically equal array"""
 LMC_MORE = _oalib.LMC_MORE
 r""" Found a permutation which leads to a lexicographically larger array"""
 LMC_NONSENSE = _oalib.LMC_NONSENSE
@@ -7105,37 +7351,37 @@
 
 
     return name of the algorithm
 
     """
     return _oalib.algnames(m)
 class rowsort_t(object):
-    r"""Proxy of C++ rowsort_t class."""
+    r""" type for value for sorting rows structure to perform row sorting"""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    r = property(_oalib.rowsort_t_r_get, _oalib.rowsort_t_r_set, doc=r"""r : rowindex_t""")
-    val = property(_oalib.rowsort_t_val_get, _oalib.rowsort_t_val_set, doc=r"""val : rowsort_value_t""")
+    r = property(_oalib.rowsort_t_r_get, _oalib.rowsort_t_r_set, doc=r""" index of row""")
+    val = property(_oalib.rowsort_t_val_get, _oalib.rowsort_t_val_set, doc=r""" value of row""")
 
     def __init__(self):
         r"""__init__(rowsort_t self) -> rowsort_t"""
         _oalib.rowsort_t_swiginit(self, _oalib.new_rowsort_t())
     __swig_destroy__ = _oalib.delete_rowsort_t
 
 # Register rowsort_t in _oalib:
 _oalib.rowsort_t_swigregister(rowsort_t)
 MODE_ORIGINAL = cvar.MODE_ORIGINAL
 
 
 def __lt__(a, b):
-    r"""__lt__(rowsort_t a, rowsort_t b) -> bool"""
+    r"""Comparision operator for the rowsort_t structure"""
     return _oalib.__lt__(a, b)
 
 def __gt__(a, b):
-    r"""__gt__(rowsort_t a, rowsort_t b) -> bool"""
+    r"""Comparision operator for the rowsort_t structure"""
     return _oalib.__gt__(a, b)
 
 def apply_hadamard(al, hcolumn):
     r"""
     apply_hadamard(array_link al, colindex_t hcolumn)
 
 
@@ -7203,24 +7449,24 @@
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     LMC_non_root_init = property(_oalib.LMCreduction_helper_t_LMC_non_root_init_get, _oalib.LMCreduction_helper_t_LMC_non_root_init_set, doc=r"""LMC_non_root_init : int""")
     LMC_root_init = property(_oalib.LMCreduction_helper_t_LMC_root_init_get, _oalib.LMCreduction_helper_t_LMC_root_init_set, doc=r"""LMC_root_init : int""")
     LMC_reduce_root_rowperms_init = property(_oalib.LMCreduction_helper_t_LMC_reduce_root_rowperms_init_get, _oalib.LMCreduction_helper_t_LMC_reduce_root_rowperms_init_set, doc=r"""LMC_reduce_root_rowperms_init : int""")
     ad = property(_oalib.LMCreduction_helper_t_ad_get, _oalib.LMCreduction_helper_t_ad_set, doc=r"""ad : p.arraydata_t""")
     LMC_root_rowperms_init = property(_oalib.LMCreduction_helper_t_LMC_root_rowperms_init_get, _oalib.LMCreduction_helper_t_LMC_root_rowperms_init_set, doc=r"""LMC_root_rowperms_init : int""")
-    nrootrowperms = property(_oalib.LMCreduction_helper_t_nrootrowperms_get, _oalib.LMCreduction_helper_t_nrootrowperms_set, doc=r"""nrootrowperms : int""")
-    rootrowperms = property(_oalib.LMCreduction_helper_t_rootrowperms_get, _oalib.LMCreduction_helper_t_rootrowperms_set, doc=r"""rootrowperms : p.rowperm_t""")
+    nrootrowperms = property(_oalib.LMCreduction_helper_t_nrootrowperms_get, _oalib.LMCreduction_helper_t_nrootrowperms_set, doc=r""" number of root row permutations""")
+    rootrowperms = property(_oalib.LMCreduction_helper_t_rootrowperms_get, _oalib.LMCreduction_helper_t_rootrowperms_set, doc=r""" pointer to row permutations that leave the root unchanged""")
     LMC_root_rowperms_init_full = property(_oalib.LMCreduction_helper_t_LMC_root_rowperms_init_full_get, _oalib.LMCreduction_helper_t_LMC_root_rowperms_init_full_set, doc=r"""LMC_root_rowperms_init_full : int""")
     nrootrowperms_full = property(_oalib.LMCreduction_helper_t_nrootrowperms_full_get, _oalib.LMCreduction_helper_t_nrootrowperms_full_set, doc=r"""nrootrowperms_full : int""")
     rootrowperms_full = property(_oalib.LMCreduction_helper_t_rootrowperms_full_get, _oalib.LMCreduction_helper_t_rootrowperms_full_set, doc=r"""rootrowperms_full : p.rowperm_t""")
     colbuffer = property(_oalib.LMCreduction_helper_t_colbuffer_get, _oalib.LMCreduction_helper_t_colbuffer_set, doc=r"""colbuffer : p.array_t""")
-    dyndata_p = property(_oalib.LMCreduction_helper_t_dyndata_p_get, _oalib.LMCreduction_helper_t_dyndata_p_set, doc=r"""dyndata_p : p.p.dyndata_t""")
-    colperm_p = property(_oalib.LMCreduction_helper_t_colperm_p_get, _oalib.LMCreduction_helper_t_colperm_p_set, doc=r"""colperm_p : p.p.colindex_t""")
-    localcolperm_p = property(_oalib.LMCreduction_helper_t_localcolperm_p_get, _oalib.LMCreduction_helper_t_localcolperm_p_set, doc=r"""localcolperm_p : p.p.colindex_t""")
-    current_trans = property(_oalib.LMCreduction_helper_t_current_trans_get, _oalib.LMCreduction_helper_t_current_trans_set, doc=r"""current_trans : p.array_transformation_t""")
+    dyndata_p = property(_oalib.LMCreduction_helper_t_dyndata_p_get, _oalib.LMCreduction_helper_t_dyndata_p_set, doc=r""" buffer for a single column""")
+    colperm_p = property(_oalib.LMCreduction_helper_t_colperm_p_get, _oalib.LMCreduction_helper_t_colperm_p_set, doc=r""" dynamic data; row permutations""")
+    localcolperm_p = property(_oalib.LMCreduction_helper_t_localcolperm_p_get, _oalib.LMCreduction_helper_t_localcolperm_p_set, doc=r""" column permutations""")
+    current_trans = property(_oalib.LMCreduction_helper_t_current_trans_get, _oalib.LMCreduction_helper_t_current_trans_set, doc=r""" local column permutation""")
 
     def __init__(self):
         r"""
         __init__(LMCreduction_helper_t self) -> LMCreduction_helper_t
 
 
         """
@@ -7304,15 +7550,14 @@
 
         """
         return _oalib.LMCreduction_helper_t_init_rootrowperms_full(self, totalperms, rootrowperms, lperm_p)
 
 # Register LMCreduction_helper_t in _oalib:
 _oalib.LMCreduction_helper_t_swigregister(LMCreduction_helper_t)
 
-
 def acquire_LMCreduction_object():
     r"""
     acquire_LMCreduction_object() -> LMCreduction_helper_t
 
 
     return static structure from dynamic global pool, return with
     releaseGlobalStatic
@@ -7345,15 +7590,15 @@
 r""" test for minimal form"""
 OA_REDUCE = _oalib.OA_REDUCE
 r""" reduce to minimal form"""
 OA_REDUCE_PARTIAL = _oalib.OA_REDUCE_PARTIAL
 r""" reduce to partial minimal form"""
 
 def valid_ptr(sd):
-    r"""valid_ptr(symmdata sd) -> bool"""
+    r""" Return true if the (smart) symmdataPointer pointer is allocated"""
     return _oalib.valid_ptr(sd)
 INIT_STATE_INVALID = _oalib.INIT_STATE_INVALID
 
 COPY = _oalib.COPY
 r""" copy from array argument"""
 INIT = _oalib.INIT
 r"""  initialized by user"""
@@ -7415,21 +7660,21 @@
 
     C++ includes: lmc.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     array = property(_oalib.LMCreduction_t_array_get, _oalib.LMCreduction_t_array_set, doc=r"""array : p.array_t""")
-    transformation = property(_oalib.LMCreduction_t_transformation_get, _oalib.LMCreduction_t_transformation_set, doc=r"""transformation : p.array_transformation_t""")
+    transformation = property(_oalib.LMCreduction_t_transformation_get, _oalib.LMCreduction_t_transformation_set, doc=r""" pointer to transformation_t structure""")
     mode = property(_oalib.LMCreduction_t_mode_get, _oalib.LMCreduction_t_mode_set, doc=r"""mode : OA_MODE""")
     state = property(_oalib.LMCreduction_t_state_get, _oalib.LMCreduction_t_state_set, doc=r"""state : REDUCTION_STATE""")
     init_state = property(_oalib.LMCreduction_t_init_state_get, _oalib.LMCreduction_t_init_state_set, doc=r"""init_state : INIT_STATE""")
-    maxdepth = property(_oalib.LMCreduction_t_maxdepth_get, _oalib.LMCreduction_t_maxdepth_set, doc=r"""maxdepth : int""")
-    lastcol = property(_oalib.LMCreduction_t_lastcol_get, _oalib.LMCreduction_t_lastcol_set, doc=r"""lastcol : int""")
-    nred = property(_oalib.LMCreduction_t_nred_get, _oalib.LMCreduction_t_nred_set, doc=r"""nred : long""")
+    maxdepth = property(_oalib.LMCreduction_t_maxdepth_get, _oalib.LMCreduction_t_maxdepth_set, doc=r""" maximum depth for search tree""")
+    lastcol = property(_oalib.LMCreduction_t_lastcol_get, _oalib.LMCreduction_t_lastcol_set, doc=r""" last column visited in algorithm""")
+    nred = property(_oalib.LMCreduction_t_nred_get, _oalib.LMCreduction_t_nred_set, doc=r""" counter for number of reductions made""")
     targetcol = property(_oalib.LMCreduction_t_targetcol_get, _oalib.LMCreduction_t_targetcol_set, doc=r"""targetcol : int""")
     mincol = property(_oalib.LMCreduction_t_mincol_get, _oalib.LMCreduction_t_mincol_set, doc=r"""mincol : int""")
     nrows = property(_oalib.LMCreduction_t_nrows_get, _oalib.LMCreduction_t_nrows_set, doc=r"""nrows : int""")
     ncols = property(_oalib.LMCreduction_t_ncols_get, _oalib.LMCreduction_t_ncols_set, doc=r"""ncols : int""")
     staticdata = property(_oalib.LMCreduction_t_staticdata_get, _oalib.LMCreduction_t_staticdata_set, doc=r"""staticdata : p.LMCreduction_helper_t""")
     sd = property(_oalib.LMCreduction_t_sd_get, _oalib.LMCreduction_t_sd_set, doc=r"""sd : symmdataPointer""")
 
@@ -7554,15 +7799,14 @@
 
 
         """
         return _oalib.LMCreduction_t_updateLastCol(self, col)
 
 # Register LMCreduction_t in _oalib:
 _oalib.LMCreduction_t_swigregister(LMCreduction_t)
-
 class rowsorter_t(object):
     r"""
 
     `rowsorter_t(number_of_rows)`
 
     Structure to sort rows of arrays.
 
@@ -7592,15 +7836,14 @@
 
         """
         _oalib.rowsorter_t_swiginit(self, _oalib.new_rowsorter_t(number_of_rows))
     __swig_destroy__ = _oalib.delete_rowsorter_t
 
 # Register rowsorter_t in _oalib:
 _oalib.rowsorter_t_swigregister(rowsorter_t)
-
 class dyndata_t(object):
     r"""
 
     `dyndata_t(N, col=0)`
     `dyndata_t(dd)`
     `dyndata_t(arg1)`
 
@@ -7646,19 +7889,19 @@
 
     C++ includes: lmc.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    col = property(_oalib.dyndata_t_col_get, _oalib.dyndata_t_col_set, doc=r"""col : colindex_t""")
-    N = property(_oalib.dyndata_t_N_get, _oalib.dyndata_t_N_set, doc=r"""N : rowindex_t""")
-    rowsort = property(_oalib.dyndata_t_rowsort_get, _oalib.dyndata_t_rowsort_set, doc=r"""rowsort : p.rowsort_t""")
+    col = property(_oalib.dyndata_t_col_get, _oalib.dyndata_t_col_set, doc=r""" active column""")
+    N = property(_oalib.dyndata_t_N_get, _oalib.dyndata_t_N_set, doc=r""" number of rows""")
+    rowsort = property(_oalib.dyndata_t_rowsort_get, _oalib.dyndata_t_rowsort_set, doc=r""" ordering of rows""")
     rowsortl = property(_oalib.dyndata_t_rowsortl_get, _oalib.dyndata_t_rowsortl_set, doc=r"""rowsortl : p.rowsortlight_t""")
-    colperm = property(_oalib.dyndata_t_colperm_get, _oalib.dyndata_t_colperm_set, doc=r"""colperm : colperm_t""")
+    colperm = property(_oalib.dyndata_t_colperm_get, _oalib.dyndata_t_colperm_set, doc=r""" current column permutation""")
 
     def __init__(self, *args):
         r"""
         __init__(dyndata_t self, int N, int col=0) -> dyndata_t
         __init__(dyndata_t self, dyndata_t dd) -> dyndata_t
 
 
@@ -7760,15 +8003,14 @@
 
         """
         return _oalib.dyndata_t_copydata(self, dd)
 
 # Register dyndata_t in _oalib:
 _oalib.dyndata_t_swigregister(dyndata_t)
 
-
 def is_root_form(array, strength):
     r"""
     is_root_form(array_link array, int strength) -> bool
 
 
     Return True if the array is in root form
 
@@ -8016,33 +8258,52 @@
     -------
     Relabelling of the graph vertices
 
     """
     return _oalib.reduceNauty(graph, colors, verbose)
 
 def transformGraph(graph, vertex_permutation, verbose=1):
-    r"""transformGraph(array_link graph, intVector vertex_permutation, int verbose=1) -> array_link"""
+    r""" Apply a vertex permutation to a graph"""
     return _oalib.transformGraph(graph, vertex_permutation, verbose)
 
 def reduceOAnauty(*args):
     r"""
-    reduceOAnauty(array_link array, int verbose=0) -> array_transformation_t
-    reduceOAnauty(array_link array, int verbose, arraydata_t arrayclass) -> array_transformation_t
+    *Overload 1:*
+    Reduce an orthogonal array to Nauty minimal form. the array transformation is returned
+
+    |
+
+    *Overload 2:*
+    Reduce an orthogonal array to Nauty minimal form. the array transformation is returned
     """
     return _oalib.reduceOAnauty(*args)
 
 def array2graph(*args):
     r"""
-    array2graph(array_link array, int verbose=1) -> pairGraphColors
-    array2graph(array_link array, int verbose, arraydata_t arrayclass) -> pairGraphColors
+    *Overload 1:*
+    Convert orthogonal array to graph representation
+
+    The conversion method is as in Ryan and Bulutoglu.
+    The resulting graph is bi-partite.
+    The graph representation can be used for isomorphism testing.
+
+
+    |
+
+    *Overload 2:*
+    Convert orthogonal array to graph representation
+
+    The conversion method is as in Ryan and Bulutoglu.
+    The resulting graph is bi-partite.
+    The graph representation can be used for isomorphism testing.
     """
     return _oalib.array2graph(*args)
 
 def oagraph2transformation(pp, arrayclass, verbose=1):
-    r"""oagraph2transformation(intVector pp, arraydata_t arrayclass, int verbose=1) -> array_transformation_t"""
+    r""" From a relabelling of the graph return the corresponding array transformation"""
     return _oalib.oagraph2transformation(pp, arrayclass, verbose)
 class depth_path_t(object):
     r"""
 
     `depth_path_t()`
 
     structure containing current position in search tree
@@ -8069,18 +8330,18 @@
 
     C++ includes: evenodd.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    ncurr = property(_oalib.depth_path_t_ncurr_get, _oalib.depth_path_t_ncurr_set, doc=r"""ncurr : std::vector<(int,std::allocator<(int)>)>""")
-    nmax = property(_oalib.depth_path_t_nmax_get, _oalib.depth_path_t_nmax_set, doc=r"""nmax : std::vector<(int,std::allocator<(int)>)>""")
-    necols = property(_oalib.depth_path_t_necols_get, _oalib.depth_path_t_necols_set, doc=r"""necols : std::vector<(int,std::allocator<(int)>)>""")
-    ngecols = property(_oalib.depth_path_t_ngecols_get, _oalib.depth_path_t_ngecols_set, doc=r"""ngecols : std::vector<(int,std::allocator<(int)>)>""")
+    ncurr = property(_oalib.depth_path_t_ncurr_get, _oalib.depth_path_t_ncurr_set, doc=r""" vector with current position""")
+    nmax = property(_oalib.depth_path_t_nmax_get, _oalib.depth_path_t_nmax_set, doc=r""" vector with target""")
+    necols = property(_oalib.depth_path_t_necols_get, _oalib.depth_path_t_necols_set, doc=r""" number of extension columns""")
+    ngecols = property(_oalib.depth_path_t_ngecols_get, _oalib.depth_path_t_ngecols_set, doc=r""" number of good extension columns""")
     depthstart = property(_oalib.depth_path_t_depthstart_get, _oalib.depth_path_t_depthstart_set, doc=r"""depthstart : int""")
 
     def __init__(self):
         r"""
         __init__(depth_path_t self) -> depth_path_t
 
 
@@ -8209,15 +8470,14 @@
 
         """
         return _oalib.counter_t_showcounts(self, *args)
     __swig_destroy__ = _oalib.delete_counter_t
 
 # Register counter_t in _oalib:
 _oalib.counter_t_swigregister(counter_t)
-
 class depth_extend_sub_t(object):
     r"""
 
     `depth_extend_sub_t(nn=0)`
 
     Helper structure for dynamic extension
 
@@ -8243,15 +8503,15 @@
     C++ includes: evenodd.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     lmctype = property(_oalib.depth_extend_sub_t_lmctype_get, _oalib.depth_extend_sub_t_lmctype_set, doc=r"""lmctype : std::vector<(int,std::allocator<(int)>)>""")
-    lastcol = property(_oalib.depth_extend_sub_t_lastcol_get, _oalib.depth_extend_sub_t_lastcol_set, doc=r"""lastcol : std::vector<(int,std::allocator<(int)>)>""")
+    lastcol = property(_oalib.depth_extend_sub_t_lastcol_get, _oalib.depth_extend_sub_t_lastcol_set, doc=r""" last column changed in lmc check""")
     strengthcheck = property(_oalib.depth_extend_sub_t_strengthcheck_get, _oalib.depth_extend_sub_t_strengthcheck_set, doc=r"""strengthcheck : std::vector<(double,std::allocator<(double)>)>""")
     valididx = property(_oalib.depth_extend_sub_t_valididx_get, _oalib.depth_extend_sub_t_valididx_set, doc=r"""valididx : std::vector<(int,std::allocator<(int)>)>""")
     verbose = property(_oalib.depth_extend_sub_t_verbose_get, _oalib.depth_extend_sub_t_verbose_set, doc=r"""verbose : int""")
 
     def __init__(self, nn=0):
         r"""
         __init__(depth_extend_sub_t self, int nn=0) -> depth_extend_sub_t
@@ -8319,15 +8579,14 @@
 
         """
         return _oalib.depth_extend_sub_t_info(self)
     __swig_destroy__ = _oalib.delete_depth_extend_sub_t
 
 # Register depth_extend_sub_t in _oalib:
 _oalib.depth_extend_sub_t_swigregister(depth_extend_sub_t)
-
 class depth_extend_t(object):
     r"""
 
     `depth_extend_t(ad_, _logtime=10000000, _discardJ5=-1)`
     `depth_extend_t(de)`
 
     Helper structure for dynamic extension.
@@ -8381,19 +8640,19 @@
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     verbose = property(_oalib.depth_extend_t_verbose_get, _oalib.depth_extend_t_verbose_set, doc=r"""verbose : int""")
     oaextend = property(_oalib.depth_extend_t_oaextend_get, _oalib.depth_extend_t_oaextend_set, doc=r"""oaextend : OAextend""")
     ad = property(_oalib.depth_extend_t_ad_get, _oalib.depth_extend_t_ad_set, doc=r"""ad : p.q(const).arraydata_t""")
     loglevelcol = property(_oalib.depth_extend_t_loglevelcol_get, _oalib.depth_extend_t_loglevelcol_set, doc=r"""loglevelcol : int""")
-    logtime = property(_oalib.depth_extend_t_logtime_get, _oalib.depth_extend_t_logtime_set, doc=r"""logtime : double""")
+    logtime = property(_oalib.depth_extend_t_logtime_get, _oalib.depth_extend_t_logtime_set, doc=r""" print progress every x seconds""")
     extension_column_list = property(_oalib.depth_extend_t_extension_column_list_get, _oalib.depth_extend_t_extension_column_list_set, doc=r"""extension_column_list : arraylist_t""")
-    writearrays = property(_oalib.depth_extend_t_writearrays_get, _oalib.depth_extend_t_writearrays_set, doc=r"""writearrays : int""")
+    writearrays = property(_oalib.depth_extend_t_writearrays_get, _oalib.depth_extend_t_writearrays_set, doc=r""" if set to true write arrays to disk""")
     discardJ5 = property(_oalib.depth_extend_t_discardJ5_get, _oalib.depth_extend_t_discardJ5_set, doc=r"""discardJ5 : int""")
-    discardJ5number = property(_oalib.depth_extend_t_discardJ5number_get, _oalib.depth_extend_t_discardJ5number_set, doc=r"""discardJ5number : long""")
+    discardJ5number = property(_oalib.depth_extend_t_discardJ5number_get, _oalib.depth_extend_t_discardJ5number_set, doc=r""" if true, then we discard the designs which have J5 maximal""")
     arraywriter = property(_oalib.depth_extend_t_arraywriter_get, _oalib.depth_extend_t_arraywriter_set, doc=r"""arraywriter : p.arraywriter_t""")
     counter = property(_oalib.depth_extend_t_counter_get, _oalib.depth_extend_t_counter_set, doc=r"""counter : p.counter_t""")
     t0 = property(_oalib.depth_extend_t_t0_get, _oalib.depth_extend_t_t0_set, doc=r"""t0 : double""")
     tp = property(_oalib.depth_extend_t_tp_get, _oalib.depth_extend_t_tp_set, doc=r"""tp : double""")
 
     def __init__(self, *args):
         r"""
@@ -8473,15 +8732,14 @@
         set the position in the dextend structure
 
         """
         return _oalib.depth_extend_t_setpositionGEC(self, k, goodextensioncols)
 
 # Register depth_extend_t in _oalib:
 _oalib.depth_extend_t_swigregister(depth_extend_t)
-
 DEPTH_DIRECT = _oalib.DEPTH_DIRECT
 
 DEPTH_EXTENSIONS = _oalib.DEPTH_EXTENSIONS
 
 class depth_extensions_storage_t(object):
     r"""
 
@@ -8547,15 +8805,14 @@
         """
         _oalib.depth_extensions_storage_t_swiginit(self, _oalib.new_depth_extensions_storage_t())
     __swig_destroy__ = _oalib.delete_depth_extensions_storage_t
 
 # Register depth_extensions_storage_t in _oalib:
 _oalib.depth_extensions_storage_t_swigregister(depth_extensions_storage_t)
 
-
 def processDepth(goodarrays, depthalg, dextend, dextendsublight, extensioncol, verbose=0):
     r"""
     processDepth(arraylist_t goodarrays, depth_alg_t depthalg, depth_extend_t dextend, depth_extend_sub_t dextendsublight, int extensioncol, int verbose=0)
 
 
     Extend arrays using a depth-first or breadth-first approach
 
@@ -8643,16 +8900,16 @@
 
     C++ includes: evenodd.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    k = property(_oalib.jindex_t_k_get, _oalib.jindex_t_k_set, doc=r"""k : int""")
-    j = property(_oalib.jindex_t_j_get, _oalib.jindex_t_j_set, doc=r"""j : int""")
+    k = property(_oalib.jindex_t_k_get, _oalib.jindex_t_k_set, doc=r""" number of columns""")
+    j = property(_oalib.jindex_t_j_get, _oalib.jindex_t_j_set, doc=r""" J-value""")
 
     def __init__(self, colindex, jvalue):
         r"""
         __init__(jindex_t self, int colindex, int jvalue) -> jindex_t
 
 
         """
@@ -8669,15 +8926,14 @@
 
         """
         return _oalib.jindex_t_toString(self)
     __swig_destroy__ = _oalib.delete_jindex_t
 
 # Register jindex_t in _oalib:
 _oalib.jindex_t_swigregister(jindex_t)
-
 class Jcounter(object):
     r"""
 
     `Jcounter()`
     `Jcounter(N, jj=5, k=-1)`
 
     object to hold counts of maximum J_k-values
@@ -8704,19 +8960,19 @@
 
     C++ includes: evenodd.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    N = property(_oalib.Jcounter_N_get, _oalib.Jcounter_N_set, doc=r"""N : int""")
+    N = property(_oalib.Jcounter_N_get, _oalib.Jcounter_N_set, doc=r""" number of rows""")
     jj = property(_oalib.Jcounter_jj_get, _oalib.Jcounter_jj_set, doc=r"""jj : int""")
     fvals = property(_oalib.Jcounter_fvals_get, _oalib.Jcounter_fvals_set, doc=r"""fvals : std::vector<(int,std::allocator<(int)>)>""")
     maxJcounts = property(_oalib.Jcounter_maxJcounts_get, _oalib.Jcounter_maxJcounts_set, doc=r"""maxJcounts : std::map<(jindex_t,long,std::less<(jindex_t)>,std::allocator<(std::pair<(q(const).jindex_t,long)>)>)>""")
-    dt = property(_oalib.Jcounter_dt_get, _oalib.Jcounter_dt_set, doc=r"""dt : double""")
+    dt = property(_oalib.Jcounter_dt_get, _oalib.Jcounter_dt_set, doc=r""" time needed for calculation""")
 
     def __init__(self, *args):
         r"""
         __init__(Jcounter self) -> Jcounter
         __init__(Jcounter self, int N, int jj=5, int k=-1) -> Jcounter
 
 
@@ -8841,15 +9097,14 @@
         """
         return _oalib.Jcounter_addArray(self, al, verbose)
     __swig_destroy__ = _oalib.delete_Jcounter
 
 # Register Jcounter in _oalib:
 _oalib.Jcounter_swigregister(Jcounter)
 
-
 def readStatisticsFile(numbersfile, verbose):
     r"""
     readStatisticsFile(char const * numbersfile, int verbose) -> Jcounter
 
 
     read statistics object from disk
 
@@ -8987,26 +9242,26 @@
         if true then J3 values should be zero
 
     C++ includes: conference.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    N = property(_oalib.conference_t_N_get, _oalib.conference_t_N_set, doc=r"""N : rowindex_t""")
-    ncols = property(_oalib.conference_t_ncols_get, _oalib.conference_t_ncols_set, doc=r"""ncols : colindex_t""")
+    N = property(_oalib.conference_t_N_get, _oalib.conference_t_N_set, doc=r""" number of runs""")
+    ncols = property(_oalib.conference_t_ncols_get, _oalib.conference_t_ncols_set, doc=r""" total number of columns (factors) in the design""")
     CONFERENCE_NORMAL = _oalib.conference_t_CONFERENCE_NORMAL
     r""" normal conference design"""
     CONFERENCE_DIAGONAL = _oalib.conference_t_CONFERENCE_DIAGONAL
     r""" conference design with zeros only on diagonal"""
     DCONFERENCE = _oalib.conference_t_DCONFERENCE
     r""" double conference design"""
-    ctype = property(_oalib.conference_t_ctype_get, _oalib.conference_t_ctype_set, doc=r"""ctype : conference_t::conference_type""")
-    itype = property(_oalib.conference_t_itype_get, _oalib.conference_t_itype_set, doc=r"""itype : matrix_isomorphism_t""")
-    j1zero = property(_oalib.conference_t_j1zero_get, _oalib.conference_t_j1zero_set, doc=r"""j1zero : bool""")
-    j3zero = property(_oalib.conference_t_j3zero_get, _oalib.conference_t_j3zero_set, doc=r"""j3zero : bool""")
+    ctype = property(_oalib.conference_t_ctype_get, _oalib.conference_t_ctype_set, doc=r""" defines the type of designs""")
+    itype = property(_oalib.conference_t_itype_get, _oalib.conference_t_itype_set, doc=r""" defines the isomorphism type""")
+    j1zero = property(_oalib.conference_t_j1zero_get, _oalib.conference_t_j1zero_set, doc=r""" if true then J1 values should be zero""")
+    j3zero = property(_oalib.conference_t_j3zero_get, _oalib.conference_t_j3zero_set, doc=r""" if true then J3 values should be zero""")
 
     def __init__(self, *args):
         r"""
         __init__(conference_t self) -> conference_t
         __init__(conference_t self, int N, int k, int j1zero) -> conference_t
         __init__(conference_t self, conference_t rhs) -> conference_t
 
@@ -9074,15 +9329,14 @@
         """
         return _oalib.conference_t___repr__(self)
     __swig_destroy__ = _oalib.delete_conference_t
 
 # Register conference_t in _oalib:
 _oalib.conference_t_swigregister(conference_t)
 
-
 def reduceConference(arg1, verbose=0):
     r"""
     reduceConference(array_link arg1, int verbose=0) -> array_link
 
 
     Reduce conference matrix to normal form using Nauty
 
@@ -9151,18 +9405,18 @@
 
     C++ includes: conference.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    ct = property(_oalib.CandidateGeneratorBase_ct_get, _oalib.CandidateGeneratorBase_ct_set, doc=r"""ct : conference_t""")
-    verbose = property(_oalib.CandidateGeneratorBase_verbose_get, _oalib.CandidateGeneratorBase_verbose_set, doc=r"""verbose : int""")
-    al = property(_oalib.CandidateGeneratorBase_al_get, _oalib.CandidateGeneratorBase_al_set, doc=r"""al : array_link""")
-    last_valid = property(_oalib.CandidateGeneratorBase_last_valid_get, _oalib.CandidateGeneratorBase_last_valid_set, doc=r"""last_valid : int""")
+    ct = property(_oalib.CandidateGeneratorBase_ct_get, _oalib.CandidateGeneratorBase_ct_set, doc=r""" type of designs to generate""")
+    verbose = property(_oalib.CandidateGeneratorBase_verbose_get, _oalib.CandidateGeneratorBase_verbose_set, doc=r""" verbosity level""")
+    al = property(_oalib.CandidateGeneratorBase_al_get, _oalib.CandidateGeneratorBase_al_set, doc=r""" last array analyzed""")
+    last_valid = property(_oalib.CandidateGeneratorBase_last_valid_get, _oalib.CandidateGeneratorBase_last_valid_set, doc=r""" index of last valid column""")
 
     def __init__(self, al, ct):
         r"""
         __init__(CandidateGeneratorBase self, array_link al, conference_t ct) -> CandidateGeneratorBase
 
 
         """
@@ -9187,15 +9441,14 @@
 
         """
         return _oalib.CandidateGeneratorBase_candidates(self, k)
     __swig_destroy__ = _oalib.delete_CandidateGeneratorBase
 
 # Register CandidateGeneratorBase in _oalib:
 _oalib.CandidateGeneratorBase_swigregister(CandidateGeneratorBase)
-
 class CandidateGeneratorConference(CandidateGeneratorBase):
     r"""
 
     `CandidateGeneratorConference(al, ct)`
 
     Class to generate conference candidate extensions.
 
@@ -9237,15 +9490,14 @@
 
         """
         return _oalib.CandidateGeneratorConference_generateCandidatesZero(self, al, kz)
     __swig_destroy__ = _oalib.delete_CandidateGeneratorConference
 
 # Register CandidateGeneratorConference in _oalib:
 _oalib.CandidateGeneratorConference_swigregister(CandidateGeneratorConference)
-
 class CandidateGeneratorDouble(CandidateGeneratorBase):
     r"""
 
     `CandidateGeneratorDouble(al, ct)`
 
     Class to generate double conference candidate extensions with caching.
 
@@ -9280,15 +9532,14 @@
 
         """
         return _oalib.CandidateGeneratorDouble_generateCandidates(self, al)
     __swig_destroy__ = _oalib.delete_CandidateGeneratorDouble
 
 # Register CandidateGeneratorDouble in _oalib:
 _oalib.CandidateGeneratorDouble_swigregister(CandidateGeneratorDouble)
-
 class conference_extend_t(object):
     r"""
 
 
     Helper structure containing extensions of conference designs
 
     Attributes
@@ -9304,16 +9555,16 @@
     C++ includes: conference.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     first = property(_oalib.conference_extend_t_first_get, _oalib.conference_extend_t_first_set, doc=r"""first : std::vector<(conference_column,std::allocator<(conference_column)>)>""")
-    second = property(_oalib.conference_extend_t_second_get, _oalib.conference_extend_t_second_set, doc=r"""second : std::vector<(conference_column,std::allocator<(conference_column)>)>""")
-    extensions = property(_oalib.conference_extend_t_extensions_get, _oalib.conference_extend_t_extensions_set, doc=r"""extensions : std::vector<(conference_column,std::allocator<(conference_column)>)>""")
+    second = property(_oalib.conference_extend_t_second_get, _oalib.conference_extend_t_second_set, doc=r""" list of first block candidate extensions""")
+    extensions = property(_oalib.conference_extend_t_extensions_get, _oalib.conference_extend_t_extensions_set, doc=r""" list of first block candidate extensions""")
 
     def combine(self, i, j):
         r"""
         combine(conference_extend_t self, int i, int j) -> charVector
 
 
         list of candidate extensions
@@ -9361,15 +9612,14 @@
         """
         _oalib.conference_extend_t_swiginit(self, _oalib.new_conference_extend_t())
     __swig_destroy__ = _oalib.delete_conference_extend_t
 
 # Register conference_extend_t in _oalib:
 _oalib.conference_extend_t_swigregister(conference_extend_t)
 
-
 def extend_conference_matrix(design, conference_type, extcol, verbose=1, maxzpos=-1):
     r"""
     extend_conference_matrix(array_link design, conference_t conference_type, int extcol, int verbose=1, int maxzpos=-1) -> conference_extend_t
 
 
     Extend a single conference design with candidate columns
 
@@ -9780,21 +10030,21 @@
     C++ includes: conference.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     als = property(_oalib.DconferenceFilter_als_get, _oalib.DconferenceFilter_als_set, doc=r"""als : array_link""")
-    filtersymm = property(_oalib.DconferenceFilter_filtersymm_get, _oalib.DconferenceFilter_filtersymm_set, doc=r"""filtersymm : int""")
-    filterj2 = property(_oalib.DconferenceFilter_filterj2_get, _oalib.DconferenceFilter_filterj2_set, doc=r"""filterj2 : int""")
-    filterj3 = property(_oalib.DconferenceFilter_filterj3_get, _oalib.DconferenceFilter_filterj3_set, doc=r"""filterj3 : int""")
-    filterfirst = property(_oalib.DconferenceFilter_filterfirst_get, _oalib.DconferenceFilter_filterfirst_set, doc=r"""filterfirst : int""")
-    filterzero = property(_oalib.DconferenceFilter_filterzero_get, _oalib.DconferenceFilter_filterzero_set, doc=r"""filterzero : int""")
+    filtersymm = property(_oalib.DconferenceFilter_filtersymm_get, _oalib.DconferenceFilter_filtersymm_set, doc=r""" filter based on symmetry""")
+    filterj2 = property(_oalib.DconferenceFilter_filterj2_get, _oalib.DconferenceFilter_filterj2_set, doc=r""" filter based on j2 value""")
+    filterj3 = property(_oalib.DconferenceFilter_filterj3_get, _oalib.DconferenceFilter_filterj3_set, doc=r""" filter based on j3 value""")
+    filterfirst = property(_oalib.DconferenceFilter_filterfirst_get, _oalib.DconferenceFilter_filterfirst_set, doc=r""" filter only columns with first value >=0""")
+    filterzero = property(_oalib.DconferenceFilter_filterzero_get, _oalib.DconferenceFilter_filterzero_set, doc=r""" filter based on first occurence of zero in a column""")
     ngood = property(_oalib.DconferenceFilter_ngood_get, _oalib.DconferenceFilter_ngood_set, doc=r"""ngood : long""")
-    inline_row = property(_oalib.DconferenceFilter_inline_row_get, _oalib.DconferenceFilter_inline_row_set, doc=r"""inline_row : int""")
+    inline_row = property(_oalib.DconferenceFilter_inline_row_get, _oalib.DconferenceFilter_inline_row_set, doc=r""" row at which infile filtering is performed""")
     sd = property(_oalib.DconferenceFilter_sd_get, _oalib.DconferenceFilter_sd_set, doc=r"""sd : symmdata""")
 
     def __init__(self, _als, filter_symmetry, filterj2_, filterj3_=1):
         r"""
         __init__(DconferenceFilter self, array_link _als, int filter_symmetry, int filterj2_, int filterj3_=1) -> DconferenceFilter
 
 
@@ -9971,15 +10221,14 @@
         """
         return _oalib.DconferenceFilter_filterZero(self, c)
     __swig_destroy__ = _oalib.delete_DconferenceFilter
 
 # Register DconferenceFilter in _oalib:
 _oalib.DconferenceFilter_swigregister(DconferenceFilter)
 
-
 def unittest_reduceConferenceTransformation():
     r"""
     unittest_reduceConferenceTransformation() -> int
 
 
     """
     return _oalib.unittest_reduceConferenceTransformation()
@@ -10076,15 +10325,14 @@
             self.first = val
         else:
             self.second = val
     __swig_destroy__ = _oalib.delete_pairDoptimize
 
 # Register pairDoptimize in _oalib:
 _oalib.pairDoptimize_swigregister(pairDoptimize)
-
 class pairGraphColors(object):
     r"""Proxy of C++ std::pair< array_link,std::vector< int > > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
@@ -10110,15 +10358,14 @@
             self.first = val
         else:
             self.second = val
     __swig_destroy__ = _oalib.delete_pairGraphColors
 
 # Register pairGraphColors in _oalib:
 _oalib.pairGraphColors_swigregister(pairGraphColors)
-
 class pairEigenMatrix(object):
     r"""Proxy of C++ std::pair< MatrixFloat,MatrixFloat > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def __init__(self, *args):
@@ -10144,15 +10391,14 @@
             self.first = val
         else:
             self.second = val
     __swig_destroy__ = _oalib.delete_pairEigenMatrix
 
 # Register pairEigenMatrix in _oalib:
 _oalib.pairEigenMatrix_swigregister(pairEigenMatrix)
-
 class mvalue_t_long(object):
     r"""
 
 
     Multi-value type.
 
     This object represents a multi-valued object. The objects are ordered using
@@ -10168,20 +10414,20 @@
 
     C++ includes: mathtools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    values = property(_oalib.mvalue_t_long_values_get, _oalib.mvalue_t_long_values_set, doc=r"""values : std::vector<(long,std::allocator<(long)>)>""")
+    values = property(_oalib.mvalue_t_long_values_get, _oalib.mvalue_t_long_values_set, doc=r""" vector containing the values""")
     direction_t_HIGH = _oalib.mvalue_t_long_direction_t_HIGH
     r""" Order from high to low values"""
     direction_t_LOW = _oalib.mvalue_t_long_direction_t_LOW
     r""" Order from low to high values"""
-    ordering = property(_oalib.mvalue_t_long_ordering_get, _oalib.mvalue_t_long_ordering_set, doc=r"""ordering : mvalue_t<(long)>::direction_t""")
+    ordering = property(_oalib.mvalue_t_long_ordering_get, _oalib.mvalue_t_long_ordering_set, doc=r""" value representing the ordering used""")
     __swig_destroy__ = _oalib.delete_mvalue_t_long
 
     def __init__(self, *args):
         r"""
         __init__(mvalue_t_long self) -> mvalue_t_long
         __init__(mvalue_t_long self, long element, mvalue_t< long >::direction_t dd=mvalue_t< long >::direction_t::HIGH) -> mvalue_t_long
         __init__(mvalue_t_long self, longVector elements, mvalue_t< long >::direction_t dd=mvalue_t< long >::direction_t::HIGH) -> mvalue_t_long
@@ -10216,15 +10462,15 @@
         size(mvalue_t_long self) -> size_t
 
 
         """
         return _oalib.mvalue_t_long_size(self)
 
     def __eq__(self, rhs):
-        r"""__eq__(mvalue_t_long self, mvalue_t_long rhs) -> bool"""
+        r""" comparison operator"""
         return _oalib.mvalue_t_long___eq__(self, rhs)
 
     def __ne__(self, rhs):
         r"""__ne__(mvalue_t_long self, mvalue_t_long rhs) -> bool"""
         return _oalib.mvalue_t_long___ne__(self, rhs)
 
     def __le__(self, rhs):
@@ -10261,15 +10507,14 @@
         return a string representation of the object
 
         """
         return _oalib.mvalue_t_long_string_representation(self, *args)
 
 # Register mvalue_t_long in _oalib:
 _oalib.mvalue_t_long_swigregister(mvalue_t_long)
-
 class mvalue_t_double(object):
     r"""
 
 
     Multi-value type.
 
     This object represents a multi-valued object. The objects are ordered using
@@ -10285,20 +10530,20 @@
 
     C++ includes: mathtools.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
-    values = property(_oalib.mvalue_t_double_values_get, _oalib.mvalue_t_double_values_set, doc=r"""values : std::vector<(double,std::allocator<(double)>)>""")
+    values = property(_oalib.mvalue_t_double_values_get, _oalib.mvalue_t_double_values_set, doc=r""" vector containing the values""")
     direction_t_HIGH = _oalib.mvalue_t_double_direction_t_HIGH
     r""" Order from high to low values"""
     direction_t_LOW = _oalib.mvalue_t_double_direction_t_LOW
     r""" Order from low to high values"""
-    ordering = property(_oalib.mvalue_t_double_ordering_get, _oalib.mvalue_t_double_ordering_set, doc=r"""ordering : mvalue_t<(double)>::direction_t""")
+    ordering = property(_oalib.mvalue_t_double_ordering_get, _oalib.mvalue_t_double_ordering_set, doc=r""" value representing the ordering used""")
     __swig_destroy__ = _oalib.delete_mvalue_t_double
 
     def __init__(self, *args):
         r"""
         __init__(mvalue_t_double self) -> mvalue_t_double
         __init__(mvalue_t_double self, double element, mvalue_t< double >::direction_t dd=mvalue_t< double >::direction_t::HIGH) -> mvalue_t_double
         __init__(mvalue_t_double self, doubleVector elements, mvalue_t< double >::direction_t dd=mvalue_t< double >::direction_t::HIGH) -> mvalue_t_double
@@ -10333,15 +10578,15 @@
         size(mvalue_t_double self) -> size_t
 
 
         """
         return _oalib.mvalue_t_double_size(self)
 
     def __eq__(self, rhs):
-        r"""__eq__(mvalue_t_double self, mvalue_t_double rhs) -> bool"""
+        r""" comparison operator"""
         return _oalib.mvalue_t_double___eq__(self, rhs)
 
     def __ne__(self, rhs):
         r"""__ne__(mvalue_t_double self, mvalue_t_double rhs) -> bool"""
         return _oalib.mvalue_t_double___ne__(self, rhs)
 
     def __le__(self, rhs):
@@ -10394,15 +10639,14 @@
           raise AttributeError("%r object has no attribute %r" %
                              (self.__class__, attr))
 
 
 
 # Register mvalue_t_double in _oalib:
 _oalib.mvalue_t_double_swigregister(mvalue_t_double)
-
 class ParetoLongLong(object):
     r"""
 
 
     Class to the calculate Pareto optimal elements.
 
     The class is templated by the type of values to be compared and an index type.
@@ -10419,16 +10663,16 @@
         contains a list of all Pareto optimal elements
 
     C++ includes: pareto.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    verbose = property(_oalib.ParetoLongLong_verbose_get, _oalib.ParetoLongLong_verbose_set, doc=r"""verbose : int""")
-    elements = property(_oalib.ParetoLongLong_elements_get, _oalib.ParetoLongLong_elements_set, doc=r"""elements : std::deque<(pareto_element<(long,long)>,std::allocator<(pareto_element<(long,long)>)>)>""")
+    verbose = property(_oalib.ParetoLongLong_verbose_get, _oalib.ParetoLongLong_verbose_set, doc=r""" Verbosity level""")
+    elements = property(_oalib.ParetoLongLong_elements_get, _oalib.ParetoLongLong_elements_set, doc=r""" contains a list of all Pareto optimal elements""")
 
     def __init__(self):
         r"""
         __init__(ParetoLongLong self) -> ParetoLongLong
 
 
         Create an empty Pareto class.
@@ -10524,25 +10768,14 @@
         add a new element
 
         """
         return _oalib.ParetoLongLong_addvalue(self, value, idx)
 
 # Register ParetoLongLong in _oalib:
 _oalib.ParetoLongLong_swigregister(ParetoLongLong)
-
-def ParetoLongLong_showvalue(p):
-    r"""
-    ParetoLongLong_showvalue(longVector p)
-
-
-    show a Pareto element
-
-    """
-    return _oalib.ParetoLongLong_showvalue(p)
-
 class ParetoMultiLongLong(object):
     r"""
 
 
     Class to the calculate Pareto optimal elements.
 
     The class is templated by the type of values to be compared and an index type.
@@ -10559,16 +10792,16 @@
         contains a list of all Pareto optimal elements
 
     C++ includes: pareto.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    verbose = property(_oalib.ParetoMultiLongLong_verbose_get, _oalib.ParetoMultiLongLong_verbose_set, doc=r"""verbose : int""")
-    elements = property(_oalib.ParetoMultiLongLong_elements_get, _oalib.ParetoMultiLongLong_elements_set, doc=r"""elements : std::deque<(pareto_element<(mvalue_t<(long)>,long)>,std::allocator<(pareto_element<(mvalue_t<(long)>,long)>)>)>""")
+    verbose = property(_oalib.ParetoMultiLongLong_verbose_get, _oalib.ParetoMultiLongLong_verbose_set, doc=r""" Verbosity level""")
+    elements = property(_oalib.ParetoMultiLongLong_elements_get, _oalib.ParetoMultiLongLong_elements_set, doc=r""" contains a list of all Pareto optimal elements""")
 
     def __init__(self):
         r"""
         __init__(ParetoMultiLongLong self) -> ParetoMultiLongLong
 
 
         Create an empty Pareto class.
@@ -10664,25 +10897,14 @@
         add a new element
 
         """
         return _oalib.ParetoMultiLongLong_addvalue(self, value, idx)
 
 # Register ParetoMultiLongLong in _oalib:
 _oalib.ParetoMultiLongLong_swigregister(ParetoMultiLongLong)
-
-def ParetoMultiLongLong_showvalue(p):
-    r"""
-    ParetoMultiLongLong_showvalue(vector_mvalue_t_long p)
-
-
-    show a Pareto element
-
-    """
-    return _oalib.ParetoMultiLongLong_showvalue(p)
-
 class ParetoMultiDoubleLong(object):
     r"""
 
 
     Class to the calculate Pareto optimal elements.
 
     The class is templated by the type of values to be compared and an index type.
@@ -10699,16 +10921,16 @@
         contains a list of all Pareto optimal elements
 
     C++ includes: pareto.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    verbose = property(_oalib.ParetoMultiDoubleLong_verbose_get, _oalib.ParetoMultiDoubleLong_verbose_set, doc=r"""verbose : int""")
-    elements = property(_oalib.ParetoMultiDoubleLong_elements_get, _oalib.ParetoMultiDoubleLong_elements_set, doc=r"""elements : std::deque<(pareto_element<(mvalue_t<(double)>,long)>,std::allocator<(pareto_element<(mvalue_t<(double)>,long)>)>)>""")
+    verbose = property(_oalib.ParetoMultiDoubleLong_verbose_get, _oalib.ParetoMultiDoubleLong_verbose_set, doc=r""" Verbosity level""")
+    elements = property(_oalib.ParetoMultiDoubleLong_elements_get, _oalib.ParetoMultiDoubleLong_elements_set, doc=r""" contains a list of all Pareto optimal elements""")
 
     def __init__(self):
         r"""
         __init__(ParetoMultiDoubleLong self) -> ParetoMultiDoubleLong
 
 
         Create an empty Pareto class.
@@ -10804,25 +11026,14 @@
         add a new element
 
         """
         return _oalib.ParetoMultiDoubleLong_addvalue(self, value, idx)
 
 # Register ParetoMultiDoubleLong in _oalib:
 _oalib.ParetoMultiDoubleLong_swigregister(ParetoMultiDoubleLong)
-
-def ParetoMultiDoubleLong_showvalue(p):
-    r"""
-    ParetoMultiDoubleLong_showvalue(vector_mvalue_t_double p)
-
-
-    show a Pareto element
-
-    """
-    return _oalib.ParetoMultiDoubleLong_showvalue(p)
-
 class ParetoDoubleLong(object):
     r"""
 
 
     Class to the calculate Pareto optimal elements.
 
     The class is templated by the type of values to be compared and an index type.
@@ -10839,16 +11050,16 @@
         contains a list of all Pareto optimal elements
 
     C++ includes: pareto.h
 
     """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
-    verbose = property(_oalib.ParetoDoubleLong_verbose_get, _oalib.ParetoDoubleLong_verbose_set, doc=r"""verbose : int""")
-    elements = property(_oalib.ParetoDoubleLong_elements_get, _oalib.ParetoDoubleLong_elements_set, doc=r"""elements : std::deque<(pareto_element<(double,long)>,std::allocator<(pareto_element<(double,long)>)>)>""")
+    verbose = property(_oalib.ParetoDoubleLong_verbose_get, _oalib.ParetoDoubleLong_verbose_set, doc=r""" Verbosity level""")
+    elements = property(_oalib.ParetoDoubleLong_elements_get, _oalib.ParetoDoubleLong_elements_set, doc=r""" contains a list of all Pareto optimal elements""")
 
     def __init__(self):
         r"""
         __init__(ParetoDoubleLong self) -> ParetoDoubleLong
 
 
         Create an empty Pareto class.
@@ -10944,25 +11155,14 @@
         add a new element
 
         """
         return _oalib.ParetoDoubleLong_addvalue(self, value, idx)
 
 # Register ParetoDoubleLong in _oalib:
 _oalib.ParetoDoubleLong_swigregister(ParetoDoubleLong)
-
-def ParetoDoubleLong_showvalue(p):
-    r"""
-    ParetoDoubleLong_showvalue(doubleVector p)
-
-
-    show a Pareto element
-
-    """
-    return _oalib.ParetoDoubleLong_showvalue(p)
-
 class ParetoElementLong(object):
     r"""
 
 
     helper class for the Pareto class to hold elements
 
     Attributes
@@ -11027,15 +11227,14 @@
 
         """
         _oalib.ParetoElementLong_swiginit(self, _oalib.new_ParetoElementLong())
     __swig_destroy__ = _oalib.delete_ParetoElementLong
 
 # Register ParetoElementLong in _oalib:
 _oalib.ParetoElementLong_swigregister(ParetoElementLong)
-
 class ParetoMElementLong(object):
     r"""
 
 
     helper class for the Pareto class to hold elements
 
     Attributes
@@ -11100,15 +11299,14 @@
 
         """
         _oalib.ParetoMElementLong_swiginit(self, _oalib.new_ParetoMElementLong())
     __swig_destroy__ = _oalib.delete_ParetoMElementLong
 
 # Register ParetoMElementLong in _oalib:
 _oalib.ParetoMElementLong_swigregister(ParetoMElementLong)
-
 class vector_mvalue_t_double(object):
     r"""Proxy of C++ std::vector< mvalue_t< double > > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -11143,29 +11341,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(vector_mvalue_t_double self, std::vector< mvalue_t< double > >::difference_type i, std::vector< mvalue_t< double > >::difference_type j)"""
         return _oalib.vector_mvalue_t_double___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(vector_mvalue_t_double self, std::vector< mvalue_t< double > >::difference_type i)
-        __delitem__(vector_mvalue_t_double self, PySliceObject * slice)
+        __delitem__(vector_mvalue_t_double self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.vector_mvalue_t_double___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(vector_mvalue_t_double self, PySliceObject * slice) -> vector_mvalue_t_double
+        __getitem__(vector_mvalue_t_double self, SWIGPY_SLICEOBJECT * slice) -> vector_mvalue_t_double
         __getitem__(vector_mvalue_t_double self, std::vector< mvalue_t< double > >::difference_type i) -> mvalue_t_double
         """
         return _oalib.vector_mvalue_t_double___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(vector_mvalue_t_double self, PySliceObject * slice, vector_mvalue_t_double v)
-        __setitem__(vector_mvalue_t_double self, PySliceObject * slice)
+        __setitem__(vector_mvalue_t_double self, SWIGPY_SLICEOBJECT * slice, vector_mvalue_t_double v)
+        __setitem__(vector_mvalue_t_double self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(vector_mvalue_t_double self, std::vector< mvalue_t< double > >::difference_type i, mvalue_t_double x)
         """
         return _oalib.vector_mvalue_t_double___setitem__(self, *args)
 
     def pop(self):
         r"""pop(vector_mvalue_t_double self) -> mvalue_t_double"""
         return _oalib.vector_mvalue_t_double_pop(self)
@@ -11267,15 +11465,14 @@
     def capacity(self):
         r"""capacity(vector_mvalue_t_double self) -> std::vector< mvalue_t< double > >::size_type"""
         return _oalib.vector_mvalue_t_double_capacity(self)
     __swig_destroy__ = _oalib.delete_vector_mvalue_t_double
 
 # Register vector_mvalue_t_double in _oalib:
 _oalib.vector_mvalue_t_double_swigregister(vector_mvalue_t_double)
-
 class vector_mvalue_t_int(object):
     r"""Proxy of C++ std::vector< mvalue_t< int > > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -11310,29 +11507,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(vector_mvalue_t_int self, std::vector< mvalue_t< int > >::difference_type i, std::vector< mvalue_t< int > >::difference_type j)"""
         return _oalib.vector_mvalue_t_int___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(vector_mvalue_t_int self, std::vector< mvalue_t< int > >::difference_type i)
-        __delitem__(vector_mvalue_t_int self, PySliceObject * slice)
+        __delitem__(vector_mvalue_t_int self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.vector_mvalue_t_int___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(vector_mvalue_t_int self, PySliceObject * slice) -> vector_mvalue_t_int
+        __getitem__(vector_mvalue_t_int self, SWIGPY_SLICEOBJECT * slice) -> vector_mvalue_t_int
         __getitem__(vector_mvalue_t_int self, std::vector< mvalue_t< int > >::difference_type i) -> std::vector< mvalue_t< int > >::value_type const &
         """
         return _oalib.vector_mvalue_t_int___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(vector_mvalue_t_int self, PySliceObject * slice, vector_mvalue_t_int v)
-        __setitem__(vector_mvalue_t_int self, PySliceObject * slice)
+        __setitem__(vector_mvalue_t_int self, SWIGPY_SLICEOBJECT * slice, vector_mvalue_t_int v)
+        __setitem__(vector_mvalue_t_int self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(vector_mvalue_t_int self, std::vector< mvalue_t< int > >::difference_type i, std::vector< mvalue_t< int > >::value_type const & x)
         """
         return _oalib.vector_mvalue_t_int___setitem__(self, *args)
 
     def pop(self):
         r"""pop(vector_mvalue_t_int self) -> std::vector< mvalue_t< int > >::value_type"""
         return _oalib.vector_mvalue_t_int_pop(self)
@@ -11434,15 +11631,14 @@
     def capacity(self):
         r"""capacity(vector_mvalue_t_int self) -> std::vector< mvalue_t< int > >::size_type"""
         return _oalib.vector_mvalue_t_int_capacity(self)
     __swig_destroy__ = _oalib.delete_vector_mvalue_t_int
 
 # Register vector_mvalue_t_int in _oalib:
 _oalib.vector_mvalue_t_int_swigregister(vector_mvalue_t_int)
-
 class vector_mvalue_t_long(object):
     r"""Proxy of C++ std::vector< mvalue_t< long > > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -11477,29 +11673,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(vector_mvalue_t_long self, std::vector< mvalue_t< long > >::difference_type i, std::vector< mvalue_t< long > >::difference_type j)"""
         return _oalib.vector_mvalue_t_long___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(vector_mvalue_t_long self, std::vector< mvalue_t< long > >::difference_type i)
-        __delitem__(vector_mvalue_t_long self, PySliceObject * slice)
+        __delitem__(vector_mvalue_t_long self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.vector_mvalue_t_long___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(vector_mvalue_t_long self, PySliceObject * slice) -> vector_mvalue_t_long
+        __getitem__(vector_mvalue_t_long self, SWIGPY_SLICEOBJECT * slice) -> vector_mvalue_t_long
         __getitem__(vector_mvalue_t_long self, std::vector< mvalue_t< long > >::difference_type i) -> mvalue_t_long
         """
         return _oalib.vector_mvalue_t_long___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(vector_mvalue_t_long self, PySliceObject * slice, vector_mvalue_t_long v)
-        __setitem__(vector_mvalue_t_long self, PySliceObject * slice)
+        __setitem__(vector_mvalue_t_long self, SWIGPY_SLICEOBJECT * slice, vector_mvalue_t_long v)
+        __setitem__(vector_mvalue_t_long self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(vector_mvalue_t_long self, std::vector< mvalue_t< long > >::difference_type i, mvalue_t_long x)
         """
         return _oalib.vector_mvalue_t_long___setitem__(self, *args)
 
     def pop(self):
         r"""pop(vector_mvalue_t_long self) -> mvalue_t_long"""
         return _oalib.vector_mvalue_t_long_pop(self)
@@ -11601,15 +11797,14 @@
     def capacity(self):
         r"""capacity(vector_mvalue_t_long self) -> std::vector< mvalue_t< long > >::size_type"""
         return _oalib.vector_mvalue_t_long_capacity(self)
     __swig_destroy__ = _oalib.delete_vector_mvalue_t_long
 
 # Register vector_mvalue_t_long in _oalib:
 _oalib.vector_mvalue_t_long_swigregister(vector_mvalue_t_long)
-
 class DequeParetoElementLong(object):
     r"""Proxy of C++ std::deque< pareto_element< mvalue_t< long >,long > > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -11644,29 +11839,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(DequeParetoElementLong self, std::deque< pareto_element< mvalue_t< long >,long > >::difference_type i, std::deque< pareto_element< mvalue_t< long >,long > >::difference_type j)"""
         return _oalib.DequeParetoElementLong___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(DequeParetoElementLong self, std::deque< pareto_element< mvalue_t< long >,long > >::difference_type i)
-        __delitem__(DequeParetoElementLong self, PySliceObject * slice)
+        __delitem__(DequeParetoElementLong self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.DequeParetoElementLong___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(DequeParetoElementLong self, PySliceObject * slice) -> DequeParetoElementLong
+        __getitem__(DequeParetoElementLong self, SWIGPY_SLICEOBJECT * slice) -> DequeParetoElementLong
         __getitem__(DequeParetoElementLong self, std::deque< pareto_element< mvalue_t< long >,long > >::difference_type i) -> ParetoElementLong
         """
         return _oalib.DequeParetoElementLong___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(DequeParetoElementLong self, PySliceObject * slice, DequeParetoElementLong v)
-        __setitem__(DequeParetoElementLong self, PySliceObject * slice)
+        __setitem__(DequeParetoElementLong self, SWIGPY_SLICEOBJECT * slice, DequeParetoElementLong v)
+        __setitem__(DequeParetoElementLong self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(DequeParetoElementLong self, std::deque< pareto_element< mvalue_t< long >,long > >::difference_type i, ParetoElementLong x)
         """
         return _oalib.DequeParetoElementLong___setitem__(self, *args)
 
     def pop(self):
         r"""pop(DequeParetoElementLong self) -> ParetoElementLong"""
         return _oalib.DequeParetoElementLong_pop(self)
@@ -11768,15 +11963,14 @@
     def push_front(self, x):
         r"""push_front(DequeParetoElementLong self, ParetoElementLong x)"""
         return _oalib.DequeParetoElementLong_push_front(self, x)
     __swig_destroy__ = _oalib.delete_DequeParetoElementLong
 
 # Register DequeParetoElementLong in _oalib:
 _oalib.DequeParetoElementLong_swigregister(DequeParetoElementLong)
-
 class conference_columnVector(object):
     r"""Proxy of C++ std::vector< conference_column > class."""
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
 
     def iterator(self):
@@ -11811,29 +12005,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(conference_columnVector self, std::vector< std::vector< signed char,std::allocator< signed char > > >::difference_type i, std::vector< std::vector< signed char,std::allocator< signed char > > >::difference_type j)"""
         return _oalib.conference_columnVector___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(conference_columnVector self, std::vector< std::vector< signed char,std::allocator< signed char > > >::difference_type i)
-        __delitem__(conference_columnVector self, PySliceObject * slice)
+        __delitem__(conference_columnVector self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.conference_columnVector___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(conference_columnVector self, PySliceObject * slice) -> conference_columnVector
+        __getitem__(conference_columnVector self, SWIGPY_SLICEOBJECT * slice) -> conference_columnVector
         __getitem__(conference_columnVector self, std::vector< std::vector< signed char,std::allocator< signed char > > >::difference_type i) -> charVector
         """
         return _oalib.conference_columnVector___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(conference_columnVector self, PySliceObject * slice, conference_columnVector v)
-        __setitem__(conference_columnVector self, PySliceObject * slice)
+        __setitem__(conference_columnVector self, SWIGPY_SLICEOBJECT * slice, conference_columnVector v)
+        __setitem__(conference_columnVector self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(conference_columnVector self, std::vector< std::vector< signed char,std::allocator< signed char > > >::difference_type i, charVector x)
         """
         return _oalib.conference_columnVector___setitem__(self, *args)
 
     def pop(self):
         r"""pop(conference_columnVector self) -> charVector"""
         return _oalib.conference_columnVector_pop(self)
@@ -11936,15 +12130,14 @@
         r"""capacity(conference_columnVector self) -> std::vector< std::vector< signed char,std::allocator< signed char > > >::size_type"""
         return _oalib.conference_columnVector_capacity(self)
     __swig_destroy__ = _oalib.delete_conference_columnVector
 
 # Register conference_columnVector in _oalib:
 _oalib.conference_columnVector_swigregister(conference_columnVector)
 
-
 def calculateArrayParetoJ5(al, verbose):
     r"""
     calculateArrayParetoJ5(array_link al, int verbose) -> Pareto< mvalue_t< long >,array_link >::pValue
 
 
     Calculate Pareto element with J5 criterium.
 
@@ -12008,29 +12201,29 @@
     def __delslice__(self, i, j):
         r"""__delslice__(vector_vector_double self, std::vector< std::vector< double > >::difference_type i, std::vector< std::vector< double > >::difference_type j)"""
         return _oalib.vector_vector_double___delslice__(self, i, j)
 
     def __delitem__(self, *args):
         r"""
         __delitem__(vector_vector_double self, std::vector< std::vector< double > >::difference_type i)
-        __delitem__(vector_vector_double self, PySliceObject * slice)
+        __delitem__(vector_vector_double self, SWIGPY_SLICEOBJECT * slice)
         """
         return _oalib.vector_vector_double___delitem__(self, *args)
 
     def __getitem__(self, *args):
         r"""
-        __getitem__(vector_vector_double self, PySliceObject * slice) -> vector_vector_double
+        __getitem__(vector_vector_double self, SWIGPY_SLICEOBJECT * slice) -> vector_vector_double
         __getitem__(vector_vector_double self, std::vector< std::vector< double > >::difference_type i) -> doubleVector
         """
         return _oalib.vector_vector_double___getitem__(self, *args)
 
     def __setitem__(self, *args):
         r"""
-        __setitem__(vector_vector_double self, PySliceObject * slice, vector_vector_double v)
-        __setitem__(vector_vector_double self, PySliceObject * slice)
+        __setitem__(vector_vector_double self, SWIGPY_SLICEOBJECT * slice, vector_vector_double v)
+        __setitem__(vector_vector_double self, SWIGPY_SLICEOBJECT * slice)
         __setitem__(vector_vector_double self, std::vector< std::vector< double > >::difference_type i, doubleVector x)
         """
         return _oalib.vector_vector_double___setitem__(self, *args)
 
     def pop(self):
         r"""pop(vector_vector_double self) -> doubleVector"""
         return _oalib.vector_vector_double_pop(self)
@@ -12133,123 +12326,155 @@
         r"""capacity(vector_vector_double self) -> std::vector< std::vector< double > >::size_type"""
         return _oalib.vector_vector_double_capacity(self)
     __swig_destroy__ = _oalib.delete_vector_vector_double
 
 # Register vector_vector_double in _oalib:
 _oalib.vector_vector_double_swigregister(vector_vector_double)
 
-
 def krawtchouk(j, x, n, s, verbose=0):
     r"""
     krawtchouk(long j, long x, long n, long s, int verbose=0) -> long
 
 
     calculate value of Krawtchouk polynomial
 
     """
     return _oalib.krawtchouk(j, x, n, s, verbose)
 
 def choose_long(n, k):
-    r"""choose_long(long const n, long const k) -> long"""
+    r"""
+    Calculate binomial
+
+     Calculates n!/(k! * (n-k)!)
+
+     A recursive formala is used to prevent overflows.
+
+     The number of combinations is calculated using the an addapted formula
+     Calculates number of combinations
+     :type n: int
+     :param n: Total number of entries to choose from
+     :type k: int
+     :param k: Number of entries in a certain combination
+     :rtype: int
+     :return: Binomal n, k
+    """
     return _oalib.choose_long(n, k)
 
 def macwilliams_transform(B, N, s):
-    r"""macwilliams_transform(doubleVector B, int N, int s) -> doubleVector"""
+    r""" Calculate MacWilliams transform"""
     return _oalib.macwilliams_transform(B, N, s)
 
 # for legacy reasons and for name consistency
 GWLPvalueVector = vector_mvalue_t_double
 mvalueVector = vector_mvalue_t_long
 
 
 __doc__ = """
 Python Orthogonal Array Interface
 """
 
 class ndarray_double(object):
-    r"""Proxy of C++ ndarray< double > class."""
+    r"""
+     Class representing an n-dimensional array
+
+    The data is stored in a flat array. The dimensions are stored in a vector ``dims``.
+
+    """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     data = property(_oalib.ndarray_double_data_get, _oalib.ndarray_double_data_set, doc=r"""data : p.double""")
     dims = property(_oalib.ndarray_double_dims_get, _oalib.ndarray_double_dims_set, doc=r"""dims : std::vector<(int,std::allocator<(int)>)>""")
-    k = property(_oalib.ndarray_double_k_get, _oalib.ndarray_double_k_set, doc=r"""k : int""")
+    k = property(_oalib.ndarray_double_k_get, _oalib.ndarray_double_k_set, doc=r""" dimensions of the array""")
     n = property(_oalib.ndarray_double_n_get, _oalib.ndarray_double_n_set, doc=r"""n : int""")
     cumdims = property(_oalib.ndarray_double_cumdims_get, _oalib.ndarray_double_cumdims_set, doc=r"""cumdims : std::vector<(int,std::allocator<(int)>)>""")
     cumprod = property(_oalib.ndarray_double_cumprod_get, _oalib.ndarray_double_cumprod_set, doc=r"""cumprod : std::vector<(int,std::allocator<(int)>)>""")
 
     def __init__(self, *args):
         r"""
-        __init__(ndarray_double self, intVector dims) -> ndarray_double
-        __init__(ndarray_double self, ndarray_double rhs) -> ndarray_double
+        *Overload 1:*
+         Class represensing an n-dimensional array
+        :type dims: std::vector< int,std::allocator< int > >
+        :param dims: Dimension of the array
+
+        |
+
+        *Overload 2:*
+         Copy constructor
+         Copies the internal data
         """
         _oalib.ndarray_double_swiginit(self, _oalib.new_ndarray_double(*args))
     __swig_destroy__ = _oalib.delete_ndarray_double
 
     def initialize(self, value):
-        r"""initialize(ndarray_double self, double const value)"""
+        r""" Initialize array with specified value"""
         return _oalib.ndarray_double_initialize(self, value)
 
     def sizeof_type(self):
-        r"""sizeof_type(ndarray_double self) -> int"""
+        r""" Return size of ndarray template type"""
         return _oalib.ndarray_double_sizeof_type(self)
 
     def type_is_floating_point(self):
-        r"""type_is_floating_point(ndarray_double self) -> bool"""
+        r""" Return True is the data type is of floating point type"""
         return _oalib.ndarray_double_type_is_floating_point(self)
 
     def info(self):
         r"""info(ndarray_double self)"""
         return _oalib.ndarray_double_info(self)
 
     def idxstring(self, linear_idx):
-        r"""idxstring(ndarray_double self, int linear_idx) -> std::string"""
+        r""" Convert linear index to string representing the index"""
         return _oalib.ndarray_double_idxstring(self, linear_idx)
 
     def totalsize(self):
-        r"""totalsize(ndarray_double self) -> long"""
+        r""" size of the array (product of all dimensions)"""
         return _oalib.ndarray_double_totalsize(self)
 
     def show(self):
-        r"""show(ndarray_double self)"""
+        r""" print the array to stdout"""
         return _oalib.ndarray_double_show(self)
 
     def linear2idx(self, *args):
         r"""
-        linear2idx(ndarray_double self, int ndx, int * nidx=None)
-        linear2idx(ndarray_double self, int ndx, intVector nidx)
+        *Overload 1:*
+        convert a linear index to normal indices
+
+        |
+
+        *Overload 2:*
+        convert a linear index to normal indices
         """
         return _oalib.ndarray_double_linear2idx(self, *args)
 
     def getlinearidx(self, idx):
-        r"""getlinearidx(ndarray_double self, int * idx) -> int"""
+        r""" From an n-dimensional index return the linear index in the data"""
         return _oalib.ndarray_double_getlinearidx(self, idx)
 
     def data_pointer(self):
-        r"""data_pointer(ndarray_double self) -> void *"""
+        r""" Return pointer to data"""
         return _oalib.ndarray_double_data_pointer(self)
 
     def setconstant(self, val):
-        r"""setconstant(ndarray_double self, double val)"""
+        r""" set all values of the array to specified value"""
         return _oalib.ndarray_double_setconstant(self, val)
 
     def set(self, idx, val):
-        r"""set(ndarray_double self, int * idx, double val)"""
+        r""" set value at position"""
         return _oalib.ndarray_double_set(self, idx, val)
 
     def setlinear(self, idx, val):
-        r"""setlinear(ndarray_double self, int idx, double val)"""
+        r""" set value using linear index"""
         return _oalib.ndarray_double_setlinear(self, idx, val)
 
     def getlinear(self, idx):
-        r"""getlinear(ndarray_double self, int idx) -> double"""
+        r""" get value using linear index"""
         return _oalib.ndarray_double_getlinear(self, idx)
 
     def get(self, idx):
-        r"""get(ndarray_double self, int * idx) -> double"""
+        r""" get value using n-dimensional index"""
         return _oalib.ndarray_double_get(self, idx)
 
 
     @property
     def shape(self):
         return tuple(self.dims)
 
@@ -12274,96 +12499,113 @@
           raise AttributeError("%r object has no attribute %r" %
                              (self.__class__, attr))
 
 
 
 # Register ndarray_double in _oalib:
 _oalib.ndarray_double_swigregister(ndarray_double)
-
 class ndarray_long(object):
-    r"""Proxy of C++ ndarray< long > class."""
+    r"""
+     Class representing an n-dimensional array
+
+    The data is stored in a flat array. The dimensions are stored in a vector ``dims``.
+
+    """
 
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
     data = property(_oalib.ndarray_long_data_get, _oalib.ndarray_long_data_set, doc=r"""data : p.long""")
     dims = property(_oalib.ndarray_long_dims_get, _oalib.ndarray_long_dims_set, doc=r"""dims : std::vector<(int,std::allocator<(int)>)>""")
-    k = property(_oalib.ndarray_long_k_get, _oalib.ndarray_long_k_set, doc=r"""k : int""")
+    k = property(_oalib.ndarray_long_k_get, _oalib.ndarray_long_k_set, doc=r""" dimensions of the array""")
     n = property(_oalib.ndarray_long_n_get, _oalib.ndarray_long_n_set, doc=r"""n : int""")
     cumdims = property(_oalib.ndarray_long_cumdims_get, _oalib.ndarray_long_cumdims_set, doc=r"""cumdims : std::vector<(int,std::allocator<(int)>)>""")
     cumprod = property(_oalib.ndarray_long_cumprod_get, _oalib.ndarray_long_cumprod_set, doc=r"""cumprod : std::vector<(int,std::allocator<(int)>)>""")
 
     def __init__(self, *args):
         r"""
-        __init__(ndarray_long self, intVector dims) -> ndarray_long
-        __init__(ndarray_long self, ndarray_long rhs) -> ndarray_long
+        *Overload 1:*
+         Class represensing an n-dimensional array
+        :type dims: std::vector< int,std::allocator< int > >
+        :param dims: Dimension of the array
+
+        |
+
+        *Overload 2:*
+         Copy constructor
+         Copies the internal data
         """
         _oalib.ndarray_long_swiginit(self, _oalib.new_ndarray_long(*args))
     __swig_destroy__ = _oalib.delete_ndarray_long
 
     def initialize(self, value):
-        r"""initialize(ndarray_long self, long const value)"""
+        r""" Initialize array with specified value"""
         return _oalib.ndarray_long_initialize(self, value)
 
     def sizeof_type(self):
-        r"""sizeof_type(ndarray_long self) -> int"""
+        r""" Return size of ndarray template type"""
         return _oalib.ndarray_long_sizeof_type(self)
 
     def type_is_floating_point(self):
-        r"""type_is_floating_point(ndarray_long self) -> bool"""
+        r""" Return True is the data type is of floating point type"""
         return _oalib.ndarray_long_type_is_floating_point(self)
 
     def info(self):
         r"""info(ndarray_long self)"""
         return _oalib.ndarray_long_info(self)
 
     def idxstring(self, linear_idx):
-        r"""idxstring(ndarray_long self, int linear_idx) -> std::string"""
+        r""" Convert linear index to string representing the index"""
         return _oalib.ndarray_long_idxstring(self, linear_idx)
 
     def totalsize(self):
-        r"""totalsize(ndarray_long self) -> long"""
+        r""" size of the array (product of all dimensions)"""
         return _oalib.ndarray_long_totalsize(self)
 
     def show(self):
-        r"""show(ndarray_long self)"""
+        r""" print the array to stdout"""
         return _oalib.ndarray_long_show(self)
 
     def linear2idx(self, *args):
         r"""
-        linear2idx(ndarray_long self, int ndx, int * nidx=None)
-        linear2idx(ndarray_long self, int ndx, intVector nidx)
+        *Overload 1:*
+        convert a linear index to normal indices
+
+        |
+
+        *Overload 2:*
+        convert a linear index to normal indices
         """
         return _oalib.ndarray_long_linear2idx(self, *args)
 
     def getlinearidx(self, idx):
-        r"""getlinearidx(ndarray_long self, int * idx) -> int"""
+        r""" From an n-dimensional index return the linear index in the data"""
         return _oalib.ndarray_long_getlinearidx(self, idx)
 
     def data_pointer(self):
-        r"""data_pointer(ndarray_long self) -> void *"""
+        r""" Return pointer to data"""
         return _oalib.ndarray_long_data_pointer(self)
 
     def setconstant(self, val):
-        r"""setconstant(ndarray_long self, long val)"""
+        r""" set all values of the array to specified value"""
         return _oalib.ndarray_long_setconstant(self, val)
 
     def set(self, idx, val):
-        r"""set(ndarray_long self, int * idx, long val)"""
+        r""" set value at position"""
         return _oalib.ndarray_long_set(self, idx, val)
 
     def setlinear(self, idx, val):
-        r"""setlinear(ndarray_long self, int idx, long val)"""
+        r""" set value using linear index"""
         return _oalib.ndarray_long_setlinear(self, idx, val)
 
     def getlinear(self, idx):
-        r"""getlinear(ndarray_long self, int idx) -> long"""
+        r""" get value using linear index"""
         return _oalib.ndarray_long_getlinear(self, idx)
 
     def get(self, idx):
-        r"""get(ndarray_long self, int * idx) -> long"""
+        r""" get value using n-dimensional index"""
         return _oalib.ndarray_long_get(self, idx)
 
 
     @property
     def shape(self):
         return tuple(self.dims)
 
@@ -12389,9 +12631,7 @@
                              (self.__class__, attr))
 
 
 
 # Register ndarray_long in _oalib:
 _oalib.ndarray_long_swigregister(ndarray_long)
 
-
-
```

### Comparing `OApackage-2.7.6/oapackage/Doptim.py` & `OApackage-2.7.7/oapackage/Doptim.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,329 +6,376 @@
 
 """
 
 import logging
 import os
 import time
 import warnings
-from typing import List, Optional
+from typing import Any, Callable, List, Optional, Tuple, Union
 
+import matplotlib
+import matplotlib.cm
+import matplotlib.pyplot as plt
 import numpy as np
+import numpy.typing
 
-import oalib
+import oalib  # type: ignore
 import oapackage.markup as markup
 import oapackage.oahelper as oahelper
 from oapackage.markup import oneliner as e
 
-try:
-    import matplotlib
-    import matplotlib.cm
-    import matplotlib.pyplot as plt
-except BaseException:
-    matplotlib = None
-
-
-class MissingMatplotLibException(Exception):
-    pass
-
+FloatArray = np.typing.NDArray[np.float64]
 
 # %%
 
 
 def array2Dtable(array_list: List, verbose: int = 1, titlestr: Optional[str] = None):
-    """ Generate HTML table with information about for a list of designs
+    """Generate HTML table with information about for a list of designs
 
     Args:
         array_list: list of arrays
         verbose: verbosity level
         titlestr: Not used
     """
     page = markup.page()
-    page.table(style=' border-collapse: collapse;')
-    page.tr(style='font-weight: bold; border-bottom: solid 1px black;')
-    page.th('Array', style='padding-right:30px; ')
-    page.th(('D-efficiency', 'Ds-efficiency', 'D1-efficiency'),
-            style='padding-right:14px;')
-    page.th(('GWLP'), style='padding-right:14px;')
+    page.table(style=" border-collapse: collapse;")
+    page.tr(style="font-weight: bold; border-bottom: solid 1px black;")
+    page.th("Array", style="padding-right:30px; ")
+    page.th(("D-efficiency", "Ds-efficiency", "D1-efficiency"), style="padding-right:14px;")
+    page.th(("GWLP"), style="padding-right:14px;")
     page.tr.close()
     for ii, al in enumerate(array_list):
         aidx = ii
         (D, Ds, D1) = al.Defficiencies()
         gwlp = al.GWLP()
-        page.tr(style='font-weight: normal;')
-        page.td('%d' % aidx, style='padding-right:10px;')
+        page.tr(style="font-weight: normal;")
+        page.td("%d" % aidx, style="padding-right:10px;")
         for statistic in [D, Ds, D1]:
-            page.td('%.4f' % statistic, style='padding-right:1px;')
+            page.td("%.4f" % statistic, style="padding-right:1px;")
         gstr = oahelper.gwlp2str(gwlp)
-        page.td(e.small(gstr), style='padding-right:1px;')
+        page.td(e.small(gstr), style="padding-right:1px;")
         page.tr.close()
     page.table.close()
     return page
 
+
 # %%
 
 
-def generateDscatter(dds, second_index=0, first_index=1, lbls=None, ndata=3, nofig=False, fig=20,
-                     scatterarea=80, verbose=0, setWindowRectangle=False):
-    """ Generate scatter plot for D and Ds efficiencies
+def generateDscatter(
+    dds,
+    second_index=0,
+    first_index=1,
+    lbls=None,
+    ndata=3,
+    nofig=False,
+    fig=20,
+    scatterarea=80,
+    verbose=0,
+    setWindowRectangle=False,
+):
+    """Generate scatter plot for D and Ds efficiencies
 
     Args:
         dds (array): array with D-efficiencies
     Returns:
         dict: contains handles to plotting elements
     """
-    if matplotlib is None:
-        raise MissingMatplotLibException
     data = dds.T
     pp = oahelper.createPareto(dds)
     paretoidx = np.array(pp.allindices())
 
     nn = dds.shape[0]
-    area = scatterarea * np.ones(nn,) / 2
+    area = (
+        scatterarea
+        * np.ones(
+            nn,
+        )
+        / 2
+    )
     area[np.array(pp.allindices())] = scatterarea
     alpha = 1.0
 
     if dds.shape[1] > ndata:
         colors = dds[:, ndata]
     else:
         colors = np.zeros((nn, 1))
 
     idx = np.unique(colors).astype(int)
 
     if verbose:
-        print('generateDscatter: unique colors: %s' % (idx, ))
+        print(f"generateDscatter: unique colors: {idx}")
     ncolors = idx.size
     try:
         import brewer2mpl
+
         ncolors = max(ncolors, 4)
-        mycmap = brewer2mpl.get_map('Set1', 'qualitative', ncolors).mpl_colors
+        mycmap = brewer2mpl.get_map("Set1", "qualitative", ncolors).mpl_colors
     except BaseException:
         mycmap = [matplotlib.cm.jet(ii) for ii in np.linspace(0, 1, ncolors)]
 
     nonparetoidx = np.setdiff1d(range(nn), paretoidx)
     if lbls is None:
-        lbls = ['%d' % i for i in range(len(idx))]
+        lbls = ["%d" % i for i in range(len(idx))]
 
     if fig is not None:
         figh = plt.figure(fig)
         plt.clf()
-        figh.set_facecolor('w')
+        figh.set_facecolor("w")
         ax = plt.subplot(111)
 
-        ax.scatter(data[first_index, nonparetoidx], data[second_index, nonparetoidx], s=.33 * scatterarea,
-                   c=[(.5, .5, .5)], linewidths=0, alpha=alpha, label='Non-pareto design')
+        ax.scatter(
+            data[first_index, nonparetoidx],
+            data[second_index, nonparetoidx],
+            s=0.33 * scatterarea,
+            c=[(0.5, 0.5, 0.5)],
+            linewidths=0,
+            alpha=alpha,
+            label="Non-pareto design",
+        )
 
         for jj, ii in enumerate(idx):
             gidx = (colors == ii).nonzero()[0]
             gp = np.intersect1d(paretoidx, gidx)
 
             color = mycmap[jj]
             cc = [color] * len(gp)
             if verbose:
-                print('index %d: %d points' % (ii, gidx.size))
-            ax.scatter(data[first_index, gp], data[second_index, gp], s=scatterarea, c=cc,
-                       linewidths=0, alpha=alpha, label=lbls[jj])
+                print("index %d: %d points" % (ii, gidx.size))
+            ax.scatter(
+                data[first_index, gp],
+                data[second_index, gp],
+                s=scatterarea,
+                c=cc,
+                linewidths=0,
+                alpha=alpha,
+                label=lbls[jj],
+            )
             plt.draw()
 
         if data[second_index, :].std() < 1e-3:
             y_formatter = matplotlib.ticker.ScalarFormatter(useOffset=False)
             ax.yaxis.set_major_formatter(y_formatter)
 
-        xlabelhandle = plt.xlabel('$D_s$-efficiency', fontsize=16)
-        plt.ylabel('D-efficiency', fontsize=16)
+        xlabelhandle = plt.xlabel("$D_s$-efficiency", fontsize=16)
+        plt.ylabel("D-efficiency", fontsize=16)
 
         if setWindowRectangle:
             try:
                 oahelper.setWindowRectangle(10, 10, 860, 600)
             except Exception as ex:
-                print('generateDscatter: setWindowRectangle failed')
+                print("generateDscatter: setWindowRectangle failed")
                 logging.exception(ex)
 
-        plt.axis('image')
+        plt.axis("image")
         pltlegend = ax.legend(loc=3, scatterpoints=1)  # , fontcolor=almost_black)
         if not nofig:
             plt.show()
-        ax.grid(visible=True, which='both', color='0.85', linestyle='-')
+        ax.grid(visible=True, which="both", color="0.85", linestyle="-")
         ax.set_axisbelow(True)
 
         if nofig:
             plt.close(figh.number)
         else:
             plt.draw()
             plt.pause(1e-3)
     else:
         ax = None
         xlabelhandle = None
         pltlegend = None
-    hh = dict({'ax': ax, 'xlabelhandle': xlabelhandle, 'pltlegend': pltlegend})
+    hh = dict({"ax": ax, "xlabelhandle": xlabelhandle, "pltlegend": pltlegend})
     return hh
 
 
-def generateDpage(outputdir, arrayclass, dds, allarrays, fig=20, optimfunc=(1, 0, 0),
-                  nofig=False, urlprefix='', makeheader=True, verbose=1, lbls=None):
-    """ Helper function to generate web page with D-optimal design results """
+def generateDpage(
+    outputdir,
+    arrayclass,
+    dds,
+    allarrays,
+    fig=20,
+    optimfunc=(1, 0, 0),
+    nofig=False,
+    urlprefix="",
+    makeheader=True,
+    verbose=1,
+    lbls=None,
+):
+    """Helper function to generate web page with D-optimal design results"""
     if verbose:
-        print('generateDpage: dds %s' % str(dds.shape))
+        print("generateDpage: dds %s" % str(dds.shape))
 
     pp = oahelper.createPareto(dds)
 
     narrays = dds.shape[0]
     npareto = pp.number()
 
     if verbose:
-        print('generateDpage: narrays %d' % narrays)
+        print("generateDpage: narrays %d" % narrays)
 
     xstr = oahelper.series2htmlstr(arrayclass, case=1)
     xstrplain = oahelper.series2htmlstr(arrayclass, html=0, case=1)
 
     if verbose:
-        print('generateDpage: selectParetoArrays ')
+        print("generateDpage: selectParetoArrays ")
     paretoarrays = oahelper.selectParetoArrays(allarrays, pp)
     at = array2Dtable(paretoarrays, verbose=1)
 
     if verbose:
-        print('generateDpage: write file with Pareto arrays')
+        print("generateDpage: write file with Pareto arrays")
 
-    pfile0 = 'paretoarrays.oa'
+    pfile0 = "paretoarrays.oa"
     pfile = os.path.join(outputdir, pfile0)
     oalib.writearrayfile(pfile, paretoarrays)
 
-    istrlnk = markup.oneliner.a('paretoarrays.oa', href=urlprefix + pfile0)
+    istrlnk = markup.oneliner.a("paretoarrays.oa", href=urlprefix + pfile0)
 
     if lbls is None:
-        lbls = ['Optimization of $D$']
+        lbls = ["Optimization of $D$"]
     if fig is not None:
         hh = generateDscatter(dds, lbls=lbls, fig=fig, nofig=nofig)
-        oahelper.niceplot(hh.get('ax', None), despine=True, legend=hh['pltlegend'])
+        oahelper.niceplot(hh.get("ax", None), despine=True, legend=hh["pltlegend"])
 
-        scatterfile = os.path.join(outputdir, 'scatterplot.png')
+        scatterfile = os.path.join(outputdir, "scatterplot.png")
         if verbose:
-            print('generateDpage: writen scatterplot to %s' % scatterfile)
-        plt.savefig(scatterfile, bbox_inches='tight', pad_inches=0.25, dpi=160)
+            print("generateDpage: writen scatterplot to %s" % scatterfile)
+        plt.savefig(scatterfile, bbox_inches="tight", pad_inches=0.25, dpi=160)
 
     page = markup.page()
 
     if makeheader:
-        page.init(title="Class %s" % xstrplain,
-                  css=('../oastyle.css'),
-                  lang='en', htmlattrs=dict({'xmlns': 'http://www.w3.org/1999/xhtml', 'xml:lang': 'en'}),
-                  header="<!-- Start of page -->",
-                  bodyattrs=dict({'style': 'padding-left: 3px;'}),
-                       doctype='<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">',
-                       metainfo=({'text/html': 'charset=utf-8', 'keywords': 'orthogonal arrays designs',
-                                  'robots': 'index, follow', 'description': 'Even-Odd arrays'}),
-                       footer="<!-- End of page -->")
+        page.init(
+            title="Class %s" % xstrplain,
+            css=("../oastyle.css"),
+            lang="en",
+            htmlattrs=dict({"xmlns": "http://www.w3.org/1999/xhtml", "xml:lang": "en"}),
+            header="<!-- Start of page -->",
+            bodyattrs=dict({"style": "padding-left: 3px;"}),
+            doctype='<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"'
+            + ' "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">',
+            metainfo=(
+                {
+                    "text/html": "charset=utf-8",
+                    "keywords": "orthogonal arrays designs",
+                    "robots": "index, follow",
+                    "description": "Even-Odd arrays",
+                }
+            ),
+            footer="<!-- End of page -->",
+        )
 
-    page.h1('Results for array class %s ' % xstr)
+    page.h1("Results for array class %s " % xstr)
 
-    ss = r'The Pareto optimaly was calculated according to the statistics D, D<sub>1</sub> and D<sub>s</sub>.'
+    ss = r"The Pareto optimaly was calculated according to the statistics D, D<sub>1</sub> and D<sub>s</sub>."
     if npareto == 1:
-        page.p('Generated %d arrays, %d is Pareto optimal. %s' %
-               (narrays, npareto, ss))
+        page.p("Generated %d arrays, %d is Pareto optimal. %s" % (narrays, npareto, ss))
     else:
-        page.p('Generated %d arrays, %d are Pareto optimal. %s' %
-               (narrays, npareto, ss))
+        page.p("Generated %d arrays, %d are Pareto optimal. %s" % (narrays, npareto, ss))
 
     if narrays > 0:
-
         scores = calcScore(dds, optimfunc)
         _, dd, sols = selectDn(scores, dds, allarrays, nout=1)
         A = sols[0]
-        bestdesignfile = os.path.join(outputdir, 'best-design.oa')
+        bestdesignfile = os.path.join(outputdir, "best-design.oa")
         oalib.writearrayfile(bestdesignfile, A)
 
-        page.h2('Best design')
-        page.p('The best design: %s.' %
-               e.a('best-design.oa', href=os.path.join(urlprefix, 'best-design.oa')))
+        page.h2("Best design")
+        page.p("The best design: %s." % e.a("best-design.oa", href=os.path.join(urlprefix, "best-design.oa")))
 
         page.p()
 
         dd = dd[0]
-        page.span('D-efficiency: %.4f, ' % A.Defficiency())  # page.br()
-        page.span('D<sub>s</sub>-efficiency: %.4f, ' % dd[1])  # page.br()
-        page.span('D<sub>1</sub>-efficiency: %.4f' % dd[2])
+        page.span("D-efficiency: %.4f, " % A.Defficiency())  # page.br()
+        page.span("D<sub>s</sub>-efficiency: %.4f, " % dd[1])  # page.br()
+        page.span("D<sub>1</sub>-efficiency: %.4f" % dd[2])
         page.br()
-        page.span('A-efficiency: %.3f' % A.Aefficiency())
+        page.span("A-efficiency: %.3f" % A.Aefficiency())
         page.br()
         gwlp = A.GWLP()
         # gwlp=','.join(['%.3f' % xq for xq in gwlp])
-        gwlp = oahelper.gwlp2str(gwlp, jstr=', ')
-        page.span('Generalized wordlength pattern: %s' % gwlp)
+        gwlp = oahelper.gwlp2str(gwlp, jstr=", ")
+        page.span("Generalized wordlength pattern: %s" % gwlp)
         page.br()
         # page.p('D-efficiency: %.3f' % A.Defficiency() )
         pec = oalib.PECsequence(A)
-        pec = ','.join(['%.3f' % xq for xq in pec])
-        page.span('PEC-sequence: %s' % pec)
+        pec = ",".join(["%.3f" % xq for xq in pec])
+        page.span("PEC-sequence: %s" % pec)
         page.br()
 
-    page.h2('Table of Pareto optimal arrays ')
+    page.h2("Table of Pareto optimal arrays ")
 
     page.span(str(at))
-    page.p('All Pareto optimal arrays: %s' % istrlnk)
+    page.p("All Pareto optimal arrays: %s" % istrlnk)
 
-    page.img(src=urlprefix + 'scatterplot.png',
-             style="margin: 10px; width:95%; min-width: 300px;  max-width:1100px; height: auto; ")
+    page.img(
+        src=urlprefix + "scatterplot.png",
+        style="margin: 10px; width:95%; min-width: 300px;  max-width:1100px; height: auto; ",
+    )
 
     citationstr = markup.oneliner.a(
-        'Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays', href='https://doi.org/10.1002/jcd.20236')
+        "Complete Enumeration of Pure-Level and Mixed-Level Orthogonal Arrays", href="https://doi.org/10.1002/jcd.20236"
+    )
 
-    page.br(clear='both')
-    page.p(
-        'Citation notice: if you make use of the results on this page, please cite the following paper:')
-    page.p('%s, Journal of Combinatorial Designs, Volume 18, Issue 2, pages 123-140, 2010.' %
-           citationstr)
+    page.br(clear="both")
+    page.p("Citation notice: if you make use of the results on this page, please cite the following paper:")
+    page.p("%s, Journal of Combinatorial Designs, Volume 18, Issue 2, pages 123-140, 2010." % citationstr)
 
-    page.p('Generated with oapackage %s, date %s.' %
-           (oalib.version(), oahelper.timeString()))
+    page.p(f"Generated with oapackage {oalib.version()}, date {oahelper.timeString()}.")
 
-    outfile = os.path.join(outputdir, 'Dresults.html')
-    fid = open(outfile, 'w')
+    outfile = os.path.join(outputdir, "Dresults.html")
+    fid = open(outfile, "w")
     fid.write(str(page))
     fid.close()
-    print('written to file %s' % outfile)
+    print("written to file %s" % outfile)
 
     return outfile
 
 
-def scoreDn(dds, optimfunc):
-    """ Calculate scores from various efficiencies
+def scoreDn(dds: FloatArray, optimfunc: List) -> FloatArray:
+    """Calculate scores from various efficiencies
 
     Args:
-        dds (array): calculated D-efficiencies
-        optimfunc (list): parameters for optimization function
+        dds: calculated D-efficiencies
+        optimfunc: parameters for optimization function
     Returns:
-        scores (array)
+        Calculated scores
     """
     scores = np.array([oalib.scoreD(dd, optimfunc) for dd in dds])
     return scores
 
 
-def calcScore(dds, optimfunc):
-    """ Calculate D-efficiency score using multiple efficiencies and a weight factor
+def calcScore(dds: FloatArray, optimfunc: FloatArray) -> FloatArray:
+    """Calculate D-efficiency score using multiple efficiencies and a weight factor
 
     Args:
         dds (array): the rows contains the effieciencies for various designs
         optimfunc (array): aray with the weight factors for the efficiencies
     """
-    scores = np.array(dds).dot(np.array(optimfunc))
+    scores = np.asarray(dds).dot(np.asarray(optimfunc))
 
     return scores
 
 
-def optimDeffPython(A0, arrayclass=None, niter=10000, nabort=2500, verbose=1, alpha=[1, 0, 0], method=0):
-    """ Optimize array using specified optimization method
+def optimDeffPython(
+    A0,
+    arrayclass=None,
+    niter: int = 10000,
+    nabort: int = 2500,
+    verbose: int = 1,
+    alpha: Union[Callable, List[float]] = [1, 0, 0],
+    method: int = 0,
+) -> Tuple[FloatArray, Any]:
+    """Optimize array using specified optimization method
 
     Args:
         A0 (array_link): design to optimize
         arrayclass (object): contains class of designs to optimize
         alpha (list): specifies the optimization function
 
     Returns:
-        d (array): efficiencies
-        A (array): optimized design
+        Tuple with efficiencies and optimized design
     """
     # get factor levels
     if arrayclass is None:
         s = A0.getarray().max(axis=0) + 1
     else:
         s = arrayclass.factor_levels()
     sx = tuple(s.astype(np.int64))
@@ -339,22 +386,22 @@
     gsize = tuple(sg.gsize)
     gstart = tuple(sg.gstart)
 
     nx = 0
 
     Dinitial = A0.Defficiency()
     if verbose:
-        print('optimDeff: initial Deff %.4f' % Dinitial)
+        print("optimDeff: initial Deff %.4f" % Dinitial)
     N = A0.n_rows
     k = A0.n_columns
 
     alpha_is_function = str(type(alpha)) == "<type 'function'>" or callable(alpha)
     # initialize score
     if alpha_is_function:
-        efficiencies = alpha(A0)
+        efficiencies = alpha(A0)  # type: ignore
     else:
         D, Ds, D1 = A0.Defficiencies()
         efficiencies = alpha[0] * D + alpha[1] * Ds + alpha[2] * D1
     A = A0.clone()
     lc = 0
     for ii in range(0, niter):
         r = np.random.randint(N)
@@ -375,54 +422,53 @@
         elif method == oalib.DOPTIM_NONE:
             pass
         else:
             # flip
             A._setvalue(r, c, 1 - o)
 
         if alpha_is_function:
-            dn = alpha(A)
+            dn = alpha(A)  # type: ignore
         else:
             D, Ds, D1 = A.Defficiencies()
             nx = nx + 1
-            dn = alpha[0] * D + alpha[1] * Ds + alpha[2] * D1
+            dn = alpha[0] * D + alpha[1] * Ds + alpha[2] * D1  # type: ignore
         if dn >= efficiencies:
             if dn > efficiencies:
                 lc = ii
                 efficiencies = dn
             if verbose >= 2:
-                print('ii %d: %.6f -> %.6f' % (ii, efficiencies, dn))
+                print("ii %d: %.6f -> %.6f" % (ii, efficiencies, dn))
 
         else:
             # restore to original
             if method == oalib.DOPTIM_SWAP:
                 A._setvalue(r, c, o)
                 A._setvalue(r2, c2, o2)
             elif method == oalib.DOPTIM_NONE:
                 pass
             else:
                 A._setvalue(r, c, o)
         if (ii - lc) > nabort:
             if verbose:
-                print('optimDeff: early abort ii %d, lc %d' % (ii, lc))
+                print("optimDeff: early abort ii %d, lc %d" % (ii, lc))
             break
 
     if verbose:
         Dfinal = A.Defficiency()
         if Dfinal > Dinitial:
-            print('optimDeff: final Deff improved: %.4f -> %.4f' %
-                  (Dinitial, A.Defficiency()))
+            print(f"optimDeff: final Deff improved: {Dinitial:.4f} -> {A.Defficiency():.4f}")
         else:
-            print('optimDeff: final Deff %.4f' % A.Defficiency())
+            print("optimDeff: final Deff %.4f" % A.Defficiency())
 
     return efficiencies, A
 
 
 # %%
 def filterPareto(scores, dds, arrays, verbose=0):
-    """ From a list of designs select only the pareto optimal designs
+    """From a list of designs select only the pareto optimal designs
 
     Args:
         scores (array): array of scores
         dds (array): array with D-efficiency values
         arrays (list): list of designs
     Returns:
         pareto_scores (list) : list of scores of pareto optimal designs
@@ -436,15 +482,15 @@
     pareto_efficiencies = dds[paretoidx]
     pareto_designs = [arrays[i] for i in paretoidx]
 
     return pareto_scores, pareto_efficiencies, pareto_designs
 
 
 def selectDn(scores, dds, sols, nout=1, sortfull=True):
-    """ Select best arrays according to given scores
+    """Select best arrays according to given scores
 
     The resulting data is sorted
 
     Parameters
     ----------
     scores : array
         scores for the designs
@@ -479,33 +525,46 @@
         nout = np.minimum(nout, scores.size)
         scores = scores[0:nout]
         dds = dds[range(nout), :]
         sols = sols[0:nout]
     return scores, dds, sols
 
 
-def Doptimize(arrayclass, nrestarts=10, optimfunc=[
-              1, 0, 0], verbose=1, maxtime=180, selectpareto=True, nout=None, method=oalib.DOPTIM_UPDATE, niter=100000, nabort=0, dverbose=1):
-    """ Calculate D-efficient designs
-
-    The method uses a coordinate-exchange algorithm find a D-efficient (sometimes called D-optimal) design in the class specified by the
-    arrayclass. The optimality is defined in terms of the optimization parameters. The optimization is performed
-    multiple times (specified by the nrestarts parameter) to prevent finding a design in a local minmum of the
-    target function.
+def Doptimize(
+    arrayclass,
+    nrestarts=10,
+    optimfunc=[1, 0, 0],
+    verbose=1,
+    maxtime=180,
+    selectpareto=True,
+    nout=None,
+    method=oalib.DOPTIM_UPDATE,
+    niter=100000,
+    nabort=0,
+    dverbose=1,
+):
+    """Calculate D-efficient designs
+
+    The method uses a coordinate-exchange algorithm find a D-efficient (sometimes called D-optimal) design in the
+    class specified by the arrayclass. The optimality is defined in terms of the optimization parameters.
+    The optimization is performed multiple times (specified by the nrestarts parameter) to prevent finding a design
+    in a local minmum of the target function.
 
 
     Args:
       arrayclass (object): Specifies the type of design to optimize
       nrestarts (int): Number of restarts of the algorithm
-      optimfunc (list with 3 floats): Gives the optimization weights :math:`\\alpha` of the target function :math:`\\alpha[0] D+\\alpha[1] D_s+\\alpha[2] D_1`
+      optimfunc (list with 3 floats): Gives the optimization weights :math:`\\alpha` of the target
+                                  function :math:`\\alpha[0] D+\\alpha[1] D_s+\\alpha[2] D_1`
       verbose (int): Verbosity level. A higher numer gives more output
       maxtime (float): Maximum running time of the algorithm. If this time is exceeded the algorithm is aborted.
       selectpareto (bool): default is True. If True then only the Pareto optimal designs are returned
       nout (int or None): Maximum number of designs to return. If None,  return all designs
-      method (coordinate_exchange_method_t): Specifies the method use for updating elements in the coordinate-exchange algorithm.
+      method (coordinate_exchange_method_t): Specifies the method use for updating elements
+              in the coordinate-exchange algorithm.
       niter (int): Maximum number of iterations of the coordinate-exchange algorithm
       nabort (int): If no improvements have been found after this number of updates, then abort this run
       dverbose (int): Verbosity level passed to the C++ Doptimize function
 
     Returns
     -------
             scores : list
@@ -516,90 +575,99 @@
                 list of generated designs
             nrestarts: int
                 number of restarts used
 
 
     The optimization target and the Pareto optimality are defined in terms of the D-efficiency, main effect robustness
     (or Ds-optimality) and the D1-efficiency of the design. A full definition of these efficiencies is available
-    in the documentation at https://oapackage.readthedocs.io/en/latest/properties.html#optimality-criteria-for-d-efficient-designs. For more details and motivation of these efficiencies,
-    see the paper "Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions", https://doi.org/10.1080/00401706.2016.1142903.
+    in the documentation
+    at https://oapackage.readthedocs.io/en/latest/properties.html#optimality-criteria-for-d-efficient-designs.
+    For more details and motivation of these efficiencies, see the
+    paper "Two-Level Designs to Estimate All Main Effects and Two-Factor Interactions",
+    https://doi.org/10.1080/00401706.2016.1142903.
 
 
     """
     if arrayclass.strength != 0:
-        warnings.warn('Doptimize can only handle designs with strength 0', UserWarning)
+        warnings.warn("Doptimize can only handle designs with strength 0", UserWarning)
 
     if verbose:
-        print('Doptim: optimization class %s' % arrayclass.idstr())
-    t0 = time.time()
+        print("Doptim: optimization class %s" % arrayclass.idstr())
+    t0 = time.perf_counter()
 
     if optimfunc is None:
         optimfunc = [1, 2, 0]
 
     if isinstance(optimfunc, list):
-        rr = oalib.Doptimize(arrayclass, nrestarts, alpha=optimfunc, verbose=dverbose,
-                             method=method, niter=niter, maxtime=maxtime, nabort=nabort)
+        rr = oalib.Doptimize(
+            arrayclass,
+            nrestarts,
+            alpha=optimfunc,
+            verbose=dverbose,
+            method=method,
+            niter=niter,
+            maxtime=maxtime,
+            nabort=nabort,
+        )
         dds, sols = rr.dds, rr.designs
         dds = np.array([x for x in dds])
         # needed because of SWIG wrapping of struct type
         sols = [design.clone() for design in sols]
         nrestarts = rr.nrestarts
-        scores = np.array(
-            [oalib.scoreD(A.Defficiencies(), optimfunc) for A in sols])
+        scores = np.array([oalib.scoreD(A.Defficiencies(), optimfunc) for A in sols])
 
         if verbose >= 3:
-            print('Doptimize: max score %.3f, max D: %.6f' %
-                  (np.max(scores), np.max([A.Defficiency() for A in sols])))
+            print(f"Doptimize: max score {np.max(scores):.3f}, max D: {np.max([A.Defficiency() for A in sols]):.6f}")
     else:
         # assume optimfunc is a function
         scores = np.zeros((0, 1))
         dds = np.zeros((0, 3))
         sols = []
 
         nrestarts_requested = nrestarts
         nrestarts = 0
         for ii in range(nrestarts_requested):
             if verbose:
-                oahelper.tprint('Doptim: iteration %d/%d (time %.1f/%.1f)' %
-                                (ii, nrestarts, time.time() - t0, maxtime), dt=4)
+                oahelper.tprint(
+                    "Doptim: iteration %d/%d (time %.1f/%.1f)" % (ii, nrestarts, time.perf_counter() - t0, maxtime),
+                    dt=4,
+                )
             al = arrayclass.randomarray(1)
 
             if isinstance(optimfunc, list):
                 alpha = optimfunc
-                Ax = oalib.optimDeff(
-                    al, arrayclass, alpha, verbose >= 2, method, niter, nabort)
+                Ax = oalib.optimDeff(al, arrayclass, alpha, verbose >= 2, method, niter, nabort)
                 dd = Ax.Defficiencies()
                 score = oalib.scoreD(dd, optimfunc)
             else:
-                score, Ax = optimDeffPython(
-                    al, verbose=0, niter=niter, alpha=optimfunc, method=method, nabort=nabort)
+                score, Ax = optimDeffPython(al, verbose=0, niter=niter, alpha=optimfunc, method=method, nabort=nabort)
                 dd = Ax.Defficiencies()
 
-            if time.time() - t0 > maxtime:
+            if time.perf_counter() - t0 > maxtime:
                 if verbose:
-                    print('Doptim: max time exceeded, aborting')
+                    print("Doptim: max time exceeded, aborting")
                 break
 
             scores = np.vstack((scores, [score]))
             dds = np.vstack((dds, dd))
             sols.append(Ax)
             nrestarts = nrestarts + 1
 
             if verbose >= 2:
-                print('  generated array: %f %f %f' % (dd[0], dd[1], dd[2]))
+                print(f"  generated array: {dd[0]:f} {dd[1]:f} {dd[2]:f}")
 
             if selectpareto and ii % 502 == 0:
                 scores, dds, sols = filterPareto(scores, dds, sols)
 
     if selectpareto:
         if verbose >= 2:
-            print('Doptim: before Pareto filter (%d arrays)' % len(sols))
+            print("Doptim: before Pareto filter (%d arrays)" % len(sols))
         scores, dds, sols = filterPareto(scores, dds, sols)
 
     if verbose:
-        dt = time.time() - t0
-        print('Doptim: done (%d arrays, %.1f [s])' % (len(sols), dt))
+        dt = time.perf_counter() - t0
+        print("Doptim: done (%d arrays, %.1f [s])" % (len(sols), dt))
 
     # sort & select
     scores, dds, sols = selectDn(scores, dds, sols, nout=nout)
 
     return scores, dds, sols, nrestarts
```

### Comparing `OApackage-2.7.6/oapackage/_scanf.py` & `OApackage-2.7.7/oapackage/_scanf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import sys
 import re
+import sys
+
 """ https://github.com/joshburnett/scanf
 
 This file is extracted from https://github.com/joshburnett/scanf. The code is protected by an MIT license.
 
 """
 """
 Small scanf implementation.
@@ -27,54 +28,48 @@
 skip fields.
 """
 try:
     from functools import lru_cache
 except ImportError:
     from backports.functools_lru_cache import lru_cache  # type: ignore
 
-__version__ = '1.5.2'
+__version__ = "1.5.2"
 
-__all__ = ["scanf", 'extractdata', 'scanf_translate', 'scanf_compile']
+__all__ = ["scanf", "extractdata", "scanf_translate", "scanf_compile"]
 
 
 DEBUG = False
 
 
 # As you can probably see it is relatively easy to add more format types.
 # Make sure you add a second entry for each new item that adds the extra
 #   few characters needed to handle the field ommision.
 scanf_translate = [
-    (re.compile(_token), _pattern, _cast) for _token, _pattern, _cast in [
-        (r"%c", r"(.)", lambda x:x),
+    (re.compile(_token), _pattern, _cast)
+    for _token, _pattern, _cast in [
+        (r"%c", r"(.)", lambda x: x),
         (r"%\*c", r"(?:.)", None),
-
-        (r"%(\d)c", r"(.{%s})", lambda x:x),
+        (r"%(\d)c", r"(.{%s})", lambda x: x),
         (r"%\*(\d)c", r"(?:.{%s})", None),
-
         (r"%(\d)[di]", r"([+-]?\d{%s})", int),
         (r"%\*(\d)[di]", r"(?:[+-]?\d{%s})", None),
-
         ("%[di]", r"([+-]?\d+)", int),
         (r"%\*[di]", r"(?:[+-]?\d+)", None),
-
         ("%u", r"(\d+)", int),
         (r"%\*u", r"(?:\d+)", None),
-
         (r"%[fgeE]", r"([-+]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][-+]?\d+)?)", float),
         (r"%\*[fgeE]", r"(?:[-+]?(?:\d+(?:\.\d*)?|\.\d+)(?:[eE][-+]?\d+)?)", None),
-
-        (r"%s", r"(\S+)", lambda x:x),
+        (r"%s", r"(\S+)", lambda x: x),
         (r"%\*s", r"(?:\S+)", None),
-
-        (r"%([xX])", r"(0%s[\dA-Za-f]+)", lambda x:int(x, 16)),
+        (r"%([xX])", r"(0%s[\dA-Za-f]+)", lambda x: int(x, 16)),
         (r"%\*([xX])", r"(?:0%s[\dA-Za-f]+)", None),
-
-        (r"%o", r"(0[0-7]*)", lambda x:int(x, 8)),
+        (r"%o", r"(0[0-7]*)", lambda x: int(x, 8)),
         (r"%\*o", r"(?:0[0-7]*)", None),
-    ]]
+    ]
+]
 
 
 # Cache formats
 SCANF_CACHE_SIZE = 1000
 
 
 @lru_cache(maxsize=SCANF_CACHE_SIZE)
@@ -111,17 +106,17 @@
             char = format[i]
             # escape special characters
             if char in "|^$()[]-.+*?{}<>\\":
                 format_pat += "\\"
             format_pat += char
             i += 1
     if DEBUG:
-        print("DEBUG: %r -> %s" % (format, format_pat))
+        print(f"DEBUG: {format!r} -> {format_pat}")
     if collapseWhitespace:
-        format_pat = re.sub(r'\s+', r'\\s+', format_pat)
+        format_pat = re.sub(r"\s+", r"\\s+", format_pat)
 
     format_re = re.compile(format_pat)
     return format_re, cast_list
 
 
 def scanf(format, s=None, collapseWhitespace=True):
     """
@@ -166,15 +161,15 @@
     pattern string and ignore the rest.
 
     If *text* is supplied, it will be parsed according to the *pattern* string.
     If *text* is not supplied, the file at *filepath* will be opened and parsed.
     """
     y = []
     if text is None:
-        textsource = open(filepath, 'r')
+        textsource = open(filepath)
     else:
         textsource = text.splitlines()
 
     for line in textsource:
         match = scanf(pattern, line)
         if match:
             if len(y) == 0:
@@ -187,8 +182,9 @@
         textsource.close()
 
     return y
 
 
 if __name__ == "__main__":
     import doctest
+
     doctest.testmod(verbose=True, report=True)
```

### Comparing `OApackage-2.7.6/oapackage/conference.py` & `OApackage-2.7.7/oapackage/conference.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,68 +8,74 @@
 import numpy as np
 
 import oapackage
 
 # %%
 
 
-def momentMatrix(k):
-    """ Return the moment matrix of a conference design
+def momentMatrix(k: int) -> np.ndarray:
+    """Return the moment matrix of a conference design
 
     Args:
         k (int): number of columns of the conference design
     Returns:
         array: moment matrix
     """
     pk = int(1 + 0.5 * k * (k + 1) + k)
     M = np.zeros((pk, pk))
     M[0, 0] = 1
-    M[0, int(0.5 * k * (k + 1) + 1):] = 1. / 3
-    M[int(0.5 * k * (k + 1) + 1):, 0] = 1. / 3
-    M[1:(k + 1), 1:(k + 1)] = np.eye(k) * 1. / 3
-    M[(k + 1):int(0.5 * k * (k + 1) + 1), (k + 1):int(0.5 * k * (k + 1) + 1)] = np.eye(int(0.5 * k * (k - 1))) / 9.
-    M[int(0.5 * k * (k + 1) + 1):, int(0.5 * k * (k + 1) + 1):] = np.eye(k) / 5 + (np.ones((k, k)) - np.eye(k)) / 9.
+    M[0, int(0.5 * k * (k + 1) + 1) :] = 1.0 / 3
+    M[int(0.5 * k * (k + 1) + 1) :, 0] = 1.0 / 3
+    M[1 : (k + 1), 1 : (k + 1)] = np.eye(k) * 1.0 / 3
+    M[(k + 1) : int(0.5 * k * (k + 1) + 1), (k + 1) : int(0.5 * k * (k + 1) + 1)] = np.eye(int(0.5 * k * (k - 1))) / 9.0
+    M[int(0.5 * k * (k + 1) + 1) :, int(0.5 * k * (k + 1) + 1) :] = np.eye(k) / 5 + (np.ones((k, k)) - np.eye(k)) / 9.0
     return M
 
 
 def _leftDivide(A, B):
-    r""" Perform left division of a matrix
+    r"""Perform left division of a matrix
 
     Args:
         A (aray)
         B (array)
     Returns:
         array: the result of A\B
     """
     solution = np.linalg.solve(A.T.dot(A), A.T.dot(B))
     return solution
 
 
 def modelStatistics(dsd, verbose=0, moment_matrix=None, use_condition_number=True):
-    """ Calculate statistics of a definitive screening design from the model matrix
+    """Calculate statistics of a definitive screening design from the model matrix
 
     Args:
         dsd (array): definitive screening design
     Returns:
       list: calculated statistics. Calculated are whether the model is estible, the Defficiency and the inverse APV.
     """
     ncolumns = dsd.shape[1]
-    modelmatrix = np.array(oapackage.conference_design2modelmatrix(dsd, 'q', verbose=0))
+    modelmatrix = np.array(oapackage.conference_design2modelmatrix(dsd, "q", verbose=0))
     M = (modelmatrix.T).dot(modelmatrix)
 
     if use_condition_number:
         fullrank = np.linalg.cond(M) < 1000
     else:
         mr = np.linalg.matrix_rank(M)
-        fullrank = (mr == modelmatrix.shape[1])
+        fullrank = mr == modelmatrix.shape[1]
         if verbose >= 2:
-            print('modelStatistics: fullrank %d, condition number %.4f' % (fullrank, np.linalg.cond(M), ))
+            print(
+                "modelStatistics: fullrank %d, condition number %.4f"
+                % (
+                    fullrank,
+                    np.linalg.cond(M),
+                )
+            )
 
     if verbose >= 2:
-        print('modelStatistics: condition number: %s' % (np.linalg.cond(M)))
+        print("modelStatistics: condition number: %s" % (np.linalg.cond(M)))
     if fullrank:
         if moment_matrix is None:
             moment_matrix = momentMatrix(ncolumns)
         Eest = 1
         pk = int(1 + ncolumns + ncolumns * (ncolumns + 1) / 2)
         kappa = np.linalg.det(M)
         lnkappa = np.log(kappa) / (pk)
@@ -82,15 +88,15 @@
         Defficiency = 0
         invAPV = 0
 
     return Eest, Defficiency, invAPV
 
 
 def conferenceProjectionStatistics(array, ncolumns=4, verbose=0):
-    """ Calculate the projection statistics of a conference design
+    """Calculate the projection statistics of a conference design
 
     The PECk, PICk and PPCk are calculated with k the number of columns specified.
     The projection statistics are calculated by determined the :meth:`modelStatistics` of all k-column subdesigns
     and then taking the mean of the statistics for the subdesigns.
     For more details of the calculation, see https://oapackage.readthedocs.io/.
 
     Args:
@@ -113,10 +119,12 @@
         Eest, D, invAPV = modelStatistics(proj_dsd, verbose=0, moment_matrix=moment_matrix)
 
         Deff[idx] = D
         Eestx[idx] = Eest
         invAPV_values[idx] = invAPV
     pec, pic, ppc = np.mean(Eestx), np.mean(Deff), np.mean(invAPV_values)
     if verbose:
-        print('conferenceProjectionStatistics: projection to %d columns: PEC %.3f PIC %.3f PPC %.3f  ' %
-              (ncolumns, pec, pic, ppc))
+        print(
+            "conferenceProjectionStatistics: projection to %d columns: PEC %.3f PIC %.3f PPC %.3f  "
+            % (ncolumns, pec, pic, ppc)
+        )
     return pec, pic, ppc
```

### Comparing `OApackage-2.7.6/oapackage/graphtools.py` & `OApackage-2.7.7/oapackage/graphtools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ Module to work with designs and graphs
 
 @author: Pieter Eendebak <pieter.eendebak@gmail.com>
 """
 
 # %% Load packages
+from typing import Any, List, Tuple
+
 import numpy as np
 
 import oapackage
 
 # %%
 
 
@@ -21,33 +23,32 @@
     Example
     -------
     >     im, colors, r = oa2graph( A, oadata );
 
     """
     A = al.getarray(verbose=0)
     if verbose:
-        print('oa2graph: array of shape %s' % (A.shape, ))
+        print(f"oa2graph: array of shape {A.shape}")
     nrows = adata.N
     ncols = A.shape[1]
     nColumnLevelVertices = sum(adata.factor_levels())
     nVertices = adata.N + ncols + nColumnLevelVertices
     nColVertices = ncols
     colOffset = adata.N
 
     s = np.array(adata.factor_levels())
     sc = np.cumsum(s)
     sc0 = np.hstack(([0], sc))
     qq = np.ones(nColumnLevelVertices)  # colors for column level vertices
     for ii in range(sc.size):
-        qq[sc0[ii]:sc0[ii + 1]] = 2 + ii
+        qq[sc0[ii] : sc0[ii + 1]] = 2 + ii
     qq = 2 * np.ones(nColumnLevelVertices)  # colors for column level vertices
 
     vertexOffsets = adata.N + ncols + np.hstack((0, s[0:-1])).cumsum()
-    colors = np.hstack(
-        (np.zeros(adata.N), np.ones(ncols), qq))
+    colors = np.hstack((np.zeros(adata.N), np.ones(ncols), qq))
 
     im = np.zeros((nVertices, nVertices))  # incidence matrix
 
     for row in range(0, nrows):
         idx = A[row, :] + vertexOffsets
         im[row, idx] = 1
         im[idx, row] = 1
@@ -57,19 +58,19 @@
         for col in range(0, ncols):
             sel = vertexOffsets[col] + range(0, s[col])
             im[colOffset + col, sel] = colidx
             im[sel, colOffset + col] = colidx
 
     # The non-row vertices do not have any connections to other non-row
     # vertices.
-    return im, colors, dict({'adata': adata, 'im': im, 'colors': colors, 'nVertices': nVertices})
+    return im, colors, dict({"adata": adata, "im": im, "colors": colors, "nVertices": nVertices})
 
 
-def selectIsomorphismClasses(sols, verbose=1):
-    """ Select isomorphism classes from a list of designs
+def selectIsomorphismClasses(sols, verbose: int = 1) -> Tuple[List[int], List[Any]]:
+    """Select isomorphism classes from a list of designs
 
     Args:
         sols (list of arrays): list of arrays from which to determine the unique ones
         verbose (int): verbosity level
     Return:
         indices (list of integers): indices of the isomorphism classes
         mm (list of arrays): the arrays in normal form
@@ -85,16 +86,15 @@
         >>> representatives = [sols[idx] for idx in unique_indices]
 
     """
 
     mm = []
     for ii, al in enumerate(sols):
         if verbose:
-            oapackage.tprint(
-                'selectIsomorphismClasses: process aray %d/%d' % (ii, len(sols)))
+            oapackage.tprint("selectIsomorphismClasses: process aray %d/%d" % (ii, len(sols)))
         al = oapackage.makearraylink(al)
 
         tt = oapackage.reduceOAnauty(al, verbose >= 2)
 
         alx = tt.apply(al)
         mm.append(np.array(alx))
 
@@ -104,11 +104,10 @@
     for ii in range(nn):
         qq[ii] = mm[ii].flatten()
 
     # Trick to make unique work...
     _, indices = np.unique(np.vstack(qq), axis=0, return_inverse=True)
 
     if verbose >= 1:
-        print('selectIsomorphismClasses: reduce %d to %d' %
-              (len(sols), np.unique(indices).size))
+        print("selectIsomorphismClasses: reduce %d to %d" % (len(sols), np.unique(indices).size))
 
     return indices, mm
```

### Comparing `OApackage-2.7.6/oapackage/markup.py` & `OApackage-2.7.7/oapackage/markup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,113 +1,107 @@
 # This code is in the public domain, it comes
 # with absolutely no warranty and you can do
 # absolutely whatever you want with it.
+import keyword
 
-__date__ = '16 March 2015'
-__version__ = '1.10'
+__date__ = "16 March 2015"
+__version__ = "1.10"
 __doc__ = """
 This is markup.py - a Python module that attempts to
 make it easier to generate HTML/XML from a Python program
 in an intuitive, lightweight, customizable and pythonic way.
 It works with both python 2 and 3.
 
 The code is in the public domain.
 
-Version: %s as of %s.
+Version: {} as of {}.
 
 Documentation and further info is at http://markup.sourceforge.net/
 
 Please send bug reports, feature requests, enhancement
 ideas or questions to nogradi at gmail dot com.
 
 Installation: drop markup.py somewhere into your Python path.
-""" % (__version__, __date__)
-
-try:
-    basestring
-    import string
-except BaseException:
-    # python 3
-    basestring = str
-    string = str
-    long = int
-
-# tags which are reserved python keywords will be referred
-# to by a leading underscore otherwise we end up with a syntax error
-import keyword
+""".format(
+    __version__,
+    __date__,
+)
+
+# python 3
+basestring = str
+string = str
+long = int
 
 
 class element:
 
     """This class handles the addition of a new element."""
 
-    def __init__(self, tag, case='lower', parent=None):
+    def __init__(self, tag, case="lower", parent=None):
         self.parent = parent
 
-        if case == 'upper':
+        if case == "upper":
             self.tag = tag.upper()
-        elif case == 'lower':
+        elif case == "lower":
             self.tag = tag.lower()
-        elif case == 'given':
+        elif case == "given":
             self.tag = tag
         else:
             self.tag = tag
 
     def __call__(self, *args, **kwargs):
         if len(args) > 1:
             raise ArgumentError(self.tag)
 
         # if class_ was defined in parent it should be added to every element
         if self.parent is not None and self.parent.class_ is not None:
-            if 'class_' not in kwargs:
-                kwargs['class_'] = self.parent.class_
+            if "class_" not in kwargs:
+                kwargs["class_"] = self.parent.class_
 
         if self.parent is None and len(args) == 1:
-            x = [self.render(self.tag, False, myarg, mydict)
-                 for myarg, mydict in _argsdicts(args, kwargs)]
-            return '\n'.join(x)
+            x = [self.render(self.tag, False, myarg, mydict) for myarg, mydict in _argsdicts(args, kwargs)]
+            return "\n".join(x)
         elif self.parent is None and len(args) == 0:
-            x = [self.render(self.tag, True, myarg, mydict)
-                 for myarg, mydict in _argsdicts(args, kwargs)]
-            return '\n'.join(x)
+            x = [self.render(self.tag, True, myarg, mydict) for myarg, mydict in _argsdicts(args, kwargs)]
+            return "\n".join(x)
 
         if self.tag in self.parent.twotags:
             for myarg, mydict in _argsdicts(args, kwargs):
                 self.render(self.tag, False, myarg, mydict)
         elif self.tag in self.parent.onetags:
             if len(args) == 0:
                 for myarg, mydict in _argsdicts(args, kwargs):
                     # here myarg is always None, because len( args ) = 0
                     self.render(self.tag, True, myarg, mydict)
             else:
                 raise ClosingError(self.tag)
-        elif self.parent.mode == 'strict_html' and self.tag in self.parent.deptags:
+        elif self.parent.mode == "strict_html" and self.tag in self.parent.deptags:
             raise DeprecationError(self.tag)
         else:
             raise InvalidElementError(self.tag, self.parent.mode)
 
     def render(self, tag, single, between, kwargs):
         """Append the actual tags to content."""
 
         out = "<%s" % tag
         for key, value in list(kwargs.items()):
             # when value is None that means stuff like <... checked>
             if value is not None:
                 # strip this so class_ will mean class, etc.
-                key = key.strip('_')
+                key = key.strip("_")
                 # special cases, maybe change _ to - overall?
-                if key == 'http_equiv':
-                    key = 'http-equiv'
-                elif key == 'accept_charset':
-                    key = 'accept-charset'
-                out = "%s %s=\"%s\"" % (out, key, escape(value))
+                if key == "http_equiv":
+                    key = "http-equiv"
+                elif key == "accept_charset":
+                    key = "accept-charset"
+                out = f'{out} {key}="{escape(value)}"'
             else:
-                out = "%s %s" % (out, key)
+                out = f"{out} {key}"
         if between is not None:
-            out = "%s>%s</%s>" % (out, between, tag)
+            out = f"{out}>{between}</{tag}>"
         else:
             if single:
                 out = "%s />" % out
             else:
                 out = "%s>" % out
         if self.parent is not None:
             self.parent.content.append(out)
@@ -117,32 +111,32 @@
     def close(self):
         """Append a closing tag unless element has only opening tag."""
 
         if self.tag in self.parent.twotags:
             self.parent.content.append("</%s>" % self.tag)
         elif self.tag in self.parent.onetags:
             raise ClosingError(self.tag)
-        elif self.parent.mode == 'strict_html' and self.tag in self.parent.deptags:
+        elif self.parent.mode == "strict_html" and self.tag in self.parent.deptags:
             raise DeprecationError(self.tag)
 
     def open(self, **kwargs):
         """Append an opening tag."""
 
         if self.tag in self.parent.twotags or self.tag in self.parent.onetags:
             self.render(self.tag, False, None, kwargs)
-        elif self.mode == 'strict_html' and self.tag in self.parent.deptags:
+        elif self.mode == "strict_html" and self.tag in self.parent.deptags:
             raise DeprecationError(self.tag)
 
 
 class page:
 
     """This is our main class representing a document. Elements are added
     as attributes of an instance of this class."""
 
-    def __init__(self, mode='strict_html', case='lower', onetags=None, twotags=None, separator='\n', class_=None):
+    def __init__(self, mode="strict_html", case="lower", onetags=None, twotags=None, separator="\n", class_=None):
         """Stuff that effects the whole document.
 
         mode -- 'strict_html'   for HTML 4.01 (default)
                 'html'          alias for 'strict_html'
                 'loose_html'    to allow some deprecated elements
                 'xml'           to allow arbitrary elements
 
@@ -156,82 +150,143 @@
                                 the set of valid elements in 'xml' mode
                                 invalid elements will raise appropriate exceptions
 
         separator --            string to place between added elements, defaults to newline
 
         class_ --               a class that will be added to every element if defined"""
 
-        valid_onetags = ["AREA", "BASE", "BR", "COL", "FRAME",
-                         "HR", "IMG", "INPUT", "LINK", "META", "PARAM"]
-        valid_twotags = ["A", "ABBR", "ACRONYM", "ADDRESS", "B", "BDO", "BIG", "BLOCKQUOTE", "BODY", "BUTTON",
-                         "CAPTION", "CITE", "CODE", "COLGROUP", "DD", "DEL", "DFN", "DIV", "DL", "DT", "EM", "FIELDSET",
-                         "FORM", "FRAMESET", "H1", "H2", "H3", "H4", "H5", "H6", "HEAD", "HTML", "I", "IFRAME", "INS",
-                         "KBD", "LABEL", "LEGEND", "LI", "MAP", "NOFRAMES", "NOSCRIPT", "OBJECT", "OL", "OPTGROUP",
-                         "OPTION", "P", "PRE", "Q", "SAMP", "SCRIPT", "SELECT", "SMALL", "SPAN", "STRONG", "STYLE",
-                         "SUB", "SUP", "TABLE", "TBODY", "TD", "TEXTAREA", "TFOOT", "TH", "THEAD", "TITLE", "TR",
-                         "TT", "UL", "VAR"]
+        valid_onetags = ["AREA", "BASE", "BR", "COL", "FRAME", "HR", "IMG", "INPUT", "LINK", "META", "PARAM"]
+        valid_twotags = [
+            "A",
+            "ABBR",
+            "ACRONYM",
+            "ADDRESS",
+            "B",
+            "BDO",
+            "BIG",
+            "BLOCKQUOTE",
+            "BODY",
+            "BUTTON",
+            "CAPTION",
+            "CITE",
+            "CODE",
+            "COLGROUP",
+            "DD",
+            "DEL",
+            "DFN",
+            "DIV",
+            "DL",
+            "DT",
+            "EM",
+            "FIELDSET",
+            "FORM",
+            "FRAMESET",
+            "H1",
+            "H2",
+            "H3",
+            "H4",
+            "H5",
+            "H6",
+            "HEAD",
+            "HTML",
+            "I",
+            "IFRAME",
+            "INS",
+            "KBD",
+            "LABEL",
+            "LEGEND",
+            "LI",
+            "MAP",
+            "NOFRAMES",
+            "NOSCRIPT",
+            "OBJECT",
+            "OL",
+            "OPTGROUP",
+            "OPTION",
+            "P",
+            "PRE",
+            "Q",
+            "SAMP",
+            "SCRIPT",
+            "SELECT",
+            "SMALL",
+            "SPAN",
+            "STRONG",
+            "STYLE",
+            "SUB",
+            "SUP",
+            "TABLE",
+            "TBODY",
+            "TD",
+            "TEXTAREA",
+            "TFOOT",
+            "TH",
+            "THEAD",
+            "TITLE",
+            "TR",
+            "TT",
+            "UL",
+            "VAR",
+        ]
         deprecated_onetags = ["BASEFONT", "ISINDEX"]
-        deprecated_twotags = [
-            "APPLET", "CENTER", "DIR", "FONT", "MENU", "S", "STRIKE", "U"]
+        deprecated_twotags = ["APPLET", "CENTER", "DIR", "FONT", "MENU", "S", "STRIKE", "U"]
 
         self.header = []
         self.content = []
         self.footer = []
         self.case = case
         self.separator = separator
 
         # init( ) sets it to True so we know that </body></html> has to be
         # printed at the end
         self._full = False
         self.class_ = class_
 
-        if mode == 'strict_html' or mode == 'html':
+        if mode == "strict_html" or mode == "html":
             self.onetags = valid_onetags
             self.onetags += list(map(string.lower, self.onetags))
             self.twotags = valid_twotags
             self.twotags += list(map(string.lower, self.twotags))
             self.deptags = deprecated_onetags + deprecated_twotags
             self.deptags += list(map(string.lower, self.deptags))
-            self.mode = 'strict_html'
-        elif mode == 'loose_html':
+            self.mode = "strict_html"
+        elif mode == "loose_html":
             self.onetags = valid_onetags + deprecated_onetags
             self.onetags += list(map(string.lower, self.onetags))
             self.twotags = valid_twotags + deprecated_twotags
             self.twotags += list(map(string.lower, self.twotags))
             self.mode = mode
-        elif mode == 'xml':
+        elif mode == "xml":
             if onetags and twotags:
                 self.onetags = onetags
                 self.twotags = twotags
             elif (onetags and not twotags) or (twotags and not onetags):
                 raise CustomizationError()
             else:
                 self.onetags = russell()
                 self.twotags = russell()
             self.mode = mode
         else:
             raise ModeError(mode)
 
     def __getattr__(self, attr):
-
         # tags should start with double underscore
         if attr.startswith("__") and attr.endswith("__"):
             raise AttributeError(attr)
         # tag with single underscore should be a reserved keyword
-        if attr.startswith('_'):
-            attr = attr.lstrip('_')
+        if attr.startswith("_"):
+            attr = attr.lstrip("_")
             if attr not in keyword.kwlist:
                 raise AttributeError(attr)
 
         return element(attr, case=self.case, parent=self)
 
     def __str__(self):
-
-        if self._full and (self.mode == 'strict_html' or self.mode == 'loose_html'):
-            end = ['</body>', '</html>']
+        if self._full and (self.mode == "strict_html" or self.mode == "loose_html"):
+            end = ["</body>", "</html>"]
         else:
             end = []
 
         return self.separator.join(self.header + self.content + self.footer + end)
 
     def __call__(self, escape=False):
         """Return the document as a string.
@@ -257,16 +312,31 @@
         """Add some text to the top of the document"""
         self.header.append(text)
 
     def addcontent(self, text):
         """Add some text to the main part of the document"""
         self.content.append(text)
 
-    def init(self, lang='en', css=None, metainfo=None, title=None, header=None, htmlheader=None,
-             footer=None, charset=None, encoding=None, doctype=None, bodyattrs=None, htmlattrs=None, script=None, base=None):
+    def init(
+        self,
+        lang="en",
+        css=None,
+        metainfo=None,
+        title=None,
+        header=None,
+        htmlheader=None,
+        footer=None,
+        charset=None,
+        encoding=None,
+        doctype=None,
+        bodyattrs=None,
+        htmlattrs=None,
+        script=None,
+        base=None,
+    ):
         """This method is used for complete documents with appropriate
         doctype, encoding, title, etc information. For an HTML/XML snippet
         omit this method.
 
         lang --     language, usually a two character string, will appear
                     as <html lang='en'> in html mode (ignored in xml mode)
 
@@ -305,130 +375,124 @@
 
         doctype --  the document type string, defaults to
                     <!DOCTYPE HTML PUBLIC '-//W3C//DTD HTML 4.01 Transitional//EN'>
                     in html mode (ignored in xml mode)"""
 
         self._full = True
 
-        if self.mode == 'strict_html' or self.mode == 'loose_html':
+        if self.mode == "strict_html" or self.mode == "loose_html":
             if doctype is None:
                 doctype = "<!DOCTYPE HTML PUBLIC '-//W3C//DTD HTML 4.01 Transitional//EN'>"
             self.header.append(doctype)
             if htmlattrs is not None:
                 self.html(lang=lang, **htmlattrs)
             else:
                 self.html(lang=lang)
             self.head()
             if charset is not None:
-                self.meta(
-                    http_equiv='Content-Type', content="text/html; charset=%s" % charset)
+                self.meta(http_equiv="Content-Type", content="text/html; charset=%s" % charset)
             if metainfo is not None:
                 self.metainfo(metainfo)
             if css is not None:
                 self.css(css)
             if title is not None:
                 self.title(title)
             if script is not None:
                 self.scripts(script)
             if htmlheader is not None:
                 self.content.append(htmlheader)
             if base is not None:
-                self.base(href='%s' % base)
+                self.base(href="%s" % base)
             self.head.close()
             if bodyattrs is not None:
                 self.body(**bodyattrs)
             else:
                 self.body()
             if header is not None:
                 self.content.append(header)
             if footer is not None:
                 self.footer.append(footer)
 
-        elif self.mode == 'xml':
+        elif self.mode == "xml":
             if doctype is None:
                 if encoding is not None:
                     doctype = "<?xml version='1.0' encoding='%s' ?>" % encoding
                 else:
                     doctype = "<?xml version='1.0' ?>"
             self.header.append(doctype)
 
     def css(self, filelist):
         """This convenience function is only useful for html.
         It adds css stylesheet(s) to the document via the <link> element."""
 
         if isinstance(filelist, basestring):
-            self.link(
-                href=filelist, rel='stylesheet', type='text/css', media='all')
+            self.link(href=filelist, rel="stylesheet", type="text/css", media="all")
         else:
             for file in filelist:
-                self.link(
-                    href=file, rel='stylesheet', type='text/css', media='all')
+                self.link(href=file, rel="stylesheet", type="text/css", media="all")
 
     def metainfo(self, mydict):
         """This convenience function is only useful for html.
         It adds meta information via the <meta> element, the argument is
         a dictionary of the form { 'name':'content' }."""
 
         if isinstance(mydict, dict):
             for name, content in list(mydict.items()):
                 self.meta(name=name, content=content)
         else:
-            raise TypeError(
-                "Metainfo should be called with a dictionary argument of name:content pairs.")
+            raise TypeError("Metainfo should be called with a dictionary argument of name:content pairs.")
 
     def scripts(self, mydict):
         """Only useful in html, mydict is dictionary of src:type pairs or a list
         of script sources [ 'src1', 'src2', ... ] in which case 'javascript' is assumed for type.
         Will be rendered as <script type='text/type' src=src></script>"""
 
         if isinstance(mydict, dict):
             for src, type in list(mydict.items()):
-                self.script('', src=src, type='text/%s' % type)
+                self.script("", src=src, type="text/%s" % type)
         else:
             try:
                 for src in mydict:
-                    self.script('', src=src, type='text/javascript')
+                    self.script("", src=src, type="text/javascript")
             except BaseException:
-                raise TypeError(
-                    "Script should be given a dictionary of src:type pairs or a list of javascript src's.")
+                raise TypeError("Script should be given a dictionary of src:type pairs or a list of javascript src's.")
 
 
 class _oneliner:
 
     """An instance of oneliner returns a string corresponding to one element.
     This class can be used to write 'oneliners' that return a string
     immediately so there is no need to instantiate the page class."""
 
-    def __init__(self, case='lower'):
+    def __init__(self, case="lower"):
         self.case = case
 
     def __getattr__(self, attr):
-
         # tags should start with double underscore
         if attr.startswith("__") and attr.endswith("__"):
             raise AttributeError(attr)
         # tag with single underscore should be a reserved keyword
-        if attr.startswith('_'):
-            attr = attr.lstrip('_')
+        if attr.startswith("_"):
+            attr = attr.lstrip("_")
             if attr not in keyword.kwlist:
                 raise AttributeError(attr)
 
         return element(attr, case=self.case, parent=None)
 
 
-oneliner = _oneliner(case='lower')
-upper_oneliner = _oneliner(case='upper')
-given_oneliner = _oneliner(case='given')
+oneliner = _oneliner(case="lower")
+upper_oneliner = _oneliner(case="upper")
+given_oneliner = _oneliner(case="given")
 
 
 def _argsdicts(args, mydict):
-    """A utility generator that pads argument list and dictionary values, will only be called with len( args ) = 0, 1."""
+    """A utility generator that pads argument list and dictionary values, will only be called with len(args) = 0, 1."""
 
     if len(args) == 0:
-        args = None,
+        args = (None,)
     elif len(args) == 1:
         args = _totuple(args[0])
     else:
         raise Exception("We should have never gotten here.")
 
     mykeys = list(mydict.keys())
     myvalues = list(map(_totuple, list(mydict.values())))
@@ -450,75 +514,80 @@
         yield thisarg, thisdict
 
 
 def _totuple(x):
     """Utility stuff to convert string, int, long, float, None or anything to a usable tuple."""
 
     if isinstance(x, basestring):
-        out = x,
+        out = (x,)
     elif isinstance(x, (int, long, float)):
-        out = str(x),
+        out = (str(x),)
     elif x is None:
-        out = None,
+        out = (None,)
     else:
         out = tuple(x)
 
     return out
 
 
 def escape(text, newline=False):
     """Escape special html characters."""
 
     if isinstance(text, basestring):
-        if '&' in text:
-            text = text.replace('&', '&amp;')
-        if '>' in text:
-            text = text.replace('>', '&gt;')
-        if '<' in text:
-            text = text.replace('<', '&lt;')
-        if '\"' in text:
-            text = text.replace('\"', '&quot;')
-        if '\'' in text:
-            text = text.replace('\'', '&quot;')
+        if "&" in text:
+            text = text.replace("&", "&amp;")
+        if ">" in text:
+            text = text.replace(">", "&gt;")
+        if "<" in text:
+            text = text.replace("<", "&lt;")
+        if '"' in text:
+            text = text.replace('"', "&quot;")
+        if "'" in text:
+            text = text.replace("'", "&quot;")
         if newline:
-            if '\n' in text:
-                text = text.replace('\n', '<br>')
+            if "\n" in text:
+                text = text.replace("\n", "<br>")
 
     return text
 
 
 _escape = escape
 
 
 def unescape(text):
     """Inverse of escape."""
 
     if isinstance(text, basestring):
-        if '&amp;' in text:
-            text = text.replace('&amp;', '&')
-        if '&gt;' in text:
-            text = text.replace('&gt;', '>')
-        if '&lt;' in text:
-            text = text.replace('&lt;', '<')
-        if '&quot;' in text:
-            text = text.replace('&quot;', '\"')
+        if "&amp;" in text:
+            text = text.replace("&amp;", "&")
+        if "&gt;" in text:
+            text = text.replace("&gt;", ">")
+        if "&lt;" in text:
+            text = text.replace("&lt;", "<")
+        if "&quot;" in text:
+            text = text.replace("&quot;", '"')
 
     return text
 
 
 class dummy:
 
     """A dummy class for attaching attributes."""
+
     pass
 
 
 doctype = dummy()
-doctype.frameset = """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">"""
+doctype.frameset = (
+    """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">"""
+)
 doctype.strict = """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">"""
-doctype.loose = """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">"""
+doctype.loose = (
+    """<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">"""
+)
 
 
 class russell:
 
     """A dummy class that contains anything."""
 
     def __contains__(self, item):
@@ -530,52 +599,49 @@
     """All our exceptions subclass this."""
 
     def __str__(self):
         return self.message
 
 
 class ClosingError(MarkupError):
-
     def __init__(self, tag):
         self.message = "The element '%s' does not accept non-keyword arguments (has no closing tag)." % tag
 
 
 class OpeningError(MarkupError):
-
     def __init__(self, tag):
         self.message = "The element '%s' can not be opened." % tag
 
 
 class ArgumentError(MarkupError):
-
     def __init__(self, tag):
         self.message = "The element '%s' was called with more than one non-keyword argument." % tag
 
 
 class InvalidElementError(MarkupError):
-
     def __init__(self, tag, mode):
-        self.message = "The element '%s' is not valid for your mode '%s'." % (
-            tag, mode)
+        self.message = f"The element '{tag}' is not valid for your mode '{mode}'."
 
 
 class DeprecationError(MarkupError):
-
     def __init__(self, tag):
-        self.message = "The element '%s' is deprecated, instantiate markup.page with mode='loose_html' to allow it." % tag
+        self.message = (
+            "The element '%s' is deprecated, instantiate markup.page with mode='loose_html' to allow it." % tag
+        )
 
 
 class ModeError(MarkupError):
-
     def __init__(self, mode):
-        self.message = "Mode '%s' is invalid, possible values: strict_html, html (alias for strict_html), loose_html, xml." % mode
+        self.message = (
+            "Mode '%s' is invalid, possible values: strict_html, html (alias for strict_html), loose_html, xml." % mode
+        )
 
 
 class CustomizationError(MarkupError):
-
     def __init__(self):
         self.message = "If you customize the allowed elements, you must define both types 'onetags' and 'twotags'."
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import sys
+
     sys.stdout.write(__doc__)
```

### Comparing `OApackage-2.7.6/oapackage/oahelper.py` & `OApackage-2.7.7/oapackage/oahelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,196 +25,202 @@
 import dateutil.parser
 import numpy as np
 
 try:
     import matplotlib
     import matplotlib.pyplot as plt
 except BaseException:
-    warnings.warn(
-        'oahelper: matplotlib cannot be found, not all functionality is available')
+    warnings.warn("oahelper: matplotlib cannot be found, not all functionality is available")
 
-import oalib
+import oalib  # type: ignore
 import oapackage
 from oapackage import markup
 
 
 def deprecated(func):
-    """ This is a decorator which can be used to mark functions
+    """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
-    when the function is used. """
+    when the function is used."""
 
     @functools.wraps(func)
     def new_func(*args, **kwargs):
         try:
             filename = inspect.getfile(func)
         except BaseException:
-            filename = '?'
+            filename = "?"
         try:
             lineno = inspect.getlineno(func)
         except BaseException:
             lineno = -1
         warnings.warn_explicit(
             f"Call to deprecated function {func.__name__}.",
             category=UserWarning,
             filename=filename,
             lineno=lineno,
         )
         return func(*args, **kwargs)
+
     return new_func
 
+
 # %%
 
 
 try:
     try:
         import qtpy.QtGui
         import qtpy.QtWidgets
     except BaseException:
         # no Qt support
         pass
 
     _applocalqt = None
 
     def monitorSizes(verbose=0):
-        """ Return monitor sizes """
-        if sys.platform == 'win32':
+        """Return monitor sizes"""
+        if sys.platform == "win32":
             import ctypes
+
             user32 = ctypes.windll.user32
-            wa = [
-                [0, 0, user32.GetSystemMetrics(0), user32.GetSystemMetrics(1)]]
+            wa = [[0, 0, user32.GetSystemMetrics(0), user32.GetSystemMetrics(1)]]
         else:
             _applocalqt = qtpy.QtWidgets.QApplication.instance()
             if _applocalqt is None:
                 _applocalqt = qtpy.QtWidgets.QApplication([])
                 _qd = qtpy.QtWidgets.QDesktopWidget()
             else:
                 _qd = qtpy.QtWidgets.QDesktopWidget()
 
             nmon = _qd.screenCount()
             wa = [_qd.screenGeometry(ii) for ii in range(nmon)]
             wa = [[w.x(), w.y(), w.width(), w.height()] for w in wa]
 
             if verbose:
                 for ii, w in enumerate(wa):
-                    print('monitor %d: %s' % (ii, str(w)))
+                    print("monitor %d: %s" % (ii, str(w)))
         return wa
+
 except BaseException:
+
     def monitorSizes(verbose=0):
-        """ Dummy implementation """
+        """Dummy implementation"""
         return [[0, 0, 1280, 720]]
 
 
 def guitest_monitorSizes():
     sizes = monitorSizes()
-    assert (isinstance(sizes, list))
+    assert isinstance(sizes, list)
 
 
 def tilefigs(lst, geometry, ww=None, raisewindows=False, tofront=False, verbose=0):
-    """ Tile figure windows on a specified area """
+    """Tile figure windows on a specified area"""
     mngr = plt.get_current_fig_manager()
     be = matplotlib.get_backend()
     if ww is None:
         ww = monitorSizes()[-1]
 
     w = ww[2] / geometry[0]
     h = ww[3] / geometry[1]
 
     if verbose:
-        print('tilefigs: ww %s, w %d h %d' % (str(ww), w, h))
+        print("tilefigs: ww %s, w %d h %d" % (str(ww), w, h))
     for ii, f in enumerate(lst):
         if not plt.fignum_exists(f):
             continue
         fig = plt.figure(f)
         iim = ii % np.prod(geometry)
         ix = iim % geometry[0]
         iy = np.floor(float(iim) / geometry[0])
         x = ww[0] + ix * w
         y = ww[1] + iy * h
         if verbose:
-            print('ii %d: %d %d: f %d: %d %d %d %d' %
-                  (ii, ix, iy, f, x, y, w, h))
+            print("ii %d: %d %d: f %d: %d %d %d %d" % (ii, ix, iy, f, x, y, w, h))
             if verbose >= 2:
-                print('  window %s' % mngr.get_window_title())
-        if be == 'WXAgg':
+                print("  window %s" % mngr.get_window_title())
+        if be == "WXAgg":
             fig.canvas.manager.window.SetPosition((x, y))
             fig.canvas.manager.window.SetSize((w, h))
-        if be == 'WX':
+        if be == "WX":
             fig.canvas.manager.window.SetPosition((x, y))
             fig.canvas.manager.window.SetSize((w, h))
-        if be == 'agg':
+        if be == "agg":
             fig.canvas.manager.window.SetPosition((x, y))
             fig.canvas.manager.window.resize(w, h)
-        if be == 'Qt4Agg' or be == 'QT4' or be == 'QT5Agg':
+        if be == "Qt4Agg" or be == "QT4" or be == "QT5Agg":
             # assume Qt canvas
             try:
                 fig.canvas.manager.window.move(x, y)
                 fig.canvas.manager.window.resize(w, h)
                 fig.canvas.manager.window.setGeometry(x, y, w, h)
                 # mngr.window.setGeometry(x,y,w,h)
             except Exception as ex:
-                print('problem with window manager: ', )
-                print('backend %s' % (be,))
+                print(
+                    "problem with window manager: ",
+                )
+                print(f"backend {be}")
                 logging.exception(ex)
         if raisewindows:
             mngr.window.raise_()
         if tofront:
             plt.figure(f)
 
 
 def plot2Dline(line, *args, **kwargs):
-    """ Plot a 2D line in a matplotlib figure """
-    if np.abs(line[1]) > .001:
+    """Plot a 2D line in a matplotlib figure"""
+    if np.abs(line[1]) > 0.001:
         xx = plt.xlim()
         xx = np.array(xx)
         yy = (-line[2] - line[0] * xx) / line[1]
         plt.plot(xx, yy, *args, **kwargs)
     else:
         yy = np.array(plt.ylim())
         xx = (-line[2] - line[1] * yy) / line[0]
         plt.plot(xx, yy, *args, **kwargs)
 
 
 # %% Make nice plots
 
-def niceplot(ax, fig=None, despine=True, verbose=0, figurebg=True,
-             tightlayout=True, legend=None, almost_black='#222222'):
-    """ Create a good looking plot
+
+def niceplot(
+    ax, fig=None, despine=True, verbose=0, figurebg=True, tightlayout=True, legend=None, almost_black="#222222"
+):
+    """Create a good looking plot
 
     The code:
         - removes spines
         - makes legend and spines lighter
         - makes legend lighter
 
     """
 
     if verbose:
-        print('niceplot: remove spines')
+        print("niceplot: remove spines")
 
-    spines_to_keep = ['bottom', 'left']
+    spines_to_keep = ["bottom", "left"]
     if despine:
-        spines_to_remove = ['top', 'right']
+        spines_to_remove = ["top", "right"]
         for spine in spines_to_remove:
             ax.spines[spine].set_visible(False)
     else:
-        spines_to_keep += ['top', 'right']
+        spines_to_keep += ["top", "right"]
     ax.get_xaxis().tick_bottom()
     ax.get_yaxis().tick_left()
 
     if verbose:
-        print('niceplot: reduce spine intensity')
+        print("niceplot: reduce spine intensity")
 
     for spine in spines_to_keep:
         ax.spines[spine].set_linewidth(0.5)
         ax.spines[spine].set_color(almost_black)
 
-    ax.tick_params(axis='both', direction='out')
+    ax.tick_params(axis="both", direction="out")
 
     if legend is not None:
         if verbose:
-            print('niceplot: adjust legend')
+            print("niceplot: adjust legend")
 
         # Remove the line around the legend box, and instead fill it with a light grey
         # Also only use one point for the scatterplot legend because the user will
         # get the idea after just one, they don't need three.
         light_grey = np.array([float(241) / float(255)] * 3)
         rect = legend.get_frame()
         rect.set_facecolor(light_grey)
@@ -227,40 +233,41 @@
         for t in texts:
             t.set_color(almost_black)
 
     if (fig is not None) and tightlayout:
         fig.tight_layout(pad=1.0)
 
     if figurebg and fig is not None:
-        fig.set_facecolor('w')
+        fig.set_facecolor("w")
 
     plt.draw()
     plt.show()
 
 
 def enlargelims(factor: float = 1.05):
-    """ Enlarge the limits of a plot
+    """Enlarge the limits of a plot
 
     Args:
         factor (float): factor by which to make the plot margins wider
     """
     xl = plt.xlim()
     d = (factor - 1) * (xl[1] - xl[0]) / 2
     xl = (xl[0] - d, xl[1] + d)
     plt.xlim(xl)
     yl = plt.ylim()
     d = (factor - 1) * (yl[1] - yl[0]) / 2
     yl = (yl[0] - d, yl[1] + d)
     plt.ylim(yl)
 
+
 # %%
 
 
 def helmert_contrasts(number_of_levels, verbose=0):
-    """ Calculate Helmert contrasts for a given number of levels
+    """Calculate Helmert contrasts for a given number of levels
 
     The Helmert contrasts are orthogonal and normalize such that the square equals to number of levels.
     Args:
         number_of_levels: number of levels in the number_of_levels
     Returns:
         array: array with calculated Helmert contrasts
     """
@@ -273,40 +280,41 @@
 
     for value in range(number_of_levels):
         for ii in range(0, md + 1):
             Z[value, ii] = value > ii - 1
 
         # make Helmert contrasts (these are automatically orthogonal)
         Z[value, 0] = 1
-        if (value > 0):
+        if value > 0:
             Z[value, value] = value
 
         for q in range(1, value):
             Z[value, q] = 0
         for q in range(value + 1, md + 1):
             Z[value, q] = -1
 
     if verbose:
-        print('helmert_contrasts: %d\n' % (number_of_levels))
-        print('Z (initial creation)')
+        print("helmert_contrasts: %d\n" % (number_of_levels))
+        print("Z (initial creation)")
         print(Z)
 
     # normalize the contrasts
     for ii in range(0, md):
         normalization = Z[:, (ii + 1)].T.dot(Z[:, ii + 1])
         if verbose:
-            print('helmert_contrasts: normalize number_of_levels tmp: %s ' % (normalization,))
-        main_effects[:, meoffset + ii:(meoffset + ii + 1)] = np.sqrt(N) * \
-            Z[:, (ii + 1):(ii + 2)] / np.sqrt(normalization)
+            print(f"helmert_contrasts: normalize number_of_levels tmp: {normalization} ")
+        main_effects[:, meoffset + ii : (meoffset + ii + 1)] = (
+            np.sqrt(N) * Z[:, (ii + 1) : (ii + 2)] / np.sqrt(normalization)
+        )
 
     return main_effects
 
 
 def selectParetoArrays(array_list, pareto_object):
-    """ Select arrays using a Pareto object
+    """Select arrays using a Pareto object
 
     Args:
         array_list (list): list of arrays
         pareto (object): oapackage Pareto object
     Returns:
         list: list with all Pareto optimal designs
     """
@@ -314,49 +322,51 @@
     paretoidx = np.array(pareto_object.allindices())
     ww = oalib.longVector(tuple(paretoidx.tolist()))
     oalib.selectArrays(array_list, ww, paretoarrays)
     return paretoarrays
 
 
 def joinArrayLists(ww):
-    """ Concetenate a list of array lists into a single list """
+    """Concetenate a list of array lists into a single list"""
     ll = oalib.arraylist_t()
     for w in ww:
         for al in w:
             ll.push_back(al)
     return ll
 
 
 def createPareto(dds, verbose=1):
-    """ Create Pareto object from dataset """
+    """Create Pareto object from dataset"""
     pp = oapackage.ParetoDoubleLong()
 
     for ii in range(dds.shape[0]):
         v = (dds[ii, :]).astype(np.float64)
         pp.addvalue(v, ii)
 
     if verbose:
         pp.show(verbose)
     return pp
 
 
 # %% Utils
 
 
-def static_var(varname, value):
-    """ Helper function to create a static variable """
+def static_var(varname: str, value: Any):
+    """Helper function to create a static variable"""
+
     def decorate(func):
         setattr(func, varname, value)
         return func
+
     return decorate
 
 
 @static_var("time", 0)
 def tprint(string, dt=1, output=False):
-    """ Print progress of a loop every dt seconds """
+    """Print progress of a loop every dt seconds"""
     if (time.time() - tprint.time) > dt:
         print(string)
         tprint.time = time.time()
         if output:
             return True
         else:
             return
@@ -364,191 +374,190 @@
         if output:
             return False
         else:
             return
 
 
 def timeString(tt=None) -> str:
-    """ Return a string with the current time or specified time
+    """Return a string with the current time or specified time
 
     Args:
         tt (struct_time or None): time to convert
     Returns:
         Formatted time
     """
     if tt is None:
         tt = gmtime()
     ts = strftime("%Y-%m-%d %H:%M:%S", tt)
     return ts
 
 
-def findfilesR(directory, pattern):
-    """ Get a list of files (recursive)
+def findfilesR(directory: str, pattern) -> List[str]:
+    """Get a list of files (recursive)
 
     Args:
         directory (str): directory to search
         patt (str): pattern
     Returns:
         list: list of matched files
     """
     lst = []
     for root, _, files in os.walk(directory, topdown=False):
         lst += [os.path.join(root, f) for f in files]
     rr = re.compile(pattern)
-    lst = [l for l in lst if re.match(rr, l)]
+    lst = [filename for filename in lst if re.match(rr, filename)]
     return lst
 
 
-def findfiles(directory, pattern=None):
-    """ Get a list of files
+def findfiles(directory: str, pattern: Optional[str] = None) -> List[str]:
+    """Get a list of files
     Args:
-        directory (str): directory to search
-        patt (str): pattern
+        directory: directory to search
+        patt : pattern
     Returns:
-        list: list of matched files
+        List of matched files
     """
     lst = os.listdir(directory)
     if pattern is not None:
         rr = re.compile(pattern)
-        lst = [l for l in lst if re.match(rr, l)]
+        lst = [filename for filename in lst if re.match(rr, filename)]
     return lst
 
 
-def finddirectories(directory, pattern=None):
-    """ Get a list of directories
+def finddirectories(directory: str, pattern: Optional[str] = None) -> List[str]:
+    """Get a list of directories
     Args:
-        directory (str): directory to search
-        patt (str): pattern
+        directory: directory to search
+        patt: pattern
     Returns:
-        list: list of matched directories
+        List of matched directories
     """
     lst = os.listdir(directory)
     if pattern is not None:
         rr = re.compile(pattern)
-        lst = [l for l in lst if re.match(rr, l)]
-    lst = [l for l in lst if os.path.isdir(os.path.join(directory, l))]
+        lst = [filename for filename in lst if re.match(rr, filename)]
+    lst = [filename for filename in lst if os.path.isdir(os.path.join(directory, filename))]
     return lst
 
 
-def oainfo(filename, verbose=1):
-    """ Print information about a file containing arrays """
+def oainfo(filename: str, verbose: int = 1):
+    """Print information about a file containing arrays"""
     af = oapackage.arrayfile_t(filename, verbose)
     print(af.showstr())
     af.closefile()
 
 
 def oaIsBinary(filename: str) -> bool:
-    """ Return true if array file is in binary format """
+    """Return true if array file is in binary format"""
     af = oapackage.arrayfile_t(filename)
     ret = af.isbinary()
     af.closefile()
     return ret
 
 
-def fac(n):
-    """ Return n! (factorial)
+def fac(n: int) -> int:
+    """Return n! (factorial)
 
     Args:
         n (int): number to calculate factorial
     Returns
         integer: factorial of number
     """
     if n == 1 or n == 0:
         return 1
     else:
         return n * fac(n - 1)
 
 
 def choose(n: int, k: int) -> int:
-    """ Return n choose k """
+    """Return n choose k"""
     ntok = 1
     for t in range(min(k, n - k)):
         ntok = ntok * (n - t) // (t + 1)
     return ntok
 
 
-def array2latex(X, header=1, hlines=(), floatfmt='%g', comment=None, hlinespace=None, mode='tabular', tabchar='c'):
-    """ Convert numpy array to Latex tabular """
-    ss = ''
+def array2latex(X, header=1, hlines=(), floatfmt="%g", comment=None, hlinespace=None, mode="tabular", tabchar="c"):
+    """Convert numpy array to Latex tabular"""
+    ss = ""
     if comment is not None:
         if isinstance(comment, list):
             for line in comment:
-                ss += '%% %s\n' % str(line)
+                ss += "%% %s\n" % str(line)
         else:
-            ss += '%% %s\n' % str(comment)
+            ss += "%% %s\n" % str(comment)
     if header:
-        if mode == 'tabular':
+        if mode == "tabular":
             if len(tabchar) == 1:
                 cc = tabchar * X.shape[1]
             else:
                 cc = tabchar + tabchar[-1] * (X.shape[1] - len(tabchar))
-            ss += '\\begin{tabular}{%s}' % cc + chr(10)
-        elif mode == 'psmallmatrix':
-            ss += '\\begin{psmallmatrix}' + chr(10)
+            ss += "\\begin{tabular}{%s}" % cc + chr(10)
+        elif mode == "psmallmatrix":
+            ss += "\\begin{psmallmatrix}" + chr(10)
         else:
-            ss += '\\begin{pmatrix}' + chr(10)
+            ss += "\\begin{pmatrix}" + chr(10)
     for ii in range(X.shape[0]):
         r = X[ii, :]
         if isinstance(r[0], str):
-            ss += ' & '.join(['%s' % x for x in r])
+            ss += " & ".join(["%s" % x for x in r])
         else:
-            ss += ' & '.join([floatfmt % x for x in r])
+            ss += " & ".join([floatfmt % x for x in r])
         if ii < (X.shape[0]) - 1 or not header:
-            ss += '  \\\\' + chr(10)
+            ss += "  \\\\" + chr(10)
         else:
-            ss += '  ' + chr(10)
+            ss += "  " + chr(10)
         if ii in hlines:
-            ss += r'\hline' + chr(10)
+            ss += r"\hline" + chr(10)
             if hlinespace is not None:
-                ss += '\\rule[+%.2fex]{0pt}{0pt}' % hlinespace
+                ss += "\\rule[+%.2fex]{0pt}{0pt}" % hlinespace
     if header:
-        if mode == 'tabular':
-            ss += '\\end{tabular}'
-        elif mode == 'psmallmatrix':
-            ss += '\\end{psmallmatrix}' + chr(10)
+        if mode == "tabular":
+            ss += "\\end{tabular}"
+        elif mode == "psmallmatrix":
+            ss += "\\end{psmallmatrix}" + chr(10)
         else:
-            ss += '\\end{pmatrix}' + chr(10)
+            ss += "\\end{pmatrix}" + chr(10)
     return ss
 
 
-def array2html(X, header=1, tablestyle='border-collapse: collapse;', trclass='', tdstyle='', trstyle='', thstyle=''):
-    """ Convert Numpy array to HTML table
+def array2html(X, header=1, tablestyle="border-collapse: collapse;", trclass="", tdstyle="", trstyle="", thstyle=""):
+    """Convert Numpy array to HTML table
 
     Arguments
     ---------
         X : numpy array
             array to be converted
         header : integer
             use header or not
     Returns
     -------
         page : markup html object
             generated table in HTML
 
     """
     page = markup.page()
-    page.add('<!-- Created by array2html -->\n')
+    page.add("<!-- Created by array2html -->\n")
     page.table(style=tablestyle)
     offset = 0
     nc = X.shape[1]
     nr = X.shape[0]
 
     if isinstance(trstyle, str):
         trstyle = [trstyle] * nr
     if isinstance(trclass, str):
         trclass = [trclass] * nr
 
     ri = 0
     if header:
-        page.tr(style='font-weight: bold; border-bottom: solid 1px black;' +
-                trstyle[ri], class_=trclass[ri])
+        page.tr(style="font-weight: bold; border-bottom: solid 1px black;" + trstyle[ri], class_=trclass[ri])
         ri = ri + 1
         for ii in range(nc):
             if isinstance(X[offset, ii], tuple):
-                print('array2html: tuple instance')
+                print("array2html: tuple instance")
                 page.th(X[offset, ii][0], style=thstyle + X[offset, ii][1])
             else:
                 page.th(X[offset, ii], style=thstyle)
         page.tr.close()
         offset = offset + 1
 
     nr = X.shape[0] - offset
@@ -564,111 +573,116 @@
         offset = offset + 1
         ri = ri + 1
     page.table.close()
     return page
 
 
 def write_text_arrayfile(filename: str, designs: List[Any], comment: Optional[str] = None):
-    """ Write designs to disk in text format """
+    """Write designs to disk in text format"""
     nrows = designs[0].n_rows
     ncols = designs[0].n_columns
     afile = oapackage.oalib.arrayfile_t(filename, nrows, ncols, len(designs), oapackage.oalib.ATEXT, 8)
     if comment is not None:
-        for c in comment.split('\n'):
+        for c in comment.split("\n"):
             afile.add_comment(c)
     afile.append_arrays(designs)
     afile.closefile()
 
 
-def arrayfile_generator(afile):
-    """ Return generator to read all files in the array file """
+def arrayfile_generator(afile: str):
+    """Return generator to read all files in the array file"""
     af = oapackage.arrayfile_t(afile)
 
     na = af.narrays
     for ii in range(na):
         yield af.readnext()
     af.closefile()
 
 
-def runcommand(cmd: str, dryrun=0, idstr: Optional[None] = None, verbose: int = 1, logfile: Optional[str] = None, shell: bool = True):
-    """ Run specified command in external environment
+def runcommand(
+    cmd: str,
+    dryrun=0,
+    idstr: Optional[None] = None,
+    verbose: int = 1,
+    logfile: Optional[str] = None,
+    shell: bool = True,
+):
+    """Run specified command in external environment
 
     Args:
         cmd: Command to execute
 
     Returns:
         r (int): return value of the shell command
     """
     if idstr is not None:
         cmd = 'echo "idstr: %s";\n' % idstr + cmd
     if verbose >= 2:
-        print('cmd: %s' % cmd)
+        print("cmd: %s" % cmd)
     r: Optional[int] = 0
     if not dryrun:
-
-        process = subprocess.Popen(
-            cmd, bufsize=1, stdout=subprocess.PIPE, shell=shell)
+        process = subprocess.Popen(cmd, bufsize=1, stdout=subprocess.PIPE, shell=shell)
         for jj in range(10000000):
             r = process.poll()
             assert process.stdout is not None
             line_bytes = process.stdout.readline()
-            line = line_bytes.decode(encoding='UTF-8')
+            line = line_bytes.decode(encoding="UTF-8")
             if verbose >= 2:
-                print('runcommand: jj %d' % jj)
+                print("runcommand: jj %d" % jj)
             if verbose >= 3:
                 print('runcommand: jj %d: "%s"' % (jj, line))
             if len(line) == 0:
                 if verbose >= 2:
-                    print('runcommand: len(line) %d' % len(line))
+                    print("runcommand: len(line) %d" % len(line))
 
                 break
 
             if r is not None:
                 break
             if jj > 20000000:
-                print('error: early abort of runcommand')
+                print("error: early abort of runcommand")
                 break
             sys.stdout.write(str(line))
             if jj % 2 == 0:
                 sys.stdout.flush()
             if verbose >= 2:
-                print('end of loop...')
+                print("end of loop...")
         r = process.poll()
-        if (not r == 0):
-            print('runcommand: cmd returned error! r=%s' % str(r))
+        if not r == 0:
+            print("runcommand: cmd returned error! r=%s" % str(r))
             print(cmd)
             return r
     else:
         if verbose >= 2 or (verbose and logfile is None):
-            print(f'### dryrun of {idstr}\n{cmd}\n###\n')
+            print(f"### dryrun of {idstr}\n{cmd}\n###\n")
     if logfile is not None:
-        fid = open(logfile, 'a')
-        fid.write('\n###\n')
+        fid = open(logfile, "a")
+        fid.write("\n###\n")
         fid.write(cmd)
         fid.close()
     else:
         pass
 
     return r
 
 
 def getArrayFile(afile: str) -> str:
-    """ Return pointer to array file
+    """Return pointer to array file
     Automatically check for compressed array files
     """
-    afilegz = afile = afile + '.gz'
+    afilegz = afile = afile + ".gz"
     if not os.path.exists(afile) and os.path.exists(afilegz):
         afile = afilegz
     else:
         afile = afile
     return afile
 
 
 def checkOAfile(afile, verbose=0):
-    """ Return pointer to array file
+    """Return pointer to array file
 
     Automatically check for compressed array files
 
     Args:
         afile (str): location of array file
     Returns:
         arrayfile_t or None
@@ -678,149 +692,145 @@
     if af.isopen():
         return nm
     else:
         return None
 
 
 def checkArrayFile(afile, cache=1):
-    """ Check whether a file or list of files exists
-        If the file does not exist, check whether a compressed file does exist
-        cache: 0 (no), 1 (check), -1 (always)
+    """Check whether a file or list of files exists
+    If the file does not exist, check whether a compressed file does exist
+    cache: 0 (no), 1 (check), -1 (always)
     """
     if cache == -1:
         return True
     if cache == 0:
         return False
 
     if os.path.exists(afile):
         return True
     else:
-        if afile.endswith('.oa'):
-            if os.path.exists(afile + '.gz'):
+        if afile.endswith(".oa"):
+            if os.path.exists(afile + ".gz"):
                 return True
             else:
                 return False
         else:
             return False
 
 
 def isstr(s: Any) -> bool:
     return isinstance(s, str)
 
 
 def checkFiles(lst, cache=1, verbose=0):
-    """ Check whether a file or list of files exists
-        cache: 0 (no), 1 (check), -1 (always)
+    """Check whether a file or list of files exists
+    cache: 0 (no), 1 (check), -1 (always)
 
-        Returns False if one or more of the files do not exist
-        Returns True if all files exist
+    Returns False if one or more of the files do not exist
+    Returns True if all files exist
     """
     if cache == -1:
         return True
     if cache == 0:
         return False
 
     if isstr(lst):
         lst = [lst]
     c = True
     for f in lst:
         if not os.path.exists(f):
             if verbose:
-                print('checkFiles: file %s does not exist' % f)
+                print("checkFiles: file %s does not exist" % f)
             c = False
             break
     return c
 
 
 def test_checkFiles():
     def touch(fname):
         if os.path.exists(fname):
             os.utime(fname, None)
         else:
-            open(fname, 'a').close()
+            open(fname, "a").close()
 
     lst = [tempfile.mktemp()]
     r = checkFiles(lst, cache=1, verbose=1)
-    assert (r is False)
+    assert r is False
     touch(lst[0])
     r = checkFiles(lst, cache=1, verbose=1)
-    assert (r is True)
-
-# %%
-
+    assert r is True
 
 def checkFilesOA(lst, cache=1, verbose=0):
-    """ Check whether a file or list of files exists
+    """Check whether a file or list of files exists
+
+    Args:
+        lst (list): list of files
+        cache (int): 0 (always return False), 1 (check), -1 (always return True)
 
-        Args:
-            lst (list): list of files
-            cache (int): 0 (always return False), 1 (check), -1 (always return True)
-
-        For array files also the .gz extension is checked
-        Returns False if one or more of the files do not exist
-        Returns True if all files exist
+    For array files also the .gz extension is checked
+    Returns False if one or more of the files do not exist
+    Returns True if all files exist
     """
     if verbose >= 2:
-        print('checkFilesOA: cache %s' % (cache, ))
+        print(f"checkFilesOA: cache {cache}")
     if cache == -1:
         return True
     if cache == 0:
         return False
 
     if isstr(lst):
         lst = [lst]
     c = True
     for f in lst:
         r = checkArrayFile(f, cache=True)
         if not r:
             if verbose:
-                print('checkFiles: file %s does not exist' % f)
+                print("checkFiles: file %s does not exist" % f)
             c = False
             break
     return c
 
-# %%
 
 
 def randomizearrayfile(input_filename, output_filename, verbose=1):
-    """ Randomize a file with orthogonal arrays
+    """Randomize a file with orthogonal arrays
 
     Each array is transformed with a random transformation
 
     Args:
         afile (str): input file
         afileout (str): output file
     """
     lst = oapackage.readarrayfile(input_filename)
     rlst = oapackage.oalib.arraylist_t()
     for ii, al in enumerate(lst):
         adata = oalib.arraylink2arraydata(al)
         trans = oalib.array_transformation_t(adata)
         if verbose >= 2:
-            print('randomizing array %d\n' % ii)
+            print("randomizing array %d\n" % ii)
         trans.randomize()
         alr = trans.apply(al)
         rlst.push_back(alr)
     oapackage.writearrayfile(output_filename, rlst)
 
 
 def nArrayFile(filename, verbose=1):
-    """ Return number of arrays in file
+    """Return number of arrays in file
 
     Args:
         afile (str): name of array file
     """
     af = oalib.arrayfile_t(filename, 0)
     n = af.narrays
     af.closefile()
     return n
 
 
 def selectArraysInFile(infile, outfile, idx, afmode=oalib.ATEXT, verbose=1, cache=1):
-    """ Select arrays in a file by indices
+    """Select arrays in a file by indices
 
     Args:
         infile (str): file with designs
         outfile (str): output  file with designs
         inx (list of indices)
     Returns:
         None
@@ -829,35 +839,34 @@
     if not checkFiles(outfile, cache=cache):
         gidxint = oalib.intVector([int(x) for x in idx])
         sols = oalib.arraylist_t()
         oalib.selectArrays(infile, gidxint, sols, 0)
         af = oalib.arrayfile_t(infile, 1)
         _ = oalib.writearrayfile(outfile, sols, afmode, af.nrows, af.ncols)
         if verbose >= 2:
-            print('selectArrays: write array file %s in mode %d' %
-                  (outfile, afmode))
+            print("selectArrays: write array file %s in mode %d" % (outfile, afmode))
     else:
         if verbose >= 2:
-            print('output file %s already exists' % outfile)
+            print("output file %s already exists" % outfile)
 
 
 selectArrays = deprecated(selectArraysInFile)
 
 
 def floatformat(number, mind=2, maxd=4):
-    """ Format a floating point number into a string """
+    """Format a floating point number into a string"""
     rounded = int(number * (10**mind)) / float(10**mind)
     if number == rounded:
-        return ('%%.0%df' % mind) % number
+        return ("%%.0%df" % mind) % number
     else:
-        return ('%%.0%dg' % maxd) % number
+        return ("%%.0%dg" % maxd) % number
 
 
 def safemin(data, default=0):
-    """ Return mininum of array with default value for empty array
+    """Return mininum of array with default value for empty array
 
     Args:
         data (array or list): data to return the maximum
         default (obj): default value
     Returns:
         object: minimum value in the array or the default value
 
@@ -872,15 +881,15 @@
         minimum_value = default
     else:
         minimum_value = data.min()
     return minimum_value
 
 
 def safemax(data, default=0):
-    """ Return maximum of array with default value for empty array
+    """Return maximum of array with default value for empty array
 
     Args:
         data (array or list ): data to return the maximum
         default (obj): default value
     Returns:
         object: maximum value in the array or the default value
     """
@@ -895,66 +904,65 @@
         maximum_value = default
     else:
         maximum_value = data.max()
     return maximum_value
 
 
 def mkdirc(directory_name: str) -> str:
-    """ Create directory """
+    """Create directory"""
     if not os.path.exists(directory_name):
         os.mkdir(directory_name)
     return directory_name
 
 
 def parseProcessingTime(logfile, verbose=0):
-    """ Parse a log file to calculate the processing time """
+    """Parse a log file to calculate the processing time"""
 
     fileinput.close()
     tstart = None
     tend = None
     dtr = None
     try:
         for line in fileinput.input([logfile]):
-            if line.startswith('#time'):
+            if line.startswith("#time"):
                 if verbose >= 1:
-                    print('parseProcessingTime: line: %s' % line, end="")
-            if line.startswith('#time start:'):
+                    print("parseProcessingTime: line: %s" % line, end="")
+            if line.startswith("#time start:"):
                 tstart = dateutil.parser.parse(line[13:])
                 if verbose >= 2:
-                    print('parseProcessingTime: tstart: %s' % tstart)
-            elif line.startswith('#time end:'):
+                    print("parseProcessingTime: tstart: %s" % tstart)
+            elif line.startswith("#time end:"):
                 tend = dateutil.parser.parse(line[10:])
                 if verbose >= 2:
-                    print('parseProcessingTime: tend: %s' % tend)
-            elif line.startswith('#time total:'):
-                dtr = (line[13:])
+                    print("parseProcessingTime: tend: %s" % tend)
+            elif line.startswith("#time total:"):
+                dtr = line[13:]
                 dtr = float(dtr[:-5])
                 if verbose >= 2:
-                    print('parseProcessingTime: total: %s' % dtr)
+                    print("parseProcessingTime: total: %s" % dtr)
             else:
                 pass
         if tstart is not None and tend is not None:
             dt = tend - tstart
             dtt = dt.total_seconds()
         else:
             dtt = -1
     except BaseException:
         if verbose:
-            print('error processing log %s' % logfile)
+            print("error processing log %s" % logfile)
             traceback.print_exc(file=sys.stdout)
         dtt = -1
     if dtr is not None:
         if abs(dtr - dtt) > 10:
-            print(
-                'parseProcessingTime: warning difference in reported times %.1f dtr %.1f [s]' % (dtt, dtr))
+            print(f"parseProcessingTime: warning difference in reported times {dtt:.1f} dtr {dtr:.1f} [s]")
     return dtt
 
 
 def series2htmlstr(ad, html=1, case=0):
-    """ Convert arraydata_t to html formatted string """
+    """Convert arraydata_t to html formatted string"""
     s = list(ad.factor_levels())
     p = -1
     n = 0
     levels = []
     bb = []
     while n < len(s):
         if s[n] != p:
@@ -962,51 +970,51 @@
             levels.append(p)
             bb.append(1)
         else:
             bb[-1] += 1
         n = n + 1
     if case == 0:
         if bb[-1] > 1:
-            bb[-1] = 'a'
-    hstr = 'OA(%d; %d; ' % (ad.N, ad.strength)
+            bb[-1] = "a"
+    hstr = "OA(%d; %d; " % (ad.N, ad.strength)
     for ii, _ in enumerate(levels):
         if html:
-            hstr += '%d<sup>%s</sup>' % (levels[ii], str(bb[ii]))
+            hstr += "%d<sup>%s</sup>" % (levels[ii], str(bb[ii]))
         else:
-            hstr += '%d^%s' % (levels[ii], str(bb[ii]))
-    hstr += ')'
+            hstr += "%d^%s" % (levels[ii], str(bb[ii]))
+    hstr += ")"
     return hstr
 
 
-def gwlp2str(gmadata, t=None, sformat=None, jstr=','):
-    """ Convert GWLP value to string format """
+def gwlp2str(gmadata, t=None, sformat=None, jstr=","):
+    """Convert GWLP value to string format"""
     if gmadata is None:
-        return '-'
+        return "-"
     if isinstance(gmadata, tuple):
         pass
     else:
         if isinstance(gmadata, list):
             pass
         else:
             gmadata[gmadata < 0] = 0
         if not (np.abs(gmadata[0] - 1) < 1e-12 and np.abs(gmadata[1]) < 1e-12):
-            warnings.warn('data does not represent GWPL data', UserWarning)
-            return ''
+            warnings.warn("data does not represent GWPL data", UserWarning)
+            return ""
     bgma = np.around(gmadata, decimals=12)
     if t is not None:
-        bgma = bgma[(t + 1):]
+        bgma = bgma[(t + 1) :]
     if sformat is None:
         gstr = jstr.join([floatformat(v, mind=2, maxd=4) for v in bgma])
     else:
         gstr = jstr.join([sformat % v for v in bgma])
     return gstr
 
 
 def selectJ(sols0, jj=5, jresults=None, verbose=1):
-    """ Select only arrays with J-characteristics non-zero
+    """Select only arrays with J-characteristics non-zero
 
     We asssume the designs are in even-odd ordering (i.e. only check the J value of first columns)
     """
     if jresults is None:
         jresults = oalib.analyseArrays(sols0, verbose, jj)
 
     solseo = oalib.arraylist_t()
@@ -1015,41 +1023,41 @@
         v.append(js.values[0])
 
     si = [i for (i, j) in sorted(enumerate(v), key=operator.itemgetter(1))]
     for jj in si:
         if v[jj] > 0:
             solseo.append(sols0[jj])
     if verbose:
-        print('selectJ: kept %d/%d solutions' % (solseo.size(), len(sols0)))
+        print("selectJ: kept %d/%d solutions" % (solseo.size(), len(sols0)))
     return solseo
 
 
 def test_selectJ():
     al = oapackage.exampleArray(12, 1)
     sols0 = [al]
     r = selectJ(sols0)
-    assert (len(r) == 0)
+    assert len(r) == 0
 
 
 def extendSingleArray(A, adata, t=3, verbose=1):
-    """ Extend a single orthogonal array """
+    """Extend a single orthogonal array"""
     oaoptions = oalib.OAextend()
     oaoptions.setAlgorithmAuto(adata)
     sols0 = oalib.arraylist_t()
     solsx = oalib.arraylist_t()
     sols0.push_back(A)
     k = A.n_columns
     n = oalib.extend_arraylist(sols0, adata, oaoptions, k, solsx)
-    assert (n >= len(solsx))
+    assert n >= len(solsx)
     sys.stdout.flush()
     return solsx
 
 
-def runExtend(N, k, t=3, l=2, verbose=1, initsols=None, nums=[], algorithm=None):
-    """ Run extension algorithm and return arrays
+def runExtend(N: int, k: int, t: int = 3, l: int = 2, verbose: int = 1, initsols=None, nums=[], algorithm=None):  # noqa
+    """Run extension algorithm and return arrays
 
     Args:
       N (int): number of rows
       k (int): number of columns to extend to
       t (int): strength of the arrays
       l (int): factors of the designs
       initsols (None or list): list of arrays to extend, None to start with root
@@ -1058,15 +1066,15 @@
         list: list of generated designs
 
     Example:
        >>> import oapackage
        >>> designs = oapackage.oahelper.runExtend(16, 5, 3, verbose=0)
     """
     if verbose:
-        print('runExtend: N=%d, k=%d, t=%d' % (N, k, t))
+        print("runExtend: N=%d, k=%d, t=%d" % (N, k, t))
     if isinstance(l, list):
         ll = l
     else:
         ll = [l]
     ll = ll + [ll[-1]] * (k - len(ll))
     s = oalib.intVector(ll)
     adata = oalib.arraydata_t(s, N, t, k)
@@ -1086,133 +1094,131 @@
     else:
         oaoptions.setAlgorithm(algorithm, adata)
     solsx = sols0
     for ii in range(tstart, k):
         solsx = oalib.arraylist_t()
         oalib.extend_arraylist(sols0, adata, oaoptions, ii, solsx)
         if verbose >= 2:
-            print(' ii %d: %d' % (ii, solsx.size()))
+            print(" ii %d: %d" % (ii, solsx.size()))
         sols0 = solsx
         nums.append(solsx.size())
         sys.stdout.flush()
     return solsx
 
 
 def compressOAfile(afile, decompress=False, verbose=1):
-    """ Compress an OA array file
+    """Compress an OA array file
 
     Args:
         afile (str): array to compress
         decompress (bool): If True then decompress
         verbose (int): verbosity level
     """
     af = oalib.arrayfile_t(afile, 0)
     if decompress:
-        raise NotImplementedError('decompressing file not implemted')
+        raise NotImplementedError("decompressing file not implemted")
 
     if verbose >= 2:
-        print('file %s: binary %s' % (afile, af.isbinary()))
-    if not (sys.platform == 'linux2' or sys.platform == 'linux'):
+        print(f"file {afile}: binary {af.isbinary()}")
+    if not (sys.platform == "linux2" or sys.platform == "linux"):
         if verbose:
-            print('compressOAfile: not compressing file %s (platform not supported)' %
-                  afile)
+            print("compressOAfile: not compressing file %s (platform not supported)" % afile)
         return False
-    if af.isbinary() and not af.iscompressed and sys.platform == 'linux2':
+    if af.isbinary() and not af.iscompressed and sys.platform == "linux2":
         if verbose:
-            print('compressOAfile: compressing file %s' % afile)
-        cmd = 'gzip -f %s' % afile
+            print("compressOAfile: compressing file %s" % afile)
+        cmd = "gzip -f %s" % afile
         r = os.system(cmd)
         if not r == 0:
-            print('compressOAfile: error compressing file %s' % afile)
+            print("compressOAfile: error compressing file %s" % afile)
         return True
     else:
         if not af.isbinary():
             if verbose:
-                print('compressOAfile: not compressing file %s (file is in text mode)' %
-                      afile)
+                print("compressOAfile: not compressing file %s (file is in text mode)" % afile)
         else:
             if verbose:
-                print('compressOAfile: not compressing file %s (file %s is compressed)' %
-                      (afile, af.filename))
+                print(f"compressOAfile: not compressing file {afile} (file {af.filename} is compressed)")
         return False
 
 
 def argsort(seq):
-    """ Stable version of argsort """
+    """Stable version of argsort"""
     # http://stackoverflow.com/questions/3382352/equivalent-of-numpy-argsort-in-basic-python/3382369#3382369
     return sorted(range(len(seq)), key=seq.__getitem__)
 
 
 @deprecated
 def jseq(xx, comb):
     pp = functools.reduce(lambda y, i: xx[:, i] + y, comb, 0)
     jseq = 1 - 2 * np.mod(pp, 2)
     return jseq
 
 
 def sortrows(x):
-    """ Sort rows of an array, return indices
+    """Sort rows of an array, return indices
 
     The array is sorted low to high with the first column as the major column.
 
     Args:
         array (numpy array)
     Returns:
         list: indices of rows of sorted array
     """
     if len(x.shape) == 1:
         nn = 1
         sind = np.argsort(x)
         return sind
     else:
         nn = x.shape[1]
-    dt = [('x%d' % xx, 'f8') for xx in range(0, nn)]
+    dt = [("x%d" % xx, "f8") for xx in range(0, nn)]
     if x.size == 0:
         sind = np.array([])
         return sind
     v = [tuple(x[kk, :]) for kk in range(0, x.shape[0])]
     w = np.array(v, dtype=dt)
     sind = np.argsort(w)
     return sind
 
 
 def sortcols(array):
-    """ Sort columns of an array, return indices
+    """Sort columns of an array, return indices
 
     The array is sorted low to high with the row column as the major row.
 
     Args:
         array (numpy array)
     Returns:
         list: indices of columns of sorted array
     """
     sind = sortrows(array.transpose())
     return sind
 
+
 # %%
 
 
 def testHtml(html_code=None):
-    """ Test a short snippet of HTML """
+    """Test a short snippet of HTML"""
     if html_code is None:
         return
     page = markup.page()
     page.init()
     page.body()
     page.add(html_code)
     page.body.close()
-    _, f = tempfile.mkstemp('.html')
-    with open(f, 'w') as fname:
+    _, f = tempfile.mkstemp(".html")
+    with open(f, "w") as fname:
         fname.write(str(page))
         fname.close()
         webbrowser.open(fname.name)
 
 
 def designStandardError(al) -> Tuple[float, float, float]:
-    """ Return standard errors for a design
+    """Return standard errors for a design
 
     Args:
       al (array): design
 
     Returns:
         array: array with standard errors
 
@@ -1222,134 +1228,138 @@
     k = al.n_columns
 
     scalefac = 1
     M = np.linalg.inv(X.transpose().dot(X) / scalefac)
 
     mm = np.array(M.diagonal()).flatten()
 
-    m1 = mm[1:(1 + k)].flatten()
+    m1 = mm[1 : (1 + k)].flatten()
     m1 = m1[np.argsort(m1)]
-    m2 = mm[(1 + k):]
+    m2 = mm[(1 + k) :]
     m2 = m2[np.argsort(m2)]
     m0 = mm[0]
     return np.sqrt(m0), np.sqrt(m1), np.sqrt(m2)
 
 
 # %%
-def DefficiencyBound(D, k, k2):
-    """ Calculate the D-efficiency bound of an array extension
+def DefficiencyBound(D: float, k: int, k2: int) -> float:
+    """Calculate the D-efficiency bound of an array extension
 
     Args:
-        D (float): D-efficiency of the design
-        k (int): numbers of columns
-        k2 (int): numbers of columns
+        D: D-efficiency of the design
+        k: numbers of columns
+        k2: numbers of columns in extension
 
     Returns:
-        float: bound on the D-efficiency of extensions of a design with k columns to k2 columns
+        Bound on the D-efficiency of extensions of a design with k columns to k2 columns
 
     """
-    m = 1. + k + k * (k - 1) / 2
-    m2 = 1. + k2 + k2 * (k2 - 1) / 2
-    Dbound = D**(m / m2)
+    m = 1.0 + k + k * (k - 1) / 2
+    m2 = 1.0 + k2 + k2 * (k2 - 1) / 2
+    Dbound = D ** (m / m2)
     return Dbound
 
+
 # %% Misc
 
 
 def setWindowRectangle(x, y=None, w=None, h=None, mngr=None, be=None):
-    """ Position the current Matplotlib figure at the specified position
-
-    """
+    """Position the current Matplotlib figure at the specified position"""
     if y is None:
         y = x[1]
         w = x[2]
         h = x[3]
         x = x[0]
     if mngr is None:
         mngr = plt.get_current_fig_manager()
     be = matplotlib.get_backend()
-    if be == 'WXAgg':
+    if be == "WXAgg":
         mngr.canvas.manager.window.SetPosition((x, y))
         mngr.canvas.manager.window.SetSize((w, h))
-    elif be == 'agg':
+    elif be == "agg":
         mngr.canvas.manager.window.SetPosition((x, y))
         mngr.canvas.manager.window.resize(w, h)
-    elif be == 'module://IPython.kernel.zmq.pylab.backend_inline':
+    elif be == "module://IPython.kernel.zmq.pylab.backend_inline":
         pass
     else:
         # assume Qt canvas
         mngr.canvas.manager.window.move(x, y)
         mngr.canvas.manager.window.resize(w, h)
         mngr.canvas.manager.window.setGeometry(x, y, w, h)
 
 
 def makearraylink(array):
-    """ Convert array to array_link object
+    """Convert array to array_link object
 
     Args:
         array (numpy array or array_link): array to convert
     Returns:
         array_link
     """
     if isinstance(array, np.ndarray):
         array = oapackage.create_array_link(array)
     return array
 
 
 def formatC(al, wrap: bool = True) -> str:
-    """ Format array for inclusion in C code
+    """Format array for inclusion in C code
 
     Args:
         array: Array to be converted to C code representation
         wrap: If True, then add code to create a variable
     Returns:
         Formatted string
     """
-    l = np.array(al).T.flatten().tolist()
-    s = ','.join(['%d' % x for x in l])
+    A = np.array(al).T.flatten().tolist()
+    s = ",".join(["%d" % x for x in A])
     if wrap:
-        s = '\tarray_link array ( %d,%d, 0 );\n\tint array_data_tmp[] = {' % (
-            al.n_rows, al.n_columns) + s + '};'
-        s += '\tarray.setarraydata(array_data_tmp, array.n_rows * array.n_columns);\n'
+        s = "\tarray_link array ( %d,%d, 0 );\n\tint array_data_tmp[] = {" % (al.n_rows, al.n_columns) + s + "};"
+        s += "\tarray.setarraydata(array_data_tmp, array.n_rows * array.n_columns);\n"
     return s
 
 
 def create_pareto_element(values, pareto=None):
-    """ Create a vector of mvalue_t elements
+    """Create a vector of mvalue_t elements
     Args:
         vv (list): list with tuples or arrays
     Returns:
         object: Pareto element
     """
     if pareto is None:
         pareto = oalib.ParetoDoubleLong()
     if isinstance(pareto, oalib.ParetoMultiLongLong):
         vector_pareto = oalib.mvalueVector()
         for v in values:
             if isinstance(v, (int)):
                 # convert to list type
                 v = [v]
             if not isinstance(v, (list, type)):
-                raise Exception('creating Pareto element for Pareto object of type %s and input of type %s not supported' % (
-                    type(pareto), type(v)))
+                raise Exception(
+                    "creating Pareto element for Pareto object of type %s and input of type %s not supported"
+                    % (type(pareto), type(v))
+                )
             vec = oalib.mvalue_t_long(list(v))
             vector_pareto.push_back(vec)
     elif isinstance(pareto, oalib.ParetoMultiDoubleLong):
         vector_pareto = oalib.vector_mvalue_t_double()
         for v in values:
             if isinstance(v, (int, float)):
                 # convert to list type
                 v = [float(v)]
             if not isinstance(v, (list, tuple)):
-                raise Exception('creating Pareto element for Pareto object of type %s and input of type %s not supported' % (
-                    type(pareto), type(v)))
+                raise Exception(
+                    "creating Pareto element for Pareto object of type %s and input of type %s not supported"
+                    % (type(pareto), type(v))
+                )
 
             vec = oalib.mvalue_t_double(list(v))
             vector_pareto.push_back(vec)
     elif isinstance(pareto, oalib.ParetoDoubleLong):
         if not isinstance(values, (list, tuple, np.ndarray)):
-            raise Exception('cannot handle input of type %s' % (tuple(values), ))
+            raise Exception(f"cannot handle input of type {tuple(values)}")
         vector_pareto = values
     else:
-        raise Exception('creating Pareto element for Pareto object of type %s and input of type %s not supported' % (
-            type(pareto), type(values)))
+        raise Exception(
+            "creating Pareto element for Pareto object of type %s and input of type %s not supported"
+            % (type(pareto), type(values))
+        )
     return vector_pareto
```

### Comparing `OApackage-2.7.6/src/Deff.cpp` & `OApackage-2.7.7/src/Deff.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Deff.h` & `OApackage-2.7.7/src/Deff.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/CMakeLists.txt` & `OApackage-2.7.7/src/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Cholesky` & `OApackage-2.7.7/src/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/CholmodSupport` & `OApackage-2.7.7/src/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Core` & `OApackage-2.7.7/src/Eigen/Core`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Eigenvalues` & `OApackage-2.7.7/src/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Geometry` & `OApackage-2.7.7/src/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Householder` & `OApackage-2.7.7/src/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/IterativeLinearSolvers` & `OApackage-2.7.7/src/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Jacobi` & `OApackage-2.7.7/src/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/LU` & `OApackage-2.7.7/src/Eigen/LU`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/MetisSupport` & `OApackage-2.7.7/src/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/OrderingMethods` & `OApackage-2.7.7/src/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/PaStiXSupport` & `OApackage-2.7.7/src/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/PardisoSupport` & `OApackage-2.7.7/src/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/QR` & `OApackage-2.7.7/src/Eigen/QR`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/QtAlignedMalloc` & `OApackage-2.7.7/src/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SPQRSupport` & `OApackage-2.7.7/src/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SVD` & `OApackage-2.7.7/src/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/Sparse` & `OApackage-2.7.7/src/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SparseCholesky` & `OApackage-2.7.7/src/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SparseCore` & `OApackage-2.7.7/src/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SparseLU` & `OApackage-2.7.7/src/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SparseQR` & `OApackage-2.7.7/src/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/StdDeque` & `OApackage-2.7.7/src/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/StdList` & `OApackage-2.7.7/src/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/StdVector` & `OApackage-2.7.7/src/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/SuperLUSupport` & `OApackage-2.7.7/src/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/UmfPackSupport` & `OApackage-2.7.7/src/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Cholesky/LDLT.h` & `OApackage-2.7.7/src/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Cholesky/LLT.h` & `OApackage-2.7.7/src/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Cholesky/LLT_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/CholmodSupport/CholmodSupport.h` & `OApackage-2.7.7/src/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Array.h` & `OApackage-2.7.7/src/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ArrayBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ArrayWrapper.h` & `OApackage-2.7.7/src/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Assign.h` & `OApackage-2.7.7/src/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/AssignEvaluator.h` & `OApackage-2.7.7/src/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Assign_MKL.h` & `OApackage-2.7.7/src/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/BandMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Block.h` & `OApackage-2.7.7/src/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/BooleanRedux.h` & `OApackage-2.7.7/src/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CommaInitializer.h` & `OApackage-2.7.7/src/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ConditionEstimator.h` & `OApackage-2.7.7/src/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CoreEvaluators.h` & `OApackage-2.7.7/src/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CoreIterators.h` & `OApackage-2.7.7/src/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CwiseBinaryOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CwiseNullaryOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CwiseTernaryOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CwiseUnaryOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/CwiseUnaryView.h` & `OApackage-2.7.7/src/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/DenseBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/DenseCoeffsBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/DenseStorage.h` & `OApackage-2.7.7/src/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Diagonal.h` & `OApackage-2.7.7/src/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/DiagonalMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/DiagonalProduct.h` & `OApackage-2.7.7/src/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Dot.h` & `OApackage-2.7.7/src/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/EigenBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ForceAlignedAccess.h` & `OApackage-2.7.7/src/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Fuzzy.h` & `OApackage-2.7.7/src/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/GeneralProduct.h` & `OApackage-2.7.7/src/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/GenericPacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/GlobalFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/IO.h` & `OApackage-2.7.7/src/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Inverse.h` & `OApackage-2.7.7/src/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Map.h` & `OApackage-2.7.7/src/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/MapBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/MathFunctionsImpl.h` & `OApackage-2.7.7/src/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Matrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/MatrixBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/NestByValue.h` & `OApackage-2.7.7/src/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/NoAlias.h` & `OApackage-2.7.7/src/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/NumTraits.h` & `OApackage-2.7.7/src/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/PermutationMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/PlainObjectBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Product.h` & `OApackage-2.7.7/src/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ProductEvaluators.h` & `OApackage-2.7.7/src/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Random.h` & `OApackage-2.7.7/src/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Redux.h` & `OApackage-2.7.7/src/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Ref.h` & `OApackage-2.7.7/src/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Replicate.h` & `OApackage-2.7.7/src/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/ReturnByValue.h` & `OApackage-2.7.7/src/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Reverse.h` & `OApackage-2.7.7/src/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Select.h` & `OApackage-2.7.7/src/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/SelfAdjointView.h` & `OApackage-2.7.7/src/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/SelfCwiseBinaryOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Solve.h` & `OApackage-2.7.7/src/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/SolveTriangular.h` & `OApackage-2.7.7/src/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/SolverBase.h` & `OApackage-2.7.7/src/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/StableNorm.h` & `OApackage-2.7.7/src/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Stride.h` & `OApackage-2.7.7/src/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Swap.h` & `OApackage-2.7.7/src/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Transpose.h` & `OApackage-2.7.7/src/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Transpositions.h` & `OApackage-2.7.7/src/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/TriangularMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/VectorBlock.h` & `OApackage-2.7.7/src/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/VectorwiseOp.h` & `OApackage-2.7.7/src/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/Visitor.h` & `OApackage-2.7.7/src/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX/TypeCasting.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AVX512/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/Half.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/Default/ConjHelper.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/Default/Settings.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/NEON/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/SSE/TypeCasting.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/Complex.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/arch/ZVector/PacketMath.h` & `OApackage-2.7.7/src/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/AssignmentFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/BinaryFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/NullaryFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/StlFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/TernaryFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/functors/UnaryFunctors.h` & `OApackage-2.7.7/src/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixVector.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/Parallelizer.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointProduct.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/SelfadjointRank2Update.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixVector.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverMatrix.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/products/TriangularSolverVector.h` & `OApackage-2.7.7/src/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/BlasUtil.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/Constants.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/DisableStupidWarnings.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/ForwardDeclarations.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/MKL_support.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/Macros.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/Memory.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/Meta.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/ReenableStupidWarnings.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/StaticAssert.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Core/util/XprHelper.h` & `OApackage-2.7.7/src/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexSchur.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/EigenSolver.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealQZ.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealSchur.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Eigenvalues/Tridiagonalization.h` & `OApackage-2.7.7/src/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/AlignedBox.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/AngleAxis.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/EulerAngles.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Homogeneous.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Hyperplane.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/OrthoMethods.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/ParametrizedLine.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Quaternion.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Rotation2D.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/RotationBase.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Scaling.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Transform.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Translation.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/Umeyama.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Geometry/arch/Geometry_SSE.h` & `OApackage-2.7.7/src/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Householder/BlockHouseholder.h` & `OApackage-2.7.7/src/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Householder/Householder.h` & `OApackage-2.7.7/src/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Householder/HouseholderSequence.h` & `OApackage-2.7.7/src/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `OApackage-2.7.7/src/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/Jacobi/Jacobi.h` & `OApackage-2.7.7/src/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/Determinant.h` & `OApackage-2.7.7/src/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/FullPivLU.h` & `OApackage-2.7.7/src/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/InverseImpl.h` & `OApackage-2.7.7/src/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/PartialPivLU.h` & `OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/LU/arch/Inverse_SSE.h` & `OApackage-2.7.7/src/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/MetisSupport/MetisSupport.h` & `OApackage-2.7.7/src/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/OrderingMethods/Amd.h` & `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/OrderingMethods/Ordering.h` & `OApackage-2.7.7/src/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `OApackage-2.7.7/src/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/PardisoSupport/PardisoSupport.h` & `OApackage-2.7.7/src/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/ColPivHouseholderQR.h` & `OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `OApackage-2.7.7/src/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/FullPivHouseholderQR.h` & `OApackage-2.7.7/src/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/HouseholderQR.h` & `OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `OApackage-2.7.7/src/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SVD/BDCSVD.h` & `OApackage-2.7.7/src/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SVD/JacobiSVD.h` & `OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `OApackage-2.7.7/src/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SVD/SVDBase.h` & `OApackage-2.7.7/src/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SVD/UpperBidiagonalization.h` & `OApackage-2.7.7/src/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `OApackage-2.7.7/src/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/AmbiVector.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/CompressedStorage.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/MappedSparseMatrix.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseAssign.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseBlock.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseColEtree.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCompressedBase.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDenseProduct.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseDot.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseFuzzy.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMap.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMatrix.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseMatrixBase.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparsePermutation.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseProduct.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseRedux.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseRef.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSolverBase.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseTranspose.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseTriangularView.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseUtil.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseVector.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/SparseView.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseCore/TriangularSolver.h` & `OApackage-2.7.7/src/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLUImpl.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Memory.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Structs.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_Utils.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_pivotL.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_pruneL.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `OApackage-2.7.7/src/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SparseQR/SparseQR.h` & `OApackage-2.7.7/src/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/StlSupport/StdDeque.h` & `OApackage-2.7.7/src/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/StlSupport/StdList.h` & `OApackage-2.7.7/src/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/StlSupport/StdVector.h` & `OApackage-2.7.7/src/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/StlSupport/details.h` & `OApackage-2.7.7/src/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `OApackage-2.7.7/src/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `OApackage-2.7.7/src/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/Image.h` & `OApackage-2.7.7/src/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/Kernel.h` & `OApackage-2.7.7/src/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/RealSvd2x2.h` & `OApackage-2.7.7/src/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/blas.h` & `OApackage-2.7.7/src/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/lapack.h` & `OApackage-2.7.7/src/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/misc/lapacke.h` & `OApackage-2.7.7/src/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/BlockMethods.h` & `OApackage-2.7.7/src/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `OApackage-2.7.7/src/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/InfInt.h` & `OApackage-2.7.7/src/InfInt.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/anyoption.cpp` & `OApackage-2.7.7/src/anyoption.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/anyoption.h` & `OApackage-2.7.7/src/anyoption.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/arrayproperties.cpp` & `OApackage-2.7.7/src/arrayproperties.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1406,17 +1406,16 @@
         return dd;
 }
 
 // typedef Eigen::MatrixXd MyMatrix;
 typedef MatrixFloat EigenMatrixFloat;
 
 std::vector< double > Defficiencies (const array_link &array, const arraydata_t &arrayclass, int verbose, int addDs0) {
-        if ((array.n_rows > 500) || (array.n_columns > 500)) {
-                myprintf ("Defficiencies: array size not supported\n");
-                return std::vector< double > (3);
+        if ((array.n_rows > 50000) || (array.n_columns > 500)) {
+                throw_runtime_exception( printfstring("Defficiencies: array size %d x %d not supported\n", array.n_rows, array.n_columns));
         }
 
         int k = array.n_columns;
         int k1 = array.n_columns + 1;
         int nrows = array.n_rows;
         int m = 1 + k + k * (k - 1) / 2;
 
@@ -1550,36 +1549,14 @@
                                 myprintf ("  singular!\n");
                         S[j] = 0;
                 } else {
                         S[j] = sqrt (S[j]);
                 }
         }
 
-        if (verbose >= 2) {
-                JacobiSVD< DMatrix > svd (mymatrix);
-                const DVector S2 = svd.singularValues ();
-
-                if (!(S2[m - 1] < 1e-15)) {
-                        for (int ii = 0; ii < m - 3; ii++) {
-                                myprintf ("ii %d: singular values sqrt(SelfAdjointEigenSolver) SelfAdjointEigenSolver "
-                                          "svd %f %f %f\n",
-                                          ii, (double)S[m - ii - 1], (double)evs[m - ii - 1], (double)S2[ii]);
-                        }
-                        for (int ii = m - 3; ii < m - 1; ii++) {
-                                myprintf ("ii %d: %f %f %f\n", ii, (double)S[m - ii - 1], (double)evs[m - ii - 1],
-                                          (double)S2[ii]);
-                        }
-
-                        DMatrix Smat (S);
-                        DArray Sa = Smat.array ();
-                        Deff = exp (2 * Sa.log ().sum () / m) / N;
-                        myprintf ("  Aold: %.6f\n", Deff);
-                }
-        }
-
         if (S[0] < 1e-15) {
                 if (verbose >= 2)
                         myprintf ("Avalue: singular matrix\n");
                 Deff = 0;
                 return Deff;
         }
```

### Comparing `OApackage-2.7.6/src/arrayproperties.h` & `OApackage-2.7.7/src/arrayproperties.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/arraytools.cpp` & `OApackage-2.7.7/src/arraytools.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2780,15 +2780,15 @@
         if (this->n_rows < 1) {
                 myprintf ("Defficiencies: error: input array should have more than zero rows\n");
                 std::vector< double > x (3 + addDs0);
                 x[0] = NaN;
                 x[1] = NaN;
                 return x;
         }
-        arraydata_t arrayclass = arraylink2arraydata (al);
+        arraydata_t arrayclass = arraylink2arraydata (al, 0, 0);
 
         return ::Defficiencies (al, arrayclass, verbose, addDs0);
 }
 
 double array_link::Defficiency () const {
         if (!this->is2level ()) {
                 return this->Defficiencies ()[0];
@@ -4747,15 +4747,14 @@
 		arrayfile_t afout(output_filename.c_str(), nr, nc, narrays, output_format, nb);
 
 		if (input_array_file.narrays < 0) {
 			narrays = arrayfile_t::NARRAYS_MAX;
 			myprintf("untested code! (number of arrays undefined)\n");
 		}
 
-		int index;
 		for (long i = 0; i < narrays; i++) {
 			if ((i % 10000 == 0 && verbose) || (verbose >= 3)) {
 				log_print(QUIET, "oaconvert: loading arrays: %d/%d\n", i, input_array_file.narrays);
 			}
 
 			int g = input_array_file.read_array(al);
 			if (g < 0) {
@@ -4985,18 +4984,14 @@
         }
 #else
         this->iscompressed = 0;
         this->nfid = fopen (fname.c_str (), "r+b");
         this->gzfid = 0;
 #endif
 
-        if (verbose >= 2) {
-                myprintf (" nfid %ld, gzfid %ld, isopen %d \n", (long)nfid, (long)gzfid, this->isopen ());
-        }
-
         if (!this->isopen ()) {
                 if (verbose) {
                         myprintf ("problem opening file %s (iscompressed %d)\n", fname.c_str (), this->iscompressed);
                 }
                 this->closefile ();
                 return;
         }
@@ -5177,17 +5172,14 @@
 
 void arrayfile_t::updatenumbers () {
         if (narraycounter >= 0 && narrays == -1 && (this->rwmode == WRITE || this->rwmode == READWRITE) &&
             this->isbinary ()) {
                 if (verbose >= 2) {
                         myprintf ("arrayfile_t: updating numbers %d->%d\n", narrays, narraycounter);
                 }
-                if (verbose >= 3) {
-                        myprintf ("arrayfile_t: nfid %ld\n", long(nfid));
-                }
                 if (nfid != 0) {
                         long pos = ftell (nfid);
                         int r = fseek (nfid, 4 * sizeof (int32_t), SEEK_SET);
                         r = this->afwrite (&narraycounter, sizeof (int32_t), 1);
                         if (verbose >= 2) {
                                 myprintf ("   arrayfile_t::updatenumbers: result of write: %d\n", (int)r);
                         }
@@ -5197,19 +5189,14 @@
 }
 
 arrayfile_t::~arrayfile_t () {
 #ifdef SWIG
         swigcheck ();
 #endif
 
-        if (verbose >= 2) {
-                myprintf ("arrayfile_t: destructor: filename %s, nfid %ld, narraycounter %d, this->rwmode %d\n",
-                          filename.c_str (), (long)nfid, narraycounter, this->rwmode);
-        }
-
         closefile ();
 }
 
 
 void arrayfile_t::read_array_binary (array_t *array, const int nrows, const int ncols) {
         switch (this->nbits) {
         case 1: {
```

### Comparing `OApackage-2.7.6/src/arraytools.h` & `OApackage-2.7.7/src/arraytools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/bitarray/bit_array.cpp` & `OApackage-2.7.7/src/bitarray/bit_array.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/bitarray/bit_array.h` & `OApackage-2.7.7/src/bitarray/bit_array.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/bitarray/bit_array_test.cpp` & `OApackage-2.7.7/src/bitarray/bit_array_test.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/conference.cpp` & `OApackage-2.7.7/src/conference.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/conference.h` & `OApackage-2.7.7/src/conference.h`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 #include <stdio.h>
 #include <stdlib.h>
 
 #include "arrayproperties.h"
 #include "arraytools.h"
 #include "graphtools.h"
 
-
 /// print a candidate extension
 void print_column(const conference_column &column, const char *msg = 0);
 
 /** Show a list of candidate extensions
  *
  * \param column_candidates List of candidates to show
  */
```

### Comparing `OApackage-2.7.6/src/depth_extend.cpp` & `OApackage-2.7.7/src/depth_extend.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/depth_extend.h` & `OApackage-2.7.7/src/depth_extend.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/evenodd.cpp` & `OApackage-2.7.7/src/evenodd.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/evenodd.h` & `OApackage-2.7.7/src/evenodd.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/extend.cpp` & `OApackage-2.7.7/src/extend.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -645,15 +645,15 @@
                         break;
                 }
         }
 
         if (stack->count == 0) {
                 /* since all elements of the column are set the extend loop thinks it will return to a braching point,
                  * since there is no branching point set we make the last element -1 */
-                log_print (DEBUG, "init_column_previous: there is a unique extention to the array??\n");
+                log_print (DEBUG, "init_column_previous: there is a unique extention to the array\n");
                 log_print (DEBUG, "stack->count %d, p->row %d (N %d)\n", stack->count, p->row, p->ad->N);
                 array[col_offset + N - 1] = -1;
         }
 
         /* we set this for designs with strength 1 (here columns can be repeated) */
         array[col_offset + N - 1] = -1;
 }
@@ -735,17 +735,17 @@
 
         return more_branches;
 }
 
 inline void showLoopProgress (array_t *array, const int col_offset, const rowindex_t N, const int node_rank = 0,
                               int nlmcarrays = -1) {
 
-        static long nloops = 0;
+        static unsigned long long nloops = 0;
         nloops++;
-        if (nloops % 20000 == 0) {
+        if (nloops % 50 * 1000 == 0) {
                 fflush (stdout);
 
                 if (nloops % (500 * 1000 * 1000) == 0) {
                     if (checkloglevel(QUIET)) {
                         std::cout << "node [" << node_rank << "]: extend loop " << nloops / (1000 * 1000);
                         cout << "m, ";
                         print_perm (array + col_offset, N, 28);
@@ -917,15 +917,15 @@
                 } else { // reached end of column
                         narrays++;
 
                         if ((narrays % oaextend.nLMC == 0) ||
                             ((get_time_ms () - extendTime) > oaextend.singleExtendTime)) {
                                 extendTime = get_time_ms ();
                                 if (log_print (QUIET, "")) {
-                                        logstream (QUIET) << printfstring ("  OA extension: ") << narrays - 1
+                                        logstream (QUIET) << printfstring ("  OA extension: ") << narrays
                                                           << " arrays checked, " << extensions.size ()
                                                           << " solutions so far";
                                         logstream (QUIET) << ", time " << printtime ();
                                         myprintf ("  OA extension: current row: ");
                                         print_perm (array + col_offset, N, 36);
                                 }
                         }
```

### Comparing `OApackage-2.7.6/src/extend.h` & `OApackage-2.7.7/src/extend.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/graphtools.cpp` & `OApackage-2.7.7/src/graphtools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/graphtools.h` & `OApackage-2.7.7/src/graphtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/lmc.cpp` & `OApackage-2.7.7/src/lmc.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/lmc.h` & `OApackage-2.7.7/src/lmc.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/mathtools.cpp` & `OApackage-2.7.7/src/mathtools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/mathtools.h` & `OApackage-2.7.7/src/mathtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/md5.cpp` & `OApackage-2.7.7/src/md5.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/mpitools/mpitools.cpp` & `OApackage-2.7.7/src/mpitools/mpitools.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/mpitools/mpitools.h` & `OApackage-2.7.7/src/mpitools/mpitools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/msstdint.h` & `OApackage-2.7.7/src/msstdint.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/gtools.c` & `OApackage-2.7.7/src/nauty/gtools.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/gtools.h` & `OApackage-2.7.7/src/nauty/gtools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naugraph.c` & `OApackage-2.7.7/src/nauty/naugraph.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naugroup.c` & `OApackage-2.7.7/src/nauty/naugroup.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naugroup.h` & `OApackage-2.7.7/src/nauty/naugroup.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naurng.c` & `OApackage-2.7.7/src/nauty/naurng.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naurng.h` & `OApackage-2.7.7/src/nauty/naurng.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nausparse.h` & `OApackage-2.7.7/src/nauty/nausparse.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nautil.c` & `OApackage-2.7.7/src/nauty/nautil.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nautinv.c` & `OApackage-2.7.7/src/nauty/nautinv.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nautinv.h` & `OApackage-2.7.7/src/nauty/nautinv.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/naututil.h` & `OApackage-2.7.7/src/nauty/naututil.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nauty.c` & `OApackage-2.7.7/src/nauty/nauty.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/nauty.h` & `OApackage-2.7.7/src/nauty/nauty.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/schreier.c` & `OApackage-2.7.7/src/nauty/schreier.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/schreier.h` & `OApackage-2.7.7/src/nauty/schreier.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nauty/sorttemplates.c` & `OApackage-2.7.7/src/nauty/sorttemplates.c`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nonroot.cpp` & `OApackage-2.7.7/src/nonroot.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/nonroot.h` & `OApackage-2.7.7/src/nonroot.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/oaoptions.cpp` & `OApackage-2.7.7/src/oaoptions.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/oaoptions.h` & `OApackage-2.7.7/src/oaoptions.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/pareto.h` & `OApackage-2.7.7/src/pareto.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/printfheader.h` & `OApackage-2.7.7/src/printfheader.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/strength.cpp` & `OApackage-2.7.7/src/strength.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/strength.h` & `OApackage-2.7.7/src/strength.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/tools.cpp` & `OApackage-2.7.7/src/tools.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -327,30 +327,33 @@
         static int _loglevel = (int)SYSTEM;
 #else
         static int _loglevel = (int)QUIET;
 #endif
 
 		char buf[64 * 1024];
 
-		va_list va;
-		va_start(va, message);
-		vsprintf(buf, message, va);
-		va_end(va);
-
         if (level < 0) { // level < 0 means set level, any message appended is printed as well
 #pragma omp critical(logprint)
                 {
+						va_list va;
+						va_start(va, message);
+						vsprintf(buf, message, va);
+						va_end(va);
                         int mlevel = -level;
                         _loglevel = mlevel;
 						myprintf ("%s", buf);
                 }
         } else {
                 if (level <= _loglevel) { // if printing level is high enough, the message is shown
 #pragma omp critical(logprint)
                         {
+							va_list va;
+							va_start(va, message);
+							vsprintf(buf, message, va);
+							va_end(va);
 							myprintf ("%s", buf);
                         }
                 }
         }
         result = (level <= _loglevel);
 
         return result;
```

### Comparing `OApackage-2.7.6/src/tools.h` & `OApackage-2.7.7/src/tools.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/unittests.cpp` & `OApackage-2.7.7/src/unittests.cpp`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/src/unittests.h` & `OApackage-2.7.7/src/unittests.h`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_Doptim.py` & `OApackage-2.7.7/tests/test_Doptim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,171 @@
 """ Orthogonal Array package test functions
 """
 
-import sys
-import numpy as np
+import io
 import tempfile
-import logging
 import unittest
-if sys.version_info >= (3, 4):
-    import unittest.mock as mock
-    import io
-    from unittest.mock import patch
-    python3 = True
-else:
-    try:
-        import mock
-    except ImportError as ex:
-        logging.exception(ex)
-        raise Exception('to perform tests with python2 install the mock package (see https://pypi.org/project/mock/)')
-    python3 = False
-    patch = None
+import unittest.mock as mock
+
+import numpy as np
 
 import oalib
 import oapackage
-import oapackage.scanf
 import oapackage.Doptim
-
-
-def only_python3(function):
-    if python3:
-        def only_python3_function(*args, **kwargs):
-            return function(*args, **kwargs)
-    else:
-        def only_python3_function(*args, **kwargs):
-            return None
-    return only_python3_function
+import oapackage.scanf
 
 
 class TestDoptimize(unittest.TestCase):
-
     def setUp(self):
-
         self.arrayclass = oapackage.arraydata_t(2, 16, 0, 6)
         self.dds = np.random.rand(20, 3)
         self.dds2 = np.array([[1, 1, 1], [1, 2, 1], [1, 2, 3], [2, 0, 1]])
 
         self.guitest = True
-        try:
-            import matplotlib.pyplot
-        except:
-            self.guitest = False
 
-    @only_python3
+    def test_Doptimize_large_number_of_runs(self):
+        arrayclass = oapackage.arraydata_t(2, 1000, 0, 3)
+        scores, dds, sols, _ = oapackage.Doptim.Doptimize(
+            arrayclass, nrestarts=10, optimfunc=[1, 0, 0], verbose=0, maxtime=9, niter=10, dverbose=0
+        )
+
+        with self.assertRaises(Exception):
+            arrayclass = oapackage.arraydata_t(2, 100_000, 0, 3)
+            scores, dds, sols, _ = oapackage.Doptim.Doptimize(
+                arrayclass, nrestarts=10, optimfunc=[1, 0, 0], verbose=0, maxtime=9, niter=10
+            )
+
     def test_custom_optim(self):
-        def optimfunc(x): return x[0] + x[1] + x[2]
-        with mock.patch('sys.stdout', new_callable=io.StringIO) as mock_stdout:
-            scores, dds, sols, n = oapackage.Doptim.Doptimize(self.arrayclass, nrestarts=2, optimfunc=optimfunc, verbose=1,
-                                                              maxtime=18, selectpareto=False, nout=None, method=oalib.DOPTIM_UPDATE, niter=1000, nabort=0, dverbose=0)
+        def optimfunc(x):
+            return x[0] + x[1] + x[2]
+
+        with mock.patch("sys.stdout", new_callable=io.StringIO):
+            scores, dds, sols, n = oapackage.Doptim.Doptimize(
+                self.arrayclass,
+                nrestarts=2,
+                optimfunc=optimfunc,
+                verbose=1,
+                maxtime=18,
+                selectpareto=False,
+                nout=None,
+                method=oalib.DOPTIM_UPDATE,
+                niter=1000,
+                nabort=0,
+                dverbose=0,
+            )
         self.assertEqual(len(scores), n)
         self.assertEqual(len(dds), n)
         self.assertEqual(len(sols), n)
-        scores, dds, sols, n = oapackage.Doptim.Doptimize(self.arrayclass, nrestarts=2, optimfunc=None, verbose=0,
-                                                          maxtime=6, selectpareto=False, nout=None, method=oalib.DOPTIM_UPDATE, niter=30, nabort=0, dverbose=0)
+        scores, dds, sols, n = oapackage.Doptim.Doptimize(
+            self.arrayclass,
+            nrestarts=2,
+            optimfunc=None,
+            verbose=0,
+            maxtime=6,
+            selectpareto=False,
+            nout=None,
+            method=oalib.DOPTIM_UPDATE,
+            niter=30,
+            nabort=0,
+            dverbose=0,
+        )
 
-    @only_python3
     def test_Doptimize_nonzero_strength(self):
         arrayclass = oapackage.arraydata_t(2, 16, 2, 6)
         with self.assertWarns(UserWarning):
             scores, dds, sols, _ = oapackage.Doptim.Doptimize(
-                arrayclass, nrestarts=1, verbose=0, maxtime=9, selectpareto=False, nout=None, niter=1000, dverbose=0)
+                arrayclass, nrestarts=1, verbose=0, maxtime=9, selectpareto=False, nout=None, niter=1000, dverbose=0
+            )
 
     def test_Doptimize_selectDn(self):
-        scores, dds, sols, _ = oapackage.Doptim.Doptimize(self.arrayclass, nrestarts=10, optimfunc=[
-                                                          1, 0, 0], verbose=0, maxtime=9, selectpareto=False, nout=None, method=oalib.DOPTIM_UPDATE, niter=1000, nabort=0, dverbose=0)
+        scores, dds, sols, _ = oapackage.Doptim.Doptimize(
+            self.arrayclass,
+            nrestarts=10,
+            optimfunc=[1, 0, 0],
+            verbose=0,
+            maxtime=9,
+            selectpareto=False,
+            nout=None,
+            method=oalib.DOPTIM_UPDATE,
+            niter=1000,
+            nabort=0,
+            dverbose=0,
+        )
 
         result = oapackage.Doptim.selectDn(scores, dds, sols, nout=1, sortfull=True)
         self.assertTrue(len(result[2]) == 1)
 
-    @only_python3
     def test_optimDeffPython(self):
         al = oapackage.exampleArray(2, 0)
-        with mock.patch('sys.stdout', new_callable=io.StringIO) as mock_stdout:
+        with mock.patch("sys.stdout", new_callable=io.StringIO) as mock_stdout:
             _, al = oapackage.Doptim.optimDeffPython(
-                al, arrayclass=None, niter=1000, nabort=1500, verbose=1, alpha=[1, 0, 0], method=0)
+                al, arrayclass=None, niter=1000, nabort=1500, verbose=1, alpha=[1, 0, 0], method=0
+            )
             stdout = mock_stdout.getvalue()
-            self.assertTrue(stdout.startswith('optimDeff: initial Deff 0.0000'))
+            self.assertTrue(stdout.startswith("optimDeff: initial Deff 0.0000"))
 
         for method in [oapackage.oalib.DOPTIM_SWAP, oapackage.oalib.DOPTIM_FLIP, oapackage.oalib.DOPTIM_UPDATE]:
             r, al = oapackage.Doptim.optimDeffPython(
-                al, arrayclass=None, niter=100, nabort=200, verbose=0, alpha=[1, 0, 0], method=method)
+                al, arrayclass=None, niter=100, nabort=200, verbose=0, alpha=[1, 0, 0], method=method
+            )
 
-    @only_python3
     def test_generateDscatter(self):
         if self.guitest:
             fig = 100
-            with mock.patch('sys.stdout', new_callable=io.StringIO) as mock_stdout:
-                r = oapackage.Doptim.generateDscatter(self.dds, second_index=0, first_index=1, lbls=None, verbose=1,
-                                                      ndata=3, nofig=True, fig=fig, scatterarea=80)
-        else:
-            pass
+            with mock.patch("sys.stdout", new_callable=io.StringIO):
+                oapackage.Doptim.generateDscatter(
+                    self.dds,
+                    second_index=0,
+                    first_index=1,
+                    lbls=None,
+                    verbose=1,
+                    ndata=3,
+                    nofig=True,
+                    fig=fig,
+                    scatterarea=80,
+                )
 
-    @only_python3
     def test_generateDpage(self):
         outputdir = tempfile.mkdtemp()
         allarrays = [oapackage.exampleArray(2, 0), oapackage.exampleArray(2, 0)]
         dds = np.array([A.Defficiencies() for A in allarrays])
         arrayclass = oapackage.arraylink2arraydata(allarrays[0])
 
-        with mock.patch('sys.stdout', new_callable=io.StringIO) as mock_stdout:
-            page = oapackage.Doptim.generateDpage(outputdir, arrayclass, dds, allarrays,
-                                                  fig=None, optimfunc=[1, 0, 0], nofig=True)
+        with mock.patch("sys.stdout", new_callable=io.StringIO):
+            page = oapackage.Doptim.generateDpage(
+                outputdir, arrayclass, dds, allarrays, fig=None, optimfunc=[1, 0, 0], nofig=True
+            )
         if self.guitest and 0:
-            print('test_generateDpage: run gui test')
-            page = oapackage.Doptim.generateDpage(outputdir, arrayclass, dds, allarrays,
-                                                  fig=100, optimfunc=[1, 0, 0], nofig=True)
+            print("test_generateDpage: run gui test")
+            page = oapackage.Doptim.generateDpage(
+                outputdir, arrayclass, dds, allarrays, fig=100, optimfunc=[1, 0, 0], nofig=True
+            )
 
             self.assertIsInstance(page, oapackage.markup.page)
             try:
                 import matplotlib
+
                 matplotlib.pyplot.close(100)
             except ImportError:
                 pass
 
     def test_filterPareto(self):
         dds = self.dds2
         scores = np.arange(dds.shape[0])
         sols = [None] * scores.size
         s, _, _ = oapackage.Doptim.filterPareto(scores, dds, sols, verbose=0)
         self.assertEqual(list(s), [2, 3])
 
     def test_calcScore(self):
         dds = np.random.rand(10, 3)
         scores = oapackage.Doptim.calcScore(dds, optimfunc=[1, 2, 3])
-        self.assertEqual(scores.shape, (dds.shape[0], ))
+        self.assertEqual(scores.shape, (dds.shape[0],))
 
     def test_array2Dtable(self):
         sols = [oapackage.exampleArray(9, 0)]
         _ = oapackage.Doptim.array2Dtable(sols, verbose=1, titlestr=None)
 
 
-if __name__ == '__main__':
-    """ Test code """
+if __name__ == "__main__":
+    """Test code"""
     unittest.main()
     # t=TestDoptimize()
```

### Comparing `OApackage-2.7.6/tests/test_conference.py` & `OApackage-2.7.7/tests/test_conference.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_cpplibrary.py` & `OApackage-2.7.7/tests/test_cpplibrary.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_cpplibrary_gwlp.py` & `OApackage-2.7.7/tests/test_cpplibrary_gwlp.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_cpplibrary_macwilliams.py` & `OApackage-2.7.7/tests/test_cpplibrary_macwilliams.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_nauty.py` & `OApackage-2.7.7/tests/test_nauty.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_oapackage.py` & `OApackage-2.7.7/tests/test_oapackage.py`

 * *Files identical despite different names*

### Comparing `OApackage-2.7.6/tests/test_oapackage_graphtools.py` & `OApackage-2.7.7/tests/test_oapackage_graphtools.py`

 * *Files identical despite different names*

