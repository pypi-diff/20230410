# Comparing `tmp/MParT-2.0.1.tar.gz` & `tmp/MParT-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MParT-2.0.1.tar", last modified: Fri Apr  7 17:58:29 2023, max compression
+gzip compressed data, was "MParT-2.0.2.tar", last modified: Mon Apr 10 18:25:34 2023, max compression
```

## Comparing `MParT-2.0.1.tar` & `MParT-2.0.2.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.docker/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-07 17:58:17.000000 MParT-2.0.1/.docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-07 17:58:17.000000 MParT-2.0.1/.docker/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-07 17:58:17.000000 MParT-2.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/install-doxygen.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.572093 MParT-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-bindings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-external-lib-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-push-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/build-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-07 17:58:17.000000 MParT-2.0.1/.github/workflows/pypi-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 17:58:17.000000 MParT-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-07 17:58:17.000000 MParT-2.0.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-04-07 17:58:17.000000 MParT-2.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-07 17:58:17.000000 MParT-2.0.1/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-07 17:58:17.000000 MParT-2.0.1/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.580093 MParT-2.0.1/MParT/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/AffineFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/AffineMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ComposedMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ConditionalMapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/DerivativeFlags.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.584093 MParT-2.0.1/MParT/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/DensityBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/Distribution.h
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/GaussianSamplerDensity.h
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PullbackDensity.h
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PullbackSampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PushforwardDensity.h
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/PushforwardSampler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/SampleGenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Distributions/TransportDistributionFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/HermiteFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/IdentityMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Initialization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/LinearizedBasis.h
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapObjective.h
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MapOptions.h
--rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MonotoneComponent.h
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MonotoneIntegrand.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.584093 MParT-2.0.1/MParT/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/FixedMultiIndexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndex.h
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexLimiter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexNeighborhood.h
--rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultiIndices/MultiIndexSet.h
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultivariateExpansion.h
--rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/MultivariateExpansionWorker.h
--rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/OrthogonalPolynomial.h
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/ParameterizedFunctionBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/PositiveBijectors.h
--rw-r--r--   0 runner    (1001) docker     (123)    43493 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Quadrature.h
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/SummarizedMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TensorProductFunction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TrainMap.h
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TrainMapAdaptive.h
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/TriangularMap.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/MParT/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/ArrayConversions.h
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/EigenTypes.h
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/GPUtils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/KokkosHelpers.h
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/KokkosSpaceMappings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/LinearAlgebra.h
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/Miscellaneous.h
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-07 17:58:17.000000 MParT-2.0.1/MParT/Utilities/Serialization.h
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 17:58:29.652094 MParT-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-07 17:58:17.000000 MParT-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.564093 MParT-2.0.1/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.564093 MParT-2.0.1/bindings/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/common/include/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/common/include/CommonUtilities.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/common/src/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/common/src/CommonUtilities.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.588093 MParT-2.0.1/bindings/julia/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.592093 MParT-2.0.1/bindings/julia/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/include/CommonJuliaUtilities.h
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/include/JlArrayConversions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.592093 MParT-2.0.1/bindings/julia/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/CommonJuliaUtilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/JlArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapObjective.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MapOptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TrainMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TrainMapAdaptive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/TriangularMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/julia/src/Wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/mexplus/
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14160 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/arguments.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/dispatch.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxarray.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11613 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxtypes.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus/mexplus.h
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/external/mexplus_eigen.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.596093 MParT-2.0.1/bindings/matlab/include/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexArrayConversions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexOptionsConversions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/include/MexWrapperTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.600093 MParT-2.0.1/bindings/matlab/mat/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ATMOptions.m
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/AdaptiveTransportMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/AffineMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ComposedMap.m
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ConditionalMap.m
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/CreateComponent.m
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/CreateTriangular.m
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/DeserializeMap.m
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/FixedMultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/GaussianKLObjective.m
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/KokkosInitialize.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.604093 MParT-2.0.1/bindings/matlab/mat/MapOptions/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/BasisTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/MapOptions.m
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/PosFuncTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MapOptions/QuadTypes.m
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MultiIndex.m
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/MultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/ParameterizedFunction.m
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TrainMap.m
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TrainOptions.m
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/mat/TriangularMap.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.604093 MParT-2.0.1/bindings/matlab/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/BasisTypes_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/ConditionalMap_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/FixedMultiIndexSet_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/KokkosUtilities_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MapObjective_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MexArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MexOptionsConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MultiIndexSet_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/MultiIndex_mex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/matlab/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/FixedMultiIndexSetTest.m
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_AffineMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_ComposedMap.m
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_MultiIndex.m
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_MultiIndexSet.m
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_ParameterizedFunction.m
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/Test_TriangularMap.m
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/TrainMapAdaptiveTest.m
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/TrainMapTest.m
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/matlab/tests/runtests.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/include/CommonPybindUtilities.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/package/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.608093 MParT-2.0.1/bindings/python/package/MParT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 17:58:29.000000 MParT-2.0.1/bindings/python/package/MParT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.612093 MParT-2.0.1/bindings/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/CommonPybindUtilities.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapObjective.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MapOptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/Serialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TrainMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TrainMapAdaptive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/TriangularMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/src/Wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.616093 MParT-2.0.1/bindings/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_AffineFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_AffineMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ComposedMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ComposedMap_moveCoeffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_ConditionalMapBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_IdentityMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MapFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MultiIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_MultiIndexSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_Serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_SummarizedMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TrainMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TrainMapAdaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TriangularMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-07 17:58:17.000000 MParT-2.0.1/bindings/python/tests/test_TriangularMap_moveCoeffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.616093 MParT-2.0.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/BuildDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/FindJulia.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/FindSphinx.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 17:58:17.000000 MParT-2.0.1/cmake/SetInstallPaths.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.568093 MParT-2.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/_static/pics/
--rw-r--r--   0 runner    (1001) docker     (123)    44355 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Density.png
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Regression.png
--rw-r--r--   0 runner    (1001) docker     (123)   426141 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Samples.png
--rw-r--r--   0 runner    (1001) docker     (123)   123355 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/_static/pics/Transformation2d.png
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)   114543 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/mpart.doxyfile.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.620093 MParT-2.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.624093 MParT-2.0.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/composedmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.624093 MParT-2.0.1/docs/source/api/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/concepts/cachedparameterization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/concepts/parameterizedfunction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/conditionalmapbase.rst
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/mapfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/monotonecomponent.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/multiindices/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/fixedmultiindexset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexlimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexneighborhood.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multiindices/multiindexset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multivariateexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/multivariateexpansionworker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/parameterizedfunctionbase.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/adaptivesimpson.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/clenshawcurtis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature/recursivequadrature.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/quadrature.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/templateconcepts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/tensorproductfunction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/triangularmap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/api/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/initialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/kokkoswrappers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/linearalgebra.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/api/utilities/serialization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/mathematics.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-07 17:58:17.000000 MParT-2.0.1/docs/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.628093 MParT-2.0.1/joss/
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)   922955 2023-04-07 17:58:17.000000 MParT-2.0.1/joss/performance_comparison.png
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-07 17:58:17.000000 MParT-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 17:58:29.652094 MParT-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-07 17:58:17.000000 MParT-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-07 17:58:17.000000 MParT-2.0.1/src/AffineFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-07 17:58:17.000000 MParT-2.0.1/src/AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-07 17:58:17.000000 MParT-2.0.1/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ConditionalMapBase.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/DensityBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/GaussianSamplerDensity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Distributions/PullbackDensity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-07 17:58:17.000000 MParT-2.0.1/src/IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Initialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl10.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl11.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl12.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl13.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl14.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl15.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl16.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl17.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl18.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl6.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl7.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl8.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapFactoryImpl9.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MapObjective.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.640093 MParT-2.0.1/src/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/FixedMultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexLimiter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexNeighborhood.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-07 17:58:17.000000 MParT-2.0.1/src/MultiIndices/MultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-07 17:58:17.000000 MParT-2.0.1/src/ParameterizedFunctionBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-07 17:58:17.000000 MParT-2.0.1/src/SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TrainMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TrainMapAdaptive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-07 17:58:17.000000 MParT-2.0.1/src/TriangularMap.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.644093 MParT-2.0.1/src/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Utilities/LinearAlgebra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-07 17:58:17.000000 MParT-2.0.1/src/Utilities/Miscellaneous.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.648093 MParT-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/tests/Distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_DensityBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distribution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distributions_Common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_Distributions_Common.h
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_GaussianDistribution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_SampleGenerator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportDensity.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportDistributionFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Distributions/Test_TransportSampler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/KokkosInfo.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:58:29.652094 MParT-2.0.1/tests/MultiIndices/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/MultiIndices/Test_MultiIndex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/MultiIndices/Test_MultiIndexSet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/RunTests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_AffineFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_AffineMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ArrayConversions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32651 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ComposedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_ConditionalMapBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_HermiteFunctions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_IdentityMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_LinearAlgebra.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_LinearizedBasis.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MapFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MapObjective.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MonotoneComponent.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MultivariateExpansion.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_MultivariateExpansionWorker.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_OrthogonalPolynomials.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_PositiveBijectors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_Quadrature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_Serialization.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_SummarizedMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TensorProductFunction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TrainMap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TrainMapAdaptive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    39093 2023-04-07 17:58:17.000000 MParT-2.0.1/tests/Test_TriangularMap.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.329967 MParT-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.281964 MParT-2.0.2/.docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-10 18:25:23.000000 MParT-2.0.2/.docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 18:25:23.000000 MParT-2.0.2/.docker/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-10 18:25:23.000000 MParT-2.0.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.281964 MParT-2.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/install-doxygen.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.285965 MParT-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/build-bindings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/build-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/build-external-lib-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/build-push-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/build-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-10 18:25:23.000000 MParT-2.0.2/.github/workflows/pypi-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 18:25:23.000000 MParT-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-10 18:25:23.000000 MParT-2.0.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-04-10 18:25:23.000000 MParT-2.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-10 18:25:23.000000 MParT-2.0.2/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 18:25:23.000000 MParT-2.0.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.289965 MParT-2.0.2/MParT/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/AffineFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/AffineMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/ComposedMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/ConditionalMapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/DerivativeFlags.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.289965 MParT-2.0.2/MParT/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/DensityBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/Distribution.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/GaussianSamplerDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/PullbackDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/PullbackSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/PushforwardDensity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/PushforwardSampler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/SampleGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Distributions/TransportDistributionFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/HermiteFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/IdentityMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Initialization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/LinearizedBasis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MapFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MapObjective.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MapOptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MonotoneComponent.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MonotoneIntegrand.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/MParT/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultiIndices/FixedMultiIndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultiIndices/MultiIndex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultiIndices/MultiIndexLimiter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultiIndices/MultiIndexNeighborhood.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultiIndices/MultiIndexSet.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultivariateExpansion.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/MultivariateExpansionWorker.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/OrthogonalPolynomial.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/ParameterizedFunctionBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/PositiveBijectors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    43493 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Quadrature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/SummarizedMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/TensorProductFunction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/TrainMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/TrainMapAdaptive.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/TriangularMap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/MParT/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    33316 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/ArrayConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/EigenTypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/GPUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/KokkosHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/KokkosSpaceMappings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/LinearAlgebra.h
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/Miscellaneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-10 18:25:23.000000 MParT-2.0.2/MParT/Utilities/Serialization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-10 18:25:34.329967 MParT-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-10 18:25:23.000000 MParT-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.277964 MParT-2.0.2/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.277964 MParT-2.0.2/bindings/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/bindings/common/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/common/include/CommonUtilities.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/bindings/common/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/common/src/CommonUtilities.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/bindings/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.293965 MParT-2.0.2/bindings/julia/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/include/CommonJuliaUtilities.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/include/JlArrayConversions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/julia/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/CommonJuliaUtilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/JlArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/MapOptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/TriangularMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/julia/src/Wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/matlab/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/matlab/external/mexplus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14160 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/arguments.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/dispatch.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/mxarray.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11613 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/mxtypes.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus/mexplus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/external/mexplus_eigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.297965 MParT-2.0.2/bindings/matlab/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/include/MexArrayConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/include/MexOptionsConversions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/include/MexWrapperTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.301965 MParT-2.0.2/bindings/matlab/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/ATMOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/AdaptiveTransportMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/AffineMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/ComposedMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/ConditionalMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/CreateComponent.m
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/CreateTriangular.m
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/DeserializeMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/FixedMultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/GaussianKLObjective.m
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/KokkosInitialize.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.301965 MParT-2.0.2/bindings/matlab/mat/MapOptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MapOptions/BasisTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MapOptions/MapOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MapOptions/PosFuncTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MapOptions/QuadTypes.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MultiIndex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/MultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/ParameterizedFunction.m
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/TrainMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/TrainOptions.m
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/mat/TriangularMap.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.301965 MParT-2.0.2/bindings/matlab/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/BasisTypes_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/ConditionalMap_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/FixedMultiIndexSet_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/KokkosUtilities_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/MapObjective_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/MexArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/MexOptionsConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/MultiIndexSet_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/MultiIndex_mex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/matlab/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/FixedMultiIndexSetTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_AffineMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_ComposedMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_MultiIndex.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_MultiIndexSet.m
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_ParameterizedFunction.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/Test_TriangularMap.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/TrainMapAdaptiveTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/TrainMapTest.m
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/matlab/tests/runtests.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/python/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/include/CommonPybindUtilities.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/python/package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/python/package/MParT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-10 18:25:34.000000 MParT-2.0.2/bindings/python/package/MParT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-04-10 18:25:34.000000 MParT-2.0.2/bindings/python/package/MParT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:25:34.000000 MParT-2.0.2/bindings/python/package/MParT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:25:34.000000 MParT-2.0.2/bindings/python/package/MParT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.305966 MParT-2.0.2/bindings/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/CommonPybindUtilities.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/MapOptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/Serialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/TriangularMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/src/Wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.309966 MParT-2.0.2/bindings/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_AffineFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_AffineMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_ComposedMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_ComposedMap_moveCoeffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_ConditionalMapBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_IdentityMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_MapFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_MultiIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_MultiIndexSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_Serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_SummarizedMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_TrainMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_TrainMapAdaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_TriangularMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-10 18:25:23.000000 MParT-2.0.2/bindings/python/tests/test_TriangularMap_moveCoeffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.309966 MParT-2.0.2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-10 18:25:23.000000 MParT-2.0.2/cmake/BuildDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-10 18:25:23.000000 MParT-2.0.2/cmake/FindJulia.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-10 18:25:23.000000 MParT-2.0.2/cmake/FindSphinx.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-10 18:25:23.000000 MParT-2.0.2/cmake/SetInstallPaths.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.309966 MParT-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.281964 MParT-2.0.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.313966 MParT-2.0.2/docs/_static/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)    44355 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/_static/pics/Density.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/_static/pics/Regression.png
+-rw-r--r--   0 runner    (1001) docker     (123)   426141 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/_static/pics/Samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123355 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/_static/pics/Transformation2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)   114543 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/mpart.doxyfile.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.313966 MParT-2.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.313966 MParT-2.0.2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/composedmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.313966 MParT-2.0.2/docs/source/api/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/concepts/cachedparameterization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/concepts/parameterizedfunction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/conditionalmapbase.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/mapfactory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/monotonecomponent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.313966 MParT-2.0.2/docs/source/api/multiindices/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindices/fixedmultiindexset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindices/multiindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindices/multiindexlimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindices/multiindexneighborhood.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multiindices/multiindexset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multivariateexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/multivariateexpansionworker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/parameterizedfunctionbase.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.317966 MParT-2.0.2/docs/source/api/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/quadrature/adaptivesimpson.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/quadrature/clenshawcurtis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/quadrature/recursivequadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/quadrature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/templateconcepts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/tensorproductfunction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/triangularmap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.317966 MParT-2.0.2/docs/source/api/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/utilities/initialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/utilities/kokkoswrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/utilities/linearalgebra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/api/utilities/serialization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.317966 MParT-2.0.2/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/mathematics.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.317966 MParT-2.0.2/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-10 18:25:23.000000 MParT-2.0.2/docs/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.317966 MParT-2.0.2/joss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-10 18:25:23.000000 MParT-2.0.2/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-10 18:25:23.000000 MParT-2.0.2/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)   922955 2023-04-10 18:25:23.000000 MParT-2.0.2/joss/performance_comparison.png
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-10 18:25:23.000000 MParT-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:25:34.329967 MParT-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-10 18:25:23.000000 MParT-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.321967 MParT-2.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-10 18:25:23.000000 MParT-2.0.2/src/AffineFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-10 18:25:23.000000 MParT-2.0.2/src/AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-10 18:25:23.000000 MParT-2.0.2/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19026 2023-04-10 18:25:23.000000 MParT-2.0.2/src/ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-04-10 18:25:23.000000 MParT-2.0.2/src/ConditionalMapBase.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.321967 MParT-2.0.2/src/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Distributions/DensityBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Distributions/GaussianSamplerDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Distributions/PullbackDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-10 18:25:23.000000 MParT-2.0.2/src/IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Initialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl10.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl11.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl12.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl13.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl14.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl15.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl16.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl17.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl18.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl6.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl7.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl8.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapFactoryImpl9.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MapObjective.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.321967 MParT-2.0.2/src/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MultiIndices/FixedMultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MultiIndices/MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MultiIndices/MultiIndexLimiter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MultiIndices/MultiIndexNeighborhood.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-10 18:25:23.000000 MParT-2.0.2/src/MultiIndices/MultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-10 18:25:23.000000 MParT-2.0.2/src/ParameterizedFunctionBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10972 2023-04-10 18:25:23.000000 MParT-2.0.2/src/SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-10 18:25:23.000000 MParT-2.0.2/src/TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-10 18:25:23.000000 MParT-2.0.2/src/TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-10 18:25:23.000000 MParT-2.0.2/src/TriangularMap.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.321967 MParT-2.0.2/src/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    16367 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Utilities/LinearAlgebra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-10 18:25:23.000000 MParT-2.0.2/src/Utilities/Miscellaneous.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.325967 MParT-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.329967 MParT-2.0.2/tests/Distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_DensityBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_Distribution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_Distributions_Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_Distributions_Common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_GaussianDistribution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_SampleGenerator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_TransportDensity.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_TransportDistributionFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Distributions/Test_TransportSampler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/KokkosInfo.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:25:34.329967 MParT-2.0.2/tests/MultiIndices/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/MultiIndices/Test_MultiIndex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/MultiIndices/Test_MultiIndexSet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/RunTests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_AffineFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_AffineMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_ArrayConversions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32651 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_ComposedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_ConditionalMapBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_HermiteFunctions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_IdentityMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_LinearAlgebra.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_LinearizedBasis.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_MapFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_MapObjective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39231 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_MonotoneComponent.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_MultivariateExpansion.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_MultivariateExpansionWorker.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_OrthogonalPolynomials.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_PositiveBijectors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_Quadrature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_Serialization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_SummarizedMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_TensorProductFunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_TrainMap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_TrainMapAdaptive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    39093 2023-04-10 18:25:23.000000 MParT-2.0.2/tests/Test_TriangularMap.cpp
```

### Comparing `MParT-2.0.1/.docker/Dockerfile` & `MParT-2.0.2/.docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/build-bindings.yml` & `MParT-2.0.2/.github/workflows/build-bindings.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/build-doc.yml` & `MParT-2.0.2/.github/workflows/build-doc.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/build-external-lib-tests.yml` & `MParT-2.0.2/.github/workflows/build-external-lib-tests.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/build-push-docker.yml` & `MParT-2.0.2/.github/workflows/build-push-docker.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/build-tests.yml` & `MParT-2.0.2/.github/workflows/build-tests.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/.github/workflows/pypi-deploy.yml` & `MParT-2.0.2/.github/workflows/pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/CITATION.cff` & `MParT-2.0.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/CMakeLists.txt` & `MParT-2.0.2/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.13)
-project(MParT VERSION 2.0.1)
+project(MParT VERSION 2.0.2)
 
 message(STATUS "Will install MParT to ${CMAKE_INSTALL_PREFIX}")
 
 # Add the cmake folder as a search path and include files
 LIST(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake/)
 Include(FetchContent)
 
@@ -49,14 +49,15 @@
 set(CMAKE_CXX_FLAGS_DEBUG "-g")
 set(CMAKE_CXX_FLAGS_RELEASE "-O3")
 
 option(BUILD_SHARED_LIBS "Build using shared libraries" ON)
 
 # #############################################################
 # RPATH settings
+# See https://gist.github.com/kprussing/db21614ca5b51cedff07dfb70059f280 for scikit-build example
 
 # use, i.e. don't skip the full RPATH for the build tree
 set(CMAKE_SKIP_BUILD_RPATH FALSE)
 
 # when building, don't use the install RPATH already
 # (but later on when installing)
 set(CMAKE_BUILD_WITH_INSTALL_RPATH FALSE)
@@ -66,17 +67,17 @@
 # add the automatically determined parts of the RPATH
 # which point to directories outside the build tree to the install RPATH
 set(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # the RPATH to be used when installing, but only if it's not a system directory
 list(FIND CMAKE_PLATFORM_IMPLICIT_LINK_DIRECTORIES "${CMAKE_INSTALL_PREFIX}/lib" isSystemDir)
 
-if("${isSystemDir}" STREQUAL "-1")
-    set(CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/lib")
-endif("${isSystemDir}" STREQUAL "-1")
+# if("${isSystemDir}" STREQUAL "-1")
+#     set(CMAKE_INSTALL_RPATH "${CMAKE_INSTALL_PREFIX}/lib")
+# endif("${isSystemDir}" STREQUAL "-1")
 
 # #############################################################
 # Dependencies
 
 # Add Kokkos
 find_package(Kokkos QUIET)
```

### Comparing `MParT-2.0.1/LICENSE.txt` & `MParT-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/AffineFunction.h` & `MParT-2.0.2/MParT/AffineFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/AffineMap.h` & `MParT-2.0.2/MParT/AffineMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/ComposedMap.h` & `MParT-2.0.2/MParT/ComposedMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/ConditionalMapBase.h` & `MParT-2.0.2/MParT/ConditionalMapBase.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/DerivativeFlags.h` & `MParT-2.0.2/MParT/DerivativeFlags.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/DensityBase.h` & `MParT-2.0.2/MParT/Distributions/DensityBase.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/Distribution.h` & `MParT-2.0.2/MParT/Distributions/Distribution.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/GaussianSamplerDensity.h` & `MParT-2.0.2/MParT/Distributions/GaussianSamplerDensity.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/PullbackDensity.h` & `MParT-2.0.2/MParT/Distributions/PullbackDensity.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/PullbackSampler.h` & `MParT-2.0.2/MParT/Distributions/PullbackSampler.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/PushforwardDensity.h` & `MParT-2.0.2/MParT/Distributions/PushforwardDensity.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/PushforwardSampler.h` & `MParT-2.0.2/MParT/Distributions/PushforwardSampler.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/SampleGenerator.h` & `MParT-2.0.2/MParT/Distributions/SampleGenerator.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Distributions/TransportDistributionFactory.h` & `MParT-2.0.2/MParT/Distributions/TransportDistributionFactory.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/HermiteFunction.h` & `MParT-2.0.2/MParT/HermiteFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/IdentityMap.h` & `MParT-2.0.2/MParT/IdentityMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Initialization.h` & `MParT-2.0.2/MParT/Initialization.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/LinearizedBasis.h` & `MParT-2.0.2/MParT/LinearizedBasis.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MapFactory.h` & `MParT-2.0.2/MParT/MapFactory.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MapObjective.h` & `MParT-2.0.2/MParT/MapObjective.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MapOptions.h` & `MParT-2.0.2/MParT/MapOptions.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MonotoneComponent.h` & `MParT-2.0.2/MParT/MonotoneComponent.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MonotoneIntegrand.h` & `MParT-2.0.2/MParT/MonotoneIntegrand.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultiIndices/FixedMultiIndexSet.h` & `MParT-2.0.2/MParT/MultiIndices/FixedMultiIndexSet.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultiIndices/MultiIndex.h` & `MParT-2.0.2/MParT/MultiIndices/MultiIndex.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultiIndices/MultiIndexLimiter.h` & `MParT-2.0.2/MParT/MultiIndices/MultiIndexLimiter.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultiIndices/MultiIndexNeighborhood.h` & `MParT-2.0.2/MParT/MultiIndices/MultiIndexNeighborhood.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultiIndices/MultiIndexSet.h` & `MParT-2.0.2/MParT/MultiIndices/MultiIndexSet.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultivariateExpansion.h` & `MParT-2.0.2/MParT/MultivariateExpansion.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/MultivariateExpansionWorker.h` & `MParT-2.0.2/MParT/MultivariateExpansionWorker.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/OrthogonalPolynomial.h` & `MParT-2.0.2/MParT/OrthogonalPolynomial.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/ParameterizedFunctionBase.h` & `MParT-2.0.2/MParT/ParameterizedFunctionBase.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/PositiveBijectors.h` & `MParT-2.0.2/MParT/PositiveBijectors.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Quadrature.h` & `MParT-2.0.2/MParT/Quadrature.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/SummarizedMap.h` & `MParT-2.0.2/MParT/SummarizedMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/TensorProductFunction.h` & `MParT-2.0.2/MParT/TensorProductFunction.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/TrainMap.h` & `MParT-2.0.2/MParT/TrainMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/TrainMapAdaptive.h` & `MParT-2.0.2/MParT/TrainMapAdaptive.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/TriangularMap.h` & `MParT-2.0.2/MParT/TriangularMap.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/ArrayConversions.h` & `MParT-2.0.2/MParT/Utilities/ArrayConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/KokkosHelpers.h` & `MParT-2.0.2/MParT/Utilities/KokkosHelpers.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/KokkosSpaceMappings.h` & `MParT-2.0.2/MParT/Utilities/KokkosSpaceMappings.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/LinearAlgebra.h` & `MParT-2.0.2/MParT/Utilities/LinearAlgebra.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/Miscellaneous.h` & `MParT-2.0.2/MParT/Utilities/Miscellaneous.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/MParT/Utilities/Serialization.h` & `MParT-2.0.2/MParT/Utilities/Serialization.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/PKG-INFO` & `MParT-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MParT
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Monotone Parameterization Toolkit
 Author: Matthew Parno
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Massachusetts Institute of Technology
         All rights reserved.
```

### Comparing `MParT-2.0.1/README.md` & `MParT-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/CMakeLists.txt` & `MParT-2.0.2/bindings/julia/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/include/CommonJuliaUtilities.h` & `MParT-2.0.2/bindings/julia/include/CommonJuliaUtilities.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/include/JlArrayConversions.h` & `MParT-2.0.2/bindings/julia/include/JlArrayConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/AffineMap.cpp` & `MParT-2.0.2/bindings/julia/src/AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/CommonJuliaUtilities.cpp` & `MParT-2.0.2/bindings/julia/src/CommonJuliaUtilities.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/ComposedMap.cpp` & `MParT-2.0.2/bindings/julia/src/ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/ConditionalMapBase.cpp` & `MParT-2.0.2/bindings/julia/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/JlArrayConversions.cpp` & `MParT-2.0.2/bindings/julia/src/JlArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/MapObjective.cpp` & `MParT-2.0.2/bindings/julia/src/MapObjective.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/MapOptions.cpp` & `MParT-2.0.2/bindings/julia/src/MapOptions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/MultiIndex.cpp` & `MParT-2.0.2/bindings/julia/src/MultiIndex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/ParameterizedFunctionBase.cpp` & `MParT-2.0.2/bindings/julia/src/ParameterizedFunctionBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/TrainMap.cpp` & `MParT-2.0.2/bindings/julia/src/TrainMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/TrainMapAdaptive.cpp` & `MParT-2.0.2/bindings/julia/src/TrainMapAdaptive.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/TriangularMap.cpp` & `MParT-2.0.2/bindings/julia/src/TriangularMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/julia/src/Wrapper.cpp` & `MParT-2.0.2/bindings/julia/src/Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/CMakeLists.txt` & `MParT-2.0.2/bindings/matlab/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus/LICENSE` & `MParT-2.0.2/bindings/matlab/external/mexplus/LICENSE`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/arguments.h` & `MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/arguments.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/dispatch.h` & `MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/dispatch.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxarray.h` & `MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/mxarray.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus/mexplus/mxtypes.h` & `MParT-2.0.2/bindings/matlab/external/mexplus/mexplus/mxtypes.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/external/mexplus_eigen.h` & `MParT-2.0.2/bindings/matlab/external/mexplus_eigen.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/include/MexArrayConversions.h` & `MParT-2.0.2/bindings/matlab/include/MexArrayConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/include/MexOptionsConversions.h` & `MParT-2.0.2/bindings/matlab/include/MexOptionsConversions.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/include/MexWrapperTypes.h` & `MParT-2.0.2/bindings/matlab/include/MexWrapperTypes.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/ATMOptions.m` & `MParT-2.0.2/bindings/matlab/mat/ATMOptions.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/ConditionalMap.m` & `MParT-2.0.2/bindings/matlab/mat/ConditionalMap.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/FixedMultiIndexSet.m` & `MParT-2.0.2/bindings/matlab/mat/FixedMultiIndexSet.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/GaussianKLObjective.m` & `MParT-2.0.2/bindings/matlab/mat/GaussianKLObjective.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/MapOptions/MapOptions.m` & `MParT-2.0.2/bindings/matlab/mat/MapOptions/MapOptions.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/MultiIndex.m` & `MParT-2.0.2/bindings/matlab/mat/MultiIndex.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/MultiIndexSet.m` & `MParT-2.0.2/bindings/matlab/mat/MultiIndexSet.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/ParameterizedFunction.m` & `MParT-2.0.2/bindings/matlab/mat/ParameterizedFunction.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/mat/TrainOptions.m` & `MParT-2.0.2/bindings/matlab/mat/TrainOptions.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/BasisTypes_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/BasisTypes_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/ConditionalMap_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/ConditionalMap_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/FixedMultiIndexSet_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/FixedMultiIndexSet_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/MapObjective_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/MapObjective_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/MexArrayConversions.cpp` & `MParT-2.0.2/bindings/matlab/src/MexArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/MexOptionsConversions.cpp` & `MParT-2.0.2/bindings/matlab/src/MexOptionsConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/MultiIndexSet_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/MultiIndexSet_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/MultiIndex_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/MultiIndex_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp` & `MParT-2.0.2/bindings/matlab/src/ParameterizedFunctionBase_mex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/tests/Test_MultiIndexSet.m` & `MParT-2.0.2/bindings/matlab/tests/Test_MultiIndexSet.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/tests/Test_TriangularMap.m` & `MParT-2.0.2/bindings/matlab/tests/Test_TriangularMap.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/tests/TrainMapAdaptiveTest.m` & `MParT-2.0.2/bindings/matlab/tests/TrainMapAdaptiveTest.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/matlab/tests/TrainMapTest.m` & `MParT-2.0.2/bindings/matlab/tests/TrainMapTest.m`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/include/CommonPybindUtilities.h` & `MParT-2.0.2/bindings/python/include/CommonPybindUtilities.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/package/MParT.egg-info/PKG-INFO` & `MParT-2.0.2/bindings/python/package/MParT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MParT
-Version: 2.0.1
+Version: 2.0.2
 Summary: A Monotone Parameterization Toolkit
 Author: Matthew Parno
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Massachusetts Institute of Technology
         All rights reserved.
```

### Comparing `MParT-2.0.1/bindings/python/package/MParT.egg-info/SOURCES.txt` & `MParT-2.0.2/bindings/python/package/MParT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/AffineMap.cpp` & `MParT-2.0.2/bindings/python/src/AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/CommonPybindUtilities.cpp` & `MParT-2.0.2/bindings/python/src/CommonPybindUtilities.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/ComposedMap.cpp` & `MParT-2.0.2/bindings/python/src/ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/ConditionalMapBase.cpp` & `MParT-2.0.2/bindings/python/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/IdentityMap.cpp` & `MParT-2.0.2/bindings/python/src/IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/MapFactory.cpp` & `MParT-2.0.2/bindings/python/src/MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/MapObjective.cpp` & `MParT-2.0.2/bindings/python/src/MapObjective.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/MapOptions.cpp` & `MParT-2.0.2/bindings/python/src/MapOptions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/MultiIndex.cpp` & `MParT-2.0.2/bindings/python/src/MultiIndex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/ParameterizedFunctionBase.cpp` & `MParT-2.0.2/bindings/python/src/ParameterizedFunctionBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/Serialization.cpp` & `MParT-2.0.2/bindings/python/src/Serialization.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/SummarizedMap.cpp` & `MParT-2.0.2/bindings/python/src/SummarizedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/TrainMap.cpp` & `MParT-2.0.2/bindings/python/src/TrainMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/TrainMapAdaptive.cpp` & `MParT-2.0.2/bindings/python/src/TrainMapAdaptive.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/TriangularMap.cpp` & `MParT-2.0.2/bindings/python/src/TriangularMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/src/Wrapper.cpp` & `MParT-2.0.2/bindings/python/src/Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_AffineFunction.py` & `MParT-2.0.2/bindings/python/tests/test_AffineFunction.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_AffineMap.py` & `MParT-2.0.2/bindings/python/tests/test_AffineMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_ComposedMap.py` & `MParT-2.0.2/bindings/python/tests/test_ComposedMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_ComposedMap_moveCoeffs.py` & `MParT-2.0.2/bindings/python/tests/test_ComposedMap_moveCoeffs.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_ConditionalMapBase.py` & `MParT-2.0.2/bindings/python/tests/test_ConditionalMapBase.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_IdentityMap.py` & `MParT-2.0.2/bindings/python/tests/test_IdentityMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_MapFactory.py` & `MParT-2.0.2/bindings/python/tests/test_MapFactory.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_MultiIndex.py` & `MParT-2.0.2/bindings/python/tests/test_MultiIndex.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_MultiIndexSet.py` & `MParT-2.0.2/bindings/python/tests/test_MultiIndexSet.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_Serialization.py` & `MParT-2.0.2/bindings/python/tests/test_Serialization.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_SummarizedMap.py` & `MParT-2.0.2/bindings/python/tests/test_SummarizedMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_TrainMap.py` & `MParT-2.0.2/bindings/python/tests/test_TrainMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_TrainMapAdaptive.py` & `MParT-2.0.2/bindings/python/tests/test_TrainMapAdaptive.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_TriangularMap.py` & `MParT-2.0.2/bindings/python/tests/test_TriangularMap.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/bindings/python/tests/test_TriangularMap_moveCoeffs.py` & `MParT-2.0.2/bindings/python/tests/test_TriangularMap_moveCoeffs.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/cmake/BuildDocs.cmake` & `MParT-2.0.2/cmake/BuildDocs.cmake`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/cmake/FindJulia.cmake` & `MParT-2.0.2/cmake/FindJulia.cmake`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/cmake/SetInstallPaths.cmake` & `MParT-2.0.2/cmake/SetInstallPaths.cmake`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/Makefile` & `MParT-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/_static/pics/Density.png` & `MParT-2.0.2/docs/_static/pics/Density.png`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/_static/pics/Regression.png` & `MParT-2.0.2/docs/_static/pics/Regression.png`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/_static/pics/Samples.png` & `MParT-2.0.2/docs/_static/pics/Samples.png`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/_static/pics/Transformation2d.png` & `MParT-2.0.2/docs/_static/pics/Transformation2d.png`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/conf.py` & `MParT-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/index.rst` & `MParT-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/make.bat` & `MParT-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/mpart.doxyfile.in` & `MParT-2.0.2/docs/mpart.doxyfile.in`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/api/concepts/cachedparameterization.rst` & `MParT-2.0.2/docs/source/api/concepts/cachedparameterization.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/api/multiindex.rst` & `MParT-2.0.2/docs/source/api/multiindex.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/api/templateconcepts.rst` & `MParT-2.0.2/docs/source/api/templateconcepts.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/api/utilities/linearalgebra.rst` & `MParT-2.0.2/docs/source/api/utilities/linearalgebra.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/api/utilities/serialization.rst` & `MParT-2.0.2/docs/source/api/utilities/serialization.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/development/index.rst` & `MParT-2.0.2/docs/source/development/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/getting_started.rst` & `MParT-2.0.2/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/installation.rst` & `MParT-2.0.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/mathematics.rst` & `MParT-2.0.2/docs/source/mathematics.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/docs/source/tutorials/index.rst` & `MParT-2.0.2/docs/source/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/joss/paper.bib` & `MParT-2.0.2/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/joss/paper.md` & `MParT-2.0.2/joss/paper.md`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/joss/performance_comparison.png` & `MParT-2.0.2/joss/performance_comparison.png`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/pyproject.toml` & `MParT-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 authors = [
     {name = "Matthew Parno"},
 ]
 license={file="LICENSE.txt"}
 readme="README.md"
 requires-python = ">=3.7"
 description="A Monotone Parameterization Toolkit"
-version="2.0.1"
+version="2.0.2"
 keywords=["Measure Transport", "Monotone", "Transport Map", "Isotonic Regression", "Triangular", "Knothe-Rosenblatt"]
 
 [project.urls]
 Documentation = "https://measuretransport.github.io/MParT/"
 Source = "https://github.com/MeasureTransport/MParT"
```

### Comparing `MParT-2.0.1/src/AffineFunction.cpp` & `MParT-2.0.2/src/AffineFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/AffineMap.cpp` & `MParT-2.0.2/src/AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/CMakeLists.txt` & `MParT-2.0.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/ComposedMap.cpp` & `MParT-2.0.2/src/ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/ConditionalMapBase.cpp` & `MParT-2.0.2/src/ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/Distributions/DensityBase.cpp` & `MParT-2.0.2/src/Distributions/DensityBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/Distributions/GaussianSamplerDensity.cpp` & `MParT-2.0.2/src/Distributions/GaussianSamplerDensity.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/Distributions/PullbackDensity.cpp` & `MParT-2.0.2/src/Distributions/PullbackDensity.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/IdentityMap.cpp` & `MParT-2.0.2/src/IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactory.cpp` & `MParT-2.0.2/src/MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl1.cpp` & `MParT-2.0.2/src/MapFactoryImpl1.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl10.cpp` & `MParT-2.0.2/src/MapFactoryImpl10.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl11.cpp` & `MParT-2.0.2/src/MapFactoryImpl11.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl12.cpp` & `MParT-2.0.2/src/MapFactoryImpl12.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl13.cpp` & `MParT-2.0.2/src/MapFactoryImpl13.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl14.cpp` & `MParT-2.0.2/src/MapFactoryImpl14.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl15.cpp` & `MParT-2.0.2/src/MapFactoryImpl15.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl16.cpp` & `MParT-2.0.2/src/MapFactoryImpl16.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl17.cpp` & `MParT-2.0.2/src/MapFactoryImpl17.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl18.cpp` & `MParT-2.0.2/src/MapFactoryImpl18.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl2.cpp` & `MParT-2.0.2/src/MapFactoryImpl2.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl3.cpp` & `MParT-2.0.2/src/MapFactoryImpl3.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl4.cpp` & `MParT-2.0.2/src/MapFactoryImpl4.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl5.cpp` & `MParT-2.0.2/src/MapFactoryImpl5.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl6.cpp` & `MParT-2.0.2/src/MapFactoryImpl6.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl7.cpp` & `MParT-2.0.2/src/MapFactoryImpl7.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl8.cpp` & `MParT-2.0.2/src/MapFactoryImpl8.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapFactoryImpl9.cpp` & `MParT-2.0.2/src/MapFactoryImpl9.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MapObjective.cpp` & `MParT-2.0.2/src/MapObjective.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MultiIndices/FixedMultiIndexSet.cpp` & `MParT-2.0.2/src/MultiIndices/FixedMultiIndexSet.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MultiIndices/MultiIndex.cpp` & `MParT-2.0.2/src/MultiIndices/MultiIndex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MultiIndices/MultiIndexLimiter.cpp` & `MParT-2.0.2/src/MultiIndices/MultiIndexLimiter.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MultiIndices/MultiIndexNeighborhood.cpp` & `MParT-2.0.2/src/MultiIndices/MultiIndexNeighborhood.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/MultiIndices/MultiIndexSet.cpp` & `MParT-2.0.2/src/MultiIndices/MultiIndexSet.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/ParameterizedFunctionBase.cpp` & `MParT-2.0.2/src/ParameterizedFunctionBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/SummarizedMap.cpp` & `MParT-2.0.2/src/SummarizedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/TrainMap.cpp` & `MParT-2.0.2/src/TrainMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/TrainMapAdaptive.cpp` & `MParT-2.0.2/src/TrainMapAdaptive.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/TriangularMap.cpp` & `MParT-2.0.2/src/TriangularMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/Utilities/LinearAlgebra.cpp` & `MParT-2.0.2/src/Utilities/LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/src/Utilities/Miscellaneous.cpp` & `MParT-2.0.2/src/Utilities/Miscellaneous.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/CMakeLists.txt` & `MParT-2.0.2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_DensityBase.cpp` & `MParT-2.0.2/tests/Distributions/Test_DensityBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_Distribution.cpp` & `MParT-2.0.2/tests/Distributions/Test_Distribution.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_Distributions_Common.cpp` & `MParT-2.0.2/tests/Distributions/Test_Distributions_Common.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_Distributions_Common.h` & `MParT-2.0.2/tests/Distributions/Test_Distributions_Common.h`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_GaussianDistribution.cpp` & `MParT-2.0.2/tests/Distributions/Test_GaussianDistribution.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_SampleGenerator.cpp` & `MParT-2.0.2/tests/Distributions/Test_SampleGenerator.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_TransportDensity.cpp` & `MParT-2.0.2/tests/Distributions/Test_TransportDensity.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_TransportDistributionFactory.cpp` & `MParT-2.0.2/tests/Distributions/Test_TransportDistributionFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Distributions/Test_TransportSampler.cpp` & `MParT-2.0.2/tests/Distributions/Test_TransportSampler.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/MultiIndices/Test_MultiIndex.cpp` & `MParT-2.0.2/tests/MultiIndices/Test_MultiIndex.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/MultiIndices/Test_MultiIndexSet.cpp` & `MParT-2.0.2/tests/MultiIndices/Test_MultiIndexSet.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/RunTests.cpp` & `MParT-2.0.2/tests/RunTests.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_AffineFunction.cpp` & `MParT-2.0.2/tests/Test_AffineFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_AffineMap.cpp` & `MParT-2.0.2/tests/Test_AffineMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_ArrayConversions.cpp` & `MParT-2.0.2/tests/Test_ArrayConversions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_ComposedMap.cpp` & `MParT-2.0.2/tests/Test_ComposedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_ConditionalMapBase.cpp` & `MParT-2.0.2/tests/Test_ConditionalMapBase.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_HermiteFunctions.cpp` & `MParT-2.0.2/tests/Test_HermiteFunctions.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_IdentityMap.cpp` & `MParT-2.0.2/tests/Test_IdentityMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_LinearAlgebra.cpp` & `MParT-2.0.2/tests/Test_LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_LinearizedBasis.cpp` & `MParT-2.0.2/tests/Test_LinearizedBasis.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_MapFactory.cpp` & `MParT-2.0.2/tests/Test_MapFactory.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_MapObjective.cpp` & `MParT-2.0.2/tests/Test_MapObjective.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_MonotoneComponent.cpp` & `MParT-2.0.2/tests/Test_MonotoneComponent.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_MultivariateExpansion.cpp` & `MParT-2.0.2/tests/Test_MultivariateExpansion.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_MultivariateExpansionWorker.cpp` & `MParT-2.0.2/tests/Test_MultivariateExpansionWorker.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_OrthogonalPolynomials.cpp` & `MParT-2.0.2/tests/Test_OrthogonalPolynomials.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_PositiveBijectors.cpp` & `MParT-2.0.2/tests/Test_PositiveBijectors.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_Quadrature.cpp` & `MParT-2.0.2/tests/Test_Quadrature.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_Serialization.cpp` & `MParT-2.0.2/tests/Test_Serialization.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_SummarizedMap.cpp` & `MParT-2.0.2/tests/Test_SummarizedMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_TensorProductFunction.cpp` & `MParT-2.0.2/tests/Test_TensorProductFunction.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_TrainMap.cpp` & `MParT-2.0.2/tests/Test_TrainMap.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_TrainMapAdaptive.cpp` & `MParT-2.0.2/tests/Test_TrainMapAdaptive.cpp`

 * *Files identical despite different names*

### Comparing `MParT-2.0.1/tests/Test_TriangularMap.cpp` & `MParT-2.0.2/tests/Test_TriangularMap.cpp`

 * *Files identical despite different names*

