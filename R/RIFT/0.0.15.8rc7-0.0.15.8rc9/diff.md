# Comparing `tmp/RIFT-0.0.15.8rc7.tar.gz` & `tmp/RIFT-0.0.15.8rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RIFT-0.0.15.8rc7.tar", last modified: Sun Apr 16 18:25:20 2023, max compression
+gzip compressed data, was "dist/RIFT-0.0.15.8rc9.tar", last modified: Thu Apr 20 10:33:07 2023, max compression
```

## Comparing `RIFT-0.0.15.8rc7.tar` & `RIFT-0.0.15.8rc9.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    99712 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1529 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   117293 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    74024 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12192 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    96043 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10494 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   241710 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28330 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   108901 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc7/Dockerfile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/README.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/setup.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MANIFEST.in
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/LICENSE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/setup.cfg
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/requirements.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/README.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/requirements.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/LICENSE.md
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10563 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   100226 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   119468 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    76651 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    96043 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1885 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109131 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:06.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28330 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   244270 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/setup.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc9/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-20 10:33:07.000000 RIFT-0.0.15.8rc9/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc9/MANIFEST.in
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.8rc9/Dockerfile
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
 optp.add_option("--force-xpy", action="store_true", help="Use the xpy code path.  Use with --vectorized --gpu to use the fallback CPU-based code path. Useful for debugging.")
 optp.add_option("-o", "--output-file", help="Save result to this file.")
 optp.add_option("-O", "--output-format", default='xml', help="[xml|hdf5]")
 optp.add_option("-S", "--save-samples", action="store_true", help="Save sample points to output-file. Requires --output-file to be defined.")
 optp.add_option("-L", "--save-deltalnL", type=float, default=float("Inf"), help="Threshold on deltalnL for points preserved in output file.  Requires --output-file to be defined")
 optp.add_option("-P", "--save-P", type=float,default=0.1, help="Threshold on cumulative probability for points preserved in output file.  Requires --output-file to be defined")
 optp.add_option("--internal-hard-fail-on-error",action='store_true',help='If true, fails with exit code 1 if any point is unsuccessful')
+optp.add_option("--internal-soft-fail-on-cuda-error",action='store_true',help='If true, returns with exit code 0 on any CUDA error. Use with care (e.g., if many jobs failing)')
 optp.add_option("--internal-make-empty-file-on-error",action='store_true',help='If true, failed points generate empty output file. Protects against OSG workflow problems')
 optp.add_option("--verbose",action='store_true')
 optp.add_option("--save-eccentricity", action="store_true")
 #
 # Add the integration options
 #
 integration_params = OptionGroup(optp, "Integration Parameters", "Control the integration with these options.")
@@ -232,14 +233,15 @@
 integration_params.add_option("--n-eff", type=int, default=100, help="Total number of effective samples points to calculate before the integration will terminate. Default is 100")
 integration_params.add_option("--fairdraw-extrinsic-output", action='store_true' , help="Output is fair draw, rather than being comprehensive")
 integration_params.add_option("--n-chunk", type=int, help="Chunk'.",default=10000)
 integration_params.add_option("--convergence-tests-on",default=False,action='store_true')
 integration_params.add_option("--seed", type=int, help="Random seed to use. Default is to not seed the RNG.")
 integration_params.add_option("--no-adapt", action="store_true", help="Turn off adaptive sampling. Adaptive sampling is on by default.")
 integration_params.add_option("--force-adapt-all", action="store_true", help="Force adaptive sampling for all parameters.")
+integration_params.add_option("--force-reset-all", action="store_true", help="Force reset of sampling every iteration. (Recommended if AC and not using no-adapt-after-first)")
 integration_params.add_option("--no-adapt-distance", action="store_true", help="Turn off adaptive sampling, just for distance. Adaptive sampling is on by default.")
 integration_params.add_option("--no-adapt-after-first",action='store_true',help="Disables adaptation after first iteration with significant lnL")
 integration_params.add_option("--adapt-weight-exponent", type=float, default=1.0, help="Exponent to use with weights (likelihood integrand) when doing adaptive sampling. Used in tandem with --adapt-floor-level to prevent overconvergence. Default is 1.0.")
 integration_params.add_option("--adapt-floor-level", type=float, default=0.1, help="Floor to use with weights (likelihood integrand) when doing adaptive sampling. This is necessary to ensure the *sampling* prior is non zero during adaptive sampling and to prevent overconvergence. Default is 0.1 (no floor)")
 integration_params.add_option("--adapt-adapt",action='store_true',help="Adapt the tempering exponent")
 integration_params.add_option("--adapt-log",action='store_true',help="Use a logarithmic tempering exponent")
 integration_params.add_option("--interpolate-time", default=False,help="If using time marginalization, compute using a continuously-interpolated array. (Default=false)")
@@ -1746,14 +1748,17 @@
 
 lnL_sofar = -np.inf
 no_adapt_sky = False
 for indx in numpy.arange(len(P_list)):
  try:
   res = analyze_event(P_list, indx, data_dict, psd_dict, fmax, opts)
   lnL_sofar = np.max([lnL_sofar,res])
+  if opts.force_reset_all:
+    for name in sampler.params:
+      sampler.reset_sampling(param)
   if opts.no_adapt_after_first and (not no_adapt_sky):
     if lnL_sofar > 20:  # Use absolute threshold.  Expect this will give modest sky localization.
       # remove right_ascension, declination from adaptive parameters
       params_adapt = sampler.adaptive
       params_adapt  = list(set(params_adapt) - set(['right_ascension','declination']))
       sampler.adaptive = params_adapt
       # Disable saving of the integrand -- saves on memory and will reduce speed. 
@@ -1767,14 +1772,16 @@
     open(fname_output_txt,'a').close()  # create empty file
   if opts.internal_hard_fail_on_error:
     sys.exit(1)
 #  if len(exception_failure) >0:
 #    if "CUBLAS" in exception_failure[0]:  # Hard fail if a cuda error!
 #      sys.exit(1) 
   if ("CUDA" in str(exception_failure)) or ('CUBLAS' in str(exception_failure) or ('cuda' in str(exception_failure))): # Hard fail if a cuda error with a catchable error code
+    if (opts.internal_soft_fail_on_cuda_error):
+      sys.exit(0)
     sys.exit(62)
   if 'Out of memory' in str(exception_failure):   # should never happen, most likely a crappy node or failure to set correct memory limit for ILE.
     sys.exit(63)
   str_err = " {} ".format(exception_failure)
   if ('Zero prior failure' in str_err) or ('effective samples' in str_err):
     # common failures that require reset of sampler
     #    - zero prior : very rare case where the prior is exactly zero for some reason. User error most likely (floors, etc). Should never happen
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#! /usr/bin/env python
 """
 Code to load and combine all the  weights and then rejection sample the results
 """
 
 import os
 import sys
 
@@ -41,10 +42,18 @@
 
 for weight_file in weight_files:
     weights_individual_list.append(np.atleast_1d(np.genfromtxt(weight_file)))
 
 weights = np.concatenate(weights_individual_list)
 np.savetxt(f'{outdir}/weights.dat', weights)
 
+# Truncate samples to weight size, if larger
+npts_wts = len(weights)
+npts_samples = len(result.posterior['m1'])
+print(" Sizes ", npts_samples, npts_wts)
+if npts_samples > len(weights):
+    print(" Truncating input samples to weight size (=requested output size) ")
+    result.posterior = result.posterior.truncate(after=npts_wts-1)
+
 print(f'Importance sampling efficiency: {np.sum(weights)**2/np.sum(weights**2)/len(weights)}')
 result.posterior = bilby.core.result.rejection_sample(result.posterior, weights)
 result.save_posterior_samples(filename=outdir+'/reweighted_posterior_samples.dat', outdir=outdir)
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files 2% similar despite different names*

```diff
@@ -210,14 +210,15 @@
 parser.add_argument("--ile-runtime-max-minutes",default=None,type=int,help="If not none, kills ILE jobs that take longer than the specified integer number of minutes. Do not use unless an expert")
 parser.add_argument("--cip-exe",default=None,help="filename of CIP or equivalent executable. Will default to `which util_ConstructIntrinsicPosterior_GenericCoordinates` in low-level code")
 parser.add_argument("--cip-exe-G",default=None,help="filename of CIP or equivalent executable, as ALTERNATE CIP used when a 'G' iteration is requested ")
 parser.add_argument("--use-eccentricity",default=False,action='store_true')
 parser.add_argument("--test-exe",default=None,help="filename of test code or equivalent executable.  Must have a --test-output <fname> argument.  Used for convergence testing or other termination. NOT ACTIVE; see 'convergence_test_samples.py' for example")
 parser.add_argument("--plot-exe",default=None,help="filename of plot code or equivalent executable.  Will default to `which plot_posterior_corner.py`.  Default is to plot last set of samples")
 parser.add_argument("--gridinit-exe",default=None,help="filename of initial grid creation or equivalent executable.  Will default to `which util_ManualOverlapGrid.py`.  Must create overlap-grid-0.xml.gz")
+parser.add_argument("--frame-rotation",action='store_true',help=" Calculation was done in J frame, not L frame.  Rotate at end. Only if extrinsic samples.")
 parser.add_argument("--calibration-reweighting-exe",default=None,help="Calibration reweighting script")
 parser.add_argument("--calibration-reweighting",action='store_true',help="Run calibration reweighting on final posterior samples")
 parser.add_argument("--calibration-reweighting-batchsize",type=int,default=None,help="If not 'None', tries to group the final set of points based on jobs of a fixed size")
 parser.add_argument("--convert-ascii2h5-exe",default=None,help="Converting ascii to h5 file script")
 parser.add_argument("--comov-distance-reweighting-exe",default=None,help="Comoving distance reweighting script")
 parser.add_argument("--comov-distance-reweighting",action='store_true',help="Run comoving distance reweighting on final posterior samples")
 parser.add_argument("--bilby-pickle-exe",default=None,help="Bilby pickle generation script")
@@ -578,15 +579,19 @@
         test_dir = opts.working_directory+"/iteration_"+str(indx)+"_test"
         mkdir(test_dir); mkdir(test_dir+'/logs')
         
     if opts.plot_args:  # Overkill: currently only making plots on last iteration
         plot_dir = opts.working_directory+"/iteration_"+str(indx)+"_plot"
         mkdir(plot_dir); mkdir(plot_dir+'/logs')
 
-
+# make calmarg directory and log directory
+if opts.calibration_reweighting:
+    cal_dir = opts.working_directory+"/calmarg"
+    mkdir(cal_dir)
+    mkdir(cal_dir+"/logs")
 
 # ++++
 # Create workflow tasks
 # ++++
 
 ##   ILE job
 
@@ -1032,49 +1037,80 @@
     gridinit_job.set_stdout_file(opts.working_directory+"/init-$(cluster)-$(process).out")
     gridinit_job.add_condor_cmd('request_disk',opts.general_request_disk)
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+gridinit_job.get_sub_file()
         gridinit_job.set_sub_file(fname)
     gridinit_job.write_sub_file()
 
+if opts.frame_rotation:
+    # Wriite command to do the conversion
+    extra_arg=''
+    if 'fref' in ile_args:
+        # retrieve fref
+        tmp_args = ile_args.split('--')
+        lines = [x for x in tmp_args if x.startswith('reference-freq')]
+        fref_str = lines[-1].split()[-1]
+        extra_arg = ' --fref {} '.format(fref_str)
+    with open('fix_frame_rot.sh','w') as f:
+        f.write("""#!/bin/bash
+if [ ! -e extrinsic_posterior_samples_orig.dat ]; then
+   mv extrinsic_posterior_samples.dat  extrinsic_posterior_samples_orig.dat;
+   convert_ascii_framechange_xphm.py --extrinsic-posterior-file   extrinsic_posterior_samples_orig .dat --fname-out extrinsic_posterior_samples.dat {}
+fi;
+""".format(extra_arg))
+    # Write submit file for the conversion
+    rotate_job, rotate_job_name = dag_utils.write_convert_sub(exe=which('fix_frame_rot.sh'),tag='ROTATE',log_dir=None,arg_str='',file_input='',file_output=None, out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
+    rotate_job.add_condor_cmd("initialdir",opts.working_directory)
+    rotate_job.set_log_file(opts.working_directory+"/reweight-merge-$(cluster)-$(process).log")
+    rotate_job.set_stderr_file(opts.working_directory+"/reweight-merge-$(cluster)-$(process).err")
+    rotate_job.set_stdout_file(opts.working_directory+"/reweight-merge-$(cluster)-$(process).out")
+    rotate_job.add_condor_cmd('request_disk',opts.cal_request_disk)
+    if opts.use_full_submit_paths:
+        fname = opts.working_directory+"/"+rotate_job.get_sub_file()
+        rotate_job.set_sub_file(fname)
+    if opts.use_osg:
+        rotate_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+        rotate_job.add_condor_cmd("+flock_local",'true')
+    rotate_job.write_sub_file()
+
 if opts.calibration_reweighting:
     if opts.last_iteration_extrinsic_time_resampling and opts.bilby_pickle_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
     elif opts.last_iteration_extrinsic_time_resampling and opts.bilby_ini_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_ini_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_pickle_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
         
     if not(opts.calibration_reweighting_batchsize): # single run
-        calibration_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).log")
-        calibration_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).err")
-        calibration_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).out")
+        calibration_job.set_log_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).log")
+        calibration_job.set_stderr_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).err")
+        calibration_job.set_stdout_file(opts.working_directory+"/calmarg/logs/calibration-$(cluster)-$(process).out")
     else:
         calibration_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
         calibration_job.add_arg(" --start_index $(macrostartidx) ")
         calibration_job.add_arg(" --end_index $(macroendidx) ")
-        calibration_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/calibration-$(macrostartidx)-$(cluster)-$(process).log")
-        calibration_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(macrostartidx)-$(cluster)-$(process).err")
-        calibration_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(macrostartidx)-$(cluster)-$(process).out")
+        calibration_job.set_log_file(opts.working_directory+"/calmarg/logs/calibration-$(macrostartidx)-$(cluster)-$(process).log")
+        calibration_job.set_stderr_file(opts.working_directory+"/calmarg/logs/calibration-$(macrostartidx)-$(cluster)-$(process).err")
+        calibration_job.set_stdout_file(opts.working_directory+"/calmarg/logs/calibration-$(macrostartidx)-$(cluster)-$(process).out")
     calibration_job.add_condor_cmd('request_disk',opts.general_request_disk)
 
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+calibration_job.get_sub_file()
         calibration_job.set_sub_file(fname)
     calibration_job.write_sub_file()
 
     # job to combine things. Write here to make logic human-readable
     if (opts.calibration_reweighting_batchsize): # single run
         reweight_merge_job, reweight_merge_job_name = dag_utils.write_convert_sub(exe=which('combine_weights_and_rejection_sample.py'),tag='CAL_REWEIGHT_COMBINE',log_dir=None,arg_str='',file_input=opts.working_directory+'/extrinsic_posterior_samples.dat weight_files/',file_output=None, out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
         reweight_merge_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
-        reweight_merge_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).log")
-        reweight_merge_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).err")
-        reweight_merge_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).out")
+        reweight_merge_job.set_log_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).log")
+        reweight_merge_job.set_stderr_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).err")
+        reweight_merge_job.set_stdout_file(opts.working_directory+"/calmarg/logs/reweight-merge-$(cluster)-$(process).out")
         reweight_merge_job.add_condor_cmd('request_disk',opts.cal_request_disk)
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+reweight_merge_job.get_sub_file()
             reweight_merge_job.set_sub_file(fname)
         if opts.use_osg:
             reweight_merge_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
             reweight_merge_job.add_condor_cmd("+flock_local",'true')
@@ -1582,14 +1618,22 @@
     if not(opts.last_iteration_extrinsic_time_resampling):
         dag.add_node(cat_node)
         last_node=cat_node
     else:
         dag.add_node(convert_node)   # this is the time resampling task
         last_node=convert_node
 
+# Create rotation job (if extrinsic available)
+if opts.frame_rotation and opts.add_extrinsic:
+    rotate_node = pipeline.CondorDAGNode(rotate_job)
+    rotate_node.set_category("ROTATE")
+    rotate_node.add_parent(last_node)
+    last_node=rotate_node
+    dag.add_node(rotate_node)
+
 # Creating calibration uncertainty job
 if opts.calibration_reweighting:
     if opts.bilby_ini_file:
         pickle_node = pipeline.CondorDAGNode(pickle_job)
         pickle_node.add_macro("macroiteration",it)
         pickle_node.set_category("PICKLE")
         pickle_node.add_parent(last_node)
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,23 @@
 
 def unsafe_parse_arg_string(my_argstr,match):
     arglist  = [x for x in my_argstr.split("--") if len(x)>0]
     for x in arglist:
         if match in x:
             return x
     return None
-        
+def unsafe_parse_arg_string_dict(my_argstr):
+    arglist  = [x for x in my_argstr.split("--") if len(x)>0]
+    dict_return = {}
+    for x in arglist:
+        net = x.split(' ')
+        if len(net)>0:
+            dict_return[net[0]] = net[1]
+    return dict_return
+
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--use-production-defaults",action='store_true',help="Use production defaults. Intended for use with tools like asimov or by nonexperts who just want something to run on a real event.  Will require manual setting of other arguments!")
 parser.add_argument("--use-subdags",action='store_true',help="Use CEPP_Alternate instead of CEPP_BasicIteration")
 parser.add_argument("--bilby-ini-file",default=None,type=str,help="Pass ini file for parsing. Intended to use for calibration reweighting. Full path recommended")
 parser.add_argument("--bilby-pickle-file",default=None,type=str,help="Bilby Pickle file with event settings. Intended to use for calibration reweighting. Full path recommended")
@@ -219,14 +227,16 @@
 parser.add_argument("--internal-cip-cap-neff",type=int,default=500,help="Largest value for CIP n_eff to use for *non-final* iterations. ALWAYS APPLIED. ")
 parser.add_argument('--internal-cip-tripwire',type=float,help="Passed to CIP")
 parser.add_argument("--internal-cip-temper-log",action='store_true',help="Use temper_log in CIP.  Helps stabilize adaptation for high q for example")
 parser.add_argument("--internal-ile-sky-network-coordinates",action='store_true',help="Passthrough to ILE ")
 parser.add_argument("--internal-ile-rotate-phase", action='store_true')
 parser.add_argument("--internal-loud-signal-mitigation-suite",action='store_true',help="Enable more aggressive adaptation - make sure we adapt in distance, sky location, etc rather than use uniform sampling, because we are constraining normally subdominant parameters")
 parser.add_argument("--internal-ile-freezeadapt",action='store_true',help="Passthrough to ILE ")
+parser.add_argument("--internal-ile-reset-adapt",action='store_true',help="Force reset of adaptation")
+parser.add_argument("--internal-ile-force-noreset-adapt",action='store_true',help="Undo any attempt to --force-reset-all")
 parser.add_argument("--internal-ile-adapt-log",action='store_true',help="Passthrough to ILE ")
 parser.add_argument("--internal-ile-auto-logarithm-offset",action='store_true',help="Passthrough to ILE")
 parser.add_argument("--internal-ile-use-lnL",action='store_true',help="Passthrough to ILE via helper.  Will DISABLE auto-logarithm-offset and manual-logarithm-offset for ILE")
 parser.add_argument("--internal-cip-use-lnL",action='store_true')
 parser.add_argument("--manual-initial-grid",default=None,type=str,help="Filename (full path) to initial grid. Copied into proposed-grid.xml.gz, overwriting any grid assignment done here")
 parser.add_argument("--manual-extra-ile-args",default=None,type=str,help="Avenue to adjoin extra ILE arguments.  Needed for unusual configurations (e.g., if channel names are not being selected, etc)")
 parser.add_argument("--manual-extra-puff-args",default=None,type=str,help="Avenue to adjoin extra PUFF arguments.  ")
@@ -735,14 +745,38 @@
     dmax_guess = 10000
 # Last stage of commands done by other tools: too annoying to copy stuff over and run the next generation of the pipeline
 instructions_ile = np.loadtxt("helper_ile_args.txt", dtype=str)  # should be one line
 line = ' '.join(instructions_ile)
 if opts.internal_ile_n_max:
     line = line.replace('--n-max 4000000 ', str(opts.internal_ile_n_max)+" ")
 line += " --l-max " + str(opts.l_max) 
+if 'data-start-time' in line:
+    # Print warnings based on duration and fmin
+    line_dict = unsafe_parse_arg_string_dict(line)
+    data_start_time = line_dict['data-start-time']
+    data_end_time = line_dict['data-end-time']
+    P.m1 = event_dict["m1"]*lal.MSUN_SI; P.m2=event_dict["m2"]*lal.MSUN_SI; P.s1z = event_dict["s1z"]; P.s2z = event_dict["s2z"]
+    P.fmin = opts.fmin  #  fmin we will use internally
+    if opts.fmin_template:
+        P.fmin = opts.fmin_template
+    if opts.l_max > 2 and (("IMRPhenomXP" in opts.approx) or ('XO4a' in opts.approx)):
+        # fmin is start for all modes.   If Lmax>2, use fmin*(2/Lmax) to estimate starting frequecy
+        P_temp = P.copy()
+        P_temp.fmin *= 2./opts.l_max
+        t_HM = lalsimutils.estimateWaveformDuration(P_temp)
+        if  opts.data_LI_seglen < t_HM/2:
+            print("""  WARNING WARNING WARNING WARNING WARNING WARNING WARNING WARNING 
+Your choice of fmin, lmax, and approximant suggests waveform wraparound will occur.  We recommend a longer segment length
+"""
+)
+    elif opts.l_max > 2 and opts.fmin_template:
+        # all modes start at the same time, possibly with different frequencies. Starting frequency needs to be reduced 
+        # User has specified fmin_template, and therefore overridden our default plan to lower the starting frequency
+        if opts.l_max/2 * opts.fmin_template > opts.fmin:
+            print(" WARNING WARNING WARNING: You have modes starting in band. You should probably reduce your starting frequency")
 if (opts.use_ini is None) and not('--d-max' in line):
     line += " --d-max " + str(dmax_guess)
 if opts.ile_distance_prior:
     line += " --d-prior {} ".format(opts.ile_distance_prior)
 if opts.ile_force_gpu:
     line +=" --force-gpu-only "
 sur_location_prefix = "my_surrogates/nr_surrogates/"
@@ -761,24 +795,31 @@
 elif opts.use_gwsurrogate and "NRSur7dq4" in opts.approx:
         line += " --rom-group {} --rom-param NRSur7dq4.h5  --approx {}".format(sur_location_prefix,opts.approx)
 elif ("SEOBNR" in opts.approx) or ("NRHybSur" in opts.approx) or ("NRSur7d" in opts.approx) or ("NRTidal" in opts.approx): 
         line += " --approx " + opts.approx
 else:
         print( " Unknown approx ", opts.approx)
         sys.exit(1)
+if opts.internal_ile_reset_adapt or ((opts.ile_sampler_method =='adaptive_cartesian_gpu' or not(opts.ile_sampler_method)) and not(opts.internal_ile_freezeadapt) ):
+    # force reset if
+    #   - requested or
+    #   - AC + not freezeadapt
+    line += " --force-reset-all "
 if not(opts.manual_extra_ile_args is None):
     line += " {} ".format(opts.manual_extra_ile_args)  # embed with space on each side, avoid collisions
     if '--declination ' in opts.manual_extra_ile_args:   # if we are pinning dec, we aren't using a cosine coordinate. Don't mess up.
         line = line.replace('--declination-cosine-sampler', '')  
 if not(opts.ile_sampler_method is None):
     line += " --sampler-method {} ".format(opts.ile_sampler_method)
 if opts.internal_ile_sky_network_coordinates:
     line += " --internal-sky-network-coordinates "
 if opts.ile_no_gpu:  # make sure we are using the standard code path if not using GPUs
     line += " --force-xpy " 
+if opts.internal_ile_force_noreset_adapt:
+    line = line.replace(' --force-reset-all ', ' ')
 with open('args_ile.txt','w') as f:
         f.write(line)
 
 
 #os.system("cp helper_test_args.txt args_test.txt")
 with open ("helper_test_args.txt",'r') as f:
     line = f.readline()
@@ -1213,14 +1254,17 @@
 if opts.condor_nogrid_nonworker:
     cmd += " --condor-nogrid-nonworker "
 if opts.use_osg_simple_requirements:
     cmd += " --use-osg-simple-reqirements "
 if opts.archive_pesummary_label:
 #    cmd += " --plot-exe `which summarypages` --plot-args  args_plot.txt "
     cmd += " --plot-exe summarypages --plot-args  args_plot.txt "
+# Horribly annoying XPHM/XO4a fix because ChooseFDWaveform called.  Seems to be UNIVERSAL for the approximant name, but only if precessing
+if (opts.approx == 'IMRPhenomXPHM' or 'XO4a' in opts.approx) and opts.assume_precessing:
+    cmd += " --frame-rotation "
 print(cmd)
 os.system(cmd)
 
 if opts.use_osg_file_transfer and opts.internal_truncate_files_for_osg_file_transfer:
     # build truncated frames.  Note this parses ILE arguments, so must be done last
     os.system("util_ForOSG_MakeTruncatedLocalFramesDir.sh .")
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,20 @@
         for old_key in result.posterior.keys():
             if old_key in key_swap_dict:
                 result.posterior[key_swap_dict[old_key]] = result.posterior[old_key]
                 del result.posterior[old_key]
         # add tides if not present
         if not('lambda_1' in result.posterior):
             print(" Populating empty tidal params to avoid hang")
-            result.posterior['lambda_1'] = np.zeros(end_index-start_index)
-            result.posterior['lambda_2'] = np.zeros(end_index-start_index)
+            if end_index:
+              result.posterior['lambda_1'] = np.zeros(end_index-start_index)
+              result.posterior['lambda_2'] = np.zeros(end_index-start_index)
+            else:
+              result.posterior['lambda_1'] = np.zeros(len(result.posterior['mass_1']))
+              result.posterior['lambda_2'] = np.zeros(len(result.posterior['mass_1']))
 
 outdir = os.path.dirname(os.path.abspath(args.posterior_sample_file))
 
 ifos = data.interferometers
 time_marginalization_interval = args.time_marginalization_interval
 
 spline_calibration_envelope_dict = bilby_pipe.utils.convert_string_to_dict(
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc7
+Version: 0.0.15.8rc9
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
 MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
 MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
 MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
 MonteCarloMarginalizeCode/Code/bin/config_yank.py
 MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
 MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
 MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
 MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
 MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3114,24 +3114,31 @@
 
 
 ## Version protection
 #   Pull out arguments of the ModesFromPolarizations function
 #argist_FromPolarizations=lalsim.SimInspiralTDModesFromPolarizations.__doc__.split('->')[0].replace('SimInspiralTDModesFromPolarizations','').replace('REAL8','').replace('Dict','').replace('Approximant','').replace('(','').replace(')','').split(',')
 
 
-def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False, silent=True, **kwargs ):
+def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False, silent=True, fd_standoff_factor=0.964,no_condition=False,**kwargs ):
     """
     Generate the TD h_lm -2-spin-weighted spherical harmonic modes of a GW
     with parameters P. Returns a SphHarmTimeSeries, a linked-list of modes with
     a COMPLEX16TimeSeries and indices l and m for each node.
 
     The linked list will contain all modes with l <= Lmax
     and all values of m for these l.
 
     nr_polarization_convention : apply a factor -1 to all modes provided by lalsuite
+
+    fd_standoff_factor: for ChooseFDWaveform, reduce starting frequency P.fmin by this factor internally when generating.
+          FD waveform calculation implicitly assumes fmin is in the inspiral regime (if not you are making bad life choices).
+          Default value of 0.964 is based on changing inspiral duration by 10% (1.1^(3/8) ~ 1.036). Any constant factor will change
+          the inspiral duration by a factor (1./fd_standoff_factor)^(8/3) or so.
+
+    no_condition: disable conditioning (for ChooseFDModes specifically). For diagnostic plots on impact of/need for conditioning.
     """
     assert Lmax >= 2
 
     # Check that masses are not nan!
     assert (not np.isnan(P.m1)) and (not np.isnan(P.m2)), " masses are NaN "
 
     sign_factor = 1
@@ -3146,24 +3153,52 @@
        fNyq_offset = fNyq - P.deltaF
        # Argh: https://git.ligo.org/waveforms/reviews/imrphenomxhm-amplitude-recalibration/-/wikis/home#review-statement
        if P.approx == lalIMRPhenomXPHM and 'release' in kwargs:
            lalsim.SimInspiralWaveformParamsInsertPhenomXHMReleaseVersion(extra_params, kwargs['release'])
        hlms_struct = lalsim.SimInspiralChooseFDModes(P.m1, P.m2, \
                                                      P.s1x, P.s1y, P.s1z, \
                                                      P.s2x, P.s2y, P.s2z, \
-                                                     P.deltaF, P.fmin, fNyq, P.fref, P.phiref, P.dist, P.incl, extra_params, P.approx)
+                                                     P.deltaF, P.fmin*fd_standoff_factor, fNyq, P.fref, P.phiref, P.dist, P.incl, extra_params, P.approx)
        hlmsT = {}
        hlms = {}
        hlmsdict = SphHarmFrequencySeries_to_dict(hlms_struct,Lmax)
+       # Base taper, based on 1% of waveform length
+       ntaper = int(0.01*TDlen)  # fixed 1% of waveform length, at start
+       ntaper = np.max([ntaper, int(1./(P.fmin*P.deltaT))])  # require at least one waveform cycle of tapering; should never happen
+       vectaper= 0.5 - 0.5*np.cos(np.pi*np.arange(ntaper)/(1.*ntaper))
+
+       # Taper any wraparound that has happened after the peak
+       #    - Based on SimInspiralTDFromTD  https://git.ligo.org/lscsoft/lalsuite/-/blob/master/lalsimulation/lib/LALSimInspiral.c
+       tchirp = lalsim.SimInspiralChirpTimeBound(P.fmin, P.m1,P.m2, P.s1z, P.s2z)
+       s = lalsim.SimInspiralFinalBlackHoleSpinBound(P.s1z,P.s2z)
+       t_merge = lalsim.SimInspiralMergeTimeBound(P.m1,P.m2) + lalsim.SimInspiralRingdownTimeBound(P.m1+P.m2,s)
+       t_extra = 3./P.fmin
+       indx_crit = int(TDlen/2) + int((t_merge+t_extra)/P.deltaT)  # t_extra is a lot of time generally if fmin is low
+       if indx_crit + ntaper > TDlen:
+           indx_crit = TDlen - ntaper
+
        for mode in hlmsdict:
           hlmsdict[mode] = lal.ResizeCOMPLEX16FrequencySeries(hlmsdict[mode],0, TDlen)
           hlmsT[mode] = DataInverseFourier(hlmsdict[mode])
           hlmsT[mode].data.data = -1*hlmsT[mode].data.data
           hlmsT[mode].data.data = np.roll(hlmsT[mode].data.data,-int(hlmsT[mode].data.length/2))
           hlmsT[mode].epoch = -(hlmsT[mode].data.length*hlmsT[mode].deltaT/2)
+          if not(no_condition):
+              # Taper at the start of the segment
+              hlmsT[mode].data.data[:ntaper]*=vectaper
+              # Taper anything at the *end* of the segment. This could be  important when interacting with real data, which when wrapped is strongly discontinuous
+              #     - this generally will NOT taper everything, because some of the turn-on generally extends well past this
+              if TDlen-ntaper < indx_crit:
+                  # just multiply the very end by a small amount of tapering
+                  hlmsT[mode].data.data[TDlen-ntaper:]*=vectaper[::-1]
+              else:
+                  # zero out a a lot of time at the end, and taper time as we approach this critical extra time
+                  hlmsT[mode].data.data[indx_crit:indx_crit+ntaper] *= vectaper[::-1]
+                  hlmsT[mode].data.data[indx_crit+ntaper:] = 0
+
        if P.deltaF is not None:
           if not silent:
               print(hlmsT[mode].data.length,TDlen, " and in seconds ", hlmsT[mode].data.length*hlmsT[mode].deltaT,TDlen*P.deltaT, " with deltaT={} {}".format(hlmsT[mode].deltaT,P.deltaT))
           for mode in hlmsT:
              hlms[mode] = lal.ResizeCOMPLEX16TimeSeries(hlmsT[mode],0,TDlen)
        return hlms
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,15 +779,19 @@
         ile_job.add_opt("cache-file",cache_file)
 
     ile_job.add_var_opt("event")
 
     if not use_osg:
         ile_job.add_condor_cmd('getenv', 'True')
     else:
-        ile_job.add_condor_cmd('getenv', '*RIFT*')  # retrieve any RIFT commands -- specifically RIFT_LOWLATENCY
+        env_statement="*RIFT*"
+        # special-purpose  environment variable to help tweak remote execution/driver issues
+        if 'CUDA_LAUNCH_BLOCKING' in os.environ:
+            env_statement+= ",CUDA_LAUNCH_BLOCKING"
+        ile_job.add_condor_cmd('getenv', env_statement)  # retrieve any RIFT commands -- specifically RIFT_LOWLATENCY
     ile_job.add_condor_cmd('request_memory', str(request_memory)) 
     if not(request_disk is False):
         ile_job.add_condor_cmd('request_disk', str(request_disk)) 
     nGPUs =0
     requirements = []
     if request_gpu:
         nGPUs=1
```

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.8rc9/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/INSTALL.md` & `RIFT-0.0.15.8rc9/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.8rc9/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/Dockerfile` & `RIFT-0.0.15.8rc9/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
       python3.9 -m pip --no-cache-dir install -U \
       cupy-cuda117 \
       vegas \
       healpy \
       cython \
       pypandoc \
       NRSur7dq2 \
-      RIFT==0.0.15.7rc1 && \
+      RIFT==0.0.15.8rc7 && \
       python3.9 -c "import gwsurrogate; gwsurrogate.catalog.pull('NRHybSur3dq8'); gwsurrogate.catalog.pull('NRSur7dq4')"
 
 # Needs numpy to finish first:
 ENV GW_SURROGATE=/usr/local/lib64/python3.6/site-packages/gwsurrogate
 ENV CUPY_CACHE_IN_MEMORY=1
 
 # Directories we may want to bind
```

### Comparing `RIFT-0.0.15.8rc7/README.md` & `RIFT-0.0.15.8rc9/README.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/howto.md` & `RIFT-0.0.15.8rc9/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.8rc9/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/PKG-INFO` & `RIFT-0.0.15.8rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc7
+Version: 0.0.15.8rc9
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
```

### Comparing `RIFT-0.0.15.8rc7/setup.py` & `RIFT-0.0.15.8rc9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.8rc7", # do not build on OSX machine, side effects
+    version="0.0.15.8rc9", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

### Comparing `RIFT-0.0.15.8rc7/PACKAGING.md` & `RIFT-0.0.15.8rc9/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/LICENSE.md` & `RIFT-0.0.15.8rc9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/TROUBLESHOOTING.md` & `RIFT-0.0.15.8rc9/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc7/GETTING_STARTED.md` & `RIFT-0.0.15.8rc9/GETTING_STARTED.md`

 * *Files identical despite different names*

