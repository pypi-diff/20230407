# Comparing `tmp/RIFT-0.0.15.8rc5.tar.gz` & `tmp/RIFT-0.0.15.8rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RIFT-0.0.15.8rc5.tar", last modified: Fri Mar 24 18:44:44 2023, max compression
+gzip compressed data, was "dist/RIFT-0.0.15.8rc6.tar", last modified: Fri Apr  7 18:25:00 2023, max compression
```

## Comparing `RIFT-0.0.15.8rc5.tar` & `RIFT-0.0.15.8rc6.tar`

### file list

```diff
@@ -1,182 +1,186 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc5/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/requirements.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MANIFEST.in
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc5/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5648 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/README.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc5/Dockerfile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc5/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/LICENSE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/setup.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6802 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/setup.cfg
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10170 2023-03-24 18:44:41.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-03-24 18:44:41.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6802 2023-03-24 18:44:41.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-03-24 18:44:41.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-03-24 18:44:41.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    62207 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18076 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26904 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    67261 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   240388 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:43.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    90370 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-03-24 18:44:44.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    95287 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   112733 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98368 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11855 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    73238 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29365 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   157172 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/LICENSE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MANIFEST.in
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   241367 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18359 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28094 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   108434 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11893 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    73473 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98549 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    95698 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   113357 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10419 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/requirements.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/setup.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc6/Dockerfile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/README.md
```

### Comparing `RIFT-0.0.15.8rc5/INSTALL.md` & `RIFT-0.0.15.8rc6/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/howto.md` & `RIFT-0.0.15.8rc6/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/PACKAGING.md` & `RIFT-0.0.15.8rc6/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/README.md` & `RIFT-0.0.15.8rc6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
   6. If you are using a distance-marginalized likeliihood, please acknowledge 
      1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
 
   7. If you are using a special coordinate system
      1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
      1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+  
+  8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
 
 ## Authorlists: Opt-in model
 Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
 
 We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
  * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
  * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
```

### Comparing `RIFT-0.0.15.8rc5/Dockerfile` & `RIFT-0.0.15.8rc6/Dockerfile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/GETTING_STARTED.md` & `RIFT-0.0.15.8rc6/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/TROUBLESHOOTING.md` & `RIFT-0.0.15.8rc6/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/LICENSE.md` & `RIFT-0.0.15.8rc6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.8rc6/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/setup.py` & `RIFT-0.0.15.8rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.8rc5", # do not build on OSX machine, side effects
+    version="0.0.15.8rc6", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

### Comparing `RIFT-0.0.15.8rc5/PKG-INFO` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc5
+Version: 0.0.15.8rc6
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
@@ -49,14 +49,16 @@
         
           6. If you are using a distance-marginalized likeliihood, please acknowledge 
              1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
         
           7. If you are using a special coordinate system
              1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
              1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+          
+          8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
         
         ## Authorlists: Opt-in model
         Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
         
         We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
          * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
          * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
```

### Comparing `RIFT-0.0.15.8rc5/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.8rc6/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
 MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
 MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
 MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
 MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
 MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
 MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
 MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
 MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
 MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
@@ -121,14 +122,17 @@
 MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
 MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
 MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
 MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
 MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
 MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
 MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
 MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
 MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
 MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
 MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
 MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
 MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
 MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.8rc6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc5
+Version: 0.0.15.8rc6
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
@@ -49,14 +49,16 @@
         
           6. If you are using a distance-marginalized likeliihood, please acknowledge 
              1. Distance marginalization : Soichiro Morisaki, Dan Wysocki, see  Wofford et al https://dcc.ligo.org/P2200059
         
           7. If you are using a special coordinate system
              1. Rotated inspiral-phase : cite the original Lee, Morisaki, Tagoshi paper ([journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.105.124057) [dcc](https://dcc.ligo.org/LIGO-P2200037)); also cite Wofford et al  [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
              1. Pseudo-cylindrical coordinates: see Wofford et al   [journal](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.107.024040) [dcc](https://dcc.ligo.org/P2200059)
+          
+          8. If you are using calibration marginalization, please acknowledge Ethan Payne  (PRD 122004 (2020)), with RIFT integration provided by Jacob Lange and Daniel Williams
         
         ## Authorlists: Opt-in model
         Several aspects of this code are very actively developed.  We encourage  close collaboration with the lead developers (O'Shaughnessy and Lange) to produce the best possible results, particularly given comparatively rapid changes to the interface and pipeline in the past and planned for the future as the user- and developer-base expands.
         
         We expect to make the final developed code widely available and free to use, in a release-based distribution model.  But we're not there yet.  To simplify discussions about authorlist and ettiquete, we have adopted the following simple model, to be revised 4 times per year (1/15, 4/15, 7/15, 10/15):  
          * Free to use: Any code commit older than 3 years from the date an analysis <i>commences</i> is free to use for any scientific work.  
          * Opt-in: Any more recent use should offer (opt-in) authorship to the lead developers, as well as to developers who contributed significantly to features used in the version of the code adopted in an analysis.  Loosely speaking, the newer the features you use, the more proactive you should be in contacting relevant developers, to insure all authors are suitably engaged with the final product.
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,16 @@
     import pyreprimand as pyr
     has_reprimand=True
 except:
     has_reprimand=False
 
 #import gwemlightcurves.table as gw_eos_table
 
-#from . import MonotonicSpline as ms
-from RIFT.physics import MonotonicSpline as ms
-
+from . import MonotonicSpline as ms
+#from RIFT.physics import MonotonicSpline as ms
 
 C_CGS=lal.C_SI*100
 DENSITY_CGS_IN_MSQUARED=1000*lal.G_SI/lal.C_SI**2  # g/cm^3 -> 1/m^2 //GRUnits. Multiply by this to convert from CGS -> 1/m^2 units (_geom). lal.G_SI/lal.C_SI**2 takes kg/m^3 -> 1/m^2  ||  https://lscsoft.docs.ligo.org/lalsuite/lalsimulation/_l_a_l_sim_neutron_star_8h_source.html
 PRESSURE_CGS_IN_MSQUARED = DENSITY_CGS_IN_MSQUARED/(lal.C_SI*100)**2
 
 
 def make_compactness_from_lambda_approximate(lambda_vals):
@@ -245,15 +244,15 @@
            WARNING: Will generally match imperfectly, need some resolution to that procedure
     Creates
         * LALSimulation data structure as desired
     Warning: 
         * Currently generates intermediate data file by writing to disk
     """
     
-    def __init__(self,name=None,eos_data=None,eos_units=None,reject_phase_transitions=True,debug=False, add_low_density=False):
+    def __init__(self,name=None,eos_data=None,eos_units=None,reject_phase_transitions=False,debug=False, add_low_density=False):
         if eos_data is None:
             raise Exception("EOS data required to use EOSFromTabularData")
         if not(name):
             name="default"
         self.name = name
         self.bdens = None
         self.press = None
@@ -297,28 +296,19 @@
             '''
             
         except:
             self.press = eos_data[:,0]      #LALSim EOS format
             self.edens = eos_data[:,1]
         
         if reject_phase_transitions:   # Normally lalsuite can't handle regions of constant pressure. Using a pressure/density only approach isn't suited to phase transitions
-            if not np.all(np.diff(self.press) > 0):    # BLOCKS PHASE TRANSITIONS
-                keep_idx = np.where(np.diff(self.press) > 0)[0] + 1
-                keep_idx = np.concatenate(([0], keep_idx))
-                print(keep_idx)
-                self.press = self.press[keep_idx]
-                self.edens = self.edens[keep_idx]
-            assert np.all(np.diff(self.press) > 0)
-            if not np.all(np.diff(self.edens) > 0):
-                keep_idx = np.where(np.diff(self.edens) > 0)[0] + 1
-                keep_idx = np.concatenate(([0], keep_idx))
-                self.press = self.press[keep_idx]
-                self.edens = self.edens[keep_idx]
-            assert np.all(np.diff(self.edens) > 0)
-        
+            param_dict = {'energy_density': self.edens,'pressure': self.press}
+            check_monotonic(param_dict,preserve_same_length = True)
+            
+            self.edens = param_dict['energy_density']
+            self.press = param_dict['pressure']
         # Create temporary file
         if debug:
                 print("Dumping to %s" % self.fname)
         eos_fname = "./" +name + "_geom.dat" # assume write acces
         np.savetxt(eos_fname, np.transpose((self.press, self.edens)), delimiter='\t', header='pressure \t energy_density ')
         
         self.eos = lalsim.SimNeutronStarEOSFromFile(eos_fname)
@@ -501,16 +491,16 @@
         self.eos = None
         self.eos_fam = None
 
         self.spec_params = spec_params
 #        print spec_params
 
         if use_lal_spec_eos:
-#            self.eos=lalsim.SimNeutronStarEOS4ParameterSpectralDecomposition(spec_params['gamma1'], spec_params['gamma2'], spec_params['gamma3'], spec_params['gamma4'])   # Should have this function! but only on master
-            self.eos=lalsim.SimNeutronStarEOSSpectralDecomposition_for_plot(spec_params['gamma1'], spec_params['gamma2'], spec_params['gamma3'], spec_params['gamma4'],4)
+            self.eos=lalsim.SimNeutronStarEOS4ParameterSpectralDecomposition(spec_params['gamma1'], spec_params['gamma2'], spec_params['gamma3'], spec_params['gamma4'])  
+#            self.eos=lalsim.SimNeutronStarEOSSpectralDecomposition_for_plot(spec_params['gamma1'], spec_params['gamma2'], spec_params['gamma3'], spec_params['gamma4'],4)        
         else:
             # Create data file
             self.make_spec_param_eos(500,save_dat=True,ligo_units=True,verbose=verbose)
             # Use data file
             #print " Trying to load ",name+"_geom.dat"
             import os; #print os.listdir('.')
             cwd = os.getcwd()
@@ -741,15 +731,17 @@
             
             param_dict = dict()
             param_dict['pseudo_enthalpy'] = qry_object.extract_param('pseudo_enthalpy',hvals)
             param_dict['rest_mass_density'] = qry_object.extract_param('rest_mass_density',hvals)
             param_dict['energy_density'] = qry_object.extract_param('energy_density',hvals)
             param_dict['pressure'] = qry_object.extract_param('pressure',hvals)
             param_dict['sound_speed_over_c'] = qry_object.extract_param('sound_speed_over_c',hvals)
-            param_dict = eos_monotonic_parts_and_causal_sound_speed(param_dict)
+            
+            #just_check_monotonicity_and_causality(param_dict)
+            #param_dict = eos_monotonic_parts_and_causal_sound_speed(param_dict,preserve_same_length = False) # Don't enable by default. First check if monotonicity or causality is violated indeed, and document if it does.
             self.update(param_dict,specific_internal_energy)
         else:
             print(" Warning: Empty EOS object created")
         return None
     
     def update(self,param_dict,specific_internal_energy):
         # minimum required input, cgs units like everything else above
@@ -800,14 +792,16 @@
 
 # RePrimAnd
 def make_mr_lambda_reprimand(eos,n_bins=800,save_tov_sequence=False,read_tov_sequence=False,return_eos_object=False, m_b_units = lal.MP_SI):
     """
     Construct mass-radius curve from EOS using RePrimAnd (https://wokast.github.io/RePrimAnd/tov_solver.html).
     Parameter `eos` should be in RePrimAnd's eos object format, made with something like `make_eos_barotr_spline` (https://wokast.github.io/RePrimAnd/eos_barotr_ref.html).
     By default this returns the Mass_g-Radius-Lambda-Mass_b. But if `return_eos_object` is True, this will also return the RePrimAnd EOS object.
+    Wolfgang Kastaun, Jay Vijay Kalinani, and Riccardo Ciolfi. Robust recovery of primitive variables in relativistic ideal magnetohydrodynamics. Phys. Rev. D, 103(2):023018, 2021. doi:10.1103/PhysRevD.103.023018.
+    Roland Haas and Wolfgang Kastaun. (2023). wokast/RePrimAnd: Release 1.6 (v1.6). Zenodo. https://doi.org/10.5281/zenodo.7700296
     """
     
     """
     For units refer: https://wokast.github.io/RePrimAnd/little_helpers.html#units
     uni = pyr.units.geom_solar(g_si=6.673e-11)
     uni.length, uni.time, uni.mass
     pyr.units.geom_meter() is such that length = 1, time = 1/c, mass = Mo/1000 in [kg] . length and time are related (factor of c). mass is related to G.
@@ -826,14 +820,15 @@
     acc_tov=1e-10; acc_deform=1e-8; minsteps=500; num_samp=2500; mgrav_min=0.3
     acc = pyr.tov_acc_simple(acc_tov, acc_deform, minsteps)
     try: seq = pyr.make_tov_branch_stable(eos, acc, num_samp=num_samp, mgrav_min=mgrav_min)
     except:
         if read_tov_sequence:
             sol_units = pyr.units.geom_solar(msun_si=lal.MSUN_SI)
             seq = pyr.load_star_branch(eos, sol_units)
+        else: raise Exception("No EOS supplied.")
     if save_tov_sequence:
             try:
                 #bpath = p.parent
                 #spath = bpath / "tov.seq.h5"
                 spath = "tov.seq.h5"
                 pyr.save_star_branch(str(spath), seq)
             except:
@@ -852,74 +847,89 @@
     c = mrL_dat[:,0]/mrL_dat[:,1]    #compactness
     
     if return_eos_object: return mrL_dat, seq
     
     return mrL_dat
 
 
+def just_check_monotonicity_and_causality(param_dict):
+    """
+    To be used for only checking monotonicity and causality
+    True means good. False means violation.
+    """
+    monotonicity_and_causality = {'pseudo_enthalpy_is_monotonic': True,
+                      'rest_mass_density_is_monotonic': True,
+                      'energy_density_is_monotonic': True,
+                      'pressure_is_monotonic': True,
+                      'sound_speed_over_c_is_causal': True}
+    for param in param_dict:
+        if param == 'sound_speed_over_c':
+            if not all(param_dict[param]<=1): monotonicity_and_causality['sound_speed_over_c_is_causal'] = False
+        else:
+            if not all(np.diff(param_dict[param])>0) : monotonicity_and_causality[param+'_is_monotonic'] = False
+    return monotonicity_and_causality
 
 
 def check_monotonic(monotonic_params, other_params=None, preserve_same_length = False):
     """
     Checks monotonicity of monotonic_params and removes non-monotonic parts in it for both monotonic_params and other_params.
     By default this will reduce the length of data due to deletion of non-monotonic patches, but preserve_same_length can be turned true to keep length of data intact.
     """
     if not preserve_same_length:
         for param in monotonic_params:
             i = 0
             while i < len(monotonic_params[param])-1:
-                if monotonic_params[param][i+1] < monotonic_params[param][i]:
+                if monotonic_params[param][i+1] <= monotonic_params[param][i]:
                     for param2 in monotonic_params:
                         try: monotonic_params[param2] = np.delete(monotonic_params[param2], i+1)
                         except:    del monotonic_params[param2][i+1]
                     if other_params is None: pass
                     else:
                         for param2 in other_params:
                             try: other_params[param2] = np.delete(other_params[param2], i+1)
                             except:    del other_params[param2][i+1]
                     i-=1
-                i +=1
+                i+=1
     else:
         for param in monotonic_params:
             i = 0
             while i < len(monotonic_params[param])-1:
-                if monotonic_params[param][i+1] < monotonic_params[param][i]:
-                    for param2 in monotonic_params:
-                        monotonic_params[param][i+1] = monotonic_params[param][i]*1.0001
-                    if 'pseudo_enthalpy' in other_params: other_params['sound_speed_over_c'][i+1] = other_params['sound_speed_over_c'][i]*1.0001
-                    if 'sound_speed_over_c' in other_params:other_params['sound_speed_over_c'][i+1] = 0
-                i +=1
+                if monotonic_params[param][i+1] <= monotonic_params[param][i]:
+                    monotonic_params[param][i+1] = monotonic_params[param][i]*1.01
+                    if other_params is not None: 
+                        if 'sound_speed_over_c' in other_params:other_params['sound_speed_over_c'][i+1] = 0
+                i+=1
     return
 
-def check_sound_speed_causal(param_dict, truncate = True):
-    """Checks if sound speed exceeds 1 anywhere, and depending on option `truncate` removes that region or or forces it =1. """
+def check_sound_speed_causal(param_dict, preserve_same_length = False):
+    """Checks if sound speed exceeds 1 anywhere, and depending on the option `preserve_same_length` removes that region or forces it =1. """
     below_speed_of_light = np.where(param_dict['sound_speed_over_c']<= 1)
-    if truncate :
+    if not preserve_same_length :
         param_dict = {'pseudo_enthalpy': param_dict['pseudo_enthalpy'][below_speed_of_light],
                       'rest_mass_density': param_dict['rest_mass_density'][below_speed_of_light],
                       'energy_density': param_dict['energy_density'][below_speed_of_light],
                       'pressure': param_dict['pressure'][below_speed_of_light],
                       'sound_speed_over_c': param_dict['sound_speed_over_c'][below_speed_of_light]}
     else: param_dict['sound_speed_over_c'][np.where(param_dict['sound_speed_over_c']> 1)[0]] = 1
     return param_dict
 
 
 def eos_monotonic_parts_and_causal_sound_speed(param_dict, preserve_same_length = False):
     param_dict_main = {'rest_mass_density': param_dict['rest_mass_density'], 'energy_density': param_dict['energy_density'],'pressure': param_dict['pressure']}
     param_dict_others = {'pseudo_enthalpy': param_dict['pseudo_enthalpy'], 'sound_speed_over_c': param_dict['sound_speed_over_c']}
     
-    check_monotonic(param_dict_main, param_dict_others, preserve_same_length =preserve_same_length)
+    check_monotonic(param_dict_main, param_dict_others, preserve_same_length=preserve_same_length)
     
     param_dict = {'pseudo_enthalpy': param_dict_others['pseudo_enthalpy'],
                   'rest_mass_density': param_dict_main['rest_mass_density'],
                   'energy_density':param_dict_main['energy_density'],
                   'pressure':param_dict_main['pressure'],
                   'sound_speed_over_c':param_dict_others['sound_speed_over_c']
                   }
-    param_dict = check_sound_speed_causal(param_dict)
+    param_dict = check_sound_speed_causal(param_dict, preserve_same_length=preserve_same_length)
     return param_dict
 
 ####
 #### SUPPORT CODE FOLLOWS
 
 def gamma_of_x(x, coeffs):
         """
@@ -1326,8 +1336,8 @@
             return ##Check this conversion. possibly same as density with or without c**2. [MeV fm^-3]
         
         # IN PROGRESS
         #   - adiabatic index
         #Gamma = (self.extraction_dict_lalsim['energy_density']()*(lal.C_SI*100)**2 + self.extraction_dict_lalsim['pressure']())/(self.extraction_dict_lalsim['pressure']()) *np.square(self.extraction_dict_lalsim['sound_speed_over_c']())
     
     def extract_param(self, p, pseudo_enthalpy):
-        return self.extraction_dict_lalsim[p](pseudo_enthalpy)
+        return self.extraction_dict_lalsim[p](pseudo_enthalpy)
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     is a combination of one or more Gaussian curves, in one or more dimensions.
 
     Parameters
     ----------
     d : int
         Total number of dimensions.
 
-    bounds : np.ndarray
+    bounds : dictionary with array bounds, with keys matching gmm_dict
         Limits of integration, where each row represents [left_lim, right_lim]
         for its corresponding dimension.
 
     gmm_dict : dict
         Dictionary where each key is a tuple of one or more dimensions
         that are to be modeled together. If the integrand has strong correlations between
         two or more dimensions, they should be grouped. Each value is by default initialized
@@ -194,15 +194,19 @@
 
     def _calculate_results(self):
         if self.use_lnL:
             lnL = np.copy(self.value_array) # changing the naming convention, just for this function, now that I know better
         else:
             lnL = np.log(self.value_array+regularize_log_scale)
         # strip off any samples with likelihoods less than our cutoff
-        mask = lnL > (np.log(self.L_cutoff) if self.L_cutoff > 0 else -np.inf)
+        mask = np.ones(lnL.shape,dtype=bool)
+        if not(self.L_cutoff is None):  # if not none
+            if not(np.isinf(self.L_cutoff)):  # and not infinite, then apply the cutoff
+                mask = lnL > (np.log(self.L_cutoff) if self.L_cutoff > 0 else -np.inf)
+#        print(mask, self.L_cutoff, lnL)
         lnL = lnL[mask]
         prior = self.prior_array[mask]
         sampling_prior = self.sampling_prior_array[mask]
         
         # append to the cumulative arrays
         self.cumulative_samples = np.append(self.cumulative_samples, self.sample_array[mask], axis=0)
         self.cumulative_values = np.append(self.cumulative_values, lnL, axis=0)
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from collections import defaultdict
 
 import numpy as np
 
 import itertools
 import functools
 
+import scipy.special
+
 #from statutils import cumvar
 
 from multiprocessing import Pool
 
 
 # Mirror healpy stuff
 from RIFT.integrators.mcsampler import HealPixSampler
@@ -268,15 +270,18 @@
         dict_return_q = kwargs["dict_return"] if "dict_return" in kwargs else False  # default.  Method for passing back rich data structures for debugging
 
         tripwire_fraction = kwargs["tripwire_fraction"] if "tripwire_fraction" in kwargs else 2  # make it impossible to trigger
         tripwire_epsilon = kwargs["tripwire_epsilon"] if "tripwire_epsilon" in kwargs else 0.001 # if we are not reasonably far away from unity, fail!
 
         use_lnL = kwargs["use_lnL"] if "use_lnL" in kwargs else False 
         return_lnI = kwargs["return_lnI"] if "return_lnI" in kwargs else False
-        
+
+        bFairdraw  = kwargs["igrand_fairdraw_samples"] if "igrand_fairdraw_samples" in kwargs else False
+        n_extr = kwargs["igrand_fairdraw_samples_max"] if "igrand_fairdraw_samples_max" in kwargs else None
+
         # set up a lot of preliminary stuff
         self.func = func
         self.curr_args = args
         if n_comp is None:
             print('No n_comp given, assuming 1 component per dimension')
             n_comp = 1
         dim = len(args)
@@ -346,14 +351,34 @@
         for param in args:
             self._rvs[param] = sample_array[:,index]
             index += 1
         self._rvs['joint_prior'] = prior_array
         self._rvs['joint_s_prior'] = p_array
         self._rvs['integrand'] = value_array
 
+        # Do a fair draw of points, if option is set. CAST POINTS BACK TO NUMPY, IDEALLY
+        if bFairdraw and not(n_extr is None):
+           n_extr = int(np.min([n_extr,1.5*eff_samp,1.5*neff]))
+           print(" Fairdraw size : ", n_extr)
+           if return_lnI:
+               ln_wt =  integrator.cumulative_values
+           else:
+               ln_wt = np.log(value_array)
+           ln_wt += np.log(prior_array/p_array)
+           ln_wt += - scipy.special.logsumexp(ln_wt)
+           wt = np.exp(ln_wt)
+           if n_extr < len(value_array):
+               indx_list = np.random.choice(np.arange(len(wt)), size=n_extr,replace=True,p=wt) # fair draw
+               # FIXME: See previous FIXME
+               for key in list(self._rvs.keys()):
+                   if isinstance(key, tuple):
+                       self._rvs[key] = self._rvs[key][:,indx_list]
+                   else:
+                       self._rvs[key] = self._rvs[key][indx_list]
+
         # if special return structure, fill it
         dict_return = {}
         if dict_return_q:
             dict_return["integrator"] = integrator
 
         # write data to file
         if write_to_file:
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,15 @@
         # the spacing used.
         histogram_edges, dx = self.xpy.linspace(
             0.0, 1.0, n_bins+1,
             retstep=True,
         )
 
         # Initialize output array for CDF.
+        # Reminder:   histogram_cdf[0] ==0 (hardcoded) and we *should* have histogram_cdf[-1 == n_bins+1] == 1
         histogram_cdf = self.xpy.empty(n_bins+1, dtype=numpy.float64)
 
         # Store basic setup parameters
         self.x_min[param] = x_min
         self.x_max[param] = x_max
         self.x_max_minus_min[param] = x_max_minus_min
         self.dx[param] = dx
@@ -277,14 +278,20 @@
         )
         # Evaluate the histogram at each of the bins.
         histogram_values = vectorized_general_tools.histogram(
             y_samples, self.n_bins[param],
             xpy=self.xpy,
             weights=weights
         )
+        # *renormalize* histogram
+        #   - ideally this isn't necessary, BUT mainly for GPUs there can be some points lost to the nbins+1 region due to truncation
+        #   - this slightly breaks normalization, and produces an overabundance in the highest bin when we build the CDF. Which (I think) cascades.
+        #    - because we use a histogram CDF later
+        histogram_values *= 1./self.xpy.sum(histogram_values)
+
         # Smooth the histogram
 #        kernel_size =3
 #        histogram_values = self.xpy.convolve( histogram_values, self.xpy.ones(kernel_size)/kernel_size,mode='same')
         # Mix with a uniform sampling
         histogram_values =    histogram_values*(1-floor_level)+floor_level*self.xpy.ones(len(histogram_values))/len(histogram_values)
 
         # Evaluate the CDF by taking a cumulative sum of the histogram.
@@ -792,14 +799,32 @@
             # FIXME: See previous FIXME
             for key in list(self._rvs.keys()):
                 if isinstance(key, tuple):
                     self._rvs[key] = self._rvs[key][:,indx_list]
                 else:
                     self._rvs[key] = self._rvs[key][indx_list]
 
+        # Do a fair draw of points, if option is set. CAST POINTS BACK TO NUMPY, IDEALLY
+        if bFairdraw and not(n_extr is None):
+           n_extr = int(numpy.min([n_extr,1.5*eff_samp,1.5*neff]))
+           print(" Fairdraw size : ", n_extr)
+           ln_wt = self.xpy.array(self._rvs["log_integrand"] + self._rvs["log_joint_prior"] - self._rvs["log_joint_s_prior"] ,dtype=float)
+           ln_wt = identity_convert(ln_wt)  # send to CPU
+           ln_wt += - scipy.special.logsumexp(ln_wt)
+           wt = xpy.exp(identity_convert_togpu(ln_wt))
+           if n_extr < len(self._rvs["log_integrand"]):
+               indx_list = self.xpy.random.choice(self.xpy.arange(len(wt)), size=n_extr,replace=True,p=wt) # fair draw
+               # FIXME: See previous FIXME
+               for key in list(self._rvs.keys()):
+                   if isinstance(key, tuple):
+                       self._rvs[key] = identity_convert(self._rvs[key][:,indx_list])
+                   else:
+                       self._rvs[key] = identity_convert(self._rvs[key][indx_list])
+
+
         # Create extra dictionary to return things
         dict_return ={}
         if convergence_tests is not None:
             dict_return["convergence_test_results"] = last_convergence_test
 
         # perform type conversion of all stored variables
         if cupy_ok:
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,29 @@
 A collection of useful data analysis routines
 built from the SWIG wrappings of LAL and LALSimulation.
 """
 import sys
 import copy
 import types
 has_external_teobresum=False
-try:
+import os
+info_use_ext = True
+if 'RIFT_NO_EXTERNAL' in os.environ:
+    info_use_ext = False
+    has_external_teobresum=False
+else:
+ try:
     import EOBRun_module
     has_external_teobresum=True
-except:
+ except:
+    has_external_teobresum=False
     True; # print(" - no EOBRun (TEOBResumS) - ")
+info_use_resum_polarizations = False
+if 'RIFT_RESUM_POLARIZATIONS' in os.environ:
+    info_use_resum_polarizations=True  # fallback to ChooseTDModesFromPolarizations for TEOBResumS (since ChooseTDModes is not available at present)
 from six.moves import range
 
 import numpy as np
 from numpy import sin, cos
 from scipy import interpolate
 from scipy import signal
 import scipy  # for decimate
@@ -260,15 +270,15 @@
 except:
    lalIMRPhenomXP = -11
    lalIMRPhenomHM = -14
    lalIMRPhenomXHM = -15
    lalSEOBNRv4HM_ROM = -16
    lalIMRPhenomXPHM = -17
 
-pending_FD_approx = ['IMRPhenomXP_NRTidalv2', 'IMRPhenomXAS_NRTidalv2']
+pending_FD_approx = ['IMRPhenomXP_NRTidalv2', 'IMRPhenomXAS_NRTidalv2','IMRPhenomXO4a']
 pending_approx_code = {}
 pending_default_code = -18
 for name in pending_FD_approx:
     if hasattr(lalsim, name):
         pending_approx_code[name] = getattr(lalsim, name)
     else:
         pending_approx_code[name] = pending_default_code
@@ -1665,17 +1675,20 @@
                 self.approx = lalSEOBNRv4HM
             if rosDebugMessagesContainer[0]:
                 print( " Loaded approximant ", self.approx,  " AKA ", lalsim.GetStringFromApproximant(self.approx), " from ", row.waveform)
         self.theta = row.latitude # Declination
         self.phi = row.longitude # Right ascension
         self.radec = True # Flag to interpret (theta,phi) as (DEC,RA)
         self.psi = row.polarization
-        self.tref = row.geocent_end_time
-        if lalmetaio_old_style or hasattr(row, 'geocent_end_time_ns'):
-            self.tref += 1e-9*row.geocent_end_time_ns
+        if 'time_geocent' in dir(row):
+            self.tref = row.time_geocent
+        else:
+            self.tref = row.geocent_end_time
+            if lalmetaio_old_style or hasattr(row, 'geocent_end_time_ns'):
+                self.tref += 1e-9*row.geocent_end_time_ns
         if hasattr(row, 'taper'):
             self.taper = lalsim.GetTaperFromString(str(row.taper))
         # FAKED COLUMNS (nonstandard)
         self.lambda1 = row.alpha5
         self.lambda2 = row.alpha6
         self.eccentricity=row.alpha4
         self.snr = row.alpha3   # lnL info
@@ -1693,15 +1706,15 @@
         Create a sim_inspiral table from P.  *One* element from it
         """
         global rosDebugMessagesContainer
         if rosDebugMessagesContainer[0]:
             print( " --- Creating XML row for the following ---- ")
             self.print_params()
         sim_valid_cols = [ "simulation_id", "inclination", "longitude", "latitude", "polarization", "geocent_end_time",  "coa_phase", "distance", "mass1", "mass2", "spin1x", "spin1y", "spin1z", "spin2x", "spin2y", "spin2z"] # ,  "alpha1", "alpha2", "alpha3"
-        if lalmetaio_old_style:
+        if True: #lalmetaio_old_style:
             sim_valid_cols += [ "geocent_end_time_ns"]
         si_table = lsctables.New(lsctables.SimInspiralTable, sim_valid_cols)
         row = si_table.RowType()
         row.simulation_id = si_table.get_next_id()
         # Set all parameters to default value of zero
         for slot in row.__slots__: setattr(row, slot, 0.)
         # Copy parameters
@@ -1715,16 +1728,19 @@
         row.mass2 = self.m2/lsu_MSUN
         row.mchirp = mchirp(row.mass1,row.mass2)
         row.longitude = self.phi
         row.latitude   = self.theta
         row.inclination = self.incl
         row.polarization = self.psi
         row.coa_phase = self.phiref
+        # New code for managing times in output: see https://git.ligo.org/kipp.cannon/python-ligo-lw/-/blob/master/ligo/lw/lsctables.py
+        if 'time_geocent' in dir(row):
+            row.time_geocent = float(self.tref)
         # http://stackoverflow.com/questions/6032781/pythonnumpy-why-does-numpy-log-throw-an-attribute-error-if-its-operand-is-too
-        if lalmetaio_old_style:
+        elif  hasattr(row, 'geocent_time_ns'):   # old school approach, will not work now
             row.geocent_end_time = np.floor( float(self.tref))
             row.geocent_end_time_ns = np.floor( float(1e9*(self.tref - row.geocent_end_time)))
         else:
             row.geocent_end_time = float(self.tref)
         row.distance = self.dist/(1e6*lsu_PC)
         row.amp_order = self.ampO
         # PROBLEM: This line is NOT ROBUST, because of type conversions
@@ -2766,15 +2782,15 @@
     """
 
     # special sauce for EOB, because it is so finicky regarding
     if P.approx == lalsim.EOBNRv2HM and P.m1 == P.m2:
 #        print " Using ridiculous tweak for equal-mass line EOB"
         P.m2 = P.m1*(1-1e-6)
     extra_params = P.to_lal_dict()
-    if P.approx==lalsim.TEOBResumS and has_external_teobresum:
+    if P.approx==lalsim.TEOBResumS and has_external_teobresum and info_use_ext:
         Lmax=8
         modes_used = []
         distance_s = P.dist/lal.C_SI
         m_total_s = MsunInSec*(P.m1+P.m2)/lal.MSUN_SI
         for l in np.arange(2,Lmax+1,1):
             for m in np.arange(0,l+1,1):
                 if m !=0:
@@ -3191,30 +3207,30 @@
                 hlms[key].data.data *= sign_factor
                 hlms[key].data.data[:ntaper]*=vectaper
 
         return hlms
 
     if lalsim.SimInspiralImplementedFDApproximants(P.approx)==1:
         hlms = hlmoft_FromFD_dict(P,Lmax=Lmax)
-    elif (P.approx == lalsim.TaylorT1 or P.approx==lalsim.TaylorT2 or P.approx==lalsim.TaylorT3 or P.approx==lalsim.TaylorT4 or P.approx == lalsim.EOBNRv2HM or P.approx==lalsim.EOBNRv2 or P.approx==lalsim.SpinTaylorT1 or P.approx==lalsim.SpinTaylorT2 or P.approx==lalsim.SpinTaylorT3 or P.approx==lalsim.SpinTaylorT4 or P.approx == lalSEOBNRv4P or P.approx == lalSEOBNRv4PHM or P.approx == lalNRSur7dq4 or P.approx == lalNRSur7dq2 or P.approx==lalNRHybSur3dq8 or P.approx == lalIMRPhenomTPHM) or (P.approx ==lalsim.TEOBResumS and not(has_external_teobresum)):
+    elif (P.approx == lalsim.TaylorT1 or P.approx==lalsim.TaylorT2 or P.approx==lalsim.TaylorT3 or P.approx==lalsim.TaylorT4 or P.approx == lalsim.EOBNRv2HM or P.approx==lalsim.EOBNRv2 or P.approx==lalsim.SpinTaylorT1 or P.approx==lalsim.SpinTaylorT2 or P.approx==lalsim.SpinTaylorT3 or P.approx==lalsim.SpinTaylorT4 or P.approx == lalSEOBNRv4P or P.approx == lalSEOBNRv4PHM or P.approx == lalNRSur7dq4 or P.approx == lalNRSur7dq2 or P.approx==lalNRHybSur3dq8 or P.approx == lalIMRPhenomTPHM) or (P.approx ==lalsim.TEOBResumS and not(has_external_teobresum) and not(info_use_resum_polarizations)):
         # approximant likst: see https://git.ligo.org/lscsoft/lalsuite/blob/master/lalsimulation/lib/LALSimInspiral.c#2541
         extra_params = P.to_lal_dict()
         # prevent segmentation fault when hitting nyquist frequency violations
         if (P.approx == lalSEOBNRv4PHM or P.approx == lalSEOBNRv4P) and P.approx >0:
             try:
                 # fails on error, throws EDOM. This *should* be done internally by ChooseTDModes, but is not working
                 test = lalsim.EOBCheckNyquistFrequency(P.m1/lal.MSUN_SI,P.m2/lal.MSUN_SI, np.array([P.s1x,P.s1y, P.s1z]), np.array([P.s2x,P.s2y, P.s2z]), Lmax,P.approx, P.deltaT)
             except Exception as e:
                 raise NameError(" Nyquist frequency error for v4P/v4PHM, check srate")
         hlms = lalsim.SimInspiralChooseTDModes(P.phiref, P.deltaT, P.m1, P.m2, \
 	    P.s1x, P.s1y, P.s1z, \
 	    P.s2x, P.s2y, P.s2z, \
             P.fmin, P.fref, P.dist, extra_params, \
              Lmax, P.approx)
-    elif P.approx ==lalsim.TEOBResumS and has_external_teobresum:
+    elif P.approx ==lalsim.TEOBResumS and has_external_teobresum and not(info_use_resum_polarizations):  # don't call external if fallback to polarizations
         print("Using TEOBResumS hlms")
         modes_used = []
         distance_s = P.dist/lal.C_SI
         m_total_s = MsunInSec*(P.m1+P.m2)/lal.MSUN_SI
         for l in np.arange(2,Lmax+1,1):
             for m in np.arange(0,l+1,1):
                 if m !=0:
@@ -5206,15 +5222,15 @@
     return x_out
 
 def convert_waveform_coordinates_with_eos(x_in,coord_names=['mc', 'eta'],low_level_coord_names=['m1','m2'],enforce_kerr=False,eos_class=None,no_matter1=False,no_matter2=False,source_redshift=0):
     """
     A wrapper for ChooseWaveformParams() 's coordinate tools (extract_param, assign_param) providing array-formatted coordinate changes.  BE VERY CAREFUL, because coordinates may be defined inconsistently (e.g., holding different variables constant: M and eta, or mc and q)
     """
     try:
-        import EOSManager  # be careful to avoid recursive dependence!
+        import RIFT.physics.EOSManager  as EOSManager # be careful to avoid recursive dependence!
     except:
         print( " - Failed to load EOSManager - ")  # this will occur at the start
     assert not (eos_class==None)
     x_out = np.zeros( (len(x_in), len(coord_names) ) )
     P = ChooseWaveformParams()
     for indx_out  in np.arange(len(x_in)):
         # WARNING UNUSUAL CONVENTION
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import os, sys
 import numpy as np
 from time import time
 from hashlib import md5
 
 from glue import pipeline
+import configparser
 
 __author__ = "Evan Ochsner <evano@gravity.phys.uwm.edu>, Chris Pankow <pankow@gravity.phys.uwm.edu>"
 
 # Taken from
 # http://pythonadventures.wordpress.com/2011/03/13/equivalent-of-the-which-command-in-python/
 def is_exe(fpath):
     return os.path.exists(fpath) and os.access(fpath, os.X_OK)
@@ -1926,15 +1927,15 @@
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
         print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
     return ile_job, ile_sub_name
 
 
-def write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight', exe=None, log_dir=None, ncopies=1,request_memory=8192,time_marg=True,pickle_file=None,posterior_file=None,universe='vanilla',**kwargs):
+def write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight', exe=None, log_dir=None, ncopies=1,request_memory=8192,time_marg=True,pickle_file=None,posterior_file=None,universe='vanilla',no_grid=False,ile_args=None,**kwargs):
     """
     Write a submit file for launching jobs to reweight final posterior samples due to calibration uncertainty 
 
     Inputs:
      - posterior samples, event pickle file (generated by Bilby)
     Outputs:
      - reweighted samples due to calibration uncertainty and corresponding weights
@@ -1968,15 +1969,33 @@
     ile_job.add_opt('data_dump_file', str(pickle_file))
     ile_job.add_opt('posterior_sample_file', str(posterior_file))
     ile_job.add_opt('number_of_calibration_curves', '100')
     ile_job.add_opt('reevaluate_likelihood', 'True')
     ile_job.add_opt('use_rift_samples', 'True')
     ile_job.add_opt('time_marginalization', str(time_marg))
 
-
+    lmax=None
+    if ile_args:
+        ile_args_split = ile_args.split('--')
+        fmin_list = []
+        fmin_template = None
+        for line in ile_args_split:
+            line_split = line.split()
+            if len(line_split)>1:
+                if line_split[0] == 'fmin-ifo':
+                    fmin_list += [line_split[1]]
+                if line_split[0] == 'fmin-template':
+                    fmin_template = line_split[1]
+                elif line_split[0] == 'l-max':
+                    lmax = int(line_split[1])
+#        fmin = np.min(fmin_list)
+        if fmin_template:
+            ile_job.add_arg(" --fmin-template {} ".format(fmin_template))  # code will fail without this, and it is always written anyways, but 
+        if lmax:
+            ile_job.add_arg(" --l-max {} ".format(lmax))
 
     #
     # Add normal arguments
     #
     for opt, param in list(kwargs.items()):
         if isinstance(param, list) or isinstance(param, tuple):
             # NOTE: Hack to get around multiple instances of the same option
@@ -1988,34 +2007,48 @@
             continue
         else:
             ile_job.add_opt(opt.replace("_", "-"), str(param))
 
     ile_job.add_condor_cmd('getenv', 'True')
     ile_job.add_condor_cmd('request_memory', str(request_memory))
 
+    # no grid
+    if no_grid:
+        ile_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        ile_job.add_condor_cmd("+flock_local",'true')
+
     # Write requirements
     ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
 
     try:
         ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
          print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
 
     return ile_job, ile_sub_name
 
-def write_bilby_pickle_sub(tag='Bilby_pickle', exe=None, universe='vanilla', log_dir=None, ncopies=1,request_memory=4096,bilby_ini_file=None,**kwargs):
+def bilby_prior_dict_string_from_mc_q(mc_range,dmax_Mpc):
+    out_str = """chirp-mass: bilby.gw.prior.UniformInComponentsChirpMass(minimum={}, maximum={}, name='chirp_mass', boundary=None), mass-ratio: bilby.gw.prior.UniformInComponentsMassRatio(minimum=0.05, maximum=1.0, name='mass_ratio', latex_label='$q$', unit=None, boundary=None), mass-1: Constraint(minimum=1, maximum=1000, name='mass_1', latex_label='$m_1$', unit=None), mass-2: Constraint(minimum=1, maximum=1000, name='mass_2', latex_label='$m_2$', unit=None), a-1: Uniform(minimum=0, maximum=0.99, name='a_1', latex_label='$a_1$', unit=None, boundary=None), a-2: Uniform(minimum=0, maximum=0.99, name='a_2', latex_label='$a_2$', unit=None, boundary=None), tilt-1: Sine(minimum=0, maximum=3.141592653589793, name='tilt_1'), tilt-2: Sine(minimum=0, maximum=3.141592653589793, name='tilt_2'), phi-12: Uniform(minimum=0, maximum=6.283185307179586, name='phi_12', boundary='periodic'), phi-jl: Uniform(minimum=0, maximum=6.283185307179586, name='phi_jl', boundary='periodic'), luminosity-distance: PowerLaw(alpha=2, minimum=10, maximum={}, name='luminosity_distance', latex_label='$d_L$', unit='Mpc', boundary=None), theta-jn: Sine(minimum=0, maximum=3.141592653589793, name='theta_jn'), psi: Uniform(minimum=0, maximum=3.141592653589793, name='psi', boundary='periodic'), phase: Uniform(minimum=0, maximum=6.283185307179586, name='phase', boundary='periodic'), dec: Cosine(name='dec'), ra: Uniform(name='ra', minimum=0, maximum=2 * np.pi, boundary='periodic')
+""".format(mc_range[0],mc_range[1],dmax_Mpc)
+    out_str = "{" + out_str.rstrip() + "}"
+    return out_str
+
+def write_bilby_pickle_sub(tag='Bilby_pickle', exe=None, universe='local', log_dir=None, ncopies=1,request_memory=4096,bilby_ini_file=None,no_grid=False,frames_dir=None,cache_file=None,ile_args=None,**kwargs):
     """
     Write a submit file for launching a job to generate a pickle file based off a bilby ini file; needed for  reweight final posterior samples due to calibration uncertainty
     
     Inputs:
      - bilby ini file
     Outputs:
      - pickle file of event settings; needed as input for calibration reweighting
+
+     Notes:
+       - local universe is generally safer: we need access to frame files in a standard location (typically datafind returns cvmfs, etc). That may not be available on remote nodes.
     """
     exe = exe or which("bilby_pipe_generation")
     if exe is None:
         print(" Pickle generation code unavailable. ")
         sys.exit(0)
     ile_job = pipeline.CondorDAGJob(universe=universe, executable=exe)
     # This is a hack since CondorDAGJob hides the queue property
@@ -2024,59 +2057,188 @@
     if universe=='local':
         requirements.append("IS_GLIDEIN=?=undefined")
 
 
     ile_sub_name = tag + '.sub'
     ile_job.set_sub_file(ile_sub_name)
 
-    # Add manual options for input, output
-    ile_job.add_opt('data-dump-file', str('bilby.pickle'))
-    ile_job.add_arg(str(bilby_ini_file)) # needs to be a bilby ini file for the particular event being analyzed
-
     #
     #Logging options
     #
     uniq_str = "$(macromassid)-$(cluster)-$(process)"
     ile_job.set_log_file("%s%s-%s.log" % (log_dir, tag, uniq_str))
     ile_job.set_stderr_file("%s%s-%s.err" % (log_dir, tag, uniq_str))
     ile_job.set_stdout_file("%s%s-%s.out" % (log_dir, tag, uniq_str))
 
 
+    # Add manual options for input, output.  Hopefully this all happens in order as needed, if not we will just concatenate
+    # 
+    ile_job.add_arg(str(bilby_ini_file)) # needs to be a bilby ini file for the particular event being analyzed
+    ile_job.add_arg(' --data-dump-file calmarg/data/calmarg_data_dump.pickle')
+
+    # Problem: bilby ini file may not have 'data-dict', in which case we need to backstop it with data from 'frames_dir' or 'cache_file'
+    # Problem: bilby ini file does not have sections.
+    # Workaround: https://stackoverflow.com/questions/2885190/using-configparser-to-read-a-file-without-section-name
+    config = configparser.ConfigParser()
+    config.optionxform=str # force preserve case! Important for --choose-data-LI-seglen
+    with open(bilby_ini_file) as stream:
+        config.read_string("[top]\n" + stream.read())
+        bilby_items = dict(config["top"])
+        ifo_list = list(bilby_items['channel-dict'])  # PSDs must be listed, implicitly provides all ifos
+    bilby_data_dict = {}
+    # remove entries with the None keyword, as misleading
+    dict_names = list(bilby_data_dict)
+    for name in dict_names:
+        if bilby_data_dict[name] == 'None':
+            del bilby_data_dict[name]
+    if not('data-dict' in bilby_items):
+        if cache_file:
+            print(" calmarg: bilby ini file does not have data_dict, attempting to identify data from (host) directory: {} ".format(frames_dir))
+            cache_lines = np.loadtxt(cache_file,dtype=str)
+            if len(cache_lines) > len(ifo_list):
+                raise Exception(" Pipeline failure: cache file must contain one line per IFO to identify files in this approach")
+            for indx in np.arange(len(cache_lines)):
+                ifo = cache_lines[indx][0]+"1"
+                bilby_data_dict[ifo] = cache_lines[indx][-1].replace('file://localhost','')
+        elif frames_dir:  # Danger : this directory might be EMPTY and generated at runtile
+            import glob
+            print(" calmarg: bilby ini file does not have data_dict, attempting to identify data from directory: {} ".format(frames_dir))
+            fnames_gwf = list(glob.glob(frames_dir+"/*.gwf")  )
+            # get dictionary matching files
+            for name in fnames_gwf:
+                this_frame_ifo = None
+                for ifo in ifo_list:
+                    if name.startswith(frames_dir+"/{}-".format(ifo)):
+                        this_frame_ifo=ifo
+                bilby_data_dict[ifo] = this_frame_ifo
+            if len(list(bilby_data_dict)) ==0 :
+                print("  Failed to find files in frames_dir, warning! ")
+        else:
+            print(" ==== WARNING FALLTHROUGH : calmarg attempting to identify correct frame files to use but falling back to 'magic' options from bilby ===")
+        # add to command-line arguments, IF NONEMPTY.  Otherwise we're stuck, and we have to hope magic works
+        if len(list(bilby_data_dict))>0:
+            data_argstr = '{}'.format(bilby_data_dict)
+            data_argstr = '  --data-dict ""{}""  '.format(data_argstr.replace(' ',''))  # double "" because we are in a condor submit script!  Annoying but seemt to be correct
+            ile_job.add_arg(data_argstr)
+        else:
+            print(" ==== WARNING FALLTHROUGH : calmarg failed to pull out options  ===",bilby_data_dict)
+
+
+    # Other required settings from ILE
+    # approximant: if ile_args present, ALWAYS parse it and set it that way, so we are consistent with our own analysis
+    if ile_args:
+        approx = bilby_items['waveform-approximant']
+        ile_args_split = ile_args.split('--')
+        start_time =None
+        end_time=None
+        trigger_time =None
+        rift_window_shape=None    # remember this is a dimensionless number, not a time
+        rift_srate =None
+        fmin_list = []
+        channel_list=[]
+        fmax=None
+        for line in ile_args_split:
+            line_split = line.split()
+            if len(line_split)>1:
+                if line_split[0]=='approx':
+                    approx = line_split[1]
+                elif line_split[0] == 'event-time':
+                    event_time = float(line_split[1])
+                elif line_split[0] == 'data-start-time':
+                    start_time = float(line_split[1])
+                elif line_split[0] == 'data-end-time':
+                    end_time = float(line_split[1])
+                elif line_split[0] == 'window-shape':
+                    rift_window_shape = float(line_split[1])
+                elif line_split[0] == 'srate':
+                    rift_srate = int(float(line_split[1]))  # safety
+                elif line_split[0] == 'fmin-ifo':
+                    fmin_list += [line_split[1]]
+                elif line_split[0] == 'fmax':
+                    fmax = int(float(line_split[1]))  # safety
+                elif line_split[0] == 'channel-name':
+                    channel_list += [line_split[1]]
+        ile_job.add_arg(" --waveform-approximant {} ".format(approx))
+        if rift_srate:
+            ile_job.add_arg(" --sampling-frequency {} ".format(rift_srate))
+        if event_time:
+            ile_job.add_arg(" --trigger-time {} ".format(event_time))
+        # t_tukey
+        t_tukey = (end_time-start_time)*rift_window_shape/2   # basically the fraction of time not in the window; see formula in helper
+        ile_job.add_arg(" --tukey-roll-off {} ".format(t_tukey))
+        # channel list
+        channel_dict ={}
+        for channel_id in channel_list:
+            if '=' in channel_id:
+                ifo, channel_name = channel_id.split('=')
+                channel_dict[ifo] = channel_name
+        channel_argstr = '{}'.format(channel_dict)
+        channel_argstr = '  --channel-dict ""{}""  '.format(channel_argstr.replace(' ',''))
+        ile_job.add_arg(channel_argstr)
+        # fmin
+        if len(fmin_list)>0:
+            fmin_dict = {}
+            for fmin_id in fmin_list:
+                if '=' in fmin_id:
+                    ifo, fmin = fmin_id.split('=')
+                    fmin_dict[ifo] = float(fmin)
+            fmin_argstr = '{}'.format(fmin_dict)
+            fmin_argstr = '  --minimum-frequency ""{}""  '.format(fmin_argstr.replace(' ',''))  # inside condor
+            ile_job.add_arg(fmin_argstr)
+            # fmax.  Use previous to get ifo list
+            if fmax:
+                fmax_dict = {}
+                for ifo in fmin_dict:
+                    fmax_dict[ifo] =fmax
+                fmax_argstr = '{}'.format(fmax_dict)
+                fmax_argstr = '  --maximum-frequency ""{}""  '.format(fmax_argstr.replace(' ',''))
+                ile_job.add_arg(fmax_argstr)
+
+    # Add outdir, label so we can control filename for output
+    ile_job.add_arg(" --outdir calmarg ")
+    ile_job.add_arg(" --label calmarg ")
 
     #
     # Add normal arguments
+    # Note these need to appear *after* the bilby ini file
     #
     for opt, param in list(kwargs.items()):
         if isinstance(param, list) or isinstance(param, tuple):
             # NOTE: Hack to get around multiple instances of the same option
             for p in param:
                 ile_job.add_arg("--%s %s" % (opt.replace("_", "-"), str(p)))
         elif param is True:
             ile_job.add_opt(opt.replace("_", "-"), None)
         elif param is None or param is False:
             continue
         else:
             ile_job.add_opt(opt.replace("_", "-"), str(param))
 
+
     ile_job.add_condor_cmd('getenv', 'True')
     ile_job.add_condor_cmd('request_memory', str(request_memory))
 
+    # no grid
+    if no_grid:
+        ile_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        ile_job.add_condor_cmd("+flock_local",'true')
+
     # Write requirements
     ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
 
     try:
         ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
          print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
 
     return ile_job, ile_sub_name
 
-def write_comov_distance_reweighting_sub(tag='Comov_dist', comov_distance_reweighting_exe=None, reweight_location=None, universe='vanilla', log_dir=None, ncopies=1,request_memory=4096,posterior_file=None,**kwargs):
+def write_comov_distance_reweighting_sub(tag='Comov_dist', comov_distance_reweighting_exe=None, reweight_location=None, universe='vanilla', log_dir=None, ncopies=1,request_memory=4096,posterior_file=None,no_grid=False,**kwargs):
     """
     Write a submit file for launching a job to generate reweight posterior samples to reflect a comoving distance prior
     
     Inputs:
      - posterior samples in h5 format
     Outputs:
      - reweighted samples in h5 format
@@ -2124,27 +2286,33 @@
             continue
         else:
             ile_job.add_opt(opt.replace("_", "-"), str(param))
 
     ile_job.add_condor_cmd('getenv', 'True')
     ile_job.add_condor_cmd('request_memory', str(request_memory))
 
+    # no grid
+    if no_grid:
+        ile_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        ile_job.add_condor_cmd("+flock_local",'true')
+
+
     # Write requirements
     ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
 
     try:
         ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
          print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
 
     return ile_job, ile_sub_name
 
-def write_convert_ascii_to_h5_sub(tag='Convert_ascii2h5', convert_ascii_to_h5_exe=None,output_file=None, universe='vanilla', log_dir=None, ncopies=1,request_memory=4096,posterior_file=None,**kwargs):
+def write_convert_ascii_to_h5_sub(tag='Convert_ascii2h5', convert_ascii_to_h5_exe=None,output_file=None, universe='vanilla', log_dir=None, ncopies=1,request_memory=4096,posterior_file=None,no_grid=False,**kwargs):
     """
     Converts posterior samples file from ascii to h5 format
     
     Inputs:
      - posterior samples in ascii format
     Outputs:
      - posterior samples in h5 format
@@ -2193,19 +2361,202 @@
             continue
         else:
             ile_job.add_opt(opt.replace("_", "-"), str(param))
 
     ile_job.add_condor_cmd('getenv', 'True')
     ile_job.add_condor_cmd('request_memory', str(request_memory))
 
+    # no grid
+    if no_grid:
+        ile_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        ile_job.add_condor_cmd("+flock_local",'true')
+
     # Write requirements
     ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
 
     try:
         ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
     except:
          print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
 
 
     return ile_job, ile_sub_name
 
+
+def write_hyperpost_sub(tag='HYPER', exe=None, input_net='all.marg_net',output='output-samples',universe="vanilla",out_dir=None,log_dir=None, ncopies=1,arg_str=None,request_memory=8192,arg_vals=None, no_grid=False,request_disk=False, transfer_files=None,transfer_output_files=None,use_singularity=False,use_osg=False,use_simple_osg_requirements=False,singularity_image=None,max_runtime_minutes=None,condor_commands=None,**kwargs):
+    """
+    Write a submit file for launching jobs to marginalize the likelihood over hyperparameters.
+    Almost identical to CIP 
+
+    Inputs:
+    Outputs:
+        - An instance of the CondorDAGJob that was generated for ILE
+    """
+
+    if use_singularity and (singularity_image == None)  :
+        print(" FAIL : Need to specify singularity_image to use singularity ")
+        sys.exit(0)
+    if use_singularity and (transfer_files == None)  :
+        print(" FAIL : Need to specify transfer_files to use singularity at present!  (we will append the prescript; you should transfer any PSDs as well as the grid file ")
+        sys.exit(0)
+
+
+    exe = exe or which("util_ConstructEOSPosterior.py")
+    if use_singularity:
+        path_split = exe.split("/")
+        print((" Executable: name breakdown ", path_split, " from ", exe))
+        singularity_base_exe_path = "/usr/bin/"  # should not hardcode this ...!
+        if 'SINGULARITY_BASE_EXE_DIR' in list(os.environ.keys()) :
+            singularity_base_exe_path = os.environ['SINGULARITY_BASE_EXE_DIR']
+        exe=singularity_base_exe_path + path_split[-1]
+        if path_split[-1] == 'true':  # special universal path for /bin/true, don't override it!
+            exe = "/usr/bin/true"
+    ile_job = pipeline.CondorDAGJob(universe=universe, executable=exe)
+    # This is a hack since CondorDAGJob hides the queue property
+    ile_job._CondorJob__queue = ncopies
+
+
+    # no grid
+    if no_grid:
+        ile_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        ile_job.add_condor_cmd("+flock_local",'true')
+
+    requirements=[]
+    if universe=='local':
+        requirements.append("IS_GLIDEIN=?=undefined")
+
+    ile_sub_name = tag + '.sub'
+    ile_job.set_sub_file(ile_sub_name)
+
+    #
+    # Add options en mass, by brute force
+    #
+    arg_str = arg_str.lstrip() # remove leading whitespace and minus signs
+    arg_str = arg_str.lstrip('-')
+    ile_job.add_opt(arg_str,'')  
+
+    ile_job.add_opt("fname", input_net)
+    ile_job.add_opt("fname-output-samples", out_dir+"/"+output)
+    ile_job.add_opt("fname-output-integral", out_dir+"/"+output)
+
+    #
+    # Macro based options.
+    #     - select EOS from list (done via macro)
+    #     - pass spectral parameters
+    #
+
+    #
+    # Logging options
+    #
+    uniq_str = "$(macroevent)-$(cluster)-$(process)"
+    ile_job.set_log_file("%s%s-%s.log" % (log_dir, tag, uniq_str))
+    ile_job.set_stderr_file("%s%s-%s.err" % (log_dir, tag, uniq_str))
+    ile_job.set_stdout_file("%s%s-%s.out" % (log_dir, tag, uniq_str))
+
+    if "fname_output_samples" in kwargs and kwargs["fname_output_samples"] is not None:
+        #
+        # Need to modify the output file so it's unique
+        #
+        ofname = kwargs["fname_output_samples"].split(".")
+        ofname, ext = ofname[0], ".".join(ofname[1:])
+        ile_job.add_file_opt("fname-output-samples", "%s-%s.%s" % (ofname, uniq_str, ext))
+
+    #
+    # Add normal arguments
+    # FIXME: Get valid options from a module
+    #
+    for opt, param in list(kwargs.items()):
+        if isinstance(param, list) or isinstance(param, tuple):
+            # NOTE: Hack to get around multiple instances of the same option
+            for p in param:
+                ile_job.add_arg("--%s %s" % (opt.replace("_", "-"), str(p)))
+        elif param is True:
+            ile_job.add_opt(opt.replace("_", "-"), None)
+        elif param is None or param is False:
+            continue
+        else:
+            ile_job.add_opt(opt.replace("_", "-"), str(param))
+
+    if not use_osg:
+        ile_job.add_condor_cmd('getenv', 'True')
+    ile_job.add_condor_cmd('request_memory', str(request_memory)) 
+    if not(request_disk is False):
+        ile_job.add_condor_cmd('request_disk', str(request_disk)) 
+    # To change interactively:
+    #   condor_qedit
+    # for example: 
+    #    for i in `condor_q -hold  | grep oshaughn | awk '{print $1}'`; do condor_qedit $i RequestMemory 30000; done; condor_release -all 
+
+    requirements = []
+    if use_singularity:
+        # Compare to https://github.com/lscsoft/lalsuite/blob/master/lalinference/python/lalinference/lalinference_pipe_utils.py
+        ile_job.add_condor_cmd('request_CPUs', str(1))
+        ile_job.add_condor_cmd('transfer_executable', 'False')
+        ile_job.add_condor_cmd("+SingularityBindCVMFS", 'True')
+        ile_job.add_condor_cmd("+SingularityImage", '"' + singularity_image + '"')
+        requirements.append("HAS_SINGULARITY=?=TRUE")
+
+    if use_osg:
+           # avoid black-holing jobs to specific machines that consistently fail. Uses history attribute for ad
+           ile_job.add_condor_cmd('periodic_release','(HoldReasonCode == 45) && (HoldReasonSubCode == 0)')
+           ile_job.add_condor_cmd('job_machine_attrs','Machine')
+           ile_job.add_condor_cmd('job_machine_attrs_history_length','4')
+#           for indx in [1,2,3,4]:
+#               requirements.append("TARGET.GLIDEIN_ResourceName=!=MY.MachineAttrGLIDEIN_ResourceName{}".format(indx))
+           if "OSG_DESIRED_SITES" in os.environ:
+               ile_job.add_condor_cmd('+DESIRED_SITES',os.environ["OSG_DESIRED_SITES"])
+           if "OSG_UNDESIRED_SITES" in os.environ:
+               ile_job.add_condor_cmd('+UNDESIRED_SITES',os.environ["OSG_UNDESIRED_SITES"])
+           # Some options to automate restarts, acts on top of RETRY in dag
+    if use_singularity or use_osg:
+            # Set up file transfer options
+           ile_job.add_condor_cmd("when_to_transfer_output",'ON_EXIT')
+
+           # Stream log info
+           if not ('RIFT_NOSTREAM_LOG' in os.environ):
+               ile_job.add_condor_cmd("stream_error",'True')
+               ile_job.add_condor_cmd("stream_output",'True')
+
+
+    ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
+
+    # Stream log info: always stream CIP error, it is a critical bottleneck
+    if True: # not ('RIFT_NOSTREAM_LOG' in os.environ):
+        ile_job.add_condor_cmd("stream_error",'True')
+        ile_job.add_condor_cmd("stream_output",'True')
+
+    try:
+        ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
+        ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
+    except:
+        print(" LIGO accounting information not available.  You must add this manually to integrate.sub !")
+        
+    
+    if not transfer_files is None:
+        if not isinstance(transfer_files, list):
+            fname_str=transfer_files
+        else:
+            fname_str = ','.join(transfer_files)
+        fname_str=fname_str.strip()
+        ile_job.add_condor_cmd('transfer_input_files', fname_str)
+        ile_job.add_condor_cmd('should_transfer_files','YES')
+
+    # Periodic remove: kill jobs running longer than max runtime
+    # https://stackoverflow.com/questions/5900400/maximum-run-time-in-condor
+    if not(max_runtime_minutes is None):
+        remove_str = 'JobStatus =?= 2 && (CurrentTime - JobStartDate) > ( {})'.format(60*max_runtime_minutes)
+        ile_job.add_condor_cmd('periodic_remove', remove_str)
+
+
+    ###
+    ### SUGGESTION FROM STUART (for later)
+    # request_memory = ifthenelse( (LastHoldReasonCode=!=34 && LastHoldReasonCode=!=26), InitialRequestMemory, int(1.5 * NumJobStarts * MemoryUsage) )
+    # periodic_release = ((HoldReasonCode =?= 34) || (HoldReasonCode =?= 26))
+    # This will automatically release a job that is put on hold for using too much memory with a 50% increased memory request each tim.e
+    if condor_commands is not None:
+        for cmd, value in condor_commands.iteritems():
+            ile_job.add_condor_cmd(cmd, value)
+
+
+    return ile_job, ile_sub_name
+
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,16 @@
 parser.add_argument("--force-chi-small-max",default=None,type=float,help="Provde this value to override the value of chi-max provided")
 parser.add_argument("--force-lambda-max",default=None,type=float,help="Provde this value to override the value of lambda-max provided")
 parser.add_argument("--force-lambda-small-max",default=None,type=float,help="Provde this value to override the value of lambda-small-max provided")
 parser.add_argument("--fmin-template",default=20,type=float,help="Minimum frequency for template. Used to estimate signal duration. If fmin not specified, also the minimum frequency for integration")
 parser.add_argument("--fmax",default=None,type=float,help="fmax. Use this ONLY if you want to override the default settings, which are set based on the PSD used")
 parser.add_argument("--data-start-time",default=None)
 parser.add_argument("--data-end-time",default=None,help="If both data-start-time and data-end-time are provided, this interval will be used.")
-parser.add_argument("--data-LI-seglen",default=None,type=float,help="If provided, use a buffer this long, placing the signal 2s after this, and try to use 0.4s tukey windowing on each side, to be consistent with LI.  ")
+parser.add_argument("--data-LI-seglen",default=None,type=float,help="If provided, use a buffer this long, placing the signal 2s after this, and try to use 0.4s tukey windowing on each side, to be consistent with LI.  Note next argument to change windowing")
+parser.add_argument("--data-tukey-window-time",default=0.4,type=float,help="The default amount of time (in seconds) during the turn-on phase of the tukey window. Note that for massive signals, the amount of unfiltered data is (seglen - 2s  - window_time), and can be as short as 1.6 s by default")
 parser.add_argument("--no-enforce-duration-bound",action='store_true',help="Allow user to perform LI-style behavior and reequest signals longer than the seglen. Argh, by request.")
 #parser.add_argument("--enforce-q-min",default=None,type=float,help='float.  If provided ,the grid will go down to this mass ratio. SEGMENT LENGTH WILL BE ADJUSTED')
 parser.add_argument("--working-directory",default=".")
 parser.add_argument("--datafind-exe",default="gw_data_find")
 parser.add_argument("--gracedb-exe",default="gracedb")
 parser.add_argument("--fake-data",action='store_true',help="If this argument is present, the channel names are overridden to FAKE_STRAIN")
 parser.add_argument("--cache",type=str,default=None,help="If this argument is present, the various routines will use the frame files in this cache. The user is responsible for setting this up")
@@ -995,15 +996,15 @@
         data_end_time = int(P.tref + 2)
         helper_ile_args += " --data-start-time " + str(data_start_time) + " --data-end-time " + str(data_end_time)  + " --inv-spec-trunc-time 0 --window-shape 0.01"
     if use_ini:
         T_window_raw = unsafe_config_get(config,['engine','seglen'])
         data_start_time = np.max([int(P.tref - T_window_raw -2 )  , data_start_time_orig])  # don't request data we don't have! 
         data_end_time = int(P.tref + 2)
         T_window = data_start_time - data_end_time
-        window_shape = 0.4*2/T_window
+        window_shape = opts.data_tukey_window_time*2/T_window  # make it clear that this is a one-sided interval
         helper_ile_args += " --data-start-time " + str(data_start_time) + " --data-end-time " + str(data_end_time)  + " --inv-spec-trunc-time 0 --window-shape " + str(window_shape)
 
 if not(internal_dmax is None):
     helper_ile_args +=  " --d-max " + str(int(internal_dmax))
     if opts.ile_distance_prior:
         helper_ile_args += " --d-prior {} ".format(opts.ile_distance_prior)   # moving here from pseudo_pipe
     if opts.internal_marginalize_distance and not(opts.internal_marginalize_distance_file):
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files 1% similar despite different names*

```diff
@@ -1032,48 +1032,48 @@
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+gridinit_job.get_sub_file()
         gridinit_job.set_sub_file(fname)
     gridinit_job.write_sub_file()
 
 if opts.calibration_reweighting:
     if opts.last_iteration_extrinsic_time_resampling and opts.bilby_pickle_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
     elif opts.last_iteration_extrinsic_time_resampling and opts.bilby_ini_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/bilby_defaults_output/data/"+opts.bilby_ini_file.split('/')[-1].split('.')[0]+"_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_ini_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/bilby_defaults_output/data/"+opts.bilby_ini_file.split('/')[-1].split('.')[0]+"_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_pickle_file:
-        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe)
+        calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
         
     calibration_job.set_log_file(opts.working_directory+"/calibration-$(cluster)-$(process).log")
     calibration_job.set_stderr_file(opts.working_directory+"/calibration-$(cluster)-$(process).err")
     calibration_job.set_stdout_file(opts.working_directory+"/calibration-$(cluster)-$(process).out")
     calibration_job.add_condor_cmd('request_disk',opts.general_request_disk)
 
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+calibration_job.get_sub_file()
         calibration_job.set_sub_file(fname)
     calibration_job.write_sub_file()
     
     if opts.bilby_ini_file:
-        pickle_job, pickle_job_name = dag_utils.write_bilby_pickle_sub(tag='Bilby_pickle',log_dir=None,bilby_ini_file=opts.bilby_ini_file,exe=opts.bilby_pickle_exe,universe=local_worker_universe)
+        pickle_job, pickle_job_name = dag_utils.write_bilby_pickle_sub(tag='Bilby_pickle',log_dir=None,bilby_ini_file=opts.bilby_ini_file,exe=opts.bilby_pickle_exe,universe='local',no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
         pickle_job.set_log_file(opts.working_directory+"/pickle-$(cluster)-$(process).log")
         pickle_job.set_stderr_file(opts.working_directory+"/pickle-$(cluster)-$(process).err")
         pickle_job.set_stdout_file(opts.working_directory+"/pickle-$(cluster)-$(process).out")
         pickle_job.add_condor_cmd('request_disk',opts.general_request_disk)
 
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+pickle_job.get_sub_file()
             pickle_job.set_sub_file(fname)
         pickle_job.write_sub_file()
 
 if opts.comov_distance_reweighting:
     if opts.calibration_reweighting:
         print(opts.convert_ascii2h5_exe)
-        convert_ascii_job, convert_ascii_job_name = dag_utils.write_convert_ascii_to_h5_sub(tag='Convert_ascii2h5',log_dir=None,output_file=opts.working_directory+"/posterior_samples.h5",posterior_file=opts.working_directory+"/reweighted_posterior_samples.dat",convert_ascii_to_h5_exe=opts.convert_ascii2h5_exe,universe=local_worker_universe)
+        convert_ascii_job, convert_ascii_job_name = dag_utils.write_convert_ascii_to_h5_sub(tag='Convert_ascii2h5',log_dir=None,output_file=opts.working_directory+"/posterior_samples.h5",posterior_file=opts.working_directory+"/reweighted_posterior_samples.dat",convert_ascii_to_h5_exe=opts.convert_ascii2h5_exe,universe=local_worker_universe,no_grid=no_worker_grid)
         convert_ascii_job.set_log_file(opts.working_directory+"/convert-ascii-$(cluster)-$(process).log")
         convert_ascii_job.set_stderr_file(opts.working_directory+"/convert_ascii-$(cluster)-$(process).err")
         convert_ascii_job.set_stdout_file(opts.working_directory+"/convert_ascii-$(cluster)-$(process).out")
         convert_ascii_job.add_condor_cmd('request_disk',opts.general_request_disk)
 
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+convert_ascii_job.get_sub_file()
@@ -1120,14 +1120,15 @@
 #      - if not iteration 0, grid should be in place (from previous stage)
 #      - Loop over events, make ILE node per event
 #      - create consolidate job, make it depend on all events in that iteration
 #      - create fit job, make it depend on consolidate job
 #    
 
 parent_fit_node = None
+last_node=None
 
 if opts.gridinit_args:
    grid_node = pipeline.CondorDAGNode(gridinit_job) 
    dag.add_node(grid_node)
    parent_fit_node = grid_node  # this must happen before the first ILE jobs
 
 convert_psd_node_list = []
@@ -1271,18 +1272,21 @@
         with open(fname_subdag_cip_args,'w') as f:
             f.write(cip_args_here)
         # Create dag inside directory, as usual,  pointing to existing run (note grid size issue problem)
         cmd = "create_event_parameter_pipeline_BasicIteration --use-full-submit-paths --first-iteration-jumpstart "  # we don't use overlap-grid-0.xml.gz !
         # note we will use subdags, and do this actively.  The 0th iteration needs a SPECIFIC grid though!
         cmd += " --ile-n-events-to-analyze {} --input-grid {} --ile-exe {} --ile-args {} ".format(opts.ile_n_events_to_analyze,opts.working_directory+"/overlap-grid-0.xml.gz".format(it),opts.ile_exe, opts.ile_args)
         cmd += " --cip-args {}/iteration_{}_cip/args_cip.txt ".format(opts.working_directory,it)
-        cmd += "  --convert-args {} ".format(opts.convert_args) # passthrough, important for tides
+        if opts.convert_args:
+            cmd += "  --convert-args {} ".format(opts.convert_args) # passthrough, important for tides
         cmd += " --n-samples-per-job {} ".format(opts.n_samples_per_job) 
         cmd += " --neff-threshold {} ".format(opts.neff_threshold)
         cmd += " --general-request-disk {} --ile-request-disk {} ".format(opts.general_request_disk,opts.ile_request_disk)
+        if opts.use_eccentricity:
+            cmd += " --use-eccentricity "
         if opts.cip_explode_jobs:
             cmd += " --cip-explode-jobs {} ".format(opts.cip_explode_jobs)
         if opts.cip_explode_jobs_dag:   # should be deafult
             cmd += " --cip-explode-jobs-dag "  
         if opts.request_gpu_ILE:
             cmd += " --request-gpu-ILE "  # DAG writer needs to make appropririate requests
         if opts.ile_retries:
@@ -1544,37 +1548,45 @@
 
             # Add nodes
             dag.add_node(convert_node)
             dag.add_node(resample_node)
    
     if not(opts.last_iteration_extrinsic_time_resampling):
         dag.add_node(cat_node)
+        last_node=cat_node
     else:
         dag.add_node(convert_node)   # this is the time resampling task
+        last_node=convert_node
 
 # Creating calibration uncertainty job
 if opts.calibration_reweighting:
     if opts.bilby_ini_file:
         pickle_node = pipeline.CondorDAGNode(pickle_job)
         pickle_node.add_macro("macroiteration",it)
         pickle_node.set_category("PICKLE")
+        pickle_node.add_parent(last_node)
+        last_node=pickle_node
         dag.add_node(pickle_node)
     calibration_node = pipeline.CondorDAGNode(calibration_job)
     calibration_node.add_macro("macroiteration",it)
     calibration_node.set_category("CALIBRATION")
+    calibration_node.add_parent(last_node)
     dag.add_node(calibration_node)
     
 if opts.comov_distance_reweighting:
     convert_ascii_node = pipeline.CondorDAGNode(convert_ascii_job)
     convert_ascii_node.add_macro("macroiteration",it)
     convert_ascii_node.set_category("CONVERT_ASCII")
+    convert_ascii_node.add_parent(last_node)
     dag.add_node(convert_ascii_node)
     distance_node = pipeline.CondorDAGNode(distance_job)
     distance_node.add_macro("macroiteration",it)
     distance_node.set_category("COMOV")
+    distance_node.add_parent(convert_ascii_node)
+    last_node=distance_node
     dag.add_node(distance_node)
 # Create final node for overall plots.  (Note: default setup is designed to enable plots of the last two iterations *at each step* but this seems like overkill)
 if plot_args:
         # Cannot run test on first iteration
         plot_node = pipeline.CondorDAGNode(plot_job)
         plot_node.add_macro("macroiteration", it)
         plot_node.add_macro("macroiterationlast", it-1)
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files 1% similar despite different names*

```diff
@@ -133,19 +133,25 @@
 def get_unpinned_params(opts, params):
     """
     Retrieve a set of unpinned parameters.
     """
     return params - set([p for p, v in opts.__dict__.items() if p in LIKELIHOOD_PINNABLE_PARAMS and v is not None])
 
 def zero_like(*args,**kwargs):
-  arg0 = kwargs['psi']
+  if len(kwargs)>0:
+    arg0 = kwargs['psi']
+  else:
+    arg0 = args[0]
   return xpy_default.zeros(len(arg0))
 
 def unit_like(*args,**kwargs):
-  arg0 = kwargs['psi']
+  if len(kwargs)>0:
+    arg0 = kwargs['psi']
+  else:
+    arg0 = args[0]
   return xpy_default.ones(len(arg0))
 
 #
 # Option parsing
 #
 
 optp = OptionParser()
@@ -301,19 +307,19 @@
 
 if opts.resample_time_marginalization:
   import scipy.special
 if opts.resample_time_marginalization and not(opts.fairdraw_extrinsic_output):
   raise Exception(" Resampled time output requires --fairdraw-extrinsic-output ")
 
 # Fairdraw is NOT YET IMPLEMENTED for these other integrators!
-if opts.fairdraw_extrinsic_output:
+#if opts.fairdraw_extrinsic_output:
 #  if opts.sampler_method == 'adaptive_cartesian_gpu':
 #    raise Exception(" Fairdraw not available  for this sampler")
-  if opts.sampler_method == 'GMM':
-    raise Exception(" Fairdraw not available  for this sampler")
+#  if opts.sampler_method == 'GMM':
+#    raise Exception(" Fairdraw not available  for this sampler")
 
 
 supplemental_ln_likelihood= None
 supplemental_ln_likelhood_prep=None
 supplemental_ln_likelhood_parsed_ini=None
 # Supplemental likelihood factor. Must have identical call sequence to 'likelihood_function'. Called with identical raw inputs (including cosines/etc)
 if opts.supplementary_likelihood_factor_code and opts.supplementary_likelihood_factor_function:
@@ -1050,14 +1056,16 @@
     for name in ['phi','theta', 'phiref','incl', 'psi','dist']:
       setattr(P,name, getattr(P,name).astype(float) )
 
   lnLt = factored_likelihood.DiscreteFactoredLogLikelihoodViaArrayVectorNoLoop(tvals,
                         P, lookupNKDict, rholmArrayDict, ctUArrayDict, ctVArrayDict,epochDict,Lmax=opts.l_max,xpy=xpy_default,return_lnLt=True)
 
   lnLt = identity_convert(lnLt) # back to CPU.  Note we have removed offsets 
+  if opts.zero_likelihood:
+    lnLt =np.zeros(lnLt.shape)  # zero likelihood
   lnLt_norm = scipy.special.logsumexp(lnLt,axis=-1)
   tvals = identity_convert(tvals) # back to CPU
 #  print(lnLt.shape, lnLt_norm.shape,tvals.shape)
   # Loop over and resample in time, picking index according to weights
   t_out = np.zeros(n_samples)
   lnL_out = np.zeros(n_samples)
   indx_list =np.arange(len(tvals))
@@ -1428,15 +1436,15 @@
                   # rotate phase if needed
                   # make copies of arrays
                   #   Sampling assumes P.phiref == phi+ \psi ,   P.psi == phi - psi
                   if opts.internal_rotate_phase:
                     phi_orb_true = (P.phiref + P.psi)/2.
                     psi_true = (P.phiref - P.psi)/2.
                     P.psi= psi_true
-                    P.phi = phi_orb_true
+                    P.phiref = phi_orb_true
 
                   lnL = factored_likelihood.DiscreteFactoredLogLikelihoodViaArrayVectorNoLoop(tvals,
                     P, lookupNKDict, rholmArrayDict, ctUArrayDict, ctVArrayDict,epochDict,Lmax=opts.l_max,xpy=xpy_default, loglikelihood=distmarg_loglikelihood)
 #                  nEvals +=len(right_ascension)
                   if supplemental_ln_likelihood:
                     lnL += supplemental_ln_likelihood(P.phi, P.theta, P.phiref ,P.incl, P.psi, 0,xpy=xpy_default) # Same API
                   if return_lnL:
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 import pickle
 
 import bilby
 import bilby_pipe
 
 # So I can import the RIFT source while not making this some setup.py-able package
 # TODO this should not be a hardcoded path!
-sys.path.append('/home/ethan.payne/code_libraries/generic-calibration-reweighting')
-import rift_source
+
+import RIFT.calmarg.rift_source as rift_source
 
 parser = argparse.ArgumentParser(description='calibration marginalization via reweighting of posterior samples')
 parser.add(
     "--posterior_sample_file", default=None,
     help="Bilby result file or text file with posterior samples to reweight")
 parser.add(
     "--data_dump_file", default=None,
@@ -81,14 +81,15 @@
 parser.add(
     "--time_marginalization_interval", default=0.1, type=float,
     help="Interval over which the time marginalization is undertaken")
 parser.add(
     "--use_rift_samples", type=bool, default=False,
     help="Uses a different waveform function if using RIFT samples. This matches the phase definitions in RIFT")
 parser.add("--fmin", default=None, type=float)
+parser.add("--l-max", default=4, type=int)
 parser.add("--start_index", default=None, type=int)
 parser.add("--end_index", default=None, type=int)
 
 args = parser.parse_args()
 
 with open(args.data_dump_file, "rb") as data_file:
     data = pickle.load(data_file)
@@ -111,15 +112,15 @@
             end_index = len(result.posterior)
     result.posterior = result.posterior.iloc[start_index:end_index].reset_index(drop=True)
     result.meta_data = {}
 
     if args.use_rift_samples:
         key_swap_dict = {'m1':'mass_1', 'm2':'mass_2', 'a1x':'spin_1x', 'a1y':'spin_1y', 'a1z':'spin_1z',
             'a2x':'spin_2x', 'a2y':'spin_2y', 'a2z':'spin_2z', 'incl':'iota', 'time':'geocent_time',
-            'phiorb':'phase', 'p':'log_prior', 'distance':'luminosity_distance'}
+        'phiorb':'phase', 'p':'log_prior', 'distance':'luminosity_distance', 'lambda1':'lambda_1', 'lambda2':'lambda_2'}
 
         for old_key in result.posterior.keys():
             if old_key in key_swap_dict:
                 result.posterior[key_swap_dict[old_key]] = result.posterior[old_key]
                 del result.posterior[old_key]
 
 outdir = os.path.dirname(os.path.abspath(args.posterior_sample_file))
@@ -146,16 +147,16 @@
 waveform_arguments = dict(
     reference_frequency=data.meta_data['command_line_args']['reference_frequency'],
     minimum_frequency=args.fmin,
     waveform_approximant=data.meta_data['command_line_args']['waveform_approximant'],
     sampling_frequency=ifos.sampling_frequency)
 
 if args.use_rift_samples:
-    waveform_arguments['Lmax'] = 4
-    waveform_arguments['waveform_approximant'] = 'SEOBNRv4PHM'
+    waveform_arguments['Lmax'] = args.l_max
+#    waveform_arguments['waveform_approximant'] = 'SEOBNRv4PHM'
     wf_func = rift_source.RIFT_lal_binary_black_hole
 else:
     wf_func = eval('bilby.gw.source.'+data.meta_data['command_line_args']['frequency_domain_source_model'])
 
 waveform_generator = bilby.gw.waveform_generator.WaveformGenerator(
             frequency_domain_source_model=wf_func,
             sampling_frequency=ifos.sampling_frequency,
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 parser.add_argument("--hierarchical-merger-prior-1g",action='store_true',help="As in 1903.06742")
 parser.add_argument("--hierarchical-merger-prior-2g",action='store_true',help="As in 1903.06742")
 parser.add_argument("--link-reference-pe",action='store_true',help="If present, creates a directory 'reference_pe' and adds symbolic links to fiducial samples. These can be used by the automated plotting code.  Requires LVC_PE_SAMPLES environment variable defined!")
 parser.add_argument("--link-reference-psds",action='store_true',help="If present, uses the varialbe LVC_PE_CONFIG to find a 'reference_pe_config_map.dat' file, which provides the location for reference PSDs.  Will override PSDs used / setup by default")
 parser.add_argument("--make-bw-psds",action='store_true',help='If present, adds nodes to create BW PSDs to the dag.  If at all possible, avoid this and re-use existing PSDs')
 parser.add_argument("--link-bw-psds",action='store_true',help='If present, uses the script retrieve_bw_psd_for_event.sh  to find a precomputed BW psd, and convert it to our format')
 parser.add_argument("--use-online-psd",action='store_true', help="If present, will use the online PSD estimates")
+parser.add_argument("--ile-copies",default=1,type=int)
 parser.add_argument("--ile-retries",default=3,type=int)
 parser.add_argument("--general-retries",default=3,type=int)
 parser.add_argument("--ile-runtime-max-minutes",default=None,type=int,help="If not none, kills ILE jobs that take longer than the specified integer number of minutes. Do not use unless an expert")
 parser.add_argument("--fit-save-gp",action="store_true",help="If true, pass this argument to CIP. GP plot for each iteration will be saved. Useful for followup investigations or reweighting. Warning: lots of disk space (1G or so per iteration)")
 parser.add_argument("--cip-explode-jobs",type=int,default=None)
 parser.add_argument("--cip-explode-jobs-last",type=int,default=None,help="Number of jobs to use in last stage.  Hopefully in future auto-set")
 parser.add_argument("--cip-explode-jobs-auto",action='store_true',help="Auto-select --cip-explode-jobs based on SNR. Changes both cip-explode-jobs and cip-explode-jobs-last")
@@ -243,15 +244,14 @@
 parser.add_argument("--condor-nogrid-nonworker",action='store_true',help="NOW STANDARD, auto-set if you pass use-osg   Causes flock_local for 'internal' jobs")
 parser.add_argument("--use-osg-simple-requirements",action='store_true',help="Provide this option if job should use a more aggressive setting for OSG matching ")
 parser.add_argument("--archive-pesummary-label",default=None,help="If provided, creates a 'pesummary' directory and fills it with this run's final output at the end of the run")
 parser.add_argument("--archive-pesummary-event-label",default="this_event",help="Label to use on the pesummary page itself")
 opts=  parser.parse_args()
 
 
-
 if (opts.use_ini):
     # Attempt to lazy-parse all command line arguments from ini file
     config = ConfigParser.ConfigParser()
     config.optionxform=str # force preserve case! Important for --choose-data-LI-seglen
     config.read(opts.use_ini)
     if 'rift-pseudo-pipe' in config:
         # get the list of items
@@ -278,14 +278,17 @@
                 print(" ini file parser (overrides command line, except booleans): ",item, rift_items[item])
                 if val != "":
                     config_dict[item_renamed] = eval(rift_items[item])
                 else:
                     config_dict[item_renamed] = True
         print(config_dict)
 
+if opts.ile_copies <=0:
+    raise Exception(" Must have 1 or more ILE instances per intrinsic point")
+
 if opts.internal_loud_signal_mitigation_suite:
     opts.internal_ile_freezeadapt=False  # make sure to adapt every iteration, and adapt in distance if present
     opts.internal_ile_sky_network_coordinates=True # skymap is better
     opts.internal_ile_rotate_phase = True  # phase coordinates can be sharper
 
 # Default prior for aligned analysis should be z prior !
 if opts.assume_nonprecessing or opts.approx == "IMRPhenomD":
@@ -588,21 +591,21 @@
     cmd+= " --internal-ile-use-lnL "
 if opts.internal_cip_use_lnL:
     cmd += " --internal-cip-use-lnL "
 
 if not(opts.ile_n_eff is None):
     cmd += " --ile-n-eff {} ".format(opts.ile_n_eff)
 if opts.limit_mc_range:
-    cmd+= " --limit-mc-range {} ".format(opts.limit_mc_range)
+    cmd+= " --limit-mc-range  " + str(opts.limit_mc_range).replace(' ','')
 if not(opts.force_mc_range is None):
-    cmd+= " --force-mc-range {} ".format(opts.force_mc_range)
+    cmd+= " --force-mc-range  " + str(opts.force_mc_range).replace(' ','')
 elif opts.scale_mc_range:
-    cmd += " --scale-mc-range {} ".format(opts.scale_mc_range)
+    cmd += " --scale-mc-range  " + str(opts.scale_mc_range).replace(' ','')
 if not(opts.force_eta_range is None):
-    cmd+= " --force-eta-range {} ".format(opts.force_eta_range)
+    cmd+= " --force-eta-range  " + str(opts.force_eta_range).replace(' ','')
 if opts.force_chi_max:
     cmd+= " --force-chi-max {} ".format(opts.force_chi_max)
 if opts.force_chi_small_max:
     cmd+= " --force-chi-small-max {} ".format(opts.force_chi_small_max)
 if opts.force_lambda_max:
     cmd+= " --force-lambda-max {} ".format(opts.force_lambda_max)
 if opts.force_lambda_small_max:
@@ -1078,15 +1081,15 @@
 if opts.cip_fit_method == 'rf':
     cip_mem = 15000  # more typical for long-duration single-worker runs
 if opts.cip_fit_method =='quadratic' or opts.cip_fit_method =='polynomial':  # much lower memory requirement
     cip_mem = 4000
 cepp = "create_event_parameter_pipeline_BasicIteration"
 if opts.use_subdags:
     cepp = "create_event_parameter_pipeline_AlternateIteration"
-cmd =cepp+ "  --ile-n-events-to-analyze {} --input-grid proposed-grid.xml.gz --ile-exe  `which integrate_likelihood_extrinsic_batchmode`   --ile-args `pwd`/args_ile.txt --cip-args-list args_cip_list.txt --test-args args_test.txt --request-memory-CIP {} --request-memory-ILE 4096 --n-samples-per-job ".format(n_jobs_per_worker,cip_mem) + str(npts_it) + " --working-directory `pwd` --n-iterations " + str(n_iterations) + " --n-iterations-subdag-max {} ".format(opts.internal_n_iterations_subdag_max) + "  --n-copies 1" + "   --ile-retries "+ str(opts.ile_retries) + " --general-retries " + str(opts.general_retries)
+cmd =cepp+ "  --ile-n-events-to-analyze {} --input-grid proposed-grid.xml.gz --ile-exe  `which integrate_likelihood_extrinsic_batchmode`   --ile-args `pwd`/args_ile.txt --cip-args-list args_cip_list.txt --test-args args_test.txt --request-memory-CIP {} --request-memory-ILE 4096 --n-samples-per-job ".format(n_jobs_per_worker,cip_mem) + str(npts_it) + " --working-directory `pwd` --n-iterations " + str(n_iterations) + " --n-iterations-subdag-max {} ".format(opts.internal_n_iterations_subdag_max) + "  --n-copies {} ".format(opts.ile_copies) + "   --ile-retries "+ str(opts.ile_retries) + " --general-retries " + str(opts.general_retries)
 if opts.assume_matter or opts.assume_eccentric:
     cmd +=  " --convert-args `pwd`/helper_convert_args.txt "
 if not(opts.ile_runtime_max_minutes is None):
     cmd += " --ile-runtime-max-minutes {} ".format(opts.ile_runtime_max_minutes)
 if not(opts.internal_use_amr) or opts.internal_use_amr_puff:
     cmd+= " --puff-exe `which util_ParameterPuffball.py` --puff-cadence 1 --puff-max-it " + str(puff_max_it)+ " --puff-args `pwd`/args_puff.txt "
 if opts.assume_eccentric:
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 #! /usr/bin/env python
 #
-# GOAL
-#   - load in lnL data
-#   - fit peak to quadratic (standard), GP, etc. 
-#   - pass as input to mcsampler, to generate posterior samples
-#
-# FORMAT
-#   - pankow simplification of standard format
-#
-# COMPARE TO
-#   util_NRQuadraticFit.py
-#   postprocess_1d_cumulative
-#   util_QuadraticMassPosterior.py
-#
+#  util_ConstructEOSPosterior.py
+#     - takes in *generic-format* hyperparameter likelihood data
+#     - uses *uniform* prior on hyperparameters.  [non-uniform priors can  be applied by the user with a supplementary function]
+#     - generates posterior distribution by weighted Monte Carlo
 #
 # EXAMPLE:
 #   python `which util_ConstructEOSPosterior.py` --fname fake_int_grid.dat  --parameter gamma1 --parameter gamma2 --lnL-offset 50
 
 import RIFT.interpolators.BayesianLeastSquares as BayesianLeastSquares
 
 import argparse
 import sys
 import numpy as np
 import numpy.lib.recfunctions
 import scipy
 import scipy.stats
-import RIFT.lalsimutils as lalsimutils
-import lalsimulation as lalsim
-import lalframe
-import lal
 import functools
 import itertools
 
 import joblib  # http://scikit-learn.org/stable/modules/model_persistence.html
 
 no_plots = True
 internal_dtype = np.float32  # only use 32 bit storage! Factor of 2 memory savings for GP code in high dimensions
 
-C_CGS=2.997925*10**10 # Argh, Monica!
  
 try:
     import matplotlib.pyplot as plt
     from mpl_toolkits.mplot3d import Axes3D
     import matplotlib.lines as mlines
     import corner
 
@@ -62,88 +48,15 @@
 from ligo.lw import lsctables, utils, ligolw
 lsctables.use_in(ligolw.LIGOLWContentHandler)
 
 import RIFT.integrators.mcsampler as mcsampler
 
 
 
-def render_coord(x):
-    if x in lalsimutils.tex_dictionary.keys():
-        return lalsimutils.tex_dictionary[x]
-    if 'product(' in x:
-        a=x.replace(' ', '') # drop spaces
-        a = a[:len(a)-1] # drop last
-        a = a[8:]
-        terms = a.split(',')
-        exprs =map(render_coord, terms)
-        exprs = map( lambda x: x.replace('$', ''), exprs)
-        my_label = ' '.join(exprs)
-        return '$'+my_label+'$'
-    else:
-        return x
-
-def render_coordinates(coord_names):
-    return map(render_coord, coord_names)
-
 
-def extract_combination_from_LI(samples_LI, p):
-    """
-    extract_combination_from_LI
-      - reads in known columns from posterior samples
-      - for selected known combinations not always available, it will compute them from standard quantities
-    """
-    if p in samples_LI.dtype.names:  # e.g., we have precomputed it
-        return samples_LI[p]
-    if p in remap_ILE_2_LI.keys():
-       if remap_ILE_2_LI[p] in samples_LI.dtype.names:
-         return samples_LI[ remap_ILE_2_LI[p] ]
-    # Return cartesian components of spin1, spin2.  NOTE: I may already populate these quantities in 'Add important quantities'
-    if p == 'chiz_plus':
-        print(" Transforming ")
-        if 'a1z' in samples_LI.dtype.names:
-            return (samples_LI['a1z']+ samples_LI['a2z'])/2.
-        if 'theta1' in samples_LI.dtype.names:
-            return (samples_LI['a1']*np.cos(samples_LI['theta1']) + samples_LI['a2']*np.cos(samples_LI['theta2']) )/2.
-#        return (samples_LI['a1']+ samples_LI['a2'])/2.
-    if p == 'chiz_minus':
-        print(" Transforming ")
-        if 'a1z' in samples_LI.dtype.names:
-            return (samples_LI['a1z']- samples_LI['a2z'])/2.
-        if 'theta1' in samples_LI.dtype.names:
-            return (samples_LI['a1']*np.cos(samples_LI['theta1']) - samples_LI['a2']*np.cos(samples_LI['theta2']) )/2.
-#        return (samples_LI['a1']- samples_LI['a2'])/2.
-    if  'theta1' in samples_LI.dtype.names:
-        if p == 's1x':
-            return samples_LI["a1"]*np.sin(samples_LI[ 'theta1']) * np.cos( samples_LI['phi1'])
-        if p == 's1y' :
-            return samples_LI["a1"]*np.sin(samples_LI[ 'theta1']) * np.sin( samples_LI['phi1'])
-        if p == 's2x':
-            return samples_LI["a2"]*np.sin(samples_LI[ 'theta2']) * np.cos( samples_LI['phi2'])
-        if p == 's2y':
-            return samples_LI["a2"]*np.sin(samples_LI[ 'theta2']) * np.sin( samples_LI['phi2'])
-        if p == 'chi1_perp' :
-            return samples_LI["a1"]*np.sin(samples_LI[ 'theta1']) 
-        if p == 'chi2_perp':
-            return samples_LI["a2"]*np.sin(samples_LI[ 'theta2']) 
-    if 'lambdat' in samples_LI.dtype.names:  # LI does sampling in these tidal coordinates
-        lambda1, lambda2 = lalsimutils.tidal_lambda_from_tilde(samples_LI["m1"], samples_LI["m2"], samples_LI["lambdat"], samples_LI["dlambdat"])
-        if p == "lambda1":
-            return lambda1
-        if p == "lambda2":
-            return lambda2
-    if p == 'delta' or p=='delta_mc':
-        return (samples_LI['m1']  - samples_LI['m2'])/((samples_LI['m1']  + samples_LI['m2']))
-    # Return cartesian components of Lhat
-    if p == 'product(sin_beta,sin_phiJL)':
-        return np.sin(samples_LI[ remap_ILE_2_LI['beta'] ]) * np.sin(  samples_LI['phi_jl'])
-    if p == 'product(sin_beta,cos_phiJL)':
-        return np.sin(samples_LI[ remap_ILE_2_LI['beta'] ]) * np.cos(  samples_LI['phi_jl'])
-
-    print(" No access for parameter ", p)
-    return np.zeros(len(samples_LI['m1']))  # to avoid causing a hard failure
 
 def add_field(a, descr):
     """Return a new array that is like "a", but has additional fields.
 
     Arguments:
       a     -- a structured numpy array
       descr -- a numpy type description of the new fields
@@ -170,24 +83,24 @@
     b = numpy.empty(a.shape, dtype=a.dtype.descr + descr)
     for name in a.dtype.names:
         b[name] = a[name]
     return b
 
 
 parser = argparse.ArgumentParser()
-parser.add_argument("--fname",help="filename of *.dat file [EOS table: int_res gamma1 gamma2 ...]")
-parser.add_argument("--fname-output-samples",default="output-EOS-samples",help="output posterior samples (default output-ILE-samples -> output-ILE)")
+parser.add_argument("--fname",help="filename of *.dat file (EOS-format: lnL sigma_lnL p1 p2 ... .  ASSUME any stacking over events already performed.")
+parser.add_argument("--fname-output-samples",default="output-EOS-samples",help="output grid")
+parser.add_argument("--fname-output-integral",default="output-EOS-samples",help="for evidencees and pipeline compatibility")
 parser.add_argument("--n-output-samples",default=2000,type=int,help="output posterior samples (default 3000)")
 parser.add_argument("--eos-param", type=str, default=None, help="parameterization of equation of state [spectral only, for now]")
-parser.add_argument("--parameter", action='append', help="Parameters used as fitting parameters AND varied at a low level to make a posterior. Currently can only specify gamma1,gamma2, ..., and these MUST be columns in --fname")
-parser.add_argument("--parameter-implied", action='append', help="Parameter used in fit, but not independently varied for Monte Carlo")
+parser.add_argument("--parameter", action='append', help="Parameters used as fitting parameters AND varied at a low level to make a posterior. Currently can only specify gamma1,gamma2, ..., and these MUST be columns in --fname. IF NOT PROVIDED, DEFAULTS TO LIST IN FILE.  ")
+parser.add_argument("--parameter-implied", action='append', help="Parameter used in fit, but not independently varied for Monte Carlo. For EOS objects, only possible for physical quantities like R1.4, etc. NOT YET PROVIDED")
 #parser.add_argument("--no-adapt-parameter",action='append',help="Disable adaptive sampling in a parameter. Useful in cases where a parameter is not well-constrained, and the a prior sampler is well-chosen.")
-parser.add_argument("--parameter-nofit", action='append', help="Parameter used to initialize the implied parameters, and varied at a low level, but NOT the fitting parameters")
-parser.add_argument("--trust-sample-parameter-box",action='store_true', help="If used, sets the prior range to the SAMPLE range for any parameters. NOT IMPLEMENTED. This should be automatically done for mc!")
-parser.add_argument("--plots-do-not-force-large-range",action='store_true', help = "If used, the plots do NOT automatically set the chieff range to [-1,1], the eta range to [0,1/4], etc")
+parser.add_argument("--parameter-nofit", action='append', help="Parameter used to initialize the implied parameters, and varied at a low level, but NOT the fitting parameters.")
+parser.add_argument("--integration-parameter-range",action='append', help="Integration parameter ranges. Syntax is name:[a,b]")
 parser.add_argument("--downselect-parameter",action='append', help='Name of parameter to be used to eliminate grid points ')
 parser.add_argument("--downselect-parameter-range",action='append',type=str)
 parser.add_argument("--no-downselect",action='store_true')
 parser.add_argument("--aligned-prior", default="uniform",help="Options are 'uniform', 'volumetric', and 'alignedspin-zprior'")
 parser.add_argument("--cap-points",default=-1,type=int,help="Maximum number of points in the sample, if positive. Useful to cap the number of points ued for GP. See also lnLoffset. Note points are selected AT RANDOM")
 parser.add_argument("--lambda-max", default=4000,type=float,help="Maximum range of 'Lambda' allowed.  Minimum value is ZERO, not negative.")
 parser.add_argument("--lnL-shift-prevent-overflow",default=None,type=float,help="Define this quantity to be a large positive number to avoid overflows. Note that we do *not* define this dynamically based on sample values, to insure reproducibility and comparable integral results. BEWARE: If you shift the result to be below zero, because the GP relaxes to 0, you will get crazy answers.")
@@ -197,32 +110,41 @@
 parser.add_argument("--ignore-errors-in-data",action='store_true',help='Ignore reported error in lnL. Helpful for testing purposes (i.e., if the error is zero)')
 parser.add_argument("--lnL-peak-insane-cut",type=float,default=np.inf,help="Throw away lnL greater than this value. Should not be necessary")
 parser.add_argument("--verbose", action="store_true",default=False, help="Required to build post-frame-generating sanity-test plots")
 parser.add_argument("--save-plots",default=False,action='store_true', help="Write plots to file (only useful for OSX, where interactive is default")
 parser.add_argument("--n-max",default=3e5,type=float)
 parser.add_argument("--n-eff",default=3e3,type=int)
 parser.add_argument("--pool-size",default=3,type=int,help="Integer. Number of GPs to use (result is averaged)")
+parser.add_argument("--fit-method",default="rf",help="rf (default) : rf|gp|quadratic|polynomial|gp_hyper|gp_lazy|cov|kde.  Note 'polynomial' with --fit-order 0  will fit a constant")
 parser.add_argument("--fit-load-gp",default=None,type=str,help="Filename of GP fit to load. Overrides fitting process, but user MUST correctly specify coordinate system to interpret the fit with.  Does not override loading and converting the data.")
 parser.add_argument("--fit-save-gp",default=None,type=str,help="Filename of GP fit to save. ")
 parser.add_argument("--fit-order",type=int,default=2,help="Fit order (polynomial case: degree)")
 parser.add_argument("--no-plots",action='store_true')
-parser.add_argument("--using-eos", type=str, default=None, help="Name of EOS if not already determined in lnL")
+parser.add_argument("--using-eos-type", type=str, default=None, help="Name of EOS parameterization (must match what is used for inputs). Will use EOS parameterization to identify appropriate field headers")
+parser.add_argument("--sampler-method",default="adaptive_cartesian",help="adaptive_cartesian|GMM|adaptive_cartesian_gpu")
+parser.add_argument("--internal-use-lnL",action='store_true',help="integrator internally manipulates lnL. ")
+parser.add_argument("--internal-correlate-parameters",default=None,type=str,help="comman-separated string indicating parameters that should be sampled allowing for correlations. Must be sampling parameters. Only implemented for gmm.  If string is 'all', correlate *all* parameters")
+parser.add_argument("--internal-n-comp",default=1,type=int,help="number of components to use for GMM sampling. Default is 1, because we expect a unimodal posterior in well-adapted coordinates.  If you have crappy coordinates, use more")
+parser.add_argument("--force-no-adapt",action='store_true',help="Disable adaptation, both of the tempering exponent *and* the individual sampling prior(s)")
+parser.add_argument("--tripwire-fraction",default=0.05,type=float,help="Fraction of nmax of iterations after which n_eff needs to be greater than 1+epsilon for a small number epsilon")
+
+# Supplemental likelihood factors: convenient way to effectively change the mass/spin prior in arbitrary ways for example
+# Note this supplemental factor is passed the *fitting* arguments, directly.  Use with extreme caution, since we often change the dimension in a DAG 
+parser.add_argument("--supplementary-likelihood-factor-code", default=None,type=str,help="Import a module (in your pythonpath!) containing a supplementary factor for the likelihood.  Used to impose supplementary external priors of arbitrary complexity and external dependence (e.g., imposing alternate EOS priors)")
+parser.add_argument("--supplementary-likelihood-factor-function", default=None,type=str,help="With above option, specifies the specific function used as an external likelihood. EXPERTS ONLY")
+parser.add_argument("--supplementary-likelihood-factor-ini", default=None,type=str,help="With above option, specifies an ini file that is parsed (here) and passed to the preparation code, called when the module is first loaded, to configure the module. EXPERTS ONLY")
 opts=  parser.parse_args()
 no_plots = no_plots |  opts.no_plots
 lnL_shift = 0
+lnL_default_large_negative = -500
 if opts.lnL_shift_prevent_overflow:
     lnL_shift  = opts.lnL_shift_prevent_overflow
 
 
 
-with open('args.txt','w') as fp:
-    import sys
-    fp.write(' '.join(sys.argv))
-
-###
 ### Comparison data (from LI)
 ###
 
 downselect_dict = {}
 dlist = []
 dlist_ranges=[]
 if opts.downselect_parameter:
@@ -239,72 +161,124 @@
 if opts.no_downselect:
     downselect_dict={}
 
 
 test_converged={}
 
 ###
+### Retrieve data
+###
+#  int_sig sigma/L gamma1 gamma2 ...
+col_lnL = 0
+dat_orig = dat = np.loadtxt(opts.fname)
+dat_orig = dat[dat[:,col_lnL].argsort()] # sort  http://stackoverflow.com/questions/2828059/sorting-arrays-in-numpy-by-column
+print(" Original data size = ", len(dat), dat.shape)
+dat_orig_names = None
+with open(opts.fname,'r') as f:
+    header_str = f.readline()
+    header_str = header_str.rstrip()
+dat_orig_names = header_str.replace('#','').split()[2:]
+
+###
 ### Parameters in use
 ###
 
 coord_names = opts.parameter # Used  in fit
 if coord_names is None:
-    coord_names = []
+    coord_names = dat_orig_names
 low_level_coord_names = coord_names # Used for Monte Carlo
 if opts.parameter_implied:
     coord_names = coord_names+opts.parameter_implied
 if opts.parameter_nofit:
     if opts.parameter is None:
         low_level_coord_names = opts.parameter_nofit # Used for Monte Carlo
     else:
         low_level_coord_names = opts.parameter+opts.parameter_nofit # Used for Monte Carlo
 error_factor = len(coord_names)
+name_index_dict ={}
+for name in dat_orig_names:
+    try:
+        name_index_dict[name] = 2+dat_orig_names.index(name)
+    except:
+        raise Exception(" Currently fitting parameter names must match columns in data file ")
 # TeX dictionary
-#tex_dictionary = lalsimutils.tex_dictionary
-print(" Coordinate names for fit :, ", coord_names)
+print(" Coordinate names for fit :, ", coord_names, " from ", dat_orig_names, " indexed as ", name_index_dict)
 print(" Coordinate names for Monte Carlo :, ", low_level_coord_names)
-#print " Rendering coordinate names : ", map(lambda x: tex_dictionary[x], low_level_coord_names)
 
 
 ###
-### Prior functions : a dictionary
+### Integration ranges
 ###
 
-def eos_param_uniform_prior(x):
+param_ranges = {}
+for range_code  in opts.integration_parameter_range:
+    name, range_str  = range_code.split(':')
+    range_expr =     eval(range_str)  # define. Better to split on , for example
+    param_ranges[name]  = range_expr
+
+# Add in integration range for everything else, if nothing specified
+for name in dat_orig_names:
+    if not name in param_ranges:
+        vals = dat_orig[:,name_index_dict[name]]
+        param_ranges[name] = [np.min(vals), np.max(vals)]
+
+###
+### Prior functions : default is UNIFORM, since it is unmodeled and generic
+###
+
+def uniform_prior(x):
     return np.ones(x.shape)
 
+prior_map = {}
+for name in low_level_coord_names:
+    prior_map[name] = uniform_prior
+    if not(name in param_ranges):
+        raise Exception(" {} not provided a parameter range ".format(name))  # change later, should fall back to using prior range from above
+
 
-prior_map  = { 'gamma1':eos_param_uniform_prior, 'gamma2':eos_param_uniform_prior,
-}
-# Les: somewhat more aggressive: 
-#    gamma1: 0.2,2
-#    gamma2: -1.67, 1.7
-prior_range_map = { 'gamma1':  [0.707899,1.31], 'gamma2':[-1.6,1.7], 'gamma3':[-0.6,0.6], 'gamma4':[-0.02,0.02]
-}
-
-
-# tex_dictionary  = {
-#  "mtot": '$M$',
-#  "mc": '${\cal M}_c$',
-#  "m1": '$m_1$',
-#  "m2": '$m_2$',
-#   "q": "$q$",
-#   "delta" : "$\delta$",
-#   "DeltaOverM2_perp" : "$\Delta_\perp$",
-#   "DeltaOverM2_L" : "$\Delta_{||}$",
-#   "SOverM2_perp" : "$S_\perp$",
-#   "SOverM2_L" : "$S_{||}$",
-#   "eta": "$\eta$",
-#   "chi_eff": "$\chi_{eff}$",
-#   "xi": "$\chi_{eff}$",
-#   "s1z": "$\chi_{1,z}$",
-#   "s2z": "$\chi_{2,z}$"
+prior_range_map = param_ranges
+
+# prior_map  = { 'gamma1':eos_param_uniform_prior, 'gamma2':eos_param_uniform_prior,
+# }
+# # Les: somewhat more aggressive: 
+# #    gamma1: 0.2,2
+# #    gamma2: -1.67, 1.7
+# prior_range_map = { 'gamma1':  [0.707899,1.31], 'gamma2':[-1.6,1.7], 'gamma3':[-0.6,0.6], 'gamma4':[-0.02,0.02]
 # }
 
 
+###
+### Supplemental likelihood: load (as in ILE)
+###
+supplemental_ln_likelihood= None
+supplemental_ln_likelihood_prep =None
+supplemental_ln_likelihood_parsed_ini=None
+# Supplemental likelihood factor. Must have identical call sequence to 'likelihood_function'. Called with identical raw inputs (including cosines/etc)
+if opts.supplementary_likelihood_factor_code and opts.supplementary_likelihood_factor_function:
+  print(" EXTERNAL SUPPLEMENTARY LIKELIHOOD FACTOR : {}.{} ".format(opts.supplementary_likelihood_factor_code,opts.supplementary_likelihood_factor_function))
+  __import__(opts.supplementary_likelihood_factor_code)
+  external_likelihood_module = sys.modules[opts.supplementary_likelihood_factor_code]
+  supplemental_ln_likelihood = getattr(external_likelihood_module,opts.supplementary_likelihood_factor_function)
+  name_prep = "prepare_"+opts.supplementary_likelihood_factor_function
+  if hasattr(external_likelihood_module,name_prep):
+    supplemental_ln_likelhood_prep=getattr(external_likelihood_module,name_prep)
+    # Check for and load in ini file associated with external library
+    if opts.supplementary_likelihood_factor_ini:
+      import configparser as ConfigParser
+      config = ConfigParser.ConfigParser()
+      config.optionxform=str # force preserve case! 
+      config.read(opts.supplementary_likelihood_factor_ini)
+      supplemental_ln_likelhood_parsed_ini=config
+
+      # Call the ini file, tell it what coordinates we are using by name
+      supplemental_ln_likelihood_prep(config=supplemental_ln_likelihood_parsed_ini,coords=coord_names)
+
+
+
+
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import RBF, WhiteKernel, ConstantKernel as C
 
 def adderr(y):
     val,err = y
     return val+error_factor*err
 
@@ -386,32 +360,55 @@
         print(" Fitting partition ")
         gp_fit_list.append(fit_gp(x[part],y[part],**kwargs))
     fn_out =  lambda x: np.mean( map_funcs( gp_fit_list,x), axis=0)
     print(" Testing ", fn_out([x[0]]))
     return fn_out
 
 
+def fit_rf(x,y,y_errors=None,fname_export='nn_fit'):
+#    from sklearn.ensemble import RandomForestRegressor
+    from sklearn.ensemble import ExtraTreesRegressor
+    # Instantiate model. Usually not that many structures to find, don't overcomplicate
+    #   - should scale like number of samples
+    rf = ExtraTreesRegressor(n_estimators=100, verbose=True,n_jobs=-1) # no more than 5% of samples in a leaf
+    if y_errors is None:
+        rf.fit(x,y)
+    else:
+        rf.fit(x,y,sample_weight=1./y_errors**2)
+
+    ### reject points with infinities : problems for inputs
+    def fn_return(x_in,rf=rf):
+        f_out = -lnL_default_large_negative*np.ones(len(x_in))
+        # remove infinity or Nan
+        indx_ok = np.all(np.isfinite(np.array(x_in,dtype=float)),axis=-1)
+        # rf internally uses float32, so we need to remove points > 10^37 or so ! 
+        #    ... this *should* never happen due to bounds constraints, but ...
+        indx_ok_size = np.all( np.logical_not(np.greater(np.abs(x_in),1e37)), axis=-1)
+        indx_ok = np.logical_and(indx_ok, indx_ok_size)
+        f_out[indx_ok] = rf.predict(x_in[indx_ok])
+        return f_out
+#    fn_return = lambda x_in: rf.predict(x_in) 
+
+    print( " Demonstrating RF")   # debugging
+    residuals = rf.predict(x)-y
+    print( "    std ", np.std(residuals), np.max(y), np.max(fn_return(x)))
+    return fn_return
+
+
+
 
 
 # initialize
 dat_mass  = [] 
 weights = []
 n_params = -1
 
-###
-### Retrieve data
-###
-#  int_sig sigma/L gamma1 gamma2 ...
-col_lnL = 0
-dat_orig = dat = np.loadtxt(opts.fname)
-dat_orig = dat[dat[:,col_lnL].argsort()] # sort  http://stackoverflow.com/questions/2828059/sorting-arrays-in-numpy-by-column
-print(" Original data size = ", len(dat), dat.shape)
 
  ###
- ### Convert data.  
+ ### Convert data.   RIGHT NOW JUST DOWNSELECTING, no intermediate fitting parameters defined
  ###
 
 dat_out = []
 for line in dat:
   dat_here= np.zeros(len(coord_names)+2)
   if line[col_lnL+1] > opts.sigma_cut:
       print("skipping", line)
@@ -425,23 +422,14 @@
 X =dat_out[:,0:len(coord_names)]
 Y = dat_out[:,-2]
 Y_err = dat_out[:,-1]
 # Save copies for later (plots)
 X_orig = X.copy()
 Y_orig = Y.copy()
 
-# Plot cumulative distribution in lnL, for all points.  Useful sanity check for convergence.  Start with RAW
-if not opts.no_plots:
-    Yvals_copy = Y_orig.copy()
-    Yvals_copy = Yvals_copy[Yvals_copy.argsort()[::-1]]
-    pvals = np.arange(len(Yvals_copy))*1.0/len(Yvals_copy)
-    plt.plot(Yvals_copy, pvals)
-    plt.xlabel(r"$\ln{\cal L}$")
-    plt.ylabel(r"evaluation fraction $(<\ln{\cal L})$")
-    plt.savefig("lnL_cumulative_distribution_of_input_points.png"); plt.clf()
 
 
 # Eliminate values with Y too small
 max_lnL = np.max(Y)
 indx_ok = Y>np.max(Y)-opts.lnL_offset
 # Provide some random points, to insure reasonable tapering behavior away from the sample
 print(" Points used in fit : ", sum(indx_ok), " given max lnL ", max_lnL)
@@ -456,49 +444,50 @@
     indx_list = np.array( [[k, Y[k]] for k in idx_sorted_index])     # pair up with the weights again
     indx_list = indx_list[::-1]  # reverse, so most significant are first
     indx_ok = map(int,indx_list[:10,0])
     print(" Revised number of points for fit: ", sum(indx_ok), indx_ok, indx_list[:10])
 X_raw = X.copy()
 
 my_fit= None
-if True:
+if opts.fit_method =='gp':
     print(" FIT METHOD : GP")
     # some data truncation IS used for the GP, but beware
     print(" Truncating data set used for GP, to reduce memory usage needed in matrix operations")
     X=X[indx_ok]
     Y=Y[indx_ok] - lnL_shift
     Y_err = Y_err[indx_ok]
     # Cap the total number of points retained, AFTER the threshold cut
     if opts.cap_points< len(Y) and opts.cap_points> 100:
         n_keep = opts.cap_points
         indx = np.random.choice(np.arange(len(Y)),size=n_keep,replace=False)
         Y=Y[indx]
         X=X[indx]
         Y_err=Y_err[indx]
     my_fit = fit_gp(X,Y,y_errors=Y_err)
+elif opts.fit_method == 'rf':
+    print( " FIT METHOD ", opts.fit_method, " IS RF ")
+    # NO data truncation for NN needed?  To be *consistent*, have the code function the same way as the others
+    X=X[indx_ok]
+    Y=Y[indx_ok] - lnL_shift
+    Y_err = Y_err[indx_ok]
+    # Cap the total number of points retained, AFTER the threshold cut
+    if opts.cap_points< len(Y) and opts.cap_points> 100:
+        n_keep = opts.cap_points
+        indx = np.random.choice(np.arange(len(Y)),size=n_keep,replace=False)
+        Y=Y[indx]
+        X=X[indx]
+        Y_err=Y_err[indx]
+    my_fit = fit_rf(X,Y,y_errors=Y_err)
 
 
 # Sort for later convenience (scatterplots, etc)
 indx = Y.argsort()#[::-1]
 X=X[indx]
 Y=Y[indx]
 
-# Make grid plots for all pairs of points, to facilitate direct validation of where posterior support lies
-if not no_plots:
- import itertools
- for i, j in itertools.product( np.arange(len(coord_names)),np.arange(len(coord_names)) ):
-  if i < j:
-    plt.scatter( X[:,i],X[:,j],label='rapid_pe',c=Y); plt.legend(); plt.colorbar()
-    x_name = str(coord_names[i])
-    y_name = str(coord_names[j])
-    plt.xlabel( x_name)
-    plt.ylabel( y_name )
-    plt.title("rapid_pe evaluations (=inputs); no fits")
-    plt.savefig("scatter_"+coord_names[i]+"_"+coord_names[j]+".png"); plt.clf()
-
 
 
 ###
 ### Integrate posterior
 ###
 
 
@@ -581,21 +570,89 @@
     def likelihood_function(x,y,z,a,b,c,d,e,f,g):  
         if isinstance(x,float):
             return np.exp(my_fit([x,y,z,a,b,c,d,e,f,g]))
         else:
             return np.exp(my_fit(convert_coords(np.c_[x,y,z,a,b,c,d,e,f,g])))
 
 
+
+
 n_step = 1e5
 my_exp = np.min([1,0.8*np.log(n_step)/np.max(Y)])   # target value : scale to slightly sublinear to (n_step)^(0.8) for Ymax = 200. This means we have ~ n_step points, with peak value wt~ n_step^(0.8)/n_step ~ 1/n_step^(0.2), limiting contrast
 #my_exp = np.max([my_exp,  1/np.log(n_step)]) # do not allow extreme contrast in adaptivity, to the point that one iteration will dominate
 print(" Weight exponent ", my_exp, " and peak contrast (exp)*lnL = ", my_exp*np.max(Y), "; exp(ditto) =  ", np.exp(my_exp*np.max(Y)), " which should ideally be no larger than of order the number of trials in each epoch, to insure reweighting doesn't select a single preferred bin too strongly.  Note also the floor exponent also constrains the peak, de-facto")
 
+
+extra_args={}
+if opts.sampler_method == "GMM":
+    n_max_blocks = ((1.0*int(opts.n_max))/n_step) 
+    n_comp = opts.internal_n_comp # default
+    def parse_corr_params(my_str):
+        """
+        Takes a string with no spaces, and returns a tuple
+        """
+        corr_param_names = my_str.replace(',',' ').split()
+        corr_param_indexes = []
+        for param in corr_param_names:
+            try:
+                indx = low_level_coord_names.index(param)
+                corr_param_indexes.append(indx)
+            except:
+                continue
+        return tuple(corr_param_indexes)
+    if opts.internal_correlate_parameters == 'all':
+        gmm_dict = {tuple(range(len(low_level_coord_names))):None} # integrate *jointly* in all parameters together
+    elif not (opts.internal_correlate_parameters is None):
+        # Correlate identified parameters
+        my_blocks = opts.internal_correlate_parameters.split()
+        my_tuples = list(map( parse_corr_params, my_blocks))
+        gmm_dict = {x:None for x in my_tuples}
+        # What about un-labelled parameters? Make a null tuple for them as well
+        correlated_params = set(()); correlated_params = correlated_params.union( *list(map(set,my_tuples)))
+        uncorrelated_params = set(np.arange(len(low_level_coord_names))); 
+        uncorrelated_params = uncorrelated_params.difference(correlated_params)
+        for x in uncorrelated_params:
+            gmm_dict[(x,)] = None
+        print( " Using correlated GMM sampling on sampling variable indexes " , gmm_dict, " out of ", low_level_coord_names)
+    else:
+        param_indexes = range(len(low_level_coord_names))
+        gmm_dict  = {(k,):None for k in param_indexes} # no correlations
+    if opts.internal_gmm_memory_chisquared_factor:
+        lnL_offset_saving = len(low_level_coord_names)*opts.internal_gmm_memory_chisquared_factor  # based on chisquared distribution, we should not be keeping more than this for output.  This is PURELY FOR MEMORY MANAGEMENT
+    else:
+        lnL_offset_saving = opts.lnL_offset
+    extra_args = {'n_comp':n_comp,'max_iter':n_max_blocks,'L_cutoff': (np.exp(max_lnL-lnL_shift - lnL_offset_saving)),'gmm_dict':gmm_dict,'max_err':50}  # made up for now, should adjust
+extra_args.update({
+    "n_adapt": 100, # Number of chunks to allow adaption over
+    "history_mult": 10, # Multiplier on 'n' - number of samples to estimate marginalized 1D histograms with, 
+    "force_no_adapt":opts.force_no_adapt,
+    "tripwire_fraction":opts.tripwire_fraction
+})
+
+fn_passed = likelihood_function
+if supplemental_ln_likelihood:
+    fn_passed =  lambda *x: likelihood_function(*x)*np.exp(supplemental_ln_likelihood(*x))
+if opts.internal_use_lnL:
+    fn_passed = log_likelihood_function   # helps regularize large values
+    if supplemental_ln_likelihood:
+        fn_passed =  lambda *x: log_likelihood_function(*x) + supplemental_ln_likelihood(*x)
+    extra_args.update({"use_lnL":True,"return_lnI":True})
+
+
+
 res, var, neff, dict_return = sampler.integrate(likelihood_function, *coord_names,  verbose=True,nmax=int(opts.n_max),n=n_step,neff=opts.n_eff, save_intg=True,tempering_adapt=True, floor_level=1e-3,igrand_threshold_p=1e-3,convergence_tests=test_converged,adapt_weight_exponent=my_exp,no_protect_names=True)  # weight ecponent needs better choice. We are using arbitrary-name functions
 
+n_ESS = -1
+if True:
+    # Compute n_ESS.  Should be done by integrator!
+    weights_scaled = sampler._rvs["integrand"]*sampler._rvs["joint_prior"]/sampler._rvs["joint_s_prior"]
+    weights_scaled = weights_scaled/np.max(weights_scaled)  # try to reduce dynamic range
+    n_ESS = np.sum(weights_scaled)**2/np.sum(weights_scaled**2)
+    print(" n_eff n_ESS ", neff, n_ESS)
+
 
 # Save result -- needed for odds ratios, etc.
 np.savetxt("integral_result.dat", [np.log(res)])
 
 if neff < len(coord_names):
     print(" PLOTS WILL FAIL ")
     print(" Not enough independent Monte Carlo points to generate useful contours")
@@ -629,59 +686,22 @@
 ps =samples["joint_s_prior"]
 lnL = dat_logL
 lnLmax = np.max(lnL)
 weights = np.exp(lnL-lnLmax)*p/ps
 
 
 
-
-if not no_plots:
- for indx in np.arange(len(coord_names)):
-   if True:
-    dat_out = []; dat_out_LI=[]
-    p = coord_names[indx]
-    print(" -- 1d cumulative "+ str(indx)+ ":"+ coord_names[indx]+" ----")
-    dat_here = samples[coord_names[indx]]
-    range_x = [np.min(dat_here), np.max(dat_here)]
-    for x in np.linspace(range_x[0],range_x[1],200):
-         dat_out.append([x, np.sum( weights[ dat_here< x])/np.sum(weights)])
-    
-    np.savetxt(p+"_cdf_nocut_beware.dat", np.array(dat_out))
-    dat_out = np.array(dat_out); 
-    plt.plot(dat_out[:,0],dat_out[:,1],label="rapid_pe")
-   
-    x_name = p
-    plt.xlabel(x_name); plt.legend()
-    y_name  = x_name.replace('$','')
-    y_name = "$P(<"+y_name + ")$"
-    plt.ylabel(y_name)
-    plt.title("CDF: "+x_name)
-    plt.savefig(p+"_cdf_nocut_beware.png"); plt.clf()
-   else:
-      plt.clf()  # clear plot, just in case
-      print(" No 1d plot for variable")
-
+print(" ---- Subset for posterior samples (and further corner work) --- ")
 
 
-print(" ---- Subset for posterior samples (and further corner work) --- ")
+p_norm = (weights/np.sum(weights))
+indx_list = np.random.choice(np.arange(len(weights)), p=p_norm.astype(np.float64),size=opts.n_output_samples)
 
-# pick random numbers
-p_thresholds =  np.random.uniform(low=0.0,high=1.0,size=opts.n_output_samples)
-if opts.verbose:
-    print(" output size: selected thresholds N=", len(p_thresholds))
-# find sample indexes associated with the random numbers
-#    - FIXME: first truncate the bad ones
-# idx_sorted_index = numpy.lexsort((numpy.arange(len(weights)), weights))  # Sort the array of weights, recovering index values
-# indx_list = numpy.array( [[k, weights[k]] for k in idx_sorted_index])     # pair up with the weights again
-# cum_weights = np.cumsum(indx_list[:,1)
-# cum_weights = cum_weights/cum_weights[-1]
-# indx_list = [indx_list[k, 0] for k, value in enumerate(cum_sum > deltaP) if value]  # find the indices that preserve > 1e-7 of total probabilit
-cum_sum  = np.cumsum(weights)
-cum_sum = cum_sum/cum_sum[-1]
-indx_list = np.array(map(lambda x : np.sum(cum_sum < x),  p_thresholds))  # this can lead to duplicates
 
-dat_out = np.zeros( (len(p_thresholds),len(coord_names)))
+dat_out = np.zeros( (opts.n_output_samples,2+len(dat_orig_names)) )
 for indx in np.arange(len(coord_names)):
-    dat_out[:,indx] = samples[coord_names[indx]][indx_list]
+    vals = samples[coord_names[indx]][indx_list]   # load in data for this column
+    outindx = name_index_dict[ coord_names[indx]]   # write in correct place
+    dat_out[:,outindx] = vals
 
 print(" Saving to ", opts.fname_output_samples+".dat")
-np.savetxt(opts.fname_output_samples+".dat",dat_out,header=' '.join(coord_names))
+np.savetxt(opts.fname_output_samples+".dat",dat_out,header=" lnL sigma_lnL " + ' '.join(dat_orig_names))
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files 3% similar despite different names*

```diff
@@ -309,15 +309,16 @@
 parser.add_argument("--fit-save-gp",default=None,type=str,help="Filename of GP fit to save. ")
 parser.add_argument("--fit-order",type=int,default=2,help="Fit order (polynomial case: degree)")
 parser.add_argument("--fit-uncertainty-added",default=False, action='store_true', help="Reported likelihood is lnL+(fit error). Use for placement and use of systematic errors.")
 parser.add_argument("--no-plots",action='store_true')
 parser.add_argument("--tabular-eos-file",type=str,default=None,help="Tabular file of EOS to use.  The default prior will be UNIFORM in this table!")
 parser.add_argument("--tabular-eos-file-format",type=str,default=None,help="Format of tabular file of EOS to use.  The default prior will be UNIFORM in this table!")
 parser.add_argument("--tabular-eos-order-statistic",type=str,default=None,help="Order statistic to use.  Options will include R1p4, LambdaTildeQ1, and ...}")
-parser.add_argument("--using-eos", type=str, default=None, help="Name of EOS.  Fit parameter list should physically use lambda1, lambda2 information (but need not) ")
+parser.add_argument("--using-eos", type=str, default=None, help="Name of EOS.  Fit parameter list should physically use lambda1, lambda2 information (but need not). If starts with 'file:', uses a filename with EOS parameters ")
+parser.add_argument("--using-eos-index", type=int, default=None, help="Index of EOS parameters in file.")
 parser.add_argument("--no-use-lal-eos",action='store_true',help="Do not use LAL EOS interface. Used for spectral EOS. Do not use this.")
 parser.add_argument("--no-matter1", action='store_true', help="Set the lambda parameters to zero (BBH) but return them")
 parser.add_argument("--no-matter2", action='store_true', help="Set the lambda parameters to zero (BBH) but return them")
 parser.add_argument("--protect-coordinate-conversions", action='store_true', help="Adds an extra layer to coordinate conversions with range tests. Slows code down, but adds layer of safety for out-of-range EOS parameters for example")
 parser.add_argument("--source-redshift",default=0,type=float,help="Source redshift (used to convert from source-frame mass [integration limits] to arguments of fitting function.  Note that if nonzero, integration done in SOURCE FRAME MASSES, but the fit is calculated using DETECTOR FRAME")
 parser.add_argument("--eos-param", type=str, default=None, help="parameterization of equation of state")
 parser.add_argument("--eos-param-values", default=None, help="Specific parameter list for EOS")
@@ -331,44 +332,90 @@
 parser.add_argument("--tripwire-fraction",default=0.05,type=float,help="Fraction of nmax of iterations after which n_eff needs to be greater than 1+epsilon for a small number epsilon")
 
 # FIXME hacky options added by me (Liz) to try to get my capstone project to work.
 # I needed a way to fix the component masses and nothing else seemed to work.
 parser.add_argument("--fixed-parameter", action="append")
 parser.add_argument("--fixed-parameter-value", action="append")
 
+# Supplemental likelihood factors: convenient way to effectively change the mass/spin prior in arbitrary ways for example
+# Note this supplemental factor is passed the *fitting* arguments, directly.  Use with extreme caution, since we often change the dimension in a DAG 
+parser.add_argument("--supplementary-likelihood-factor-code", default=None,type=str,help="Import a module (in your pythonpath!) containing a supplementary factor for the likelihood.  Used to impose supplementary external priors of arbitrary complexity and external dependence (e.g., external astro priors). EXPERTS-ONLY")
+parser.add_argument("--supplementary-likelihood-factor-function", default=None,type=str,help="With above option, specifies the specific function used as an external likelihood. EXPERTS ONLY")
+parser.add_argument("--supplementary-likelihood-factor-ini", default=None,type=str,help="With above option, specifies an ini file that is parsed (here) and passed to the preparation code, called when the module is first loaded, to configure the module. EXPERTS ONLY")
+
 opts=  parser.parse_args()
 if not(opts.no_adapt_parameter):
     opts.no_adapt_parameter =[] # needs to default to empty list
 ECC_MAX = opts.ecc_max
 ECC_MIN = opts.ecc_min
 no_plots = no_plots |  opts.no_plots
 lnL_shift = 0
 lnL_default_large_negative = -500
 if opts.lnL_shift_prevent_overflow:
     lnL_shift  = opts.lnL_shift_prevent_overflow
 if not(opts.force_no_adapt):
     opts.force_no_adapt=False  # force explicit boolean false
 
+ok_lnL_methods = ['GMM', 'adaptive_cartesian', 'adaptive_cartesian_gpu']
+if opts.internal_use_lnL and not(opts.sampler_method  in ok_lnL_methods ):
+  print(" OPTION MISMATCH : --internal-use-lnL not compatible with", opts.sampler_method, " can only use ", ok_lnL_methods)
+  sys.exit(99)
+
+
 source_redshift=opts.source_redshift
 
 #  require eos index input and 
 if  opts.input_eos_index and not(opts.tabular_eos_file):
     print(" warning: input EOS index, but not using it; presumably you are doing a model-free test ")
 if  not(opts.input_eos_index) and (opts.tabular_eos_file):
     raise Exception(" Fail: must process EOS input to be able to use it ")
 
 my_eos=None
 #option to be used if gridded values not calculated assuming EOS
 if opts.using_eos!=None:
     import RIFT.physics.EOSManager as EOSManager
     eos_name=opts.using_eos
     if opts.verbose:
-        print(" Using EOS ", eos_name, opts.eos_param, opts.eos_param_values)
+        print(" Using EOS ", eos_name, opts.using_eos_index, opts.eos_param, opts.eos_param_values)
 
-    if opts.eos_param == 'spectral':
+    if eos_name.startswith("file:") and not(opts.using_eos_index is None):
+        # Load in filename
+        fname = eos_name.replace('file:', '')
+        # Retrieve row with parameters
+        dat = np.loadtxt(fname)[opts.using_eos_index]
+        spec_param_array = dat[2:]  # drop first two as lnL, sigma_lnL
+        if opts.eos_param == 'spectral':
+            spec_params ={}
+            spec_params['gamma1']=spec_param_array[0]
+            spec_params['gamma2']=spec_param_array[1]
+            if len(spec_param_array) <3:
+                spec_params['gamma3']=spec_params['gamma4']=0
+            else:
+                spec_params['gamma3']=spec_param_array[2]
+                spec_params['gamma4']=spec_param_array[3]
+            eos_base = EOSManager.EOSLindblomSpectral(name=eos_name,spec_params=spec_params,use_lal_spec_eos=not opts.no_use_lal_eos)
+            my_eos=eos_base
+        elif opts.eos_param == 'cs_spectral' and len(spec_param_array >=4):
+            spec_params['gamma1']=spec_param_array[0]
+            spec_params['gamma2']=spec_param_array[1]
+            spec_params['gamma3']=spec_params['gamma4']=0
+            spec_params['gamma3']=spec_param_array[2]
+            spec_params['gamma4']=spec_param_array[3]
+            eos_base = EOSManager.EOSLindblomSpectralSoundSpeedVersusPressure(name=eos_name,spec_params=spec_params,use_lal_spec_eos=not opts.no_use_lal_eos)
+            my_eos = eos_base
+        elif opts.eos_param == 'PP' and len(spec_param_array >=4):
+            spec_params['logP1'] = spec_param_array[0]
+            spec_params['gamma1'] = spec_param_array[1]
+            spec_params['gamma2'] = spec_param_array[2]
+            spec_params['gamma3'] = spec_param_array[3]
+            eos_base = EOSManager.EOSPiecewisePolytrope(name=eos_name,params_dict=spec_params)
+            my_eos = eos_base
+        else:
+            raise Exception("Unknown method for parametric EOS data file {} : {} ".format(eos_name,opts.eos_param))
+    elif opts.eos_param == 'spectral':
         # Will not work yet -- need to modify to parse command-line arguments
         spec_param_packed=eval(opts.eos_param_values) # two lists: first are 'fixed' and second are specific
         fixed_param_array=spec_param_packed[0]
         spec_param_array=spec_param_packed[1]
         spec_params ={}
         spec_params['gamma1']=spec_param_array[0]
         spec_params['gamma2']=spec_param_array[1]
@@ -422,14 +469,15 @@
 with open('args.txt','w') as fp:
     import sys
     fp.write(' '.join(sys.argv))
 
 if opts.fit_method == "quadratic":
     opts.fit_order = 2  # overrride
 
+
 ###
 ### Comparison data (from LI)
 ###
 remap_ILE_2_LI = {
  "s1z":"a1z", "s2z":"a2z", 
  "s1x":"a1x", "s1y":"a1y",
  "s2x":"a2x", "s2y":"a2y",
@@ -587,14 +635,43 @@
 if opts.fit_method =="polynomial" or opts.fit_method == 'quadratic':
     print(" Symmetry for these fitting coordinates :", lalsimutils.symmetry_sign_exchange(coord_names))
 print(" Coordinate names for Monte Carlo :, ", low_level_coord_names)
 if not(opts.no_plots):
     print(" Rendering coordinate names : ", list(map(lambda x: tex_dictionary[x], low_level_coord_names)))
 
 
+
+###
+### Supplemental likelihood: load (as in ILE)
+###
+supplemental_ln_likelihood= None
+supplemental_ln_likelihood_prep =None
+supplemental_ln_likelihood_parsed_ini=None
+# Supplemental likelihood factor. Must have identical call sequence to 'likelihood_function'. Called with identical raw inputs (including cosines/etc)
+if opts.supplementary_likelihood_factor_code and opts.supplementary_likelihood_factor_function:
+  print(" EXTERNAL SUPPLEMENTARY LIKELIHOOD FACTOR : {}.{} ".format(opts.supplementary_likelihood_factor_code,opts.supplementary_likelihood_factor_function))
+  __import__(opts.supplementary_likelihood_factor_code)
+  external_likelihood_module = sys.modules[opts.supplementary_likelihood_factor_code]
+  supplemental_ln_likelihood = getattr(external_likelihood_module,opts.supplementary_likelihood_factor_function)
+  name_prep = "prepare_"+opts.supplementary_likelihood_factor_function
+  if hasattr(external_likelihood_module,name_prep):
+    supplemental_ln_likelhood_prep=getattr(external_likelihood_module,name_prep)
+    # Check for and load in ini file associated with external library
+    if opts.supplementary_likelihood_factor_ini:
+      import configparser as ConfigParser
+      config = ConfigParser.ConfigParser()
+      config.optionxform=str # force preserve case! 
+      config.read(opts.supplementary_likelihood_factor_ini)
+      supplemental_ln_likelhood_parsed_ini=config
+
+      # Call the ini file, tell it what coordinates we are using by name
+      supplemental_ln_likelihood_prep(config=supplemental_ln_likelihood_parsed_ini,coords=coord_names)
+
+
+
 ###
 ### Prior functions : a dictionary
 ###
 
 # mcmin, mcmax : to be defined later
 def M_prior(x):  # not normalized; see section II.C of https://arxiv.org/pdf/1701.01137.pdf
     return 2*x/(mc_max**2-mc_min**2)
@@ -2320,16 +2397,20 @@
     "tripwire_fraction":opts.tripwire_fraction
 })
 tempering_adapt=True
 if opts.force_no_adapt:   
     tempering_adapt=False
 # Result shifted by lnL_shift
 fn_passed = likelihood_function
-if opts.sampler_method=="GMM" and opts.internal_use_lnL:
+if supplemental_ln_likelihood:
+    fn_passed =  lambda *x: likelihood_function(*x)*np.exp(supplemental_ln_likelihood(*x))
+if opts.internal_use_lnL:
     fn_passed = log_likelihood_function   # helps regularize large values
+    if supplemental_ln_likelihood:
+        fn_passed =  lambda *x: log_likelihood_function(*x) + supplemental_ln_likelihood(*x)
     extra_args.update({"use_lnL":True,"return_lnI":True})
 if opts.internal_temper_log:
     extra_args.update({'temper_log':True})
 res, var, neff, dict_return = sampler.integrate(fn_passed, *low_level_coord_names,  verbose=True,nmax=int(opts.n_max),n=n_step,neff=opts.n_eff, save_intg=True,tempering_adapt=tempering_adapt, floor_level=1e-3,igrand_threshold_p=1e-3,convergence_tests=test_converged,tempering_exp=my_exp,no_protect_names=True, **extra_args)  # weight ecponent needs better choice. We are using arbitrary-name functions
 
 
 n_ESS = -1
@@ -2386,27 +2467,39 @@
 
 
 # Save result -- needed for odds ratios, etc.
 #   Warning: integral_result.dat uses *original* prior, before any reweighting
 np.savetxt(opts.fname_output_integral+".dat", [np.log(res)+lnL_shift])
 eos_extra = []
 annotation_header = "lnL sigmaL neff "
-if opts.using_eos:
+if opts.using_eos and not(opts.using_eos.startswith('file:')):
     eos_extra = [opts.using_eos]
     annotation_header += 'eos_name '
     if opts.eos_param == 'spectral':
         # Should also 
         my_eos_params = my_eos.spec_params
         eos_extra += list(map( lambda x: str(my_eos_params[x]), ["gamma1", "gamma2", "gamma3", "gamma4", "p0", "epsilon0", "xmax"]))
 #        eos_extra += opts.eos_param
         annotation_header += "gamma1 gamma2 gamma3 gamma4 p0 epsilon0 xmax"
+elif opts.using_eos and opts.using_eos.startswith('file:'):
+    fname = opts.using_eos.replace('file:','')
+    params_here = np.loadtxt(fname)[opts.using_eos_index][2:]
+    linefirst =''
+    with open(fname) as f:
+        linefirst = f.readline()
+    linefirst = linefirst[2:]
+    annotation_header = linefirst # this will/must be lnL sigma_lnL and then parameter names, which we want to preserve
 with open(opts.fname_output_integral+"+annotation.dat", 'w') as file_out:
+  if not(opts.using_eos) or not(opts.using_eos.startswith('file:')):
     str_out =list( map(str,[np.log(res), np.sqrt(var)/res, neff]))
     file_out.write("# " + annotation_header + "\n")
     file_out.write(' '.join( str_out + eos_extra + ["\n"]))
+  else:
+    file_out.write("# " + annotation_header + "\n")
+    file_out.write(" {} {} ".format(np.log(res), np.sqrt(var)/res) + ' '.join(map(str,params_here)))
 #np.savetxt(opts.fname_output_integral+"+annotation.dat", np.array([[np.log(res), np.sqrt(var)/res, neff]]), header=eos_extra)
 # since not EOS, can just use np.savetxt
 np.savetxt(opts.fname_output_integral+"+annotation_ESS.dat",[[np.log(res), np.sqrt(var)/res, neff, n_ESS]],header=" lnL sigmaL neff n_ESS ")
 # with open(opts.fname_output_integral+"+annotation_ESS.dat", 'w') as file_out:
 #     annotation_header = "lnL sigmaL neff n_ESS "
 #     str_out =list( map(str,[np.log(res), np.sqrt(var)/res, neff, n_ESS]))
 #     file_out.write("# " + annotation_header + "\n")
```

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

