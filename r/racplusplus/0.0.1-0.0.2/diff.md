# Comparing `tmp/racplusplus-0.0.1.tar.gz` & `tmp/racplusplus-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racplusplus-0.0.1.tar", last modified: Sat Jun 24 00:10:01 2023, max compression
+gzip compressed data, was "racplusplus-0.0.2.tar", last modified: Sat Jun 24 00:59:04 2023, max compression
```

## Comparing `racplusplus-0.0.1.tar` & `racplusplus-0.0.2.tar`

### file list

```diff
@@ -1,417 +1,417 @@
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.879769 racplusplus-0.0.1/
--rw-r--r--   0 danielfrees   (501) staff       (20)      195 2023-06-23 23:14:41.000000 racplusplus-0.0.1/.gitignore
--rw-r--r--   0 danielfrees   (501) staff       (20)     3136 2023-06-23 23:28:01.000000 racplusplus-0.0.1/CMakeLists.txt
--rw-r--r--   0 danielfrees   (501) staff       (20)     1056 2023-06-24 00:05:14.000000 racplusplus-0.0.1/LICENSE
--rw-r--r--   0 danielfrees   (501) staff       (20)      923 2023-06-24 00:10:01.879280 racplusplus-0.0.1/PKG-INFO
--rw-r--r--   0 danielfrees   (501) staff       (20)      350 2023-06-24 00:01:35.000000 racplusplus-0.0.1/README.md
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.336501 racplusplus-0.0.1/_skbuild/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.336773 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.337060 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.337256 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.369629 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/
--rw-r--r--   0 danielfrees   (501) staff       (20)      118 2023-06-23 23:57:46.000000 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/__init__.py
--rwxr-xr-x   0 danielfrees   (501) staff       (20)   248552 2023-06-23 23:47:06.000000 racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/_racplusplus.cpython-311-darwin.so
--rw-r--r--   0 danielfrees   (501) staff       (20)     5114 2023-06-24 00:01:20.000000 racplusplus-0.0.1/oldbuild.md
--rw-r--r--   0 danielfrees   (501) staff       (20)      807 2023-06-23 23:59:19.000000 racplusplus-0.0.1/pyproject.toml
--rw-r--r--   0 danielfrees   (501) staff       (20)       38 2023-06-24 00:10:01.879925 racplusplus-0.0.1/setup.cfg
--rw-r--r--   0 danielfrees   (501) staff       (20)      169 2023-06-23 23:58:37.000000 racplusplus-0.0.1/setup.py
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.338780 racplusplus-0.0.1/src/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.386401 racplusplus-0.0.1/src/racplusplus/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.418690 racplusplus-0.0.1/src/racplusplus/Eigen/
--rw-r--r--   0 danielfrees   (501) staff       (20)     1161 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Cholesky
--rw-r--r--   0 danielfrees   (501) staff       (20)     1900 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/CholmodSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)    12799 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Core
--rw-r--r--   0 danielfrees   (501) staff       (20)      122 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Dense
--rw-r--r--   0 danielfrees   (501) staff       (20)       35 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Eigen
--rw-r--r--   0 danielfrees   (501) staff       (20)     1777 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Eigenvalues
--rw-r--r--   0 danielfrees   (501) staff       (20)     1940 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Geometry
--rw-r--r--   0 danielfrees   (501) staff       (20)      829 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Householder
--rw-r--r--   0 danielfrees   (501) staff       (20)     2083 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/IterativeLinearSolvers
--rw-r--r--   0 danielfrees   (501) staff       (20)      894 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Jacobi
--rw-r--r--   0 danielfrees   (501) staff       (20)     1389 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/KLUSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     1268 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/LU
--rw-r--r--   0 danielfrees   (501) staff       (20)      991 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/MetisSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     2451 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/OrderingMethods
--rw-r--r--   0 danielfrees   (501) staff       (20)     1751 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/PaStiXSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     1116 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/PardisoSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     1272 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/QR
--rw-r--r--   0 danielfrees   (501) staff       (20)      900 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/QtAlignedMalloc
--rw-r--r--   0 danielfrees   (501) staff       (20)     1162 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SPQRSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     1584 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SVD
--rw-r--r--   0 danielfrees   (501) staff       (20)      888 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/Sparse
--rw-r--r--   0 danielfrees   (501) staff       (20)     1235 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SparseCholesky
--rw-r--r--   0 danielfrees   (501) staff       (20)     2240 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SparseCore
--rw-r--r--   0 danielfrees   (501) staff       (20)     1814 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SparseLU
--rw-r--r--   0 danielfrees   (501) staff       (20)     1195 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SparseQR
--rw-r--r--   0 danielfrees   (501) staff       (20)      797 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/StdDeque
--rw-r--r--   0 danielfrees   (501) staff       (20)      726 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/StdList
--rw-r--r--   0 danielfrees   (501) staff       (20)      803 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/StdVector
--rw-r--r--   0 danielfrees   (501) staff       (20)     2243 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/SuperLUSupport
--rw-r--r--   0 danielfrees   (501) staff       (20)     1382 2023-06-23 23:19:24.000000 racplusplus-0.0.1/src/racplusplus/Eigen/UmfPackSupport
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.358084 racplusplus-0.0.1/src/racplusplus/Eigen/src/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.422166 racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/
--rw-r--r--   0 danielfrees   (501) staff       (20)    24934 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    18760 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3974 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.423302 racplusplus-0.0.1/src/racplusplus/Eigen/src/CholmodSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    25441 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.531695 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/
--rw-r--r--   0 danielfrees   (501) staff       (20)    19214 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    16782 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Array.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8217 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7018 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2738 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Assign.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    41673 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12488 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14075 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    18648 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Block.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4429 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5981 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6990 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    63841 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4745 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7909 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    36282 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8256 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3937 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5551 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    31529 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    24484 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    25360 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9870 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14670 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)      988 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11654 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Dot.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5841 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4909 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5759 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21679 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    38812 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11543 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8238 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/IO.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9620 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3503 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Inverse.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7256 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Map.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11281 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MapBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    60784 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7156 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    24343 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Matrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    23856 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2520 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3620 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12884 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9207 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    20748 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    49193 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7336 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Product.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    53832 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7756 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Random.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    19195 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Redux.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17821 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Ref.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5656 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Replicate.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17033 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4284 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7522 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Reverse.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6143 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Select.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14999 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1697 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6837 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Solve.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9368 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6170 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8700 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21641 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4212 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Stride.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2765 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Swap.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17606 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Transpose.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13567 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    38277 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3488 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    35168 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11997 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.348308 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.547779 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 danielfrees   (501) staff       (20)    15223 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8102 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    64608 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2564 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.565822 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 danielfrees   (501) staff       (20)    17160 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13344 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    87891 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2134 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.574911 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 danielfrees   (501) staff       (20)    16540 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2323 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)   119355 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9490 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    24820 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rw-r--r--   0 danielfrees   (501) staff       (20)   102394 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.578711 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 danielfrees   (501) staff       (20)    17317 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/CUDA/Complex.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.587632 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/
--rw-r--r--   0 danielfrees   (501) staff       (20)    26903 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5251 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    67696 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3770 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    35534 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1746 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3746 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.591478 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 danielfrees   (501) staff       (20)     2695 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    57047 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2256 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.346468 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.592311 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 danielfrees   (501) staff       (20)      691 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.596641 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 danielfrees   (501) staff       (20)    17541 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    16159 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    33615 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.606343 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 danielfrees   (501) staff       (20)    22503 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6815 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3083 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)   189525 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    51286 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.619366 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 danielfrees   (501) staff       (20)    14251 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6765 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    64465 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3650 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.622838 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 danielfrees   (501) staff       (20)     1194 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21200 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1351 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.628734 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 danielfrees   (501) staff       (20)     7428 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12539 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    27786 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21856 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2626 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.631961 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 danielfrees   (501) staff       (20)    16728 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8024 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    36894 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.645265 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/
--rw-r--r--   0 danielfrees   (501) staff       (20)     6686 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    20921 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8334 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4998 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 danielfrees   (501) staff       (20)      607 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    40146 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.680531 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/
--rw-r--r--   0 danielfrees   (501) staff       (20)   108448 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    20104 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15948 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6936 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5106 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21724 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6368 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5582 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21354 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11570 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9958 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5209 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6164 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4126 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    20987 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13867 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14722 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    10571 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14678 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6707 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5882 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.723010 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/
--rw-r--r--   0 danielfrees   (501) staff       (20)    23156 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    19876 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21931 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4892 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15555 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6696 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    10949 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/IntegralConstant.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4268 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    52909 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    46661 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    29336 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 danielfrees   (501) staff       (20)       85 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1024 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1432 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    10676 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12003 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    35762 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.736928 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/
--rw-r--r--   0 danielfrees   (501) staff       (20)    12559 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17274 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4178 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    22970 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17176 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9716 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14349 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5575 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    23640 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21078 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3650 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    35182 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4104 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    22764 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.750822 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/
--rw-r--r--   0 danielfrees   (501) staff       (20)    18939 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8403 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3624 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    20726 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11962 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8955 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9812 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    34367 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6862 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8063 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6724 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    61930 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7664 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6190 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.751819 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/arch/
--rw-r--r--   0 danielfrees   (501) staff       (20)     5945 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/arch/Geometry_SIMD.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.755190 racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/
--rw-r--r--   0 danielfrees   (501) staff       (20)     4784 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5365 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/Householder.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    23611 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.763900 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 danielfrees   (501) staff       (20)     6771 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6850 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8887 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15036 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14940 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13379 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7349 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4212 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.764783 racplusplus-0.0.1/src/racplusplus/Eigen/src/Jacobi/
--rw-r--r--   0 danielfrees   (501) staff       (20)    16383 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.765762 racplusplus-0.0.1/src/racplusplus/Eigen/src/KLUSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    11555 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.769526 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/
--rw-r--r--   0 danielfrees   (501) staff       (20)     3439 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/Determinant.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    32383 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15727 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    22069 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3555 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.770258 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/arch/
--rw-r--r--   0 danielfrees   (501) staff       (20)    13693 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/arch/InverseSize4.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.771364 racplusplus-0.0.1/src/racplusplus/Eigen/src/MetisSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)     4588 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.774971 racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/
--rw-r--r--   0 danielfrees   (501) staff       (20)    16105 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    61681 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5248 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.775837 racplusplus-0.0.1/src/racplusplus/Eigen/src/PaStiXSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    22249 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.777749 racplusplus-0.0.1/src/racplusplus/Eigen/src/PardisoSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    20092 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.785867 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/
--rw-r--r--   0 danielfrees   (501) staff       (20)    25498 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4662 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    23429 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    26768 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14641 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2993 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.787315 racplusplus-0.0.1/src/racplusplus/Eigen/src/SPQRSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    11826 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.792634 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/
--rw-r--r--   0 danielfrees   (501) staff       (20)    54214 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    32988 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5099 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14743 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15957 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.794384 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCholesky/
--rw-r--r--   0 danielfrees   (501) staff       (20)    24216 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5830 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.824038 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/
--rw-r--r--   0 danielfrees   (501) staff       (20)    10670 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8743 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13166 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2191 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    11368 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    24360 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6485 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13606 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    25524 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4757 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    13256 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5808 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3080 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1107 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12589 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    57475 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    17451 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7329 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7593 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1699 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    15600 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    25889 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4424 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8704 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3175 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6437 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6827 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    14832 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8127 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9657 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.842125 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/
--rw-r--r--   0 danielfrees   (501) staff       (20)    33316 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4303 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7602 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4974 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12837 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2049 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6712 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6584 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3681 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    10217 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4181 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5723 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     8485 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     9028 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4979 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4545 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2889 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.843898 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseQR/
--rw-r--r--   0 danielfrees   (501) staff       (20)    29167 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.847738 racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)     4730 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4155 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     5338 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2809 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.848474 racplusplus-0.0.1/src/racplusplus/Eigen/src/SuperLUSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    34324 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.849996 racplusplus-0.0.1/src/racplusplus/Eigen/src/UmfPackSupport/
--rw-r--r--   0 danielfrees   (501) staff       (20)    24456 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.860722 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/
--rw-r--r--   0 danielfrees   (501) staff       (20)     2913 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/Image.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     2742 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/Kernel.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     1748 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    30560 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/blas.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     7834 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/lapack.h
--rw-r--r--   0 danielfrees   (501) staff       (20)  1058369 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/lapacke.h
--rw-r--r--   0 danielfrees   (501) staff       (20)      474 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.870705 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/
--rw-r--r--   0 danielfrees   (501) staff       (20)    14060 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    21431 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    59020 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     4828 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6089 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)    12283 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6387 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     3350 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 danielfrees   (501) staff       (20)     6915 2023-06-23 23:19:25.000000 racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ReshapedMethods.h
--rw-r--r--   0 danielfrees   (501) staff       (20)      118 2023-06-23 23:21:18.000000 racplusplus-0.0.1/src/racplusplus/__init__.py
--rw-r--r--   0 danielfrees   (501) staff       (20)    48815 2023-06-23 23:37:58.000000 racplusplus-0.0.1/src/racplusplus/_racplusplus.cpp
--rw-r--r--   0 danielfrees   (501) staff       (20)     7105 2023-06-23 23:46:12.000000 racplusplus-0.0.1/src/racplusplus/_racplusplus.h
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.392729 racplusplus-0.0.1/src/racplusplus.egg-info/
--rw-r--r--   0 danielfrees   (501) staff       (20)      923 2023-06-24 00:10:01.000000 racplusplus-0.0.1/src/racplusplus.egg-info/PKG-INFO
--rw-r--r--   0 danielfrees   (501) staff       (20)    17869 2023-06-24 00:10:01.000000 racplusplus-0.0.1/src/racplusplus.egg-info/SOURCES.txt
--rw-r--r--   0 danielfrees   (501) staff       (20)        1 2023-06-24 00:10:01.000000 racplusplus-0.0.1/src/racplusplus.egg-info/dependency_links.txt
--rw-r--r--   0 danielfrees   (501) staff       (20)       12 2023-06-24 00:10:01.000000 racplusplus-0.0.1/src/racplusplus.egg-info/top_level.txt
-drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:10:01.875934 racplusplus-0.0.1/test/
--rw-r--r--   0 danielfrees   (501) staff       (20)     3248 2023-06-23 23:38:14.000000 racplusplus-0.0.1/test/benchmarks.py
--rw-r--r--   0 danielfrees   (501) staff       (20)      419 2023-06-01 21:59:41.000000 racplusplus-0.0.1/test/sklearn_agg_cluster_time_test.py
--rw-r--r--   0 danielfrees   (501) staff       (20)     7956 2023-06-23 23:16:43.000000 racplusplus-0.0.1/test/test_wrapper.ipynb
--rwxr-xr-x   0 danielfrees   (501) staff       (20)     3752 2023-06-23 23:44:52.000000 racplusplus-0.0.1/test/test_wrapper.py
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.523943 racplusplus-0.0.2/
+-rw-r--r--   0 danielfrees   (501) staff       (20)      195 2023-06-23 23:14:41.000000 racplusplus-0.0.2/.gitignore
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3476 2023-06-24 00:51:30.000000 racplusplus-0.0.2/CMakeLists.txt
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1056 2023-06-24 00:05:14.000000 racplusplus-0.0.2/LICENSE
+-rw-r--r--   0 danielfrees   (501) staff       (20)      923 2023-06-24 00:59:04.521453 racplusplus-0.0.2/PKG-INFO
+-rw-r--r--   0 danielfrees   (501) staff       (20)      350 2023-06-24 00:01:35.000000 racplusplus-0.0.2/README.md
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.809231 racplusplus-0.0.2/_skbuild/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.809456 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.809736 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.809979 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.850350 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/
+-rw-r--r--   0 danielfrees   (501) staff       (20)      118 2023-06-23 23:57:46.000000 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/__init__.py
+-rwxr-xr-x   0 danielfrees   (501) staff       (20)   248552 2023-06-23 23:47:06.000000 racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/_racplusplus.cpython-311-darwin.so
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5114 2023-06-24 00:01:20.000000 racplusplus-0.0.2/oldbuild.md
+-rw-r--r--   0 danielfrees   (501) staff       (20)      807 2023-06-24 00:58:26.000000 racplusplus-0.0.2/pyproject.toml
+-rw-r--r--   0 danielfrees   (501) staff       (20)       38 2023-06-24 00:59:04.524560 racplusplus-0.0.2/setup.cfg
+-rw-r--r--   0 danielfrees   (501) staff       (20)      169 2023-06-23 23:58:37.000000 racplusplus-0.0.2/setup.py
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.811334 racplusplus-0.0.2/src/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.852467 racplusplus-0.0.2/src/racplusplus/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.932160 racplusplus-0.0.2/src/racplusplus/Eigen/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1161 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Cholesky
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1900 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/CholmodSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12799 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Core
+-rw-r--r--   0 danielfrees   (501) staff       (20)      122 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Dense
+-rw-r--r--   0 danielfrees   (501) staff       (20)       35 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Eigen
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1777 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Eigenvalues
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1940 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Geometry
+-rw-r--r--   0 danielfrees   (501) staff       (20)      829 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Householder
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2083 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 danielfrees   (501) staff       (20)      894 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Jacobi
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1389 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/KLUSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1268 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/LU
+-rw-r--r--   0 danielfrees   (501) staff       (20)      991 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/MetisSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2451 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/OrderingMethods
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1751 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/PaStiXSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1116 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/PardisoSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1272 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/QR
+-rw-r--r--   0 danielfrees   (501) staff       (20)      900 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/QtAlignedMalloc
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1162 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SPQRSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1584 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SVD
+-rw-r--r--   0 danielfrees   (501) staff       (20)      888 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/Sparse
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1235 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SparseCholesky
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2240 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SparseCore
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1814 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SparseLU
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1195 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SparseQR
+-rw-r--r--   0 danielfrees   (501) staff       (20)      797 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/StdDeque
+-rw-r--r--   0 danielfrees   (501) staff       (20)      726 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/StdList
+-rw-r--r--   0 danielfrees   (501) staff       (20)      803 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/StdVector
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2243 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/SuperLUSupport
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1382 2023-06-23 23:19:24.000000 racplusplus-0.0.2/src/racplusplus/Eigen/UmfPackSupport
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.829912 racplusplus-0.0.2/src/racplusplus/Eigen/src/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.950042 racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24934 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    18760 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3974 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.950611 racplusplus-0.0.2/src/racplusplus/Eigen/src/CholmodSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    25441 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.094793 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    19214 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16782 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Array.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8217 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7018 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2738 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Assign.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    41673 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12488 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14075 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    18648 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Block.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4429 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5981 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6990 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    63841 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4745 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7909 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    36282 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8256 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3937 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5551 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    31529 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24484 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    25360 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9870 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14670 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)      988 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11654 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Dot.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5841 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4909 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5759 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21679 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    38812 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11543 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8238 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/IO.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9620 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3503 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7256 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Map.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11281 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    60784 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7156 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24343 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    23856 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2520 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3620 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12884 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9207 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20748 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    49193 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7336 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Product.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    53832 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7756 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Random.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    19195 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Redux.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17821 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Ref.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5656 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17033 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4284 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7522 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6143 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Select.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14999 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1697 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6837 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Solve.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9368 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6170 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8700 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21641 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4212 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Stride.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2765 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Swap.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17606 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13567 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    38277 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3488 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    35168 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11997 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.819846 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.099744 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15223 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8102 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    64608 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2564 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.113320 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17160 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13344 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    87891 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2134 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.120317 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16540 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2323 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)   119355 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9490 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24820 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)   102394 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.121189 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17317 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.128514 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    26903 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5251 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    67696 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3770 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    35534 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1746 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3746 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.132037 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2695 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    57047 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2256 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.818059 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.133215 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 danielfrees   (501) staff       (20)      691 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.135247 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17541 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16159 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    33615 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.148270 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    22503 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6815 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3083 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)   189525 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    51286 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.154673 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14251 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6765 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    64465 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3650 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.158928 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1194 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21200 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1351 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.165130 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7428 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12539 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    27786 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21856 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2626 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.166923 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16728 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8024 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    36894 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.181385 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6686 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20921 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8334 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4998 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)      607 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    40146 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.211990 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/
+-rw-r--r--   0 danielfrees   (501) staff       (20)   108448 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20104 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15948 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6936 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5106 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21724 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6368 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5582 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21354 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11570 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9958 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5209 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6164 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4126 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20987 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13867 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14722 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    10571 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14678 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6707 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5882 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.233661 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    23156 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    19876 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21931 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Constants.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4892 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15555 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6696 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    10949 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/IntegralConstant.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4268 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    52909 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    46661 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    29336 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)       85 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1024 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1432 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    10676 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12003 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    35762 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.299482 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12559 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17274 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4178 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    22970 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17176 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9716 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14349 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5575 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    23640 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21078 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3650 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    35182 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4104 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    22764 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.332549 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    18939 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8403 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3624 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20726 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11962 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8955 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9812 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    34367 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6862 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8063 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6724 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    61930 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7664 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6190 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.346200 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/arch/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5945 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.352756 racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4784 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5365 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    23611 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.362777 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6771 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6850 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8887 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15036 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14940 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13379 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7349 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4212 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.363338 racplusplus-0.0.2/src/racplusplus/Eigen/src/Jacobi/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16383 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.363912 racplusplus-0.0.2/src/racplusplus/Eigen/src/KLUSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11555 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.375816 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3439 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    32383 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15727 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    22069 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3555 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.376935 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/arch/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13693 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.378606 racplusplus-0.0.2/src/racplusplus/Eigen/src/MetisSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4588 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.383880 racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    16105 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    61681 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5248 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.384623 racplusplus-0.0.2/src/racplusplus/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    22249 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.385276 racplusplus-0.0.2/src/racplusplus/Eigen/src/PardisoSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    20092 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.399127 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    25498 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4662 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    23429 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    26768 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14641 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2993 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.399493 racplusplus-0.0.2/src/racplusplus/Eigen/src/SPQRSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11826 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.401877 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    54214 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    32988 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5099 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14743 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15957 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.407852 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCholesky/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24216 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5830 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.452545 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    10670 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8743 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13166 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2191 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    11368 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24360 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6485 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13606 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    25524 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4757 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    13256 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5808 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3080 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1107 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12589 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    57475 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17451 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7329 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7593 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1699 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    15600 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    25889 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4424 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8704 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3175 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6437 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6827 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14832 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8127 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9657 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.481731 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    33316 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4303 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7602 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4974 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12837 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2049 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6712 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6584 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3681 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    10217 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4181 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5723 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     8485 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     9028 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4979 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4545 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2889 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.482990 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseQR/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    29167 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.488017 racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4730 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4155 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     5338 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2809 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.488840 racplusplus-0.0.2/src/racplusplus/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    34324 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.489673 racplusplus-0.0.2/src/racplusplus/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    24456 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.501040 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2913 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/Image.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     2742 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     1748 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    30560 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/blas.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7834 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/lapack.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)  1058369 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)      474 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.517815 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/
+-rw-r--r--   0 danielfrees   (501) staff       (20)    14060 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    21431 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    59020 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     4828 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6089 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)    12283 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6387 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3350 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)     6915 2023-06-23 23:19:25.000000 racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ReshapedMethods.h
+-rw-r--r--   0 danielfrees   (501) staff       (20)      118 2023-06-23 23:21:18.000000 racplusplus-0.0.2/src/racplusplus/__init__.py
+-rw-r--r--   0 danielfrees   (501) staff       (20)    48815 2023-06-23 23:37:58.000000 racplusplus-0.0.2/src/racplusplus/_racplusplus.cpp
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7105 2023-06-23 23:46:12.000000 racplusplus-0.0.2/src/racplusplus/_racplusplus.h
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:03.855776 racplusplus-0.0.2/src/racplusplus.egg-info/
+-rw-r--r--   0 danielfrees   (501) staff       (20)      923 2023-06-24 00:59:03.000000 racplusplus-0.0.2/src/racplusplus.egg-info/PKG-INFO
+-rw-r--r--   0 danielfrees   (501) staff       (20)    17869 2023-06-24 00:59:03.000000 racplusplus-0.0.2/src/racplusplus.egg-info/SOURCES.txt
+-rw-r--r--   0 danielfrees   (501) staff       (20)        1 2023-06-24 00:59:03.000000 racplusplus-0.0.2/src/racplusplus.egg-info/dependency_links.txt
+-rw-r--r--   0 danielfrees   (501) staff       (20)       12 2023-06-24 00:59:03.000000 racplusplus-0.0.2/src/racplusplus.egg-info/top_level.txt
+drwxr-xr-x   0 danielfrees   (501) staff       (20)        0 2023-06-24 00:59:04.520478 racplusplus-0.0.2/test/
+-rw-r--r--   0 danielfrees   (501) staff       (20)     3248 2023-06-23 23:38:14.000000 racplusplus-0.0.2/test/benchmarks.py
+-rw-r--r--   0 danielfrees   (501) staff       (20)      419 2023-06-01 21:59:41.000000 racplusplus-0.0.2/test/sklearn_agg_cluster_time_test.py
+-rw-r--r--   0 danielfrees   (501) staff       (20)     7956 2023-06-23 23:16:43.000000 racplusplus-0.0.2/test/test_wrapper.ipynb
+-rwxr-xr-x   0 danielfrees   (501) staff       (20)     3752 2023-06-23 23:44:52.000000 racplusplus-0.0.2/test/test_wrapper.py
```

### Comparing `racplusplus-0.0.1/CMakeLists.txt` & `racplusplus-0.0.2/CMakeLists.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 cmake_minimum_required(VERSION 3.16)
 set(CMAKE_CXX_STANDARD 17)
 project(racplusplus VERSION "0.0.1")
 
-message(STATUS "\n-- Setting LLVM and Python3 Directories...\n")
+message(STATUS "\n-- Finding Prefix Paths...\n")
 list(APPEND CMAKE_PREFIX_PATH "/usr/local/opt")
+if(DEFINED ENV{YOUR_VARIABLE_NAME})
+    set(CONDA_PREFIX $ENV{CONDA_PREFIX})
+    message(STATUS "Loaded environment variable: CONDA_PREFIX=${CONDA_PREFIX_VALUE}")
+else()
+    message(STATUS "Environment variable CONDA_PREFIX is not set.")
+endif()
+list(APPEND CMAKE_PREFIX_PATH CONDA_PREFIX)
+
 
+message(STATUS "\n-- Setting LLVM and Python3 Directories...\n")
 # Set LLVM directories
 find_package(LLVM REQUIRED CONFIG)
 message(STATUS "-- -- Found LLVM ${LLVM_PACKAGE_VERSION}")
 list(APPEND CMAKE_MODULE_PATH "${LLVM_CMAKE_DIR}")
 include_directories(${LLVM_INCLUDE_DIRS})
 link_directories(${LLVM_LIBRARY_DIRS})
```

### Comparing `racplusplus-0.0.1/LICENSE` & `racplusplus-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/PKG-INFO` & `racplusplus-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: racplusplus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reciprocal Agglomerative Clustering, optimized for speed/ parallelization in C++.
 Author-email: Porter Hunley <porterhunley@themedicalboard.net>, Daniel Frees <danielfrees@g.ucla.edu>
 Project-URL: Homepage, https://github.com/mediboard/racplusplus
 Project-URL: Bug Tracker, https://github.com/mediboard/racplusplus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
```

### Comparing `racplusplus-0.0.1/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/_racplusplus.cpython-311-darwin.so` & `racplusplus-0.0.2/_skbuild/macosx-10.16-x86_64-3.11/cmake-install/src/racplusplus/_racplusplus.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/oldbuild.md` & `racplusplus-0.0.2/oldbuild.md`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/pyproject.toml` & `racplusplus-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "racplusplus"
-version = "0.0.1"
+version = "0.0.2"
 description = "Reciprocal Agglomerative Clustering, optimized for speed/ parallelization in C++."
 authors = [
     {name = "Porter Hunley", email = "porterhunley@themedicalboard.net"},
     {name = "Daniel Frees", email = "danielfrees@g.ucla.edu"}
 ]
 readme = "README.md"
 classifiers = [
```

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Cholesky` & `racplusplus-0.0.2/src/racplusplus/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/CholmodSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Core` & `racplusplus-0.0.2/src/racplusplus/Eigen/Core`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Eigenvalues` & `racplusplus-0.0.2/src/racplusplus/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Geometry` & `racplusplus-0.0.2/src/racplusplus/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Householder` & `racplusplus-0.0.2/src/racplusplus/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/IterativeLinearSolvers` & `racplusplus-0.0.2/src/racplusplus/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Jacobi` & `racplusplus-0.0.2/src/racplusplus/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/KLUSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/LU` & `racplusplus-0.0.2/src/racplusplus/Eigen/LU`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/MetisSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/OrderingMethods` & `racplusplus-0.0.2/src/racplusplus/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/PaStiXSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/PardisoSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/QR` & `racplusplus-0.0.2/src/racplusplus/Eigen/QR`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/QtAlignedMalloc` & `racplusplus-0.0.2/src/racplusplus/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SPQRSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SVD` & `racplusplus-0.0.2/src/racplusplus/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/Sparse` & `racplusplus-0.0.2/src/racplusplus/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SparseCholesky` & `racplusplus-0.0.2/src/racplusplus/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SparseCore` & `racplusplus-0.0.2/src/racplusplus/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SparseLU` & `racplusplus-0.0.2/src/racplusplus/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SparseQR` & `racplusplus-0.0.2/src/racplusplus/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/StdDeque` & `racplusplus-0.0.2/src/racplusplus/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/StdList` & `racplusplus-0.0.2/src/racplusplus/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/StdVector` & `racplusplus-0.0.2/src/racplusplus/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/SuperLUSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/UmfPackSupport` & `racplusplus-0.0.2/src/racplusplus/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LDLT.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LLT.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Cholesky/LLT_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/CholmodSupport/CholmodSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArithmeticSequence.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Array.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArrayBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ArrayWrapper.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Assign.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/AssignEvaluator.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Assign_MKL.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/BandMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Block.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/BooleanRedux.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CommaInitializer.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ConditionEstimator.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CoreEvaluators.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CoreIterators.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseBinaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseNullaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseTernaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseUnaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/CwiseUnaryView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseCoeffsBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DenseStorage.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Diagonal.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DiagonalMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/DiagonalProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Dot.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/EigenBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ForceAlignedAccess.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Fuzzy.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GeneralProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GenericPacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/GlobalFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/IO.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/IndexedView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Inverse.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Map.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MapBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MathFunctionsImpl.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Matrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/MatrixBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NestByValue.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NoAlias.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/NumTraits.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PartialReduxEvaluator.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PermutationMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/PlainObjectBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Product.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ProductEvaluators.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Random.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Redux.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Ref.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Replicate.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Reshaped.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/ReturnByValue.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Reverse.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Select.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SelfAdjointView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SelfCwiseBinaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Solve.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SolveTriangular.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/SolverBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/StableNorm.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/StlIterators.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Stride.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Swap.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Transpose.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Transpositions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/TriangularMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/VectorBlock.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/VectorwiseOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/Visitor.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/CUDA/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/BFloat16.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/ConjHelper.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/Half.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/Settings.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/Default/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/GPU/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/MSA/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/NEON/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SSE/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SVE/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/Complex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/arch/ZVector/PacketMath.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/AssignmentFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/BinaryFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/NullaryFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/StlFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/TernaryFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/functors/UnaryFunctors.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/Parallelizer.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/SelfadjointRank2Update.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/products/TriangularSolverVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/BlasUtil.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ConfigureVectorization.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Constants.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/DisableStupidWarnings.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ForwardDeclarations.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/IndexedViewHelper.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/IntegralConstant.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/MKL_support.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Macros.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Memory.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/Meta.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ReenableStupidWarnings.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/ReshapedHelper.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/StaticAssert.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/SymbolicIndex.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Core/util/XprHelper.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/EigenSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealQZ.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealSchur.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Eigenvalues/Tridiagonalization.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/AlignedBox.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/AngleAxis.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/EulerAngles.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Homogeneous.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Hyperplane.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/OrthoMethods.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/ParametrizedLine.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Quaternion.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Rotation2D.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/RotationBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Scaling.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Transform.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Translation.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/Umeyama.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/BlockHouseholder.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/Householder.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Householder/HouseholderSequence.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/Jacobi/Jacobi.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/KLUSupport/KLUSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/Determinant.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/FullPivLU.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/InverseImpl.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/PartialPivLU.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/LU/arch/InverseSize4.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/MetisSupport/MetisSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Amd.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/OrderingMethods/Ordering.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/PardisoSupport/PardisoSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/FullPivHouseholderQR.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/HouseholderQR.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/BDCSVD.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/JacobiSVD.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/SVDBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SVD/UpperBidiagonalization.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/AmbiVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/CompressedStorage.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/MappedSparseMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseAssign.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseBlock.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseColEtree.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCompressedBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDenseProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseDot.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseFuzzy.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMap.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseMatrixBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparsePermutation.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseProduct.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseRedux.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseRef.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSolverBase.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseTranspose.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseTriangularView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseUtil.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/SparseView.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseCore/TriangularSolver.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLUImpl.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Memory.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Structs.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_Utils.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_pivotL.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_pruneL.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SparseQR/SparseQR.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdDeque.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdList.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/StdVector.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/StlSupport/details.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/Image.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/Kernel.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/RealSvd2x2.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/blas.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/lapack.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/misc/lapacke.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/BlockMethods.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/IndexedViewMethods.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/Eigen/src/plugins/ReshapedMethods.h` & `racplusplus-0.0.2/src/racplusplus/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/_racplusplus.cpp` & `racplusplus-0.0.2/src/racplusplus/_racplusplus.cpp`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus/_racplusplus.h` & `racplusplus-0.0.2/src/racplusplus/_racplusplus.h`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/src/racplusplus.egg-info/PKG-INFO` & `racplusplus-0.0.2/src/racplusplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: racplusplus
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reciprocal Agglomerative Clustering, optimized for speed/ parallelization in C++.
 Author-email: Porter Hunley <porterhunley@themedicalboard.net>, Daniel Frees <danielfrees@g.ucla.edu>
 Project-URL: Homepage, https://github.com/mediboard/racplusplus
 Project-URL: Bug Tracker, https://github.com/mediboard/racplusplus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
```

### Comparing `racplusplus-0.0.1/src/racplusplus.egg-info/SOURCES.txt` & `racplusplus-0.0.2/src/racplusplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/test/benchmarks.py` & `racplusplus-0.0.2/test/benchmarks.py`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/test/test_wrapper.ipynb` & `racplusplus-0.0.2/test/test_wrapper.ipynb`

 * *Files identical despite different names*

### Comparing `racplusplus-0.0.1/test/test_wrapper.py` & `racplusplus-0.0.2/test/test_wrapper.py`

 * *Files identical despite different names*

