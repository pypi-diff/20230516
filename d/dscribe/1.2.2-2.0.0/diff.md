# Comparing `tmp/dscribe-1.2.2.tar.gz` & `tmp/dscribe-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscribe-1.2.2.tar", last modified: Mon Aug  1 19:11:33 2022, max compression
+gzip compressed data, was "dist/dscribe-2.0.0.tar", last modified: Tue May 16 17:40:46 2023, max compression
```

## Comparing `dscribe-1.2.2.tar` & `dscribe-2.0.0.tar`

### file list

```diff
@@ -1,480 +1,495 @@
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.627887 dscribe-1.2.2/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11357 2020-10-17 10:19:00.000000 dscribe-1.2.2/LICENSE
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2021-11-16 20:44:22.000000 dscribe-1.2.2/MANIFEST.in
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1363 2022-08-01 19:11:33.627887 dscribe-1.2.2/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3260 2021-11-16 20:56:57.000000 dscribe-1.2.2/README.md
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.567883 dscribe-1.2.2/dependencies/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.567883 dscribe-1.2.2/dependencies/eigen/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.571884 dscribe-1.2.2/dependencies/eigen/Eigen/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1161 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Cholesky
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1900 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/CholmodSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12935 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Core
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Dense
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       35 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Eigen
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1777 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Eigenvalues
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1940 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Geometry
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      829 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Householder
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2083 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      894 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Jacobi
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1389 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/KLUSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1268 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/LU
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      991 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/MetisSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2451 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/OrderingMethods
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1751 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/PaStiXSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1116 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/PardisoSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1272 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/QR
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      900 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/QtAlignedMalloc
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1162 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SPQRSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1584 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SVD
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      888 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/Sparse
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1235 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SparseCholesky
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2240 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SparseCore
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1814 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SparseLU
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1195 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SparseQR
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      797 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/StdDeque
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      726 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/StdList
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      803 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/StdVector
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2243 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/SuperLUSupport
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1382 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/UmfPackSupport
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.571884 dscribe-1.2.2/dependencies/eigen/Eigen/src/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.571884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24880 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18706 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4010 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.571884 dscribe-1.2.2/dependencies/eigen/Eigen/src/CholmodSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25477 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/CholmodSupport/InternalHeaderCheck.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.579884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19497 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArithmeticSequence.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16552 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Array.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8252 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7054 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2774 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Assign.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    41665 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/AssignEvaluator.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)    12524 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14111 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18756 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Block.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4465 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6017 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7026 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    63877 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4781 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7905 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    36318 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8268 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3973 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5587 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    31391 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24520 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25396 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9906 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14706 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1024 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11690 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Dot.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5877 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4945 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5795 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21715 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    38856 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11579 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8274 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/IO.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9669 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/IndexedView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      134 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3539 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7127 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Map.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11317 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    60814 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7193 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24110 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23892 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2556 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3656 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12920 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9242 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PartialReduxEvaluator.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20784 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    49096 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7372 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Product.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    53868 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7792 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Random.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19231 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Redux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17858 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Ref.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5692 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17069 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Reshaped.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4320 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7558 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6179 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Select.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15024 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1733 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6905 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Solve.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9404 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6206 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8736 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21677 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/StlIterators.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4248 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Stride.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2801 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Swap.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17642 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13603 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    38314 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3461 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    35204 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12033 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.567883 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.579884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14975 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8142 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    72351 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2604 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.579884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15918 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13384 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   101935 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2174 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16241 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2363 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   119395 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9530 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24860 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)   102434 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17995 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/CUDA/Complex.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26696 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/BFloat16.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5291 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    68873 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4007 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    35574 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/Half.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1746 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/Settings.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3786 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2735 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    55819 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9563 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/Tuple.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2297 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.567883 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/HIP/
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      691 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17448 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16199 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    33655 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21953 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6855 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3123 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   193649 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    51326 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13818 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6805 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)    64504 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3690 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1234 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21240 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1391 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7468 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12579 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    27826 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21897 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2666 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16305 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8064 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)    36934 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.583884 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6723 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22435 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8371 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5035 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      644 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    40182 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.599885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   108486 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20141 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15985 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6973 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5143 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21762 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6405 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5619 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21391 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11607 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9995 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5246 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6201 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4163 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21024 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13904 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14759 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10608 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14715 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6744 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5919 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.599885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)    23193 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    19913 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ConfigureVectorization.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21968 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Constants.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)     5488 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15592 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6307 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/IndexedViewHelper.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11043 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/IntegralConstant.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)     4305 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    53453 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    46698 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Memory.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)    31051 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       85 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1026 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1469 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ReshapedHelper.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6533 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Serializer.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5496 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12076 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/SymbolicIndex.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    35799 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.603885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12494 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17309 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4214 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23006 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17108 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9752 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14385 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5611 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23676 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21114 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3686 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    35097 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4140 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22742 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.603885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    18975 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8439 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3660 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20762 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11998 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8991 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9848 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    34337 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6898 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8099 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6760 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    61966 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7700 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6226 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.603885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/arch/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5982 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.603885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4820 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5401 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23647 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/HouseholderSequence.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/InternalHeaderCheck.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6807 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6886 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8923 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15072 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14976 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      170 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13415 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7385 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4248 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/Jacobi/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      138 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Jacobi/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16419 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/KLUSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      146 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/KLUSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11591 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/KLUSupport/KLUSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3475 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    32328 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      130 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15763 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22014 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3591 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/arch/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13730 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/arch/InverseSize4.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/MetisSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/MetisSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4624 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16141 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    61681 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      156 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5284 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      152 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/PaStiXSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    22284 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/PardisoSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/PardisoSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    20124 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25443 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4698 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23382 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    26713 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14584 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3029 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      130 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/InternalHeaderCheck.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.607885 dscribe-1.2.2/dependencies/eigen/Eigen/src/SPQRSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SPQRSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11862 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.611886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    54248 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/BDCSVD.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      132 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    33023 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5135 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14692 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15993 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.611886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24252 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5866 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.615886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10706 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8779 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13202 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      146 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2227 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11404 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24395 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6521 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13642 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25513 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4793 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    13292 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5844 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3116 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1143 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12625 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMap.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    57216 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17487 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7365 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7629 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1735 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15636 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    25541 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4460 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8740 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3211 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6473 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6762 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14642 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8163 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9693 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.615886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    33351 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4339 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7638 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5010 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12872 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2085 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6748 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6620 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3717 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    10253 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4217 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5759 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8521 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9064 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5015 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4581 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2925 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.615886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseQR/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseQR/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    29202 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.615886 dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4850 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4273 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5460 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2809 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.615886 dscribe-1.2.2/dependencies/eigen/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SuperLUSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    34360 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.619886 dscribe-1.2.2/dependencies/eigen/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/UmfPackSupport/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    24492 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.619886 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2949 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/Image.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      134 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2778 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1784 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    30560 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/blas.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7834 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/lapack.h
--rwxrwxr-x   0 lauri     (1000) lauri     (1000)  1058369 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      474 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.619886 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    14060 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21431 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    59020 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4827 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6089 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    12311 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/IndexedViewMethods.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      137 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/InternalHeaderCheck.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6387 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3350 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6915 2021-10-18 17:38:51.000000 dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ReshapedMethods.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.619886 dscribe-1.2.2/dscribe/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      629 2020-10-17 10:19:00.000000 dscribe-1.2.2/dscribe/__init__.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.623886 dscribe-1.2.2/dscribe/core/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      670 2020-10-17 10:19:00.000000 dscribe-1.2.2/dscribe/core/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7120 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/core/lattice.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9317 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/core/system.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.623886 dscribe-1.2.2/dscribe/descriptors/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1112 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    17142 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/descriptors/acsf.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    15523 2022-08-01 16:05:52.000000 dscribe-1.2.2/dscribe/descriptors/coulombmatrix.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    23410 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/descriptors/descriptor.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    16243 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/ewaldsummatrix.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    37371 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/descriptors/lmbtr.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8679 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/matrixdescriptor.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    42184 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/mbtr.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5440 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/sinematrix.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    55196 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/descriptors/soap.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4478 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/descriptors/valleoganov.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.627887 dscribe-1.2.2/dscribe/ext/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7000 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/ext/acsf.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2387 2021-11-16 20:44:22.000000 dscribe-1.2.2/dscribe/ext/acsf.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5697 2022-01-02 20:09:09.000000 dscribe-1.2.2/dscribe/ext/celllist.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2490 2021-09-07 19:07:15.000000 dscribe-1.2.2/dscribe/ext/celllist.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4516 2022-08-01 18:59:09.000000 dscribe-1.2.2/dscribe/ext/cm.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2106 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/cm.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    11883 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/descriptor.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2266 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/descriptor.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6271 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/descriptorglobal.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3292 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/descriptorglobal.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6630 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/ext.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     6736 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/geometry.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2411 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/geometry.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    27163 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/mbtr.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     8620 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/mbtr.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7307 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/soap.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4842 2022-07-08 11:50:09.000000 dscribe-1.2.2/dscribe/ext/soap.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)   439407 2022-01-02 20:09:09.000000 dscribe-1.2.2/dscribe/ext/soapGTO.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     3065 2021-08-18 17:09:08.000000 dscribe-1.2.2/dscribe/ext/soapGTO.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    47359 2021-08-18 17:09:08.000000 dscribe-1.2.2/dscribe/ext/soapGeneral.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2959 2021-08-18 17:09:08.000000 dscribe-1.2.2/dscribe/ext/soapGeneral.h
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2897 2021-08-18 17:09:08.000000 dscribe-1.2.2/dscribe/ext/weighting.cpp
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1303 2021-08-18 17:09:08.000000 dscribe-1.2.2/dscribe/ext/weighting.h
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.627887 dscribe-1.2.2/dscribe/kernels/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      702 2020-10-17 10:19:00.000000 dscribe-1.2.2/dscribe/kernels/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1790 2021-04-23 17:01:22.000000 dscribe-1.2.2/dscribe/kernels/averagekernel.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     7264 2021-04-23 17:01:22.000000 dscribe-1.2.2/dscribe/kernels/localsimilaritykernel.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     5219 2021-04-23 17:01:22.000000 dscribe-1.2.2/dscribe/kernels/rematchkernel.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.627887 dscribe-1.2.2/dscribe/utils/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)      590 2020-10-17 10:19:00.000000 dscribe-1.2.2/dscribe/utils/__init__.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1057 2021-04-23 17:01:22.000000 dscribe-1.2.2/dscribe/utils/dimensionality.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     9349 2021-04-23 17:01:22.000000 dscribe-1.2.2/dscribe/utils/geometry.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2727 2022-01-19 18:24:25.000000 dscribe-1.2.2/dscribe/utils/species.py
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     2922 2020-10-17 10:19:00.000000 dscribe-1.2.2/dscribe/utils/stats.py
-drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2022-08-01 19:11:33.619886 dscribe-1.2.2/dscribe.egg-info/
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     1363 2022-08-01 19:11:33.000000 dscribe-1.2.2/dscribe.egg-info/PKG-INFO
--rw-rw-r--   0 lauri     (1000) lauri     (1000)    21376 2022-08-01 19:11:33.000000 dscribe-1.2.2/dscribe.egg-info/SOURCES.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2022-08-01 19:11:33.000000 dscribe-1.2.2/dscribe.egg-info/dependency_links.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       72 2022-08-01 19:11:33.000000 dscribe-1.2.2/dscribe.egg-info/requires.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)        8 2022-08-01 19:11:33.000000 dscribe-1.2.2/dscribe.egg-info/top_level.txt
--rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2022-08-01 19:11:33.627887 dscribe-1.2.2/setup.cfg
--rw-rw-r--   0 lauri     (1000) lauri     (1000)     4496 2022-08-01 18:59:09.000000 dscribe-1.2.2/setup.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11357 2020-10-17 10:19:00.000000 dscribe-2.0.0/LICENSE
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2023-01-24 19:40:17.000000 dscribe-2.0.0/MANIFEST.in
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1302 2023-05-16 17:40:46.000000 dscribe-2.0.0/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3535 2023-05-16 17:25:34.000000 dscribe-2.0.0/README.md
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1161 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Cholesky
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1900 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/CholmodSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12935 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Core
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      122 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Dense
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       35 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Eigen
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1777 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Eigenvalues
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1940 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Geometry
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      829 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Householder
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2083 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      894 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Jacobi
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1389 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/KLUSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1268 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/LU
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      991 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/MetisSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2451 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/OrderingMethods
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1751 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/PaStiXSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1116 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/PardisoSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1272 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/QR
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      900 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1162 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SPQRSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1584 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SVD
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      888 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/Sparse
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1235 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SparseCholesky
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2240 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SparseCore
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1814 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SparseLU
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1195 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SparseQR
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      797 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/StdDeque
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      726 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/StdList
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      803 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/StdVector
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2243 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/SuperLUSupport
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1382 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/UmfPackSupport
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24880 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18706 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4010 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25477 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/CholmodSupport/CholmodSupport.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/CholmodSupport/InternalHeaderCheck.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19497 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArithmeticSequence.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16552 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Array.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8252 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7054 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2774 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    41665 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/AssignEvaluator.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)    12524 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14111 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18756 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Block.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4465 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6017 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7026 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    63877 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4781 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7905 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    36318 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8268 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3973 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5587 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    31391 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24520 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25396 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9906 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14706 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1024 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11690 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5877 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4945 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5795 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21715 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    38856 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11579 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8274 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/IO.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9669 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/IndexedView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      134 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3539 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Inverse.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7127 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Map.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11317 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    60814 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7193 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24110 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23892 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2556 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3656 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12920 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9242 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20784 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    49096 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7372 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Product.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    53868 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7792 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Random.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19231 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17858 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5692 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17069 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Reshaped.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4320 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7558 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6179 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Select.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15024 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1733 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6905 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Solve.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9404 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6206 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SolverBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8736 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21677 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/StlIterators.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4248 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2801 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17642 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13603 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    38314 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3461 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35204 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12033 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14975 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8142 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    72351 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2604 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15918 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13384 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   101935 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2174 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16241 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2363 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   119395 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9530 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24860 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)   102434 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/CUDA/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17995 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/CUDA/Complex.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26696 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5291 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    68873 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4007 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35574 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/Half.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1746 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/Settings.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3786 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2735 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    55819 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9563 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/Tuple.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2297 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/HIP/
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      691 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17448 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16199 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    33655 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21953 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6855 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3123 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   193649 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    51326 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13818 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6805 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)    64504 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3690 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1234 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21240 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1391 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7468 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12579 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    27826 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21897 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2666 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16305 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8064 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)    36934 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6723 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22435 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8371 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5035 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      644 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    40182 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   108486 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20141 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15985 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6973 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5143 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21762 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6405 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5619 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21391 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11607 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9995 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5246 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6201 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4163 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21024 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13904 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14759 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10608 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14715 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6744 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5919 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)    23193 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    19913 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21968 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Constants.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)     5488 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15592 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6307 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11043 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/IntegralConstant.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)     4305 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    53453 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    46698 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Memory.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)    31051 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       85 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1026 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1469 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ReshapedHelper.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6533 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Serializer.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5496 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12076 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/SymbolicIndex.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35799 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12494 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17309 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4214 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23006 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17108 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9752 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14385 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5611 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23676 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21114 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3686 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35097 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4140 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22742 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    18975 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8439 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3660 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20762 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11998 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8991 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9848 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    34337 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6898 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8099 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6760 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    61966 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7700 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6226 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5982 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4820 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5401 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23647 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/HouseholderSequence.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/InternalHeaderCheck.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6807 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6886 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8923 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15072 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14976 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      170 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13415 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7385 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4248 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Jacobi/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      138 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Jacobi/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16419 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/KLUSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      146 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/KLUSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11591 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/KLUSupport/KLUSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3475 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    32328 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      130 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15763 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/InverseImpl.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22014 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3591 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/arch/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13730 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/arch/InverseSize4.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/MetisSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      150 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/MetisSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4624 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16141 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    61681 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      156 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5284 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      152 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PaStiXSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    22284 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PardisoSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    20124 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25443 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4698 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    23382 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    26713 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14584 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3029 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      130 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/InternalHeaderCheck.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      148 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SPQRSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11862 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    54248 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/BDCSVD.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      132 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    33023 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5135 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14692 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/SVDBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15993 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24252 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5866 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10706 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8779 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13202 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      146 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2227 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11404 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24395 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6521 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13642 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25513 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4793 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    13292 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5844 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3116 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1143 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12625 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    57216 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17487 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7365 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7629 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1735 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15636 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    25541 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4460 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8740 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3211 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6473 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6762 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14642 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8163 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9693 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    33351 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4339 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7638 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5010 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12872 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2085 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6748 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6620 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3717 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10253 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4217 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5759 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8521 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9064 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5015 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4581 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2925 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseQR/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      142 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseQR/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29202 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4850 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4273 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5460 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2809 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SuperLUSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    34360 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      154 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/UmfPackSupport/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24492 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2949 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/Image.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      134 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2778 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1784 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    30560 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/blas.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7834 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/lapack.h
+-rwxrwxr-x   0 lauri     (1000) lauri     (1000)  1058369 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/lapacke.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      474 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/lapacke_mangling.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14060 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21431 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    59020 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4827 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6089 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    12311 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/IndexedViewMethods.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      137 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/InternalHeaderCheck.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6387 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3350 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6915 2021-10-18 17:38:51.000000 dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ReshapedMethods.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      629 2020-10-17 10:19:00.000000 dscribe-2.0.0/dscribe/__init__.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/core/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      670 2020-10-17 10:19:00.000000 dscribe-2.0.0/dscribe/core/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7120 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/core/lattice.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9315 2023-03-14 20:10:50.000000 dscribe-2.0.0/dscribe/core/system.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/descriptors/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      992 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17184 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/acsf.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6696 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/coulombmatrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24234 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/descriptor.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10959 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/descriptorglobal.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    16651 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/descriptorlocal.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    10034 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/descriptormatrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    15809 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/ewaldsummatrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35672 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/lmbtr.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    36971 2023-05-16 17:27:11.000000 dscribe-2.0.0/dscribe/descriptors/mbtr.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5142 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/sinematrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    44115 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/soap.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3040 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/descriptors/valleoganov.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/ext/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7000 2023-05-02 17:12:07.000000 dscribe-2.0.0/dscribe/ext/acsf.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2387 2023-05-02 17:12:07.000000 dscribe-2.0.0/dscribe/ext/acsf.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5697 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/celllist.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2490 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/celllist.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4516 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/cm.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2106 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/cm.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    11883 2023-05-09 15:02:57.000000 dscribe-2.0.0/dscribe/ext/descriptor.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2266 2023-05-09 15:02:57.000000 dscribe-2.0.0/dscribe/ext/descriptor.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6271 2023-05-09 15:02:57.000000 dscribe-2.0.0/dscribe/ext/descriptorglobal.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3292 2023-05-09 15:02:57.000000 dscribe-2.0.0/dscribe/ext/descriptorglobal.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6630 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/ext.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     6736 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/geometry.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2411 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/geometry.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    35335 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/mbtr.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9147 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/mbtr.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7488 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/soap.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4920 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/soap.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)   440691 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/soapGTO.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     3125 2023-05-16 17:25:34.000000 dscribe-2.0.0/dscribe/ext/soapGTO.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    47359 2023-05-02 19:43:08.000000 dscribe-2.0.0/dscribe/ext/soapGeneral.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2959 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/ext/soapGeneral.h
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2897 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/ext/weighting.cpp
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1303 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/ext/weighting.h
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/kernels/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      702 2020-10-17 10:19:00.000000 dscribe-2.0.0/dscribe/kernels/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1790 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/kernels/averagekernel.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7262 2023-03-14 20:10:50.000000 dscribe-2.0.0/dscribe/kernels/localsimilaritykernel.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5219 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/kernels/rematchkernel.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe/utils/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)      590 2020-10-17 10:19:00.000000 dscribe-2.0.0/dscribe/utils/__init__.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1057 2023-01-24 19:40:18.000000 dscribe-2.0.0/dscribe/utils/dimensionality.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9348 2023-03-14 20:10:50.000000 dscribe-2.0.0/dscribe/utils/geometry.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2728 2023-03-14 19:55:18.000000 dscribe-2.0.0/dscribe/utils/species.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     2922 2020-10-17 10:19:00.000000 dscribe-2.0.0/dscribe/utils/stats.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1302 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/PKG-INFO
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    21727 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/SOURCES.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        1 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/dependency_links.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       72 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/requires.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)        8 2023-05-16 17:40:46.000000 dscribe-2.0.0/dscribe.egg-info/top_level.txt
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)       38 2023-05-16 17:40:46.000000 dscribe-2.0.0/setup.cfg
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4443 2023-05-16 17:25:34.000000 dscribe-2.0.0/setup.py
+drwxrwxr-x   0 lauri     (1000) lauri     (1000)        0 2023-05-16 17:40:46.000000 dscribe-2.0.0/tests/
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     9945 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_acsf.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7041 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_coulombmatrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7725 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_ewaldsummatrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     1485 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_examples.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    17356 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_general.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     7253 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_kernels.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     8743 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_lmbtr.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    29340 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_mbtr.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     5424 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_sinematrix.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    24367 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_soap.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)     4019 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/test_valle_oganov.py
+-rw-rw-r--   0 lauri     (1000) lauri     (1000)    14516 2023-05-16 17:25:34.000000 dscribe-2.0.0/tests/testutils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dscribe-1.2.2/LICENSE` & `dscribe-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/PKG-INFO` & `dscribe-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: dscribe
-Version: 1.2.2
+Version: 2.0.0
 Summary: A Python package for creating feature transformations in applications of machine learning to materials science.
 Home-page: https://singroup.github.io/dscribe/
 License: Apache License 2.0
+Description: A Python package for creating feature transformations in applications of machine learning to materials science.
 Keywords: descriptor machine learning atomistic structure materials science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-License-File: LICENSE
-
-A Python package for creating feature transformations in applications of machine learning to materials science.
-
+Requires-Python: >=3.7
```

### Comparing `dscribe-1.2.2/README.md` & `dscribe-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 <img src="https://raw.githubusercontent.com/SINGROUP/dscribe/master/logo/dscribe_logo.png" width="400">
 
-[![Build Status](https://dev.azure.com/laurihimanen/DScribe%20CI/_apis/build/status/SINGROUP.dscribe?branchName=master)](https://dev.azure.com/laurihimanen/DScribe%20CI/_build/latest?definitionId=1&branchName=master)
+![Build status](https://github.com/SINGROUP/dscribe/actions/workflows/actions.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/SINGROUP/dscribe/badge.svg?branch=master)](https://coveralls.io/github/SINGROUP/dscribe?branch=master)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 DScribe is a Python package for transforming atomic structures into fixed-size
 numerical fingerprints. These fingerprints are often called "descriptors" and
 they can be used in various tasks, including machine learning, visualization,
 similarity analysis, etc.
 
-# Homepage
-For more details and tutorials, visit the homepage at:
+# Documentation
+For more details and tutorials, visit our documentation at:
 [https://singroup.github.io/dscribe/](https://singroup.github.io/dscribe/)
 
+You can find even more details in our open-access articles:
+
+- [DScribe: Library of descriptors for machine learning in materials science](<https://doi.org/10.1016/j.cpc.2019.106949>)
+- [Updates to the DScribe Library: New Descriptors and Derivatives](https://doi.org/10.48550/arXiv.2303.14046)
+
+
 # Quick Example
 ```python
 import numpy as np
 from ase.build import molecule
 from dscribe.descriptors import SOAP
 from dscribe.descriptors import CoulombMatrix
 
@@ -26,38 +32,38 @@
 # Setup descriptors
 cm_desc = CoulombMatrix(n_atoms_max=3, permutation="sorted_l2")
 soap_desc = SOAP(species=["C", "H", "O", "N"], rcut=5, nmax=8, lmax=6, crossover=True)
 
 # Create descriptors as numpy arrays or sparse arrays
 water = samples[0]
 coulomb_matrix = cm_desc.create(water)
-soap = soap_desc.create(water, positions=[0])
+soap = soap_desc.create(water, centers=[0])
 
 # Easy to use also on multiple systems, can be parallelized across processes
 coulomb_matrices = cm_desc.create(samples)
 coulomb_matrices = cm_desc.create(samples, n_jobs=3)
 oxygen_indices = [np.where(x.get_atomic_numbers() == 8)[0] for x in samples]
 oxygen_soap = soap_desc.create(samples, oxygen_indices, n_jobs=3)
 
-# Some descriptors also allow calculating derivatives with respect to atomic
+# Descriptors also allow calculating derivatives with respect to atomic
 # positions
-der, des = soap_desc.derivatives(samples, method="auto", return_descriptor=True)
+der, des = soap_desc.derivatives(samples, return_descriptor=True)
 ```
 
 # Currently implemented descriptors
- | Descriptor                                    |  Spectrum |  Derivatives |
+ | Descriptor                                    |  Spectrum | Derivatives |
  |-----------------------------------------------|-----|-------|
  | Coulomb matrix                                | :heavy_check_mark: | :heavy_check_mark: |
- | Sine matrix                                   | :heavy_check_mark: | |
- | Ewald matrix                                  | :heavy_check_mark: | |
- | Atom-centered Symmetry Functions (ACSF)       | :heavy_check_mark: | |
- | Smooth Overlap of Atomic Positions (SOAP)     | :heavy_check_mark: |:heavy_check_mark: |
- | Many-body Tensor Representation (MBTR)        | :heavy_check_mark: | |
- | Local Many-body Tensor Representation (LMBTR) | :heavy_check_mark: | |
- | Valle-Oganov descriptor                       | :heavy_check_mark: | |
+ | Sine matrix                                   | :heavy_check_mark: | :heavy_check_mark: |
+ | Ewald matrix                                  | :heavy_check_mark: | :heavy_check_mark: |
+ | Atom-centered Symmetry Functions (ACSF)       | :heavy_check_mark: | :heavy_check_mark: |
+ | Smooth Overlap of Atomic Positions (SOAP)     | :heavy_check_mark: | :heavy_check_mark: |
+ | Many-body Tensor Representation (MBTR)        | :heavy_check_mark: | :heavy_check_mark: |
+ | Local Many-body Tensor Representation (LMBTR) | :heavy_check_mark: | :heavy_check_mark: |
+ | Valle-Oganov descriptor                       | :heavy_check_mark: | :heavy_check_mark: |
 
 # Installation
 In-depth installation instructions can be found [in the
 documentation](https://singroup.github.io/dscribe/latest/install.html), but in
 short:
 
 ## pip
```

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Cholesky` & `dscribe-2.0.0/dependencies/eigen/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/CholmodSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Core` & `dscribe-2.0.0/dependencies/eigen/Eigen/Core`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Eigenvalues` & `dscribe-2.0.0/dependencies/eigen/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Geometry` & `dscribe-2.0.0/dependencies/eigen/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Householder` & `dscribe-2.0.0/dependencies/eigen/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/IterativeLinearSolvers` & `dscribe-2.0.0/dependencies/eigen/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Jacobi` & `dscribe-2.0.0/dependencies/eigen/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/KLUSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/LU` & `dscribe-2.0.0/dependencies/eigen/Eigen/LU`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/MetisSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/OrderingMethods` & `dscribe-2.0.0/dependencies/eigen/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/PaStiXSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/PardisoSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/QR` & `dscribe-2.0.0/dependencies/eigen/Eigen/QR`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/QtAlignedMalloc` & `dscribe-2.0.0/dependencies/eigen/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SPQRSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SVD` & `dscribe-2.0.0/dependencies/eigen/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/Sparse` & `dscribe-2.0.0/dependencies/eigen/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SparseCholesky` & `dscribe-2.0.0/dependencies/eigen/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SparseCore` & `dscribe-2.0.0/dependencies/eigen/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SparseLU` & `dscribe-2.0.0/dependencies/eigen/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SparseQR` & `dscribe-2.0.0/dependencies/eigen/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/StdDeque` & `dscribe-2.0.0/dependencies/eigen/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/StdList` & `dscribe-2.0.0/dependencies/eigen/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/StdVector` & `dscribe-2.0.0/dependencies/eigen/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/SuperLUSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/UmfPackSupport` & `dscribe-2.0.0/dependencies/eigen/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LDLT.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LLT.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/CholmodSupport/CholmodSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArithmeticSequence.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Array.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArrayBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ArrayWrapper.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Assign.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/AssignEvaluator.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Assign_MKL.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/BandMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Block.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/BooleanRedux.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CommaInitializer.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ConditionEstimator.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CoreEvaluators.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CoreIterators.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseBinaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseNullaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseTernaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseUnaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/CwiseUnaryView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseCoeffsBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DenseStorage.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Diagonal.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DiagonalMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/DiagonalProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Dot.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/EigenBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ForceAlignedAccess.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Fuzzy.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GeneralProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GenericPacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/GlobalFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/IO.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/IndexedView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Inverse.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Map.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MapBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MathFunctionsImpl.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Matrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/MatrixBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NestByValue.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NoAlias.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/NumTraits.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PartialReduxEvaluator.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PermutationMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/PlainObjectBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Product.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ProductEvaluators.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Random.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Redux.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Ref.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Replicate.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Reshaped.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/ReturnByValue.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Reverse.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Select.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SelfAdjointView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Solve.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SolveTriangular.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/SolverBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/StableNorm.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/StlIterators.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Stride.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Swap.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Transpose.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Transpositions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/TriangularMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/VectorBlock.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/VectorwiseOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/Visitor.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/CUDA/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/BFloat16.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/ConjHelper.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/Half.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/Settings.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/Default/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/Tuple.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/Tuple.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/MSA/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/Complex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/AssignmentFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/BinaryFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/NullaryFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/StlFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/TernaryFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/functors/UnaryFunctors.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/Parallelizer.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/products/TriangularSolverVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/BlasUtil.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ConfigureVectorization.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Constants.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/DisableStupidWarnings.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ForwardDeclarations.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/IndexedViewHelper.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/IntegralConstant.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/MKL_support.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Macros.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Memory.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Meta.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/ReshapedHelper.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/Serializer.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/Serializer.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/StaticAssert.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/SymbolicIndex.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Core/util/XprHelper.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/EigenSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealQZ.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/AlignedBox.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/AngleAxis.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/EulerAngles.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Homogeneous.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Hyperplane.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/OrthoMethods.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/ParametrizedLine.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Quaternion.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Rotation2D.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/RotationBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Scaling.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Transform.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Translation.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/Umeyama.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/BlockHouseholder.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/Householder.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Householder/HouseholderSequence.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/Jacobi/Jacobi.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/KLUSupport/KLUSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/Determinant.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/FullPivLU.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/InverseImpl.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/PartialPivLU.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/LU/arch/InverseSize4.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/MetisSupport/MetisSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Amd.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/OrderingMethods/Ordering.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/PardisoSupport/PardisoSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/FullPivHouseholderQR.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/HouseholderQR.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/BDCSVD.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/JacobiSVD.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/SVDBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SVD/UpperBidiagonalization.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/AmbiVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/CompressedStorage.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseAssign.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseBlock.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseColEtree.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCompressedBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDenseProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseDot.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseFuzzy.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMap.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseMatrixBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparsePermutation.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseProduct.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseRedux.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseRef.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSolverBase.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseTranspose.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseTriangularView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseUtil.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/SparseView.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseCore/TriangularSolver.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLUImpl.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Memory.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Structs.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Utils.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SparseQR/SparseQR.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdDeque.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdList.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/StdVector.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/StlSupport/details.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/Image.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/Kernel.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/RealSvd2x2.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/blas.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/lapack.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/misc/lapacke.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/BlockMethods.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/IndexedViewMethods.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dependencies/eigen/Eigen/src/plugins/ReshapedMethods.h` & `dscribe-2.0.0/dependencies/eigen/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/__init__.py` & `dscribe-2.0.0/dscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/core/__init__.py` & `dscribe-2.0.0/dscribe/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/core/lattice.py` & `dscribe-2.0.0/dscribe/core/lattice.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/core/system.py` & `dscribe-2.0.0/dscribe/core/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         celldisp=None,
         constraint=None,
         calculator=None,
         info=None,
         wyckoff_positions=None,
         equivalent_atoms=None,
     ):
-
         super().__init__(
             symbols,
             positions,
             numbers,
             tags,
             momenta,
             masses,
@@ -153,15 +152,14 @@
         the distance of two different atoms is the distance of two closest
         copies.
 
         Returns:
             np.array: 3D matrix containing the pairwise distance vectors.
         """
         if self._displacement_tensor is None:
-
             D, D_len = ase.geometry.geometry.get_distances(
                 self.get_positions(), cell=self.get_cell(), pbc=self.get_pbc()
             )
 
             # Figure out the smallest basis vector and set it as
             # displacement for diagonal
             if self.get_pbc().any():
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/__init__.py` & `dscribe-2.0.0/dscribe/descriptors/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from dscribe.descriptors.descriptor import Descriptor
 from dscribe.descriptors.acsf import ACSF
 from dscribe.descriptors.mbtr import MBTR
 from dscribe.descriptors.valleoganov import ValleOganov
 from dscribe.descriptors.lmbtr import LMBTR
 from dscribe.descriptors.ewaldsummatrix import EwaldSumMatrix
 from dscribe.descriptors.coulombmatrix import CoulombMatrix
 from dscribe.descriptors.sinematrix import SineMatrix
-from dscribe.descriptors.matrixdescriptor import MatrixDescriptor
 from dscribe.descriptors.soap import SOAP
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/acsf.py` & `dscribe-2.0.0/dscribe/descriptors/acsf.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,55 +12,51 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
 
 import numpy as np
-
-import sparse
+import sparse as sp
 from scipy.sparse import coo_matrix
-
-from dscribe.descriptors.descriptor import Descriptor
-from dscribe.core import System
-
 from ase import Atoms
 
+from dscribe.descriptors.descriptorlocal import DescriptorLocal
 from dscribe.ext import ACSFWrapper
-
 import dscribe.utils.geometry
 
 
-class ACSF(Descriptor):
+class ACSF(DescriptorLocal):
     """Implementation of Atom-Centered Symmetry Functions.
 
     Notice that the species of the central atom is not encoded in the output,
     only the surrounding environment is encoded. In a typical application one
     can train a different model for each central species.
 
     For reference, see:
         "Atom-centered symmetry functions for constructing high-dimensional
         neural network potentials", Jörg Behler, The Journal of Chemical
         Physics, 134, 074106 (2011), https://doi.org/10.1063/1.3553717
     """
 
     def __init__(
         self,
-        rcut,
+        r_cut,
         g2_params=None,
         g3_params=None,
         g4_params=None,
         g5_params=None,
         species=None,
         periodic=False,
         sparse=False,
+        dtype="float64",
     ):
         """
         Args:
-            rcut (float): The smooth cutoff value in angstroms. This cutoff
+            r_cut (float): The smooth cutoff value in angstroms. This cutoff
                 value is used throughout the calculations for all symmetry
                 functions.
             g2_params (n*2 np.ndarray): A list of pairs of :math:`\eta` and
                 :math:`R_s` parameters for :math:`G^2` functions.
             g3_params (n*1 np.ndarray): A list of :math:`\kappa` parameters for
                 :math:`G^3` functions.
             g4_params (n*3 np.ndarray): A list of triplets of :math:`\eta`,
@@ -76,39 +72,39 @@
                 preferable.
             periodic (bool): Set to true if you want the descriptor output to
                 respect the periodicity of the atomic systems (see the
                 pbc-parameter in the constructor of ase.Atoms).
             sparse (bool): Whether the output should be a sparse matrix or a
                 dense numpy array.
         """
-        super().__init__(periodic=periodic, flatten=True, sparse=sparse)
+        super().__init__(periodic=periodic, sparse=sparse, dtype=dtype)
 
         self.acsf_wrapper = ACSFWrapper()
 
         # Setup
         self.species = species
         self.g2_params = g2_params
         self.g3_params = g3_params
         self.g4_params = g4_params
         self.g5_params = g5_params
-        self.rcut = rcut
+        self.r_cut = r_cut
 
     def create(
-        self, system, positions=None, n_jobs=1, only_physical_cores=False, verbose=False
+        self, system, centers=None, n_jobs=1, only_physical_cores=False, verbose=False
     ):
-        """Return the ACSF output for the given systems and given positions.
+        """Return the ACSF output for the given systems and given centers.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
                 many atomic structures.
-            positions (list): Positions where to calculate ACSF. Can be
+            centers (list): Centers where to calculate ACSF. Can be
                 provided as cartesian positions or atomic indices. If no
-                positions are defined, the SOAP output will be created for all
-                atoms in the system. When calculating SOAP for multiple
-                systems, provide the positions as a list for each system.
+                centers are defined, the output will be created for all
+                atoms in the system. When calculating output for multiple
+                systems, provide the centers as a list for each system.
             n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
                 the calculation across samples. Defaults to serial calculation
                 with n_jobs=1. If a negative number is given, the used cpus
                 will be calculated with, n_cpus + n_jobs, where n_cpus is the
                 amount of CPUs as reported by the OS. With only_physical_cores
                 you can control which types of CPUs are counted in n_cpus.
             only_physical_cores (bool): If a negative n_jobs is given,
@@ -116,45 +112,45 @@
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             np.ndarray | sparse.COO: The ACSF output for the given
-            systems and positions. The return type depends on the
+            systems and centers. The return type depends on the
             'sparse'-attribute. The first dimension is determined by the amount
-            of positions and systems and the second dimension is determined by
+            of centers and systems and the second dimension is determined by
             the get_number_of_features()-function. When multiple systems are
             provided the results are ordered by the input order of systems and
-            their positions.
+            their centers.
         """
         # Validate input / combine input arguments
         if isinstance(system, Atoms):
             system = [system]
-            positions = [positions]
-        if positions is None:
+            centers = [centers]
+        if centers is None:
             inp = [(i_sys,) for i_sys in system]
         else:
-            inp = list(zip(system, positions))
+            inp = list(zip(system, centers))
 
         # Determine if the outputs have a fixed size
         n_features = self.get_number_of_features()
         static_size = None
-        if positions is None:
+        if centers is None:
             n_centers = len(inp[0][0])
         else:
             first_sample, first_pos = inp[0]
             if first_pos is not None:
                 n_centers = len(first_pos)
             else:
                 n_centers = len(first_sample)
 
         def is_static():
             for i_job in inp:
-                if positions is None:
+                if centers is None:
                     if len(i_job[0]) != n_centers:
                         return False
                 else:
                     if i_job[1] is not None:
                         if len(i_job[1]) != n_centers:
                             return False
                     else:
@@ -173,67 +169,68 @@
             static_size,
             only_physical_cores,
             verbose=verbose,
         )
 
         return output
 
-    def create_single(self, system, positions=None):
+    def create_single(self, system, centers=None):
         """Creates the descriptor for the given system.
 
         Args:
             system (:class:`ase.Atoms` | :class:`.System`): Input system.
-            positions (iterable): Indices of the atoms around which the ACSF
-                will be returned. If no positions defined, ACSF will be created
+            centers (iterable): Indices of the atoms around which the ACSF
+                will be returned. If no centers defined, ACSF will be created
                 for all atoms in the system.
 
         Returns:
-            np.ndarray | sparse.COO: The ACSF output for the
-            given system and positions. The return type depends on the
-            'sparse'-attribute. The first dimension is given by the number of
-            positions and the second dimension is determined by the
-            get_number_of_features()-function.
+            np.ndarray: The ACSF output for the given system and centers. The
+            first dimension is given by the number of centers and the second
+            dimension is determined by the get_number_of_features()-function.
         """
+        # Check if there are types that have not been declared
+        self.check_atomic_numbers(system.get_atomic_numbers())
+
         # Create C-compatible list of atomic indices for which the ACSF is
         # calculated
         calculate_all = False
-        if positions is None:
+        if centers is None:
             calculate_all = True
             indices = np.arange(len(system))
         else:
-            indices = positions
+            indices = centers
 
         # If periodicity is not requested, and the output is requested for all
         # atoms, we skip all the intricate optimizations that will make things
         # actually slower for this case.
         if calculate_all and not self.periodic:
             n_atoms = len(system)
             all_pos = system.get_positions()
             dmat = dscribe.utils.geometry.get_adjacency_matrix(
-                self.rcut, all_pos, all_pos
+                self.r_cut, all_pos, all_pos
             )
         # Otherwise the amount of pairwise distances that are calculated is
         # kept at minimum. Only distances for the given indices (and possibly
         # the secondary neighbours if G4 is specified) are calculated.
         else:
             # Create the extended system if periodicity is requested. For ACSF only
             # the distance from central atom needs to be considered in extending
             # the system.
             if self.periodic:
                 system = dscribe.utils.geometry.get_extended_system(
-                    system, self.rcut, return_cell_indices=False
+                    system, self.r_cut, return_cell_indices=False
                 )
 
             # First calculate distances from specified centers to all other
             # atoms. This is already enough for everything else except G4.
             n_atoms = len(system)
             all_pos = system.get_positions()
             central_pos = all_pos[indices]
             dmat_primary = dscribe.utils.geometry.get_adjacency_matrix(
-                self.rcut, central_pos, all_pos
+                self.r_cut, central_pos, all_pos
             )
 
             # Create symmetric full matrix
             col = dmat_primary.col
             row = [
                 indices[x] for x in dmat_primary.row
             ]  # Fix row numbering to refer to original system
@@ -243,15 +240,15 @@
             dmat_lil[col, row] = dmat_lil[row, col]
 
             # If G4 terms are requested, calculate also secondary neighbour distances
             if len(self.g4_params) != 0:
                 neighbour_indices = np.unique(col)
                 neigh_pos = all_pos[neighbour_indices]
                 dmat_secondary = dscribe.utils.geometry.get_adjacency_matrix(
-                    self.rcut, neigh_pos, neigh_pos
+                    self.r_cut, neigh_pos, neigh_pos
                 )
                 col = [
                     neighbour_indices[x] for x in dmat_secondary.col
                 ]  # Fix col numbering to refer to original system
                 row = [
                     neighbour_indices[x] for x in dmat_secondary.row
                 ]  # Fix row numbering to refer to original system
@@ -271,24 +268,17 @@
             self.acsf_wrapper.create(
                 system.get_positions(),
                 system.get_atomic_numbers(),
                 dmat_dense,
                 neighbours,
                 indices,
             ),
-            dtype=np.float32,
+            dtype=np.float64,
         )
 
-        # Check if there are types that have not been declared
-        self.check_atomic_numbers(system.get_atomic_numbers())
-
-        # Return sparse matrix if requested
-        if self._sparse:
-            output = sparse.COO.from_numpy(output)
-
         return output
 
     def get_number_of_features(self):
         """Used to inquire the final number of features that this descriptor
         will have.
 
         Returns:
@@ -296,14 +286,21 @@
         """
         wrapper = self.acsf_wrapper
         descsize = (1 + wrapper.n_g2 + wrapper.n_g3) * wrapper.n_types
         descsize += (wrapper.n_g4 + wrapper.n_g5) * wrapper.n_type_pairs
 
         return int(descsize)
 
+    def validate_derivatives_method(self, method, attach):
+        if not attach:
+            raise ValueError(
+                "ACSF derivatives can only be calculated with attach=True."
+            )
+        return super().validate_derivatives_method(method, attach)
+
     @property
     def species(self):
         return self._species
 
     @species.setter
     def species(self, value):
         """Used to check the validity of given atomic numbers and to initialize
@@ -314,19 +311,19 @@
                 numbers or list of chemical symbols.
         """
         # The species are stored as atomic numbers for internal use.
         self._set_species(value)
         self.acsf_wrapper.atomic_numbers = self._atomic_numbers.tolist()
 
     @property
-    def rcut(self):
+    def r_cut(self):
         return self.acsf_wrapper.rcut
 
-    @rcut.setter
-    def rcut(self, value):
+    @r_cut.setter
+    def r_cut(self, value):
         """Used to check the validity of given radial cutoff.
 
         Args:
             value(float): Radial cutoff.
         """
         if value <= 0:
             raise ValueError("Cutoff radius should be positive.")
@@ -344,15 +341,15 @@
             value(n*3 array): List of G2 parameters.
         """
         # Disable case
         if value is None:
             value = np.array([])
         else:
             # Check dimensions
-            value = np.array(value, dtype=np.float)
+            value = np.array(value, dtype=np.float64)
             if value.ndim != 2:
                 raise ValueError(
                     "g2_params should be a matrix with two columns (eta, Rs)."
                 )
             if value.shape[1] != 2:
                 raise ValueError(
                     "g2_params should be a matrix with two columns (eta, Rs)."
@@ -377,15 +374,15 @@
             value(array): List of G3 parameters.
         """
         # Handle the disable case
         if value is None:
             value = np.array([])
         else:
             # Check dimensions
-            value = np.array(value, dtype=np.float)
+            value = np.array(value, dtype=np.float64)
             if value.ndim != 1:
                 raise ValueError("g3_params should be a vector.")
 
         self.acsf_wrapper.g3_params = value.tolist()
 
     @property
     def g4_params(self):
@@ -400,15 +397,15 @@
             value(n*3 array): List of G4 parameters.
         """
         # Handle the disable case
         if value is None:
             value = np.array([])
         else:
             # Check dimensions
-            value = np.array(value, dtype=np.float)
+            value = np.array(value, dtype=np.float64)
             if value.ndim != 2:
                 raise ValueError(
                     "g4_params should be a matrix with three columns (eta, zeta, lambda)."
                 )
             if value.shape[1] != 3:
                 raise ValueError(
                     "g4_params should be a matrix with three columns (eta, zeta, lambda)."
@@ -433,15 +430,15 @@
             value(n*3 array): List of G5 parameters.
         """
         # Handle the disable case
         if value is None:
             value = np.array([])
         else:
             # Check dimensions
-            value = np.array(value, dtype=np.float)
+            value = np.array(value, dtype=np.float64)
             if value.ndim != 2:
                 raise ValueError(
                     "g5_params should be a matrix with three columns (eta, zeta, lambda)."
                 )
             if value.shape[1] != 3:
                 raise ValueError(
                     "g5_params should be a matrix with three columns (eta, zeta, lambda)."
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/coulombmatrix.py` & `dscribe-2.0.0/dscribe/descriptors/descriptorlocal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,220 +1,92 @@
 # -*- coding: utf-8 -*-
 """Copyright 2019 DScribe developers
-
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
-
     http://www.apache.org/licenses/LICENSE-2.0
-
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import numpy as np
-
+import sparse as sp
 from ase import Atoms
-import ase.geometry.cell
 
-import sparse
-
-from dscribe.core import System
-from dscribe.descriptors.matrixdescriptor import MatrixDescriptor
+from dscribe.descriptors.descriptor import Descriptor
 from dscribe.utils.dimensionality import is1d
 
-import dscribe.ext
-
-
-class CoulombMatrix(MatrixDescriptor):
-    """Calculates the zero padded Coulomb matrix.
-
-    The Coulomb matrix is defined as:
-
-        C_ij = 0.5 Zi**exponent, when i = j
-             = (Zi*Zj)/(Ri-Rj), when i != j
-
-    The matrix is padded with invisible atoms, which means that the matrix is
-    padded with zeros until the maximum allowed size defined by n_max_atoms is
-    reached.
-
-    To reach invariance against permutation of atoms, specify a valid option
-    for the permutation parameter.
-
-    For reference, see:
-        "Fast and Accurate Modeling of Molecular Atomization Energies with
-        Machine Learning", Matthias Rupp, Alexandre Tkatchenko, Klaus-Robert
-        Mueller, and O.  Anatole von Lilienfeld, Phys. Rev. Lett, (2012),
-        https://doi.org/10.1103/PhysRevLett.108.058301
-    and
-        "Learning Invariant Representations of Molecules for Atomization Energy
-        Prediction", Gregoire Montavon et. al, Advances in Neural Information
-        Processing Systems 25 (NIPS 2012)
-    """
-
-    def __init__(
-        self,
-        n_atoms_max,
-        permutation="sorted_l2",
-        sigma=None,
-        seed=None,
-        sparse=False,
-        flatten=True,
-    ):
-        super().__init__(
-            n_atoms_max,
-            permutation,
-            sigma,
-            seed,
-            flatten,
-            sparse,
-        )
-        self.wrapper = dscribe.ext.CoulombMatrix(
-            n_atoms_max,
-            permutation,
-            0 if sigma is None else sigma,
-            0 if seed is None else seed,
-        )
-
-    def create(self, system, n_jobs=1, only_physical_cores=False, verbose=False):
-        """Return the Coulomb matrix for the given systems.
-
-        Args:
-            system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
-                many atomic structures.
-            n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
-                the calculation across samples. Defaults to serial calculation
-                with n_jobs=1. If a negative number is given, the used cpus
-                will be calculated with, n_cpus + n_jobs, where n_cpus is the
-                amount of CPUs as reported by the OS. With only_physical_cores
-                you can control which types of CPUs are counted in n_cpus.
-            only_physical_cores (bool): If a negative n_jobs is given,
-                determines which types of CPUs are used in calculating the
-                number of jobs. If set to False (default), also virtual CPUs
-                are counted.  If set to True, only physical CPUs are counted.
-            verbose(bool): Controls whether to print the progress of each job
-                into to the console.
-
-        Returns:
-            np.ndarray | sparse.COO: Coulomb matrix for the given systems. The
-            return type depends on the 'sparse'-attribute. The first dimension
-            is determined by the amount of systems.
-        """
-        # Combine input arguments / check input validity
-        system = [system] if isinstance(system, Atoms) else system
-        for s in system:
-            if len(s) > self.n_atoms_max:
-                raise ValueError(
-                    "One of the given systems has more atoms ({}) than allowed "
-                    "by n_atoms_max ({}).".format(len(s), self.n_atoms_max)
-                )
-        inp = [(i_sys,) for i_sys in system]
-
-        # Create in parallel
-        output = self.create_parallel(
-            inp,
-            self.create_single,
-            n_jobs,
-            [self.get_number_of_features()],
-            only_physical_cores,
-            verbose=verbose,
-        )
-
-        # Unflatten output if so requested
-        if not self.flatten and self.permutation != "eigenspectrum":
-            output = self.unflatten(output, system)
 
-        return output
+class DescriptorLocal(Descriptor):
+    """An abstract base class for all local descriptors."""
 
-    def create_single(self, system):
+    def __init__(self, periodic, sparse, dtype="float64", average="off"):
+        super().__init__(periodic=periodic, sparse=sparse, dtype=dtype)
+        self.average = average
+
+    def validate_derivatives_method(self, method, attach):
+        """Used to validate and determine the final method for calculating the
+        derivatives.
         """
-        Args:
-            system (:class:`ase.Atoms`): Input system.
-
-        Returns:
-            ndarray: The zero padded matrix as a flattened 1D array.
-        """
-        # Initialize output array in dense format.
-        out_des = np.zeros((self.get_number_of_features()), dtype=np.float64)
-
-        # Calculate with C++ extension
-        self.wrapper.create(
-            out_des,
-            system.get_positions(),
-            system.get_atomic_numbers(),
-            system.get_cell(),
-            system.get_pbc(),
-        )
-
-        # If a sparse matrix is requested, convert to sparse.COO
-        if self._sparse:
-            out_des = sparse.COO.from_numpy(out_des)
-
-        return out_des
-
-    def unflatten(self, output, systems):
-        n_systems = len(systems)
-        if self.sparse:
-            if n_systems != 1:
-                full = sparse.zeros(
-                    (n_systems, self.n_atoms_max, self.n_atoms_max), format="dok"
-                )
-                for i_sys, system in enumerate(systems):
-                    n_atoms = len(system)
-                    full[i_sys] = (
-                        output[i_sys]
-                        .reshape((self.n_atoms_max, self.n_atoms_max))
-                        .todense()
-                    )
-                full = full.to_coo()
-            else:
-                full = output.reshape((self.n_atoms_max, self.n_atoms_max))
-        else:
-            if n_systems != 1:
-                full = np.zeros((n_systems, self.n_atoms_max, self.n_atoms_max))
-                for i_sys, system in enumerate(systems):
-                    n_atoms = len(system)
-                    full[i_sys] = output[i_sys].reshape(
-                        (self.n_atoms_max, self.n_atoms_max)
-                    )
-            else:
-                full = output.reshape((self.n_atoms_max, self.n_atoms_max))
-        return full
+        methods = {"numerical", "auto"}
+        if method not in methods:
+            raise ValueError(
+                "Invalid method specified. Please choose from: {}".format(methods)
+            )
+        if method == "auto":
+            method = "numerical"
+        return method
 
     def derivatives(
         self,
         system,
+        centers=None,
         include=None,
         exclude=None,
         method="auto",
         return_descriptor=True,
+        attach=False,
         n_jobs=1,
         only_physical_cores=False,
         verbose=False,
     ):
-        """Return the descriptor derivatives for the given system(s).
+        """Return the descriptor derivatives for the given systems and given centers.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
                 many atomic structures.
+            centers (list): Centers where to calculate the descriptor. Can be
+                provided as cartesian positions or atomic indices. Also see the
+                "attach"-argument that controls the interperation of centers
+                given as atomic indices. If no centers are defined, the
+                descriptor output will be created for all atoms in the system.
+                When calculating descriptor for multiple systems, provide the
+                centers as a list for each system.
             include (list): Indices of atoms to compute the derivatives on.
                 When calculating descriptor for multiple systems, provide
                 either a one-dimensional list that if applied to all systems or
                 a two-dimensional list of indices. Cannot be provided together
                 with 'exclude'.
             exclude (list): Indices of atoms not to compute the derivatives on.
                 When calculating descriptor for multiple systems, provide
                 either a one-dimensional list that if applied to all systems or
                 a two-dimensional list of indices. Cannot be provided together
                 with 'include'.
-            method (str): The method for calculating the derivatives. Supports
-                'numerical' and 'auto'. Defaults to using 'auto' which corresponds
-                to the the most efficient available method.
+            method (str): The method for calculating the derivatives. Provide
+                either 'numerical', 'analytical' or 'auto'. If using 'auto',
+                the most efficient available method is automatically chosen.
+            attach (bool): Controls the behaviour of centers defined as
+                atomic indices. If True, the centers tied to an atomic index will
+                move together with the atoms with respect to which the derivatives
+                are calculated against. If False, centers defined as atomic
+                indices will be converted into cartesian locations that are
+                completely independent of the atom location during derivative
+                calculation.
             return_descriptor (bool): Whether to also calculate the descriptor
                 in the same function call. Notice that it typically is faster
                 to calculate both in one go.
             n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
                 the calculation across samples. Defaults to serial calculation
                 with n_jobs=1. If a negative number is given, the number of jobs
                 will be calculated with, n_cpus + n_jobs, where n_cpus is the
@@ -227,46 +99,62 @@
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             If return_descriptor is True, returns a tuple, where the first item
             is the derivative array and the second is the descriptor array.
             Otherwise only returns the derivatives array. The derivatives array
-            is a either a 3D or 4D array, depending on whether you have
+            is a either a 4D or 5D array, depending on whether you have
             provided a single or multiple systems. If the output shape for each
             system is the same, a single monolithic numpy array is returned.
-            For variable sized output (e.g. differently sized systems,different
-            number of included atoms), a regular python list is returned. The
-            dimensions are: [(n_systems,) n_atoms, 3, n_features]. The first
+            For variable sized output (e.g. differently sized systems,
+            different number of centers or different number of included atoms),
+            a regular python list is returned. The dimensions are:
+            [(n_systems,) n_centers, n_atoms, 3, n_features]. The first
             dimension goes over the different systems in case multiple were
-            given. The second dimension goes over the included atoms. The order
-            is same as the order of atoms in the given system. The third
-            dimension goes over the cartesian components, x, y and z. The
-            fourth dimension goes over the features in the default order.
+            given. The second dimension goes over the descriptor centers in
+            the same order as they were given in the argument. The third
+            dimension goes over the included atoms. The order is same as the
+            order of atoms in the given system. The fourth dimension goes over
+            the cartesian components, x, y and z. The fifth dimension goes over
+            the features in the default order.
         """
-        # Validate/determine the appropriate calculation method.
-        methods = {"numerical", "auto"}
-        if method not in methods:
-            raise ValueError(
-                "Invalid method specified. Please choose from: {}".format(methods)
+        method = self.validate_derivatives_method(method, attach)
+
+        # If single system given, skip the parallelization
+        if isinstance(system, Atoms):
+            n_atoms = len(system)
+            indices = self._get_indices(n_atoms, include, exclude)
+            return self.derivatives_single(
+                system,
+                centers,
+                indices,
+                method=method,
+                attach=attach,
+                return_descriptor=return_descriptor,
             )
-        if method == "auto":
-            method = "numerical"
 
         # Check input validity
-        system = [system] if isinstance(system, Atoms) else system
         n_samples = len(system)
+        if centers is None:
+            centers = [None] * n_samples
         if include is None:
             include = [None] * n_samples
         elif is1d(include, np.integer):
             include = [include] * n_samples
         if exclude is None:
             exclude = [None] * n_samples
         elif is1d(exclude, np.integer):
             exclude = [exclude] * n_samples
+        n_pos = len(centers)
+        if n_pos != n_samples:
+            raise ValueError(
+                "The given number of centers does not match the given "
+                "number of systems."
+            )
         n_inc = len(include)
         if n_inc != n_samples:
             raise ValueError(
                 "The given number of includes does not match the given "
                 "number of systems."
             )
         n_exc = len(exclude)
@@ -282,26 +170,35 @@
             n_atoms = len(sys)
             indices.append(self._get_indices(n_atoms, inc, exc))
 
         # Combine input arguments
         inp = list(
             zip(
                 system,
+                centers,
                 indices,
                 [method] * n_samples,
+                [attach] * n_samples,
                 [return_descriptor] * n_samples,
             )
         )
 
-        # Determine a fixed output size if possible
+        # For the descriptor, the output size for each job depends on the exact arguments.
+        # Here we precalculate the size for each job to preallocate memory and
+        # make the process faster.
         n_features = self.get_number_of_features()
 
         def get_shapes(job):
-            n_indices = len(job[1])
-            return (n_indices, 3, n_features), (n_features,)
+            centers = job[1]
+            if centers is None:
+                n_centers = len(job[0])
+            else:
+                n_centers = 1 if self.average != "off" else len(centers)
+            n_indices = len(job[2])
+            return (n_centers, n_indices, 3, n_features), (n_centers, n_features)
 
         derivatives_shape, descriptor_shape = get_shapes(inp[0])
 
         def is_variable(inp):
             for job in inp[1:]:
                 i_der_shape, i_desc_shape = get_shapes(job)
                 if i_der_shape != derivatives_shape or i_desc_shape != descriptor_shape:
@@ -322,76 +219,155 @@
             return_descriptor,
             only_physical_cores,
             verbose=verbose,
         )
 
         return output
 
+    def init_descriptor_array(self, n_centers):
+        """Return a zero-initialized numpy array for the descriptor."""
+        n_features = self.get_number_of_features()
+        if self.average != "off":
+            c = np.zeros((1, n_features), dtype=np.float64)
+        else:
+            c = np.zeros((n_centers, n_features), dtype=np.float64)
+        return c
+
+    def init_derivatives_array(self, n_centers, n_indices):
+        """Return a zero-initialized numpy array for the derivatives."""
+        n_features = self.get_number_of_features()
+        if self.average != "off":
+            return np.zeros((1, n_indices, 3, n_features), dtype=np.float64)
+        else:
+            return np.zeros((n_centers, n_indices, 3, n_features), dtype=np.float64)
+
     def derivatives_single(
         self,
         system,
+        centers,
         indices,
         method="numerical",
+        attach=False,
         return_descriptor=True,
     ):
         """Return the derivatives for the given system.
-
         Args:
             system (:class:`ase.Atoms`): Atomic structure.
+            centers (list): Centers where to calculate SOAP. Can be
+                provided as cartesian positions or atomic indices. If no
+                centers are defined, the SOAP output will be created for all
+                atoms in the system. When calculating SOAP for multiple
+                systems, provide the centers as a list for each system.
             indices (list): Indices of atoms for which the derivatives will be
                 computed for.
             method (str): The method for calculating the derivatives. Supports
                 'numerical'.
+            attach (bool): Controls the behaviour of centers defined as
+                atomic indices. If True, the centers tied to an atomic index will
+                move together with the atoms with respect to which the derivatives
+                are calculated against. If False, centers defined as atomic
+                indices will be converted into cartesian locations that are
+                completely independent of the atom location during derivative
+                calculation.
             return_descriptor (bool): Whether to also calculate the descriptor
                 in the same function call. This is true by default as it
                 typically is faster to calculate both in one go.
-
         Returns:
             If return_descriptor is True, returns a tuple, where the first item
             is the derivative array and the second is the descriptor array.
             Otherwise only returns the derivatives array. The derivatives array
-            is a 3D numpy array. The dimensions are: [n_atoms, 3, n_features].
-            The first dimension goes over the included atoms. The order is same
-            as the order of atoms in the given system. The second dimension
-            goes over the cartesian components, x, y and z. The last dimension
-            goes over the features in the default order.
+            is a 4D numpy array. The dimensions are: [n_centers, n_atoms, 3,
+            n_features]. The first dimension goes over the SOAP centers in the
+            same order as they were given in the argument. The second dimension
+            goes over the included atoms. The order is same as the order of
+            atoms in the given system. The third dimension goes over the
+            cartesian components, x, y and z. The last dimension goes over the
+            features in the default order.
         """
-        pos = system.get_positions()
-        Z = system.get_atomic_numbers()
-        sorted_species = self._atomic_numbers
         n_indices = len(indices)
+        n_centers = len(system) if centers is None else len(centers)
 
         # Initialize numpy arrays for storing the descriptor and derivatives.
-        n_features = self.get_number_of_features()
         if return_descriptor:
-            c = np.zeros(n_features)
+            c = self.init_descriptor_array(n_centers)
         else:
             c = np.empty(0)
-        d = np.zeros((n_indices, 3, n_features), dtype=np.float64)
+        d = self.init_derivatives_array(n_centers, n_indices)
 
         # Calculate numerically with extension
         if method == "numerical":
-            self.wrapper.derivatives_numerical(
-                d,
-                c,
-                pos,
-                Z,
-                ase.geometry.cell.complete_cell(system.get_cell()),
-                np.asarray(system.get_pbc(), dtype=bool),
-                indices,
-                return_descriptor,
+            self.derivatives_numerical(
+                d, c, system, centers, indices, attach, return_descriptor
+            )
+        elif method == "analytical":
+            self.derivatives_analytical(
+                d, c, system, centers, indices, attach, return_descriptor
             )
 
-        # Convert to the final output precision.
-        if self.dtype == "float32":
-            d = d.astype(self.dtype)
-            c = c.astype(self.dtype)
-
-        # Convert to sparse here. Currently everything up to this point is
-        # calculated with dense matrices. This imposes some memory limitations.
-        if self.sparse:
-            d = sp.COO.from_numpy(d)
-            c = sp.COO.from_numpy(c)
+        d = self.format_array(d)
+        c = self.format_array(c)
 
         if return_descriptor:
             return (d, c)
         return d
+
+    def derivatives_numerical(
+        self,
+        d,
+        c,
+        system,
+        centers,
+        indices,
+        attach=False,
+        return_descriptor=True,
+    ):
+        """Return the numerical derivatives for the given system. This is the
+        default numerical implementation with python. You should overwrite this
+        with a more optimized method whenever possible.
+
+        Args:
+            d (np.array): The derivatives array.
+            c (np.array): The descriptor array.
+            system (:class:`ase.Atoms`): Atomic structure.
+            centers (list): Centers where to calculate SOAP. Can be
+                provided as cartesian positions or atomic indices. If no
+                centers are defined, the SOAP output will be created for all
+                atoms in the system. When calculating SOAP for multiple
+                systems, provide the centers as a list for each system.
+            indices (list): Indices of atoms for which the derivatives will be
+                computed for.
+            attach (bool): Controls the behaviour of centers defined as
+                atomic indices. If True, the centers tied to an atomic index will
+                move together with the atoms with respect to which the derivatives
+                are calculated against. If False, centers defined as atomic
+                indices will be converted into cartesian locations that are
+                completely independent of the atom location during derivative
+                calculation.
+            return_descriptor (bool): Whether to also calculate the descriptor
+                in the same function call. This is true by default as it
+                typically is faster to calculate both in one go.
+        """
+        h = 0.0001
+        coeffs = [-1.0 / 2.0, 1.0 / 2.0]
+        deltas = [-1.0, 1.0]
+        if centers is None:
+            centers = range(len(system))
+        if not attach and np.issubdtype(type(centers[0]), np.integer):
+            centers = system.get_positions()[centers]
+
+        for index, i_atom in enumerate(indices):
+            for i_center, center in enumerate(centers):
+                for i_comp in range(3):
+                    for i_stencil in range(2):
+                        system_disturbed = system.copy()
+                        i_pos = system_disturbed.get_positions()
+                        i_pos[i_atom, i_comp] += h * deltas[i_stencil]
+                        system_disturbed.set_positions(i_pos)
+                        d1 = self.create_single(system_disturbed, [center])
+                        d[i_center, index, i_comp, :] += (
+                            coeffs[i_stencil] * d1[0, :] / h
+                        )
+            index += 1
+
+        if return_descriptor:
+            d0 = self.create_single(system, centers)
+            np.copyto(c, d0)
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/descriptor.py` & `dscribe-2.0.0/dscribe/descriptors/descriptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,33 +15,37 @@
 """
 from abc import ABC, abstractmethod
 
 import numpy as np
 
 import sparse as sp
 
-from ase import Atoms
-from dscribe.core.system import System
 from dscribe.utils.species import get_atomic_numbers
 
 import joblib
 from joblib import Parallel, delayed
 
 
 class Descriptor(ABC):
     """An abstract base class for all descriptors."""
 
-    def __init__(self, periodic, flatten, sparse, dtype="float64"):
+    def __init__(self, periodic, sparse, dtype="float64"):
         """
         Args:
-            flatten (bool): Whether the output of create() should be flattened
-                to a 1D array.
+            periodic (bool): Whether the descriptor should take PBC into account.
+            sparse (bool): Whether the output should use a sparse format.
+            dtype (str): The output data type.
         """
+        supported_dtype = set(("float32", "float64"))
+        if dtype not in supported_dtype:
+            raise ValueError(
+                "Invalid output data type '{}' given. Please use "
+                "one of the following: {}".format(dtype, supported_dtype)
+            )
         self.sparse = sparse
-        self.flatten = flatten
         self.periodic = periodic
         self.dtype = dtype
         self._atomic_numbers = None
         self._atomic_number_set = None
         self._species = None
 
     @abstractmethod
@@ -62,14 +66,27 @@
         """Used to inquire the final number of features that this descriptor
         will have.
 
         Returns:
             int: Number of features for this descriptor.
         """
 
+    def validate_derivatives_method(self, method):
+        """Used to validate and determine the final method for calculating the
+        derivatives.
+        """
+        methods = {"numerical", "auto"}
+        if method not in methods:
+            raise ValueError(
+                "Invalid method specified. Please choose from: {}".format(methods)
+            )
+        if method == "auto":
+            method = "numerical"
+        return method
+
     @property
     def sparse(self):
         return self._sparse
 
     @sparse.setter
     def sparse(self, value):
         """Sets whether the output should be sparse or not.
@@ -88,27 +105,14 @@
         """Sets whether the inputs should be considered periodic or not.
 
         Args:
             value(float): Are the systems periodic.
         """
         self._periodic = value
 
-    @property
-    def flatten(self):
-        return self._flatten
-
-    @flatten.setter
-    def flatten(self, value):
-        """Sets whether the output should be flattened or not.
-
-        Args:
-            value(float): Should the output be flattened.
-        """
-        self._flatten = value
-
     def _set_species(self, species):
         """Used to setup the species information for this descriptor. This
         information includes an ordered list of unique atomic numbers, a set
         of atomic numbers and the original variable contents.
 
         Args:
             species(iterable): Chemical species either as a list of atomic
@@ -136,14 +140,25 @@
         zs = set(atomic_numbers)
         if not zs.issubset(self._atomic_number_set):
             raise ValueError(
                 "The following atomic numbers are not defined "
                 "for this descriptor: {}".format(zs.difference(self._atomic_number_set))
             )
 
+    def format_array(self, input):
+        """Used to format a float64 numpy array in the final format that will be
+        returned to the user.
+        """
+        if self.dtype != "float64":
+            input = input.astype(self.dtype)
+        if self.sparse:
+            input = sp.COO.from_numpy(input)
+
+        return input
+
     def create_parallel(
         self,
         inp,
         func,
         n_jobs,
         static_size=None,
         only_physical_cores=False,
@@ -192,15 +207,15 @@
         Returns:
             np.ndarray | sparse.COO | list: The descriptor output
             for each given input. The return type depends on the desciptor
             setup.
         """
         # If single system given, skip the parallelization overhead
         if len(inp) == 1:
-            return func(*inp[0])
+            return self.format_array(func(*inp[0]))
 
         # Determine the number of jobs
         if n_jobs < 0:
             n_jobs = joblib.cpu_count(only_physical_cores) + n_jobs
         if n_jobs <= 0:
             raise ValueError("Invalid number of jobs specified.")
 
@@ -230,14 +245,15 @@
 
             i_sample = 0
             old_percent = 0
             n_samples = len(arguments)
 
             for i_sample, i_arg in enumerate(arguments):
                 i_out = func(*i_arg)
+                i_out = self.format_array(i_out)
 
                 # If the shape varies, just add result into a list
                 if static_size is None:
                     results.append(i_out)
                 else:
                     if is_sparse:
                         sample_index = np.full((1, i_out.data.size), i_sample)
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/ewaldsummatrix.py` & `dscribe-2.0.0/dscribe/descriptors/ewaldsummatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,19 @@
 
 import numpy as np
 
 from ase import Atoms
 
 from scipy.special import erfc
 
-from dscribe.core import System
-from dscribe.descriptors.matrixdescriptor import MatrixDescriptor
+from dscribe.descriptors.descriptormatrix import DescriptorMatrix
 from dscribe.core.lattice import Lattice
 
 
-class EwaldSumMatrix(MatrixDescriptor):
+class EwaldSumMatrix(DescriptorMatrix):
     """
     Calculates an Ewald sum matrix for the a given system.
 
     Each entry M_ij of the Ewald sum matrix will contain the Coulomb energy
     between atoms i and j calculated with the Ewald summation method. In the
     Ewald method a constant neutralizing background charge has been added to
     counteract the positive net charge.
@@ -68,17 +67,14 @@
         w=1,
         r_cut=None,
         g_cut=None,
         a=None,
         n_jobs=1,
         only_physical_cores=False,
         verbose=False,
-        # For backwards compatibility with < v1.2.2
-        rcut=None,
-        gcut=None,
     ):
         """Return the Ewald sum matrix for the given systems.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
                 many atomic structures.
             accuracy (float): The accuracy to which the sum is converged to.
@@ -114,18 +110,16 @@
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             np.ndarray | sparse.COO: Ewald sum matrix for the given systems.
-            The return type depends on the 'sparse' and 'flatten'-attributes.
-            For flattened output a single numpy array or sparse.COO is
-            returned. The first dimension is determined by the amount of
-            systems.
+            The return type depends on the 'sparse'-attribute. The first
+            dimension is determined by the amount of systems.
         """
         var_dict = {}
         for var_new in ["r_cut", "g_cut"]:
             loc = locals()
             var_old = "".join(var_new.split("_"))
             if loc.get(var_old) is not None:
                 var_dict[var_new] = loc[var_old]
@@ -164,20 +158,15 @@
             for i_sys, i_accuracy, i_w, i_r_cut, i_g_cut, i_a in zip(
                 system, accuracy, w, r_cut, g_cut, a
             )
         ]
 
         # Determine if the outputs have a fixed size
         n_features = self.get_number_of_features()
-        if self._flatten:
-            static_size = [n_features]
-        elif self.permutation == "eigenspectrum":
-            static_size = [self.n_atoms_max]
-        else:
-            static_size = [self.n_atoms_max, self.n_atoms_max]
+        static_size = [n_features]
 
         # Create in parallel
         output = self.create_parallel(
             inp,
             self.create_single,
             n_jobs,
             static_size,
@@ -315,15 +304,14 @@
         ereal = np.zeros((n_atoms, n_atoms), dtype=np.float64)
         lattice = Lattice(system.get_cell())
 
         # For each atom in the original cell, get the neighbours in the
         # infinite system within the real space cutoff and calculate the real
         # space portion of the Ewald sum.
         for i in range(n_atoms):
-
             # Get points that are within the real space cutoff
             nfcoords, rij, js = lattice.get_points_in_sphere(
                 fcoords, coords[i], self.r_cut, zip_results=False
             )
             # Remove the rii term, because a charge does not interact with
             # itself (but does interact with copies of itself).
             mask = rij > 1e-8
@@ -383,15 +371,14 @@
         factors = np.divide(expvals, g2s)
         charges = self.q
 
         # Create array where q_2[i,j] is qi * qj
         qiqj = charges[None, :] * charges[:, None]
 
         for gr, factor in zip(grs, factors):
-
             # Uses the identity sin(x)+cos(x) = 2**0.5 sin(x + pi/4)
             m = (gr[None, :] + math.pi / 4) - gr[:, None]
             np.sin(m, m)
             m *= factor
             erecip += m
 
         erecip *= 4 * math.pi / self.volume * qiqj * 2**0.5
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/lmbtr.py` & `dscribe-2.0.0/dscribe/descriptors/lmbtr.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,216 +11,291 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
 import math
-import numpy as np
 
+import numpy as np
+import scipy.spatial.distance
 from sklearn.preprocessing import normalize
-
-from scipy.sparse import lil_matrix
 import sparse
-
-import scipy.spatial.distance
-
 from ase import Atoms
 import ase.data
 
 from dscribe.core import System
-from dscribe.descriptors import MBTR
+from dscribe.descriptors.mbtr import (
+    check_geometry,
+    check_weighting,
+    check_grid,
+    k1_geometry_functions,
+)
+from dscribe.descriptors.descriptorlocal import DescriptorLocal
 from dscribe.ext import MBTRWrapper
 import dscribe.utils.geometry
 
 
-class LMBTR(MBTR):
-    """Implementation of local -- per chosen atom -- kind of the Many-body
-    tensor representation up to k=3.
+class LMBTR(DescriptorLocal):
+    """
+    Implementation of the Local Many-body tensor representation.
+
+    You can use this descriptor for finite and periodic systems. When dealing
+    with periodic systems or when using machine learning models that use the
+    Euclidean norm to measure distance between vectors, it is advisable to use
+    some form of normalization. This implementation does not support the use of
+    a non-identity correlation matrix.
 
     Notice that the species of the central atom is not encoded in the output,
     but is instead represented by a chemical species X with atomic number 0.
     This allows LMBTR to be also used on general positions not corresponding to
     real atoms. The surrounding environment is encoded by the two- and
     three-body interactions with neighouring atoms. If there is a need to
-    distinguish the central species, one can for example train a different
-    model for each central species.
-
-    You can choose which terms to include by providing a dictionary in the k2
-    or k3 arguments. The k1 term is not used in the local version. This
-    dictionary should contain information under three keys: "geometry", "grid"
-    and "weighting". See the examples below for how to format these
-    dictionaries.
-
-    You can use this descriptor for finite and periodic systems. When dealing
-    with periodic systems or when using machine learning models that use the
-    Euclidean norm to measure distance between vectors, it is advisable to use
-    some form of normalization.
-
-    For the geometry functions the following choices are available:
-
-    * :math:`k=2`:
-
-       * "distance": Pairwise distance in angstroms.
-       * "inverse_distance": Pairwise inverse distance in 1/angstrom.
-
-    * :math:`k=3`:
-
-       * "angle": Angle in degrees.
-       * "cosine": Cosine of the angle.
-
-    For the weighting the following functions are available:
-
-    * :math:`k=2`:
-
-       * "unity": No weighting.
-       * "exp": Weighting of the form :math:`e^{-sx}`
-
-    * :math:`k=3`:
-
-       * "unity": No weighting.
-       * "exp": Weighting of the form :math:`e^{-sx}`
-
-    The exponential weighting is motivated by the exponential decay of screened
-    Coulombic interactions in solids. In the exponential weighting the
-    parameters **threshold** determines the value of the weighting function after
-    which the rest of the terms will be ignored and the parameter **scale**
-    corresponds to :math:`s`. The meaning of :math:`x` changes for different
-    terms as follows:
-
-    * :math:`k=2`: :math:`x` = Distance between A->B
-    * :math:`k=3`: :math:`x` = Distance from A->B->C->A.
-
-    In the grid setup *min* is the minimum value of the axis, *max* is the
-    maximum value of the axis, *sigma* is the standard deviation of the
-    gaussian broadening and *n* is the number of points sampled on the
-    grid.
-
-    If flatten=False, a list of dense np.ndarrays for each k in ascending order
-    is returned. These arrays are of dimension (n_elements x n_elements x
-    n_grid_points), where the elements are sorted in ascending order by their
-    atomic number.
-
-    If flatten=True, a sparse.COO is returned. This sparse matrix
-    is of size (n_features,), where n_features is given by
-    get_number_of_features(). This vector is ordered so that the different
-    k-terms are ordered in ascending order, and within each k-term the
-    distributions at each entry (i, j, h) of the tensor are ordered in an
-    ascending order by (i * n_elements) + (j * n_elements) + (h * n_elements).
-
-    This implementation does not support the use of a non-identity correlation
-    matrix.
+    distinguish the central species, one can for example train a different model
+    for each central species.
     """
 
     def __init__(
         self,
-        k2=None,
-        k3=None,
+        geometry=None,
+        grid=None,
+        weighting=None,
         normalize_gaussians=True,
         normalization="none",
-        flatten=True,
         species=None,
         periodic=False,
         sparse=False,
+        dtype="float64",
     ):
         """
         Args:
+            geometry (dict): Setup the geometry function.
+                For example::
+
+                "geometry": {"function": "distance"}
+
+                The geometry function determines the degree :math:`k` for MBTR.
+                The order :math:`k` tells how many atoms are involved in the
+                calculation and thus also heavily influence the computational
+                time.
+
+                The following geometry functions are available:
+
+                * :math:`k=2`
+                    * ``"distance"``: Pairwise distance in angstroms.
+                    * ``"inverse_distance"``: Pairwise inverse distance in 1/angstrom.
+                * :math:`k=3`
+                    * ``"angle"``: Angle in degrees.
+                    * ``"cosine"``: Cosine of the angle.
+
+            grid (dict): Setup the discretization grid.
+                For example::
+
+                "grid": {"min": 0.1, "max": 2, "sigma": 0.1, "n": 50}
+
+                In the grid setup *min* is the minimum value of the axis, *max*
+                is the maximum value of the axis, *sigma* is the standard
+                deviation of the gaussian broadening and *n* is the number of
+                points sampled on the grid.
+
+            weighting (dict): Setup the weighting function and its parameters.
+                For example::
+
+                "weighting" : {"function": "exp", "r_cut": 10, "threshold": 1e-3}
+
+                The following weighting functions are available:
+
+                * :math:`k=2`
+                    * ``"unity"``: No weighting.
+                    * ``"exp"``: Weighting of the form :math:`e^{-sx}`
+                    * ``"inverse_square"``: Weighting of the form :math:`1/(x^2)`
+                * :math:`k=3`
+                    * ``"unity"``: No weighting.
+                    * ``"exp"``: Weighting of the form :math:`e^{-sx}`
+                    * ``"smooth_cutoff"``: Weighting of the form :math:`f_{ij}f_{ik}`,
+                        where :math:`f = 1+y(x/r_{cut})^{y+1}-(y+1)(x/r_{cut})^{y}`
+
+                The meaning of :math:`x` changes for different terms as follows:
+
+                * For :math:`k=2`: :math:`x` = Distance between A->B
+                * For :math:`k=3`: :math:`x` = Distance from A->B->C->A.
+
+                The exponential weighting is motivated by the exponential decay
+                of screened Coulombic interactions in solids. In the exponential
+                weighting the parameters **threshold** determines the value of
+                the weighting function after which the rest of the terms will be
+                ignored. Either the parameter **scale** or **r_cut** can be used
+                to determine the parameter :math:`s`: **scale** directly
+                corresponds to this value whereas **r_cut** can be used to
+                indirectly determine it through :math:`s=-\log()`:.
+
+                The inverse square and smooth cutoff function weightings use a
+                cutoff parameter **r_cut**, which is a radial distance after
+                which the rest of the atoms will be ignored. For the smooth
+                cutoff function, additional weighting key **sharpness** can be
+                added, which changes the value of :math:`y`. If a value for it
+                is not provided, it defaults to `2`.
+
+            normalize_gaussians (bool): Determines whether the gaussians are
+                normalized to an area of 1. Defaults to True. If False, the
+                normalization factor is dropped and the gaussians have the form.
+                :math:`e^{-(x-\mu)^2/2\sigma^2}`
+            normalization (str): Determines the method for normalizing the
+                output. The available options are:
+
+                * ``"none"``: No normalization.
+                * ``"l2"``: Normalize the Euclidean length of the output to unity.
             species (iterable): The chemical species as a list of atomic
                 numbers or as a list of chemical symbols. Notice that this is not
                 the atomic numbers that are present for an individual system, but
                 should contain all the elements that are ever going to be
                 encountered when creating the descriptors for a set of systems.
                 Keeping the number of chemical speices as low as possible is
                 preferable.
             periodic (bool): Set to true if you want the descriptor output to
                 respect the periodicity of the atomic systems (see the
                 pbc-parameter in the constructor of ase.Atoms).
-            k2 (dict): Dictionary containing the setup for the k=2 term.
-                Contains setup for the used geometry function, discretization and
-                weighting function. For example::
-
-                    k2 = {
-                        "geometry": {"function": "inverse_distance"},
-                        "grid": {"min": 0.1, "max": 2, "sigma": 0.1, "n": 50},
-                        "weighting": {"function": "exp", "scale": 0.75, "threshold": 1e-2}
-                    }
-
-            k3 (dict): Dictionary containing the setup for the k=3 term.
-                Contains setup for the used geometry function, discretization and
-                weighting function. For example::
-
-                    k3 = {
-                        "geometry": {"function": "angle"},
-                        "grid": {"min": 0, "max": 180, "sigma": 5, "n": 50},
-                        "weighting" = {"function": "exp", "scale": 0.5, "threshold": 1e-3}
-                    }
-            normalize_gaussians (bool): Determines whether the gaussians are
-                normalized to an area of 1. Defaults to True. If False, the
-                normalization factor is dropped and the gaussians have the form.
-                :math:`e^{-(x-\mu)^2/2\sigma^2}`
-            normalization (str): Determines the method for normalizing the
-                output. The available options are:
-
-                * "none": No normalization.
-                * "l2_each": Normalize the Euclidean length of each k-term
-                  individually to unity.
-
-            flatten (bool): Whether the output should be flattened to a 1D
-                array. If False, a dictionary of the different tensors is
-                provided, containing the values under keys: "k1", "k2", and
-                "k3":
             sparse (bool): Whether the output should be a sparse matrix or a
                 dense numpy array.
+            dtype (str): The data type of the output. Valid options are:
+
+                    * ``"float32"``: Single precision floating point numbers.
+                    * ``"float64"``: Double precision floating point numbers.
         """
         super().__init__(
-            k1=None,
-            k2=k2,
-            k3=k3,
             periodic=periodic,
-            species=species,
-            normalization=normalization,
-            normalize_gaussians=normalize_gaussians,
-            flatten=flatten,
             sparse=sparse,
+            dtype=dtype,
         )
+        self.system = None
+        self.geometry = geometry
+        self.grid = grid
+        self.weighting = weighting
+        self.species = species
+        self.normalization = normalization
+        self.normalize_gaussians = normalize_gaussians
+
+        if self.normalization == "valle_oganov" and not periodic:
+            raise ValueError(
+                "Valle-Oganov normalization does not support non-periodic systems."
+            )
+
+        # Initializing .create() level variables
+        self._interaction_limit = None
+
+    @property
+    def grid(self):
+        return self._grid
+
+    @grid.setter
+    def grid(self, value):
+        check_grid(value)
+        self._grid = value
+
+    @property
+    def geometry(self):
+        return self._geometry
+
+    @geometry.setter
+    def geometry(self, value):
+        check_geometry(value)
+        if value["function"] in k1_geometry_functions:
+            raise ValueError(
+                "LMBTR does not support geometry functions for degree k=1."
+            )
+        k_map = {
+            "distance": 2,
+            "inverse_distance": 2,
+            "angle": 3,
+            "cosine": 3,
+        }
+        self.k = k_map[value["function"]]
+        self._geometry = value
+
+    @property
+    def weighting(self):
+        return self._weighting
+
+    @weighting.setter
+    def weighting(self, value):
+        check_weighting(self.k, value, self.periodic)
+        self._weighting = value
+
+    @property
+    def species(self):
+        return self._species
+
+    @species.setter
+    def species(self, value):
+        """Used to check the validity of given atomic numbers and to initialize
+        the C-memory layout for them.
+
+        Args:
+            value(iterable): Chemical species either as a list of atomic
+                numbers or list of chemical symbols.
+        """
+        # The species are stored as atomic numbers for internal use.
+        self._set_species(value)
+
+        # The atomic number 0 is reserved for ghost atoms in this
+        # implementation.
+        if 0 in self._atomic_number_set:
+            raise ValueError(
+                "The atomic number 0 is reserved for the ghost atoms in this "
+                "implementation."
+            )
+        self._atomic_number_set.add(0)
+        indices = np.searchsorted(self._atomic_numbers, 0)
+        self._atomic_numbers = np.insert(self._atomic_numbers, indices, 0)
+
+        # Setup mappings between atom indices and types together with some
+        # statistics
+        self.atomic_number_to_index = {}
+        self.index_to_atomic_number = {}
+        for i_atom, atomic_number in enumerate(self._atomic_numbers):
+            self.atomic_number_to_index[atomic_number] = i_atom
+            self.index_to_atomic_number[i_atom] = atomic_number
+        self.n_elements = len(self._atomic_numbers)
+        self.max_atomic_number = max(self._atomic_numbers)
+        self.min_atomic_number = min(self._atomic_numbers)
 
     @property
     def normalization(self):
         return self._normalization
 
     @normalization.setter
     def normalization(self, value):
         """Checks that the given normalization is valid. Overrides the
         normalization check from original MBTR because the normalization with
         respect to number of atoms is not valid for a local descriptor.
 
         Args:
             value(str): The normalization method to use.
         """
-        norm_options = set(("l2_each", "none"))
+        norm_options = set(("none", "l2"))
         if value not in norm_options:
             raise ValueError(
                 "Unknown normalization option given. Please use one of the "
-                "following: {}.".format(", ".join([str(x) for x in norm_options]))
+                "following: {}.".format(", ".join(sorted(list(norm_options))))
             )
         self._normalization = value
 
     def create(
-        self, system, positions=None, n_jobs=1, only_physical_cores=False, verbose=False
+        self, system, centers=None, n_jobs=1, only_physical_cores=False, verbose=False
     ):
-        """Return the LMBTR output for the given systems and given positions.
+        """Return the LMBTR output for the given systems and given centers.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
                 many atomic structures.
-            positions (list): Positions where to calculate LMBTR. Can be
+            centers (list): Centers where to calculate LMBTR. Can be
                 provided as cartesian positions or atomic indices. If no
-                positions are defined, the LMBTR output will be created for all
+                centers are defined, the LMBTR output will be created for all
                 atoms in the system. When calculating LMBTR for multiple
-                systems, provide the positions as a list for each system.
+                systems, provide the centers as a list for each system.
             n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
                 the calculation across samples. Defaults to serial calculation
                 with n_jobs=1. If a negative number is given, the used cpus
                 will be calculated with, n_cpus + n_jobs, where n_cpus is the
                 amount of CPUs as reported by the OS. With only_physical_cores
                 you can control which types of CPUs are counted in n_cpus.
             only_physical_cores (bool): If a negative n_jobs is given,
@@ -228,50 +303,50 @@
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             np.ndarray | scipy.sparse.csr_matrix: The LMBTR output for the given
-            systems and positions. The return type depends on the
+            systems and centers. The return type depends on the
             'sparse'-attribute. The first dimension is determined by the amount
-            of positions and systems and the second dimension is determined by
+            of centers and systems and the second dimension is determined by
             the get_number_of_features()-function.
         """
         # Combine input arguments
         if isinstance(system, Atoms):
             system = [system]
-            positions = [positions]
+            centers = [centers]
         n_samples = len(system)
-        if positions is None:
+        if centers is None:
             inp = [(i_sys,) for i_sys in system]
         else:
-            n_pos = len(positions)
+            n_pos = len(centers)
             if n_pos != n_samples:
                 raise ValueError(
-                    "The given number of positions does not match the given"
+                    "The given number of centers does not match the given"
                     "number of systems."
                 )
-            inp = list(zip(system, positions))
+            inp = list(zip(system, centers))
 
         # Determine if the outputs have a fixed size
         n_features = self.get_number_of_features()
         static_size = None
-        if positions is None:
+        if centers is None:
             n_centers = len(inp[0][0])
         else:
             first_sample, first_pos = inp[0]
             if first_pos is not None:
                 n_centers = len(first_pos)
             else:
                 n_centers = len(first_sample)
 
         def is_static():
             for i_job in inp:
-                if positions is None:
+                if centers is None:
                     if len(i_job[0]) != n_centers:
                         return False
                 else:
                     if i_job[1] is not None:
                         if len(i_job[1]) != n_centers:
                             return False
                     else:
@@ -293,32 +368,32 @@
         )
 
         return output
 
     def create_single(
         self,
         system,
-        positions=None,
+        centers=None,
     ):
         """Return the local many-body tensor representation for the given
-        system and positions.
+        system and centers.
 
         Args:
             system (:class:`ase.Atoms` | :class:`.System`): Input system.
-            positions (iterable): Positions or atom index of points, from
-                which local_mbtr is created. Can be a list of integer numbers
-                or a list of xyz-coordinates. If integers provided, the atoms
-                at that index are used as centers. If positions provided, new
-                atoms are added at that position. If no positions are provided,
-                all atoms in the system will be used as centers.
+            centers (iterable): Centers for which LMBTR is created. Can be
+                a list of integer numbers or a list of xyz-coordinates. If
+                integers provided, the atoms at that index are used as centers.
+                If cartesian positions are provided, new atoms are added at that
+                position. If no centers are provided, all atoms in the system
+                will be used as centers.
 
         Returns:
             1D ndarray: The local many-body tensor representations of given
-            positions, for k terms, as an array. These are ordered as given in
-            positions.
+            centers, for k terms, as an array. These are ordered as given in
+            centers.
         """
         # Check that the system does not have elements that are not in the list
         # of atomic numbers
         atomic_number_set = set(system.get_atomic_numbers())
         self.check_atomic_numbers(atomic_number_set)
         self._interaction_limit = len(system)
         system_positions = system.get_positions()
@@ -327,139 +402,106 @@
         # Ensure that the atomic number 0 is not present in the system
         if 0 in atomic_number_set:
             raise ValueError(
                 "Please do not use the atomic number 0 in local MBTR as it "
                 "is reserved to mark the atoms use as analysis centers."
             )
 
-        # Form a list of indices, positions and atomic numbers for the local
+        # Form a list of indices, centers and atomic numbers for the local
         # centers. k=3 and k=2 use a slightly different approach, so two
         # versions are built
         i_new = len(system)
         indices_k2 = []
         new_pos_k2 = []
         new_atomic_numbers_k2 = []
         indices_k3 = []
         new_pos_k3 = []
         new_atomic_numbers_k3 = []
         n_atoms = len(system)
-        if positions is not None:
-            n_loc = len(positions)
-
-            # Check validity of position definitions and create final cartesian
+        if centers is not None:
+            # Check validity of centers definitions and create final cartesian
             # position list
-            if len(positions) == 0:
+            if len(centers) == 0:
                 raise ValueError(
-                    "The argument 'positions' should contain a non-empty set of"
+                    "The argument 'centers' should contain a non-empty set of"
                     " atomic indices or cartesian coordinates with x, y and z "
                     "components."
                 )
-            for i in positions:
+            for i in centers:
                 if np.issubdtype(type(i), np.integer):
                     i_len = len(system)
                     if i >= i_len or i < 0:
                         raise ValueError(
                             "The provided index {} is not valid for the system "
                             "with {} atoms.".format(i, i_len)
                         )
                     indices_k2.append(i)
                     indices_k3.append(i)
                     new_pos_k2.append(system_positions[i])
                     new_atomic_numbers_k2.append(system_atomic_numbers[i])
                 elif isinstance(i, (list, tuple, np.ndarray)):
                     if len(i) != 3:
                         raise ValueError(
-                            "The argument 'positions' should contain a "
+                            "The argument 'centers' should contain a "
                             "non-empty set of atomic indices or cartesian "
                             "coordinates with x, y and z components."
                         )
                     new_pos_k2.append(np.array(i))
                     new_pos_k3.append(np.array(i))
                     new_atomic_numbers_k2.append(0)
                     new_atomic_numbers_k3.append(0)
                     i_new += 1
                 else:
                     raise ValueError(
-                        "Create method requires the argument 'positions', a "
+                        "Create method requires the argument 'centers', a "
                         "list of atom indices and/or positions."
                     )
-        # If positions are not supplied, it is assumed that each atom is used
+        # If centers are not supplied, it is assumed that each atom is used
         # as a center
         else:
-            n_loc = n_atoms
             indices_k2 = np.arange(n_atoms)
             indices_k3 = np.arange(n_atoms)
             new_pos_k2 = system.get_positions()
             new_atomic_numbers_k2 = system.get_atomic_numbers()
 
-        # Calculate the "raw" outputs for each term.
-        mbtr = {}
-        if self.k2 is not None:
-            new_system_k2 = System(
+        # Calculate the "raw" output
+        if self.k == 2:
+            new_system = System(
                 symbols=new_atomic_numbers_k2,
                 positions=new_pos_k2,
             )
-            mbtr["k2"] = self._get_k2(system, new_system_k2, indices_k2)
-
-        if self.k3 is not None:
-            new_system_k3 = System(
+            indices = indices_k2
+        elif self.k == 3:
+            new_system = System(
                 symbols=new_atomic_numbers_k3,
                 positions=new_pos_k3,
             )
-            mbtr["k3"] = self._get_k3(system, new_system_k3, indices_k3)
+            indices = indices_k3
+        mbtr = getattr(self, f"_get_k{self.k}")(system, new_system, indices)
 
         # Handle normalization
-        if self.normalization == "l2_each":
-            if self.flatten is True:
-                for key, value in mbtr.items():
-                    norm = np.linalg.norm(value.data)
-                    value /= norm
-            else:
-                for key, value in mbtr.items():
-                    for array in value:
-                        i_data = array.ravel()
-                        i_norm = np.linalg.norm(i_data)
-                        array /= i_norm
-
-        # Flatten output if requested
-        if self.flatten:
-            keys = sorted(mbtr.keys())
-            if len(keys) > 1:
-                result = sparse.concatenate([mbtr[key] for key in keys], axis=1)
-            else:
-                result = mbtr[keys[0]]
+        if self.normalization == "l2":
+            normalize(mbtr.tocsr(), norm="l2", axis=1, copy=False)
 
-            # Make into a dense array if requested
-            if not self.sparse:
-                result = result.todense()
-
-        # Otherwise return a list of dictionaries, each dictionary containing
-        # the requested unflattened tensors
-        else:
-            result = np.empty((n_loc), dtype="object")
-            for i_loc in range(n_loc):
-                i_dict = {}
-                for key in mbtr.keys():
-                    tensor = mbtr[key]
-                    i_dict[key] = tensor[i_loc]
-                result[i_loc] = i_dict
+        # Make into a dense array
+        result = mbtr.todense()
 
         return result
 
     def get_number_of_features(self):
         """Used to inquire the final number of features that this descriptor
         will have.
 
         The number of features for the LMBTR is calculated as follows:
 
         For the pair term (k=2), only pairs where at least one of the atom is
         the central atom (in periodic systems the central atom may connect to
         itself) are considered. This means that there are only as many
         combinations as there are different elements to pair the central atom
-        with (n_elem). This nmber of combinations is the multiplied by the
+        with (n_elem). This number of combinations is the multiplied by the
         discretization of the k=2 grid.
 
         For the three-body term (k=3), only triplets where at least one of the
         atoms is the central atom (in periodic systems the central atom may
         connect to itself) and the k >= i (symmetry) are considered. This means
         that as k runs from 0 to n-1, where n is the number of elements, there
         are n + k combinations that fill this rule. This sum becomes:
@@ -467,74 +509,67 @@
         combinations is the multiplied by the discretization of the k=3 grid.
 
         Returns:
             int: Number of features for this descriptor.
         """
         n_features = 0
         n_elem = self.n_elements
+        n_grid = self.grid["n"]
 
-        if self.k2 is not None:
-            n_k2_grid = self.k2["grid"]["n"]
-            n_k2 = (n_elem) * n_k2_grid
-            n_features += n_k2
-        if self.k3 is not None:
-            n_k3_grid = self.k3["grid"]["n"]
-            n_k3 = (
-                n_elem * (3 * n_elem - 1) * n_k3_grid / 2
-            )  # = (n_elem*n_elem + (n_elem-1)*n_elem/2)*n_k3_grid
-            n_features += n_k3
+        if self.k == 2:
+            n_features = (n_elem) * n_grid
+        if self.k == 3:
+            n_features = n_elem * (3 * n_elem - 1) * n_grid / 2
 
         return int(n_features)
 
     def _make_new_klist_local(self, kx_list):
         new_kx_list = []
 
         for item in kx_list:
             new_kx_map = {}
             item = dict(item)
             for key, value in item.items():
                 new_key = tuple(int(x) for x in key.split(","))
-                new_kx_map[new_key] = np.array(value, dtype=np.float32)
+                new_kx_map[new_key] = np.array(value, dtype=self.dtype)
             new_kx_list.append(new_kx_map)
 
         return new_kx_list
 
     def _get_k2(self, system, new_system, indices):
         """Calculates the second order terms where the scalar mapping is the
         inverse distance between atoms.
 
         Returns:
             1D ndarray: flattened K2 values.
         """
-        grid = self.k2["grid"]
-        start = grid["min"]
-        stop = grid["max"]
-        n = grid["n"]
-        sigma = grid["sigma"]
+        start = self.grid["min"]
+        stop = self.grid["max"]
+        n = self.grid["n"]
+        sigma = self.grid["sigma"]
 
         # Determine the weighting function and possible radial cutoff
         radial_cutoff = None
-        weighting = self.k2.get("weighting")
         parameters = {}
-        if weighting is not None:
-            weighting_function = weighting["function"]
+        if self.weighting is not None:
+            weighting_function = self.weighting["function"]
             if weighting_function == "exponential" or weighting_function == "exp":
-                scale = weighting["scale"]
-                threshold = weighting["threshold"]
+                scale = self.weighting["scale"]
+                threshold = self.weighting["threshold"]
                 if scale != 0:
                     radial_cutoff = -math.log(threshold) / scale
                 parameters = {
-                    b"scale": weighting["scale"],
-                    b"threshold": weighting["threshold"],
+                    b"scale": self.weighting["scale"],
+                    b"threshold": self.weighting["threshold"],
                 }
         else:
             weighting_function = "unity"
 
         # Determine the geometry function
-        geom_func_name = self.k2["geometry"]["function"]
+        geom_func_name = self.geometry["function"]
 
         # Calculate extended system
         if self.periodic:
             centers = new_system.get_positions()
             ext_system, cell_indices = dscribe.utils.geometry.get_extended_system(
                 system,
                 radial_cutoff,
@@ -589,80 +624,63 @@
             parameters,
             start,
             stop,
             sigma,
             n,
         )
         k2_list = self._make_new_klist_local(k2_list)
-
-        # Depending on flattening, use either a sparse matrix or a dense one.
         n_elem = self.n_elements
         n_loc = len(indices)
-        if self.flatten:
-            k2 = sparse.DOK((n_loc, n_elem * n), dtype=np.float32)
+        k2 = sparse.DOK((n_loc, n_elem * n), dtype=self.dtype)
 
-            for i_loc, k2_map in enumerate(k2_list):
-                for key, gaussian_sum in k2_map.items():
-                    i = key[1]
-                    m = i
-                    start = int(m * n)
-                    end = int((m + 1) * n)
-
-                    # Denormalize if requested
-                    if not self.normalize_gaussians:
-                        max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                        gaussian_sum /= max_val
+        for i_loc, k2_map in enumerate(k2_list):
+            for key, gaussian_sum in k2_map.items():
+                i = key[1]
+                m = i
+                start = int(m * n)
+                end = int((m + 1) * n)
+
+                # Denormalize if requested
+                if not self.normalize_gaussians:
+                    max_val = 1 / (sigma * math.sqrt(2 * math.pi))
+                    gaussian_sum /= max_val
 
-                    k2[i_loc, start:end] = gaussian_sum
-            k2 = k2.to_coo()
-        else:
-            k2 = np.zeros((n_loc, n_elem, n), dtype=np.float32)
-            for i_loc, k2_map in enumerate(k2_list):
-                for key, gaussian_sum in k2_map.items():
-                    i = key[1]
-
-                    # Denormalize if requested
-                    if not self.normalize_gaussians:
-                        max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                        gaussian_sum /= max_val
-
-                    k2[i_loc, i, :] = gaussian_sum
+                k2[i_loc, start:end] = gaussian_sum
+        k2 = k2.to_coo()
 
         return k2
 
     def _get_k3(self, system, new_system, indices):
         """Calculates the second order terms where the scalar mapping is the
         inverse distance between atoms.
 
         Returns:
             1D ndarray: flattened K2 values.
         """
-        grid = self.k3["grid"]
-        start = grid["min"]
-        stop = grid["max"]
-        n = grid["n"]
-        sigma = grid["sigma"]
+        start = self.grid["min"]
+        stop = self.grid["max"]
+        n = self.grid["n"]
+        sigma = self.grid["sigma"]
 
         # Determine the weighting function and possible radial cutoff
         radial_cutoff = None
-        weighting = self.k3.get("weighting")
         parameters = {}
-        if weighting is not None:
-            weighting_function = weighting["function"]
+        if self.weighting is not None:
+            weighting_function = self.weighting["function"]
             if weighting_function == "exponential" or weighting_function == "exp":
-                scale = weighting["scale"]
-                threshold = weighting["threshold"]
+                scale = self.weighting["scale"]
+                threshold = self.weighting["threshold"]
                 if scale != 0:
                     radial_cutoff = -0.5 * math.log(threshold) / scale
                 parameters = {b"scale": scale, b"threshold": threshold}
         else:
             weighting_function = "unity"
 
         # Determine the geometry function
-        geom_func_name = self.k3["geometry"]["function"]
+        geom_func_name = self.geometry["function"]
 
         # Calculate extended system
         if self.periodic:
             centers_new = new_system.get_positions()
             centers_existing = system.get_positions()[indices]
             centers = np.concatenate((centers_new, centers_existing), axis=0)
             ext_system, cell_indices = dscribe.utils.geometry.get_extended_system(
@@ -686,15 +704,14 @@
         fin_system = ext_system + new_system
         n_atoms_ext = len(ext_system)
         n_atoms_fin = len(fin_system)
         n_atoms_new = len(new_system)
         ext_pos = ext_system.get_positions()
         new_pos = new_system.get_positions()
         if radial_cutoff is not None:
-
             # Calculate distance within the extended system
             dmat_ext_to_ext = ext_system.get_distance_matrix_within_radius(
                 radial_cutoff, pos=ext_pos
             )
             col = dmat_ext_to_ext.col
             row = dmat_ext_to_ext.row
             data = dmat_ext_to_ext.data
@@ -768,61 +785,47 @@
             start,
             stop,
             sigma,
             n,
         )
 
         k3_list = self._make_new_klist_local(k3_list)
-        # Depending on flattening, use either a sparse matrix or a dense one.
+
         n_elem = self.n_elements
         n_loc = len(indices)
-        if self.flatten:
-            k3 = sparse.DOK(
-                (n_loc, int((n_elem * (3 * n_elem - 1) * n / 2))), dtype=np.float32
-            )
-
-            for i_loc, k3_map in enumerate(k3_list):
-                for key, gaussian_sum in k3_map.items():
-                    i = key[0]
-                    j = key[1]
-                    k = key[2]
-
-                    # This is the index of the spectrum. It is given by enumerating the
-                    # elements of a three-dimensional array and only considering
-                    # elements for which k>=i and i || j == 0. The enumeration begins
-                    # from [0, 0, 0], and ends at [n_elem, n_elem, n_elem], looping the
-                    # elements in the order k, i, j.
-                    if j == 0:
-                        m = k + i * n_elem - i * (i + 1) / 2
-                    else:
-                        m = n_elem * (n_elem + 1) / 2 + (j - 1) * n_elem + k
-                    start = int(m * n)
-                    end = int((m + 1) * n)
-
-                    # Denormalize if requested
-                    if not self.normalize_gaussians:
-                        max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                        gaussian_sum /= max_val
+        k3 = sparse.DOK(
+            (n_loc, int((n_elem * (3 * n_elem - 1) * n / 2))), dtype=self.dtype
+        )
 
-                    k3[i_loc, start:end] = gaussian_sum
-            k3 = k3.to_coo()
-        else:
-            k3 = np.zeros((n_loc, n_elem, n_elem, n_elem, n), dtype=np.float32)
-            for i_loc, k3_map in enumerate(k3_list):
-                for key, gaussian_sum in k3_map.items():
-                    i = key[0]
-                    j = key[1]
-                    k = key[2]
-
-                    # Denormalize if requested
-                    if not self.normalize_gaussians:
-                        max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                        gaussian_sum /= max_val
+        for i_loc, k3_map in enumerate(k3_list):
+            for key, gaussian_sum in k3_map.items():
+                i = key[0]
+                j = key[1]
+                k = key[2]
+
+                # This is the index of the spectrum. It is given by enumerating the
+                # elements of a three-dimensional array and only considering
+                # elements for which k>=i and i || j == 0. The enumeration begins
+                # from [0, 0, 0], and ends at [n_elem, n_elem, n_elem], looping the
+                # elements in the order k, i, j.
+                if j == 0:
+                    m = k + i * n_elem - i * (i + 1) / 2
+                else:
+                    m = n_elem * (n_elem + 1) / 2 + (j - 1) * n_elem + k
+                start = int(m * n)
+                end = int((m + 1) * n)
+
+                # Denormalize if requested
+                if not self.normalize_gaussians:
+                    max_val = 1 / (sigma * math.sqrt(2 * math.pi))
+                    gaussian_sum /= max_val
+
+                k3[i_loc, start:end] = gaussian_sum
+        k3 = k3.to_coo()
 
-                    k3[i_loc, i, j, k, :] = gaussian_sum
         return k3
 
     def get_location(self, species):
         """Can be used to query the location of a species combination in the
         the flattened output.
 
         Args:
@@ -838,105 +841,68 @@
 
         Raises:
             ValueError: If the requested species combination is not in the
             output or if invalid species defined.
         """
         # Check that the corresponding part is calculated
         k = len(species)
-        term = getattr(self, "k{}".format(k))
-        if term is None:
+        if k is not self.k:
             raise ValueError(
-                "Cannot retrieve the location for {}, as the term {} has not "
-                "been specifed.".format(species, term)
+                "Cannot retrieve the location for {}, as the term k={} has not "
+                "been specified.".format(species, k)
             )
 
         # Change chemical elements into atomic numbers
         numbers = []
         for specie in species:
             if isinstance(specie, str):
                 try:
                     specie = ase.data.atomic_numbers[specie]
                 except KeyError:
                     raise ValueError("Invalid chemical species")
             numbers.append(specie)
 
+        # Check that species exists and that X is included
+        self.check_atomic_numbers(numbers)
+        if 0 not in numbers:
+            raise ValueError(
+                "The central species X (atomic number 0) has to be one of the elements."
+            )
+
         # Change into internal indexing
         numbers = [self.atomic_number_to_index[x] for x in numbers]
         n_elem = self.n_elements
+        n = self.grid["n"]
 
         # k=2
-        if len(numbers) == 2:
+        if k == 2:
             if numbers[0] > numbers[1]:
                 numbers = list(reversed(numbers))
 
-            n2 = self.k2["grid"]["n"]
             j = numbers[1]
             m = j
-            start = int(m * n2)
-            end = int((m + 1) * n2)
+            start = int(m * n)
+            end = int((m + 1) * n)
 
         # k=3
-        if len(numbers) == 3:
+        if k == 3:
             if numbers[0] > numbers[2]:
                 numbers = list(reversed(numbers))
 
-            n3 = self.k3["grid"]["n"]
             i = numbers[0]
             j = numbers[1]
             k = numbers[2]
 
             # This is the index of the spectrum. It is given by enumerating the
             # elements of a three-dimensional array and only considering
             # elements for which k>=i and i || j == 0. The enumeration begins
             # from [0, 0, 0], and ends at [n_elem, n_elem, n_elem], looping the
             # elements in the order k, i, j.
             if j == 0:
                 m = k + i * n_elem - i * (i + 1) / 2
             else:
                 m = n_elem * (n_elem + 1) / 2 + (j - 1) * n_elem + k
 
-            offset = 0
-            if self.k2 is not None:
-                n2 = self.k2["grid"]["n"]
-                offset += n_elem * n2
-            start = int(offset + m * n3)
-            end = int(offset + (m + 1) * n3)
+            start = int(m * n)
+            end = int((m + 1) * n)
 
         return slice(start, end)
-
-    @property
-    def species(self):
-        return self._species
-
-    @species.setter
-    def species(self, value):
-        """Used to check the validity of given atomic numbers and to initialize
-        the C-memory layout for them.
-
-        Args:
-            value(iterable): Chemical species either as a list of atomic
-                numbers or list of chemical symbols.
-        """
-        # The species are stored as atomic numbers for internal use.
-        self._set_species(value)
-
-        # The atomic number 0 is reserved for ghost atoms in this
-        # implementation.
-        if 0 in self._atomic_number_set:
-            raise ValueError(
-                "The atomic number 0 is reserved for the ghost atoms in this "
-                "implementation."
-            )
-        self._atomic_number_set.add(0)
-        indices = np.searchsorted(self._atomic_numbers, 0)
-        self._atomic_numbers = np.insert(self._atomic_numbers, indices, 0)
-
-        # Setup mappings between atom indices and types together with some
-        # statistics
-        self.atomic_number_to_index = {}
-        self.index_to_atomic_number = {}
-        for i_atom, atomic_number in enumerate(self._atomic_numbers):
-            self.atomic_number_to_index[atomic_number] = i_atom
-            self.index_to_atomic_number[i_atom] = atomic_number
-        self.n_elements = len(self._atomic_numbers)
-        self.max_atomic_number = max(self._atomic_numbers)
-        self.min_atomic_number = min(self._atomic_numbers)
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/matrixdescriptor.py` & `dscribe-2.0.0/dscribe/descriptors/descriptormatrix.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 limitations under the License.
 """
 import numpy as np
 from numpy.random import RandomState
 
 import sparse
 
-from dscribe.descriptors import Descriptor
-from abc import abstractmethod
+from dscribe.descriptors.descriptorglobal import DescriptorGlobal
 
 
-class MatrixDescriptor(Descriptor):
+class DescriptorMatrix(DescriptorGlobal):
     """A common base class for two-body matrix-like descriptors."""
 
     def __init__(
         self,
         n_atoms_max,
         permutation="sorted_l2",
         sigma=None,
         seed=None,
-        flatten=True,
         sparse=False,
+        dtype="float64",
     ):
         """
         Args:
             n_atoms_max (int): The maximum nuber of atoms that any of the
                 samples can have. This controls how much zeros need to be
                 padded to the final result.
             permutation (string): Defines the method for handling permutational
@@ -53,20 +52,18 @@
             sigma (float): Provide only when using the *random*-permutation
                 option. Standard deviation of the gaussian distributed noise
                 determining how much the rows and columns of the randomly
                 sorted matrix are scrambled.
             seed (int): Provide only when using the *random*-permutation
                 option. A seed to use for drawing samples from a normal
                 distribution.
-            flatten (bool): Whether the output of create() should be flattened
-                to a 1D array.
             sparse (bool): Whether the output should be a sparse matrix or a
                 dense numpy array.
         """
-        super().__init__(periodic=False, flatten=flatten, sparse=sparse)
+        super().__init__(periodic=False, sparse=sparse, dtype=dtype)
 
         # Check parameter validity
         if n_atoms_max <= 0:
             raise ValueError("The maximum number of atoms must be a positive number.")
         perm_options = set(
             ("sorted_l2", "none", "eigenspectrum", "eigenspectrum", "random")
         )
@@ -105,16 +102,15 @@
 
     def create_single(self, system):
         """
         Args:
             system (:class:`ase.Atoms` | :class:`.System`): Input system.
 
         Returns:
-            ndarray: The zero padded matrix either as a 2D array or as
-                a 1D array depending on the setting self._flatten.
+            ndarray: The zero padded matrix either as a 1D array.
         """
         # Remove the old norm vector for the new system
         self._norm_vector = None
 
         matrix = self.get_matrix(system)
 
         # Handle the permutation option
@@ -125,22 +121,16 @@
         elif self.permutation == "eigenspectrum":
             matrix = self.get_eigenspectrum(matrix)
         elif self.permutation == "random":
             matrix = self.sort_randomly(matrix, self.sigma)
 
         # Add zero padding
         matrix = self.zero_pad(matrix)
-
         # Flatten
-        if self.permutation == "eigenspectrum" or self._flatten:
-            matrix = np.reshape(matrix, (matrix.size,))
-
-        # If a sparse matrix is requested, convert to coo_matrix
-        if self._sparse:
-            matrix = sparse.COO.from_numpy(matrix)
+        matrix = np.reshape(matrix, (matrix.size,))
 
         return matrix
 
     def sort(self, matrix):
         """Sorts the given matrix by using the L2 norm.
 
         Args:
@@ -164,16 +154,18 @@
 
         Args:
             matrix(np.ndarray): The matrix to sort.
 
         Returns:
             np.ndarray: A list of eigenvalues sorted by absolute value.
         """
-        # Calculate eigenvalues
+        # Calculate eigenvalues. Due to numerical instability there maybe very
+        # small imaginary parts that are ignored.
         eigenvalues, _ = np.linalg.eig(matrix)
+        eigenvalues = eigenvalues.real
 
         # Remove sign
         abs_values = np.absolute(eigenvalues)
 
         # Get ordering that sorts the values in descending order by absolute
         # value
         sorted_indices = np.argsort(abs_values)[::-1]
@@ -243,7 +235,48 @@
         Returns:
             np.ndarray: L2 norm of each row / column.
 
         """
         if self._norm_vector is None:
             self._norm_vector = np.linalg.norm(matrix, axis=1)
         return self._norm_vector
+
+    def unflatten(self, features, n_systems=None):
+        """
+        Can be used to "unflatten" a matrix descriptor back into a 2D array.
+        Useful for testing and visualization purposes.
+
+        Args:
+            features(np.ndarray): Flattened features.
+            n_systems(int): Number of systems. If not specified a value will be
+                guessed from the input features.
+
+        Returns:
+            np.ndarray: The features as a 2D array.
+        """
+        if n_systems is None:
+            n_dim = len(features.shape)
+            n_systems = 1 if n_dim == 1 else features.shape[0]
+        if self.sparse:
+            if n_systems != 1:
+                full = sparse.zeros(
+                    (n_systems, self.n_atoms_max, self.n_atoms_max), format="dok"
+                )
+                for i_sys in range(n_systems):
+                    full[i_sys] = (
+                        features[i_sys]
+                        .reshape((self.n_atoms_max, self.n_atoms_max))
+                        .todense()
+                    )
+                full = full.to_coo()
+            else:
+                full = features.reshape((self.n_atoms_max, self.n_atoms_max))
+        else:
+            if n_systems != 1:
+                full = np.zeros((n_systems, self.n_atoms_max, self.n_atoms_max))
+                for i_sys in range(n_systems):
+                    full[i_sys] = features[i_sys].reshape(
+                        (self.n_atoms_max, self.n_atoms_max)
+                    )
+            else:
+                full = features.reshape((self.n_atoms_max, self.n_atoms_max))
+        return full
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/mbtr.py` & `dscribe-2.0.0/dscribe/descriptors/mbtr.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,421 +13,296 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import sys
 import math
 import numpy as np
 
-import sparse
-
 from ase import Atoms
 import ase.data
 
 from dscribe.core import System
-from dscribe.descriptors import Descriptor
+from dscribe.descriptors.descriptorglobal import DescriptorGlobal
 from dscribe.ext import MBTRWrapper
 import dscribe.utils.geometry
 
 
-class MBTR(Descriptor):
-    """Implementation of the Many-body tensor representation up to :math:`k=3`.
-
-    You can choose which terms to include by providing a dictionary in the
-    k1, k2 or k3 arguments. This dictionary should contain information
-    under three keys: "geometry", "grid" and "weighting". See the examples
-    below for how to format these dictionaries.
-
-    You can use this descriptor for finite and periodic systems. When dealing
-    with periodic systems or when using machine learning models that use the
-    Euclidean norm to measure distance between vectors, it is advisable to use
-    some form of normalization.
-
-    For the geometry functions the following choices are available:
-
-    * :math:`k=1`:
-
-       * "atomic_number": The atomic numbers.
-
-    * :math:`k=2`:
-
-       * "distance": Pairwise distance in angstroms.
-       * "inverse_distance": Pairwise inverse distance in 1/angstrom.
+k1_geometry_functions = set(["atomic_number"])
+k2_geometry_functions = set(["distance", "inverse_distance"])
+k3_geometry_functions = set(["angle", "cosine"])
 
-    * :math:`k=3`:
 
-       * "angle": Angle in degrees.
-       * "cosine": Cosine of the angle.
+def check_grid(grid: dict):
+    """Used to ensure that the given grid settings are valid.
 
-    For the weighting the following functions are available:
-
-    * :math:`k=1`:
-
-       * "unity": No weighting.
-
-    * :math:`k=2`:
+    Args:
+        grid(dict): Dictionary containing the grid setup.
+    """
+    msg = "The grid information is missing the value for {}"
+    val_names = ["min", "max", "sigma", "n"]
+    for val_name in val_names:
+        try:
+            grid[val_name]
+        except Exception:
+            raise KeyError(msg.format(val_name))
+
+    # Make the n into integer
+    grid["n"] = int(grid["n"])
+    if grid["min"] >= grid["max"]:
+        raise ValueError("The min value should be smaller than the max value.")
 
-       * "unity": No weighting.
-       * "exp": Weighting of the form :math:`e^{-sx}`
-       * "inverse_square": Weighting of the form :math:`1/(x^2)`
 
-    * :math:`k=3`:
+def check_geometry(geometry: dict):
+    """Used to ensure that the given geometry settings are valid.
 
-       * "unity": No weighting.
-       * "exp": Weighting of the form :math:`e^{-sx}`
-       * "smooth_cutoff": Weighting of the form :math:`f_{ij}f_{ik}`,
-         where :math:`f = 1+y(x/r_{cut})^{y+1}-(y+1)(x/r_{cut})^{y}`
+    Args:
+        geometry: Dictionary containing the geometry setup.
+    """
 
-    The exponential weighting is motivated by the exponential decay of screened
-    Coulombic interactions in solids. In the exponential weighting the
-    parameters **threshold** determines the value of the weighting function after
-    which the rest of the terms will be ignored. Either the parameter **scale**
-    or **r_cut** can be used to determine the parameter :math:`s`: **scale**
-    directly corresponds to this value whereas **r_cut** can be used to
-    indirectly determine it through :math:`s=-\log()`:. The meaning of
-    :math:`x` changes for different terms as follows:
+    if "function" in geometry:
+        function = geometry["function"]
+        valid_functions = (
+            k1_geometry_functions | k2_geometry_functions | k3_geometry_functions
+        )
+        if function not in valid_functions:
+            raise ValueError(
+                f"Unknown geometry function. Please use one of the following: {sorted(list(valid_functions))}"
+            )
+    else:
+        raise ValueError("Please specify a geometry function.")
 
-    * :math:`k=2`: :math:`x` = Distance between A->B
-    * :math:`k=3`: :math:`x` = Distance from A->B->C->A.
 
-    The inverse square and smooth cutoff function weightings use a cutoff
-    parameter **r_cut**, which is a radial distance after which the rest of
-    the atoms will be ignored. For both, :math:`x` means the distance between
-    A->B. For the smooth cutoff function, additional weighting key **sharpness**
-    can be added, which changes the value of :math:`y`. If not, it defaults to `2`.
+def check_weighting(k: int, weighting: dict, periodic: bool):
+    """Used to ensure that the given weighting settings are valid.
 
-    In the grid setup *min* is the minimum value of the axis, *max* is the
-    maximum value of the axis, *sigma* is the standard deviation of the
-    gaussian broadening and *n* is the number of points sampled on the
-    grid.
+    Args:
+        k: The MBTR degree.
+        weighting: Dictionary containing the weighting setup.
+        periodic: Whether the descriptor is periodic or not.
+    """
+    if weighting is not None:
+        if k == 1:
+            valid_functions = set(["unity"])
+        elif k == 2:
+            valid_functions = set(["unity", "exp", "inverse_square"])
+        elif k == 3:
+            valid_functions = set(["unity", "exp", "smooth_cutoff"])
+        function = weighting.get("function")
+        if function not in valid_functions:
+            raise ValueError(
+                f"Unknown weighting function specified for k={k}. Please use one of the following: {sorted(list(valid_functions))}"
+            )
+        else:
+            if function == "exp":
+                if "threshold" not in weighting:
+                    raise ValueError("Missing value for 'threshold' in the weighting.")
+                if "scale" not in weighting and "r_cut" not in weighting:
+                    raise ValueError(
+                        "Provide either 'scale' or 'r_cut' in the weighting."
+                    )
+                if "scale" in weighting and "r_cut" in weighting:
+                    raise ValueError(
+                        "Provide either 'scale' or 'r_cut', not both in the weighting."
+                    )
+            elif function == "inverse_square":
+                if "r_cut" not in weighting:
+                    raise ValueError("Missing value for 'r_cut' in the weighting.")
+            elif function == "smooth_cutoff":
+                if "r_cut" not in weighting:
+                    raise ValueError("Missing value for 'r_cut' in the weighting.")
+
+    # Check that weighting function is specified for periodic systems
+    if periodic and k > 1:
+        valid = False
+        if weighting is not None:
+            function = weighting.get("function")
+            if function is not None:
+                if function != "unity":
+                    valid = True
+        if not valid:
+            raise ValueError("Periodic systems need to have a weighting function.")
 
-    If flatten=False, a list of dense np.ndarrays for each k in ascending order
-    is returned. These arrays are of dimension (n_elements x n_elements x
-    n_grid_points), where the elements are sorted in ascending order by their
-    atomic number.
 
-    If flatten=True, a sparse.COO sparse matrix is returned. This sparse matrix
-    is of size (n_features,), where n_features is given by
-    get_number_of_features(). This vector is ordered so that the different
-    k-terms are ordered in ascending order, and within each k-term the
-    distributions at each entry (i, j, h) of the tensor are ordered in an
-    ascending order by (i * n_elements) + (j * n_elements) + (h * n_elements).
+class MBTR(DescriptorGlobal):
+    """Implementation of the Many-body tensor representation.
 
-    This implementation does not support the use of a non-identity correlation
-    matrix.
+    You can use this descriptor for finite and periodic systems. When dealing
+    with periodic systems or when using machine learning models that use the
+    Euclidean norm to measure distance between vectors, it is advisable to use
+    some form of normalization. This implementation does not support the use of
+    a non-identity correlation matrix.
     """
 
     def __init__(
         self,
-        k1=None,
-        k2=None,
-        k3=None,
+        geometry=None,
+        grid=None,
+        weighting=None,
         normalize_gaussians=True,
         normalization="none",
-        flatten=True,
         species=None,
         periodic=False,
         sparse=False,
+        dtype="float64",
     ):
         """
         Args:
-            k1 (dict): Setup for the k=1 term. For example::
+            geometry (dict): Setup the geometry function.
+                For example::
 
-                k1 = {
-                    "geometry": {"function": "atomic_number"},
-                    "grid": {"min": 1, "max": 10, "sigma": 0.1, "n": 50}
-                }
+                "geometry": {"function": "atomic_number"}
 
-            k2 (dict): Dictionary containing the setup for the k=2 term.
-                Contains setup for the used geometry function, discretization and
-                weighting function. For example::
-
-                    k2 = {
-                        "geometry": {"function": "inverse_distance"},
-                        "grid": {"min": 0.1, "max": 2, "sigma": 0.1, "n": 50},
-                        "weighting": {"function": "exp", "r_cut": 10, "threshold": 1e-2}
-                    }
-
-            k3 (dict): Dictionary containing the setup for the k=3 term.
-                Contains setup for the used geometry function, discretization and
-                weighting function. For example::
-
-                    k3 = {
-                        "geometry": {"function": "angle"},
-                        "grid": {"min": 0, "max": 180, "sigma": 5, "n": 50},
-                        "weighting" : {"function": "exp", "r_cut": 10, "threshold": 1e-3}
-                    }
+                The geometry function determines the degree :math:`k` for MBTR.
+                The order :math:`k` tells how many atoms are involved in the
+                calculation and thus also heavily influence the computational
+                time.
+
+                The following geometry functions are available:
+
+                * :math:`k=1`
+                    * ``"atomic_number"``: The atomic number.
+                * :math:`k=2`
+                    * ``"distance"``: Pairwise distance in angstroms.
+                    * ``"inverse_distance"``: Pairwise inverse distance in 1/angstrom.
+                * :math:`k=3`
+                    * ``"angle"``: Angle in degrees.
+                    * ``"cosine"``: Cosine of the angle.
+
+            grid (dict): Setup the discretization grid.
+                For example::
+
+                "grid": {"min": 0.1, "max": 2, "sigma": 0.1, "n": 50}
+
+                In the grid setup *min* is the minimum value of the axis, *max*
+                is the maximum value of the axis, *sigma* is the standard
+                deviation of the gaussian broadening and *n* is the number of
+                points sampled on the grid.
+
+            weighting (dict): Setup the weighting function and its parameters.
+                For example::
+
+                "weighting" : {"function": "exp", "r_cut": 10, "threshold": 1e-3}
+
+                The following weighting functions are available:
+
+                * :math:`k=1`
+                    * ``"unity"``: No weighting.
+                * :math:`k=2`
+                    * ``"unity"``: No weighting.
+                    * ``"exp"``: Weighting of the form :math:`e^{-sx}`
+                    * ``"inverse_square"``: Weighting of the form :math:`1/(x^2)`
+                * :math:`k=3`
+                    * ``"unity"``: No weighting.
+                    * ``"exp"``: Weighting of the form :math:`e^{-sx}`
+                    * ``"smooth_cutoff"``: Weighting of the form :math:`f_{ij}f_{ik}`,
+                        where :math:`f = 1+y(x/r_{cut})^{y+1}-(y+1)(x/r_{cut})^{y}`
+
+                The meaning of :math:`x` changes for different terms as follows:
+
+                * For :math:`k=2`: :math:`x` = Distance between A->B
+                * For :math:`k=3`: :math:`x` = Distance from A->B->C->A.
+
+                The exponential weighting is motivated by the exponential decay
+                of screened Coulombic interactions in solids. In the exponential
+                weighting the parameters **threshold** determines the value of
+                the weighting function after which the rest of the terms will be
+                ignored. Either the parameter **scale** or **r_cut** can be used
+                to determine the parameter :math:`s`: **scale** directly
+                corresponds to this value whereas **r_cut** can be used to
+                indirectly determine it through :math:`s=-\log()`:.
+
+                The inverse square and smooth cutoff function weightings use a
+                cutoff parameter **r_cut**, which is a radial distance after
+                which the rest of the atoms will be ignored. For the smooth
+                cutoff function, additional weighting key **sharpness** can be
+                added, which changes the value of :math:`y`. If a value for it
+                is not provided, it defaults to `2`.
 
             normalize_gaussians (bool): Determines whether the gaussians are
                 normalized to an area of 1. Defaults to True. If False, the
                 normalization factor is dropped and the gaussians have the form.
                 :math:`e^{-(x-\mu)^2/2\sigma^2}`
             normalization (str): Determines the method for normalizing the
                 output. The available options are:
 
-                * "none": No normalization.
-                * "l2_each": Normalize the Euclidean length of each k-term
-                  individually to unity.
-                * "n_atoms": Normalize the output by dividing it with the number
+                * ``"none"``: No normalization.
+                * ``"l2"``: Normalize the Euclidean length of the output to unity.
+                * ``"n_atoms"``: Normalize the output by dividing it with the number
                   of atoms in the system. If the system is periodic, the number
                   of atoms is determined from the given unit cell.
-                * "valle_oganov": Use Valle-Oganov descriptor normalization, with
+                * ``"valle_oganov"``: Use Valle-Oganov descriptor normalization, with
                   system cell volume and numbers of different atoms in the cell.
-
-            flatten (bool): Whether the output should be flattened to a 1D
-                array. If False, a dictionary of the different tensors is
-                provided, containing the values under keys: "k1", "k2", and
-                "k3":
             species (iterable): The chemical species as a list of atomic
                 numbers or as a list of chemical symbols. Notice that this is not
                 the atomic numbers that are present for an individual system, but
                 should contain all the elements that are ever going to be
                 encountered when creating the descriptors for a set of systems.
                 Keeping the number of chemical speices as low as possible is
                 preferable.
             periodic (bool): Set to true if you want the descriptor output to
                 respect the periodicity of the atomic systems (see the
                 pbc-parameter in the constructor of ase.Atoms).
             sparse (bool): Whether the output should be a sparse matrix or a
                 dense numpy array.
+            dtype (str): The data type of the output. Valid options are:
+
+                    * ``"float32"``: Single precision floating point numbers.
+                    * ``"float64"``: Double precision floating point numbers.
         """
-        if sparse and not flatten:
-            raise ValueError(
-                "Sparse, non-flattened output is currently not supported. If "
-                "you want a non-flattened output, please specify sparse=False "
-                "in the MBTR constructor."
-            )
-        super().__init__(periodic=periodic, flatten=flatten, sparse=sparse)
+        super().__init__(periodic=periodic, sparse=sparse, dtype=dtype)
         self.system = None
-        self.k1 = k1
-        self.k2 = k2
-        self.k3 = k3
-
-        # Setup the involved chemical species
+        self.geometry = geometry
+        self.grid = grid
+        self.weighting = weighting
         self.species = species
-
         self.normalization = normalization
         self.normalize_gaussians = normalize_gaussians
 
         if self.normalization == "valle_oganov" and not periodic:
             raise ValueError(
                 "Valle-Oganov normalization does not support non-periodic systems."
             )
 
         # Initializing .create() level variables
         self._interaction_limit = None
 
-        # Check that weighting function is specified for periodic systems
-        if self.periodic:
-            if self.k2 is not None:
-                valid = False
-                weighting = self.k2.get("weighting")
-                if weighting is not None:
-                    function = weighting.get("function")
-                    if function is not None:
-                        if function != "unity":
-                            valid = True
-                if not valid:
-                    raise ValueError(
-                        "Periodic systems need to have a weighting function."
-                    )
-
-            if self.k3 is not None:
-                valid = False
-                weighting = self.k3.get("weighting")
-                if weighting is not None:
-                    function = weighting.get("function")
-                    if function is not None:
-                        if function != "unity":
-                            valid = True
-
-                if not valid:
-                    raise ValueError(
-                        "Periodic systems need to have a weighting function."
-                    )
-
-    def check_grid(self, grid):
-        """Used to ensure that the given grid settings are valid.
-
-        Args:
-            grid(dict): Dictionary containing the grid setup.
-        """
-        msg = "The grid information is missing the value for {}"
-        val_names = ["min", "max", "sigma", "n"]
-        for val_name in val_names:
-            try:
-                grid[val_name]
-            except Exception:
-                raise KeyError(msg.format(val_name))
-
-        # Make the n into integer
-        grid["n"] = int(grid["n"])
-        if grid["min"] >= grid["max"]:
-            raise ValueError("The min value should be smaller than the max value.")
-
     @property
-    def k1(self):
-        return self._k1
+    def grid(self):
+        return self._grid
 
-    @k1.setter
-    def k1(self, value):
-        if value is not None:
-
-            # Check that only valid keys are used in the setups
-            for key in value.keys():
-                valid_keys = set(("geometry", "grid", "weighting"))
-                if key not in valid_keys:
-                    raise ValueError(
-                        "The given setup contains the following invalid key: {}".format(
-                            key
-                        )
-                    )
-
-            # Check the geometry function
-            geom_func = value["geometry"].get("function")
-            if geom_func is not None:
-                valid_geom_func = set(("atomic_number",))
-                if geom_func not in valid_geom_func:
-                    raise ValueError(
-                        "Unknown geometry function specified for k=1. Please use one of"
-                        " the following: {}".format(valid_geom_func)
-                    )
-
-            # Check the weighting function
-            weighting = value.get("weighting")
-            if weighting is not None:
-                valid_weight_func = set(("unity",))
-                weight_func = weighting.get("function")
-                if weight_func not in valid_weight_func:
-                    raise ValueError(
-                        "Unknown weighting function specified for k=1. Please use one of"
-                        " the following: {}".format(valid_weight_func)
-                    )
-
-            # Check grid
-            self.check_grid(value["grid"])
-        self._k1 = value
+    @grid.setter
+    def grid(self, value):
+        check_grid(value)
+        self._grid = value
 
     @property
-    def k2(self):
-        return self._k2
-
-    @k2.setter
-    def k2(self, value):
-        if value is not None:
-
-            # Check that only valid keys are used in the setups
-            for key in value.keys():
-                valid_keys = set(("geometry", "grid", "weighting"))
-                if key not in valid_keys:
-                    raise ValueError(
-                        "The given setup contains the following invalid key: {}".format(
-                            key
-                        )
-                    )
-
-            # Check the geometry function
-            geom_func = value["geometry"].get("function")
-            if geom_func is not None:
-                valid_geom_func = set(("distance", "inverse_distance"))
-                if geom_func not in valid_geom_func:
-                    raise ValueError(
-                        "Unknown geometry function specified for k=2. Please use one of"
-                        " the following: {}".format(valid_geom_func)
-                    )
+    def geometry(self):
+        return self._geometry
 
-            # Check the weighting function
-            weighting = value.get("weighting")
-            if weighting is not None:
-                valid_weight_func = set(("unity", "exp", "inverse_square"))
-                weight_func = weighting.get("function")
-                if weight_func not in valid_weight_func:
-                    raise ValueError(
-                        "Unknown weighting function specified for k=2. Please use one of"
-                        " the following: {}".format(valid_weight_func)
-                    )
-                else:
-                    if weight_func == "exp":
-                        threshold = weighting.get("threshold")
-                        if threshold is None:
-                            raise ValueError(
-                                "Missing value for 'threshold' in the k=2 weighting."
-                            )
-                        param = weighting.get("scale", weighting.get("r_cut"))
-                        if param is None:
-                            raise ValueError(
-                                "Provide either 'scale' or 'r_cut' in the k=2 weighting."
-                            )
-                    elif weight_func == "inverse_square":
-                        if weighting.get("r_cut") is None:
-                            raise ValueError(
-                                "Missing value for 'r_cut' in the k=2 weighting."
-                            )
-
-            # Check grid
-            self.check_grid(value["grid"])
-        self._k2 = value
+    @geometry.setter
+    def geometry(self, value):
+        check_geometry(value)
+        k_map = {
+            "atomic_number": 1,
+            "distance": 2,
+            "inverse_distance": 2,
+            "angle": 3,
+            "cosine": 3,
+        }
+        self.k = k_map[value["function"]]
+        self._geometry = value
 
     @property
-    def k3(self):
-        return self._k3
-
-    @k3.setter
-    def k3(self, value):
-        if value is not None:
-
-            # Check that only valid keys are used in the setups
-            for key in value.keys():
-                valid_keys = set(("geometry", "grid", "weighting"))
-                if key not in valid_keys:
-                    raise ValueError(
-                        "The given setup contains the following invalid key: {}".format(
-                            key
-                        )
-                    )
+    def weighting(self):
+        return self._weighting
 
-            # Check the geometry function
-            geom_func = value["geometry"].get("function")
-            if geom_func is not None:
-                valid_geom_func = set(("angle", "cosine"))
-                if geom_func not in valid_geom_func:
-                    raise ValueError(
-                        "Unknown geometry function specified for k=2. Please use one of"
-                        " the following: {}".format(valid_geom_func)
-                    )
-
-            # Check the weighting function
-            weighting = value.get("weighting")
-            if weighting is not None:
-                valid_weight_func = set(("unity", "exp", "smooth_cutoff"))
-                weight_func = weighting.get("function")
-                if weight_func not in valid_weight_func:
-                    raise ValueError(
-                        "Unknown weighting function specified for k=2. Please use one of"
-                        " the following: {}".format(valid_weight_func)
-                    )
-                else:
-                    if weight_func == "exp":
-                        threshold = weighting.get("threshold")
-                        if threshold is None:
-                            raise ValueError(
-                                "Missing value for 'threshold' in the k=3 weighting."
-                            )
-                        param = weighting.get("scale", weighting.get("r_cut"))
-                        if param is None:
-                            raise ValueError(
-                                "Provide either 'scale' or 'r_cut' in the k=3 weighting."
-                            )
-                    elif weight_func == "smooth_cutoff":
-                        if weighting.get("r_cut") is None:
-                            raise ValueError(
-                                "Missing value for 'r_cut' in the k=3 weighting."
-                            )
-            # Check grid
-            self.check_grid(value["grid"])
-        self._k3 = value
+    @weighting.setter
+    def weighting(self, value):
+        check_weighting(self.k, value, self.periodic)
+        self._weighting = value
 
     @property
     def species(self):
         return self._species
 
     @species.setter
     def species(self, value):
@@ -459,61 +334,22 @@
     @normalization.setter
     def normalization(self, value):
         """Checks that the given normalization is valid.
 
         Args:
             value(str): The normalization method to use.
         """
-        norm_options = set(("l2_each", "none", "n_atoms", "valle_oganov"))
+        norm_options = set(("none", "l2", "n_atoms", "valle_oganov"))
         if value not in norm_options:
             raise ValueError(
                 "Unknown normalization option given. Please use one of the "
-                "following: {}.".format(", ".join([str(x) for x in norm_options]))
+                "following: {}.".format(", ".join(sorted(list(norm_options))))
             )
         self._normalization = value
 
-    def get_k1_axis(self):
-        """Used to get the discretized axis for geometry function of the k=1
-        term.
-
-        Returns:
-            np.ndarray: The discretized axis for the k=1 term.
-        """
-        start = self.k1["grid"]["min"]
-        stop = self.k1["grid"]["max"]
-        n = self.k1["grid"]["n"]
-
-        return np.linspace(start, stop, n)
-
-    def get_k2_axis(self):
-        """Used to get the discretized axis for geometry function of the k=2
-        term.
-
-        Returns:
-            np.ndarray: The discretized axis for the k=2 term.
-        """
-        start = self.k2["grid"]["min"]
-        stop = self.k2["grid"]["max"]
-        n = self.k2["grid"]["n"]
-
-        return np.linspace(start, stop, n)
-
-    def get_k3_axis(self):
-        """Used to get the discretized axis for geometry function of the k=3
-        term.
-
-        Returns:
-            np.ndarray: The discretized axis for the k=3 term.
-        """
-        start = self.k3["grid"]["min"]
-        stop = self.k3["grid"]["max"]
-        n = self.k3["grid"]["n"]
-
-        return np.linspace(start, stop, n)
-
     def create(self, system, n_jobs=1, only_physical_cores=False, verbose=False):
         """Return MBTR output for the given systems.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or many atomic structures.
             n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
                 the calculation across samples. Defaults to serial calculation
@@ -525,30 +361,23 @@
                 determines which types of CPUs are used in calculating the
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
-            np.ndarray | sparse.COO | list: MBTR for the
-            given systems. The return type depends on the 'sparse' and
-            'flatten'-attributes. For flattened output a single numpy array or
-            sparse.COO matrix is returned. If the output is not flattened,
-            dictionaries containing the MBTR tensors for each k-term are
-            returned.
+            np.ndarray | sparse.COO: MBTR for the given systems. The return type
+            depends on the 'sparse' attribute.
         """
         # Combine input arguments
         system = [system] if isinstance(system, Atoms) else system
         inp = [(i_sys,) for i_sys in system]
 
         # Determine if the outputs have a fixed size
-        if self.flatten:
-            static_size = [self.get_number_of_features()]
-        else:
-            static_size = None
+        static_size = [self.get_number_of_features()]
 
         # Create in parallel
         output = self.create_parallel(
             inp,
             self.create_single,
             n_jobs,
             static_size,
@@ -561,100 +390,58 @@
     def create_single(self, system):
         """Return the many-body tensor representation for the given system.
 
         Args:
             system (:class:`ase.Atoms` | :class:`.System`): Input system.
 
         Returns:
-            dict | np.ndarray | sparse.COO: The return type is
-            specified by the 'flatten' and 'sparse'-parameters. If the output
-            is not flattened, a dictionary containing of MBTR outputs as numpy
-            arrays is created. Each output is under a "kX" key. If the output
-            is flattened, a single concatenated output vector is returned,
-            either as a sparse or a dense vector.
+            np.ndarray | sparse.COO: A single concatenated output vector is
+            returned, either as a sparse or a dense vector.
         """
         # Ensuring variables are re-initialized when a new system is introduced
         self.system = system
         self._interaction_limit = len(system)
 
         # Check that the system does not have elements that are not in the list
         # of atomic numbers
         self.check_atomic_numbers(system.get_atomic_numbers())
 
-        mbtr = {}
-        if self.k1 is not None:
-            mbtr["k1"] = self._get_k1(system)
-        if self.k2 is not None:
-            mbtr["k2"] = self._get_k2(system)
-        if self.k3 is not None:
-            mbtr["k3"] = self._get_k3(system)
+        mbtr, _ = getattr(self, f"_get_k{self.k}")(system, True, False)
 
         # Handle normalization
-        if self.normalization == "l2_each":
-            if self.flatten is True:
-                for key, value in mbtr.items():
-                    i_data = np.array(value.data)
-                    i_norm = np.linalg.norm(i_data)
-                    mbtr[key] = value / i_norm
-            else:
-                for key, value in mbtr.items():
-                    i_data = value.ravel()
-                    i_norm = np.linalg.norm(i_data)
-                    mbtr[key] = value / i_norm
+        if self.normalization == "l2":
+            mbtr /= np.linalg.norm(np.array(mbtr.data))
         elif self.normalization == "n_atoms":
-            n_atoms = len(self.system)
-            if self.flatten is True:
-                for key, value in mbtr.items():
-                    mbtr[key] = value / n_atoms
-            else:
-                for key, value in mbtr.items():
-                    mbtr[key] = value / n_atoms
-
-        # Flatten output if requested
-        if self.flatten:
-            keys = sorted(mbtr.keys())
-            if len(keys) > 1:
-                mbtr = sparse.concatenate([mbtr[key] for key in keys], axis=0)
-            else:
-                mbtr = mbtr[keys[0]]
-
-            # Make into a dense array if requested
-            if not self.sparse:
-                mbtr = mbtr.todense()
+            n_atoms = len(system)
+            mbtr /= n_atoms
 
         return mbtr
 
     def get_number_of_features(self):
         """Used to inquire the final number of features that this descriptor
         will have.
 
         Returns:
             int: Number of features for this descriptor.
         """
-        n_features = 0
         n_elem = self.n_elements
+        n_grid = self.grid["n"]
 
-        if self.k1 is not None:
-            n_k1_grid = self.k1["grid"]["n"]
-            n_k1 = n_elem * n_k1_grid
-            n_features += n_k1
-        if self.k2 is not None:
-            n_k2_grid = self.k2["grid"]["n"]
-            n_k2 = (n_elem * (n_elem + 1) / 2) * n_k2_grid
-            n_features += n_k2
-        if self.k3 is not None:
-            n_k3_grid = self.k3["grid"]["n"]
-            n_k3 = (n_elem * n_elem * (n_elem + 1) / 2) * n_k3_grid
-            n_features += n_k3
+        if self.k == 1:
+            n_features = n_elem * n_grid
+        if self.k == 2:
+            n_features = (n_elem * (n_elem + 1) / 2) * n_grid
+        if self.k == 3:
+            n_features = (n_elem * n_elem * (n_elem + 1) / 2) * n_grid
 
         return int(n_features)
 
     def get_location(self, species):
         """Can be used to query the location of a species combination in the
-        the flattened output.
+        the output.
 
         Args:
             species(tuple): A tuple containing a species combination as
                 chemical symbols or atomic numbers. The tuple can be for example
                 ("H"), ("H", "O") or ("H", "O", "H").
 
         Returns:
@@ -664,208 +451,174 @@
 
         Raises:
             ValueError: If the requested species combination is not in the
                 output or if invalid species defined.
         """
         # Check that the corresponding part is calculated
         k = len(species)
-        term = getattr(self, "k{}".format(k))
-        if term is None:
+        if self.k is not k:
             raise ValueError(
-                "Cannot retrieve the location for {}, as the term k{} has not "
-                "been specied.".format(species, k)
+                "Cannot retrieve the location for {}, as the term k={} has not "
+                "been specified.".format(species, k)
             )
 
         # Change chemical elements into atomic numbers
         numbers = []
         for specie in species:
             if isinstance(specie, str):
                 try:
                     specie = ase.data.atomic_numbers[specie]
                 except KeyError:
                     raise ValueError("Invalid chemical species: {}".format(specie))
             numbers.append(specie)
 
+        # Check that species exists
+        self.check_atomic_numbers(numbers)
+
         # Change into internal indexing
         numbers = [self.atomic_number_to_index[x] for x in numbers]
         n_elem = self.n_elements
 
-        # k=1
-        if len(numbers) == 1:
-            n1 = self.k1["grid"]["n"]
+        n = self.grid["n"]
+        if k == 1:
             i = numbers[0]
             m = i
-            start = int(m * n1)
-            end = int((m + 1) * n1)
+            start = int(m * n)
+            end = int((m + 1) * n)
 
         # k=2
-        if len(numbers) == 2:
+        if k == 2:
             if numbers[0] > numbers[1]:
                 numbers = list(reversed(numbers))
 
-            n2 = self.k2["grid"]["n"]
             i = numbers[0]
             j = numbers[1]
 
             # This is the index of the spectrum. It is given by enumerating the
             # elements of an upper triangular matrix from left to right and top
             # to bottom.
             m = j + i * n_elem - i * (i + 1) / 2
-
-            offset = 0
-            if self.k1 is not None:
-                n1 = self.k1["grid"]["n"]
-                offset += n_elem * n1
-            start = int(offset + m * n2)
-            end = int(offset + (m + 1) * n2)
+            start = int(m * n)
+            end = int((m + 1) * n)
 
         # k=3
-        if len(numbers) == 3:
+        if k == 3:
             if numbers[0] > numbers[2]:
                 numbers = list(reversed(numbers))
 
-            n3 = self.k3["grid"]["n"]
             i = numbers[0]
             j = numbers[1]
             k = numbers[2]
 
             # This is the index of the spectrum. It is given by enumerating the
             # elements of a three-dimensional array where for valid elements
             # k>=i. The enumeration begins from [0, 0, 0], and ends at [n_elem,
             # n_elem, n_elem], looping the elements in the order k, i, j.
             m = j * n_elem * (n_elem + 1) / 2 + k + i * n_elem - i * (i + 1) / 2
-
-            offset = 0
-            if self.k1 is not None:
-                n1 = self.k1["grid"]["n"]
-                offset += n_elem * n1
-            if self.k2 is not None:
-                n2 = self.k2["grid"]["n"]
-                offset += (n_elem * (n_elem + 1) / 2) * n2
-            start = int(offset + m * n3)
-            end = int(offset + (m + 1) * n3)
+            start = int(m * n)
+            end = int((m + 1) * n)
 
         return slice(start, end)
 
-    def _make_new_k1map(self, kx_map):
-        kx_map = dict(kx_map)
-        new_kx_map = {}
-
-        for key, value in kx_map.items():
-            new_key = tuple([int(key)])
-            new_kx_map[new_key] = np.array(value, dtype=np.float32)
-
-        return new_kx_map
-
-    def _make_new_kmap(self, kx_map):
-        kx_map = dict(kx_map)
-        new_kx_map = {}
-
-        for key, value in kx_map.items():
-            new_key = tuple(int(x) for x in key.split(","))
-            new_kx_map[new_key] = np.array(value, dtype=np.float32)
-
-        return new_kx_map
-
-    def _get_k1(self, system):
-        """Calculates the second order terms where the scalar mapping is the
-        inverse distance between atoms.
+    def _get_k1(self, system, return_descriptor, return_derivatives):
+        """Calculates the first order term and/or its derivatives with
+        regard to atomic positions.
 
         Returns:
-            1D ndarray: flattened K2 values.
-        """
-        grid = self.k1["grid"]
-        start = grid["min"]
-        stop = grid["max"]
-        n = grid["n"]
-        sigma = grid["sigma"]
-
-        # Determine the geometry function
-        geom_func_name = self.k1["geometry"]["function"]
-
-        cmbtr = MBTRWrapper(
-            self.atomic_number_to_index,
-            self._interaction_limit,
-            np.zeros((len(system), 3), dtype=int),
-        )
+            1D or 3D ndarray: K1 values. Returns a 1D array. If
+                return_descriptor=False, returns an array of shape (0).
+            3D ndarray: K1 derivatives. If return_derivatives=False, returns an
+                array of shape (0,0,0).
+        """
+        start = self.grid["min"]
+        stop = self.grid["max"]
+        n = self.grid["n"]
+        sigma = self.grid["sigma"]
 
-        k1_map = cmbtr.get_k1(
-            system.get_atomic_numbers(),
-            geom_func_name.encode(),
-            b"unity",
-            {},
-            start,
-            stop,
-            sigma,
-            n,
-        )
+        n_elem = self.n_elements
+        n_features = n_elem * n
 
-        k1_map = self._make_new_k1map(k1_map)
+        if return_descriptor:
+            # Determine the geometry function
+            geom_func_name = self.geometry["function"]
+
+            cmbtr = MBTRWrapper(
+                self.atomic_number_to_index,
+                self._interaction_limit,
+                np.zeros((len(system), 3), dtype=int),
+            )
 
-        # Depending on flattening, use either a sparse matrix or a dense one.
-        n_elem = self.n_elements
-        if self.flatten:
-            k1 = sparse.DOK((n_elem * n), dtype=np.float32)
+            k1 = np.zeros((n_features), dtype=np.float64)
+            cmbtr.get_k1(
+                k1,
+                system.get_atomic_numbers(),
+                geom_func_name.encode(),
+                b"unity",
+                {},
+                start,
+                stop,
+                sigma,
+                n,
+            )
         else:
-            k1 = np.zeros((n_elem, n), dtype=np.float32)
-
-        for key, gaussian_sum in k1_map.items():
-            i = key[0]
+            k1 = np.zeros((0), dtype=np.float64)
 
-            # Denormalize if requested
-            if not self.normalize_gaussians:
-                max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                gaussian_sum /= max_val
-
-            if self.flatten:
-                start = i * n
-                end = (i + 1) * n
-                k1[start:end] = gaussian_sum
-            else:
-                k1[i, :] = gaussian_sum
-        if self.flatten:
-            k1 = k1.to_coo()
-
-        return k1
-
-    def _get_k2(self, system):
-        """Calculates the second order terms where the scalar mapping is the
-        inverse distance between atoms.
+        if return_derivatives:
+            k1_d = np.zeros((self._interaction_limit, 3, n_features), dtype=np.float64)
+        else:
+            k1_d = np.zeros((0, 0, 0), dtype=np.float64)
 
+        # Denormalize if requested
+        if not self.normalize_gaussians:
+            max_val = 1 / (sigma * math.sqrt(2 * math.pi))
+            k1 /= max_val
+            k1_d /= max_val
+
+        # Convert to the final output precision.
+        if self.dtype == "float32":
+            k1 = k1.astype(self.dtype)
+            k1_d = k1_d.astype(self.dtype)
+
+        return (k1, k1_d)
+
+    def _get_k2(self, system, return_descriptor, return_derivatives):
+        """Calculates the second order term and/or its derivatives with
+        regard to atomic positions.
         Returns:
-            1D ndarray: flattened K2 values.
-        """
-        grid = self.k2["grid"]
-        start = grid["min"]
-        stop = grid["max"]
-        n = grid["n"]
-        sigma = grid["sigma"]
+            1D ndarray:   K2 values. Returns a 1D array. If
+                return_descriptor=False, returns an array of shape (0).
+            3D ndarray: K2 derivatives. If return_derivatives=False, returns an
+                array of shape (0,0,0).
+        """
+        start = self.grid["min"]
+        stop = self.grid["max"]
+        n = self.grid["n"]
+        sigma = self.grid["sigma"]
 
         # Determine the weighting function and possible radial cutoff
         r_cut = None
-        weighting = self.k2.get("weighting")
         parameters = {}
-        if weighting is not None:
-            weighting_function = weighting["function"]
+        if self.weighting is not None:
+            weighting_function = self.weighting["function"]
             if weighting_function == "exp":
-                threshold = weighting["threshold"]
-                r_cut = weighting.get("r_cut")
-                scale = weighting.get("scale")
+                threshold = self.weighting["threshold"]
+                r_cut = self.weighting.get("r_cut")
+                scale = self.weighting.get("scale")
                 if scale is not None and r_cut is None:
                     r_cut = -math.log(threshold) / scale
                 elif scale is None and r_cut is not None:
                     scale = -math.log(threshold) / r_cut
                 parameters = {b"scale": scale, b"threshold": threshold}
             elif weighting_function == "inverse_square":
-                r_cut = weighting["r_cut"]
+                r_cut = self.weighting["r_cut"]
         else:
             weighting_function = "unity"
 
         # Determine the geometry function
-        geom_func_name = self.k2["geometry"]["function"]
+        geom_func_name = self.geometry["function"]
 
         # If needed, create the extended system
         if self.periodic:
             centers = system.get_positions()
             ext_system, cell_indices = dscribe.utils.geometry.get_extended_system(
                 system, r_cut, centers, return_cell_indices=True
             )
@@ -890,124 +643,140 @@
             )  # The non-neighbor values are treated as "infinitely far".
             dmat_dense[dmat.row, dmat.col] = dmat.data
         # If no weighting is used, the full distance matrix is calculated
         else:
             dmat_dense = ext_system.get_distance_matrix()
             adj_list = np.tile(np.arange(n_atoms), (n_atoms, 1))
 
-        k2_map = cmbtr.get_k2(
+        n_elem = self.n_elements
+        n_features = int((n_elem * (n_elem + 1) / 2) * n)
+
+        if return_descriptor:
+            k2 = np.zeros((n_features), dtype=np.float64)
+        else:
+            k2 = np.zeros((0), dtype=np.float64)
+
+        if return_derivatives:
+            k2_d = np.zeros((self._interaction_limit, 3, n_features), dtype=np.float64)
+        else:
+            k2_d = np.zeros((0, 0, 0), dtype=np.float64)
+
+        # Generate derivatives for k=2 term
+        cmbtr.get_k2(
+            k2,
+            k2_d,
+            return_descriptor,
+            return_derivatives,
             ext_system.get_atomic_numbers(),
+            ext_system.get_positions(),
             dmat_dense,
             adj_list,
             geom_func_name.encode(),
             weighting_function.encode(),
             parameters,
             start,
             stop,
             sigma,
             n,
         )
 
-        k2_map = self._make_new_kmap(k2_map)
-
-        # Depending of flattening, use either a sparse matrix or a dense one.
-        n_elem = self.n_elements
-        if self.flatten:
-            k2 = sparse.DOK((int(n_elem * (n_elem + 1) / 2 * n)), dtype=np.float32)
-        else:
-            k2 = np.zeros((self.n_elements, self.n_elements, n), dtype=np.float32)
-
-        for key, gaussian_sum in k2_map.items():
-            i = key[0]
-            j = key[1]
-
-            # This is the index of the spectrum. It is given by enumerating the
-            # elements of an upper triangular matrix from left to right and top
-            # to bottom.
-            m = int(j + i * n_elem - i * (i + 1) / 2)
-
-            # Denormalize if requested
-            if not self.normalize_gaussians:
-                max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                gaussian_sum /= max_val
-
-            if self.flatten:
-                start = m * n
-                end = (m + 1) * n
-                k2[start:end] = gaussian_sum
-            else:
-                k2[i, j, :] = gaussian_sum
-
-            # Valle-Oganov normalization is calculated separately for each pair
-            if self.normalization == "valle_oganov":
-                S = self.system
-                n_elements = len(self.species)
-                V = S.cell.volume
-                imap = self.index_to_atomic_number
-                # Calculate the amount of each element for N_A*N_B term
-                counts = {}
-                for index, number in imap.items():
-                    counts[index] = list(S.get_atomic_numbers()).count(number)
-                y = gaussian_sum
-                if i == j:
-                    count_product = 0.5 * counts[i] * counts[j]
-                else:
-                    count_product = counts[i] * counts[j]
-                y_normed = (y * V) / (count_product * 4 * np.pi)
-                if self.flatten:
-                    k2[start:end] = y_normed
-                else:
-                    k2[i, j, :] = y_normed
-
-        if self.flatten:
-            k2 = k2.to_coo()
-
-        return k2
-
-    def _get_k3(self, system):
-        """Calculates the third order terms.
-
+        # Denormalize if requested
+        if not self.normalize_gaussians:
+            max_val = 1 / (sigma * math.sqrt(2 * math.pi))
+            k2 /= max_val
+            k2_d /= max_val
+
+        # Valle-Oganov normalization is calculated separately for each pair.
+        # Not implemented for derivatives.
+        if self.normalization == "valle_oganov":
+            volume = self.system.cell.volume
+            # Calculate the amount of each element for N_A*N_B term
+            values, counts = np.unique(
+                self.system.get_atomic_numbers(), return_counts=True
+            )
+            counts = dict(zip(values, counts))
+            for i_z in values:
+                for j_z in values:
+                    i = self.atomic_number_to_index[i_z]
+                    j = self.atomic_number_to_index[j_z]
+                    if j < i:
+                        continue
+                    if i == j:
+                        count_product = 0.5 * counts[i_z] * counts[j_z]
+                    else:
+                        count_product = counts[i_z] * counts[j_z]
+
+                    # This is the index of the spectrum. It is given by enumerating the
+                    # elements of an upper triangular matrix from left to right and top
+                    # to bottom.
+                    m = int(j + i * n_elem - i * (i + 1) / 2)
+                    start = m * n
+                    end = (m + 1) * n
+                    norm_factor = volume / (count_product * 4 * np.pi)
+
+                    k2[start:end] *= norm_factor
+                    k2_d[:, :, start:end] *= norm_factor
+
+        # Convert to the final output precision.
+        if self.dtype == "float32":
+            k2 = k2.astype(self.dtype)
+            k2_d = k2_d.astype(self.dtype)
+
+        return (k2, k2_d)
+
+    def _get_k3(self, system, return_descriptor, return_derivatives):
+        """Calculates the third order term and/or its derivatives with
+        regard to atomic positions.
         Returns:
-            1D ndarray: flattened K3 values.
-        """
-        grid = self.k3["grid"]
-        start = grid["min"]
-        stop = grid["max"]
-        n = grid["n"]
-        sigma = grid["sigma"]
+            1D ndarray: K3 values. Returns a 1D array. If
+                return_descriptor=False, returns an array of shape (0).
+            3D ndarray: K3 derivatives. If return_derivatives=False, returns an
+                array of shape (0,0,0).
+        """
+        start = self.grid["min"]
+        stop = self.grid["max"]
+        n = self.grid["n"]
+        sigma = self.grid["sigma"]
 
         # Determine the weighting function and possible radial cutoff
         r_cut = None
-        weighting = self.k3.get("weighting")
         parameters = {}
-        if weighting is not None:
-            weighting_function = weighting["function"]
+        if self.weighting is not None:
+            weighting_function = self.weighting["function"]
             if weighting_function == "exp":
-                threshold = weighting["threshold"]
-                r_cut = weighting.get("r_cut")
-                scale = weighting.get("scale")
+                threshold = self.weighting["threshold"]
+                r_cut = self.weighting.get("r_cut")
+                scale = self.weighting.get("scale")
                 # If we want to limit the triplets to a distance r_cut, we need
                 # to allow x=2*r_cut in the case of k=3.
                 if scale is not None and r_cut is None:
                     r_cut = -0.5 * math.log(threshold) / scale
                 elif scale is None and r_cut is not None:
                     scale = -0.5 * math.log(threshold) / r_cut
                 parameters = {b"scale": scale, b"threshold": threshold}
             if weighting_function == "smooth_cutoff":
                 try:
-                    sharpness = weighting["sharpness"]
+                    sharpness = self.weighting["sharpness"]
                 except Exception:
                     sharpness = 2
-                r_cut = weighting["r_cut"]
-                parameters = {b"sharpness": sharpness, b"cutoff": r_cut}
+                parameters = {
+                    b"sharpness": sharpness,
+                    b"cutoff": self.weighting["r_cut"],
+                }
+                # Evaluating smooth-cutoff weighting values requires distances
+                # between two neighbours of an atom, and the maximum distance
+                # between them is twice the cutoff radius. To include the
+                # neighbour-to-neighbour distances in the distance matrix, the
+                # neighbour list is generated with double radius.
+                r_cut = 2 * self.weighting["r_cut"]
         else:
             weighting_function = "unity"
 
         # Determine the geometry function
-        geom_func_name = self.k3["geometry"]["function"]
+        geom_func_name = self.geometry["function"]
 
         # If needed, create the extended system
         if self.periodic:
             centers = system.get_positions()
             ext_system, cell_indices = dscribe.utils.geometry.get_extended_system(
                 system, r_cut, centers, return_cell_indices=True
             )
@@ -1016,91 +785,166 @@
             ext_system = System.from_atoms(system)
             cell_indices = np.zeros((len(system), 3), dtype=int)
 
         cmbtr = MBTRWrapper(
             self.atomic_number_to_index, self._interaction_limit, cell_indices
         )
 
-        # If radial cutoff is finite, use it to calculate the sparse
-        # distance matrix to reduce computational complexity from O(n^2) to
-        # O(n log(n))
         n_atoms = len(ext_system)
         if r_cut is not None:
             dmat = ext_system.get_distance_matrix_within_radius(r_cut)
             adj_list = dscribe.utils.geometry.get_adjacency_list(dmat)
             dmat_dense = np.full(
                 (n_atoms, n_atoms), sys.float_info.max
             )  # The non-neighbor values are treated as "infinitely far".
             dmat_dense[dmat.col, dmat.row] = dmat.data
         # If no weighting is used, the full distance matrix is calculated
         else:
             dmat_dense = ext_system.get_distance_matrix()
             adj_list = np.tile(np.arange(n_atoms), (n_atoms, 1))
 
-        k3_map = cmbtr.get_k3(
+        n_elem = self.n_elements
+        n_features = int((n_elem * n_elem * (n_elem + 1) / 2) * n)
+
+        if return_descriptor:
+            k3 = np.zeros((n_features), dtype=np.float64)
+        else:
+            k3 = np.zeros((0), dtype=np.float64)
+
+        if return_derivatives:
+            k3_d = np.zeros((self._interaction_limit, 3, n_features), dtype=np.float64)
+        else:
+            k3_d = np.zeros((0, 0, 0), dtype=np.float64)
+
+        # Compute the k=3 term and its derivative
+        cmbtr.get_k3(
+            k3,
+            k3_d,
+            return_descriptor,
+            return_derivatives,
             ext_system.get_atomic_numbers(),
+            ext_system.get_positions(),
             dmat_dense,
             adj_list,
             geom_func_name.encode(),
             weighting_function.encode(),
             parameters,
             start,
             stop,
             sigma,
             n,
         )
 
-        k3_map = self._make_new_kmap(k3_map)
-        # Depending of flattening, use either a sparse matrix or a dense one.
-        n_elem = self.n_elements
-        if self.flatten:
-            k3 = sparse.DOK(
-                (int(n_elem * n_elem * (n_elem + 1) / 2 * n)), dtype=np.float32
+        # Denormalize if requested
+        if not self.normalize_gaussians:
+            max_val = 1 / (sigma * math.sqrt(2 * math.pi))
+            k3 /= max_val
+            k3_d /= max_val
+
+        # Valle-Oganov normalization is calculated separately for each triplet
+        # Not implemented for derivatives.
+        if self.normalization == "valle_oganov":
+            volume = self.system.cell.volume
+            # Calculate the amount of each element for N_A*N_B*N_C term
+            values, counts = np.unique(
+                self.system.get_atomic_numbers(), return_counts=True
+            )
+            counts = dict(zip(values, counts))
+            for i_z in values:
+                for j_z in values:
+                    for k_z in values:
+                        i = self.atomic_number_to_index[i_z]
+                        j = self.atomic_number_to_index[j_z]
+                        k = self.atomic_number_to_index[k_z]
+                        if k < i:
+                            continue
+                        # This is the index of the spectrum. It is given by enumerating the
+                        # elements of a three-dimensional array where for valid elements
+                        # k>=i. The enumeration begins from [0, 0, 0], and ends at [n_elem,
+                        # n_elem, n_elem], looping the elements in the order j, i, k.
+                        m = int(
+                            j * n_elem * (n_elem + 1) / 2
+                            + k
+                            + i * n_elem
+                            - i * (i + 1) / 2
+                        )
+                        start = m * n
+                        end = (m + 1) * n
+                        count_product = counts[i_z] * counts[j_z] * counts[k_z]
+                        norm_factor = volume / count_product
+
+                        k3[start:end] *= norm_factor
+                        k3_d[:, :, start:end] *= norm_factor
+
+        # Convert to the final output precision.
+        if self.dtype == "float32":
+            k3 = k3.astype(self.dtype)
+            k3_d = k3_d.astype(self.dtype)
+
+        return (k3, k3_d)
+
+    def validate_derivatives_method(self, method):
+        """Used to validate and determine the final method for calculating the
+        derivatives.
+        """
+        methods = {"numerical", "analytical", "auto"}
+        if method not in methods:
+            raise ValueError(
+                "Invalid method specified. Please choose from: {}".format(methods)
             )
+
+        if method == "numerical":
+            return method
+
+        # Check if analytical derivatives can be used
+        try:
+            supported_normalization = ["none", "n_atoms", "valle_oganov"]
+            if self.normalization not in supported_normalization:
+                raise ValueError(
+                    "Analytical derivatives not implemented for normalization option '{}'. Please choose from: {}".format(
+                        self.normalization, supported_normalization
+                    )
+                )
+            # Derivatives are not currently implemented for all k3 options
+            if self.k == 3:
+                # "angle" function is not differentiable
+                if self.geometry["function"] == "angle":
+                    raise ValueError(
+                        "Analytical derivatives not implemented for k3 geometry function 'angle'."
+                    )
+        except Exception as e:
+            if method == "analytical":
+                raise e
+            elif method == "auto":
+                method = "numerical"
         else:
-            k3 = np.zeros((n_elem, n_elem, n_elem, n), dtype=np.float32)
+            if method == "auto":
+                method = "analytical"
 
-        for key, gaussian_sum in k3_map.items():
-            i = key[0]
-            j = key[1]
-            k = key[2]
+        return method
 
-            # This is the index of the spectrum. It is given by enumerating the
-            # elements of a three-dimensional array where for valid elements
-            # k>=i. The enumeration begins from [0, 0, 0], and ends at [n_elem,
-            # n_elem, n_elem], looping the elements in the order j, i, k.
-            m = int(j * n_elem * (n_elem + 1) / 2 + k + i * n_elem - i * (i + 1) / 2)
+    def derivatives_analytical(self, d, c, system, indices, return_descriptor):
+        # Ensuring variables are re-initialized when a new system is introduced
+        self.system = system
+        self._interaction_limit = len(system)
+
+        # Check that the system does not have elements that are not in the list
+        # of atomic numbers
+        self.check_atomic_numbers(system.get_atomic_numbers())
+
+        mbtr, mbtr_d = getattr(self, f"_get_k{self.k}")(system, return_descriptor, True)
 
-            # Denormalize if requested
-            if not self.normalize_gaussians:
-                max_val = 1 / (sigma * math.sqrt(2 * math.pi))
-                gaussian_sum /= max_val
-
-            if self.flatten:
-                start = m * n
-                end = (m + 1) * n
-                k3[start:end] = gaussian_sum
-            else:
-                k3[i, j, k, :] = gaussian_sum
-
-            # Valle-Oganov normalization is calculated separately for each triplet
-            if self.normalization == "valle_oganov":
-                S = self.system
-                n_elements = len(self.species)
-                V = S.cell.volume
-                imap = self.index_to_atomic_number
-                # Calculate the amount of each element for N_A*N_B*N_C term
-                counts = {}
-                for index, number in imap.items():
-                    counts[index] = list(S.get_atomic_numbers()).count(number)
-                y = gaussian_sum
-                count_product = counts[i] * counts[j] * counts[k]
-                y_normed = (y * V) / count_product
-                if self.flatten:
-                    k3[start:end] = y_normed
-                else:
-                    k3[i, j, k, :] = y_normed
+        # Handle normalization
+        if self.normalization == "n_atoms":
+            n_atoms = len(self.system)
+            mbtr /= n_atoms
+            mbtr_d /= n_atoms
 
-        if self.flatten:
-            k3 = k3.to_coo()
+        # For now, the derivatives are calculated with regard to all atomic
+        # positions. The desired indices are extracted here at the end.
+        i = 0
+        for index in indices:
+            d[i, :] = mbtr_d[index, :, :]
+            i += 1
 
-        return k3
+        if return_descriptor:
+            np.copyto(c, mbtr)
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/sinematrix.py` & `dscribe-2.0.0/dscribe/descriptors/sinematrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 limitations under the License.
 """
 import numpy as np
 
 from ase import Atoms
 
 from dscribe.core import System
-from dscribe.descriptors.matrixdescriptor import MatrixDescriptor
+from dscribe.descriptors.descriptormatrix import DescriptorMatrix
 
 
-class SineMatrix(MatrixDescriptor):
+class SineMatrix(DescriptorMatrix):
     """Calculates the zero padded Sine matrix for different systems.
 
     The Sine matrix is defined as:
 
         Cij = 0.5 Zi**exponent      | i = j
             = (Zi*Zj)/phi(Ri, Rj)   | i != j
 
@@ -62,36 +62,30 @@
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             np.ndarray | sparse.COO: Sine matrix for the given systems. The
-            return type depends on the 'sparse' and 'flatten'-attributes. For
-            flattened output a single numpy array or sparse.COO is returned.
-            The first dimension is determined by the amount of systems.
+            return type depends on the 'sparse'-attribute. The first dimension
+            is determined by the amount of systems.
         """
         # Combine input arguments / check input validity
         system = [system] if isinstance(system, Atoms) else system
         for s in system:
             if len(s) > self.n_atoms_max:
                 raise ValueError(
                     "One of the given systems has more atoms ({}) than allowed "
                     "by n_atoms_max ({}).".format(len(s), self.n_atoms_max)
                 )
         inp = [(i_sys,) for i_sys in system]
 
         # Determine if the outputs have a fixed size
         n_features = self.get_number_of_features()
-        if self._flatten:
-            static_size = [n_features]
-        elif self.permutation == "eigenspectrum":
-            static_size = [self.n_atoms_max]
-        else:
-            static_size = [self.n_atoms_max, self.n_atoms_max]
+        static_size = [n_features]
 
         # Create in parallel
         output = self.create_parallel(
             inp,
             self.create_single,
             n_jobs,
             static_size,
```

### Comparing `dscribe-1.2.2/dscribe/descriptors/soap.py` & `dscribe-2.0.0/dscribe/descriptors/soap.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,34 +9,28 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import time
 import numpy as np
-from warnings import warn
 
 from scipy.special import gamma
 from scipy.linalg import sqrtm, inv
 
 from ase import Atoms
 import ase.geometry.cell
 import ase.data
 
-import sparse as sp
-
-from dscribe.descriptors import Descriptor
-from dscribe.core import System
-from dscribe.utils.dimensionality import is1d
+from dscribe.descriptors.descriptorlocal import DescriptorLocal
 import dscribe.ext
 
 
-class SOAP(Descriptor):
+class SOAP(DescriptorLocal):
     """Class for generating a partial power spectrum from Smooth Overlap of
     Atomic Orbitals (SOAP). This implementation uses real (tesseral) spherical
     harmonics as the angular basis set and provides two orthonormalized
     alternatives for the radial basis functions: spherical primitive gaussian
     type orbitals ("gto") or the polynomial basis set ("polynomial").
 
     For reference, see:
@@ -65,18 +59,14 @@
         weighting=None,
         crossover=True,
         average="off",
         species=None,
         periodic=False,
         sparse=False,
         dtype="float64",
-        # For backwards compatibility with < v1.2.2
-        rcut=None,
-        nmax=None,
-        lmax=None,
     ):
         """
         Args:
             r_cut (float): A cutoff for local region in angstroms. Should be
                 bigger than 1 angstrom for the gto-basis.
             n_max (int): The number of radial basis functions.
             l_max (int): The maximum degree of spherical harmonics.
@@ -169,37 +159,21 @@
                 dense numpy array.
             dtype (str): The data type of the output. Valid options are:
 
                     * ``"float32"``: Single precision floating point numbers.
                     * ``"float64"``: Double precision floating point numbers.
 
         """
-        var_dict = {}
-        for var_new in ["r_cut", "n_max", "l_max"]:
-            loc = locals()
-            var_old = "".join(var_new.split("_"))
-            if loc.get(var_old) is not None:
-                var_dict[var_new] = loc[var_old]
-                if loc.get(var_new) is not None:
-                    raise ValueError(
-                        "Please provide only either {} or {}.".format(var_new, var_old)
-                    )
-            else:
-                var_dict[var_new] = loc[var_new]
-        r_cut = var_dict["r_cut"]
-        n_max = var_dict["n_max"]
-        l_max = var_dict["l_max"]
-
         supported_dtype = set(("float32", "float64"))
         if dtype not in supported_dtype:
             raise ValueError(
                 "Invalid output data type '{}' given. Please use "
                 "one of the following: {}".format(dtype, supported_dtype)
             )
-        super().__init__(periodic=periodic, flatten=True, sparse=sparse, dtype=dtype)
+        super().__init__(periodic=periodic, sparse=sparse, dtype=dtype)
 
         # Setup the involved chemical species
         self.species = species
 
         # Test that general settings are valid
         if sigma <= 0:
             raise ValueError(
@@ -298,47 +272,44 @@
         self._weighting = weighting
         self._n_max = n_max
         self._l_max = l_max
         self._rbf = rbf
         self.average = average
         self.crossover = crossover
 
-    def prepare_centers(self, system, cutoff_padding, positions=None):
+    def prepare_centers(self, system, centers=None):
         """Validates and prepares the centers for the C++ extension."""
         # Check that the system does not have elements that are not in the list
         # of atomic numbers
         self.check_atomic_numbers(system.get_atomic_numbers())
 
         # Check if periodic is valid
         if self.periodic:
             cell = system.get_cell()
             if np.cross(cell[0], cell[1]).dot(cell[2]) == 0:
                 raise ValueError("System doesn't have cell to justify periodicity.")
 
         # Setup the local positions
-        if positions is None:
+        if centers is None:
             list_positions = system.get_positions()
             indices = np.arange(len(system))
         else:
             # Check validity of position definitions and create final cartesian
             # position list
             error = ValueError(
                 "The argument 'positions' should contain a non-empty "
                 "one-dimensional list of"
                 " atomic indices or a two-dimensional "
                 "list of cartesian coordinates with x, y and z components."
             )
-            if (
-                not isinstance(positions, (list, tuple, np.ndarray))
-                or len(positions) == 0
-            ):
+            if not isinstance(centers, (list, tuple, np.ndarray)) or len(centers) == 0:
                 raise error
             list_positions = []
-            indices = np.full(len(positions), -1, dtype=np.int)
-            for idx, i in enumerate(positions):
+            indices = np.full(len(centers), -1, dtype=np.int64)
+            for idx, i in enumerate(centers):
                 if np.issubdtype(type(i), np.integer):
                     list_positions.append(system.get_positions()[i])
                     indices[idx] = i
                 elif isinstance(i, (list, tuple, np.ndarray)):
                     if len(i) != 3:
                         raise error
                     list_positions.append(i)
@@ -377,55 +348,40 @@
             d = weighting["d"]
             r0 = weighting["r0"]
             r_cut = r0 * np.log(c / t - d)
             return r_cut
         else:
             return None
 
-    def init_descriptor_array(self, n_centers, n_features):
-        """Return a zero-initialized numpy array for the descriptor."""
-        if self.average == "inner" or self.average == "outer":
-            c = np.zeros((1, n_features), dtype=np.float64)
-        else:
-            c = np.zeros((n_centers, n_features), dtype=np.float64)
-        return c
-
-    def init_derivatives_array(self, n_centers, n_indices, n_features):
-        """Return a zero-initialized numpy array for the derivatives."""
-        if self.average == "inner" or self.average == "outer":
-            return np.zeros((1, n_indices, 3, n_features), dtype=np.float64)
-        else:
-            return np.zeros((n_centers, n_indices, 3, n_features), dtype=np.float64)
-
     def init_internal_dev_array(self, n_centers, n_atoms, n_types, n, l_max):
         d = np.zeros(
             (n_atoms, n_centers, n_types, n, (l_max + 1) * (l_max + 1)),
             dtype=np.float64,
         )
         return d
 
     def init_internal_array(self, n_centers, n_types, n, l_max):
         d = np.zeros(
             (n_centers, n_types, n, (l_max + 1) * (l_max + 1)), dtype=np.float64
         )
         return d
 
     def create(
-        self, system, positions=None, n_jobs=1, only_physical_cores=False, verbose=False
+        self, system, centers=None, n_jobs=1, only_physical_cores=False, verbose=False
     ):
-        """Return the SOAP output for the given systems and given positions.
+        """Return the SOAP output for the given systems and given centers.
 
         Args:
             system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
                 many atomic structures.
-            positions (list): Positions where to calculate SOAP. Can be
+            centers (list): Centers where to calculate SOAP. Can be
                 provided as cartesian positions or atomic indices. If no
-                positions are defined, the SOAP output will be created for all
+                centers are defined, the SOAP output will be created for all
                 atoms in the system. When calculating SOAP for multiple
-                systems, provide the positions as a list for each system.
+                systems, provide the centers as a list for each system.
             n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
                 the calculation across samples. Defaults to serial calculation
                 with n_jobs=1. If a negative number is given, the used cpus
                 will be calculated with, n_cpus + n_jobs, where n_cpus is the
                 amount of CPUs as reported by the OS. With only_physical_cores
                 you can control which types of CPUs are counted in n_cpus.
             only_physical_cores (bool): If a negative n_jobs is given,
@@ -433,55 +389,55 @@
                 number of jobs. If set to False (default), also virtual CPUs
                 are counted.  If set to True, only physical CPUs are counted.
             verbose(bool): Controls whether to print the progress of each job
                 into to the console.
 
         Returns:
             np.ndarray | sparse.COO: The SOAP output for the given systems and
-            positions. The return type depends on the 'sparse'-attribute. The
-            first dimension is determined by the amount of positions and
+            centers. The return type depends on the 'sparse'-attribute. The
+            first dimension is determined by the amount of centers and
             systems and the second dimension is determined by the
             get_number_of_features()-function. When multiple systems are
             provided the results are ordered by the input order of systems and
             their positions.
         """
         # Validate input / combine input arguments
         if isinstance(system, Atoms):
             system = [system]
-            positions = [positions]
+            centers = [centers]
         n_samples = len(system)
-        if positions is None:
+        if centers is None:
             inp = [(i_sys,) for i_sys in system]
         else:
-            n_pos = len(positions)
+            n_pos = len(centers)
             if n_pos != n_samples:
                 raise ValueError(
-                    "The given number of positions does not match the given "
+                    "The given number of centers does not match the given "
                     "number of systems."
                 )
-            inp = list(zip(system, positions))
+            inp = list(zip(system, centers))
 
         # Determine if the outputs have a fixed size
         n_features = self.get_number_of_features()
         static_size = None
         if self.average == "outer" or self.average == "inner":
             static_size = [n_features]
         else:
-            if positions is None:
+            if centers is None:
                 n_centers = len(inp[0][0])
             else:
                 first_sample, first_pos = inp[0]
                 if first_pos is not None:
                     n_centers = len(first_pos)
                 else:
                     n_centers = len(first_sample)
 
             def is_static():
                 for i_job in inp:
-                    if positions is None:
+                    if centers is None:
                         if len(i_job[0]) != n_centers:
                             return False
                     else:
                         if i_job[1] is not None:
                             if len(i_job[1]) != n_centers:
                                 return False
                         else:
@@ -500,54 +456,44 @@
             static_size,
             only_physical_cores,
             verbose=verbose,
         )
 
         return output
 
-    def create_single(self, system, positions=None):
-        """Return the SOAP output for the given system and given positions.
+    def create_single(self, system, centers=None):
+        """Return the SOAP output for the given system and given centers.
 
         Args:
             system (:class:`ase.Atoms` | :class:`.System`): Input system.
-            positions (list): Cartesian positions or atomic indices. If
+            centers (list): Cartesian positions or atomic indices. If
                 specified, the SOAP spectrum will be created for these points.
-                If no positions are defined, the SOAP output will be created
+                If no centers are defined, the SOAP output will be created
                 for all atoms in the system.
 
         Returns:
             np.ndarray | sparse.COO: The SOAP output for the
-            given system and positions. The return type depends on the
+            given system and centers. The return type depends on the
             'sparse'-attribute. The first dimension is given by the number of
-            positions and the second dimension is determined by the
+            centers and the second dimension is determined by the
             get_number_of_features()-function.
         """
         cutoff_padding = self.get_cutoff_padding()
-        centers, center_indices = self.prepare_centers(
-            system, cutoff_padding, positions
-        )
+        centers, _ = self.prepare_centers(system, centers)
         n_centers = centers.shape[0]
-        n_species = self._atomic_numbers.shape[0]
         pos = system.get_positions()
         Z = system.get_atomic_numbers()
-        n_features = self.get_number_of_features()
-        n_atoms = Z.shape[0]
-        soap_mat = self.init_descriptor_array(n_centers, n_features)
+        soap_mat = self.init_descriptor_array(n_centers)
 
         # Determine the function to call based on rbf
         if self._rbf == "gto":
-
             # Orthonormalized RBF coefficients
             alphas = self._alphas.flatten()
             betas = self._betas.flatten()
 
-            # Determine shape
-            n_features = self.get_number_of_features()
-            soap_mat = self.init_descriptor_array(n_centers, n_features)
-
             # Calculate with extension
             soap_gto = dscribe.ext.SOAPGTO(
                 self._r_cut,
                 self._n_max,
                 self._l_max,
                 self._eta,
                 self._weighting,
@@ -601,301 +547,88 @@
 
         # Averaged output is a global descriptor, and thus the first dimension
         # is squeezed out to keep the output size consistent with the size of
         # other global descriptors.
         if self.average != "off":
             soap_mat = np.squeeze(soap_mat, axis=0)
 
-        # Convert to the final output precision.
-        if self.dtype != "float64":
-            soap_mat = soap_mat.astype(self.dtype)
-
-        # Make into a sparse array if requested
-        if self._sparse:
-            soap_mat = sp.COO.from_numpy(soap_mat)
-
         return soap_mat
 
-    def derivatives(
-        self,
-        system,
-        positions=None,
-        include=None,
-        exclude=None,
-        method="auto",
-        return_descriptor=True,
-        attach=False,
-        n_jobs=1,
-        only_physical_cores=False,
-        verbose=False,
-    ):
-        """Return the descriptor derivatives for the given systems and given positions.
-
-        Args:
-            system (:class:`ase.Atoms` or list of :class:`ase.Atoms`): One or
-                many atomic structures.
-            positions (list): Positions where to calculate the descriptor. Can be
-                provided as cartesian positions or atomic indices. Also see the
-                "attach"-argument that controls the interperation of locations
-                given as atomic indices. If no positions are defined, the
-                descriptor output will be created for all atoms in the system.
-                When calculating descriptor for multiple systems, provide the
-                positions as a list for each system.
-            include (list): Indices of atoms to compute the derivatives on.
-                When calculating descriptor for multiple systems, provide
-                either a one-dimensional list that if applied to all systems or
-                a two-dimensional list of indices. Cannot be provided together
-                with 'exclude'.
-            exclude (list): Indices of atoms not to compute the derivatives on.
-                When calculating descriptor for multiple systems, provide
-                either a one-dimensional list that if applied to all systems or
-                a two-dimensional list of indices. Cannot be provided together
-                with 'include'.
-            method (str): The method for calculating the derivatives. Provide
-                either 'numerical', 'analytical' or 'auto'. If using 'auto',
-                the most efficient available method is automatically chosen.
-            attach (bool): Controls the behaviour of positions defined as
-                atomic indices. If True, the positions tied to an atomic index will
-                move together with the atoms with respect to which the derivatives
-                are calculated against. If False, positions defined as atomic
-                indices will be converted into cartesian locations that are
-                completely independent of the atom location during derivative
-                calculation.
-            return_descriptor (bool): Whether to also calculate the descriptor
-                in the same function call. Notice that it typically is faster
-                to calculate both in one go.
-            n_jobs (int): Number of parallel jobs to instantiate. Parallellizes
-                the calculation across samples. Defaults to serial calculation
-                with n_jobs=1. If a negative number is given, the number of jobs
-                will be calculated with, n_cpus + n_jobs, where n_cpus is the
-                amount of CPUs as reported by the OS. With only_physical_cores
-                you can control which types of CPUs are counted in n_cpus.
-            only_physical_cores (bool): If a negative n_jobs is given,
-                determines which types of CPUs are used in calculating the
-                number of jobs. If set to False (default), also virtual CPUs
-                are counted.  If set to True, only physical CPUs are counted.
-            verbose(bool): Controls whether to print the progress of each job
-                into to the console.
-
-        Returns:
-            If return_descriptor is True, returns a tuple, where the first item
-            is the derivative array and the second is the descriptor array.
-            Otherwise only returns the derivatives array. The derivatives array
-            is a either a 4D or 5D array, depending on whether you have
-            provided a single or multiple systems. If the output shape for each
-            system is the same, a single monolithic numpy array is returned.
-            For variable sized output (e.g. differently sized systems,
-            different number of centers or different number of included atoms),
-            a regular python list is returned. The dimensions are:
-            [(n_systems,) n_positions, n_atoms, 3, n_features]. The first
-            dimension goes over the different systems in case multiple were
-            given. The second dimension goes over the descriptor centers in
-            the same order as they were given in the argument. The third
-            dimension goes over the included atoms. The order is same as the
-            order of atoms in the given system. The fourth dimension goes over
-            the cartesian components, x, y and z. The fifth dimension goes over
-            the features in the default order.
+    def validate_derivatives_method(self, method, attach):
+        """Used to validate and determine the final method for calculating the
+        derivatives.
         """
         methods = {"numerical", "analytical", "auto"}
         if method not in methods:
             raise ValueError(
                 "Invalid method specified. Please choose from: {}".format(methods)
             )
-        if self.average != "off" and method == "analytical":
-            raise ValueError(
-                "Analytical derivatives not currently available for averaged output."
-            )
-        if self.periodic:
-            raise ValueError(
-                "Derivatives are currently not available for periodic systems."
-            )
-        if self._rbf == "polynomial" and method == "analytical":
-            raise ValueError(
-                "Analytical derivatives not currently available for polynomial "
-                "radial basis set."
-            )
-        if attach and method == "analytical":
-            raise ValueError(
-                "Analytical derivatives not currently available when attach=True."
-            )
+        if method == "numerical":
+            return method
 
-        # Determine the appropriate method if not given explicitly.
-        if method == "auto":
-            if self._rbf == "polynomial" or self.average != "off" or attach:
+        # Check if analytical derivatives can be used
+        try:
+            if self._rbf == "polynomial":
+                raise ValueError(
+                    "Analytical derivatives not currently available for polynomial "
+                    "radial basis set."
+                )
+            if self.average != "off":
+                raise ValueError(
+                    "Analytical derivatives not currently available for averaged output."
+                )
+            if self.periodic:
+                raise ValueError(
+                    "Analytical derivatives are currently not available for periodic systems."
+                )
+        except Exception as e:
+            if method == "analytical":
+                raise e
+            elif method == "auto":
                 method = "numerical"
-            else:
+        else:
+            if method == "auto":
                 method = "analytical"
 
-        # If single system given, skip the parallelization
-        if isinstance(system, (Atoms, System)):
-            n_atoms = len(system)
-            indices = self._get_indices(n_atoms, include, exclude)
-            return self.derivatives_single(
-                system,
-                positions,
-                indices,
-                method=method,
-                attach=attach,
-                return_descriptor=return_descriptor,
-            )
-
-        # Check input validity
-        n_samples = len(system)
-        if positions is None:
-            positions = [None] * n_samples
-        if include is None:
-            include = [None] * n_samples
-        elif is1d(include, np.integer):
-            include = [include] * n_samples
-        if exclude is None:
-            exclude = [None] * n_samples
-        elif is1d(exclude, np.integer):
-            exclude = [exclude] * n_samples
-        n_pos = len(positions)
-        if n_pos != n_samples:
-            raise ValueError(
-                "The given number of positions does not match the given "
-                "number of systems."
-            )
-        n_inc = len(include)
-        if n_inc != n_samples:
-            raise ValueError(
-                "The given number of includes does not match the given "
-                "number of systems."
-            )
-        n_exc = len(exclude)
-        if n_exc != n_samples:
-            raise ValueError(
-                "The given number of excludes does not match the given "
-                "number of systems."
-            )
-
-        # Determine the atom indices that are displaced
-        indices = []
-        for sys, inc, exc in zip(system, include, exclude):
-            n_atoms = len(sys)
-            indices.append(self._get_indices(n_atoms, inc, exc))
-
-        # Combine input arguments
-        inp = list(
-            zip(
-                system,
-                positions,
-                indices,
-                [method] * n_samples,
-                [attach] * n_samples,
-                [return_descriptor] * n_samples,
-            )
-        )
-
-        # For the descriptor, the output size for each job depends on the exact arguments.
-        # Here we precalculate the size for each job to preallocate memory and
-        # make the process faster.
-        n_features = self.get_number_of_features()
+        return method
 
-        def get_shapes(job):
-            centers = job[1]
-            if centers is None:
-                n_positions = len(job[0])
-            else:
-                n_positions = 1 if self.average != "off" else len(centers)
-            n_indices = len(job[2])
-            return (n_positions, n_indices, 3, n_features), (n_positions, n_features)
-
-        derivatives_shape, descriptor_shape = get_shapes(inp[0])
-
-        def is_variable(inp):
-            for job in inp[1:]:
-                i_der_shape, i_desc_shape = get_shapes(job)
-                if i_der_shape != derivatives_shape or i_desc_shape != descriptor_shape:
-                    return True
-            return False
-
-        if is_variable(inp):
-            derivatives_shape = None
-            descriptor_shape = None
-
-        # Create in parallel
-        output = self.derivatives_parallel(
-            inp,
-            self.derivatives_single,
-            n_jobs,
-            derivatives_shape,
-            descriptor_shape,
-            return_descriptor,
-            only_physical_cores,
-            verbose=verbose,
-        )
-
-        return output
-
-    def derivatives_single(
+    def derivatives_numerical(
         self,
+        d,
+        c,
         system,
-        positions,
+        centers,
         indices,
-        method="numerical",
-        attach=False,
+        attach,
         return_descriptor=True,
     ):
-        """Return the SOAP output for the given system and given positions.
-
+        """Return the numerical derivatives for the given system.
         Args:
             system (:class:`ase.Atoms`): Atomic structure.
-            positions (list): Positions where to calculate SOAP. Can be
-                provided as cartesian positions or atomic indices. If no
-                positions are defined, the SOAP output will be created for all
-                atoms in the system. When calculating SOAP for multiple
-                systems, provide the positions as a list for each system.
             indices (list): Indices of atoms for which the derivatives will be
                 computed for.
-            method (str): 'numerical' or 'analytical' derivatives. Numerical
-                derivatives are implemented with central finite difference. If
-                not specified, analytical derivatives are used when available.
-            attach (bool): Controls the behaviour of positions defined as
-                atomic indices. If True, the positions tied to an atomic index will
-                move together with the atoms with respect to which the derivatives
-                are calculated against. If False, positions defined as atomic
-                indices will be converted into cartesian locations that are
-                completely independent of the atom location during derivative
-                calculation.
             return_descriptor (bool): Whether to also calculate the descriptor
                 in the same function call. This is true by default as it
                 typically is faster to calculate both in one go.
-
         Returns:
             If return_descriptor is True, returns a tuple, where the first item
             is the derivative array and the second is the descriptor array.
             Otherwise only returns the derivatives array. The derivatives array
-            is a 4D numpy array. The dimensions are: [n_positions, n_atoms, 3,
-            n_features]. The first dimension goes over the SOAP centers in the
-            same order as they were given in the argument. The second dimension
-            goes over the included atoms. The order is same as the order of
-            atoms in the given system. The third dimension goes over the
-            cartesian components, x, y and z. The last dimension goes over the
-            features in the default order.
+            is a 3D numpy array. The dimensions are: [n_atoms, 3, n_features].
+            The first dimension goes over the included atoms. The order is same
+            as the order of atoms in the given system. The second dimension
+            goes over the cartesian components, x, y and z. The last dimension
+            goes over the features in the default order.
         """
-        cutoff_padding = self.get_cutoff_padding()
-        centers, center_indices = self.prepare_centers(
-            system, cutoff_padding, positions
-        )
         pos = system.get_positions()
         Z = system.get_atomic_numbers()
-        sorted_species = self._atomic_numbers
-        n_species = len(sorted_species)
-        n_centers = centers.shape[0]
-        n_indices = len(indices)
-        n_atoms = len(system)
-
-        n_features = self.get_number_of_features()
-        if return_descriptor:
-            c = self.init_descriptor_array(n_centers, n_features)
-        else:
-            c = np.empty(0)
-        d = self.init_derivatives_array(n_centers, n_indices, n_features)
+        cell = ase.geometry.cell.complete_cell(system.get_cell())
+        pbc = np.asarray(system.get_pbc(), dtype=bool)
+        cutoff_padding = self.get_cutoff_padding()
+        centers, center_indices = self.prepare_centers(system, centers)
 
         if self._rbf == "gto":
             alphas = self._alphas.flatten()
             betas = self._betas.flatten()
             soap_gto = dscribe.ext.SOAPGTO(
                 self._r_cut,
                 self._n_max,
@@ -908,109 +641,148 @@
                 alphas,
                 betas,
                 self._atomic_numbers,
                 self.periodic,
             )
 
             # Calculate numerically with extension
-            if method == "numerical":
-                soap_gto.derivatives_numerical(
-                    d,
-                    c,
-                    pos,
-                    Z,
-                    ase.geometry.cell.complete_cell(system.get_cell()),
-                    np.asarray(system.get_pbc(), dtype=bool),
-                    centers,
-                    center_indices,
-                    indices,
-                    attach,
-                    return_descriptor,
-                )
-            # Calculate analytically with extension
-            elif method == "analytical":
-                # These arrays are only used internally by the C++ code.
-                # Allocating them here with python is much faster than
-                # allocating similarly sized arrays within C++. It seems
-                # that numpy does some kind of lazy allocation that is
-                # highly efficient for zero-initialized arrays. Similar
-                # performace could not be achieved even with calloc.
-                xd = self.init_internal_dev_array(
-                    n_centers, n_atoms, n_species, self._n_max, self._l_max
-                )
-                yd = self.init_internal_dev_array(
-                    n_centers, n_atoms, n_species, self._n_max, self._l_max
-                )
-                zd = self.init_internal_dev_array(
-                    n_centers, n_atoms, n_species, self._n_max, self._l_max
-                )
-
-                soap_gto.derivatives_analytical(
-                    d,
-                    c,
-                    xd,
-                    yd,
-                    zd,
-                    pos,
-                    Z,
-                    ase.geometry.cell.complete_cell(system.get_cell()),
-                    np.asarray(system.get_pbc(), dtype=bool),
-                    centers,
-                    indices,
-                    return_descriptor,
-                )
-
+            soap_gto.derivatives_numerical(
+                d,
+                c,
+                pos,
+                Z,
+                cell,
+                pbc,
+                centers,
+                center_indices,
+                indices,
+                attach,
+                return_descriptor,
+            )
         elif self._rbf == "polynomial":
             rx, gss = self.get_basis_poly(self._r_cut, self._n_max)
             gss = gss.flatten()
 
             # Calculate numerically with extension
-            if method == "numerical":
-                soap_poly = dscribe.ext.SOAPPolynomial(
-                    self._r_cut,
-                    self._n_max,
-                    self._l_max,
-                    self._eta,
-                    self._weighting,
-                    self.crossover,
-                    self.average,
-                    cutoff_padding,
-                    rx,
-                    gss,
-                    self._atomic_numbers,
-                    self.periodic,
-                )
-                soap_poly.derivatives_numerical(
-                    d,
-                    c,
-                    pos,
-                    Z,
-                    ase.geometry.cell.complete_cell(system.get_cell()),
-                    np.asarray(system.get_pbc(), dtype=bool),
-                    centers,
-                    center_indices,
-                    indices,
-                    attach,
-                    return_descriptor,
-                )
+            soap_poly = dscribe.ext.SOAPPolynomial(
+                self._r_cut,
+                self._n_max,
+                self._l_max,
+                self._eta,
+                self._weighting,
+                self.crossover,
+                self.average,
+                cutoff_padding,
+                rx,
+                gss,
+                self._atomic_numbers,
+                self.periodic,
+            )
+            soap_poly.derivatives_numerical(
+                d,
+                c,
+                pos,
+                Z,
+                ase.geometry.cell.complete_cell(system.get_cell()),
+                np.asarray(system.get_pbc(), dtype=bool),
+                centers,
+                center_indices,
+                indices,
+                attach,
+                return_descriptor,
+            )
+
+    def derivatives_analytical(
+        self,
+        d,
+        c,
+        system,
+        centers,
+        indices,
+        attach,
+        return_descriptor=True,
+    ):
+        """Return the analytical derivatives for the given system.
+        Args:
+            system (:class:`ase.Atoms`): Atomic structure.
+            indices (list): Indices of atoms for which the derivatives will be
+                computed for.
+            return_descriptor (bool): Whether to also calculate the descriptor
+                in the same function call. This is true by default as it
+                typically is faster to calculate both in one go.
+        Returns:
+            If return_descriptor is True, returns a tuple, where the first item
+            is the derivative array and the second is the descriptor array.
+            Otherwise only returns the derivatives array. The derivatives array
+            is a 3D numpy array. The dimensions are: [n_atoms, 3, n_features].
+            The first dimension goes over the included atoms. The order is same
+            as the order of atoms in the given system. The second dimension
+            goes over the cartesian components, x, y and z. The last dimension
+            goes over the features in the default order.
+        """
+        pos = system.get_positions()
+        Z = system.get_atomic_numbers()
+        cell = ase.geometry.cell.complete_cell(system.get_cell())
+        pbc = np.asarray(system.get_pbc(), dtype=bool)
+        cutoff_padding = self.get_cutoff_padding()
+        centers, center_indices = self.prepare_centers(system, centers)
+        sorted_species = self._atomic_numbers
+        n_species = len(sorted_species)
+        n_centers = centers.shape[0]
+        n_atoms = len(system)
 
-        # Convert to the final output precision.
-        if self.dtype == "float32":
-            d = d.astype(self.dtype)
-            c = c.astype(self.dtype)
-
-        # Convert to sparse here. Currently everything up to this point is
-        # calculated with dense matrices. This imposes some memory limitations.
-        if self.sparse:
-            d = sp.COO.from_numpy(d)
-            c = sp.COO.from_numpy(c)
+        alphas = self._alphas.flatten()
+        betas = self._betas.flatten()
+        soap_gto = dscribe.ext.SOAPGTO(
+            self._r_cut,
+            self._n_max,
+            self._l_max,
+            self._eta,
+            self._weighting,
+            self.crossover,
+            self.average,
+            cutoff_padding,
+            alphas,
+            betas,
+            self._atomic_numbers,
+            self.periodic,
+        )
 
-        if return_descriptor:
-            return (d, c)
-        return d
+        # These arrays are only used internally by the C++ code.
+        # Allocating them here with python is much faster than
+        # allocating similarly sized arrays within C++. It seems
+        # that numpy does some kind of lazy allocation that is
+        # highly efficient for zero-initialized arrays. Similar
+        # performace could not be achieved even with calloc.
+        xd = self.init_internal_dev_array(
+            n_centers, n_atoms, n_species, self._n_max, self._l_max
+        )
+        yd = self.init_internal_dev_array(
+            n_centers, n_atoms, n_species, self._n_max, self._l_max
+        )
+        zd = self.init_internal_dev_array(
+            n_centers, n_atoms, n_species, self._n_max, self._l_max
+        )
+
+        soap_gto.derivatives_analytical(
+            d,
+            c,
+            xd,
+            yd,
+            zd,
+            pos,
+            Z,
+            cell,
+            pbc,
+            centers,
+            center_indices,
+            indices,
+            attach,
+            return_descriptor,
+        )
 
     @property
     def species(self):
         return self._species
 
     @species.setter
     def species(self, value):
```

### Comparing `dscribe-1.2.2/dscribe/ext/acsf.cpp` & `dscribe-2.0.0/dscribe/ext/acsf.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/acsf.h` & `dscribe-2.0.0/dscribe/ext/acsf.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/celllist.cpp` & `dscribe-2.0.0/dscribe/ext/celllist.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/celllist.h` & `dscribe-2.0.0/dscribe/ext/celllist.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/cm.cpp` & `dscribe-2.0.0/dscribe/ext/cm.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/cm.h` & `dscribe-2.0.0/dscribe/ext/cm.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/descriptor.cpp` & `dscribe-2.0.0/dscribe/ext/descriptor.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/descriptor.h` & `dscribe-2.0.0/dscribe/ext/descriptor.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/descriptorglobal.cpp` & `dscribe-2.0.0/dscribe/ext/descriptorglobal.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/descriptorglobal.h` & `dscribe-2.0.0/dscribe/ext/descriptorglobal.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/ext.cpp` & `dscribe-2.0.0/dscribe/ext/ext.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/geometry.cpp` & `dscribe-2.0.0/dscribe/ext/geometry.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/geometry.h` & `dscribe-2.0.0/dscribe/ext/geometry.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/mbtr.h` & `dscribe-2.0.0/dscribe/ext/mbtr.h`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 #include <numeric>
 #include <utility>
 #include <cmath>
 #include <iostream>
 #include <algorithm>
 #include <sstream>
 #include <stdexcept>
+#include <numeric>
+#include <pybind11/numpy.h>
 
+namespace py = pybind11;
 using namespace std;
 #define PI 3.1415926535897932384626433832795028841971693993751058209749445923078164062
 
 typedef tuple<int> index1d;
 typedef tuple<int, int> index2d;
 typedef tuple<int, int, int> index3d;
 
@@ -38,166 +41,166 @@
          * The atoms with indices < interactionLimit are considered to be
          * interacting with other atoms.
          * @param cellIndices 3D index of the periodically repeated cell in
          * which each atom is in the system
          * @param local Whether a local or a global MBTR is calculated.
          */
         MBTR(map<int,int> atomicNumberToIndexMap, int interactionLimit,  vector<vector<int>> cellIndices);
-        map<string, vector<float>> getK1(const vector<int> &Z, const string &geomFunc, const string &weightFunc, const map<string, float> &parameters, float min, float max, float sigma, int n);
-        map<string, vector<float>> getK2(const vector<int> &Z, const vector<vector<float>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, float> &parameters, float min, float max, float sigma, int n);
-        map<string, vector<float>> getK3(const vector<int> &Z, const vector<vector<float>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, float> &parameters, float min, float max, float sigma, int n);
-        vector<map<string, vector<float>>> getK2Local(const vector<int> &indices, const vector<int> &Z, const vector<vector<float>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, float> &parameters, float min, float max, float sigma, int n);
-        vector<map<string, vector<float>>> getK3Local(const vector<int> &indices, const vector<int> &Z, const vector<vector<float>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, float> &parameters, float min, float max, float sigma, int n);
-        vector<float> gaussian(float center, float weight, float start, float dx, float sigmasqrt2, int n);
-
-
+        void getK1(py::array_t<double> &descriptor, const vector<int> &Z, const string &geomFunc, const string &weightFunc, const map<string, double> &parameters, double min, double max, double sigma, int n);
+        void getK2(py::array_t<double> &descriptor, py::array_t<double> &derivatives, bool return_descriptor, bool return_derivatives, const vector<int> &Z, const vector<vector<double>> &positions, const vector<vector<double>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, double> &parameters, double min, double max, double sigma, int n);
+        void getK3(py::array_t<double> &descriptor, py::array_t<double> &derivatives, bool return_descriptor, bool return_derivatives, const vector<int> &Z, const vector<vector<double>> &positions, const vector<vector<double>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, double> &parameters, double min, double max, double sigma, int n);
+        vector<map<string, vector<double>>> getK2Local(const vector<int> &indices, const vector<int> &Z, const vector<vector<double>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, double> &parameters, double min, double max, double sigma, int n);
+        vector<map<string, vector<double>>> getK3Local(const vector<int> &indices, const vector<int> &Z, const vector<vector<double>> &distances, const vector<vector<int>> &neighbours, const string &geomFunc, const string &weightFunc, const map<string, double> &parameters, double min, double max, double sigma, int n);
+        vector<double> gaussian(double center, double weight, double start, double dx, double sigmasqrt2, int n);
+        vector<double> xgaussian(double center, double weight, double start, double dx, double sigma, int n);
+        
     private:
         const map<int,int> atomicNumberToIndexMap;
         const int interactionLimit;
         const vector<vector<int> > cellIndices;
 
         /**
          * Calculates the geometry function based on atomic numbers defined for
          * k=1.
          *
          * @param i Index of first atom.
          *
          * @return Atomic number for the given index.
          */
-        float k1GeomAtomicNumber(const int &i, const vector<int> &Z);
+        double k1GeomAtomicNumber(const int &i, const vector<int> &Z);
 
         /**
          * Weighting of 1. Usually used for finite small
          * systems.
          *
          * @param i Index of first atom.
          *
          * @return Weight of 1.
          */
-        float k1WeightUnity(const int &i);
+        double k1WeightUnity(const int &i);
         /**
          * Calculates the inverse distance geometry function defined for k=2.
          *
          * @return A map of inverse distance values for the given atomic pairs.
          */
         /**
          * Calculates the distance geometry function defined for k=2.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param distances Distance matrix
          *
          * @return Inverse distance between atoms.
          */
-        float k2GeomInverseDistance(const int &i, const int &j, const vector<vector<float> > &distances);
+        double k2GeomInverseDistance(const int &i, const int &j, const vector<vector<double> > &distances);
         /**
          * Weighting of 1 for all indices. Usually used for finite small
          * systems.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param distances Distance matrix
          *
          * @return Distance between atoms.
          */
-        float k2GeomDistance(const int &i, const int &j, const vector<vector<float> > &distances);
+        double k2GeomDistance(const int &i, const int &j, const vector<vector<double> > &distances);
         /**
          * Weighting of 1. Usually used for finite small
          * systems.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param distances Distance matrix
          *
          * @return Weight of 1.
          */
-        float k2WeightUnity(const int &i, const int &j, const vector<vector<float> > &distances);
+        double k2WeightUnity(const int &i, const int &j, const vector<vector<double> > &distances);
         /**
          * Weighting defined as e^(-sx), where x is the distance from
          * A->B and s is the scaling factor.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param distances Distance matrix
          * @param scale The prefactor in the exponential weighting.
          *
          * @return The exponential weight.
          */
-        float k2WeightExponential(const int &i, const int &j, const vector<vector<float> > &distances, float scale);
+        double k2WeightExponential(const int &i, const int &j, const vector<vector<double> > &distances, double scale);
         /**
          * Weighting defined as 1/(x^2), where x is the distance from
          * A->B.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param distances Distance matrix.
          *
          * @return The inverse of distance squared as weight.
          */
-        float k2WeightSquare(const int &i, const int &j, const vector<vector<float> > &distances);
+        double k2WeightSquare(const int &i, const int &j, const vector<vector<double> > &distances);
         /**
          * Calculates the cosine geometry function defined for k3.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param k Index of third atom.
          * @param distances Distance matrix
          *
          * @return The cosine value for the angle defined between the given
          * three atomic indices.
          */
-        float k3GeomCosine(const int &i, const int &j, const int &k, const vector<vector<float>> &distances);
+        double k3GeomCosine(const int &i, const int &j, const int &k, const vector<vector<double>> &distances);
         /**
          * Calculates the angle (degrees) geometry function defined for k3.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param k Index of third atom.
          * @param distances Distance matrix
          *
          * @return The angle defined between the given three atomic indices.
          * Between 0 and 180 degrees.
          */
-        float k3GeomAngle(const int &i, const int &j, const int &k, const vector<vector<float>> &distances);
+        double k3GeomAngle(const int &i, const int &j, const int &k, const vector<vector<double>> &distances);
         /**
          * Weighting of 1. Usually used for finite small
          * systems.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param k Index of third atom.
          * @param distances Distance matrix
          *
          * @return Weight of 1.
          */
-        float k3WeightUnity(const int &i, const int &j, const int &k, const vector<vector<float>> &distances);
+        double k3WeightUnity(const int &i, const int &j, const int &k, const vector<vector<double>> &distances);
         /**
          * Weighting defined as e^(-sx), where x is the distance from
          * A->B->C->A and s is the scaling factor.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param k Index of third atom.
          * @param distances Distance matrix
          * @param scale The prefactor in the exponential weighting.
          *
          * @return Exponential weight.
          */
-        float k3WeightExponential(const int &i, const int &j, const int &k, const vector<vector<float>> &distances, float scale);
+        double k3WeightExponential(const int &i, const int &j, const int &k, const vector<vector<double>> &distances, double scale);
         /**
          * Weighting defined by smooth cutoff function f(r) = 1 + y * (r/R)^(y+1)
          * - (y+1) * (r/R)^y, where r is the distance between atoms, y is
          * sharpness and R is the cutoff distance.
          *
          * @param i Index of first atom.
          * @param j Index of second atom.
          * @param k Index of third atom.
          * @param distances Distance matrix.
          * @param sharpness Sharpness of the function.
          * @param cutoff Cutoff distance of the weighting.
          *
          * @return Weight defined by smooth cutoff function.
          */
-        float k3WeightSmooth(const int &i, const int &j, const int &k, const vector<vector<float> > &distances, float sharpness, float cutoff);
+        double k3WeightSmooth(const int &i, const int &j, const int &k, const vector<vector<double> > &distances, double sharpness, double cutoff);
 };
 
-#endif
+#endif
```

### Comparing `dscribe-1.2.2/dscribe/ext/soap.cpp` & `dscribe-2.0.0/dscribe/ext/soap.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -89,36 +89,39 @@
 {
     // Empty mock arrays since we are not calculating the derivatives
     py::array_t<double> xd({1, 1, 1, 1, 1});
     py::array_t<double> yd({1, 1, 1, 1, 1});
     py::array_t<double> zd({1, 1, 1, 1, 1});
     py::array_t<double> derivatives({1, 1, 1, 1});
     py::array_t<int> indices({1});
+    py::array_t<int> center_indices({1});
 
     soapGTO(
         derivatives,
         out,
         xd,
         yd,
         zd,
         positions,
         centers,
+        center_indices,
         this->alphas,
         this->betas,
         atomic_numbers,
         this->species,
         this->rcut,
         this->cutoff_padding,
         this->nmax,
         this->lmax,
         this->eta,
         this->weighting,
         this->crossover,
         this->average,
         indices,
+        false,
         true,
         false,
         cell_list
     );
 }
 
 int SOAPGTO::get_number_of_features() const
@@ -136,15 +139,17 @@
     py::array_t<double> yd,
     py::array_t<double> zd,
     py::array_t<double> positions,
     py::array_t<int> atomic_numbers,
     py::array_t<double> cell,
     py::array_t<bool> pbc,
     py::array_t<double> centers,
+    py::array_t<int> center_indices,
     py::array_t<int> indices,
+    const bool attach,
     const bool return_descriptor
 ) const
 {
     // Extend system if periodicity is requested.
     auto pbc_u = pbc.unchecked<1>();
     bool is_periodic = this->periodic && (pbc_u(0) || pbc_u(1) || pbc_u(2));
     if (is_periodic) {
@@ -160,27 +165,29 @@
         derivatives,
         descriptor,
         xd,
         yd,
         zd,
         positions,
         centers,
+        center_indices,
         this->alphas,
         this->betas,
         atomic_numbers,
         this->species,
         this->rcut,
         this->cutoff_padding,
         this->nmax,
         this->lmax,
         this->eta,
         this->weighting,
         this->crossover,
         this->average,
         indices,
+        attach,
         return_descriptor,
         true,
         cell_list
     );
 }
 
 SOAPPolynomial::SOAPPolynomial(
```

### Comparing `dscribe-1.2.2/dscribe/ext/soap.h` & `dscribe-2.0.0/dscribe/ext/soap.h`

 * *Files 2% similar despite different names*

```diff
@@ -88,26 +88,28 @@
             py::array_t<double> yd,
             py::array_t<double> zd,
             py::array_t<double> positions,
             py::array_t<int> atomic_numbers,
             py::array_t<double> cell,
             py::array_t<bool> pbc,
             py::array_t<double> centers,
+            py::array_t<int> center_indices,
             py::array_t<int> indices,
+            const bool attach,
             const bool return_descriptor
         ) const;
 
     private:
         const double rcut;
         const int nmax;
         const int lmax;
         const double eta;
         const py::dict weighting;
         const bool crossover;
-        const float cutoff_padding;
+        const double cutoff_padding;
         const py::array_t<double> alphas;
         const py::array_t<double> betas;
         const py::array_t<int> species;
 };
 
 /**
  * SOAP descriptor with polynomial radial basis.
@@ -166,14 +168,14 @@
     private:
         const double rcut;
         const int nmax;
         const int lmax;
         const double eta;
         const py::dict weighting;
         const bool crossover;
-        const float cutoff_padding;
+        const double cutoff_padding;
         const py::array_t<double> rx;
         const py::array_t<double> gss;
         const py::array_t<int> species;
 };
 
 #endif
```

### Comparing `dscribe-1.2.2/dscribe/ext/soapGTO.cpp` & `dscribe-2.0.0/dscribe/ext/soapGTO.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -87,23 +87,23 @@
 
   int NsNs = Ns*Ns;
   double oneO1alpha;
   double oneO1alpha2;
   double oneO1alphaSqrt;
   double oneO1alphaSqrtX;
 
-  for(int myL = 0; myL < lMax + 1 ;myL++){
-    for(int k = 0; k < Ns; k++){
+  for (int myL = 0; myL < lMax + 1 ;myL++) {
+    for (int k = 0; k < Ns; k++) {
       oneO1alpha = 1.0/(1.0 + oOeta*alphas[myL*Ns + k]);
       oneO1alphaSqrt = sqrt(oneO1alpha);
       aOa[myL*Ns + k] = -alphas[myL*Ns + k]*oneO1alpha; 
       oneO1alpha2 = pow(oneO1alpha, myL+1);
       oneO1alphaSqrtX = oneO1alphaSqrt*oneO1alpha2;
-      for(int n = 0; n < Ns; n++){
-            bOa[myL*NsNs + n*Ns + k] = oOeta3O2*betas[myL*NsNs + n*Ns + k]*oneO1alphaSqrtX;
+      for (int n = 0; n < Ns; n++) {
+        bOa[myL*NsNs + n*Ns + k] = oOeta3O2*betas[myL*NsNs + n*Ns + k]*oneO1alphaSqrtX;
       } 
     }
   }
 }
 //================================================================
 void getCfactorsD(double* preCoef, double* prCofDX, double* prCofDY, double* prCofDZ, int Asize, double* x,double* x2, double* x4, double* x6, double* x8, double* x10,double* x12,double* x14,double* x16,double* x18, double* y,double* y2, double* y4, double* y6, double* y8, double* y10,double* y12,double* y14,double* y16,double* y18, double* z, double* z2, double* z4, double* z6, double* z8, double* z10,double* z12,double* z14,double* z16,double* z18, double* r2, double* r4, double* r6, double* r8,double* r10,double* r12,double* r14,double* r16,double* r18, double* r20,  double* x20,  double* y20,  double* z20, int totalAN, int lMax, bool return_derivatives){
 
@@ -1999,212 +1999,243 @@
     double* exes,
     int totalAN,
     int Asize,
     int Ns,
     int Ntypes,
     int lMax,
     int posI,
+    int posAtomI,
     int typeJ,
     const vector<int> &indices,
-    bool return_derivatives){
-  if(Asize == 0){return;}
+    bool attach,
+    bool return_derivatives) {
+  if (Asize == 0) {
+    return;
+  }
   double sumMe = 0; int NsNs = Ns*Ns; int LNsNs;
   int LNs;
   double preExp;
   double preVal;
   double preValX;
   double preValY;
   double preValZ;
 
-        double  preVal1;
-        double  preVal2;
-        double  preVal3;
-         
-        double  preValX1;
-        double  preValY1;
-        double  preValZ1;
-
-        double  preValX2;
-        double  preValY2;
-        double  preValZ2;
-
-        double  preValX3;
-        double  preValY3;
-        double  preValZ3;
-        double* preExponentArrya = (double*) malloc(Ns*Asize*sizeof(double));
-// l=0-------------------------------------------------------------------------------------------------
- int shift = 0;
-    for(int k = 0; k < Ns; k++){
-      for(int i = 0; i < Asize; i++){
-        preExponentArrya[shift] = weights[i]*1.5707963267948966*exp(aOa[k]*r2[i]);
-        shift++;
-      }}
+  double  preVal1;
+  double  preVal2;
+  double  preVal3;
+    
+  double  preValX1;
+  double  preValY1;
+  double  preValZ1;
+
+  double  preValX2;
+  double  preValY2;
+  double  preValZ2;
+
+  double  preValX3;
+  double  preValY3;
+  double  preValZ3;
+  double* preExponentArray = (double*) malloc(Ns*Asize*sizeof(double));
+
+  // l=0-------------------------------------------------------------------------------------------------
+  int shift = 0;
+  for (int k = 0; k < Ns; k++) {
+    for (int i = 0; i < Asize; i++) {
+      preExponentArray[shift] = weights[i]*1.5707963267948966*exp(aOa[k]*r2[i]);
+      shift++;
+    }
+  }
 
-    shift = 0;
-    for(int k = 0; k < Ns; k++){
-      sumMe = 0;
-      for(int i = 0; i < Asize; i++){
-        preExp = preExponentArrya[shift];
-        sumMe +=  preExp;
-        shift++;
-       }
-      for(int n = 0; n < Ns; n++){
-        C_mu(posI, typeJ, n, 0) += bOa[n*Ns + k]*sumMe;
-       } 
+  shift = 0;
+  for (int k = 0; k < Ns; k++) {
+    sumMe = 0;
+    for (int i = 0; i < Asize; i++) {
+      preExp = preExponentArray[shift];
+      sumMe += preExp;
+      shift++;
     }
-shift = 0;
-           if(return_derivatives){
-    for(int k = 0; k < Ns; k++){
-      for(int i = 0; i < Asize; i++){
-        preExp = preExponentArrya[shift];
+    for (int n = 0; n < Ns; n++) {
+      C_mu(posI, typeJ, n, 0) += bOa[n*Ns + k]*sumMe;
+    } 
+  }
+
+  shift = 0;
+  if (return_derivatives) {
+    for (int k = 0; k < Ns; k++) {
+      for (int i = 0; i < Asize; i++) {
+        preExp = preExponentArray[shift];
         shift++;
         preVal = 2.0*aOa[k]*preExp;
         preValX = preVal*x[i];
         preValY = preVal*y[i];
         preValZ = preVal*z[i];
-          for(int n = 0; n < Ns; n++){
-            CDevX_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValX;
-            CDevY_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValY;
-            CDevZ_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValZ;
-            }
-          } 
-      }
+        for (int n = 0; n < Ns; n++) {
+          CDevX_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValX;
+          CDevY_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValY;
+          CDevZ_mu(indices[i], posI, typeJ, n, 0) += bOa[n*Ns + k]*preValZ;
+        }
+      } 
     }
-// l=1-------------------------------------------------------------------------------------------------
-  if(lMax > 0) { LNsNs=NsNs; LNs=Ns;
-    shift = 0 ;
+  }
+
+  // l=1-------------------------------------------------------------------------------------------------
+  if (lMax > 0) { 
+    LNsNs = NsNs;
+    LNs = Ns;
 
-    for(int k = 0; k < Ns; k++){
-      for(int i = 0; i < Asize; i++){
-        preExponentArrya[shift] = weights[i]*2.7206990463849543*exp(aOa[LNs + k]*r2[i]);
+    shift = 0 ;
+    for (int k = 0; k < Ns; k++) {
+      for (int i = 0; i < Asize; i++) {
+        preExponentArray[shift] = weights[i]*2.7206990463849543*exp(aOa[LNs + k]*r2[i]);
         shift++;
-      }}
+      }
+    }
     
     shift = 0 ;
     double sumMe1;
     double sumMe2;
     double sumMe3;
-    for(int k = 0; k < Ns; k++){
+    for (int k = 0; k < Ns; k++) {
     sumMe1 = 0;
     sumMe2 = 0;
     sumMe3 = 0;
-      for(int i = 0; i < Asize; i++){
-        preExp = preExponentArrya[shift];
+      for (int i = 0; i < Asize; i++) {
+        preExp = preExponentArray[shift];
         sumMe1 += preExp*z[i];
         sumMe2 += preExp*x[i];
         sumMe3 += preExp*y[i];
         shift++;
       }
-        for(int n = 0; n < Ns; n++){
-          C_mu( posI, typeJ,n,1) += bOa[LNsNs + n*Ns + k]*sumMe1;
-          C_mu( posI, typeJ,n,2) += bOa[LNsNs + n*Ns + k]*sumMe2;
-          C_mu( posI, typeJ,n,3) += bOa[LNsNs + n*Ns + k]*sumMe3;
-          }
+      for (int n = 0; n < Ns; n++) {
+        C_mu(posI, typeJ, n, 1) += bOa[LNsNs + n*Ns + k]*sumMe1;
+        C_mu(posI, typeJ, n, 2) += bOa[LNsNs + n*Ns + k]*sumMe2;
+        C_mu(posI, typeJ, n, 3) += bOa[LNsNs + n*Ns + k]*sumMe3;
+      }
     }
 
-          if(return_derivatives){
-            shift = 0;
-    for(int k = 0; k < Ns; k++){
-      for(int i = 0; i < Asize; i++){
-        preExp = preExponentArrya[shift];
-        shift++;
+    if (return_derivatives) {
+      shift = 0;
+      for (int k = 0; k < Ns; k++) {
+        for (int i = 0; i < Asize; i++) {
+          preExp = preExponentArray[shift];
+          shift++;
           preVal = 2.0*aOa[LNs + k]*preExp;
-          if(return_derivatives){
-          preVal1 = preVal*z[i];
-          preVal2 = preVal*x[i];
-          preVal3 = preVal*y[i];
-         
-          preValX1 = preVal1*x[i];
-          preValY1 = preVal1*y[i];
-          preValZ1 = preVal1*z[i] + preExp;
-
-          preValX2 = preVal2*x[i] + preExp;
-          preValY2 = preVal2*y[i];
-          preValZ2 = preVal2*z[i];
-
-          preValX3 = preVal3*x[i];
-          preValY3 = preVal3*y[i] + preExp;
-          preValZ3 = preVal3*z[i];
-}
-        for(int n = 0; n < Ns; n++){
-          CDevX_mu(indices[i], posI, typeJ,n,1) += bOa[LNsNs + n*Ns + k]*preValX1;
-          CDevY_mu(indices[i], posI, typeJ,n,1) += bOa[LNsNs + n*Ns + k]*preValY1;
-          CDevZ_mu(indices[i], posI, typeJ,n,1) += bOa[LNsNs + n*Ns + k]*preValZ1;
-
-
-          CDevX_mu(indices[i], posI, typeJ,n,2) += bOa[LNsNs + n*Ns + k]*preValX2;
-          CDevY_mu(indices[i], posI, typeJ,n,2) += bOa[LNsNs + n*Ns + k]*preValY2;
-          CDevZ_mu(indices[i], posI, typeJ,n,2) += bOa[LNsNs + n*Ns + k]*preValZ2;
-
-
-          CDevX_mu(indices[i], posI, typeJ,n,3) += bOa[LNsNs + n*Ns + k]*preValX3;
-          CDevY_mu(indices[i], posI, typeJ,n,3) += bOa[LNsNs + n*Ns + k]*preValY3;
-          CDevZ_mu(indices[i], posI, typeJ,n,3) += bOa[LNsNs + n*Ns + k]*preValZ3;
-          
-          
+          if (return_derivatives) {
+            preVal1 = preVal*z[i];
+            preVal2 = preVal*x[i];
+            preVal3 = preVal*y[i];
+           
+            preValX1 = preVal1*x[i];
+            preValY1 = preVal1*y[i];
+            preValZ1 = preVal1*z[i] + preExp;
+
+            preValX2 = preVal2*x[i] + preExp;
+            preValY2 = preVal2*y[i];
+            preValZ2 = preVal2*z[i];
+
+            preValX3 = preVal3*x[i];
+            preValY3 = preVal3*y[i] + preExp;
+            preValZ3 = preVal3*z[i];
           }
-
+          for (int n = 0; n < Ns; n++) {
+            CDevX_mu(indices[i], posI, typeJ, n, 1) += bOa[LNsNs + n*Ns + k]*preValX1;
+            CDevY_mu(indices[i], posI, typeJ, n, 1) += bOa[LNsNs + n*Ns + k]*preValY1;
+            CDevZ_mu(indices[i], posI, typeJ, n, 1) += bOa[LNsNs + n*Ns + k]*preValZ1;
+
+            CDevX_mu(indices[i], posI, typeJ, n, 2) += bOa[LNsNs + n*Ns + k]*preValX2;
+            CDevY_mu(indices[i], posI, typeJ, n, 2) += bOa[LNsNs + n*Ns + k]*preValY2;
+            CDevZ_mu(indices[i], posI, typeJ, n, 2) += bOa[LNsNs + n*Ns + k]*preValZ2;
+
+            CDevX_mu(indices[i], posI, typeJ, n, 3) += bOa[LNsNs + n*Ns + k]*preValX3;
+            CDevY_mu(indices[i], posI, typeJ, n, 3) += bOa[LNsNs + n*Ns + k]*preValY3;
+            CDevZ_mu(indices[i], posI, typeJ, n, 3) += bOa[LNsNs + n*Ns + k]*preValZ3;
+          }
+        }
       }
     }
-  }}
+  }
+
 // l>2------------------------------------------------------------------------------------------------------
 //
 //[NsTs100*i_center*totalAN + Ns100*jd*totalAN + buffShift*totalAN*Ns + kd*totalAN + i_atom]
 //
-  if(lMax > 1) { 
-    for(int restOfLs = 2; restOfLs <= lMax; restOfLs++){	 
-    LNsNs=restOfLs*NsNs; LNs=restOfLs*Ns; 
-shift = 0;
-      for(int k = 0; k < Ns; k++){
-        for(int i = 0; i < Asize; i++){
+  if (lMax > 1) { 
+    for (int restOfLs = 2; restOfLs <= lMax; restOfLs++) {	 
+      LNsNs=restOfLs*NsNs; LNs=restOfLs*Ns; 
+      shift = 0;
+      for (int k = 0; k < Ns; k++) {
+        for (int i = 0; i < Asize; i++) {
           double expSholder = aOa[LNs + k]*r2[i];
-          preExponentArrya[shift] = weights[i]*exp(expSholder);
+          preExponentArray[shift] = weights[i]*exp(expSholder);
           shift++;
-        }}
+        }
+      }
 
       //double*  sumS = (double*) malloc(sizeof(double)*(restOfLs+1)*(restOfLs+1))
-shift = 0;
-      for(int k = 0; k < Ns; k++){
-          for(int m = restOfLs*restOfLs; m < (restOfLs+1)*(restOfLs+1); m++){
-        sumMe = 0;
-      for(int i = 0; i < Asize; i++){
-        preExp = preExponentArrya[Asize*k+i];
-        sumMe += preExp*preCoef[totalAN*(m-4)+i];
-        shift++;
-      }
-            for(int n = 0; n < Ns; n++){
-              C_mu( posI, typeJ,n,m) += bOa[LNsNs + n*Ns + k]*sumMe;
-             }
+      shift = 0;
+      for (int k = 0; k < Ns; k++) {
+        for (int m = restOfLs*restOfLs; m < (restOfLs+1)*(restOfLs+1); m++) {
+          sumMe = 0;
+          for (int i = 0; i < Asize; i++) {
+            preExp = preExponentArray[Asize*k+i];
+            sumMe += preExp*preCoef[totalAN*(m-4)+i];
+            shift++;
+          }
+          for (int n = 0; n < Ns; n++) {
+            C_mu(posI, typeJ, n, m) += bOa[LNsNs + n*Ns + k]*sumMe;
           }
+        }
       }
 
-           if(return_derivatives){
-             shift = 0;
-      for(int k = 0; k < Ns; k++){
-        for(int i = 0; i < Asize; i++){
-          preExp = preExponentArrya[shift];
+      if (return_derivatives) {
+        shift = 0;
+        for (int k = 0; k < Ns; k++) {
+          for (int i = 0; i < Asize; i++) {
+            preExp = preExponentArray[shift];
             shift++;
-          for(int m = restOfLs*restOfLs; m < (restOfLs+1)*(restOfLs+1); m++){
-            preVal = 2.0*aOa[LNs + k]*preExp*preCoef[totalAN*(m-4)+i];
-            preValX = x[i]*preVal + preExp*prCofDX[totalAN*(m-4)+i];
-            preValY = y[i]*preVal + preExp*prCofDY[totalAN*(m-4)+i];
-            preValZ = z[i]*preVal + preExp*prCofDZ[totalAN*(m-4)+i];
-            for(int n = 0; n < Ns; n++){
-          CDevX_mu(indices[i], posI, typeJ,n,m) += bOa[LNsNs + n*Ns + k]*preValX;
-          CDevY_mu(indices[i], posI, typeJ,n,m) += bOa[LNsNs + n*Ns + k]*preValY;
-          CDevZ_mu(indices[i], posI, typeJ,n,m) += bOa[LNsNs + n*Ns + k]*preValZ;
-          
-               }
+            for (int m = restOfLs*restOfLs; m < (restOfLs+1)*(restOfLs+1); m++) {
+              preVal = 2.0*aOa[LNs + k]*preExp*preCoef[totalAN*(m-4)+i];
+              preValX = x[i]*preVal + preExp*prCofDX[totalAN*(m-4)+i];
+              preValY = y[i]*preVal + preExp*prCofDY[totalAN*(m-4)+i];
+              preValZ = z[i]*preVal + preExp*prCofDZ[totalAN*(m-4)+i];
+              for (int n = 0; n < Ns; n++) {
+                CDevX_mu(indices[i], posI, typeJ, n, m) += bOa[LNsNs + n*Ns + k]*preValX;
+                CDevY_mu(indices[i], posI, typeJ, n, m) += bOa[LNsNs + n*Ns + k]*preValY;
+                CDevZ_mu(indices[i], posI, typeJ, n, m) += bOa[LNsNs + n*Ns + k]*preValZ;
+              }
             }
+          }
         }
       }
     }
   }
-}
-free(preExponentArrya);
+  free(preExponentArray);
+
+  // If attach=True, the derivative with respect to the center atom coordinates
+  // is the negative sum of derivatives with respect to coordinates of other
+  // atoms in the the neighbourhood.
+  if (return_derivatives && attach && (posAtomI >= 0)) {
+    for (int m = 0; m < (lMax+1)*(lMax+1); m++) {
+      for (int n = 0; n < Ns; n++) {
+        double sumX = 0;
+        double sumY = 0;
+        double sumZ = 0;
+        for (int i = 0; i < Asize; i++) {
+          if (indices[i] != posAtomI) {
+            sumX += CDevX_mu(indices[i], posI, typeJ,n,m);
+            sumY += CDevY_mu(indices[i], posI, typeJ,n,m);
+            sumZ += CDevZ_mu(indices[i], posI, typeJ,n,m);
+          }
+        }
+        CDevX_mu(posAtomI, posI, typeJ,n,m) = -sumX;
+        CDevY_mu(posAtomI, posI, typeJ,n,m) = -sumY;
+        CDevZ_mu(posAtomI, posI, typeJ,n,m) = -sumZ;
+      }
+    }
+  }
 }
 //================================================================================================
 /**
  * Used to calculate the partial power spectrum.
  */
 void getPD(
   py::detail::unchecked_mutable_reference<double, 2> &descriptor_mu,
@@ -2343,27 +2374,29 @@
     py::array_t<double> derivatives,
     py::array_t<double> descriptor,
     py::array_t<double> cdevX,
     py::array_t<double> cdevY,
     py::array_t<double> cdevZ,
     py::array_t<double> positions,
     py::array_t<double> centers,
+    py::array_t<int> center_indices,
     py::array_t<double> alphasArr,
     py::array_t<double> betasArr,
     py::array_t<int> atomicNumbersArr,
     py::array_t<int> orderedSpeciesArr,
     const double rCut,
     const double cutoffPadding,
     const int nMax,
     const int lMax,
     const double eta,
     py::dict weighting,
     const bool crossover,
     string average,
     py::array_t<int> indices,
+    const bool attach,
     const bool return_descriptor,
     const bool return_derivatives,
     CellList cell_list_atoms
 ) {
   const int totalAN = atomicNumbersArr.shape(0);
   const int nCenters = centers.shape(0);
   auto derivatives_mu = derivatives.mutable_unchecked<4>();
@@ -2373,14 +2406,15 @@
   auto indices_u = indices.unchecked<1>();
   double *alphas = (double*)alphasArr.request().ptr;
   double *betas = (double*)betasArr.request().ptr;
   double oOeta = 1.0/eta;
   double oOeta3O2 = sqrt(oOeta*oOeta*oOeta);
   double nMax2 = nMax*nMax;
   auto centers_u = centers.unchecked<2>(); 
+  auto center_indices_u = center_indices.unchecked<1>(); 
   auto positions_u = positions.unchecked<2>(); 
   const int nFeatures = crossover
         ? (nSpecies*nMax)*(nSpecies*nMax+1)/2*(lMax+1) 
         : nSpecies*(lMax+1)*((nMax+1)*nMax)/2;
   double* weights = (double*) malloc(sizeof(double)*totalAN);
   double* dx  = (double*)malloc(sizeof(double)*totalAN); double* dy  = (double*)malloc(sizeof(double)*totalAN); double* dz  = (double*)malloc(sizeof(double)*totalAN);
   double* x2  = (double*)malloc(sizeof(double)*totalAN); double* x4  = (double*)malloc(sizeof(double)*totalAN); double* x6  = (double*)malloc(sizeof(double)*totalAN);
@@ -2446,14 +2480,16 @@
       ZIndexMap[species(i)] = i;
   }
 
   getAlphaBetaD(aOa,bOa,alphas,betas,nMax,lMax,oOeta, oOeta3O2);
 
   // Loop through the centers
   for (int i = 0; i < nCenters; i++) {
+    // If computing derivatives with attach=True, index of the center atom is needed
+    int centerAtomI = (return_derivatives && attach) ? center_indices_u(i) : -1;
 
     // Get all neighbouring atoms for the center i
     double ix = centers_u(i, 0); double iy = centers_u(i, 1); double iz = centers_u(i, 2);
     CellListResult result = cell_list_atoms.getNeighboursForPosition(ix, iy, iz);
 
     // Sort the neighbours by type
     map<int, vector<int>> atomicTypeMap;
@@ -2467,30 +2503,30 @@
       int n_neighbours = ZIndexPair.second.size();
 
       // Save the neighbour distances into the arrays dx, dy and dz
       getDeltaD(dx, dy, dz, positions, ix, iy, iz, ZIndexPair.second);
       getRsZsD(dx, x2, x4, x6, x8, x10, x12, x14, x16, x18, dy, y2, y4, y6, y8, y10, y12, y14, y16, y18, dz, r2, r4, r6, r8, r10, r12, r14, r16, r18,  z2, z4, z6, z8, z10, z12, z14, z16, z18, r20, x20, y20, z20, n_neighbours, lMax);
       getWeights(n_neighbours, r1, r2, true, weighting, weights);
       getCfactorsD(preCoef, prCofDX, prCofDY, prCofDZ, n_neighbours, dx,x2, x4, x6, x8,x10,x12,x14,x16,x18, dy,y2, y4, y6, y8,y10,y12,y14,y16,y18, dz, z2, z4, z6, z8,z10,z12,z14,z16,z18, r2, r4, r6, r8,r10,r12,r14,r16,r18,r20, x20,y20,z20, totalAN, lMax, return_derivatives);
-      getCD(cdevX_mu, cdevY_mu, cdevZ_mu, prCofDX, prCofDY, prCofDZ, cnnd_mu, preCoef, dx, dy, dz, r2, weights, bOa, aOa, exes, totalAN, n_neighbours, nMax, nSpecies, lMax, i, j, ZIndexPair.second, return_derivatives);
+      getCD(cdevX_mu, cdevY_mu, cdevZ_mu, prCofDX, prCofDY, prCofDZ, cnnd_mu, preCoef, dx, dy, dz, r2, weights, bOa, aOa, exes, totalAN, n_neighbours, nMax, nSpecies, lMax, i, centerAtomI, j, ZIndexPair.second, attach, return_derivatives);
     }
   }
   free(dx); free(x2); free(x4); free(x6); free(x8); free(x10); free(x12); free(x14); free(x16); free(x18);
   free(dy); free(y2); free(y4); free(y6); free(y8); free(y10); free(y12); free(y14); free(y16); free(y18);
   free(dz); free(z2); free(z4); free(z6); free(z8); free(z10); free(z12); free(z14); free(z16); free(z18);
   free(r1);
   free(r2); free(r4); free(r6); free(r8); free(r10); free(r12); free(r14); free(r16); free(r18);
   free(r20);
   free(x20);
   free(y20);
   free(z20);
   free(exes); free(preCoef); free(bOa); free(aOa); free(cnnd_raw); free(weights);
 
   if (return_derivatives) {
-  free(prCofDX); free(prCofDY); free(prCofDZ);
+    free(prCofDX); free(prCofDY); free(prCofDZ);
   }
 
   // Calculate the descriptor value if requested
   if (return_descriptor) {
     auto descriptor_mu = descriptor.mutable_unchecked<2>();
 
     // If inner averaging is requested, average the coefficients over the
```

### Comparing `dscribe-1.2.2/dscribe/ext/soapGTO.h` & `dscribe-2.0.0/dscribe/ext/soapGTO.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,27 +33,29 @@
     py::array_t<double> derivatives,
     py::array_t<double> descriptor,
     py::array_t<double> cdevX,
     py::array_t<double> cdevY,
     py::array_t<double> cdevZ,
     py::array_t<double> positions,
     py::array_t<double> centers,
+    py::array_t<int> center_indices,
     py::array_t<double> alphasArr,
     py::array_t<double> betasArr,
     py::array_t<int> atomicNumbersArr,
     py::array_t<int> orderedSpeciesArr,
     const double rCut,
     const double cutoffPadding,
     const int Ns,
     const int lMax,
     const double eta,
     py::dict weighting,
     const bool crossover,
     string average,
     py::array_t<int> indices,
+    const bool attach,
     const bool return_descriptor,
     const bool return_derivatives,
     CellList cell_list
 );
 
 #endif
```

### Comparing `dscribe-1.2.2/dscribe/ext/soapGeneral.cpp` & `dscribe-2.0.0/dscribe/ext/soapGeneral.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/soapGeneral.h` & `dscribe-2.0.0/dscribe/ext/soapGeneral.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/weighting.cpp` & `dscribe-2.0.0/dscribe/ext/weighting.cpp`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/ext/weighting.h` & `dscribe-2.0.0/dscribe/ext/weighting.h`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/kernels/__init__.py` & `dscribe-2.0.0/dscribe/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/kernels/averagekernel.py` & `dscribe-2.0.0/dscribe/kernels/averagekernel.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/kernels/localsimilaritykernel.py` & `dscribe-2.0.0/dscribe/kernels/localsimilaritykernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         # First calculate the "raw" pairwise similarity of atomic environments
         n_x = len(x)
         n_y = len(y)
 
         C_ij_dict = {}
         for i in range(n_x):
             for j in range(n_y):
-
                 # Skip lower triangular part for symmetric matrices
                 if symmetric and j < i:
                     continue
 
                 x_i = x[i]
 
                 # Save time on symmetry
@@ -118,15 +117,14 @@
                 C_ij_dict[i, j] = C_ij
 
         # Calculate the global pairwise similarity between the entire
         # structures
         K_ij = np.zeros((n_x, n_y))
         for i in range(n_x):
             for j in range(n_y):
-
                 # Skip lower triangular part for symmetric matrices
                 if symmetric and j < i:
                     continue
 
                 C_ij = C_ij_dict[i, j]
                 k_ij = self.get_global_similarity(C_ij)
                 K_ij[i, j] = k_ij
```

### Comparing `dscribe-1.2.2/dscribe/kernels/rematchkernel.py` & `dscribe-2.0.0/dscribe/kernels/rematchkernel.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/utils/__init__.py` & `dscribe-2.0.0/dscribe/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/utils/dimensionality.py` & `dscribe-2.0.0/dscribe/utils/dimensionality.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe/utils/geometry.py` & `dscribe-2.0.0/dscribe/utils/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     ny = int(cell_images[1]) if pbc[1] else 0
     nz = int(cell_images[2]) if pbc[2] else 0
     n_copies_axis = np.array([nx, ny, nz], dtype=int)
 
     # If no centers are given, and the cell indices are not requested, simply
     # return the multiplied system. This is much faster.
     if centers is None and not return_cell_indices:
-
         n_atoms = len(system)
         n_rep = np.product(2 * n_copies_axis + 1)  # Number of repeated copies
         ext_pos = np.tile(system.get_positions(), (n_rep, 1))
 
         # Calculate the extended system positions so that the original cell
         # stays in place: both in space and in index
         i_curr = 0
```

### Comparing `dscribe-1.2.2/dscribe/utils/species.py` & `dscribe-2.0.0/dscribe/utils/species.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     # Determine if the given species are atomic numbers or chemical symbols
     if all(isinstance(x, (int, np.integer)) for x in species):
         if any([x < 0 for x in species]):
             raise ValueError(
                 "The given list of species contains negative integers. Please use only non-negative integers"
             )
         atomic_numbers = species
-    elif all(isinstance(x, (str, np.str)) for x in species):
+    elif all(isinstance(x, (str, np.str_)) for x in species):
         atomic_numbers = symbols_to_numbers(species)
     else:
         raise ValueError(
             "The given list of species does not seem to contain strictly "
             "chemical symbols or atomic numbers. Please use either one."
         )
```

### Comparing `dscribe-1.2.2/dscribe/utils/stats.py` & `dscribe-2.0.0/dscribe/utils/stats.py`

 * *Files identical despite different names*

### Comparing `dscribe-1.2.2/dscribe.egg-info/PKG-INFO` & `dscribe-2.0.0/dscribe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: dscribe
-Version: 1.2.2
+Version: 2.0.0
 Summary: A Python package for creating feature transformations in applications of machine learning to materials science.
 Home-page: https://singroup.github.io/dscribe/
 License: Apache License 2.0
+Description: A Python package for creating feature transformations in applications of machine learning to materials science.
 Keywords: descriptor machine learning atomistic structure materials science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-License-File: LICENSE
-
-A Python package for creating feature transformations in applications of machine learning to materials science.
-
+Requires-Python: >=3.7
```

### Comparing `dscribe-1.2.2/dscribe.egg-info/SOURCES.txt` & `dscribe-2.0.0/dscribe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -375,17 +375,19 @@
 dscribe/core/__init__.py
 dscribe/core/lattice.py
 dscribe/core/system.py
 dscribe/descriptors/__init__.py
 dscribe/descriptors/acsf.py
 dscribe/descriptors/coulombmatrix.py
 dscribe/descriptors/descriptor.py
+dscribe/descriptors/descriptorglobal.py
+dscribe/descriptors/descriptorlocal.py
+dscribe/descriptors/descriptormatrix.py
 dscribe/descriptors/ewaldsummatrix.py
 dscribe/descriptors/lmbtr.py
-dscribe/descriptors/matrixdescriptor.py
 dscribe/descriptors/mbtr.py
 dscribe/descriptors/sinematrix.py
 dscribe/descriptors/soap.py
 dscribe/descriptors/valleoganov.py
 dscribe/ext/acsf.cpp
 dscribe/ext/acsf.h
 dscribe/ext/celllist.cpp
@@ -413,8 +415,20 @@
 dscribe/kernels/averagekernel.py
 dscribe/kernels/localsimilaritykernel.py
 dscribe/kernels/rematchkernel.py
 dscribe/utils/__init__.py
 dscribe/utils/dimensionality.py
 dscribe/utils/geometry.py
 dscribe/utils/species.py
-dscribe/utils/stats.py
+dscribe/utils/stats.py
+tests/test_acsf.py
+tests/test_coulombmatrix.py
+tests/test_ewaldsummatrix.py
+tests/test_examples.py
+tests/test_general.py
+tests/test_kernels.py
+tests/test_lmbtr.py
+tests/test_mbtr.py
+tests/test_sinematrix.py
+tests/test_soap.py
+tests/test_valle_oganov.py
+tests/testutils.py
```

### Comparing `dscribe-1.2.2/setup.py` & `dscribe-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 # Check python version
-if sys.version_info[:2] < (3, 6):
-    raise RuntimeError("Python version >= 3.6 required.")
+if sys.version_info[:2] < (3, 7):
+    raise RuntimeError("Python version >= 3.7 required.")
 
 import platform
 from distutils.ccompiler import new_compiler
 from distutils.sysconfig import customize_compiler
 from setuptools import setup, find_packages, Extension
 from subprocess import getoutput
 
@@ -80,15 +80,15 @@
         extra_link_args=cpp_extra_link_args,
     )
 ]
 
 if __name__ == "__main__":
     setup(
         name="dscribe",
-        version="1.2.2",
+        version="2.0.0",
         url="https://singroup.github.io/dscribe/",
         description="A Python package for creating feature transformations in applications of machine learning to materials science.",
         long_description="A Python package for creating feature transformations in applications of machine learning to materials science.",
         packages=find_packages(),
         setup_requires=['pybind11>=2.4'],
         install_requires=['pybind11>=2.4', "numpy", "scipy", "ase>=3.19.0", "scikit-learn", "joblib>=1.0.0", "sparse"],
         include_package_data=True,  # This ensures that files defined in MANIFEST.in are included
@@ -103,17 +103,16 @@
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: MacOS",
             "Operating System :: Unix",
             "Programming Language :: C",
             "Programming Language :: C++",
             "Programming Language :: Python",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3 :: Only",
         ],
         keywords="descriptor machine learning atomistic structure materials science",
-        python_requires=">=3.6",
+        python_requires=">=3.7",
     )
```

