# Comparing `tmp/MParT-1.4.4.tar.gz` & `tmp/MParT-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MParT-1.4.4.tar", last modified: Fri Feb 10 21:40:00 2023, max compression
+gzip compressed data, was "MParT-2.0.1.tar", last modified: Fri Apr  7 17:58:29 2023, max compression
```

## Comparing `MParT-1.4.4.tar` & `MParT-2.0.1.tar`

### file list

```diff
@@ -1,315 +1,355 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.563185 MParT-1.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.531185 MParT-1.4.4/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-02-10 21:39:50.000000 MParT-1.4.4/.docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-10 21:39:50.000000 MParT-1.4.4/.docker/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-10 21:39:50.000000 MParT-1.4.4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.531185 MParT-1.4.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/install-doxygen.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.531185 MParT-1.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/build-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/build-doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/build-external-lib-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/build-push-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/build-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-10 21:39:50.000000 MParT-1.4.4/.github/workflows/pypi-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-10 21:39:50.000000 MParT-1.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-10 21:39:50.000000 MParT-1.4.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-02-10 21:39:50.000000 MParT-1.4.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-10 21:39:50.000000 MParT-1.4.4/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-10 21:39:50.000000 MParT-1.4.4/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.535185 MParT-1.4.4/MParT/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/AffineFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/AffineMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/ComposedMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/ConditionalMapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/DerivativeFlags.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.535185 MParT-1.4.4/MParT/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Distributions/DensityBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Distributions/Distribution.h
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Distributions/GaussianSamplerDensity.h
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Distributions/SampleGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/HermiteFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/IdentityMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Initialization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/LinearizedBasis.h
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MapFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MapOptions.h
--rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MonotoneComponent.h
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MonotoneIntegrand.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.535185 MParT-1.4.4/MParT/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultiIndices/FixedMultiIndexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultiIndices/MultiIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultiIndices/MultiIndexLimiter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultiIndices/MultiIndexNeighborhood.h
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultiIndices/MultiIndexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultivariateExpansion.h
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/MultivariateExpansionWorker.h
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/OrthogonalPolynomial.h
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/ParameterizedFunctionBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/PositiveBijectors.h
--rw-r--r--   0 runner    (1001) docker     (123)    43493 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Quadrature.h
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/SummarizedMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/TensorProductFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/TriangularMap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.535185 MParT-1.4.4/MParT/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    32671 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/ArrayConversions.h
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/EigenTypes.h
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/GPUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/KokkosHelpers.h
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/KokkosSpaceMappings.h
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/LinearAlgebra.h
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/Miscellaneous.h
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-02-10 21:39:50.000000 MParT-1.4.4/MParT/Utilities/Serialization.h
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-10 21:40:00.563185 MParT-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-10 21:39:50.000000 MParT-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.527185 MParT-1.4.4/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.527185 MParT-1.4.4/bindings/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.535185 MParT-1.4.4/bindings/common/include/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/common/include/CommonUtilities.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/common/src/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/common/src/CommonUtilities.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/julia/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/julia/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/include/CommonJuliaUtilities.h
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/include/JlArrayConversions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/julia/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/CommonJuliaUtilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/JlArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/MapOptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/TriangularMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/julia/src/Wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/matlab/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/matlab/external/mexplus/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14160 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/arguments.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/dispatch.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/mxarray.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11613 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/mxtypes.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus/mexplus.h
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/external/mexplus_eigen.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.539185 MParT-1.4.4/bindings/matlab/include/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/include/MexArrayConversions.h
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/include/MexMapOptionsConversions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/matlab/mat/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/AffineMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/ComposedMap.m
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/ConditionalMap.m
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/CreateComponent.m
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/CreateTriangular.m
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/FixedMultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/KokkosInitialize.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/matlab/mat/MapOptions/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MapOptions/BasisTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MapOptions/MapOptions.m
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MapOptions/PosFuncTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MapOptions/QuadTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MultiIndex.m
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/MultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/ParameterizedFunction.m
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/mat/TriangularMap.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/matlab/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/BasisTypes_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15067 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/ConditionalMap_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/FixedMultiIndexSet_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/KokkosUtilities_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/MexArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/MexMapOptionsConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/MultiIndexSet_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/MultiIndex_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/matlab/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/FixedMultiIndexSetTest.m
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_AffineMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_ComposedMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_MultiIndex.m
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_MultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_ParameterizedFunction.m
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/Test_TriangularMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/matlab/tests/runtests.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/python/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/python/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/include/CommonPybindUtilities.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/python/package/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.543185 MParT-1.4.4/bindings/python/package/MParT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-10 21:40:00.000000 MParT-1.4.4/bindings/python/package/MParT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-02-10 21:40:00.000000 MParT-1.4.4/bindings/python/package/MParT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 21:40:00.000000 MParT-1.4.4/bindings/python/package/MParT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 21:40:00.000000 MParT-1.4.4/bindings/python/package/MParT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.547185 MParT-1.4.4/bindings/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/CommonPybindUtilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/MapOptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/Serialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/TriangularMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/src/Wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.547185 MParT-1.4.4/bindings/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_AffineFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_AffineMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_ComposedMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_ComposedMap_moveCoeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_ConditionalMapBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_IdentityMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_MapFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_MultiIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_MultiIndexSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_SummarizedMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_TriangularMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-10 21:39:50.000000 MParT-1.4.4/bindings/python/tests/test_TriangularMap_moveCoeffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.547185 MParT-1.4.4/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-02-10 21:39:50.000000 MParT-1.4.4/cmake/BuildDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-02-10 21:39:50.000000 MParT-1.4.4/cmake/FindJulia.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-10 21:39:50.000000 MParT-1.4.4/cmake/FindSphinx.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-02-10 21:39:50.000000 MParT-1.4.4/cmake/SetInstallPaths.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.547185 MParT-1.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.527185 MParT-1.4.4/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.551185 MParT-1.4.4/docs/_static/pics/
--rw-r--r--   0 runner    (1001) docker     (123)    44355 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/_static/pics/Density.png
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/_static/pics/Regression.png
--rw-r--r--   0 runner    (1001) docker     (123)   426141 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/_static/pics/Samples.png
--rw-r--r--   0 runner    (1001) docker     (123)   123355 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/_static/pics/Transformation2d.png
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)   114543 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/mpart.doxyfile.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.551185 MParT-1.4.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.551185 MParT-1.4.4/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/composedmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.551185 MParT-1.4.4/docs/source/api/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/concepts/cachedparameterization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/concepts/parameterizedfunction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/conditionalmapbase.rst
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/mapfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/monotonecomponent.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.551185 MParT-1.4.4/docs/source/api/multiindices/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindices/fixedmultiindexset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindices/multiindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindices/multiindexlimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindices/multiindexneighborhood.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multiindices/multiindexset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multivariateexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/multivariateexpansionworker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/parameterizedfunctionbase.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.555185 MParT-1.4.4/docs/source/api/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/quadrature/adaptivesimpson.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/quadrature/clenshawcurtis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/quadrature/recursivequadrature.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/quadrature.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/templateconcepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/tensorproductfunction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/triangularmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.555185 MParT-1.4.4/docs/source/api/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/utilities/initialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/utilities/kokkoswrappers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/utilities/linearalgebra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/api/utilities/serialization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.555185 MParT-1.4.4/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/mathematics.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.555185 MParT-1.4.4/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-10 21:39:50.000000 MParT-1.4.4/docs/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.555185 MParT-1.4.4/joss/
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-02-10 21:39:50.000000 MParT-1.4.4/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-02-10 21:39:50.000000 MParT-1.4.4/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)   922955 2023-02-10 21:39:50.000000 MParT-1.4.4/joss/performance_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-10 21:39:50.000000 MParT-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 21:40:00.563185 MParT-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-10 21:39:50.000000 MParT-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.559185 MParT-1.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-02-10 21:39:50.000000 MParT-1.4.4/src/AffineFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-02-10 21:39:50.000000 MParT-1.4.4/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-10 21:39:50.000000 MParT-1.4.4/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19014 2023-02-10 21:39:50.000000 MParT-1.4.4/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-02-10 21:39:50.000000 MParT-1.4.4/src/ConditionalMapBase.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.559185 MParT-1.4.4/src/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-10 21:39:50.000000 MParT-1.4.4/src/Distributions/DensityBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-02-10 21:39:50.000000 MParT-1.4.4/src/Distributions/GaussianSamplerDensity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-02-10 21:39:50.000000 MParT-1.4.4/src/IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-10 21:39:50.000000 MParT-1.4.4/src/Initialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl10.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl12.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl13.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl14.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl15.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl6.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl7.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl8.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MapFactoryImpl9.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.559185 MParT-1.4.4/src/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MultiIndices/FixedMultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MultiIndices/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MultiIndices/MultiIndexLimiter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MultiIndices/MultiIndexNeighborhood.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19730 2023-02-10 21:39:50.000000 MParT-1.4.4/src/MultiIndices/MultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-02-10 21:39:50.000000 MParT-1.4.4/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-02-10 21:39:50.000000 MParT-1.4.4/src/SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-02-10 21:39:50.000000 MParT-1.4.4/src/TriangularMap.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.559185 MParT-1.4.4/src/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-02-10 21:39:50.000000 MParT-1.4.4/src/Utilities/LinearAlgebra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-10 21:39:50.000000 MParT-1.4.4/src/Utilities/Miscellaneous.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.563185 MParT-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.563185 MParT-1.4.4/tests/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Distributions/Test_DensityBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Distributions/Test_Distribution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Distributions/Test_Distributions_Common.h
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Distributions/Test_GaussianDistribution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Distributions/Test_SampleGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/KokkosInfo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 21:40:00.563185 MParT-1.4.4/tests/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/MultiIndices/Test_MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/MultiIndices/Test_MultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/RunTests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_AffineFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_ArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32651 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_HermiteFunctions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_LinearAlgebra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_LinearizedBasis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_MonotoneComponent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_MultivariateExpansion.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_MultivariateExpansionWorker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_OrthogonalPolynomials.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_PositiveBijectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_Quadrature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_Serialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_TensorProductFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    39093 2023-02-10 21:39:50.000000 MParT-1.4.4/tests/Test_TriangularMap.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-07 17:58:17.000000 MParT-2.0.1/.docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-07 17:58:17.000000 MParT-2.0.1/.docker/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 17:58:17.000000 MParT-2.0.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/install-doxygen.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-external-lib-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-push-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 17:58:17.000000 MParT-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 17:58:17.000000 MParT-2.0.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-04-07 17:58:17.000000 MParT-2.0.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-07 17:58:17.000000 MParT-2.0.1/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 17:58:17.000000 MParT-2.0.1/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.580093 MParT-2.0.1/MParT/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/AffineFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/AffineMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ComposedMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ConditionalMapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/DerivativeFlags.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.584093 MParT-2.0.1/MParT/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/DensityBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/Distribution.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/GaussianSamplerDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PullbackDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PullbackSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PushforwardDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PushforwardSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/SampleGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/TransportDistributionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/HermiteFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/IdentityMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Initialization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/LinearizedBasis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapObjective.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapOptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MonotoneComponent.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MonotoneIntegrand.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.584093 MParT-2.0.1/MParT/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/FixedMultiIndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexLimiter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexNeighborhood.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultivariateExpansion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultivariateExpansionWorker.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/OrthogonalPolynomial.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ParameterizedFunctionBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/PositiveBijectors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43493 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Quadrature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/SummarizedMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TensorProductFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TrainMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TrainMapAdaptive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TriangularMap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/MParT/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/ArrayConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/EigenTypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/GPUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/KokkosHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/KokkosSpaceMappings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/LinearAlgebra.h
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/Miscellaneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/Serialization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 17:58:29.652094 MParT-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-07 17:58:17.000000 MParT-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.564093 MParT-2.0.1/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.564093 MParT-2.0.1/bindings/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/common/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/common/include/CommonUtilities.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/common/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/common/src/CommonUtilities.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.592093 MParT-2.0.1/bindings/julia/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/include/CommonJuliaUtilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/include/JlArrayConversions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.592093 MParT-2.0.1/bindings/julia/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/CommonJuliaUtilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/JlArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapOptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TriangularMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/Wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/mexplus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14160 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/arguments.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/dispatch.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxarray.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11613 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxtypes.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus_eigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexArrayConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexOptionsConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexWrapperTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.600093 MParT-2.0.1/bindings/matlab/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ATMOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/AdaptiveTransportMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/AffineMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ComposedMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ConditionalMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/CreateComponent.m
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/CreateTriangular.m
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/DeserializeMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/FixedMultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/GaussianKLObjective.m
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/KokkosInitialize.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.604093 MParT-2.0.1/bindings/matlab/mat/MapOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/BasisTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/MapOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/PosFuncTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/QuadTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MultiIndex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ParameterizedFunction.m
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TrainMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TrainOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TriangularMap.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.604093 MParT-2.0.1/bindings/matlab/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/BasisTypes_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/ConditionalMap_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/FixedMultiIndexSet_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/KokkosUtilities_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MapObjective_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MexArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MexOptionsConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MultiIndexSet_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MultiIndex_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/matlab/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/FixedMultiIndexSetTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_AffineMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_ComposedMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_MultiIndex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_MultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_ParameterizedFunction.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_TriangularMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/TrainMapAdaptiveTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/TrainMapTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/runtests.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/include/CommonPybindUtilities.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/package/MParT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.612093 MParT-2.0.1/bindings/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/CommonPybindUtilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapOptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/Serialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TriangularMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/Wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.616093 MParT-2.0.1/bindings/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_AffineFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_AffineMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ComposedMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ComposedMap_moveCoeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ConditionalMapBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_IdentityMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MapFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MultiIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MultiIndexSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_SummarizedMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TrainMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TrainMapAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TriangularMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TriangularMap_moveCoeffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.616093 MParT-2.0.1/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/BuildDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/FindJulia.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/FindSphinx.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/SetInstallPaths.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.568093 MParT-2.0.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/_static/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)    44355 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Density.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Regression.png
+-rw-r--r--   0 runner    (1001) docker     (123)   426141 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123355 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Transformation2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)   114543 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/mpart.doxyfile.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.624093 MParT-2.0.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/composedmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.624093 MParT-2.0.1/docs/source/api/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/concepts/cachedparameterization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/concepts/parameterizedfunction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/conditionalmapbase.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/mapfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/monotonecomponent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/multiindices/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/fixedmultiindexset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexlimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexneighborhood.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multivariateexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multivariateexpansionworker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/parameterizedfunctionbase.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/adaptivesimpson.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/clenshawcurtis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/recursivequadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/templateconcepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/tensorproductfunction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/triangularmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/initialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/kokkoswrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/linearalgebra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/serialization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/mathematics.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/joss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)   922955 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/performance_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-07 17:58:17.000000 MParT-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 17:58:29.652094 MParT-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-07 17:58:17.000000 MParT-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-07 17:58:17.000000 MParT-2.0.1/src/AffineFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-07 17:58:17.000000 MParT-2.0.1/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-07 17:58:17.000000 MParT-2.0.1/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ConditionalMapBase.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/DensityBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/GaussianSamplerDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/PullbackDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-07 17:58:17.000000 MParT-2.0.1/src/IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Initialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl10.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl12.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl13.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl14.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl15.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl16.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl17.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl18.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl6.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl7.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl8.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl9.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapObjective.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/FixedMultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexLimiter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexNeighborhood.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-07 17:58:17.000000 MParT-2.0.1/src/SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TriangularMap.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.644093 MParT-2.0.1/src/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Utilities/LinearAlgebra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Utilities/Miscellaneous.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.648093 MParT-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/tests/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_DensityBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distribution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distributions_Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distributions_Common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_GaussianDistribution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_SampleGenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportDistributionFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportSampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/KokkosInfo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/tests/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/MultiIndices/Test_MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/MultiIndices/Test_MultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/RunTests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_AffineFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32651 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_HermiteFunctions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_LinearAlgebra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_LinearizedBasis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MonotoneComponent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MultivariateExpansion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MultivariateExpansionWorker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_OrthogonalPolynomials.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_PositiveBijectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_Quadrature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_Serialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TensorProductFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39093 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TriangularMap.cpp
```

### Comparing `MParT-1.4.4/.docker/Dockerfile` & `MParT-2.0.1/.docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/.github/workflows/build-bindings.yml` & `MParT-2.0.1/.github/workflows/build-bindings.yml`

 * *Files 12% similar despite different names*

```diff
@@ -2,41 +2,52 @@
 
 on:
   push:
     branches:
       - main
   pull_request: {}
 
+env:
+  CONDA_CACHE_NUMBER: 0  # increase to reset cache manually
+
 jobs:
   build-tests:
     runs-on: ubuntu-latest
     steps:
 
       - name: Store Date
         shell: bash -l {0}
         run: echo "DATE=$(date +'%Y%m%d')" >> $GITHUB_ENV
 
       - name: Checkout MParT
         uses: actions/checkout@v3
         with:
           path: mpart
 
-      - name: Cache Conda Deps
-        uses: actions/cache@v3
-        id: cache-conda
-        with:
-          path: "~/conda_pkgs_dir"
-          key: conda-${{ hashFiles('mpart/.github/environment.yml') }}-${{ env.DATE }}
-
       - name: Use Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
+          miniforge-variant: Mambaforge
+          miniforge-version: latest
+          activate-environment: test
+          use-mamba: true
           auto-update-conda: true
           python-version: "3.8"
-          activate-environment: "test"
+
+      - name: Cache Conda Deps
+        uses: actions/cache@v3
+        id: cache-conda
+        with:
+          path: /usr/share/miniconda3/envs/test
+          key: cache-conda-${{ hashFiles('mpart/.github/environment.yml') }}-${{ env.DATE }}-${{ env.CONDA_CACHE_NUMBER }}-BINDINGS
+
+      - name: Install Conda Dependencies
+        shell: bash -l {0}
+        run: mamba env update -n test -f $GITHUB_WORKSPACE/mpart/.github/environment.yml
+        if: steps.cache-conda.outputs.cache-hit != 'true'
 
       - name: Setup Julia
         run: |
           julia -e "using Pkg; Pkg.add([\"CxxWrap\",\"TestReports\"])"
           export GITHUB_JULIA_PATH=$(julia -e "println(DEPOT_PATH[1])")
           echo -n $'[bee5971c-294f-5168-9fcd-9fb3c811d495]\nMParT = \"' >> $GITHUB_JULIA_PATH/artifacts/Overrides.toml
           echo -n $GITHUB_WORKSPACE                                     >> $GITHUB_JULIA_PATH/artifacts/Overrides.toml
@@ -69,18 +80,14 @@
                 -DBUILD_SHARED_LIBS=ON     \
                 -DKokkos_ENABLE_SERIAL=ON  \
                 -DCMAKE_CXX_STANDARD=17    \
                 -DCMAKE_INSTALL_PREFIX=$GITHUB_WORKSPACE/KOKKOS_INSTALL/ \
                 ../
           sudo make -j2 install
 
-      - name: Install Conda Dependencies
-        shell: bash -l {0}
-        run: conda env update -n test -f $GITHUB_WORKSPACE/mpart/.github/environment.yml
-
       - name: Configure MParT
         shell: bash -l {0}
         run: |
           cd $GITHUB_WORKSPACE/mpart
           mkdir build && cd build
           cmake -DKokkos_DIR=$GITHUB_WORKSPACE/KOKKOS_INSTALL/lib/cmake/Kokkos \
                 -DMPART_FETCH_DEPS=OFF \
```

### Comparing `MParT-1.4.4/.github/workflows/build-doc.yml` & `MParT-2.0.1/.github/workflows/build-doc.yml`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/.github/workflows/build-external-lib-tests.yml` & `MParT-2.0.1/.github/workflows/build-external-lib-tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,46 @@
 
 on:
   push:
     branches:
       - main
   pull_request: {}
 
+env:
+  CONDA_CACHE_NUMBER: 0  # increase to reset cache manually
+
 jobs:
   build-tests:
     runs-on: ubuntu-latest
     steps:
       - name: Store Date
         shell: bash -l {0}
         run: echo "DATE=$(date +'%Y%m%d')" >> $GITHUB_ENV
 
       - name: Checkout MParT
         uses: actions/checkout@v3
         with:
           path: mpart
 
-      - name: Cache Conda Deps
-        uses: actions/cache@v3
-        id: cache-conda
-        with:
-          path: "~/conda_pkgs_dir"
-          key: conda-${{ hashFiles('mpart/.github/environment.yml') }}-${{ env.DATE }}
-
       - name: Use Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
+          miniforge-variant: Mambaforge
+          miniforge-version: latest
+          activate-environment: test
+          use-mamba: true
           auto-update-conda: true
           python-version: "3.8"
-          activate-environment: "test"
+
+      - name: Cache Conda Deps
+        uses: actions/cache@v3
+        id: cache-conda
+        with:
+          path: /usr/share/miniconda3/envs/test
+          key: conda-cache-${{ hashFiles('mpart/.github/environment.yml') }}-${{ env.DATE }}-${{ env.CONDA_CACHE_NUMBER }}
 
       - name: Cache Kokkos
         uses: actions/cache@v3
         id: cache-kokkos
         with:
           path: "${{ github.workspace }}/KOKKOS_INSTALL"
           key: kokkos3.7.00
@@ -60,14 +66,15 @@
                 -DCMAKE_INSTALL_PREFIX=$GITHUB_WORKSPACE/KOKKOS_INSTALL/ \
                 ../
           sudo make -j2 install
 
       - name: Install Conda Dependencies
         shell: bash -l {0}
         run: conda env update -n test -f $GITHUB_WORKSPACE/mpart/.github/environment.yml
+        if: steps.cache-conda.outputs.cache-hit != 'true'
 
       - name: Configure MParT
         shell: bash -l {0}
         run: |
           cd $GITHUB_WORKSPACE/mpart
           mkdir build && cd build
           cmake -DKokkos_DIR=$GITHUB_WORKSPACE/KOKKOS_INSTALL/lib/cmake/Kokkos -DMPART_FETCH_DEPS=OFF ../
```

### Comparing `MParT-1.4.4/.github/workflows/build-push-docker.yml` & `MParT-2.0.1/.github/workflows/build-push-docker.yml`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/.github/workflows/build-tests.yml` & `MParT-2.0.1/.github/workflows/build-tests.yml`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/.github/workflows/pypi-deploy.yml` & `MParT-2.0.1/.github/workflows/pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/CITATION.cff` & `MParT-2.0.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/CMakeLists.txt` & `MParT-2.0.1/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.13)
-project(MParT VERSION 0.0.1)
+project(MParT VERSION 2.0.1)
 
 message(STATUS "Will install MParT to ${CMAKE_INSTALL_PREFIX}")
 
 # Add the cmake folder as a search path and include files
 LIST(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake/)
 Include(FetchContent)
 
@@ -216,15 +216,14 @@
 else()
     set(EXT_LIBRARIES "")
 endif()
 
 # Add NLopt if necessary
 if(MPART_OPT)
     find_package(NLopt QUIET)
-
     if(NOT NLopt_FOUND)
         if(${MPART_FETCH_DEPS})
             message(STATUS "Could not find NLopt. Fetching source.")
 
             FetchContent_Declare(
                 NLopt
                 GIT_REPOSITORY https://github.com/stevengj/nlopt/
```

### Comparing `MParT-1.4.4/LICENSE.txt` & `MParT-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/AffineFunction.h` & `MParT-2.0.1/MParT/AffineFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/AffineMap.h` & `MParT-2.0.1/MParT/AffineMap.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/ComposedMap.h` & `MParT-2.0.1/MParT/ComposedMap.h`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         @details This function will copy the provided coeffs vectors into the savedCoeffs object in the ComposedMap class.   To avoid
         duplicating the coefficients, the savedCoeffs member variable for each component will then be set to a subview of this vector.
         @param coeffs A vector containing coefficients for all components.  If component \f$k\f$ is defined by \f$C_k\f$ coefficients,
                   then this vector should have length \f$\sum_{k=1}^K C_i\f$ and the coefficients for component \f$k\f$ should
                   start at index \f$\sum_{j=1}^{k-1} C_j\f$.
     */
     using ConditionalMapBase<MemorySpace>::SetCoeffs;
-    void SetCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs) override;
+    void SetCoeffs(Kokkos::View<const double*, Kokkos::HostSpace> coeffs) override;
     void WrapCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs) override;
 
     #if defined(MPART_ENABLE_GPU)
-    void SetCoeffs(Kokkos::View<double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs) override;
+    void SetCoeffs(Kokkos::View<const double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs) override;
     void WrapCoeffs(Kokkos::View<double*, mpart::DeviceSpace> coeffs) override;
     #endif
 
     virtual std::shared_ptr<ConditionalMapBase<MemorySpace>> GetComponent(unsigned int i){ return maps_.at(i);}
 
     /** @brief Computes the log determinant of the Jacobian matrix of this map.
```

### Comparing `MParT-1.4.4/MParT/ConditionalMapBase.h` & `MParT-2.0.1/MParT/ConditionalMapBase.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/DerivativeFlags.h` & `MParT-2.0.1/MParT/DerivativeFlags.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Distributions/DensityBase.h` & `MParT-2.0.1/MParT/Distributions/DensityBase.h`

 * *Files 0% similar despite different names*

```diff
@@ -75,11 +75,10 @@
      * @return unsigned int dimension of the density
      */
     virtual unsigned int Dim() const { return dim_; }
 
 protected:
     const unsigned int dim_;
 };
-
 }
 
 #endif // MPART_DensityBase_H
```

### Comparing `MParT-1.4.4/MParT/Distributions/Distribution.h` & `MParT-2.0.1/MParT/Distributions/Distribution.h`

 * *Files 16% similar despite different names*

```diff
@@ -102,22 +102,45 @@
      * @param pts dim x N data matrix where N is the number of points
      * @param output dim x N matrix with \f$\frac{\partial p}{\partial x_i}(\mathbf{t}_j)\f$ in the (i,j) entry (where \f$\mathbf{t}_j\f$ is the j-th data point)
      */
     void LogDensityInputGradImpl(StridedMatrix<const double, MemorySpace> const &pts, StridedMatrix<double, MemorySpace> output) {
         density_->LogDensityInputGradImpl(pts, output);
     };
 
+    /**
+     * @brief Get the Sampler object from the distribution
+     *
+     * @return std::shared_ptr<SampleGenerator<MemorySpace>> a shared pointer to the sampler that this object uses
+     */
+    std::shared_ptr<SampleGenerator<MemorySpace>> GetSampler() const { return sampler_; };
+
+    /**
+     * @brief Get the Density object from the distribution
+     *
+     * @return std::shared_ptr<DensityBase<MemorySpace>> a shared pointer to the density this object uses
+     */
+    std::shared_ptr<DensityBase<MemorySpace>> GetDensity() const { return density_; };
+
     private:
     std::shared_ptr<SampleGenerator<MemorySpace>> sampler_;
     std::shared_ptr<DensityBase<MemorySpace>> density_;
 
 }; // class Distribution
 
+/**
+ * @brief Convenient way to create a Distribution object from arguments to create an object that's both a sampler + density
+ *
+ * @tparam MemorySpace Where the data is stored for computation
+ * @tparam SamplerDensity The type of object that's both a sampler and a density
+ * @tparam T Parameter pack representing the argument types for the SamplerDensity constructor
+ * @param args arguments to create the SamplerDensity instance
+ * @return std::shared_ptr<Distribution<MemorySpace>> A distribution with sampler & density as the same object, constructed from args
+ */
 template<typename MemorySpace, typename SamplerDensity, typename... T>
-Distribution<MemorySpace> CreateDistribution(T... args) {
+std::shared_ptr<Distribution<MemorySpace>> CreateDistribution(T... args) {
     std::shared_ptr<SamplerDensity> samplerDensity = std::make_shared<SamplerDensity>(args...);
-    return Distribution<MemorySpace>(samplerDensity, samplerDensity);
+    return std::make_shared<Distribution<MemorySpace>>(samplerDensity, samplerDensity);
 };
 
 } // namespace mpart
 
 #endif //MPART_Distribution_H
```

### Comparing `MParT-1.4.4/MParT/Distributions/GaussianSamplerDensity.h` & `MParT-2.0.1/MParT/Distributions/GaussianSamplerDensity.h`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,18 @@
         logDetCov_ = std::log(covChol_.determinant());
     }
 
     private:
     StridedVector<double, MemorySpace> mean_;
     mpart::Cholesky<MemorySpace> covChol_;
     bool idCov_ = false;
-    double logDetCov_;
+    double logDetCov_ = 0.;
 };
 
 template<typename MemorySpace, typename... T>
-Distribution<MemorySpace> CreateGaussianDistribution(T... args) {
+std::shared_ptr<Distribution<MemorySpace>> CreateGaussianDistribution(T... args) {
     return CreateDistribution<MemorySpace,GaussianSamplerDensity<MemorySpace>>(args...);
 }
 
 } // namespace mpart
 
 #endif //MPART_GaussianSamplerDensity_H
```

### Comparing `MParT-1.4.4/MParT/Distributions/SampleGenerator.h` & `MParT-2.0.1/MParT/Distributions/SampleGenerator.h`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     };
 
     /**
      * @brief Set the Seed for the random pool, reinitializing it to ensure sampling has reproducible behavior
      *
      * @param seed new seed to set for the pool
      */
-    void SetSeed(unsigned int seed) {
+    virtual void SetSeed(unsigned int seed) {
         rand_pool = PoolType(seed);
     }
 
     /** Sample function with conversion from Kokkos to Eigen (and possibly copy to/from device). */
     // Eigen::RowMatrixXd SampleEigen(unsigned int N);
     using PoolType = typename Kokkos::Random_XorShift64_Pool<typename MemoryToExecution<MemorySpace>::Space>;
```

### Comparing `MParT-1.4.4/MParT/HermiteFunction.h` & `MParT-2.0.1/MParT/HermiteFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/IdentityMap.h` & `MParT-2.0.1/MParT/IdentityMap.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Initialization.h` & `MParT-2.0.1/MParT/Initialization.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/LinearizedBasis.h` & `MParT-2.0.1/MParT/LinearizedBasis.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MapFactory.h` & `MParT-2.0.1/MParT/MapFactory.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MonotoneComponent.h` & `MParT-2.0.1/MParT/MonotoneComponent.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MonotoneIntegrand.h` & `MParT-2.0.1/MParT/MonotoneIntegrand.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MultiIndices/FixedMultiIndexSet.h` & `MParT-2.0.1/MParT/MultiIndices/FixedMultiIndexSet.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MultiIndices/MultiIndex.h` & `MParT-2.0.1/MParT/MultiIndices/MultiIndex.h`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         @return A string showing the dense representation of the multiindex, e.g., "[0,1,4,2]"
     */
     std::string String() const;
 
     /** Get the number of components in the index.  When used to define a
         multivariate polynomial, this will return the dimension of the
         polynomial.
-        @return The length of the multiindex.  When used for defining multivariate polynomials, 
+        @return The length of the multiindex.  When used for defining multivariate polynomials,
                 this will be the dimension of the polynomial.
     */
     unsigned int Length() const{return length;};
 
     /** Check for equality of the multiindices.
         @param[in] b The multiindex to compare with *this.
         @return true if both multiindices have the same lengths, nonzero indices, and nonzero values.  Returns false otherwise.
@@ -117,68 +117,77 @@
 
     /** Check if two multiindices are different.
         @param[in] b The multiindex to compare with *this.
         @return false if both multiindices have the same lengths, nonzero indices, and nonzero values.  true otherwise.
     */
     bool operator!=(const MultiIndex &b) const;
 
-    /** 
+    /**
         Check if this multiindex is less than b.  The multiindices are ordered such that:
-        
+
         a<b if:
         - the length of a is less than the length of b OR
         - the lengths are the same, but the total order of "a" is less than the total order of "b" OR
         - the length and total orders are the same, but the max value of "a" is less than the max value of "b" OR
         - the lengths, total orders, and max values are the same, but "a" is lexicographically less than "b"
 
         @param[in] b The multiindex to compare with *this.
         @return true if *this < b according to the ordering described above.  false otherwise.
     */
     bool operator<(const MultiIndex &b) const;
 
-    /** 
+    /**
         Check if this multiindex is greather than b.  The multiindices are ordered such that:
-        
+
         a<b if:
         - the length of a is less than the length of b OR
         - the lengths are the same, but the total order of "a" is less than the total order of "b" OR
         - the length and total orders are the same, but the max value of "a" is less than the max value of "b" OR
         - the lengths, total orders, and max values are the same, but "a" is lexicographically less than "b"
 
         @param[in] b The multiindex to compare with *this.
         @return true if *this > b according to the ordering described above.  false otherwise.
     */
     bool operator>(const MultiIndex &b) const;
 
-    /** 
-        Check if this multiindex is greater than or equal to b.  This is checked by returning 
+    /**
+        Check if this multiindex is greater than or equal to b.  This is checked by returning
         "not (a<b)"
 
         @param[in] b The multiindex to compare with *this.
         @return true if *this >= b,  false otherwise.
     */
     bool operator>=(const MultiIndex &b) const;
 
-    /** 
-        Check if this multiindex is greater than or equal to b.  This is checked by returning 
+    /**
+        Check if this multiindex is greater than or equal to b.  This is checked by returning
         "not (a>b)"
 
         @param[in] b The multiindex to compare with *this.
         @return true if *this <= b,  false otherwise.
     */
     bool operator<=(const MultiIndex &b) const;
 
+    /**
+     * @brief Similar to operator>=, but bound must same length or longer. Further, it only
+     * returns false if every value in this is less than every value in bound.
+     *
+     * @param bound bound for this multiindex
+     * @return true if any value this[j] is at or above bound[j]
+     * @return false else
+     */
+    bool AnyBounded(const MultiIndex &bound) const;
 private:
 
     unsigned int length;
 
     /// a vector holding pairs of (dimension,index) for nonzero values of index.
     std::vector<unsigned int> nzInds;
     std::vector<unsigned int> nzVals;
-    
+
     /// The maximum index over all nzInds pairs.
     unsigned int maxValue;
 
     // the total order of the multiindex (i.e. the sum of the indices)
     unsigned int totalOrder;
 
 }; // class MultiIndex
```

### Comparing `MParT-1.4.4/MParT/MultiIndices/MultiIndexLimiter.h` & `MParT-2.0.1/MParT/MultiIndices/MultiIndexLimiter.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MultiIndices/MultiIndexNeighborhood.h` & `MParT-2.0.1/MParT/MultiIndices/MultiIndexNeighborhood.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MultiIndices/MultiIndexSet.h` & `MParT-2.0.1/MParT/MultiIndices/MultiIndexSet.h`

 * *Files 2% similar despite different names*

```diff
@@ -37,37 +37,37 @@
   /**
    Factory method for constructing a total order limited multiindex set.
    @param[in] length The length of the multiindices stored in this set.
    @param[in] maxOrder The maximum order of multiindices to include.
    @param[in] limiter An optional additional limiter to attach to the set.  Only multiindices that satisfy this limiter will be included.
    @return MultiIndexSet An instance of the MultiIndexSet class containing all multiindices of order <= maxOrder AND satisfying the limiter.
   */
-  static MultiIndexSet CreateTotalOrder(unsigned int length, 
-                                        unsigned int maxOrder, 
+  static MultiIndexSet CreateTotalOrder(unsigned int length,
+                                        unsigned int maxOrder,
                                         LimiterType const& limiter = MultiIndexLimiter::None());
 
   /**
    Factory method for constructing a full tensor product multiindex set.
    @param[in] length The length of the multiindices stored in this set.
    @param[in] maxDegree The maximum value allowed in any multiindex.
    @param[in] limiter An optional additional limiter to attach to the set.  Only multiindices that satisfy this limiter will be included.
    @return MultiIndexSet An instance of the MultiIndexSet class containing all multiindices with components a_i <= maxDegree AND satisfying the limiter.
   */
-  static MultiIndexSet CreateTensorProduct(unsigned int length, 
-                                           unsigned int maxOrder, 
+  static MultiIndexSet CreateTensorProduct(unsigned int length,
+                                           unsigned int maxOrder,
                                            LimiterType const& limiter = MultiIndexLimiter::None());
 
 
   /**
    @brief Construct a new MultiIndexSet object with a specific length.
-   @details Constructs an empty MultiIndexSet to store multi-indices of a specified length.  Also allows 
-            a functor to be be passed in as an additional limiter on the admissible set.  If no functor is 
-            provided, it is possible to include any multi-index in \f$\mathbb{N}^D\f$.  
+   @details Constructs an empty MultiIndexSet to store multi-indices of a specified length.  Also allows
+            a functor to be be passed in as an additional limiter on the admissible set.  If no functor is
+            provided, it is possible to include any multi-index in \f$\mathbb{N}^D\f$.
 
-            For example, to construct a MultiIndexSet in 2 dimensions that only allows multi-indices with maximum 
+            For example, to construct a MultiIndexSet in 2 dimensions that only allows multi-indices with maximum
             degree less than 5, we could use a lambda function:
 @code{.cpp}
 unsigned int length =2;
 auto limiter = [](MultiIndex const& multi) {return multi.Max()<5;};
 MultiIndexSet set(length, limiter);
 @endcode
             Multiple pre-defined limiter functors are defined in the mpart::MultiIndexLimiter namespace.
@@ -81,17 +81,17 @@
                 std::shared_ptr<MultiIndexNeighborhood> neigh = std::make_shared<DefaultNeighborhood>() );
 
   /** Each row of the input matrix is a multiindex. */
   MultiIndexSet(Eigen::Ref<const Eigen::MatrixXi> const& multis);
 
   /**
    @brief Converts this multiindex set into the fixed representation provided by the "FixedMultiIndexSet" class.
-   @details The FixedMultiIndexSet cannot easily be adapted, but stores the multiindices in a contiguous block of memory 
-            in a Kokkos::View that can be more amenable to fast computation.   This function creates an instance of the 
-            FixedMultiIndexSet from the current state of *this.   Note that memory is deep copied and any subsequent updates 
+   @details The FixedMultiIndexSet cannot easily be adapted, but stores the multiindices in a contiguous block of memory
+            in a Kokkos::View that can be more amenable to fast computation.   This function creates an instance of the
+            FixedMultiIndexSet from the current state of *this.   Note that memory is deep copied and any subsequent updates
             to this class will not result in updates to the FixedMultiIndexSet.
    @param[in] compress Should the fixed representation be in compressed format?
    @return An instance of the FixedMultiIndexSet class with a snapshot of the current state of this MultiIndexSet.
    */
   FixedMultiIndexSet<Kokkos::HostSpace> Fix(bool compress=true) const;
 
   /** Set the limiter of this MultiIndexSet.  This function will check to make
@@ -176,33 +176,36 @@
             already in the set and if the input function is unique, it is
             added to the set.
     @param[in] rhs The MultiIndex we want to add to the set.
     @return A reference to this MultiIndex, which may now contain the new
             MultiIndex in rhs.
     */
   MultiIndexSet& operator+=(MultiIndex const& rhs);
-  
+
   friend MultiIndexSet operator+(MultiIndexSet lhs, const MultiIndex& rhs)
   {
     lhs += rhs;
     return lhs;
   }
 
   /** Assignment operator.  Will throw a runtime_error exception if the rhs does not have the same size of *this. */
   MultiIndexSet& operator=(const MultiIndexSet& rhs);
 
+  /** Checks which MultiIndices exceed a given MultiIndex bound */
+  std::vector<bool> FilterBounded(const MultiIndex& bound) const;
+
   /** @brief Add all terms in rhs to this instance.
     @details This function adds all unique MultiIndices from the rhs into this MultiIndexSet.  In the event that a multiindex is active in one set, but not the other, the union will set that multiindex to be active.
     @param[in] rhs The MultiIndex set we want to add to this instance.
     @return The number of unique terms from rhs that were added to this set.
     */
   unsigned int Union(const MultiIndexSet &rhs);
 
   /**
-      Make the multi-index active. If the multiIndex is not admissable, an exception 
+      Make the multi-index active. If the multiIndex is not admissable, an exception
       will be thrown.  To be admissable (according to this function), the multiIndex
       must already exist as an inactive member of this set.  If that is not the case,
       use the AddActive function instead.
       @param[in] multiIndex A multiindex to make active. Note that an assert will fail if multiIndex is not admissable.
   */
   void Activate(MultiIndex const& multiIndex);
 
@@ -267,23 +270,23 @@
       Note that a forward neighbor must be admissible according to the limiter currently in place
       to be considered in the definition of the frontier.
       @return A vector with linear indices for active multi-indices on the frontier.
   */
   std::vector<unsigned int> Frontier() const;
 
 
-  /** Returns multiindices in the margin of the set.  The margin contains multiindices in the 
+  /** Returns multiindices in the margin of the set.  The margin contains multiindices in the
       limiting set that also have at least one active backward neighbor.
-      @return A std::vector containing the multiindices in the margin 
+      @return A std::vector containing the multiindices in the margin
   */
   std::vector<MultiIndex> Margin() const;
 
-  /** Returns multiindices in the reduced margin of the set.  A multiindex is in the reduced 
+  /** Returns multiindices in the reduced margin of the set.  A multiindex is in the reduced
       margin if it is in the limiting set and all of its backward neighbors are active.
-      @return A std::vector containing the multiindices in the reduced margin 
+      @return A std::vector containing the multiindices in the reduced margin
   */
   std::vector<MultiIndex> ReducedMargin() const;
 
 
   /** We define the strict frontier to be the collection of multiindices, where
       all admissible forward neighbors are inactive.
       @return A vector with linear indices for active multi-indices on the strict frontier.
@@ -292,28 +295,28 @@
 
   /** Returns the indices for the backward neighbors of a currently active multiindex.
   @param[in] activeIndex The linear index of the MultiIndex of interest
   @return A std::vector containing the linear indices of the backward neighbors.
   */
   std::vector<unsigned int> BackwardNeighbors(unsigned int activeIndex) const;
 
-  /** Returns indices for backward neighbors of an active or inactive multiindex. 
+  /** Returns indices for backward neighbors of an active or inactive multiindex.
   @param[in] multiIndex The multiindex in question.
   @return A vector with linear indices for the backward neighbors of this multiindex.
   */
   std::vector<unsigned int> BackwardNeighbors(MultiIndex const& multiIndex) const;
 
   /**
   Determines whether the input multiIndex is currently admissible.
   @param[in] multiIndex The multiindex to consider.
   @return true if the multiIndex is admissible.  false otherwise.
   */
   bool IsAdmissible(MultiIndex const& multiIndex) const;
 
-  /** 
+  /**
   Check to see if any forward neighbors of a multiIndex are admissible but not active.
   @param[in] activeIndex The linear index of the multi-index in question.
   @return true if this multiindex has at least one admissible but inactive forward neighbor.
   */
   bool IsExpandable(unsigned int activeIndex) const;
 
   ///Return true if the multiIndex is active
@@ -324,58 +327,58 @@
 
   /// Returns the number of forward neighbors (active or inactive)
   unsigned int NumForward(unsigned int activeInd) const;
 
   /** Visualizes a two-dimensional MultiIndexSet as ASCII art using "a" to denote active multiindices, "r" to denoted multiindices in the reduced margin (not active), and "m" to denoted multiindices in the margin (also not active).
       Note that the `MultiIndexSet::at` and `MultiIndexSet::IndexToMulti` only provide access to the active multiindices.  The inactive multiindices in the margin
       are typically only used for adaptation.
-      
-   The output for a total order limited set with max order 11 looks like 
-  @code 
-12 | r  
-11 | a  r  
-10 | a  a  r  
- 9 | a  a  a  r  
- 8 | a  a  a  a  r  
- 7 | a  a  a  a  a  r  
- 6 | a  a  a  a  a  a  r  
- 5 | a  a  a  a  a  a  a  r  
- 4 | a  a  a  a  a  a  a  a  r  
- 3 | a  a  a  a  a  a  a  a  a  r  
- 2 | a  a  a  a  a  a  a  a  a  a  r  
- 1 | a  a  a  a  a  a  a  a  a  a  a  r  
- 0 | a  a  a  a  a  a  a  a  a  a  a  a  r  
+
+   The output for a total order limited set with max order 11 looks like
+  @code
+12 | r
+11 | a  r
+10 | a  a  r
+ 9 | a  a  a  r
+ 8 | a  a  a  a  r
+ 7 | a  a  a  a  a  r
+ 6 | a  a  a  a  a  a  r
+ 5 | a  a  a  a  a  a  a  r
+ 4 | a  a  a  a  a  a  a  a  r
+ 3 | a  a  a  a  a  a  a  a  a  r
+ 2 | a  a  a  a  a  a  a  a  a  a  r
+ 1 | a  a  a  a  a  a  a  a  a  a  a  r
+ 0 | a  a  a  a  a  a  a  a  a  a  a  a  r
     ----------------------------------------
-     0  1  2  3  4  5  6  7  8  9  10 11 12 
-  @endcode 
+     0  1  2  3  4  5  6  7  8  9  10 11 12
+  @endcode
 
 Another example for an adaptively constructed set is
-  @code 
- 4 | r  
- 3 | a  m  
- 2 | a  r  
- 1 | a  a  r  m  
- 0 | a  a  a  a  r  
+  @code
+ 4 | r
+ 3 | a  m
+ 2 | a  r
+ 1 | a  a  r  m
+ 0 | a  a  a  a  r
     ----------------
-     0  1  2  3  4 
+     0  1  2  3  4
   @endcode
 
 The following is the same set as before, but with a multiindex limiter preventing expansion of mixed terms
-@code 
- 4 | r  
- 3 | a  
- 2 | a  
- 1 | a  a  
- 0 | a  a  a  a  r  
+@code
+ 4 | r
+ 3 | a
+ 2 | a
+ 1 | a  a
+ 0 | a  a  a  a  r
     ----------------
      0  1  2  3  4
 @endcode
 
-  @param[in,out] out The output stream where the visualization should be written.  Defaults to std::cout.  
-  */ 
+  @param[in,out] out The output stream where the visualization should be written.  Defaults to std::cout.
+  */
   void Visualize(std::ostream &out = std::cout) const;
 
 protected:
 
   // A vector of both active and admissable multiindices.  Global index.
   std::vector<MultiIndex> allMultis;
 
@@ -408,21 +411,21 @@
 
   std::vector<unsigned int> maxOrders; // the maximum order in each dimension
 
 private:
 
   int AddMulti(MultiIndex const& newMulti);
 
-  static void RecursiveTotalOrderFill(unsigned int   maxOrder, 
+  static void RecursiveTotalOrderFill(unsigned int   maxOrder,
                                       MultiIndexSet &mset,
                                       unsigned int currDim,
                                       std::vector<unsigned int> &denseMulti,
                                       LimiterType const& limiter);
 
-  static void RecursiveTensorFill(unsigned int   maxOrder, 
+  static void RecursiveTensorFill(unsigned int   maxOrder,
                                       MultiIndexSet &mset,
                                       unsigned int currDim,
                                       std::vector<unsigned int> &denseMulti,
                                       LimiterType const& limiter);
 
   std::shared_ptr<MultiIndexNeighborhood> neighborhood;
   std::map<MultiIndex, unsigned int> multi2global; // map from a multiindex to an integer
```

### Comparing `MParT-1.4.4/MParT/MultivariateExpansion.h` & `MParT-2.0.1/MParT/MultivariateExpansion.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/MultivariateExpansionWorker.h` & `MParT-2.0.1/MParT/MultivariateExpansionWorker.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/OrthogonalPolynomial.h` & `MParT-2.0.1/MParT/OrthogonalPolynomial.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/ParameterizedFunctionBase.h` & `MParT-2.0.1/MParT/ParameterizedFunctionBase.h`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,30 @@
         */
         virtual Kokkos::View<double*, MemorySpace>& Coeffs(){return this->savedCoeffs;};
 
         /** @brief Set the internally stored view of coefficients.
             @detail Performs a deep copy of the input coefficients to the internally stored coefficients.
             @param coeffs A view containing the coefficients to copy.
         */
-       virtual void SetCoeffs(Kokkos::View<double*, MemorySpace> coeffs);
+       virtual void SetCoeffs(Kokkos::View<const double*, MemorySpace> coeffs);
 
        #if defined(MPART_ENABLE_GPU)
-       void SetCoeffs(Kokkos::View<double*, std::conditional_t<std::is_same_v<MemorySpace,Kokkos::HostSpace>,mpart::DeviceSpace,Kokkos::HostSpace>> coeffs);
+       void SetCoeffs(Kokkos::View<const double*, std::conditional_t<std::is_same_v<MemorySpace,Kokkos::HostSpace>,mpart::DeviceSpace,Kokkos::HostSpace>> coeffs);
        #endif
 
         /** @brief Wrap the internal coefficient view around another view.
             @detail Performs a shallow copy of the input coefficients to the internally stored coefficients.
             If values in the view passed to this function are changed, the values will also change in the
             internally stored view.
             @param coeffs A view containing the coefficients we want to wrap.
         */
         virtual void WrapCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs);
 
         #if defined(MPART_ENABLE_GPU)
-        virtual void SetCoeffs(Kokkos::View<double*, mpart::DeviceSpace> coeffs);
+        virtual void SetCoeffs(Kokkos::View<const double*, mpart::DeviceSpace> coeffs);
         virtual void WrapCoeffs(Kokkos::View<double*, mpart::DeviceSpace> coeffs);
         #endif
 
         /** SetCoeffs function with conversion from Eigen to Kokkos vector types.*/
         virtual void SetCoeffs(Eigen::Ref<Eigen::VectorXd> coeffs);
         void WrapCoeffs(Eigen::Ref<Eigen::VectorXd> coeffs);
 
@@ -176,15 +176,15 @@
         virtual void CoeffGradImpl(StridedMatrix<const double, MemorySpace> const& pts,
                                    StridedMatrix<const double, MemorySpace> const& sens,
                                    StridedMatrix<double, MemorySpace>              output) = 0;
 
         /** Checks to see if the coefficients have been initialized yet, returns true if so, false if not */
         bool CheckCoefficients() const;
 
-        
+
         const unsigned int inputDim; /// The total dimension of the input N+M
         const unsigned int outputDim; /// The output dimension M
         const unsigned int numCoeffs; /// The number of coefficients used to parameterize this map.
 
 #if defined(MPART_HAS_CEREAL)
         template <typename Archive>
         void serialize(Archive & ar){
```

### Comparing `MParT-1.4.4/MParT/PositiveBijectors.h` & `MParT-2.0.1/MParT/PositiveBijectors.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Quadrature.h` & `MParT-2.0.1/MParT/Quadrature.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/SummarizedMap.h` & `MParT-2.0.1/MParT/SummarizedMap.h`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 
     */
     SummarizedMap(std::shared_ptr<ParameterizedFunctionBase<MemorySpace>> const& summary, std::shared_ptr<ConditionalMapBase<MemorySpace>> const& component);
 
     virtual ~SummarizedMap() = default;
 
     using ConditionalMapBase<MemorySpace>::SetCoeffs;
-    void SetCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs) override;
+    void SetCoeffs(Kokkos::View<const double*, Kokkos::HostSpace> coeffs) override;
     void WrapCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs) override;
     #if defined(MPART_ENABLE_GPU)
-    void SetCoeffs(Kokkos::View<double*, DeviceSpace> coeffs) override;
+    void SetCoeffs(Kokkos::View<const double*, DeviceSpace> coeffs) override;
     void WrapCoeffs(Kokkos::View<double*, DeviceSpace> coeffs) override;
     #endif
 
     void SummarizePts(StridedMatrix<const double, MemorySpace> const&  pts,
                       StridedMatrix<double, MemorySpace>               output);
```

### Comparing `MParT-1.4.4/MParT/TensorProductFunction.h` & `MParT-2.0.1/MParT/TensorProductFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/TriangularMap.h` & `MParT-2.0.1/MParT/TriangularMap.h`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     @details This function will copy the provided coeffs vectors into the savedCoeffs object in the TriangularMap class.   To avoid
     duplicating the coefficients, the savedCoeffs member variable for each component will then be set to a subview of this vector.
     @param coeffs A vector containing coefficients for all components.  If component \f$k\f$ is defined by \f$C_k\f$ coefficients,
                   then this vector should have length \f$\sum_{k=1}^K C_i\f$ and the coefficients for component \f$k\f$ should
                   start at index \f$\sum_{j=1}^{k-1} C_j\f$.
     */
     using ParameterizedFunctionBase<MemorySpace>::SetCoeffs;
-    void SetCoeffs(Kokkos::View<double*, MemorySpace> coeffs) override;
+    void SetCoeffs(Kokkos::View<const double*, MemorySpace> coeffs) override;
     void WrapCoeffs(Kokkos::View<double*, MemorySpace> coeffs) override;
 
     virtual std::shared_ptr<ConditionalMapBase<MemorySpace>> GetComponent(unsigned int i){ return comps_.at(i);}
 
     /** @brief Computes the log determinant of the Jacobian matrix of this map.
 
     @details
```

### Comparing `MParT-1.4.4/MParT/Utilities/ArrayConversions.h` & `MParT-2.0.1/MParT/Utilities/ArrayConversions.h`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
     template<typename ScalarType, typename MemorySpace = Kokkos::HostSpace>
     inline Kokkos::View<ScalarType*,MemorySpace> ToKokkos(ScalarType* ptr, unsigned int dim)
     {
         return Kokkos::View<ScalarType*, MemorySpace, Kokkos::MemoryTraits<Kokkos::Unmanaged>>(ptr, dim);
     }
 
     template<typename ScalarType, typename MemorySpace = Kokkos::HostSpace>
-    inline Kokkos::View<const ScalarType*,MemorySpace> ToConstKokkos(ScalarType* ptr, unsigned int dim)
+    inline Kokkos::View<const ScalarType*,MemorySpace> ToConstKokkos(const ScalarType* const_ptr, unsigned int dim)
     {
+        ScalarType* ptr = const_cast<ScalarType*>(const_ptr);
         return Kokkos::View<const ScalarType*, MemorySpace, Kokkos::MemoryTraits<Kokkos::Unmanaged>>(ptr, dim);
     }
 
     /** @brief Converts a pointer to a 2d unmanaged Kokkos view.
         @ingroup ArrayUtilities
         @details Creates a Kokkos unmanaged view around a preallocated block of memory.
                  The unmanaged view will not free the memory so all allocations and deallocations
@@ -92,16 +93,17 @@
     template<typename ScalarType, typename LayoutType=Kokkos::LayoutLeft, typename MemorySpace=Kokkos::HostSpace>
     inline Kokkos::View<ScalarType**, LayoutType, MemorySpace> ToKokkos(ScalarType* ptr, unsigned int rows, unsigned int cols)
     {
         return Kokkos::View<ScalarType**, LayoutType, MemorySpace, Kokkos::MemoryTraits<Kokkos::Unmanaged>>(ptr, rows, cols);
     }
 
     template<typename ScalarType, typename LayoutType=Kokkos::LayoutLeft, typename MemorySpace=Kokkos::HostSpace>
-    inline Kokkos::View<const ScalarType**, LayoutType, MemorySpace> ToConstKokkos(ScalarType* ptr, unsigned int rows, unsigned int cols)
+    inline Kokkos::View<const ScalarType**, LayoutType, MemorySpace> ToConstKokkos(const ScalarType* const_ptr, unsigned int rows, unsigned int cols)
     {
+        ScalarType* ptr = const_cast<ScalarType*>(const_ptr);
         return Kokkos::View<const ScalarType**, LayoutType, MemorySpace, Kokkos::MemoryTraits<Kokkos::Unmanaged>>(ptr, rows, cols);
     }
 
 
     /**
      * @brief Returns a copy of a one dimensional Kokkos::View in the form of a std::vector.
      *
@@ -129,14 +131,29 @@
     template<typename ScalarType, class MemorySpace>
     StridedVector<ScalarType, MemorySpace> VecToKokkos(std::vector<ScalarType> &vec)
     {
         return Kokkos::View<ScalarType*, MemorySpace>(vec.data(), vec.size());
     }
 
     /**
+     * @brief Wraps a const std::vector in a StridedVector
+     *
+     * @tparam ScalarType
+     * @tparam MemorySpace
+     * @param vec
+     * @return StridedVector<ScalarType*, MemorySpace>
+     */
+    template<typename ScalarType, class MemorySpace>
+    StridedVector<ScalarType, MemorySpace> ConstVecToKokkos(const std::vector<ScalarType> &vec)
+    {
+        double* ptr = const_cast<double*>(vec.data());
+        return Kokkos::View<ScalarType*, MemorySpace>(ptr, vec.size());
+    }
+
+    /**
      * @brief Wraps a std::vector in a StridedMatrix
      *
      * @tparam ScalarType
      * @tparam MemorySpace
      * @param vec
      * @return Kokkos::View<ScalarType*, MemorySpace>
      */
```

### Comparing `MParT-1.4.4/MParT/Utilities/KokkosHelpers.h` & `MParT-2.0.1/MParT/Utilities/KokkosHelpers.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Utilities/KokkosSpaceMappings.h` & `MParT-2.0.1/MParT/Utilities/KokkosSpaceMappings.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Utilities/LinearAlgebra.h` & `MParT-2.0.1/MParT/Utilities/LinearAlgebra.h`

 * *Files 7% similar despite different names*

```diff
@@ -226,14 +226,62 @@
 {
     assert(A.cols() == B.rows());
     Kokkos::View<double**, Kokkos::LayoutLeft, MemorySpace> C("C", A.rows(), B.cols());
     dgemm<MemorySpace>(1.0, A, B, 0.0, C);
     return C;
 }
 
+enum class ReduceDimMap { sum, norm };
+
+template<ReduceDimMap Map>
+KOKKOS_INLINE_FUNCTION double ReduceDimMapKernel(double) {return 0.;};
+
+template<>
+KOKKOS_INLINE_FUNCTION double ReduceDimMapKernel<ReduceDimMap::sum>(double x) {return x;};
+
+template<>
+KOKKOS_INLINE_FUNCTION double ReduceDimMapKernel<ReduceDimMap::norm>(double x) {return x*x;};
+
+
+// This struct allows you to reduce the columns of a mxn matrix
+// Performs alpha*A*[1,...,1]
+template<ReduceDimMap Map, typename MemorySpace, unsigned int Dim = 1, typename = std::enable_if_t<Dim <= 1,int> >
+struct ReduceDim {
+    using value_type = double[];
+    using size_type = typename StridedMatrix<double, MemorySpace>::size_type;
+
+    // Keep track of the dimension we are not reducing
+    size_type value_count;
+
+    StridedMatrix<const double, MemorySpace> A_;
+    double alpha_;
+
+    ReduceDim(StridedMatrix<double, MemorySpace> A, double alpha): value_count(A.extent(1-Dim)), A_(A), alpha_(alpha) {}
+
+    KOKKOS_INLINE_FUNCTION void operator()(const size_type reduce_idx, value_type sum) const {
+        for(size_type full_idx=0; full_idx<value_count; ++full_idx) {
+            double aij = 0.;
+            if(Dim == 1) aij = A_(full_idx,reduce_idx);
+            else aij = A_(reduce_idx,full_idx);
+            sum[full_idx] += ReduceDimMapKernel<Map>(aij)*alpha_;
+        }
+    }
+
+    KOKKOS_INLINE_FUNCTION void join (volatile value_type dst, const volatile value_type src) const {
+        for (size_type i = 0; i < value_count; ++i) {
+            dst[i] += src[i];
+        }
+    }
+
+    KOKKOS_INLINE_FUNCTION void init (value_type sum) const {
+        for (size_type i = 0; i < value_count; ++i) {
+            sum[i] = 0.0;
+        }
+    }
+};
 
 /** Mimics the interface of the Eigen::PartialPivLU class, but using Kokkos::Views and CUBLAS/CUSOLVER linear algebra.
 
 Note that the layout of the matrices used in this class is important.  Cublas expects column major (layout left).
 */
 template<typename MemorySpace>
 class PartialPivLU
```

### Comparing `MParT-1.4.4/MParT/Utilities/Miscellaneous.h` & `MParT-2.0.1/MParT/Utilities/Miscellaneous.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/MParT/Utilities/Serialization.h` & `MParT-2.0.1/MParT/Utilities/Serialization.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/PKG-INFO` & `MParT-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MParT
-Version: 1.4.4
+Version: 2.0.1
 Summary: A Monotone Parameterization Toolkit
 Author: Matthew Parno
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Massachusetts Institute of Technology
         All rights reserved.
```

### Comparing `MParT-1.4.4/README.md` & `MParT-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/CMakeLists.txt` & `MParT-2.0.1/bindings/python/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,41 @@
-set(JULIA_BINDING_SOURCES
-  src/CommonJuliaUtilities.cpp
-  src/ConditionalMapBase.cpp
-  src/JlArrayConversions.cpp
-  src/MapFactory.cpp
-  src/MapOptions.cpp
+
+set(PYTHON_BINDING_SOURCES
+  src/Wrapper.cpp
+  src/CommonPybindUtilities.cpp
   src/MultiIndex.cpp
+  src/MapOptions.cpp
+  src/ConditionalMapBase.cpp
   src/ParameterizedFunctionBase.cpp
-  src/TriangularMap.cpp
-  src/Wrapper.cpp
   src/AffineMap.cpp
+  src/TriangularMap.cpp
   src/ComposedMap.cpp
+  src/SummarizedMap.cpp
+  # src/DebugMap.cpp
+  src/MapFactory.cpp
+  src/IdentityMap.cpp
+
   ../common/src/CommonUtilities.cpp
 )
 
+if(MPART_ARCHIVE)
+  set(PYTHON_BINDING_SOURCES ${PYTHON_BINDING_SOURCES}
+    src/Serialization.cpp
+  )
+endif()
+
+if(MPART_OPT)
+  set(PYTHON_BINDING_SOURCES ${PYTHON_BINDING_SOURCES}
+    src/MapObjective.cpp
+    src/TrainMap.cpp
+    src/TrainMapAdaptive.cpp
+  )
+endif()
+
 include_directories(./include ../common/include)
-add_library(mpartjl SHARED ${JULIA_BINDING_SOURCES})
-target_link_libraries(mpartjl PRIVATE mpart JlCxx::cxxwrap_julia JlCxx::cxxwrap_julia_stl Kokkos::kokkos Eigen3::Eigen ${EXT_LIBRARIES})
+pybind11_add_module(pympart SHARED NO_EXTRAS ${PYTHON_BINDING_SOURCES})
+
+target_link_libraries(pympart PRIVATE mpart Kokkos::kokkos Eigen3::Eigen ${EXT_LIBRARIES})
 
-# Add an installation target for the julia bindings
-install(TARGETS mpartjl DESTINATION "${JULIA_INSTALL_PREFIX}")
+# Add an installation target for the python bindings
+install(TARGETS pympart DESTINATION "${PYTHON_INSTALL_PREFIX}")
+install(DIRECTORY package/ DESTINATION "${PYTHON_INSTALL_PREFIX}")
```

### Comparing `MParT-1.4.4/bindings/julia/include/CommonJuliaUtilities.h` & `MParT-2.0.1/bindings/julia/include/CommonJuliaUtilities.h`

 * *Files 14% similar despite different names*

```diff
@@ -67,14 +67,36 @@
 
 /**
  * @brief Adds ComposedMap bindings to the existing module m.
  * @param mod CxxWrap.jl module
  */
 void ComposedMapWrapper(jlcxx::Module &);
 
+#if defined(MPART_HAS_NLOPT)
+
+/**
+ * @brief Adds MapObjective bindings to the existing module m.
+ * @param mod CxxWrap.jl module
+ */
+void MapObjectiveWrapper(jlcxx::Module &);
+
+/**
+ * @brief Adds TrainMap and TrainOptions bindings to the existing module m.
+ * @param mod CxxWrap.jl module
+ */
+void TrainMapWrapper(jlcxx::Module&);
+
+/**
+ * @brief Adds TrainMapAdaptive and ATMOptions to the existing module m.
+ * @param mod CxxWrap.jl module
+*/
+void TrainMapAdaptiveWrapper(jlcxx::Module&);
+
+#endif // defined(MPART_HAS_NLOPT)
+
 #if defined(MPART_ENABLE_GPU)
 void ConditionalMapBaseDeviceWrapper(jlcxx::Module&);
 #endif
 
 } // namespace binding
 } // namespace mpart
```

### Comparing `MParT-1.4.4/bindings/julia/include/JlArrayConversions.h` & `MParT-2.0.1/bindings/julia/include/JlArrayConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/src/AffineMap.cpp` & `MParT-2.0.1/bindings/julia/src/AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/src/CommonJuliaUtilities.cpp` & `MParT-2.0.1/bindings/julia/src/CommonJuliaUtilities.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/src/ConditionalMapBase.cpp` & `MParT-2.0.1/bindings/julia/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/src/JlArrayConversions.cpp` & `MParT-2.0.1/bindings/julia/src/JlArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/julia/src/TriangularMap.cpp` & `MParT-2.0.1/bindings/julia/src/TriangularMap.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+#include <memory>
 #include "MParT/TriangularMap.h"
 
 #include "CommonJuliaUtilities.h"
 #include "JlArrayConversions.h"
 
 namespace jlcxx {
     // Tell CxxWrap.jl the supertype structure for TriangularMap
     template<> struct SuperType<mpart::TriangularMap<Kokkos::HostSpace>> {typedef mpart::ConditionalMapBase<Kokkos::HostSpace> type;};
 }
 
 void mpart::binding::TriangularMapWrapper(jlcxx::Module &mod) {
     mod.add_type<TriangularMap<Kokkos::HostSpace>>("TriangularMap", jlcxx::julia_base_type<ConditionalMapBase<Kokkos::HostSpace>>())
-       .constructor<std::vector<std::shared_ptr<ConditionalMapBase<Kokkos::HostSpace>>>>()
        .method("InverseInplace", [](TriangularMap<Kokkos::HostSpace> &map, jlcxx::ArrayRef<double,2> x, jlcxx::ArrayRef<double,2> r){
             map.InverseInplace(JuliaToKokkos(x), JuliaToKokkos(r));
        })
        .method("GetComponent", &TriangularMap<Kokkos::HostSpace>::GetComponent)
     ;
+
+    mod.method("TriangularMap", [](std::vector<std::shared_ptr<ConditionalMapBase<Kokkos::HostSpace>>> vec){
+        return std::static_pointer_cast<ConditionalMapBase<Kokkos::HostSpace>>(std::make_shared<TriangularMap<Kokkos::HostSpace>>(vec));
+    });
+
 }
```

### Comparing `MParT-1.4.4/bindings/matlab/CMakeLists.txt` & `MParT-2.0.1/bindings/matlab/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,21 @@
     src/KokkosUtilities_mex.cpp
     src/ConditionalMap_mex.cpp
     src/MultiIndexSet_mex.cpp
     src/MultiIndex_mex.cpp
     src/FixedMultiIndexSet_mex.cpp
     src/ParameterizedFunctionBase_mex.cpp
     src/MexArrayConversions.cpp
-    src/MexMapOptionsConversions.cpp
+    src/MexOptionsConversions.cpp
 )
 
+if(MPART_OPT)
+    set(MEX_SOURCE ${MEX_SOURCE}
+        src/MapObjective_mex.cpp
+    )
+endif()
+
 matlab_add_mex(NAME MParT_ SRC ${MEX_SOURCE} LINK_TO mpart Kokkos::kokkos Eigen3::Eigen ${EXT_LIBRARIES})
 
 # Add an installation target for the matlab bindings
 install(TARGETS MParT_ DESTINATION matlab)
 install(DIRECTORY mat/ DESTINATION matlab)
```

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus/LICENSE` & `MParT-2.0.1/bindings/matlab/external/mexplus/LICENSE`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/arguments.h` & `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/arguments.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/dispatch.h` & `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/dispatch.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/mxarray.h` & `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxarray.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus/mexplus/mxtypes.h` & `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxtypes.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/external/mexplus_eigen.h` & `MParT-2.0.1/bindings/matlab/external/mexplus_eigen.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/include/MexArrayConversions.h` & `MParT-2.0.1/bindings/matlab/include/MexArrayConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/mat/ConditionalMap.m` & `MParT-2.0.1/bindings/matlab/mat/ConditionalMap.m`

 * *Files 2% similar despite different names*

```diff
@@ -65,29 +65,29 @@
         error("Wrong input arguments");
       end
     elseif(nargin==4)
       inputDim = varargin{1};
       outputDim = varargin{2};
       totalOrder = varargin{3};
       opts = varargin{4};
-      
+
       mexOptions = opts.getMexOptions;
 
       input_str=['MParT_(',char(39),'ConditionalMap_newTotalTriMap',char(39),',inputDim,outputDim,totalOrder'];
       for o=1:length(mexOptions)
         input_o=[',mexOptions{',num2str(o),'}'];
         input_str=[input_str,input_o];
       end
       input_str=[input_str,')'];
       this.id_ = eval(input_str);
 
     elseif(nargin==1)
          this.id_=MParT_('ConditionalMap_newTriMap', varargin{1});
     else
-        error('Invalid number of inputs') 
+        error('Invalid number of inputs')
     end
   end
 
   function delete(this)
   %DELETE Destructor.
     MParT_('ConditionalMap_deleteMap', this.id_);
   end
@@ -155,16 +155,21 @@
 
   function result = get_id(this)
     result = this.id_;
   end
 
   function result = outputDim(this)
     result = MParT_('ConditionalMap_outputDim',this.id_);
-  end 
+  end
 
   function result = inputDim(this)
     result = MParT_('ConditionalMap_inputDim',this.id_);
-  end 
+  end
+
+  function Serialize(this,filename)
+    MParT_('ConditionalMap_Serialize',this.id_,filename);
+  end
+
 
 end
 
 end
```

### Comparing `MParT-1.4.4/bindings/matlab/mat/FixedMultiIndexSet.m` & `MParT-2.0.1/bindings/matlab/mat/FixedMultiIndexSet.m`

 * *Files 6% similar despite different names*

```diff
@@ -43,10 +43,18 @@
     dim = MParT_('FixedMultiIndexSet_Length', this.id_);
   end 
 
   function result = get_id(this)
     result = this.id_;
   end
 
+  function Serialize(this,filename)
+    MParT_('FixedMultiIndexSet_Serialize', this.id_, filename);
+  end
+
+  function Deserialize(this,filename)
+    MParT_('FixedMultiIndexSet_Deserialize', this.id_, filename);
+  end
+
 end
 
 end
```

### Comparing `MParT-1.4.4/bindings/matlab/mat/MultiIndex.m` & `MParT-2.0.1/bindings/matlab/mat/MultiIndex.m`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/mat/MultiIndexSet.m` & `MParT-2.0.1/bindings/matlab/mat/MultiIndexSet.m`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/mat/ParameterizedFunction.m` & `MParT-2.0.1/bindings/matlab/mat/ParameterizedFunction.m`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,16 @@
 
   function result = outputDim(this)
     result = MParT_('ParameterizedFunction_outputDim',this.id_);
   end 
 
   function result = inputDim(this)
     result = MParT_('ParameterizedFunction_inputDim',this.id_);
-  end 
+  end
+
+  function Serialize(this,filename)
+    MParT_('ParameterizedFunction_Serialize',this.id_,filename);
+  end
 
 end
 
 end
```

### Comparing `MParT-1.4.4/bindings/matlab/src/BasisTypes_mex.cpp` & `MParT-2.0.1/bindings/matlab/src/BasisTypes_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/src/ConditionalMap_mex.cpp` & `MParT-2.0.1/bindings/matlab/src/ConditionalMap_mex.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,114 @@
-#include <mexplus.h>
+#include <chrono>
+#include <Eigen/Dense>
+
 #include "MParT/MultiIndices/MultiIndexSet.h"
 #include "MParT/Utilities/ArrayConversions.h"
-#include "MexArrayConversions.h"
-#include "MexMapOptionsConversions.h"
 #include "MParT/MapOptions.h"
 #include "MParT/MapFactory.h"
-#include "MParT/ConditionalMapBase.h"
-#include "MParT/TriangularMap.h"
-#include "MParT/ComposedMap.h"
-#include "MParT/AffineMap.h"
-#include <Eigen/Dense>
-
-
-#include <chrono>
+#include "MParT/TrainMap.h"
 
+#include "MexWrapperTypes.h"
+#include "MexArrayConversions.h"
+#include "MexOptionsConversions.h"
 
 using namespace mpart;
 using namespace mexplus;
 using MemorySpace = Kokkos::HostSpace;
 
-class ConditionalMapMex {       // The class
-public:             
-  std::shared_ptr<ConditionalMapBase<MemorySpace>> map_ptr;
-
-  ConditionalMapMex(FixedMultiIndexSet<MemorySpace> const& mset, 
-                    MapOptions                             opts){
-    map_ptr = MapFactory::CreateComponent<MemorySpace>(mset,opts);
-  }
-
-  ConditionalMapMex(std::shared_ptr<ConditionalMapBase<MemorySpace>> init_ptr){
-    map_ptr = init_ptr;
-  }
-
-  ConditionalMapMex(std::vector<std::shared_ptr<ConditionalMapBase<MemorySpace>>> blocks){
-    map_ptr = std::make_shared<TriangularMap<MemorySpace>>(blocks);
-  }
-  
-  ConditionalMapMex(unsigned int inputDim, unsigned int outputDim, unsigned int totalOrder, MapOptions opts){
-    map_ptr = MapFactory::CreateTriangular<MemorySpace>(inputDim,outputDim,totalOrder,opts);
-  }
-
-  ConditionalMapMex(std::vector<std::shared_ptr<ConditionalMapBase<MemorySpace>>> triMaps,std::string typeMap){
-    map_ptr = std::make_shared<ComposedMap<MemorySpace>>(triMaps);
-  }
-
-  ConditionalMapMex(StridedMatrix<double,MemorySpace> A, StridedVector<double,MemorySpace> b){
-    map_ptr = std::make_shared<AffineMap<MemorySpace>>(A,b);
-  }
-
-  ConditionalMapMex(StridedMatrix<double,MemorySpace> A){
-    map_ptr = std::make_shared<AffineMap<MemorySpace>>(A);
-  }
-
-  ConditionalMapMex(StridedVector<double,MemorySpace> b){
-    map_ptr = std::make_shared<AffineMap<MemorySpace>>(b);
-  }
-
-}; //end class
-
-class ParameterizedFunctionMex {       // The class
-public:             
-  std::shared_ptr<ParameterizedFunctionBase<MemorySpace>> fun_ptr;
-
-  ParameterizedFunctionMex(unsigned int outputDim, FixedMultiIndexSet<MemorySpace> const& mset, 
-                    MapOptions opts){
-    fun_ptr = MapFactory::CreateExpansion<MemorySpace>(outputDim,mset,opts);
-  }
-
-  ParameterizedFunctionMex(std::shared_ptr<ParameterizedFunctionBase<MemorySpace>> init_ptr){
-    fun_ptr = init_ptr;
-  }
-}; //end class
-
-// Instance manager for ConditionalMap.
-template class mexplus::Session<ConditionalMapMex>;
-template class mexplus::Session<ParameterizedFunctionMex>;
-
 namespace {
 
 
 MEX_DEFINE(ConditionalMap_newTriMap) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
-  
+
   InputArguments input(nrhs, prhs, 1);
   OutputArguments output(nlhs, plhs, 1);
 
   std::vector<intptr_t> list_id = input.get<std::vector<intptr_t>>(0);
   unsigned int numBlocks = list_id.size();
-  
+
   std::vector<std::shared_ptr<ConditionalMapBase<Kokkos::HostSpace>>> blocks(numBlocks);
   for(unsigned int i=0;i<numBlocks;++i){
-      const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(list_id.at(i)); 
+      const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(list_id.at(i));
       blocks.at(i) = condMap.map_ptr;
     }
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(blocks)));
 }
 
+#if defined(MPART_HAS_NLOPT)
+MEX_DEFINE(ConditionalMap_TrainMapAdaptive) (int nlhs, mxArray* plhs[],
+                                      int nrhs, const mxArray* prhs[]) {
+
+  InputArguments input(nrhs, prhs, 26);
+  OutputArguments output(nlhs, plhs, 1);
+
+  std::vector<intptr_t> list_id_mset = input.get<std::vector<intptr_t>>(0);
+  unsigned int numBlocks = list_id_mset.size();
+  std::vector<MultiIndexSet> mset0 {};
+  for(unsigned int i=0;i<numBlocks;++i){
+    MultiIndexSet *mset_i = Session<MultiIndexSet>::get(list_id_mset.at(i));
+    mset0.push_back(*mset_i);
+  }
+  MapObjectiveMex *obj = Session<MapObjectiveMex>::get(input.get(1));
+  std::shared_ptr<MapObjective<MemorySpace>> obj_ptr = obj->obj_ptr;
+  ATMOptions opts = binding::ATMOptionsFromMatlab(input, 2);
+  std::shared_ptr<ConditionalMapBase<Kokkos::HostSpace>> map = TrainMapAdaptive(mset0, obj_ptr, opts);
+  for(unsigned int i=0;i<numBlocks;++i){
+    MultiIndexSet *mset_i = Session<MultiIndexSet>::get(list_id_mset.at(i));
+    *mset_i = mset0[i];
+  }
+  output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(map)));
+}
+#endif // defined(MPART_HAS_NLOPT)
+
 MEX_DEFINE(ConditionalMap_newComposedMap) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
-  
+
   InputArguments input(nrhs, prhs, 1);
   OutputArguments output(nlhs, plhs, 1);
 
   std::vector<intptr_t> list_id = input.get<std::vector<intptr_t>>(0);
   unsigned int numMaps = list_id.size();
-  
+
   std::vector<std::shared_ptr<ConditionalMapBase<Kokkos::HostSpace>>> TriMaps(numMaps);
   for(unsigned int i=0;i<numMaps;++i){
-      const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(list_id.at(i)); 
+      const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(list_id.at(i));
       TriMaps.at(i) = condMap.map_ptr;
     }
   std::string typeMap = "composed";
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(TriMaps,typeMap)));
 }
 
 MEX_DEFINE(ConditionalMap_newAffineMapAb) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
-  
+
   InputArguments input(nrhs, prhs, 2);
   OutputArguments output(nlhs, plhs, 1);
 
   auto A = MexToKokkos2d(prhs[0]);
   auto b = MexToKokkos1d(prhs[1]);
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(A,b)));
 }
 
 MEX_DEFINE(ConditionalMap_newAffineMapA) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
-  
+
   InputArguments input(nrhs, prhs, 1);
   OutputArguments output(nlhs, plhs, 1);
 
   auto A = MexToKokkos2d(prhs[0]);
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(A)));
 }
 
 MEX_DEFINE(ConditionalMap_newAffineMapb) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
-  
+
   InputArguments input(nrhs, prhs, 1);
   OutputArguments output(nlhs, plhs, 1);
 
   auto b = MexToKokkos1d(prhs[0]);
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(b)));
 }
@@ -153,53 +118,100 @@
 
   InputArguments input(nrhs, prhs, 15);
   OutputArguments output(nlhs, plhs, 1);
   unsigned int inputDim = input.get<unsigned int>(0);
   unsigned int outputDim = input.get<unsigned int>(1);
   unsigned int totalOrder = input.get<unsigned int>(2);
 
-  MapOptions opts = MapOptionsFromMatlab(input.get<std::string>(3),input.get<std::string>(4),
+  MapOptions opts = binding::MapOptionsFromMatlab(input.get<std::string>(3),input.get<std::string>(4),
                                          input.get<std::string>(5),input.get<double>(6),
                                          input.get<double>(7),input.get<unsigned int>(8),
                                          input.get<unsigned int>(9),input.get<unsigned int>(10),
                                          input.get<bool>(11),input.get<double>(12),input.get<double>(13),input.get<bool>(14));
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(inputDim,outputDim,totalOrder,opts)));
 }
 
 MEX_DEFINE(ConditionalMap_newMap) (int nlhs, mxArray* plhs[],
                     int nrhs, const mxArray* prhs[]) {
 
   InputArguments input(nrhs, prhs, 13);
   OutputArguments output(nlhs, plhs, 1);
   const MultiIndexSet& mset = Session<MultiIndexSet>::getConst(input.get(0));
-  MapOptions opts = MapOptionsFromMatlab(input.get<std::string>(1),input.get<std::string>(2),
+  MapOptions opts = binding::MapOptionsFromMatlab(input.get<std::string>(1),input.get<std::string>(2),
                                          input.get<std::string>(3),input.get<double>(4),
                                          input.get<double>(5),input.get<unsigned int>(6),
                                          input.get<unsigned int>(7),input.get<unsigned int>(8),
                                          input.get<bool>(9),input.get<double>(10),input.get<double>(11),input.get<bool>(12));
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(mset.Fix(),opts)));
 }
 
 MEX_DEFINE(ConditionalMap_newMapFixed) (int nlhs, mxArray* plhs[],
                     int nrhs, const mxArray* prhs[]) {
 
   InputArguments input(nrhs, prhs, 13);
   OutputArguments output(nlhs, plhs, 1);
   const FixedMultiIndexSet<MemorySpace>& mset = Session<FixedMultiIndexSet<MemorySpace>>::getConst(input.get(0));
-  MapOptions opts = MapOptionsFromMatlab(input.get<std::string>(1),input.get<std::string>(2),
+  MapOptions opts = binding::MapOptionsFromMatlab(input.get<std::string>(1),input.get<std::string>(2),
                                          input.get<std::string>(3),input.get<double>(4),
                                          input.get<double>(5),input.get<unsigned int>(6),
                                          input.get<unsigned int>(7),input.get<unsigned int>(8),
                                          input.get<bool>(9),input.get<double>(10),input.get<double>(11),input.get<bool>(12));
 
   output.set(0, Session<ConditionalMapMex>::create(new ConditionalMapMex(mset,opts)));
 }
 
+MEX_DEFINE(GaussianKLObjective_TestError) (int nlhs, mxArray* plhs[],
+                    int nrhs, const mxArray* prhs[]) {
+  InputArguments input(nrhs, prhs, 2);
+  OutputArguments output(nlhs, plhs, 1);
+  const MapObjectiveMex& obj = Session<MapObjectiveMex>::getConst(input.get(0));
+  ConditionalMapMex *condMap = Session<ConditionalMapMex>::get(input.get(1));
+  std::shared_ptr<ConditionalMapBase<MemorySpace>> condMap_ptr = condMap->map_ptr;
+  output.set(0, obj.obj_ptr->TestError(condMap_ptr));
+}
+
+MEX_DEFINE(GaussianKLObjective_TrainCoeffGrad) (int nlhs, mxArray* plhs[],
+                    int nrhs, const mxArray* prhs[]) {
+  InputArguments input(nrhs, prhs, 3);
+
+  const MapObjectiveMex& obj = Session<MapObjectiveMex>::getConst(input.get(0));
+  ConditionalMapMex *condMap = Session<ConditionalMapMex>::get(input.get(1));
+  std::shared_ptr<ConditionalMapBase<MemorySpace>> condMap_ptr = condMap->map_ptr;
+  StridedVector<double, Kokkos::HostSpace> out = MexToKokkos1d(prhs[2]);
+  obj.obj_ptr->TrainCoeffGradImpl(condMap_ptr, out);
+}
+
+MEX_DEFINE(GaussianKLObjective_TrainError) (int nlhs, mxArray* plhs[],
+                    int nrhs, const mxArray* prhs[]) {
+  InputArguments input(nrhs, prhs, 2);
+  OutputArguments output(nlhs, plhs, 1);
+  const MapObjectiveMex& obj = Session<MapObjectiveMex>::getConst(input.get(0));
+  ConditionalMapMex *condMap = Session<ConditionalMapMex>::get(input.get(1));
+  std::shared_ptr<ConditionalMapBase<MemorySpace>> condMap_ptr = condMap->map_ptr;
+  output.set(0, obj.obj_ptr->TrainError(condMap_ptr));
+}
+
+#if defined(MPART_HAS_NLOPT)
+MEX_DEFINE(ConditionalMap_TrainMap) (int nlhs, mxArray* plhs[],
+                                     int nrhs, const mxArray* prhs[]) {
+    InputArguments input(nrhs, prhs, 11);
+    OutputArguments output(nlhs, plhs, 0);
+    ConditionalMapMex *condMap = Session<ConditionalMapMex>::get(input.get(0));
+    std::shared_ptr<ConditionalMapBase<MemorySpace>> condMap_ptr = condMap->map_ptr;
+    MapObjectiveMex *obj = Session<MapObjectiveMex>::get(input.get(1));
+    std::shared_ptr<MapObjective<MemorySpace>> obj_ptr = obj->obj_ptr;
+
+    TrainOptions opts  = binding::TrainOptionsFromMatlab(input, 2);
+
+    TrainMap<MemorySpace>(condMap_ptr, obj_ptr, opts);
+}
+#endif //defined(MPART_HAS_NLOPT)
+
 // Defines MEX API for delete.
 MEX_DEFINE(ConditionalMap_deleteMap) (int nlhs, mxArray* plhs[],
                     int nrhs, const mxArray* prhs[]) {
   InputArguments input(nrhs, prhs, 1);
   OutputArguments output(nlhs, plhs, 0);
   Session<ConditionalMapMex>::destroy(input.get(0));
 }
@@ -287,40 +299,40 @@
 MEX_DEFINE(ConditionalMap_Evaluate) (int nlhs, mxArray* plhs[],
                                      int nrhs, const mxArray* prhs[]) {
   InputArguments input(nrhs, prhs, 3);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
   StridedMatrix<const double, Kokkos::HostSpace> pts = MexToKokkos2d(prhs[1]);
-  StridedMatrix<double, Kokkos::HostSpace> out = MexToKokkos2d(prhs[2]); 
+  StridedMatrix<double, Kokkos::HostSpace> out = MexToKokkos2d(prhs[2]);
   condMap.map_ptr->EvaluateImpl(pts, out);
 }
 
 MEX_DEFINE(ConditionalMap_LogDeterminant) (int nlhs, mxArray* plhs[],
                                            int nrhs, const mxArray* prhs[]) {
 
   InputArguments input(nrhs, prhs, 3);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
-  
-  Kokkos::View<double*, Kokkos::HostSpace> out = MexToKokkos1d(prhs[2]);  
+
+  Kokkos::View<double*, Kokkos::HostSpace> out = MexToKokkos1d(prhs[2]);
   StridedMatrix<const double, Kokkos::HostSpace> pts = MexToKokkos2d(prhs[1]);
 
   condMap.map_ptr->LogDeterminantImpl(pts, out);
  }
 
 MEX_DEFINE(ConditionalMap_Inverse) (int nlhs, mxArray* plhs[],
                                     int nrhs, const mxArray* prhs[]) {
 
   InputArguments input(nrhs, prhs, 4);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
-  
+
   auto x1 = MexToKokkos2d(prhs[1]);
   auto r = MexToKokkos2d(prhs[2]);
   auto inv = MexToKokkos2d(prhs[3]);
 
   condMap.map_ptr->InverseImpl(x1,r, inv);
 }
 
@@ -331,55 +343,78 @@
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
 
   auto pts = MexToKokkos2d(prhs[1]);
   auto sens = MexToKokkos2d(prhs[2]);
   auto out = MexToKokkos2d(prhs[3]);
-  
+
   condMap.map_ptr->CoeffGradImpl(pts,sens,out);
 }
 
 MEX_DEFINE(ConditionalMap_Gradient) (int nlhs, mxArray* plhs[],
                                       int nrhs, const mxArray* prhs[]) {
 
   InputArguments input(nrhs, prhs, 4);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
 
   auto pts = MexToKokkos2d(prhs[1]);
   auto sens = MexToKokkos2d(prhs[2]);
   auto out = MexToKokkos2d(prhs[3]);
-  
+
   condMap.map_ptr->GradientImpl(pts,sens,out);
 }
 
 MEX_DEFINE(ConditionalMap_LogDeterminantCoeffGrad) (int nlhs, mxArray* plhs[],
                  int nrhs, const mxArray* prhs[]) {
   InputArguments input(nrhs, prhs, 3);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
 
   auto pts = MexToKokkos2d(prhs[1]);
   auto out = MexToKokkos2d(prhs[2]);
-  
+
   condMap.map_ptr->LogDeterminantCoeffGradImpl(pts,out);
 }
 
 MEX_DEFINE(ConditionalMap_LogDeterminantInputGrad) (int nlhs, mxArray* plhs[],
                  int nrhs, const mxArray* prhs[]) {
   InputArguments input(nrhs, prhs, 3);
   OutputArguments output(nlhs, plhs, 0);
 
   const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
 
   auto pts = MexToKokkos2d(prhs[1]);
   auto out = MexToKokkos2d(prhs[2]);
-  
+
   condMap.map_ptr->LogDeterminantInputGradImpl(pts,out);
 }
 
+MEX_DEFINE(ConditionalMap_Serialize) (int nlhs, mxArray* plhs[],
+                                      int nrhs, const mxArray* prhs[]) {
+
+#if defined(MPART_HAS_CEREAL)
+  InputArguments input(nrhs, prhs, 2);
+  OutputArguments output(nlhs, plhs, 0);
+
+  const ConditionalMapMex& condMap = Session<ConditionalMapMex>::getConst(input.get(0));
+  int inputDim = condMap.map_ptr->inputDim;
+  int outputDim = condMap.map_ptr->outputDim;
+  int numCoeffs = condMap.map_ptr->numCoeffs;
+  auto coeffs = condMap.map_ptr->Coeffs();
+  std::string filename = input.get<std::string>(1);
+  std::ofstream os(filename);
+  cereal::BinaryOutputArchive oarchive(os);
+  oarchive(inputDim,outputDim,numCoeffs);
+  oarchive(coeffs);
+#else
+  mexErrMsgIdAndTxt("MParT:NoCereal",
+                    "MParT was not compiled with Cereal support.");
+#endif // MPART_HAS_CEREAL
+}
+
 } // namespace
 
 MEX_DISPATCH // Don't forget to add this if MEX_DEFINE() is used.
```

### Comparing `MParT-1.4.4/bindings/matlab/src/MexArrayConversions.cpp` & `MParT-2.0.1/bindings/matlab/src/MexArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/src/MultiIndexSet_mex.cpp` & `MParT-2.0.1/bindings/matlab/src/MultiIndexSet_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/src/MultiIndex_mex.cpp` & `MParT-2.0.1/bindings/matlab/src/MultiIndex_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/tests/Test_MultiIndexSet.m` & `MParT-2.0.1/bindings/matlab/tests/Test_MultiIndexSet.m`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/matlab/tests/Test_TriangularMap.m` & `MParT-2.0.1/bindings/matlab/tests/Test_TriangularMap.m`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/include/CommonPybindUtilities.h` & `MParT-2.0.1/bindings/python/include/CommonPybindUtilities.h`

 * *Files 7% similar despite different names*

```diff
@@ -42,17 +42,33 @@
 
 template<typename MemorySpace>
 void IdentityMapWrapper(pybind11::module &m);
 
 // template<typename MemorySpace>
 // void DebugMapWrapper(pybind11::module &m);
 
+#if defined(MPART_HAS_NLOPT)
+void TrainOptionsWrapper(pybind11::module &m);
+
+template<typename MemorySpace>
+void MapObjectiveWrapper(pybind11::module &m);
+
 template<typename MemorySpace>
 void MapFactoryWrapper(pybind11::module &m);
 
+template<typename MemorySpace>
+void TrainMapWrapper(pybind11::module &m);
+
+void ATMOptionsWrapper(pybind11::module &m);
+
+template<typename MemorySpace>
+void TrainMapAdaptiveWrapper(pybind11::module &m);
+#endif
+
+
 #if defined(MPART_HAS_CEREAL)
 template<typename MemorySpace>
 void DeserializeWrapper(pybind11::module &m);
 #endif // MPART_HAS_CEREAL
 
 void AffineMapWrapperHost(pybind11::module &m);
 void AffineMapWrapperDevice(pybind11::module &m);
```

### Comparing `MParT-1.4.4/bindings/python/package/MParT.egg-info/PKG-INFO` & `MParT-2.0.1/bindings/python/package/MParT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MParT
-Version: 1.4.4
+Version: 2.0.1
 Summary: A Monotone Parameterization Toolkit
 Author: Matthew Parno
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Massachusetts Institute of Technology
         All rights reserved.
```

### Comparing `MParT-1.4.4/bindings/python/package/MParT.egg-info/SOURCES.txt` & `MParT-2.0.1/bindings/python/package/MParT.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,30 +23,38 @@
 MParT/ConditionalMapBase.h
 MParT/DerivativeFlags.h
 MParT/HermiteFunction.h
 MParT/IdentityMap.h
 MParT/Initialization.h
 MParT/LinearizedBasis.h
 MParT/MapFactory.h
+MParT/MapObjective.h
 MParT/MapOptions.h
 MParT/MonotoneComponent.h
 MParT/MonotoneIntegrand.h
 MParT/MultivariateExpansion.h
 MParT/MultivariateExpansionWorker.h
 MParT/OrthogonalPolynomial.h
 MParT/ParameterizedFunctionBase.h
 MParT/PositiveBijectors.h
 MParT/Quadrature.h
 MParT/SummarizedMap.h
 MParT/TensorProductFunction.h
+MParT/TrainMap.h
+MParT/TrainMapAdaptive.h
 MParT/TriangularMap.h
 MParT/Distributions/DensityBase.h
 MParT/Distributions/Distribution.h
 MParT/Distributions/GaussianSamplerDensity.h
+MParT/Distributions/PullbackDensity.h
+MParT/Distributions/PullbackSampler.h
+MParT/Distributions/PushforwardDensity.h
+MParT/Distributions/PushforwardSampler.h
 MParT/Distributions/SampleGenerator.h
+MParT/Distributions/TransportDistributionFactory.h
 MParT/MultiIndices/FixedMultiIndexSet.h
 MParT/MultiIndices/MultiIndex.h
 MParT/MultiIndices/MultiIndexLimiter.h
 MParT/MultiIndices/MultiIndexNeighborhood.h
 MParT/MultiIndices/MultiIndexSet.h
 MParT/Utilities/ArrayConversions.h
 MParT/Utilities/EigenTypes.h
@@ -64,92 +72,110 @@
 bindings/julia/include/JlArrayConversions.h
 bindings/julia/src/AffineMap.cpp
 bindings/julia/src/CommonJuliaUtilities.cpp
 bindings/julia/src/ComposedMap.cpp
 bindings/julia/src/ConditionalMapBase.cpp
 bindings/julia/src/JlArrayConversions.cpp
 bindings/julia/src/MapFactory.cpp
+bindings/julia/src/MapObjective.cpp
 bindings/julia/src/MapOptions.cpp
 bindings/julia/src/MultiIndex.cpp
 bindings/julia/src/ParameterizedFunctionBase.cpp
+bindings/julia/src/TrainMap.cpp
+bindings/julia/src/TrainMapAdaptive.cpp
 bindings/julia/src/TriangularMap.cpp
 bindings/julia/src/Wrapper.cpp
 bindings/matlab/CMakeLists.txt
 bindings/matlab/external/mexplus_eigen.h
 bindings/matlab/external/mexplus/LICENSE
 bindings/matlab/external/mexplus/mexplus.h
 bindings/matlab/external/mexplus/mexplus/arguments.h
 bindings/matlab/external/mexplus/mexplus/dispatch.h
 bindings/matlab/external/mexplus/mexplus/mxarray.h
 bindings/matlab/external/mexplus/mexplus/mxtypes.h
 bindings/matlab/include/MexArrayConversions.h
-bindings/matlab/include/MexMapOptionsConversions.h
+bindings/matlab/include/MexOptionsConversions.h
+bindings/matlab/include/MexWrapperTypes.h
+bindings/matlab/mat/ATMOptions.m
+bindings/matlab/mat/AdaptiveTransportMap.m
 bindings/matlab/mat/AffineMap.m
 bindings/matlab/mat/ComposedMap.m
 bindings/matlab/mat/ConditionalMap.m
 bindings/matlab/mat/CreateComponent.m
 bindings/matlab/mat/CreateTriangular.m
+bindings/matlab/mat/DeserializeMap.m
 bindings/matlab/mat/FixedMultiIndexSet.m
+bindings/matlab/mat/GaussianKLObjective.m
 bindings/matlab/mat/KokkosInitialize.m
 bindings/matlab/mat/MultiIndex.m
 bindings/matlab/mat/MultiIndexSet.m
 bindings/matlab/mat/ParameterizedFunction.m
+bindings/matlab/mat/TrainMap.m
+bindings/matlab/mat/TrainOptions.m
 bindings/matlab/mat/TriangularMap.m
 bindings/matlab/mat/MapOptions/BasisTypes.m
 bindings/matlab/mat/MapOptions/MapOptions.m
 bindings/matlab/mat/MapOptions/PosFuncTypes.m
 bindings/matlab/mat/MapOptions/QuadTypes.m
 bindings/matlab/src/BasisTypes_mex.cpp
 bindings/matlab/src/ConditionalMap_mex.cpp
 bindings/matlab/src/FixedMultiIndexSet_mex.cpp
 bindings/matlab/src/KokkosUtilities_mex.cpp
+bindings/matlab/src/MapObjective_mex.cpp
 bindings/matlab/src/MexArrayConversions.cpp
-bindings/matlab/src/MexMapOptionsConversions.cpp
+bindings/matlab/src/MexOptionsConversions.cpp
 bindings/matlab/src/MultiIndexSet_mex.cpp
 bindings/matlab/src/MultiIndex_mex.cpp
 bindings/matlab/src/ParameterizedFunctionBase_mex.cpp
 bindings/matlab/tests/FixedMultiIndexSetTest.m
 bindings/matlab/tests/Test_AffineMap.m
 bindings/matlab/tests/Test_ComposedMap.m
 bindings/matlab/tests/Test_MultiIndex.m
 bindings/matlab/tests/Test_MultiIndexSet.m
 bindings/matlab/tests/Test_ParameterizedFunction.m
 bindings/matlab/tests/Test_TriangularMap.m
+bindings/matlab/tests/TrainMapAdaptiveTest.m
+bindings/matlab/tests/TrainMapTest.m
 bindings/matlab/tests/runtests.m
 bindings/python/CMakeLists.txt
 bindings/python/include/CommonPybindUtilities.h
 bindings/python/package/__init__.py
 bindings/python/package/MParT.egg-info/PKG-INFO
 bindings/python/package/MParT.egg-info/SOURCES.txt
 bindings/python/package/MParT.egg-info/dependency_links.txt
 bindings/python/package/MParT.egg-info/top_level.txt
 bindings/python/src/AffineMap.cpp
 bindings/python/src/CommonPybindUtilities.cpp
 bindings/python/src/ComposedMap.cpp
 bindings/python/src/ConditionalMapBase.cpp
 bindings/python/src/IdentityMap.cpp
 bindings/python/src/MapFactory.cpp
+bindings/python/src/MapObjective.cpp
 bindings/python/src/MapOptions.cpp
 bindings/python/src/MultiIndex.cpp
 bindings/python/src/ParameterizedFunctionBase.cpp
 bindings/python/src/Serialization.cpp
 bindings/python/src/SummarizedMap.cpp
+bindings/python/src/TrainMap.cpp
+bindings/python/src/TrainMapAdaptive.cpp
 bindings/python/src/TriangularMap.cpp
 bindings/python/src/Wrapper.cpp
 bindings/python/tests/test_AffineFunction.py
 bindings/python/tests/test_AffineMap.py
 bindings/python/tests/test_ComposedMap.py
 bindings/python/tests/test_ComposedMap_moveCoeffs.py
 bindings/python/tests/test_ConditionalMapBase.py
 bindings/python/tests/test_IdentityMap.py
 bindings/python/tests/test_MapFactory.py
 bindings/python/tests/test_MultiIndex.py
 bindings/python/tests/test_MultiIndexSet.py
 bindings/python/tests/test_Serialization.py
 bindings/python/tests/test_SummarizedMap.py
+bindings/python/tests/test_TrainMap.py
+bindings/python/tests/test_TrainMapAdaptive.py
 bindings/python/tests/test_TriangularMap.py
 bindings/python/tests/test_TriangularMap_moveCoeffs.py
 cmake/BuildDocs.cmake
 cmake/FindJulia.cmake
 cmake/FindSphinx.cmake
 cmake/SetInstallPaths.cmake
 docs/Makefile
@@ -207,27 +233,34 @@
 src/MapFactoryImpl1.cpp
 src/MapFactoryImpl10.cpp
 src/MapFactoryImpl11.cpp
 src/MapFactoryImpl12.cpp
 src/MapFactoryImpl13.cpp
 src/MapFactoryImpl14.cpp
 src/MapFactoryImpl15.cpp
+src/MapFactoryImpl16.cpp
+src/MapFactoryImpl17.cpp
+src/MapFactoryImpl18.cpp
 src/MapFactoryImpl2.cpp
 src/MapFactoryImpl3.cpp
 src/MapFactoryImpl4.cpp
 src/MapFactoryImpl5.cpp
 src/MapFactoryImpl6.cpp
 src/MapFactoryImpl7.cpp
 src/MapFactoryImpl8.cpp
 src/MapFactoryImpl9.cpp
+src/MapObjective.cpp
 src/ParameterizedFunctionBase.cpp
 src/SummarizedMap.cpp
+src/TrainMap.cpp
+src/TrainMapAdaptive.cpp
 src/TriangularMap.cpp
 src/Distributions/DensityBase.cpp
 src/Distributions/GaussianSamplerDensity.cpp
+src/Distributions/PullbackDensity.cpp
 src/MultiIndices/FixedMultiIndexSet.cpp
 src/MultiIndices/MultiIndex.cpp
 src/MultiIndices/MultiIndexLimiter.cpp
 src/MultiIndices/MultiIndexNeighborhood.cpp
 src/MultiIndices/MultiIndexSet.cpp
 src/Utilities/LinearAlgebra.cpp
 src/Utilities/Miscellaneous.cpp
@@ -240,24 +273,31 @@
 tests/Test_ComposedMap.cpp
 tests/Test_ConditionalMapBase.cpp
 tests/Test_HermiteFunctions.cpp
 tests/Test_IdentityMap.cpp
 tests/Test_LinearAlgebra.cpp
 tests/Test_LinearizedBasis.cpp
 tests/Test_MapFactory.cpp
+tests/Test_MapObjective.cpp
 tests/Test_MonotoneComponent.cpp
 tests/Test_MultivariateExpansion.cpp
 tests/Test_MultivariateExpansionWorker.cpp
 tests/Test_OrthogonalPolynomials.cpp
 tests/Test_PositiveBijectors.cpp
 tests/Test_Quadrature.cpp
 tests/Test_Serialization.cpp
 tests/Test_SummarizedMap.cpp
 tests/Test_TensorProductFunction.cpp
+tests/Test_TrainMap.cpp
+tests/Test_TrainMapAdaptive.cpp
 tests/Test_TriangularMap.cpp
 tests/Distributions/Test_DensityBase.cpp
 tests/Distributions/Test_Distribution.cpp
+tests/Distributions/Test_Distributions_Common.cpp
 tests/Distributions/Test_Distributions_Common.h
 tests/Distributions/Test_GaussianDistribution.cpp
 tests/Distributions/Test_SampleGenerator.cpp
+tests/Distributions/Test_TransportDensity.cpp
+tests/Distributions/Test_TransportDistributionFactory.cpp
+tests/Distributions/Test_TransportSampler.cpp
 tests/MultiIndices/Test_MultiIndex.cpp
 tests/MultiIndices/Test_MultiIndexSet.cpp
```

### Comparing `MParT-1.4.4/bindings/python/src/AffineMap.cpp` & `MParT-2.0.1/bindings/python/src/AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/CommonPybindUtilities.cpp` & `MParT-2.0.1/bindings/python/src/CommonPybindUtilities.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/ComposedMap.cpp` & `MParT-2.0.1/bindings/python/src/ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/ConditionalMapBase.cpp` & `MParT-2.0.1/bindings/python/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/IdentityMap.cpp` & `MParT-2.0.1/bindings/python/src/IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/MapFactory.cpp` & `MParT-2.0.1/bindings/python/src/MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/MapOptions.cpp` & `MParT-2.0.1/bindings/python/src/MapOptions.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     .value("ClenshawCurtis",QuadTypes::ClenshawCurtis)
     .value("AdaptiveSimpson",QuadTypes::AdaptiveSimpson)
     .value("AdaptiveClenshawCurtis",QuadTypes::AdaptiveClenshawCurtis);
 
     // MapOptions
     py::class_<MapOptions, std::shared_ptr<MapOptions>>(m, "MapOptions")
     .def(py::init<>())
+    .def("__eq__", &MapOptions::operator==)
+    .def("__str__", &MapOptions::String)
+    .def("__repr__", [](MapOptions opts){return "<MapOptions with fields\n" + opts.String() + ">";})
     .def_readwrite("basisType", &MapOptions::basisType)
     .def_readwrite("basisLB", &MapOptions::basisLB)
     .def_readwrite("basisUB", &MapOptions::basisUB)
     .def_readwrite("basisNorm", &MapOptions::basisNorm)
     .def_readwrite("posFuncType", &MapOptions::posFuncType)
     .def_readwrite("quadType", &MapOptions::quadType)
     .def_readwrite("quadAbsTol", &MapOptions::quadAbsTol)
```

### Comparing `MParT-1.4.4/bindings/python/src/MultiIndex.cpp` & `MParT-2.0.1/bindings/python/src/MultiIndex.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,17 @@
             Eigen::Matrix<unsigned int, Eigen::Dynamic, 1> maxDegreesEigen(maxDegrees.extent(0));
             for (unsigned int i = 0; i < maxDegrees.extent(0); i++)
             {
                 maxDegreesEigen(i) = maxDegrees(i);
             }
             return maxDegreesEigen;
         })
-
+        .def("__len__", &FixedMultiIndexSet<Kokkos::HostSpace>::Length)
+        .def("Length", &FixedMultiIndexSet<Kokkos::HostSpace>::Length)
+        .def("Size", &FixedMultiIndexSet<Kokkos::HostSpace>::Size)
 #if defined(MPART_HAS_CEREAL)
         .def("Serialize", [](FixedMultiIndexSet<Kokkos::HostSpace> const &mset, std::string const &filename){
             std::ofstream os(filename);
             cereal::BinaryOutputArchive oarchive(os);
             oarchive(mset);
             return mset;
         })
```

### Comparing `MParT-1.4.4/bindings/python/src/ParameterizedFunctionBase.cpp` & `MParT-2.0.1/bindings/python/src/ParameterizedFunctionBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/Serialization.cpp` & `MParT-2.0.1/bindings/python/src/Serialization.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/SummarizedMap.cpp` & `MParT-2.0.1/bindings/python/src/SummarizedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/TriangularMap.cpp` & `MParT-2.0.1/bindings/python/src/TriangularMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/src/Wrapper.cpp` & `MParT-2.0.1/bindings/python/src/Wrapper.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,23 @@
     AffineMapWrapperHost(m);
     AffineFunctionWrapperHost(m);
     TriangularMapWrapper<Kokkos::HostSpace>(m);
     ComposedMapWrapper<Kokkos::HostSpace>(m);
     SummarizedMapWrapper<Kokkos::HostSpace>(m);
     IdentityMapWrapper<Kokkos::HostSpace>(m);
     // DebugMapWrapper<Kokkos::HostSpace>(m);
-
     MapFactoryWrapper<Kokkos::HostSpace>(m);
+    MapObjectiveWrapper<Kokkos::HostSpace>(m);
+
+#if defined(MPART_HAS_NLOPT)
+    TrainOptionsWrapper(m);
+    ATMOptionsWrapper(m);
+    TrainMapWrapper<Kokkos::HostSpace>(m);
+    TrainMapAdaptiveWrapper<Kokkos::HostSpace>(m);
+#endif // MPART_HAS_NLOPT
 
 #if defined(MPART_HAS_CEREAL)
     DeserializeWrapper<Kokkos::HostSpace>(m);
 #endif // MPART_HAS_CEREAL
 
 #if defined(MPART_ENABLE_GPU)
     ParameterizedFunctionBaseWrapper<mpart::DeviceSpace>(m);
```

### Comparing `MParT-1.4.4/bindings/python/tests/test_AffineFunction.py` & `MParT-2.0.1/bindings/python/tests/test_AffineFunction.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_AffineMap.py` & `MParT-2.0.1/bindings/python/tests/test_AffineMap.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_ComposedMap.py` & `MParT-2.0.1/bindings/python/tests/test_ComposedMap.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_ComposedMap_moveCoeffs.py` & `MParT-2.0.1/bindings/python/tests/test_ComposedMap_moveCoeffs.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_ConditionalMapBase.py` & `MParT-2.0.1/bindings/python/tests/test_ConditionalMapBase.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_IdentityMap.py` & `MParT-2.0.1/bindings/python/tests/test_IdentityMap.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_MapFactory.py` & `MParT-2.0.1/bindings/python/tests/test_MapFactory.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_MultiIndex.py` & `MParT-2.0.1/bindings/python/tests/test_MultiIndex.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_MultiIndexSet.py` & `MParT-2.0.1/bindings/python/tests/test_MultiIndexSet.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_Serialization.py` & `MParT-2.0.1/bindings/python/tests/test_Serialization.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_SummarizedMap.py` & `MParT-2.0.1/bindings/python/tests/test_SummarizedMap.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_TriangularMap.py` & `MParT-2.0.1/bindings/python/tests/test_TriangularMap.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/bindings/python/tests/test_TriangularMap_moveCoeffs.py` & `MParT-2.0.1/bindings/python/tests/test_TriangularMap_moveCoeffs.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/cmake/BuildDocs.cmake` & `MParT-2.0.1/cmake/BuildDocs.cmake`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/cmake/FindJulia.cmake` & `MParT-2.0.1/cmake/FindJulia.cmake`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/cmake/SetInstallPaths.cmake` & `MParT-2.0.1/cmake/SetInstallPaths.cmake`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/Makefile` & `MParT-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/_static/pics/Density.png` & `MParT-2.0.1/docs/_static/pics/Density.png`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/_static/pics/Regression.png` & `MParT-2.0.1/docs/_static/pics/Regression.png`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/_static/pics/Samples.png` & `MParT-2.0.1/docs/_static/pics/Samples.png`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/_static/pics/Transformation2d.png` & `MParT-2.0.1/docs/_static/pics/Transformation2d.png`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/conf.py` & `MParT-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/index.rst` & `MParT-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/make.bat` & `MParT-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/mpart.doxyfile.in` & `MParT-2.0.1/docs/mpart.doxyfile.in`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/api/concepts/cachedparameterization.rst` & `MParT-2.0.1/docs/source/api/concepts/cachedparameterization.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/api/multiindex.rst` & `MParT-2.0.1/docs/source/api/multiindex.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/api/templateconcepts.rst` & `MParT-2.0.1/docs/source/api/templateconcepts.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/api/utilities/linearalgebra.rst` & `MParT-2.0.1/docs/source/api/utilities/linearalgebra.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/api/utilities/serialization.rst` & `MParT-2.0.1/docs/source/api/utilities/serialization.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/development/index.rst` & `MParT-2.0.1/docs/source/development/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/getting_started.rst` & `MParT-2.0.1/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/installation.rst` & `MParT-2.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/mathematics.rst` & `MParT-2.0.1/docs/source/mathematics.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/docs/source/tutorials/index.rst` & `MParT-2.0.1/docs/source/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/joss/paper.bib` & `MParT-2.0.1/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/joss/paper.md` & `MParT-2.0.1/joss/paper.md`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/joss/performance_comparison.png` & `MParT-2.0.1/joss/performance_comparison.png`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/pyproject.toml` & `MParT-2.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 authors = [
     {name = "Matthew Parno"},
 ]
 license={file="LICENSE.txt"}
 readme="README.md"
 requires-python = ">=3.7"
 description="A Monotone Parameterization Toolkit"
-version="1.4.4"
+version="2.0.1"
 keywords=["Measure Transport", "Monotone", "Transport Map", "Isotonic Regression", "Triangular", "Knothe-Rosenblatt"]
 
 [project.urls]
 Documentation = "https://measuretransport.github.io/MParT/"
 Source = "https://github.com/MeasureTransport/MParT"
```

### Comparing `MParT-1.4.4/src/AffineFunction.cpp` & `MParT-2.0.1/src/AffineFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/AffineMap.cpp` & `MParT-2.0.1/src/AffineMap.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #include "MParT/AffineMap.h"
 #include "MParT/Utilities/KokkosSpaceMappings.h"
 
 #include "MParT/Utilities/ArrayConversions.h"
 #include "MParT/Initialization.h"
- 
+
 
 using namespace mpart;
 
 template<typename MemorySpace>
-AffineMap<MemorySpace>::AffineMap(StridedVector<double,MemorySpace> b) : ConditionalMapBase<MemorySpace>(b.size(),b.size(),0), 
-                                                                  b_("b",b.layout()), 
+AffineMap<MemorySpace>::AffineMap(StridedVector<double,MemorySpace> b) : ConditionalMapBase<MemorySpace>(b.size(),b.size(),0),
+                                                                  b_("b",b.layout()),
                                                                   logDet_(0.0)
 {
     Kokkos::deep_copy(b_, b);
 }
 
 template<typename MemorySpace>
 AffineMap<MemorySpace>::AffineMap(StridedMatrix<double,MemorySpace> A) : ConditionalMapBase<MemorySpace>(A.extent(1),A.extent(0),0),
@@ -26,15 +26,15 @@
 
 
 template<typename MemorySpace>
 AffineMap<MemorySpace>::AffineMap(StridedMatrix<double,MemorySpace> A,
                                   StridedVector<double,MemorySpace> b) : ConditionalMapBase<MemorySpace>(A.extent(1),A.extent(0),0),
                                                                   A_("A", A.layout()),
                                                                   b_("b",b.layout())
-{   
+{
     Kokkos::deep_copy(A_, A);
     Kokkos::deep_copy(b_, b);
     assert(A_.extent(0)<=A_.extent(1));
     assert(A_.extent(0) == b_.extent(0));
     Factorize();
 }
 
@@ -87,23 +87,23 @@
         }else{
             outLeft = Kokkos::View<double**, Kokkos::LayoutLeft, MemorySpace>("OutLeft", output.extent(0), output.extent(1));
             copyOut = true;
         }
     }else{
         outLeft = output;
     }
-    
+
     // Bias part
     if(b_.size()>0){
 
         Kokkos::MDRangePolicy<Kokkos::Rank<2>, typename MemoryToExecution<MemorySpace>::Space> policy({{0, 0}}, {{numPts, this->outputDim}});
 
         // After this for loop, we will have out = r - b
         Kokkos::parallel_for(policy, KOKKOS_CLASS_LAMBDA(const int& j, const int& i) {
-            outLeft(i,j) = r(i,j) - b_(i); 
+            outLeft(i,j) = r(i,j) - b_(i);
         });
 
     }else{
         Kokkos::deep_copy(outLeft, r);
     }
 
     // Linear part
@@ -111,35 +111,35 @@
 
         int nrows = A_.extent(0);
         int ncols = A_.extent(1);
 
         // If the matrix is rectangular, treat it as the lower part of a block triangular matrix
         // The value of x1 contains the compute inverse for the first block
         if(nrows != ncols){
-            
+
             StridedMatrix<const double, MemorySpace> xsub = Kokkos::subview(x1, std::make_pair(0,ncols-nrows), Kokkos::ALL());
             StridedMatrix<const double, MemorySpace> Asub = Kokkos::subview(A_, Kokkos::ALL(), std::make_pair(0,ncols-nrows));
 
             dgemm<MemorySpace>(-1.0, Asub, xsub, 1.0, outLeft);
         }
 
         // Now solve with the square block of A_
         luSolver_.solveInPlace(outLeft);
 
         // Copy the inverse back if necessary
         if(copyOut)
             Kokkos::deep_copy(output, outLeft);
     }
-    
+
 }
 
 
 
 template<typename MemorySpace>
-void AffineMap<MemorySpace>::LogDeterminantCoeffGradImpl(StridedMatrix<const double, MemorySpace> const& pts, 
+void AffineMap<MemorySpace>::LogDeterminantCoeffGradImpl(StridedMatrix<const double, MemorySpace> const& pts,
                                                          StridedMatrix<double, MemorySpace>              output)
 {
     return;
 }
 
 template<typename MemorySpace>
 void AffineMap<MemorySpace>::EvaluateImpl(StridedMatrix<const double, MemorySpace> const& pts,
@@ -147,44 +147,44 @@
 {
     // Linear part
     if(A_.extent(0)>0){
         dgemm<MemorySpace>(1.0, A_, pts, 0.0, output);
     }else{
         Kokkos::deep_copy(output, pts);
     }
-    
+
     // Bias part
     if(b_.size()>0){
 
         unsigned int numPts = pts.extent(1);
         Kokkos::MDRangePolicy<Kokkos::Rank<2>, typename MemoryToExecution<MemorySpace>::Space> policy({{0, 0}}, {{numPts, this->outputDim}});
 
         Kokkos::parallel_for(policy, KOKKOS_CLASS_LAMBDA(const int& j, const int& i) {
             output(i,j) += b_(i);
         });
     }
 }
 
 template<typename MemorySpace>
-void AffineMap<MemorySpace>::CoeffGradImpl(StridedMatrix<const double, MemorySpace> const& pts,  
+void AffineMap<MemorySpace>::CoeffGradImpl(StridedMatrix<const double, MemorySpace> const& pts,
                                            StridedMatrix<const double, MemorySpace> const& sens,
                                            StridedMatrix<double, MemorySpace>              output)
 {
     return;
 }
 
-template<typename MemorySpace> 
-void AffineMap<MemorySpace>::LogDeterminantInputGradImpl(StridedMatrix<const double, MemorySpace> const& pts, 
+template<typename MemorySpace>
+void AffineMap<MemorySpace>::LogDeterminantInputGradImpl(StridedMatrix<const double, MemorySpace> const& pts,
                                                          StridedMatrix<double, MemorySpace>              output)
 {
     return;
 }
 
 template<typename MemorySpace>
-void AffineMap<MemorySpace>::GradientImpl(StridedMatrix<const double, MemorySpace> const& pts,  
+void AffineMap<MemorySpace>::GradientImpl(StridedMatrix<const double, MemorySpace> const& pts,
                                           StridedMatrix<const double, MemorySpace> const& sens,
                                           StridedMatrix<double, MemorySpace>              output)
 {
     // Linear part
     if(A_.extent(0)>0){
         dgemm<MemorySpace>(1.0, transpose(A_), sens, 0.0, output);
     }else{
@@ -192,8 +192,8 @@
     }
 }
 
 
 template class mpart::AffineMap<Kokkos::HostSpace>;
 #if defined(MPART_ENABLE_GPU)
     template class mpart::AffineMap<mpart::DeviceSpace>;
-#endif 
+#endif
```

### Comparing `MParT-1.4.4/src/CMakeLists.txt` & `MParT-2.0.1/src/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,32 @@
+
+if (MPART_OPT)
+    set(MPART_OPT_FILES
+        MapObjective.cpp
+        TrainMap.cpp
+        TrainMapAdaptive.cpp
+    )
+else()
+    set(MPART_OPT_FILES "")
+endif ()
+
 target_sources(mpart
     PRIVATE
     MultiIndices/MultiIndex.cpp
     MultiIndices/MultiIndexLimiter.cpp
     MultiIndices/MultiIndexSet.cpp
     MultiIndices/FixedMultiIndexSet.cpp
     MultiIndices/MultiIndexNeighborhood.cpp
 
     Utilities/Miscellaneous.cpp
     Utilities/LinearAlgebra.cpp
 
     Distributions/DensityBase.cpp
     Distributions/GaussianSamplerDensity.cpp
+    Distributions/PullbackDensity.cpp
 
     ParameterizedFunctionBase.cpp
     ConditionalMapBase.cpp
     TriangularMap.cpp
     IdentityMap.cpp
     ComposedMap.cpp
     SummarizedMap.cpp
@@ -34,10 +46,14 @@
     MapFactoryImpl9.cpp
     MapFactoryImpl10.cpp
     MapFactoryImpl11.cpp
     MapFactoryImpl12.cpp
     MapFactoryImpl13.cpp
     MapFactoryImpl14.cpp
     MapFactoryImpl15.cpp
+    MapFactoryImpl16.cpp
+    MapFactoryImpl17.cpp
+    MapFactoryImpl18.cpp
 
+    ${MPART_OPT_FILES}
     Initialization.cpp
 )
```

### Comparing `MParT-1.4.4/src/ComposedMap.cpp` & `MParT-2.0.1/src/ComposedMap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         }
 
         this->WrapCoeffs(coeffs);
     }
 }
 
 template<typename MemorySpace>
-void ComposedMap<MemorySpace>::SetCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs)
+void ComposedMap<MemorySpace>::SetCoeffs(Kokkos::View<const double*, Kokkos::HostSpace> coeffs)
 {
     // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::SetCoeffs(coeffs);
 
     // Now create subviews for each of the maps
     unsigned int cumNumCoeffs = 0;
     for(unsigned int i=0; i<maps_.size(); ++i){
@@ -209,15 +209,15 @@
             std::make_pair(cumNumCoeffs, cumNumCoeffs+maps_.at(i)->numCoeffs)));
         cumNumCoeffs += maps_.at(i)->numCoeffs;
     }
 }
 
 #if defined(MPART_ENABLE_GPU)
 template<typename MemorySpace>
-void ComposedMap<MemorySpace>::SetCoeffs(Kokkos::View<double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs)
+void ComposedMap<MemorySpace>::SetCoeffs(Kokkos::View<const double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs)
 {
     // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::SetCoeffs(coeffs);
 
     // Now create subviews for each of the maps
     unsigned int cumNumCoeffs = 0;
     for(unsigned int i=0; i<maps_.size(); ++i){
```

### Comparing `MParT-1.4.4/src/ConditionalMapBase.cpp` & `MParT-2.0.1/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/Distributions/DensityBase.cpp` & `MParT-2.0.1/src/Distributions/DensityBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/Distributions/GaussianSamplerDensity.cpp` & `MParT-2.0.1/src/Distributions/GaussianSamplerDensity.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -26,32 +26,32 @@
     if(M != dim_) {
         throw std::runtime_error("GaussianSamplerDensity::LogDensityImpl: The number of rows in pts must match the dimension of the distribution.");
     }
     Kokkos::MDRangePolicy<Kokkos::Rank<2>, typename MemoryToExecution<MemorySpace>::Space> policy({{0, 0}}, {{N, M}});
     Kokkos::View<double**, Kokkos::LayoutLeft, MemorySpace> diff ("diff", M, N);
 
     if(mean_.extent(0) == 0){
-        Kokkos::deep_copy(diff, pts);
+        Kokkos::parallel_for(policy, KOKKOS_LAMBDA(const int& j, const int& i) {
+            diff(i,j) = pts(i,j);
+        });
     }
     else {
         Kokkos::parallel_for(policy, KOKKOS_LAMBDA(const int& j, const int& i) {
             diff(i,j) = pts(i,j) - mean_(i);
         });
     }
 
     if(!idCov_) {
         covChol_.solveInPlaceL(diff);
     }
 
+    ReduceDim<ReduceDimMap::norm,MemorySpace,0> rr(diff, -0.5);
+    Kokkos::parallel_reduce(M, rr, &output(0));
     Kokkos::parallel_for( "log terms", N, KOKKOS_LAMBDA (const int& j) {
-        output(j) = -0.5*( M*logtau_ + logDetCov_ );
-    });
-
-    Kokkos::parallel_for( "weighted norm", policy, KOKKOS_LAMBDA (const int& j, const int& i) {
-        output(j) -= 0.5*diff(i,j)*diff(i,j);
+        output(j) -= 0.5*( M*logtau_ + logDetCov_ );
     });
 }
 
 template<typename MemorySpace>
 void GaussianSamplerDensity<MemorySpace>::LogDensityInputGradImpl(StridedMatrix<const double, MemorySpace> const &pts, StridedMatrix<double, MemorySpace> output) {
     // Compute the gradient of the log density
     int M = pts.extent(0);
@@ -77,44 +77,45 @@
     }
 }
 
 
 // Currently this requires that output be a LayoutLeft view
 template<typename MemorySpace>
 void GaussianSamplerDensity<MemorySpace>::SampleImpl(StridedMatrix<double, MemorySpace> output_) {
-    Kokkos::View<double**, Kokkos::LayoutLeft, MemorySpace> output = output_;
     // Sample from the distribution
-    int M = output.extent(0);
-    int N = output.extent(1);
+    int M = output_.extent(0);
+    int N = output_.extent(1);
     // Check dimensions
     if(M != dim_) {
         throw std::runtime_error("GaussianSamplerDensity::SampleImpl: The number of rows in output must match the dimension of the distribution.");
     }
     Kokkos::MDRangePolicy<Kokkos::Rank<2>, typename MemoryToExecution<MemorySpace>::Space> policy({{0, 0}}, {{N, M}});
     // If the covariance is the identity, we can just sample from a shifted normal
     if(idCov_) {
         // If dim_ is 0, the distribution is the standard normal
         if(mean_.extent(0) == 0) {
             Kokkos::parallel_for(policy, KOKKOS_LAMBDA(const int j, const int i) {
                 GeneratorType rgen = rand_pool.get_state();
-                output(i,j) = rgen.normal();
+                output_(i,j) = rgen.normal();
                 rand_pool.free_state(rgen);
             });
         }
         // Otherwise, we sample from the mean-shifted normal
         else {
             Kokkos::parallel_for(policy, KOKKOS_LAMBDA(const int j, const int i) {
                 GeneratorType rgen = rand_pool.get_state();
-                output(i,j) = rgen.normal() + mean_(i);
+                output_(i,j) = rgen.normal() + mean_(i);
                 rand_pool.free_state(rgen);
             });
         }
     }
     // Otherwise, we assume dense covariance
     else {
+        // Enforce that the output is the correct layout!
+        Kokkos::View<double**, Kokkos::LayoutLeft, MemorySpace> output = output_;
         // Sample from the standard normal
         Kokkos::parallel_for(policy, KOKKOS_LAMBDA(const int j, const int i) {
             GeneratorType rgen = rand_pool.get_state();
             output(i,j) = rgen.normal();
             rand_pool.free_state(rgen);
         });
         // Transform by the Cholesky factor
```

### Comparing `MParT-1.4.4/src/IdentityMap.cpp` & `MParT-2.0.1/src/IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactory.cpp` & `MParT-2.0.1/src/MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl1.cpp` & `MParT-2.0.1/src/MapFactoryImpl1.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl10.cpp` & `MParT-2.0.1/src/MapFactoryImpl10.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl11.cpp` & `MParT-2.0.1/src/MapFactoryImpl11.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl12.cpp` & `MParT-2.0.1/src/MapFactoryImpl12.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl13.cpp` & `MParT-2.0.1/src/MapFactoryImpl13.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl14.cpp` & `MParT-2.0.1/src/MapFactoryImpl14.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl15.cpp` & `MParT-2.0.1/src/MapFactoryImpl15.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl2.cpp` & `MParT-2.0.1/src/MapFactoryImpl2.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl3.cpp` & `MParT-2.0.1/src/MapFactoryImpl3.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl4.cpp` & `MParT-2.0.1/src/MapFactoryImpl4.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl5.cpp` & `MParT-2.0.1/src/MapFactoryImpl5.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl6.cpp` & `MParT-2.0.1/src/MapFactoryImpl6.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl7.cpp` & `MParT-2.0.1/src/MapFactoryImpl7.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl8.cpp` & `MParT-2.0.1/src/MapFactoryImpl8.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MapFactoryImpl9.cpp` & `MParT-2.0.1/src/MapFactoryImpl9.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MultiIndices/FixedMultiIndexSet.cpp` & `MParT-2.0.1/src/MultiIndices/FixedMultiIndexSet.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MultiIndices/MultiIndex.cpp` & `MParT-2.0.1/src/MultiIndices/MultiIndex.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,25 @@
     return !(*this < b);
 }
 
 bool MultiIndex::operator<=(const MultiIndex &b) const{
     return !(*this > b);
 }
 
+bool MultiIndex::AnyBounded(const MultiIndex &bound) const{
+  if(length > bound.length) {
+    throw std::invalid_argument("MultiIndex::AnyExceed: invalid length");
+  }
+  for(unsigned int i=0; i<length; ++i){
+    if(Get(i)>=bound.Get(i)){
+      return true;
+    }
+  }
+  return false;
+}
 
 std::string MultiIndex::String() const {
   std::string out;
   for(unsigned int i=0; i<Length(); ++i){
     if (i > 0)
       out += " ";
     out += std::to_string(Get(i));
```

### Comparing `MParT-1.4.4/src/MultiIndices/MultiIndexLimiter.cpp` & `MParT-2.0.1/src/MultiIndices/MultiIndexLimiter.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MultiIndices/MultiIndexNeighborhood.cpp` & `MParT-2.0.1/src/MultiIndices/MultiIndexNeighborhood.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/MultiIndices/MultiIndexSet.cpp` & `MParT-2.0.1/src/MultiIndices/MultiIndexSet.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -396,28 +396,46 @@
     }
 
   }
 }
 
 
 void MultiIndexSet::Visualize(std::ostream &out) const
-{ 
-  
+{
+  if(maxOrders.size() == 1) {
+    int dim = maxOrders.at(0);
+    out << " 0 | ";
+    for(int j = 0; j < dim; j++)
+        out << "a  ";
+    out << "\n    -";
+    for(int j = 0; j < dim; j++)
+        out << "--";
+    out << "\n     ";
+    for(int j = 0; j < dim; j++) {
+      out << j;
+      if(j < 10) out << "  ";
+      else out << " ";
+    }
+    out << std::endl;
+    return;
+  }
   unsigned int max_ord = maxOrders.at(1) + 1;
+
   for(unsigned int order = 0; order <= maxOrders.at(1) + 1; order++) {
     unsigned int i=max_ord - order;
 
     if(i<10)
       out << " ";
     out << i << " | ";
 
     for(unsigned int j=0; j<=maxOrders.at(0)+1; ++j){
 
       bool found = false;
       for(unsigned int k=0; k<active2global.size(); ++k){
+
         if((allMultis.at(active2global.at(k)).Get(0)==j)&&(allMultis.at(active2global.at(k)).Get(1)==i)){
           out << "a  ";
           found = true;
           break;
         }
       }
 
@@ -636,35 +654,53 @@
 
   std::vector<unsigned int> newIndices;
   unsigned int globalIndex = active2global.at(activeIndex);
 
   // loop through the forward neighbors of this index
   std::set<int> tempSet = outEdges.at(globalIndex);
   for(int neighbor : tempSet)
-  {
+  { 
     if(IsAdmissible(neighbor)&&(!IsActive(neighbor))){
       Activate(neighbor);
       newIndices.push_back(global2active.at(neighbor));
     }
   }
 
   // return the vector of newly activated indices
   return newIndices;
 }
 
 
 std::vector<unsigned int> MultiIndexSet::Expand()
 {
-  std::vector<unsigned int> frontier = Frontier();
-  std::vector<unsigned int> newInds, allNewInds;
-  for(auto& ind : frontier){
-    newInds = Expand(ind);
-    allNewInds.insert(allNewInds.end(), newInds.begin(), newInds.end());
-  }
-  return allNewInds;
+    // Figure out which terms in the frontier should be activated
+    std::vector<unsigned int> frontier = Frontier();
+    std::vector<unsigned int> toExpand; // Global indices to activate
+    for(auto& ind : frontier){
+
+        unsigned int globalIndex = active2global.at(ind);
+
+        // loop through the forward neighbors of this index
+        std::set<int> tempSet = outEdges.at(globalIndex);
+        for(int neighbor : tempSet)
+        { 
+            if(IsAdmissible(neighbor)&&(!IsActive(neighbor))){
+                toExpand.push_back(neighbor);
+            }
+        }
+    }
+
+    // Activate those terms
+    std::vector<unsigned int> allNewInds;
+    for(auto& neighbor : toExpand){ 
+        Activate(neighbor);
+        allNewInds.push_back(global2active.at(neighbor));
+    }
+    
+    return allNewInds;
 }
 
 std::vector<unsigned int> MultiIndexSet::ForciblyExpand(unsigned int const activeIndex)
 {
   assert(activeIndex<active2global.size());
 
   std::vector<unsigned int> newIndices;
@@ -718,14 +754,22 @@
 
 MultiIndexSet& MultiIndexSet::operator+=(const MultiIndexSet& rhs)
 {
   Union(rhs);
   return *this;
 }
 
+std::vector<bool> MultiIndexSet::FilterBounded(const MultiIndex& bound) const {
+  std::vector<bool> ret (active2global.size());
+  for(int i = 0; i < ret.size(); i++) {
+    ret[i] = allMultis[active2global[i]].AnyBounded(bound);
+  }
+  return ret;
+}
+
 unsigned int MultiIndexSet::Union(const MultiIndexSet& rhs)
 {
   int oldTerms = Size();
 
   for(unsigned int i = 0; i < rhs.allMultis.size(); ++i) {
 
     auto newMulti = rhs.allMultis.at(i);
@@ -753,14 +797,14 @@
         throw std::runtime_error("Cannot copy MultiIndexSet because sizes don't match.");
 
     this->allMultis = rhs.allMultis;
     this->limiter = rhs.limiter;
     this->active2global = rhs.active2global;
     this->global2active = rhs.global2active;
     this->outEdges = rhs.outEdges;
-    this->inEdges = rhs.inEdges; 
-    this->maxOrders = rhs.maxOrders; 
+    this->inEdges = rhs.inEdges;
+    this->maxOrders = rhs.maxOrders;
     this->neighborhood = rhs.neighborhood;
     this->multi2global = rhs.multi2global;
 
     return *this;
   }
```

### Comparing `MParT-1.4.4/src/ParameterizedFunctionBase.cpp` & `MParT-2.0.1/src/ParameterizedFunctionBase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 }
 
 #endif
 
 
 
 template<typename MemorySpace>
-void ParameterizedFunctionBase<MemorySpace>::SetCoeffs(Kokkos::View<double*, MemorySpace> coeffs){
+void ParameterizedFunctionBase<MemorySpace>::SetCoeffs(Kokkos::View<const double*, MemorySpace> coeffs){
 
     // If coefficients already exist, make sure the sizes match
     if(this->savedCoeffs.is_allocated()){
         if(coeffs.size() != numCoeffs){
             std::stringstream msg;
             msg << "Error in ParameterizedFunctionBase<MemorySpace>::SetCoeffs.  Expected coefficient vector with size " << numCoeffs << ", but new coefficients have size " << coeffs.size() << ".";
             throw std::invalid_argument(msg.str());
@@ -215,15 +215,15 @@
     }
     this->savedCoeffs = coeffs;
 }
 
 #if defined(MPART_ENABLE_GPU)
 
 template<>
-void ParameterizedFunctionBase<mpart::DeviceSpace>::SetCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs)
+void ParameterizedFunctionBase<mpart::DeviceSpace>::SetCoeffs(Kokkos::View<const double*, Kokkos::HostSpace> coeffs)
 {
     // Copy the coefficients to the device
     Kokkos::View<double*, mpart::DeviceSpace> coeffs_device = ToDevice<mpart::DeviceSpace>(coeffs);
     this->SetCoeffs(coeffs_device);
 }
```

### Comparing `MParT-1.4.4/src/SummarizedMap.cpp` & `MParT-2.0.1/src/SummarizedMap.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -23,34 +23,34 @@
         msg << "SummarizedMap: input dimension of map component must be 1 + output dimension of sumFunc_, but was given map->inputDim = " << comp_->inputDim << " and sumFunc_->outputDim + 1 = " << sumFunc_->outputDim + 1 << ".";
         throw std::invalid_argument(msg.str());
     }
 
 }
 
 template<typename MemorySpace>
-void SummarizedMap<MemorySpace>::SetCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs)
+void SummarizedMap<MemorySpace>::SetCoeffs(Kokkos::View<const double*, Kokkos::HostSpace> coeffs)
 {
     // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::SetCoeffs(coeffs);
-    comp_->WrapCoeffs(coeffs);
+    comp_->WrapCoeffs(this->savedCoeffs);
 }
 
 template<typename MemorySpace>
 void SummarizedMap<MemorySpace>::WrapCoeffs(Kokkos::View<double*, Kokkos::HostSpace> coeffs)
 {
 
     // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::WrapCoeffs(coeffs);
     comp_->WrapCoeffs(coeffs);
 
 }
 
 #if defined(MPART_ENABLE_GPU)
 template<typename MemorySpace>
-void SummarizedMap<MemorySpace>::SetCoeffs(Kokkos::View<double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs)
+void SummarizedMap<MemorySpace>::SetCoeffs(Kokkos::View<const double*, Kokkos::DefaultExecutionSpace::memory_space> coeffs)
 {
 
         // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::SetCoeffs(coeffs);
     comp_->WrapCoeffs(coeffs);
 
 }
@@ -74,15 +74,15 @@
 
     StridedMatrix<const double, MemorySpace> ptsToSummarize = Kokkos::subview(pts, std::make_pair(0, int(sumFunc_->inputDim)), Kokkos::ALL());
     StridedMatrix<const double, MemorySpace> ptsAfterSummary = Kokkos::subview(pts, std::make_pair(int(sumFunc_->inputDim), int(sumFunc_->inputDim+1)), Kokkos::ALL());
 
 
     // Copy summarized pts
     Kokkos::View<double**, MemorySpace> outputSummary = Kokkos::subview(output, std::make_pair(0,int(sumFunc_->outputDim)), Kokkos::ALL());
-    
+
     // Evaluate summary function
     sumFunc_->EvaluateImpl(ptsToSummarize, outputSummary);
 
     // Copy non summarized pts
     Kokkos::View<double**, MemorySpace> outputAfterSummary = Kokkos::subview(output, std::make_pair(int(sumFunc_->outputDim),int(sumFunc_->outputDim+1)), Kokkos::ALL());
     Kokkos::deep_copy(outputAfterSummary, ptsAfterSummary);
 
@@ -158,15 +158,15 @@
 
     // Split outputForSummaryAndX2 into summary and x2 parts
     Kokkos::View<double**, MemorySpace> outputForSummary = Kokkos::subview(outputForSummaryAndX2, std::make_pair(0,int(sumFunc_->outputDim)), Kokkos::ALL());
     Kokkos::View<double**, MemorySpace> outputForX2 = Kokkos::subview(outputForSummaryAndX2, std::make_pair(int(sumFunc_->outputDim),int(sumFunc_->outputDim+1)), Kokkos::ALL());
 
     // GradientImpl of summary using outputForSummary as the sens. vectors (from chain-rule)
     StridedMatrix<const double, MemorySpace>  x1 = Kokkos::subview(pts, std::make_pair(0,int(sumFunc_->inputDim)), Kokkos::ALL());
-    
+
     // Copy results over to the output
     Kokkos::View<double**, MemorySpace> outputSubX1 = Kokkos::subview(output, std::make_pair(0,int(sumFunc_->inputDim)), Kokkos::ALL());
     sumFunc_->GradientImpl(x1, outputForSummary, outputSubX1);
 
     Kokkos::View<double**, MemorySpace> outputSubX2 = Kokkos::subview(output, std::make_pair(int(sumFunc_->inputDim),int(sumFunc_->inputDim+1)), Kokkos::ALL());
     Kokkos::deep_copy(outputSubX2, outputForX2);
```

### Comparing `MParT-1.4.4/src/TriangularMap.cpp` & `MParT-2.0.1/src/TriangularMap.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 template<typename MemorySpace>
 TriangularMap<MemorySpace>::TriangularMap(std::vector<std::shared_ptr<ConditionalMapBase<MemorySpace>>> const& components, bool moveCoeffs) : ConditionalMapBase<MemorySpace>(components.back()->inputDim,
                         std::accumulate(components.begin(), components.end(), 0, [](size_t sum, std::shared_ptr<ConditionalMapBase<MemorySpace>> const& comp){ return sum + comp->outputDim; }),
                         std::accumulate(components.begin(), components.end(), 0, [](size_t sum, std::shared_ptr<ConditionalMapBase<MemorySpace>> const& comp){ return sum + comp->numCoeffs; })),
                         comps_(components)
 {
-    
+
 
     // Check the sizes of all the inputs
-    
+
     for(unsigned int i=0; i<comps_.size(); ++i){
         if(comps_.at(i)->outputDim > comps_.at(i)->inputDim){
             std::stringstream msg;
             msg << "In TriangularMap constructor, the output dimension (" << comps_.at(i)->outputDim << ") of component " << i << " is greater than the input dimension (" << comps_.at(i)->inputDim << ").";
             throw std::invalid_argument(msg.str());
         }
 
@@ -38,15 +38,15 @@
 
 
     // if moveCoeffs is set to true, we check if each component's coeffs are set, and then copy them into the new triangular map's coeffs
     if(moveCoeffs){
 
         Kokkos::View<double*,MemorySpace> coeffs("coeffs", this->numCoeffs);
         unsigned int cumNumCoeffs = 0;
-        
+
         for(unsigned int i=0; i<comps_.size(); ++i){
 
             if(!comps_.at(i)->CheckCoefficients()){
                 std::stringstream msg;
                 msg << "In TriangularMap constructor, moveCoeffs set to true, but component " << i <<" doesn't have coeffs set";
                 throw std::invalid_argument(msg.str());
             }
@@ -59,15 +59,15 @@
         this->WrapCoeffs(coeffs);
     }
 }
 
 
 
 template<typename MemorySpace>
-void TriangularMap<MemorySpace>::SetCoeffs(Kokkos::View<double*, MemorySpace> coeffs)
+void TriangularMap<MemorySpace>::SetCoeffs(Kokkos::View<const double*, MemorySpace> coeffs)
 {
     // First, call the ConditionalMapBase version of this function to copy the view into the savedCoeffs member variable
     ConditionalMapBase<MemorySpace>::SetCoeffs(coeffs);
 
     // Now create subviews for each of the components
     unsigned int cumNumCoeffs = 0;
     for(unsigned int i=0; i<comps_.size(); ++i){
@@ -241,15 +241,15 @@
 
             subPts = Kokkos::subview(pts, std::make_pair(0,int(comps_.at(i)->inputDim)), Kokkos::ALL());
             subSens = Kokkos::subview(sens, std::make_pair(startOutDim,int(startOutDim+comps_.at(i)->outputDim)), Kokkos::ALL());
 
             subOut = Kokkos::subview(output, std::make_pair(startParamDim,int(startParamDim+comps_.at(i)->numCoeffs)), Kokkos::ALL());
             comps_.at(i)->CoeffGradImpl(subPts, subSens, subOut);
 
-            
+
             startParamDim += comps_.at(i)->numCoeffs;
         }
 
         startOutDim += comps_.at(i)->outputDim;
     }
 }
```

### Comparing `MParT-1.4.4/src/Utilities/LinearAlgebra.cpp` & `MParT-2.0.1/src/Utilities/LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/src/Utilities/Miscellaneous.cpp` & `MParT-2.0.1/src/Utilities/Miscellaneous.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/CMakeLists.txt` & `MParT-2.0.1/tests/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 
+set (MPART_SERIALIZE_TESTS "")
+set (MPART_OPT_TESTS "")
 if (MPART_ARCHIVE)
-     set (SERIALIZE_FILES tests/Test_Serialization.cpp)
-else()
-     set (SERIALIZE_FILES "")
+     set (MPART_SERIALIZE_TESTS tests/Test_Serialization.cpp)
+endif ()
+if (MPART_OPT)
+     set (MPART_OPT_TESTS
+          tests/Test_MapObjective.cpp
+          tests/Test_TrainMap.cpp
+          tests/Test_TrainMapAdaptive.cpp
+     )
 endif ()
 
 set (TEST_SOURCES
      tests/RunTests.cpp
 
      # MultiIndex tests
      tests/MultiIndices/Test_MultiIndex.cpp
      tests/MultiIndices/Test_MultiIndexSet.cpp
 
      # Distributions tests
+     tests/Distributions/Test_Distributions_Common.cpp
      tests/Distributions/Test_DensityBase.cpp
      tests/Distributions/Test_SampleGenerator.cpp
      tests/Distributions/Test_Distribution.cpp
      tests/Distributions/Test_GaussianDistribution.cpp
+     tests/Distributions/Test_TransportDensity.cpp
+     tests/Distributions/Test_TransportSampler.cpp
 
      tests/Test_OrthogonalPolynomials.cpp
      tests/Test_HermiteFunctions.cpp
      tests/Test_PositiveBijectors.cpp
      tests/Test_Quadrature.cpp
      tests/Test_MonotoneComponent.cpp
      tests/Test_MultivariateExpansion.cpp
@@ -34,9 +44,10 @@
      tests/Test_AffineMap.cpp
      tests/Test_LinearAlgebra.cpp
      tests/Test_AffineFunction.cpp
      tests/Test_IdentityMap.cpp
      tests/Test_SummarizedMap.cpp
      #tests/Test_TensorProductFunction.cpp
 
-     ${SERIALIZE_FILES}
+     ${MPART_SERIALIZE_TESTS}
+     ${MPART_OPT_TESTS}
 PARENT_SCOPE)
```

### Comparing `MParT-1.4.4/tests/Distributions/Test_DensityBase.cpp` & `MParT-2.0.1/tests/Distributions/Test_DensityBase.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,23 @@
                 REQUIRE(output_eigen(j) == Approx(-2.0));
             } else {
                 REQUIRE(output_eigen(j) == Approx(-std::numeric_limits<double>::infinity()));
             }
         }
     }
 
-    SECTION("GradLogDensityKokkos") {
+    SECTION("LogDensityInputGradKokkos") {
         auto output = density->LogDensityInputGrad(ptsConst);
         for(unsigned int j = 0; j < N_pts; ++j) {
             REQUIRE(output(0,j) == Approx(0.));
             REQUIRE(output(1,j) == Approx(0.));
         }
     }
 
-    SECTION("GradLogDensityEigen") {
+    SECTION("LogDensityInputGradEigen") {
         auto output_eigen = density->LogDensityInputGrad(pts_eigen);
         for(unsigned int j = 0; j < N_pts; ++j) {
             REQUIRE(output_eigen(0,j) == Approx(0.));
             REQUIRE(output_eigen(1,j) == Approx(0.));
         }
     }
 }
```

### Comparing `MParT-1.4.4/tests/Distributions/Test_Distribution.cpp` & `MParT-2.0.1/tests/Distributions/Test_Distribution.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Distributions/Test_Distributions_Common.h` & `MParT-2.0.1/tests/Distributions/Test_Distributions_Common.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
+#ifndef TEST_DISTRIBUTIONS_COMMON_H
+#define TEST_DISTRIBUTIONS_COMMON_H
+
 #include<algorithm>
 #include <catch2/catch_all.hpp>
 #include "MParT/Utilities/ArrayConversions.h"
 #include "MParT/Distributions/DensityBase.h"
 #include "MParT/Distributions/SampleGenerator.h"
+#include "MParT/Distributions/GaussianSamplerDensity.h"
 #include "MParT/Distributions/Distribution.h"
 
 using namespace mpart;
 using namespace Catch;
 
 // Uniform generator on [0,e]^N
 // TODO: Test on GPU
 template<typename MemorySpace>
 class UniformSampler: public SampleGenerator<MemorySpace> {
 public:
 // Set a given seed for this test
-UniformSampler(int dim): SampleGenerator<MemorySpace>(dim, 160258) {}
+UniformSampler(int dim, double scale = std::exp(1.)): SampleGenerator<MemorySpace>(dim, seed), scale_(scale) {}
 
 void SampleImpl(StridedMatrix<double, MemorySpace> output) {
-    double euler = std::exp(1.);
     Kokkos::MDRangePolicy<Kokkos::Rank<2>,typename MemoryToExecution<MemorySpace>::Space> policy({0, 0}, {output.extent(0), output.extent(1)});
     Kokkos::parallel_for(policy, KOKKOS_LAMBDA(int i, int j) {
         auto rgen = this->rand_pool.get_state();
-        output(i,j) = euler*rgen.drand();
+        output(i,j) = scale_*rgen.drand();
         this->rand_pool.free_state(rgen);
     });
 }
+private:
+static const unsigned int seed = 160258;
+const double scale_;
 };
 
 // Uniform density on [0,e]^2
 template <typename MemorySpace>
 class UniformDensity : public DensityBase<MemorySpace> {
 public:
 UniformDensity(int dim): DensityBase<MemorySpace>(dim) {}
@@ -45,8 +51,13 @@
 void LogDensityInputGradImpl(StridedMatrix<const double, MemorySpace> const &pts, StridedMatrix<double, MemorySpace> output) override {
     unsigned int N = pts.extent(1);
     Kokkos::parallel_for( "uniform grad log density", N, KOKKOS_LAMBDA (const int& j) {
         output(0,j) = 0.;
         output(1,j) = 0.;
     });
 }
-};
+};
+
+// Tests samples that should be transformed to a standard normal distribution
+void TestStandardNormalSamples(StridedMatrix<double, Kokkos::HostSpace> samples);
+
+#endif //MPART_TEST_DISTRIBUTIONS_COMMON_H
```

### Comparing `MParT-1.4.4/tests/Distributions/Test_SampleGenerator.cpp` & `MParT-2.0.1/tests/Distributions/Test_SampleGenerator.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/MultiIndices/Test_MultiIndex.cpp` & `MParT-2.0.1/tests/MultiIndices/Test_MultiIndex.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -117,20 +117,26 @@
     MultiIndex b({1,0,0,0});
 
     REQUIRE( b<a );
     REQUIRE( a>b );
     REQUIRE( b<=a );
     REQUIRE( a>=b );
     REQUIRE( b!=a );
+    REQUIRE( a.AnyBounded(b) );
+    REQUIRE( b.AnyBounded(a) );
 
     b = MultiIndex({0,1,1,2});
     REQUIRE( b==a );
     REQUIRE( b<=a );
     REQUIRE( a>=b );
 
     b = MultiIndex({1,2,1,0});
     REQUIRE( a<b );
     REQUIRE( a<=b );
     REQUIRE( b>a );
     REQUIRE( b>=a );
     REQUIRE( a!=b );
+
+    b = MultiIndex({2,2,2,3});
+    REQUIRE( !a.AnyBounded(b) );
+    REQUIRE(  b.AnyBounded(a) );
 }
```

### Comparing `MParT-1.4.4/tests/MultiIndices/Test_MultiIndexSet.cpp` & `MParT-2.0.1/tests/MultiIndices/Test_MultiIndexSet.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -352,14 +352,24 @@
         REQUIRE( (oldSize+1) == indexFamily.Size());
 
         // Create MultiIndex for testing against the square.
         MultiIndex multi{3,0};
 
         // Check the result of IsAdmissable().
         REQUIRE( indexFamily.IsAdmissible(multi));
+
+        // Check to make sure https://github.com/MeasureTransport/MParT/issues/308 is resolved
+        indexFamily = MultiIndexSet(2);
+        indexFamily += MultiIndex{0,0};
+        indexFamily += MultiIndex{1,0};
+        indexFamily.Expand();
+        
+        REQUIRE( indexFamily.IsActive(MultiIndex{2,0}) );
+        REQUIRE( indexFamily.IsActive(MultiIndex{0,1}) );
+        REQUIRE(! indexFamily.IsActive(MultiIndex{1,1}) );   
     }
 
     /*
         We start with a multiindex set that looks like
         4 | 0
         3 | x
         2 | x
```

### Comparing `MParT-1.4.4/tests/RunTests.cpp` & `MParT-2.0.1/tests/RunTests.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   // Build a new parser on top of Catch2's
   using namespace Catch::Clara;
   auto cli
     = session.cli() | Opt( cores, "kokkos-thread" ) ["--kokkos-threads"]("Number of cores to use with Kokkos.");
 
   // Now pass the new composite back to Catch2 so it uses that
   session.cli( cli );
-  
+
   // Let Catch2 (using Clara) parse the command line
   int returnCode = session.applyCommandLine( argc, argv );
   if( returnCode != 0 ) // Indicates a command line error
       return returnCode;
 
   session.run();
 }
```

### Comparing `MParT-1.4.4/tests/Test_AffineFunction.cpp` & `MParT-2.0.1/tests/Test_AffineFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_AffineMap.cpp` & `MParT-2.0.1/tests/Test_AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_ArrayConversions.cpp` & `MParT-2.0.1/tests/Test_ArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_ComposedMap.cpp` & `MParT-2.0.1/tests/Test_ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_ConditionalMapBase.cpp` & `MParT-2.0.1/tests/Test_ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_HermiteFunctions.cpp` & `MParT-2.0.1/tests/Test_HermiteFunctions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_IdentityMap.cpp` & `MParT-2.0.1/tests/Test_IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_LinearAlgebra.cpp` & `MParT-2.0.1/tests/Test_LinearAlgebra.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -135,14 +135,55 @@
             for(unsigned int i=0; i<C.extent(0); ++i){
                 CHECK(C(i,j) == Approx(trueC(i,j)).epsilon(1e-14).margin(1e-14));
             }
         }
     }
 }
 
+TEST_CASE( "Testing ReduceDim", "ReduceDim" ) {
+    int N = 23;
+    StridedMatrix<double, Kokkos::HostSpace> A = Kokkos::View<double**, Kokkos::HostSpace>("A", 3, N);
+    StridedMatrix<double, Kokkos::HostSpace> AT = Kokkos::View<double**, Kokkos::HostSpace>("AT", N, 3);
+    double ref_avg = ((double) (N+1)) / 2.0;
+    for(int i = 0; i < N; i++) {
+        A(0,i) = i+1;
+        A(1,i) = N-i;
+        A(2,i) = ref_avg;
+
+        AT(i,0) = i+1;
+        AT(i,1) = N-i;
+        AT(i,2) = ref_avg;
+    }
+    ReduceDim<ReduceDimMap::sum,Kokkos::HostSpace,1> rc (A, 1.0);
+    Kokkos::View<double*, Kokkos::HostSpace> avg_col("avg_col", 3);
+    Kokkos::parallel_reduce(N, rc, avg_col.data());
+    CHECK(avg_col(0) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_col(1) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_col(2) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+    
+    ReduceDim<ReduceDimMap::sum,Kokkos::HostSpace,0> rr (AT,1.0);
+    Kokkos::View<double*, Kokkos::HostSpace> avg_row("avg_row", 3);
+    Kokkos::parallel_reduce(N, rr, avg_row.data());
+    CHECK(avg_row(0) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_row(1) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_row(2) == Approx(N*ref_avg).epsilon(1e-14).margin(1e-14));
+
+    rc = ReduceDim<ReduceDimMap::sum,Kokkos::HostSpace>(A, -1.0/((double) N));
+    Kokkos::parallel_reduce(N, rc, avg_col.data());
+    CHECK(avg_col(0) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_col(1) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_col(2) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+    
+    rr = ReduceDim<ReduceDimMap::sum,Kokkos::HostSpace,0>(AT, -1.0/((double) N));
+    Kokkos::parallel_reduce(N, rr, avg_row.data());
+    CHECK(avg_row(0) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_row(1) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+    CHECK(avg_row(2) == Approx(-ref_avg).epsilon(1e-14).margin(1e-14));
+}
+
 TEST_CASE( "Testing LU Factorization", "LinearAlgebra_LU" ) {
     Kokkos::View<double**, Kokkos::LayoutLeft, Kokkos::HostSpace> A("A", 3, 3);
     Kokkos::View<double**, Kokkos::LayoutLeft, Kokkos::HostSpace> B("B", 3, 2);
     A(0,0) = 1.; A(0,1) = 2.; A(0,2) = 3.;
     A(1,0) = 4.; A(1,1) = 5.; A(1,2) = 6.;
     A(2,0) = 7.; A(2,1) = 8.; A(2,2) = 0.;
```

### Comparing `MParT-1.4.4/tests/Test_LinearizedBasis.cpp` & `MParT-2.0.1/tests/Test_LinearizedBasis.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_MapFactory.cpp` & `MParT-2.0.1/tests/Test_MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_MonotoneComponent.cpp` & `MParT-2.0.1/tests/Test_MonotoneComponent.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_MultivariateExpansion.cpp` & `MParT-2.0.1/tests/Test_MultivariateExpansion.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_MultivariateExpansionWorker.cpp` & `MParT-2.0.1/tests/Test_MultivariateExpansionWorker.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_OrthogonalPolynomials.cpp` & `MParT-2.0.1/tests/Test_OrthogonalPolynomials.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_PositiveBijectors.cpp` & `MParT-2.0.1/tests/Test_PositiveBijectors.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_Quadrature.cpp` & `MParT-2.0.1/tests/Test_Quadrature.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_Serialization.cpp` & `MParT-2.0.1/tests/Test_Serialization.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_SummarizedMap.cpp` & `MParT-2.0.1/tests/Test_SummarizedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_TensorProductFunction.cpp` & `MParT-2.0.1/tests/Test_TensorProductFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-1.4.4/tests/Test_TriangularMap.cpp` & `MParT-2.0.1/tests/Test_TriangularMap.cpp`

 * *Files identical despite different names*

