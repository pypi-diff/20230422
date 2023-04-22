# Comparing `tmp/fmot-1.3.4-py3-none-any.whl.zip` & `tmp/fmot-1.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,148 +1,160 @@
-Zip file size: 208658 bytes, number of entries: 146
--rwxr-xr-x  2.0 unx     1355 b- defN 23-Mar-12 01:37 fmot/ENV_REQUIREMENTS.sh
--rwxr-xr-x  2.0 unx      129 b- defN 23-Mar-12 01:37 fmot/PY_REQUIREMENTS
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-12 01:37 fmot/VERSION
--rw-r--r--  2.0 unx      581 b- defN 23-Mar-12 01:37 fmot/__init__.py
--rw-r--r--  2.0 unx      370 b- defN 23-Mar-12 01:37 fmot/_open_docs.py
--rw-r--r--  2.0 unx     1611 b- defN 23-Mar-12 01:37 fmot/_supported_ops.py
--rw-r--r--  2.0 unx      929 b- defN 23-Mar-12 01:37 fmot/exceptions.py
--rw-r--r--  2.0 unx     1821 b- defN 23-Mar-12 01:37 fmot/execute_code.py
--rw-r--r--  2.0 unx       61 b- defN 23-Mar-12 01:37 fmot/functional.py
--rw-r--r--  2.0 unx     4945 b- defN 23-Mar-12 01:37 fmot/torchscript_utils.py
--rw-r--r--  2.0 unx       83 b- defN 23-Mar-12 01:37 fmot/beta/__init__.py
--rw-r--r--  2.0 unx     4169 b- defN 23-Mar-12 01:37 fmot/beta/amp.py
--rw-r--r--  2.0 unx    10740 b- defN 23-Mar-12 01:37 fmot/beta/auto_multiprecision.py
--rw-r--r--  2.0 unx     1166 b- defN 23-Mar-12 01:37 fmot/beta/quantize_part.py
--rw-r--r--  2.0 unx      200 b- defN 23-Mar-12 01:37 fmot/convert/__init__.py
--rw-r--r--  2.0 unx     2900 b- defN 23-Mar-12 01:37 fmot/convert/_convert_to_qat.py
--rw-r--r--  2.0 unx      807 b- defN 23-Mar-12 01:37 fmot/convert/configure.py
--rw-r--r--  2.0 unx    15003 b- defN 23-Mar-12 01:37 fmot/convert/conversion_api.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Mar-12 01:37 fmot/convert/default_mappings.py
--rw-r--r--  2.0 unx     9685 b- defN 23-Mar-12 01:37 fmot/convert/default_patchings.py
--rw-r--r--  2.0 unx      356 b- defN 23-Mar-12 01:37 fmot/convert/default_substitutions.py
--rw-r--r--  2.0 unx     4562 b- defN 23-Mar-12 01:37 fmot/convert/lut_registry.py
--rw-r--r--  2.0 unx     3383 b- defN 23-Mar-12 01:37 fmot/convert/mapping.py
--rw-r--r--  2.0 unx     2831 b- defN 23-Mar-12 01:37 fmot/convert/optimizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-12 01:37 fmot/convert/param_manager.py
--rw-r--r--  2.0 unx    24572 b- defN 23-Mar-12 01:37 fmot/convert/patch_ir.py
--rw-r--r--  2.0 unx     4116 b- defN 23-Mar-12 01:37 fmot/convert/patching.py
--rw-r--r--  2.0 unx     3234 b- defN 23-Mar-12 01:37 fmot/convert/prune_reparametrization.py
--rw-r--r--  2.0 unx     2963 b- defN 23-Mar-12 01:37 fmot/convert/quantizer_manager.py
--rw-r--r--  2.0 unx     2111 b- defN 23-Mar-12 01:37 fmot/convert/substitution.py
--rw-r--r--  2.0 unx      199 b- defN 23-Mar-12 01:37 fmot/fqir/__init__.py
--rw-r--r--  2.0 unx      660 b- defN 23-Mar-12 01:37 fmot/fqir/utils.py
--rw-r--r--  2.0 unx       35 b- defN 23-Mar-12 01:37 fmot/fqir/graph_proto/__init__.py
--rw-r--r--  2.0 unx    13785 b- defN 23-Mar-12 01:37 fmot/fqir/graph_proto/graph_proto.py
--rw-r--r--  2.0 unx     5214 b- defN 23-Mar-12 01:37 fmot/fqir/graph_proto/graph_runtime.py
--rw-r--r--  2.0 unx      115 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/__init__.py
--rw-r--r--  2.0 unx     5761 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/node_base.py
--rw-r--r--  2.0 unx     6731 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/node_proto.py
--rw-r--r--  2.0 unx     2207 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/opcount.py
--rw-r--r--  2.0 unx    20518 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/opcounters.py
--rw-r--r--  2.0 unx     6933 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/optype_base.py
--rw-r--r--  2.0 unx    33465 b- defN 23-Mar-12 01:37 fmot/fqir/nodes/optypes.py
--rw-r--r--  2.0 unx      398 b- defN 23-Mar-12 01:37 fmot/fqir/passes/__init__.py
--rw-r--r--  2.0 unx     7322 b- defN 23-Mar-12 01:37 fmot/fqir/passes/batchdim_removal.py
--rw-r--r--  2.0 unx      463 b- defN 23-Mar-12 01:37 fmot/fqir/passes/dimtag_removal.py
--rw-r--r--  2.0 unx     1160 b- defN 23-Mar-12 01:37 fmot/fqir/passes/helpers.py
--rw-r--r--  2.0 unx    19953 b- defN 23-Mar-12 01:37 fmot/fqir/passes/kernelize_lstm.py
--rw-r--r--  2.0 unx     2039 b- defN 23-Mar-12 01:37 fmot/fqir/passes/kernelize_temporal_unfold.py
--rw-r--r--  2.0 unx      657 b- defN 23-Mar-12 01:37 fmot/fqir/passes/uniquify_names.py
--rw-r--r--  2.0 unx       94 b- defN 23-Mar-12 01:37 fmot/fqir/variables/__init__.py
--rw-r--r--  2.0 unx     6255 b- defN 23-Mar-12 01:37 fmot/fqir/variables/tensor_proto.py
--rw-r--r--  2.0 unx     2064 b- defN 23-Mar-12 01:37 fmot/fqir/variables/variable_base.py
--rw-r--r--  2.0 unx      385 b- defN 23-Mar-12 01:37 fmot/nn/__init__.py
--rw-r--r--  2.0 unx     8315 b- defN 23-Mar-12 01:37 fmot/nn/atomics.py
--rw-r--r--  2.0 unx    11515 b- defN 23-Mar-12 01:37 fmot/nn/composites.py
--rw-r--r--  2.0 unx    27568 b- defN 23-Mar-12 01:37 fmot/nn/conv1d.py
--rw-r--r--  2.0 unx    21993 b- defN 23-Mar-12 01:37 fmot/nn/femtornn.py
--rw-r--r--  2.0 unx    10431 b- defN 23-Mar-12 01:37 fmot/nn/fft.py
--rw-r--r--  2.0 unx    31321 b- defN 23-Mar-12 01:37 fmot/nn/sequenced_rnn.py
--rw-r--r--  2.0 unx     5092 b- defN 23-Mar-12 01:37 fmot/nn/sequencer.py
--rw-r--r--  2.0 unx    19424 b- defN 23-Mar-12 01:37 fmot/nn/signal.py
--rw-r--r--  2.0 unx     9256 b- defN 23-Mar-12 01:37 fmot/nn/sparsifiers.py
--rw-r--r--  2.0 unx     2294 b- defN 23-Mar-12 01:37 fmot/nn/sru.py
--rw-r--r--  2.0 unx     6028 b- defN 23-Mar-12 01:37 fmot/nn/stft.py
--rw-r--r--  2.0 unx     1525 b- defN 23-Mar-12 01:37 fmot/nn/super_structures.py
--rw-r--r--  2.0 unx      192 b- defN 23-Mar-12 01:37 fmot/qat/__init__.py
--rw-r--r--  2.0 unx     4059 b- defN 23-Mar-12 01:37 fmot/qat/annotated_tensors.py
--rw-r--r--  2.0 unx     1659 b- defN 23-Mar-12 01:37 fmot/qat/bitwidths.py
--rw-r--r--  2.0 unx     4381 b- defN 23-Mar-12 01:37 fmot/qat/control.py
--rw-r--r--  2.0 unx     2684 b- defN 23-Mar-12 01:37 fmot/qat/fake_quantization.py
--rw-r--r--  2.0 unx      279 b- defN 23-Mar-12 01:37 fmot/qat/nn/__init__.py
--rw-r--r--  2.0 unx      276 b- defN 23-Mar-12 01:37 fmot/qat/nn/_utils.py
--rw-r--r--  2.0 unx     3783 b- defN 23-Mar-12 01:37 fmot/qat/nn/act_density.py
--rw-r--r--  2.0 unx    28123 b- defN 23-Mar-12 01:37 fmot/qat/nn/atomics.py
--rw-r--r--  2.0 unx     9167 b- defN 23-Mar-12 01:37 fmot/qat/nn/composites.py
--rw-r--r--  2.0 unx    10426 b- defN 23-Mar-12 01:37 fmot/qat/nn/density_matmul.py
--rw-r--r--  2.0 unx    13703 b- defN 23-Mar-12 01:37 fmot/qat/nn/high_level.py
--rw-r--r--  2.0 unx     3210 b- defN 23-Mar-12 01:37 fmot/qat/nn/linear.py
--rw-r--r--  2.0 unx    19301 b- defN 23-Mar-12 01:37 fmot/qat/nn/lstm.py
--rw-r--r--  2.0 unx    13738 b- defN 23-Mar-12 01:37 fmot/qat/nn/luts.py
--rw-r--r--  2.0 unx     3922 b- defN 23-Mar-12 01:37 fmot/qat/nn/norm.py
--rw-r--r--  2.0 unx     1350 b- defN 23-Mar-12 01:37 fmot/qat/nn/quant_wrap.py
--rw-r--r--  2.0 unx    21181 b- defN 23-Mar-12 01:37 fmot/qat/nn/quantizers.py
--rw-r--r--  2.0 unx     1992 b- defN 23-Mar-12 01:37 fmot/qat/nn/sequencer.py
--rw-r--r--  2.0 unx       90 b- defN 23-Mar-12 01:37 fmot/sparse/__init__.py
--rw-r--r--  2.0 unx     2657 b- defN 23-Mar-12 01:37 fmot/sparse/act_pruning.py
--rw-r--r--  2.0 unx     7357 b- defN 23-Mar-12 01:37 fmot/sparse/pruning.py
--rw-r--r--  2.0 unx     4024 b- defN 23-Mar-12 01:37 fmot/sparse/pruning_schedulers.py
--rw-r--r--  2.0 unx     7162 b- defN 23-Mar-12 01:37 fmot/sparse/pruning_utils.py
--rw-r--r--  2.0 unx      196 b- defN 23-Mar-12 01:37 fmot/test/__init__.py
--rw-r--r--  2.0 unx     5861 b- defN 23-Mar-12 01:37 fmot/test/ds_tc_resnet.py
--rw-r--r--  2.0 unx     3000 b- defN 23-Mar-12 01:37 fmot/test/kws_test_library.py
--rw-r--r--  2.0 unx      936 b- defN 23-Mar-12 01:37 fmot/test/test_automp.py
--rw-r--r--  2.0 unx     1373 b- defN 23-Mar-12 01:37 fmot/test/test_cqt.py
--rw-r--r--  2.0 unx     1688 b- defN 23-Mar-12 01:37 fmot/test/test_cuda.py
--rw-r--r--  2.0 unx     3878 b- defN 23-Mar-12 01:37 fmot/test/test_density_tracking.py
--rw-r--r--  2.0 unx     1134 b- defN 23-Mar-12 01:37 fmot/test/test_diagnosis.py
--rw-r--r--  2.0 unx     3411 b- defN 23-Mar-12 01:37 fmot/test/test_dim_anno.py
--rw-r--r--  2.0 unx      958 b- defN 23-Mar-12 01:37 fmot/test/test_dropout.py
--rw-r--r--  2.0 unx    14190 b- defN 23-Mar-12 01:37 fmot/test/test_features.py
--rw-r--r--  2.0 unx      323 b- defN 23-Mar-12 01:37 fmot/test/test_fft.py
--rw-r--r--  2.0 unx     3581 b- defN 23-Mar-12 01:37 fmot/test/test_nn_stft.py
--rw-r--r--  2.0 unx     2347 b- defN 23-Mar-12 01:37 fmot/test/test_observers.py
--rw-r--r--  2.0 unx      310 b- defN 23-Mar-12 01:37 fmot/test/test_package.py
--rw-r--r--  2.0 unx     1240 b- defN 23-Mar-12 01:37 fmot/test/test_param_reuse.py
--rw-r--r--  2.0 unx      830 b- defN 23-Mar-12 01:37 fmot/test/test_precision_mod.py
--rw-r--r--  2.0 unx     6440 b- defN 23-Mar-12 01:37 fmot/test/test_pruning.py
--rw-r--r--  2.0 unx    25081 b- defN 23-Mar-12 01:37 fmot/test/test_sequencers.py
--rw-r--r--  2.0 unx     2017 b- defN 23-Mar-12 01:37 fmot/test/test_serialization.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-12 01:37 fmot/test/test_fqir/__init__.py
--rw-r--r--  2.0 unx     1657 b- defN 23-Mar-12 01:37 fmot/test/test_fqir/test_opchecks.py
--rw-r--r--  2.0 unx     1138 b- defN 23-Mar-12 01:37 fmot/test/test_fqir/test_readme.py
--rw-r--r--  2.0 unx    15396 b- defN 23-Mar-12 01:37 fmot/test/test_fqir/test_single_ops.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-12 01:37 fmot/test/utm/__init__.py
--rw-r--r--  2.0 unx    13543 b- defN 23-Mar-12 01:37 fmot/test/utm/atomic_test_library.py
--rw-r--r--  2.0 unx     4280 b- defN 23-Mar-12 01:37 fmot/test/utm/feedforward_test_library.py
--rw-r--r--  2.0 unx      990 b- defN 23-Mar-12 01:37 fmot/test/utm/get_utms.py
--rw-r--r--  2.0 unx     2284 b- defN 23-Mar-12 01:37 fmot/test/utm/plot_errors.py
--rw-r--r--  2.0 unx     3589 b- defN 23-Mar-12 01:37 fmot/test/utm/quant_tolerances.py
--rw-r--r--  2.0 unx     9964 b- defN 23-Mar-12 01:37 fmot/test/utm/rnn_test_library.py
--rw-r--r--  2.0 unx      173 b- defN 23-Mar-12 01:37 fmot/test/utm/test_utm_converted_runtime.py
--rw-r--r--  2.0 unx      340 b- defN 23-Mar-12 01:37 fmot/test/utm/test_utm_fqir_runtime.py
--rw-r--r--  2.0 unx      316 b- defN 23-Mar-12 01:37 fmot/test/utm/test_utm_mixed_precision.py
--rw-r--r--  2.0 unx      587 b- defN 23-Mar-12 01:37 fmot/test/utm/test_utm_quantization_error.py
--rw-r--r--  2.0 unx    11995 b- defN 23-Mar-12 01:37 fmot/test/utm/unittest_objects.py
--rw-r--r--  2.0 unx       90 b- defN 23-Mar-12 01:37 fmot/tracing/__init__.py
--rw-r--r--  2.0 unx     1743 b- defN 23-Mar-12 01:37 fmot/tracing/oplinks_v1.py
--rw-r--r--  2.0 unx    22779 b- defN 23-Mar-12 01:37 fmot/tracing/tracing.py
--rw-r--r--  2.0 unx      344 b- defN 23-Mar-12 01:37 fmot/tracing/tracing_blacklist.py
--rw-r--r--  2.0 unx     2017 b- defN 23-Mar-12 01:37 fmot/tracing/utils.py
--rw-r--r--  2.0 unx      325 b- defN 23-Mar-12 01:37 fmot/utils/__init__.py
--rw-r--r--  2.0 unx     3941 b- defN 23-Mar-12 01:37 fmot/utils/activity.py
--rw-r--r--  2.0 unx     3089 b- defN 23-Mar-12 01:37 fmot/utils/conv1d_utils.py
--rw-r--r--  2.0 unx     2245 b- defN 23-Mar-12 01:37 fmot/utils/param_manager.py
--rw-r--r--  2.0 unx     6744 b- defN 23-Mar-12 01:37 fmot/utils/quant_diagnostic.py
--rw-r--r--  2.0 unx     1792 b- defN 23-Mar-12 01:37 fmot/utils/quantizer_manager.py
--rw-r--r--  2.0 unx      357 b- defN 23-Mar-12 01:37 fmot/utils/rich_attr.py
--rw-r--r--  2.0 unx     9783 b- defN 23-Mar-12 01:37 fmot/utils/saturation_opt.py
--rw-r--r--  2.0 unx     1986 b- defN 23-Mar-12 01:37 fmot/utils/serialization.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-12 01:37 fmot/utils/quant_tools/__init__.py
--rw-r--r--  2.0 unx     4118 b- defN 23-Mar-12 01:37 fmot/utils/quant_tools/diagnosis.py
--rwxr-xr-x  2.0 unx       36 b- defN 23-Mar-12 01:40 fmot-1.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3657 b- defN 23-Mar-12 01:40 fmot-1.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 01:40 fmot-1.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Mar-12 01:40 fmot-1.3.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    12139 b- defN 23-Mar-12 01:40 fmot-1.3.4.dist-info/RECORD
-146 files, 785404 bytes uncompressed, 189718 bytes compressed:  75.8%
+Zip file size: 222191 bytes, number of entries: 158
+-rwxr-xr-x  2.0 unx     1355 b- defN 23-Apr-22 01:51 fmot/ENV_REQUIREMENTS.sh
+-rwxr-xr-x  2.0 unx      138 b- defN 23-Apr-22 01:51 fmot/PY_REQUIREMENTS
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-22 01:51 fmot/VERSION
+-rw-r--r--  2.0 unx      648 b- defN 23-Apr-22 01:51 fmot/__init__.py
+-rw-r--r--  2.0 unx      414 b- defN 23-Apr-22 01:51 fmot/_open_docs.py
+-rw-r--r--  2.0 unx     1611 b- defN 23-Apr-22 01:51 fmot/_supported_ops.py
+-rw-r--r--  2.0 unx     1654 b- defN 23-Apr-22 01:51 fmot/configure.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Apr-22 01:51 fmot/exceptions.py
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-22 01:51 fmot/execute_code.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Apr-22 01:51 fmot/functional.py
+-rw-r--r--  2.0 unx     4945 b- defN 23-Apr-22 01:51 fmot/torchscript_utils.py
+-rw-r--r--  2.0 unx       83 b- defN 23-Apr-22 01:51 fmot/beta/__init__.py
+-rw-r--r--  2.0 unx     4169 b- defN 23-Apr-22 01:51 fmot/beta/amp.py
+-rw-r--r--  2.0 unx    10740 b- defN 23-Apr-22 01:51 fmot/beta/auto_multiprecision.py
+-rw-r--r--  2.0 unx     1166 b- defN 23-Apr-22 01:51 fmot/beta/quantize_part.py
+-rw-r--r--  2.0 unx      200 b- defN 23-Apr-22 01:51 fmot/convert/__init__.py
+-rw-r--r--  2.0 unx     2900 b- defN 23-Apr-22 01:51 fmot/convert/_convert_to_qat.py
+-rw-r--r--  2.0 unx    15168 b- defN 23-Apr-22 01:51 fmot/convert/conversion_api.py
+-rw-r--r--  2.0 unx     2410 b- defN 23-Apr-22 01:51 fmot/convert/default_mappings.py
+-rw-r--r--  2.0 unx     9684 b- defN 23-Apr-22 01:51 fmot/convert/default_patchings.py
+-rw-r--r--  2.0 unx      547 b- defN 23-Apr-22 01:51 fmot/convert/default_substitutions.py
+-rw-r--r--  2.0 unx     4562 b- defN 23-Apr-22 01:51 fmot/convert/lut_registry.py
+-rw-r--r--  2.0 unx     3998 b- defN 23-Apr-22 01:51 fmot/convert/mapping.py
+-rw-r--r--  2.0 unx     2831 b- defN 23-Apr-22 01:51 fmot/convert/optimizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-22 01:51 fmot/convert/param_manager.py
+-rw-r--r--  2.0 unx    24680 b- defN 23-Apr-22 01:51 fmot/convert/patch_ir.py
+-rw-r--r--  2.0 unx     4175 b- defN 23-Apr-22 01:51 fmot/convert/patching.py
+-rw-r--r--  2.0 unx     3244 b- defN 23-Apr-22 01:51 fmot/convert/prune_reparametrization.py
+-rw-r--r--  2.0 unx     2963 b- defN 23-Apr-22 01:51 fmot/convert/quantizer_manager.py
+-rw-r--r--  2.0 unx     2121 b- defN 23-Apr-22 01:51 fmot/convert/substitution.py
+-rw-r--r--  2.0 unx      199 b- defN 23-Apr-22 01:51 fmot/fqir/__init__.py
+-rw-r--r--  2.0 unx      660 b- defN 23-Apr-22 01:51 fmot/fqir/utils.py
+-rw-r--r--  2.0 unx       35 b- defN 23-Apr-22 01:51 fmot/fqir/graph_proto/__init__.py
+-rw-r--r--  2.0 unx    13950 b- defN 23-Apr-22 01:51 fmot/fqir/graph_proto/graph_proto.py
+-rw-r--r--  2.0 unx     5303 b- defN 23-Apr-22 01:51 fmot/fqir/graph_proto/graph_runtime.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/__init__.py
+-rw-r--r--  2.0 unx     5761 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/node_base.py
+-rw-r--r--  2.0 unx     6920 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/node_proto.py
+-rw-r--r--  2.0 unx     2207 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/opcount.py
+-rw-r--r--  2.0 unx    20518 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/opcounters.py
+-rw-r--r--  2.0 unx     7008 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/optype_base.py
+-rw-r--r--  2.0 unx    30178 b- defN 23-Apr-22 01:51 fmot/fqir/nodes/optypes.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Apr-22 01:51 fmot/fqir/passes/__init__.py
+-rw-r--r--  2.0 unx     7322 b- defN 23-Apr-22 01:51 fmot/fqir/passes/batchdim_removal.py
+-rw-r--r--  2.0 unx     1606 b- defN 23-Apr-22 01:51 fmot/fqir/passes/cleanup.py
+-rw-r--r--  2.0 unx      463 b- defN 23-Apr-22 01:51 fmot/fqir/passes/dimtag_removal.py
+-rw-r--r--  2.0 unx     1160 b- defN 23-Apr-22 01:51 fmot/fqir/passes/helpers.py
+-rw-r--r--  2.0 unx    19971 b- defN 23-Apr-22 01:51 fmot/fqir/passes/kernelize_lstm.py
+-rw-r--r--  2.0 unx     5496 b- defN 23-Apr-22 01:51 fmot/fqir/passes/kernelize_red_broad.py
+-rw-r--r--  2.0 unx     2039 b- defN 23-Apr-22 01:51 fmot/fqir/passes/kernelize_temporal_unfold.py
+-rw-r--r--  2.0 unx       94 b- defN 23-Apr-22 01:51 fmot/fqir/variables/__init__.py
+-rw-r--r--  2.0 unx     6255 b- defN 23-Apr-22 01:51 fmot/fqir/variables/tensor_proto.py
+-rw-r--r--  2.0 unx     2064 b- defN 23-Apr-22 01:51 fmot/fqir/variables/variable_base.py
+-rw-r--r--  2.0 unx      563 b- defN 23-Apr-22 01:51 fmot/nn/__init__.py
+-rw-r--r--  2.0 unx     8663 b- defN 23-Apr-22 01:51 fmot/nn/atomics.py
+-rw-r--r--  2.0 unx    12272 b- defN 23-Apr-22 01:51 fmot/nn/composites.py
+-rw-r--r--  2.0 unx    27568 b- defN 23-Apr-22 01:51 fmot/nn/conv1d.py
+-rw-r--r--  2.0 unx     1844 b- defN 23-Apr-22 01:51 fmot/nn/derived_param.py
+-rw-r--r--  2.0 unx    21993 b- defN 23-Apr-22 01:51 fmot/nn/femtornn.py
+-rw-r--r--  2.0 unx    17526 b- defN 23-Apr-22 01:51 fmot/nn/fft.py
+-rw-r--r--  2.0 unx    34238 b- defN 23-Apr-22 01:51 fmot/nn/sequenced_rnn.py
+-rw-r--r--  2.0 unx     5305 b- defN 23-Apr-22 01:51 fmot/nn/sequencer.py
+-rw-r--r--  2.0 unx    11986 b- defN 23-Apr-22 01:51 fmot/nn/signal_processing.py
+-rw-r--r--  2.0 unx     3742 b- defN 23-Apr-22 01:51 fmot/nn/sliding_attention.py
+-rw-r--r--  2.0 unx     9256 b- defN 23-Apr-22 01:51 fmot/nn/sparsifiers.py
+-rw-r--r--  2.0 unx     2294 b- defN 23-Apr-22 01:51 fmot/nn/sru.py
+-rw-r--r--  2.0 unx     8916 b- defN 23-Apr-22 01:51 fmot/nn/stft.py
+-rw-r--r--  2.0 unx     1525 b- defN 23-Apr-22 01:51 fmot/nn/super_structures.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Apr-22 01:51 fmot/nn/temporal_unfold.py
+-rw-r--r--  2.0 unx      192 b- defN 23-Apr-22 01:51 fmot/qat/__init__.py
+-rw-r--r--  2.0 unx     4059 b- defN 23-Apr-22 01:51 fmot/qat/annotated_tensors.py
+-rw-r--r--  2.0 unx     1659 b- defN 23-Apr-22 01:51 fmot/qat/bitwidths.py
+-rw-r--r--  2.0 unx     4381 b- defN 23-Apr-22 01:51 fmot/qat/control.py
+-rw-r--r--  2.0 unx     2684 b- defN 23-Apr-22 01:51 fmot/qat/fake_quantization.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Apr-22 01:51 fmot/qat/nn/__init__.py
+-rw-r--r--  2.0 unx      276 b- defN 23-Apr-22 01:51 fmot/qat/nn/_utils.py
+-rw-r--r--  2.0 unx     3783 b- defN 23-Apr-22 01:51 fmot/qat/nn/act_density.py
+-rw-r--r--  2.0 unx    28153 b- defN 23-Apr-22 01:51 fmot/qat/nn/atomics.py
+-rw-r--r--  2.0 unx     9198 b- defN 23-Apr-22 01:51 fmot/qat/nn/composites.py
+-rw-r--r--  2.0 unx    10828 b- defN 23-Apr-22 01:51 fmot/qat/nn/density_matmul.py
+-rw-r--r--  2.0 unx     2102 b- defN 23-Apr-22 01:51 fmot/qat/nn/derived_param.py
+-rw-r--r--  2.0 unx     8923 b- defN 23-Apr-22 01:51 fmot/qat/nn/linear.py
+-rw-r--r--  2.0 unx    19303 b- defN 23-Apr-22 01:51 fmot/qat/nn/lstm.py
+-rw-r--r--  2.0 unx    14400 b- defN 23-Apr-22 01:51 fmot/qat/nn/luts.py
+-rw-r--r--  2.0 unx     3922 b- defN 23-Apr-22 01:51 fmot/qat/nn/norm.py
+-rw-r--r--  2.0 unx     1350 b- defN 23-Apr-22 01:51 fmot/qat/nn/quant_wrap.py
+-rw-r--r--  2.0 unx    22679 b- defN 23-Apr-22 01:51 fmot/qat/nn/quantizers.py
+-rw-r--r--  2.0 unx     1992 b- defN 23-Apr-22 01:51 fmot/qat/nn/sequencer.py
+-rw-r--r--  2.0 unx     2283 b- defN 23-Apr-22 01:51 fmot/qat/nn/temporal_unfold.py
+-rw-r--r--  2.0 unx     1007 b- defN 23-Apr-22 01:51 fmot/qat/nn/tuning_eps.py
+-rw-r--r--  2.0 unx       90 b- defN 23-Apr-22 01:51 fmot/sparse/__init__.py
+-rw-r--r--  2.0 unx     2694 b- defN 23-Apr-22 01:51 fmot/sparse/act_pruning.py
+-rw-r--r--  2.0 unx     7357 b- defN 23-Apr-22 01:51 fmot/sparse/pruning.py
+-rw-r--r--  2.0 unx     4024 b- defN 23-Apr-22 01:51 fmot/sparse/pruning_schedulers.py
+-rw-r--r--  2.0 unx     7162 b- defN 23-Apr-22 01:51 fmot/sparse/pruning_utils.py
+-rw-r--r--  2.0 unx      196 b- defN 23-Apr-22 01:51 fmot/test/__init__.py
+-rw-r--r--  2.0 unx     5861 b- defN 23-Apr-22 01:51 fmot/test/ds_tc_resnet.py
+-rw-r--r--  2.0 unx     3000 b- defN 23-Apr-22 01:51 fmot/test/kws_test_library.py
+-rw-r--r--  2.0 unx      936 b- defN 23-Apr-22 01:51 fmot/test/test_automp.py
+-rw-r--r--  2.0 unx     1373 b- defN 23-Apr-22 01:51 fmot/test/test_cqt.py
+-rw-r--r--  2.0 unx     1688 b- defN 23-Apr-22 01:51 fmot/test/test_cuda.py
+-rw-r--r--  2.0 unx     3878 b- defN 23-Apr-22 01:51 fmot/test/test_density_tracking.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Apr-22 01:51 fmot/test/test_diagnosis.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Apr-22 01:51 fmot/test/test_dim_anno.py
+-rw-r--r--  2.0 unx      958 b- defN 23-Apr-22 01:51 fmot/test/test_dropout.py
+-rw-r--r--  2.0 unx    14304 b- defN 23-Apr-22 01:51 fmot/test/test_features.py
+-rw-r--r--  2.0 unx      722 b- defN 23-Apr-22 01:51 fmot/test/test_fft.py
+-rw-r--r--  2.0 unx     1664 b- defN 23-Apr-22 01:51 fmot/test/test_ifft.py
+-rw-r--r--  2.0 unx      378 b- defN 23-Apr-22 01:51 fmot/test/test_layernorm.py
+-rw-r--r--  2.0 unx     1412 b- defN 23-Apr-22 01:51 fmot/test/test_lut_grads.py
+-rw-r--r--  2.0 unx     3581 b- defN 23-Apr-22 01:51 fmot/test/test_nn_stft.py
+-rw-r--r--  2.0 unx     2347 b- defN 23-Apr-22 01:51 fmot/test/test_observers.py
+-rw-r--r--  2.0 unx      310 b- defN 23-Apr-22 01:51 fmot/test/test_package.py
+-rw-r--r--  2.0 unx     1240 b- defN 23-Apr-22 01:51 fmot/test/test_param_reuse.py
+-rw-r--r--  2.0 unx      830 b- defN 23-Apr-22 01:51 fmot/test/test_precision_mod.py
+-rw-r--r--  2.0 unx     6440 b- defN 23-Apr-22 01:51 fmot/test/test_pruning.py
+-rw-r--r--  2.0 unx    25171 b- defN 23-Apr-22 01:51 fmot/test/test_sequencers.py
+-rw-r--r--  2.0 unx     2017 b- defN 23-Apr-22 01:51 fmot/test/test_serialization.py
+-rw-r--r--  2.0 unx     4308 b- defN 23-Apr-22 01:51 fmot/test/test_stft.py
+-rw-r--r--  2.0 unx     1322 b- defN 23-Apr-22 01:51 fmot/test/test_temporal_unfold.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-22 01:51 fmot/test/test_fqir/__init__.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Apr-22 01:51 fmot/test/test_fqir/test_opchecks.py
+-rw-r--r--  2.0 unx     1138 b- defN 23-Apr-22 01:51 fmot/test/test_fqir/test_readme.py
+-rw-r--r--  2.0 unx    15396 b- defN 23-Apr-22 01:51 fmot/test/test_fqir/test_single_ops.py
+-rw-r--r--  2.0 unx      147 b- defN 23-Apr-22 01:51 fmot/test/utm/__init__.py
+-rw-r--r--  2.0 unx    13543 b- defN 23-Apr-22 01:51 fmot/test/utm/atomic_test_library.py
+-rw-r--r--  2.0 unx     5731 b- defN 23-Apr-22 01:51 fmot/test/utm/feedforward_test_library.py
+-rw-r--r--  2.0 unx      990 b- defN 23-Apr-22 01:51 fmot/test/utm/get_utms.py
+-rw-r--r--  2.0 unx     2284 b- defN 23-Apr-22 01:51 fmot/test/utm/plot_errors.py
+-rw-r--r--  2.0 unx     3603 b- defN 23-Apr-22 01:51 fmot/test/utm/quant_tolerances.py
+-rw-r--r--  2.0 unx    10015 b- defN 23-Apr-22 01:51 fmot/test/utm/rnn_test_library.py
+-rw-r--r--  2.0 unx      173 b- defN 23-Apr-22 01:51 fmot/test/utm/test_utm_converted_runtime.py
+-rw-r--r--  2.0 unx      340 b- defN 23-Apr-22 01:51 fmot/test/utm/test_utm_fqir_runtime.py
+-rw-r--r--  2.0 unx      316 b- defN 23-Apr-22 01:51 fmot/test/utm/test_utm_mixed_precision.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Apr-22 01:51 fmot/test/utm/test_utm_quantization_error.py
+-rw-r--r--  2.0 unx    12337 b- defN 23-Apr-22 01:51 fmot/test/utm/unittest_objects.py
+-rw-r--r--  2.0 unx       90 b- defN 23-Apr-22 01:51 fmot/tracing/__init__.py
+-rw-r--r--  2.0 unx     2699 b- defN 23-Apr-22 01:51 fmot/tracing/compare_fqir.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-Apr-22 01:51 fmot/tracing/oplinks_v1.py
+-rw-r--r--  2.0 unx    23682 b- defN 23-Apr-22 01:51 fmot/tracing/tracing.py
+-rw-r--r--  2.0 unx      365 b- defN 23-Apr-22 01:51 fmot/tracing/tracing_blacklist.py
+-rw-r--r--  2.0 unx     2017 b- defN 23-Apr-22 01:51 fmot/tracing/utils.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Apr-22 01:51 fmot/utils/__init__.py
+-rw-r--r--  2.0 unx     3941 b- defN 23-Apr-22 01:51 fmot/utils/activity.py
+-rw-r--r--  2.0 unx     3089 b- defN 23-Apr-22 01:51 fmot/utils/conv1d_utils.py
+-rw-r--r--  2.0 unx     2245 b- defN 23-Apr-22 01:51 fmot/utils/param_manager.py
+-rw-r--r--  2.0 unx     6744 b- defN 23-Apr-22 01:51 fmot/utils/quant_diagnostic.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-Apr-22 01:51 fmot/utils/quantizer_manager.py
+-rw-r--r--  2.0 unx      357 b- defN 23-Apr-22 01:51 fmot/utils/rich_attr.py
+-rw-r--r--  2.0 unx     8372 b- defN 23-Apr-22 01:51 fmot/utils/saturation_opt.py
+-rw-r--r--  2.0 unx     1986 b- defN 23-Apr-22 01:51 fmot/utils/serialization.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-22 01:51 fmot/utils/quant_tools/__init__.py
+-rw-r--r--  2.0 unx     4545 b- defN 23-Apr-22 01:51 fmot/utils/quant_tools/diagnosis.py
+-rwxr-xr-x  2.0 unx       36 b- defN 23-Apr-22 01:55 fmot-1.5.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3668 b- defN 23-Apr-22 01:55 fmot-1.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 01:55 fmot-1.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-22 01:55 fmot-1.5.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    13156 b- defN 23-Apr-22 01:55 fmot-1.5.6.dist-info/RECORD
+158 files, 820588 bytes uncompressed, 201679 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: fmot/_open_docs.py
 Comment: 
 
 Filename: fmot/_supported_ops.py
 Comment: 
 
+Filename: fmot/configure.py
+Comment: 
+
 Filename: fmot/exceptions.py
 Comment: 
 
 Filename: fmot/execute_code.py
 Comment: 
 
 Filename: fmot/functional.py
@@ -42,17 +45,14 @@
 
 Filename: fmot/convert/__init__.py
 Comment: 
 
 Filename: fmot/convert/_convert_to_qat.py
 Comment: 
 
-Filename: fmot/convert/configure.py
-Comment: 
-
 Filename: fmot/convert/conversion_api.py
 Comment: 
 
 Filename: fmot/convert/default_mappings.py
 Comment: 
 
 Filename: fmot/convert/default_patchings.py
@@ -126,27 +126,30 @@
 
 Filename: fmot/fqir/passes/__init__.py
 Comment: 
 
 Filename: fmot/fqir/passes/batchdim_removal.py
 Comment: 
 
+Filename: fmot/fqir/passes/cleanup.py
+Comment: 
+
 Filename: fmot/fqir/passes/dimtag_removal.py
 Comment: 
 
 Filename: fmot/fqir/passes/helpers.py
 Comment: 
 
 Filename: fmot/fqir/passes/kernelize_lstm.py
 Comment: 
 
-Filename: fmot/fqir/passes/kernelize_temporal_unfold.py
+Filename: fmot/fqir/passes/kernelize_red_broad.py
 Comment: 
 
-Filename: fmot/fqir/passes/uniquify_names.py
+Filename: fmot/fqir/passes/kernelize_temporal_unfold.py
 Comment: 
 
 Filename: fmot/fqir/variables/__init__.py
 Comment: 
 
 Filename: fmot/fqir/variables/tensor_proto.py
 Comment: 
@@ -162,41 +165,50 @@
 
 Filename: fmot/nn/composites.py
 Comment: 
 
 Filename: fmot/nn/conv1d.py
 Comment: 
 
+Filename: fmot/nn/derived_param.py
+Comment: 
+
 Filename: fmot/nn/femtornn.py
 Comment: 
 
 Filename: fmot/nn/fft.py
 Comment: 
 
 Filename: fmot/nn/sequenced_rnn.py
 Comment: 
 
 Filename: fmot/nn/sequencer.py
 Comment: 
 
-Filename: fmot/nn/signal.py
+Filename: fmot/nn/signal_processing.py
+Comment: 
+
+Filename: fmot/nn/sliding_attention.py
 Comment: 
 
 Filename: fmot/nn/sparsifiers.py
 Comment: 
 
 Filename: fmot/nn/sru.py
 Comment: 
 
 Filename: fmot/nn/stft.py
 Comment: 
 
 Filename: fmot/nn/super_structures.py
 Comment: 
 
+Filename: fmot/nn/temporal_unfold.py
+Comment: 
+
 Filename: fmot/qat/__init__.py
 Comment: 
 
 Filename: fmot/qat/annotated_tensors.py
 Comment: 
 
 Filename: fmot/qat/bitwidths.py
@@ -222,15 +234,15 @@
 
 Filename: fmot/qat/nn/composites.py
 Comment: 
 
 Filename: fmot/qat/nn/density_matmul.py
 Comment: 
 
-Filename: fmot/qat/nn/high_level.py
+Filename: fmot/qat/nn/derived_param.py
 Comment: 
 
 Filename: fmot/qat/nn/linear.py
 Comment: 
 
 Filename: fmot/qat/nn/lstm.py
 Comment: 
@@ -246,14 +258,20 @@
 
 Filename: fmot/qat/nn/quantizers.py
 Comment: 
 
 Filename: fmot/qat/nn/sequencer.py
 Comment: 
 
+Filename: fmot/qat/nn/temporal_unfold.py
+Comment: 
+
+Filename: fmot/qat/nn/tuning_eps.py
+Comment: 
+
 Filename: fmot/sparse/__init__.py
 Comment: 
 
 Filename: fmot/sparse/act_pruning.py
 Comment: 
 
 Filename: fmot/sparse/pruning.py
@@ -297,14 +315,23 @@
 
 Filename: fmot/test/test_features.py
 Comment: 
 
 Filename: fmot/test/test_fft.py
 Comment: 
 
+Filename: fmot/test/test_ifft.py
+Comment: 
+
+Filename: fmot/test/test_layernorm.py
+Comment: 
+
+Filename: fmot/test/test_lut_grads.py
+Comment: 
+
 Filename: fmot/test/test_nn_stft.py
 Comment: 
 
 Filename: fmot/test/test_observers.py
 Comment: 
 
 Filename: fmot/test/test_package.py
@@ -321,14 +348,20 @@
 
 Filename: fmot/test/test_sequencers.py
 Comment: 
 
 Filename: fmot/test/test_serialization.py
 Comment: 
 
+Filename: fmot/test/test_stft.py
+Comment: 
+
+Filename: fmot/test/test_temporal_unfold.py
+Comment: 
+
 Filename: fmot/test/test_fqir/__init__.py
 Comment: 
 
 Filename: fmot/test/test_fqir/test_opchecks.py
 Comment: 
 
 Filename: fmot/test/test_fqir/test_readme.py
@@ -372,14 +405,17 @@
 
 Filename: fmot/test/utm/unittest_objects.py
 Comment: 
 
 Filename: fmot/tracing/__init__.py
 Comment: 
 
+Filename: fmot/tracing/compare_fqir.py
+Comment: 
+
 Filename: fmot/tracing/oplinks_v1.py
 Comment: 
 
 Filename: fmot/tracing/tracing.py
 Comment: 
 
 Filename: fmot/tracing/tracing_blacklist.py
@@ -417,23 +453,23 @@
 
 Filename: fmot/utils/quant_tools/__init__.py
 Comment: 
 
 Filename: fmot/utils/quant_tools/diagnosis.py
 Comment: 
 
-Filename: fmot-1.3.4.dist-info/LICENSE
+Filename: fmot-1.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: fmot-1.3.4.dist-info/METADATA
+Filename: fmot-1.5.6.dist-info/METADATA
 Comment: 
 
-Filename: fmot-1.3.4.dist-info/WHEEL
+Filename: fmot-1.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: fmot-1.3.4.dist-info/top_level.txt
+Filename: fmot-1.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: fmot-1.3.4.dist-info/RECORD
+Filename: fmot-1.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fmot/PY_REQUIREMENTS

```diff
@@ -3,10 +3,10 @@
 numpy>=1.18.0
 scipy
 python_speech_features
 tqdm
 networkx
 deprecation
 tabulate
-datashader
+datashader>=0.14.4
 colorcet
-matplotlib
+matplotlib
```

## fmot/VERSION

```diff
@@ -1 +1 @@
-1.3.4
+1.5.6
```

## fmot/__init__.py

```diff
@@ -1,14 +1,17 @@
 def _get_dir():
     import pathlib
     return pathlib.Path(__file__).parent.resolve()
 
 __version__ = (_get_dir() / 'VERSION').read_text(encoding='utf-8').strip()
 
+import torch
 from . import torchscript_utils
+from . import configure
+from .configure import CONFIG
 from . import nn
 from . import qat, utils, convert, tracing
 from ._open_docs import open_docs
 from ._supported_ops import supported_ops, conversion_branch
 from .convert.conversion_api import ConvertedModel
 from .convert.lut_registry import LUT_REGISTRY, register_lut, LUTConfig
 from .utils import save, load, load_state_dict
```

## fmot/_open_docs.py

```diff
@@ -3,8 +3,11 @@
 import pathlib
 
 def open_docs():
     fmot_path = pathlib.Path(fmot.__file__).parent.resolve().parent.resolve()
     doc_path = os.path.join(fmot_path, 'docs')
     index_path = os.path.join(doc_path, '_build', 'html', 'index.html')
     cwd = os.getcwd()
-    os.system(f'cd {doc_path}; sphinx-apidoc -f . -o .; make html; cd {cwd}; open {index_path}')
+    os.system(f'cd {doc_path}; sphinx-apidoc -f . -o .; make html; cd {cwd}; open {index_path}')
+
+if __name__ == "__main__":
+    open_docs()
```

## fmot/convert/conversion_api.py

```diff
@@ -1,37 +1,36 @@
 import torch
 from . import patching, mapping, substitution, prune_reparametrization
 from fmot.qat import bitwidths, control, standard, double
 from fmot.exceptions import RequiredArgError, ConversionDependencyError
 from fmot.tracing import trace, trace_hybrid
 from fmot.qat.nn import DEFAULT_OBSERVERS, density_matmul, act_density, ObserverBase, QuantWrapper
-from fmot.convert.default_substitutions import DEFAULT_SUBSTITUTIONS
+from fmot.convert.default_substitutions import get_default_substitutions
 from fmot import utils
 from .quantizer_manager import generate_param2quantizer
 from .prune_reparametrization import remove_all_pruners, reapply_all_pruners
 from typing import *
-from .configure import configure_param_observer
+from fmot.configure import CONFIG, configure_act_observer, configure_param_observer
 from tabulate import tabulate
 
 
 def is_sequential(model):
     """Checks recursively if the model contains layers that will be mapped to a Sequencer"""
-    if type(model) in DEFAULT_SUBSTITUTIONS:
+    if type(model) in get_default_substitutions():
         return True
 
     for _, submodule in model.named_children():
         if is_sequential(submodule):
             return True
 
     return False
 
-
 def convert(model: torch.nn.Module, precision: str, interpolate: bool, verbose: bool, 
             dimensions: List[Literal['B', 'T', 'F']],
-            observer: ObserverBase=DEFAULT_OBSERVERS['default'], observer_conf: dict=None,
+            observer: Union[ObserverBase, str]=DEFAULT_OBSERVERS['default'], observer_conf: dict=None,
             param_observer: str=None) -> Tuple[QuantWrapper, dict]:
     """
     Args:
         model (torch.nn.Module): pytorch model to convert
         precision (str): precision -- 'standard' or 'double'
         interpolate (bool): whether to use interpolating lookup tables
         verbose (bool): if True, will print out details of the conversion process
@@ -46,14 +45,17 @@
 
         - converted_model
         - parameter_mapping_dictionary
     """
     if param_observer is not None:
         configure_param_observer(param_observer)
 
+    if isinstance(observer, str):
+        observer = configure_act_observer(observer)
+
     if isinstance(precision, str):
         precision = bitwidths.bw_conf_dict[precision]
     pinfo = prune_reparametrization.remove_all_pruners(model, verbose=verbose)
     param_map_dict = dict()
     smodel = substitution.torch_to_sequencer(model,
                                              extra_substitutions=None, substitutions_dict=param_map_dict,
                                              verbose=verbose)
@@ -98,21 +100,24 @@
         observer_config (dict): keyword arguments to pass to the observer class,
             default is :attr:`None`.
         param_observer (str, optional): algorithm used to calibrate parameter quantization.
             Options: 'min_max' (default), 'gaussian'
     """
 
     def __init__(self, model, precision='double', named_dims=None, batch_dim=0,
-                 seq_dim=None, interpolate=True, observer=DEFAULT_OBSERVERS['default'],
+                 seq_dim=None, interpolate=None, observer=DEFAULT_OBSERVERS['default'],
                  observer_config=None, param_observer: str='min_max'):
         super().__init__()
         self.named_dims = named_dims
         self.batch_dim = batch_dim
         self.seq_dim = seq_dim
 
+        if interpolate is None:
+            interpolate = CONFIG.interpolate
+
         if not isinstance(model, torch.nn.Module):
             raise ValueError('model must be a torch.nn.Module')
         if is_sequential(model) and (seq_dim is None):
             raise Exception(
                 'Cannot convert sequential models (i.e. RNNs and Conv1d) ' \
                 'without a seq_dim, denoting which input tensor dimension ' \
                 'is the sequential dimension.')
@@ -155,33 +160,36 @@
         for module in self.modules():
             if isinstance(module, density_matmul._MMBase):
                 module.reset_act_densities()
 
         self._seen_input = True
         return self.model(*args, **kwargs)
 
-    def quantize(self, calibration_inputs, insert_fixed_range_observers=True):
+    def quantize(self, calibration_inputs):
         """Quantizes the model, given a set of calibration inputs. The model
         will be quantized after calling this method.
 
         Args:
             calibration_inputs (list[Tensor] or list[tuple[Tensor]]): A list
                 of representative inputs to the model, used to calibrate the 
                 quantization configuration.
             insert_fixed_range_observers (bool): If True, will insert fixed-range
                 observers into the model upstream of saturating nonlinearities.
                 Default is :attr:`True`.
         """
         if self.tracing_input is None:
             self.tracing_input = calibration_inputs[0]
+        
+        if CONFIG.insert_fixed_range_observers:
+            self._insert_fixed_range_observers(self.tracing_input)
+
         control.quantize(self.model, input_iterator=calibration_inputs,
                          dimensions=self._dimensions)
         self.param2quant = generate_param2quantizer(self, calibration_inputs[0])
-        if insert_fixed_range_observers:
-            self._insert_fixed_range_observers(self.tracing_input)
+
         self.quantized = True
         self._seen_input = True
 
     def trace(self, experimental_hybrid_tracing=False, **experimental_kwargs):
         """Express the model's computational graph as an FQIR graph.
         The FQIR graph describes an equivalent model, using only integer datatypes
         and operations.
@@ -202,21 +210,24 @@
                 'Must quantize model before tracing. Call "quantize" method first.')
         if self.training:
             print("Switching model to eval mode")
             self.eval()
         if isinstance(tracing_input, torch.Tensor):
             tracing_input = (tracing_input,)
         if not experimental_hybrid_tracing:
-            output = trace(self.model, *tracing_input,
+            output, tsrc_dict = trace(self.model, *tracing_input,
                            batch_dim=self.batch_dim, seq_dim=self.seq_dim)
         else:
             output = trace_hybrid(self.model, *tracing_input, named_dims=self.named_dims, batch_dim=self.batch_dim,
                                   seq_dim=self.seq_dim, **experimental_kwargs)
         if training:
             self.train()
+        
+        self.tsrc_dict = tsrc_dict
+
         return output
 
     def measure_density_metrics(self, *metrics):
         """Measure density metrics after a forward pass of the converted/quantized model
 
         Args:
             metrics (str): One or more density metrics to measure.
@@ -255,22 +266,21 @@
             param_quantizer.update_bitwidth(standard)
         elif precision == 'double':
             param_quantizer.update_bitwidth(double)
         else:
             raise Exception('Unknown precision argument: available parameter precisions ' + \
                             'are `standard` and `double`')
 
-    def _insert_fixed_range_observers(self, tracing_input, scaling=2, verbose=False):
+    def _insert_fixed_range_observers(self, tracing_input):
         """
         Inserts fixed-range-observers into the model upstream of saturating nonlinearities.
         This restricts the output dynamic range of operations preceding operations like
         sigmoid or tanh to avoid wasting quantized dynamic range.
         """
-        utils.insert_fixed_range_observers(self.model, tracing_input, scaling=scaling,
-                                           verbose=verbose)
+        return utils.insert_fixed_range_observers(self.model, tracing_input)
 
     def enable_quantization(self, quantize=True):
         """
         Turns on quantization.
 
         Args:
             quantize (bool): if False, will disable quantization.
```

## fmot/convert/default_mappings.py

```diff
@@ -7,28 +7,31 @@
     fmot.nn.VVAdd               :       Q.nn.VVAdd,
     fmot.nn.VIAdd               :       Q.nn.VIAdd,
     fmot.nn.VVSub               :       Q.nn.VVSub,
     fmot.nn.Neg                 :       Q.nn.Neg,
     fmot.nn.VVMul               :       Q.nn.VVMul,
     fmot.nn.VIMul               :       Q.nn.VIMul,
     fmot.nn.Matmul              :       Q.nn.Matmul,
+    fmot.nn.TemporalUnfold1d    :       Q.nn.TemporalUnfold1d,
     fmot.nn.AddMM               :       Q.nn.AddMM,
     torch.nn.ReLU               :       Q.nn.ReLU,
     torch.nn.Linear             :       Q.nn.Linear,
     torch.nn.BatchNorm1d        :       Q.nn.BatchNorm,
     torch.nn.BatchNorm2d        :       Q.nn.BatchNorm,
     fmot.nn.StateInitializer    :       Q.nn.StateInitializer,
     fmot.nn.RSqrtPlusEps        :       Q.nn.RSqrtPlusEps,
     fmot.nn.TuningEpsilon       :       Q.nn.TuningEpsilon,
     fmot.nn.PowFrac             :       Q.nn.PowFrac,
     fmot.nn.Chunk               :       Q.nn.Chunk,
     fmot.nn.Split               :       Q.nn.Split,
     fmot.nn.Cat                 :       Q.nn.Cat,
     fmot.nn.Stack               :       Q.nn.Stack,
     fmot.nn.ParameterQuantizer  :       Q.nn.ParameterQuantizer,
+    fmot.nn.DerivedParameter    :       Q.nn.QDerivedParameter,
+    fmot.nn.MultiDerivedParameter:      Q.nn.QMultiDerivedParameter,
     fmot.nn.Transpose           :       Q.nn.Transpose,
     fmot.nn.Reshape             :       Q.nn.Reshape,
     fmot.nn.Div                 :       Q.nn.Div,
     fmot.nn.Sum                 :       Q.nn.Sum,
     fmot.nn.Mean                :       Q.nn.Mean,
     fmot.nn.Identity            :       Q.nn.Identity,
     fmot.nn.OnesLike            :       Q.nn.OnesLike,
@@ -37,15 +40,10 @@
     fmot.nn.Shift               :       Q.nn.Shift,
     fmot.nn.LUT                 :       Q.nn.LUT,
     fmot.nn.FTranspose          :       Q.nn.FTranspose,
     fmot.nn.Permute             :       Q.nn.Permute,
     fmot.nn.DepthWiseConvSummer :       Q.nn.DepthWiseConvSummer,
     fmot.nn.LogMM               :       Q.nn.LogMM,
     fmot.nn.LogEpsMM            :       Q.nn.LogEpsMM,
-    torch.nn.Conv1d             :       Q.nn.Conv1d,
-    torch.nn.Conv2d             :       Q.nn.Conv2d,
-    torch.nn.AvgPool1d          :       Q.nn.AvgPool1d,
-    torch.nn.MaxPool1d          :       Q.nn.MaxPool1d,
     fmot.nn.Squeeze             :       Q.nn.Squeeze,
-    torch.nn.AdaptiveAvgPool2d  :       Q.nn.AdaptiveAvgPool2d,
     torch.nn.LSTM               :       Q.nn.LSTM
 }
```

## fmot/convert/default_patchings.py

```diff
@@ -248,15 +248,15 @@
     'aten::squeeze': PatchRule(squeeze_rule, [fmot.nn.Squeeze]),
     'aten::linear': PatchRule(linear_rule, [fmot.nn.F_Linear, fmot.nn.F_Linear_nb]),
 ########################################################################
 # >     torch.nn.functional
     'F.relu' : nn.ReLU,
     'F.sigmoid' : nn.Sigmoid,
     'F.tanh' : nn.Tanh,
-    #'F.linear' : PatchRule(linear_rule, [fmot.nn.F_Linear, fmot.nn.F_Linear_nb]),
+    'F.linear' : PatchRule(linear_rule, [fmot.nn.F_Linear, fmot.nn.F_Linear_nb]),
     'F.layer_norm' : PatchRule(layernorm_rule, [fmot.nn.F_LayerNorm]),
     'F.softmax' : PatchRule(softmax_rule, [fmot.nn.F_Softmax]),
     'F.hardsigmoid' : fmot.nn.HardSigmoid,
     'F.hardtanh' : PatchRule(hardtanh_rule, [fmot.nn.HardTanh]),
     'F.leaky_relu' : PatchRule(leakyrelu_rule, [fmot.nn.LeakyReLU]),
     'F.dropout' : PatchRule(dropout_rule, [fmot.nn.Dropout]),
 }
```

## fmot/convert/default_substitutions.py

```diff
@@ -1,13 +1,19 @@
 import fmot
 import torch
 from ..nn.sru import SRU
 
-
 DEFAULT_SUBSTITUTIONS = {
     torch.nn.modules.rnn.RNN: fmot.nn.RNN,
     torch.nn.modules.rnn.GRU: fmot.nn.GRU,
-    # torch.nn.modules.rnn.LSTM: fmot.nn.LSTM,
-    # torch.nn.modules.conv.Conv1d: fmot.nn.Conv1d
     fmot.nn.TemporalConv1d: fmot.nn.conv1d.FmotConv1dWrapper,
     SRU: fmot.nn.SRUSequencer
 }
+
+def get_default_substitutions():
+    """Apply config settings (e.g. turn on/off LSTM substitution mapping)
+    """
+    substitutions = DEFAULT_SUBSTITUTIONS.copy()
+    if fmot.CONFIG.sequenced_lstm:
+        substitutions[torch.nn.modules.rnn.LSTM] = fmot.nn.LSTM
+    return substitutions
+
```

## fmot/convert/mapping.py

```diff
@@ -58,30 +58,49 @@
 
     return model
 
 def _map(module, mappings, bw_conf, interpolate, parent_name, verbose,
     observer, **observer_kwargs):
     to_convert = [] # Modules to attempt to map in the next recursive step
     nchildren = 0
+
+    if hasattr(module, 'precision'):
+        precision_tag = module.precision
+        bw_conf = bitwidths.bw_conf_dict.get(precision_tag, bw_conf)
+        print('Found precision tag')
+
+    if hasattr(module, 'limits'):
+        limits = module.limits
+        print(f'Found limits tag {limits}')
+
     for name, submodule in module.named_children():
         new_name = f'{parent_name}.{name}'
         nchildren += 1
-        if type(submodule) in mappings:
-            try:
-                new_module = mappings[type(submodule)]._from_float(submodule,
-                    bw_conf=bw_conf, interpolate=interpolate,
-                    observer=observer, **observer_kwargs)
-            except Exception as e:
-                raise ValueError(f'{type(submodule)}', e)
-            module.__setattr__(name, new_module)
-            if verbose:
-                verbose_printout(new_name, submodule, new_module)
-        elif issubclass(type(submodule), ProtectedModule):
-            pass
-        else:
-            to_convert.append((new_name, submodule))
+
+        curr_bw_conf = bw_conf
+        if hasattr(submodule, 'precision'):
+            precision_tag = submodule.precision
+            curr_bw_conf = bitwidths.bw_conf_dict.get(precision_tag, curr_bw_conf)
+            print('Found precision tag')
+        
+        mapped = False
+        for cls_in, cls_out in mappings.items():
+            if isinstance(submodule, cls_in):
+                new_module = cls_out._from_float(submodule,
+                        bw_conf=curr_bw_conf, interpolate=interpolate,
+                        observer=observer, **observer_kwargs)
+                module.__setattr__(name, new_module)
+                if verbose:
+                    verbose_printout(new_name, submodule, new_module)
+                mapped=True
+                break
+        if not mapped:
+            if issubclass(type(submodule), ProtectedModule):
+                pass
+            else:
+                to_convert.append((new_name, submodule))
     if nchildren == 0:
         raise ValueError(
             f'Reached leaf node {parent_name} (type: {module}) that could not be mapped.')
     for (name, submodule) in to_convert:
         _map(submodule, mappings, bw_conf, interpolate, name, verbose,
             observer, **observer_kwargs)
```

## fmot/convert/patch_ir.py

```diff
@@ -680,14 +680,19 @@
         """
         Semi-human-legible python code, generated from the PatchIR
         """
         return self.patchIR.__repr__()
 
 def get_patched_module_from_torch(module, extra_patchings=None):
     if isinstance(module, Sequencer):
-        return PatchedSequencer.from_torch(module, extra_patchings)
+        out = PatchedSequencer.from_torch(module, extra_patchings)
     else:
-        return PatchedModule.from_torch(module, extra_patchings)
+        out = PatchedModule.from_torch(module, extra_patchings)
+
+    # copy precision tags
+    if hasattr(module, 'precision'):
+        out.precision = module
+    return out
```

## fmot/convert/patching.py

```diff
@@ -75,14 +75,16 @@
 def _patch_in_place(module, extra_patchings, mappings, parent_name, verbose):
     to_patch = [] # Modules to patch in the next recursive step. Entries are (name, module)
 
     for name, submodule in module.named_children():
         # Patch everything except raw patchlists and quantdicts
         if issubclass(type(submodule), ProtectedModule):
             pass
+        elif type(submodule) in mappings:
+            pass
         elif needspatching(submodule, mappings) and not name in ['patchlist', 'quantdict']:
             patch = get_patched_module_from_torch(submodule, extra_patchings=extra_patchings)
             module.__setattr__(name, patch)
 
             # Patch the patch in the next recursive step
             to_patch.append((name, patch))
```

## fmot/convert/prune_reparametrization.py

```diff
@@ -2,15 +2,15 @@
 from torch.nn.utils import prune
 import inspect
 from collections import namedtuple
 from fmot.qat.nn import QuantWrapper
 from torch.nn.utils.prune import CustomFromMask, PruningContainer, BasePruningMethod
 from fmot.nn.sequenced_rnn import default_torch2seq_param_mapping, \
     get_trailing_number, map_param_name, rsetattr, rgetattr
-from .default_substitutions import DEFAULT_SUBSTITUTIONS
+from .default_substitutions import get_default_substitutions
 
 def get_pruner_kwargs(pruner):
     kwargs = {}
     arg_names = list(inspect.signature(pruner.apply).parameters.keys())
     for name in arg_names:
         if hasattr(pruner, name):
             kwargs[name] = getattr(pruner, name)
@@ -46,15 +46,15 @@
                     pm = hook
                 pinfo = PruningInfo(
                     module_name=mname,
                     tensor_name=tname,
                     mask=mask,
                     pruner=pm,
                     kwargs=get_pruner_kwargs(pm),
-                    is_substituted=type(module) in DEFAULT_SUBSTITUTIONS)
+                    is_substituted=type(module) in get_default_substitutions())
                 pruning_info.append(pinfo)
 
     return pruning_info
 
 def reapply_all_pruners(qmodel, model, pruning_info, substitution_dict, verbose=False):
     if isinstance(qmodel, QuantWrapper):
         qmodel = qmodel.model
```

## fmot/convert/substitution.py

```diff
@@ -1,17 +1,17 @@
 import torch
 from torch import nn
 import fmot
 from fmot import qat as Q
 from copy import deepcopy
-from .default_substitutions import DEFAULT_SUBSTITUTIONS
+from .default_substitutions import get_default_substitutions
 from ..nn.super_structures import ProtectedModule
 
 def torch_to_sequencer(model, extra_substitutions=None, substitutions_dict=dict(), verbose=False):
-    substitutions = DEFAULT_SUBSTITUTIONS
+    substitutions = get_default_substitutions()
     if extra_substitutions is not None:
         substitutions.update(extra_substitutions)
 
     model = deepcopy(model)
 
     inherited_name = ""
     if type(model) in substitutions:
```

## fmot/fqir/graph_proto/graph_proto.py

```diff
@@ -1,12 +1,14 @@
 """An FQIR Graph consists of :obj:`GraphProto`, :obj:`NodeProto`, and :obj:`TensorProto`"""
 import numpy as np
 from .graph_runtime import run_graph, run_sequential_graph
 from collections import defaultdict, OrderedDict
-from ..nodes import OpCount
+from ..nodes import OpCount, NodeProto
+from ..variables import TensorProto
+from typing import *
 
 DEF_IND = '   '
 
 class GraphProto:
     """Defines an fqir graph or subgraph
 
     The same GraphProto class is used for main graphs and subgraphs.
@@ -31,19 +33,19 @@
         parameters (list[:class:`TensorProto`]): The graph's parameters
         subgraphs (dict[:class:`GraphProto`]): Maps names to subgraphs
         reshaper (callable, optional): Reshapes input sequences
             (e.g. for when there is a strided frontend conv1d layer
     """
     def __init__(self, name="", unbind_dim=None, stack_dim=None):
         self.name = name
-        self.nodes = []
-        self.inputs = []
-        self.outputs = []
-        self.parameters = []
-        self.subgraphs = {}
+        self.nodes: List[NodeProto] = []
+        self.inputs: List[TensorProto] = []
+        self.outputs: List[TensorProto] = []
+        self.parameters: List[TensorProto] = []
+        self.subgraphs: Dict[str, GraphProto] = {}
         self.reshaper = None
         self.unbind_dim = unbind_dim
         if stack_dim is None:
             stack_dim = unbind_dim
         self.stack_dim = stack_dim
 
     def add_input(self, tensor):
```

## fmot/fqir/graph_proto/graph_runtime.py

```diff
@@ -68,15 +68,16 @@
                 if node.optype.name == 'assign':
                     objs[node.inputs['y'].name] = objs[node.inputs['x'].name]
             except Exception as e:
                 logger.warning('Error in node %s: %s', node, e)
                 raise Exception(f'Error in node {node}: {e}')
         else:
             outputs = None
-            logger.info("Skipping %s in graph runtime", node)
+            # logger.info("Skipping %s in graph runtime", node)
+            # logger.info(f'{skipped_subgraphs=}')
         if outputs is not None:
             if isinstance(outputs, dict):
                 objs.update(outputs)
             else:
                 store_outputs(node, outputs, objs)
 
     outputs = [objs[proto.name] for proto in graph.outputs]
@@ -105,14 +106,15 @@
 
 def run_sequential_graph(graph, inputs, return_objs=False, arith_only=False,
     dequant=False, objs=None, return_dict=False):
     """Run a sequential graph"""
     # initialize state variables
     if objs is None:
         __, objs = run_graph(graph.subgraphs['INIT'], return_objs=True)
+        logger.info('Running INIT')
 
     if arith_only:
         step_graph = graph.subgraphs['ARITH']
     else:
         step_graph = graph
     outputs = []
```

## fmot/fqir/nodes/node_proto.py

```diff
@@ -1,12 +1,15 @@
 from .node_base import NodeBase
 import textwrap
 from deprecation import deprecated
 import fmot
 import numpy as np
+from .optype_base import OpType
+from ..variables import TensorProto
+from typing import *
 
 DEF_IND = '   '
 
 class NodeProto(NodeBase):
     """Represents an operation or subgraph (but not both) in the fqir graph.
 
     Args:
@@ -20,15 +23,16 @@
             matching the :class:`OpType` runtime constants
             (e.g. shift-amounts, immediates, LUT values, etc.)
         subgraph (:class:`GraphProto`, optional): A subgraph for the node to contain.
             Subgraphs are wrapped in NodeProtos for the purpose of runtime execution.
             When wrapping a subgraph, set ``optype`` to ``None``.
         sourceref (str, optional): A reference to the user's original code, or :attr:`None`
     """
-    def __init__(self, name, optype, inputs, outputs, constants=None,
+    def __init__(self, name: str, optype: OpType, inputs: Dict[str, TensorProto], 
+                 outputs: List[TensorProto], constants: Optional[Dict[str, Any]]=None,
                  subgraph=None, sourceref=None):
         if optype is not None and subgraph is not None:
             raise ValueError("A Node can contain an operation or subgraph but not both")
         opname = optype.name if (optype is not None) else subgraph.name
         opcounter = optype.opcounter if (optype is not None) else None
         repr_settings = None
         if hasattr(optype, 'repr_settings'):
```

## fmot/fqir/nodes/optype_base.py

```diff
@@ -42,15 +42,16 @@
             Signature: (input_length: tuple[int], constants: dict) -> tuple[int]
     Attributes:
         runtime (callable or str): The runtime function
         seq_len_fn (callable): Function that computes sequence length (or H,W) as a function
             of input sequence length
     """
     def __init__(self, name, inputs, constants, runtime=None,
-        opcounter=None, seq_length_fn=None, repr_settings=None):
+        opcounter=None, seq_length_fn=None, repr_settings=None,
+        can_bcast_in: bool=True):
         self.name = name
 
         if runtime is not None:
             self._runtime = runtime
         else:
             runtime = self.runtime
 
@@ -68,14 +69,16 @@
 
         self._seq_length_fn = seq_length_fn
         self.repr_settings = repr_settings
 
         self._inputs: Dict[str, VariableBase] = None
         self._outputs: List[VariableBase] = None
 
+        self.can_bcast_in = can_bcast_in
+
     def runtime(self, *args, **kwargs):
         return self._runtime(*args, **kwargs)
 
     def __repr__(self):
         return "OpType<{}>".format(self.name)
 
     def check_inputs_constants(self, inputs, constants):
```

## fmot/fqir/nodes/optypes.py

```diff
@@ -56,15 +56,16 @@
         super().__init__(
             name='vvadd',
             inputs=['x', 'y'],
             constants=['shamt_x', 'shamt_y', 'shamt_bwred', 'bw', 'bw_x', 'bw_y'],
             repr_settings=NodeReprSettings(
                 # operator_symbol='+',
                 use_var_names=False),
-            opcounter=VVCounter(op='add'))
+            opcounter=VVCounter(op='add'),
+            can_bcast_in=True)
 
     @staticmethod
     def runtime(x, y, shamt_x, shamt_y, shamt_bwred, bw, bw_x, bw_y):
         """Add two vectors together
 
         Runtime Signature:
             vvadd(x, y)
@@ -94,15 +95,16 @@
             name='viadd',
             inputs=["x"], 
             constants=["y", "shamt_x", "shamt_y", "shamt_bwred", "bw", "bw_x", "bw_y"],
             opcounter=VCounter(op='add'),
             repr_settings=NodeReprSettings(
                 # operator_symbol='+', 
                 use_var_names=False,
-                constants_to_rep=['y']))
+                constants_to_rep=['y']),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, y, shamt_x, shamt_y, shamt_bwred, bw, bw_x, bw_y):
         """Add a vector to an immediate
 
         Runtime Signature:
             viadd(x)
@@ -130,15 +132,15 @@
             name='vvsub',
             inputs=["x", "y"], 
             constants=["shamt_x", "shamt_y", "shamt_bwred", "bw", "bw_x", "bw_y"],
             opcounter=VVCounter(op='add'),
             repr_settings=NodeReprSettings(
                 # operator_symbol='-',
                 use_var_names=False),
-            )
+            can_bcast_in=True)
 
     @staticmethod
     def runtime(x, y, shamt_x, shamt_y, shamt_bwred, bw, bw_x, bw_y):
         """Subtracts one vector from another
 
         Runtime Signature:
             vvsub(x, y)
@@ -173,15 +175,16 @@
 
 class VNEG(OpType):
     def __init__(self):
         super().__init__(
             name='vneg',
             inputs=['x'],
             constants=['bw'],
-            opcounter=VCounter(op='add'))
+            opcounter=VCounter(op='add'),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, bw):
         """Multiply a vector by -1
 
         Runtime Signature:
             vneg(x)
@@ -217,16 +220,16 @@
         super().__init__(
             name='vvmul',
             inputs=['x', 'y'],
             constants=['shamt_bwred', 'bw'],
             opcounter=VVCounter(op='mul'),
             repr_settings=NodeReprSettings(
                 # operator_symbol='*',
-                use_var_names=False)
-            )
+                use_var_names=False),
+            can_bcast_in=True)
 
     @staticmethod
     def runtime(x, y, shamt_bwred, bw):
         """Multiplies two vectors element-wise
 
         Runtime Signature:
             vvmul(x, y)
@@ -249,15 +252,16 @@
             name='vimul',
             inputs=["x"], 
             constants=["y", "shamt_bwred", "bw"], 
             opcounter=VCounter(op='mul'),
             repr_settings=NodeReprSettings(
                 # operator_symbol='*', 
                 constants_to_rep=['y'],
-                use_var_names=False))
+                use_var_names=False),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, y, shamt_bwred, bw):
         """Multiplies a vectors element-wise with an immediate
 
         Runtime Signature:
             vimul(x)
@@ -276,15 +280,16 @@
 
 class MATMUL(OpType):
     def __init__(self):
         super().__init__(
             name='matmul', 
             inputs=["x", "y"], 
             constants=["shamt_bwred", "bw_out"],
-            opcounter=MatmulCounter())
+            opcounter=MatmulCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, y, shamt_bwred, bw_out):
         """Matrix product
 
         Runtime Signature:
             matmul(x, y)
@@ -305,15 +310,16 @@
 
 class ADDMM(OpType):
     def __init__(self):
         super().__init__(
             name='addmm',
             inputs=["bias", "x", "y"], 
             constants=["shamt_bias", "shamt_bwred", "bw_out"],
-            opcounter=MatmulCounter())
+            opcounter=MatmulCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(bias, x, y, shamt_bias, shamt_bwred, bw_out):
         """Matrix product with bias
 
         Runtime Signature:
             addmm(bias, mat1, mat2)
@@ -340,15 +346,16 @@
 
 class RELU(OpType):
     def __init__(self):
         super().__init__(
             name='relu',
             inputs=["x"], 
             constants=[], 
-            opcounter=VCounter(op=None, sparse_out=True))
+            opcounter=VCounter(op=None, sparse_out=True),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x):
         """Element-wise rectified nonlinearity on the input vector
 
         Runtime Signature:
             relu(x)
@@ -366,15 +373,16 @@
 class LUT(OpType):
     def __init__(self):
         super().__init__(
             name='lut', 
             inputs=["x"], 
             constants=["shamt_address", "bw_address", "table", "function"],
             opcounter=VLUTCounter(),
-            repr_settings=NodeReprSettings(constants_to_rep=['function']))
+            repr_settings=NodeReprSettings(constants_to_rep=['function']),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, shamt_address, bw_address, table, function):
         """Performs an elementwise lookup table based nonlinearity on the input vector.
 
         Runtime Signature:
             lut(x)
@@ -401,15 +409,16 @@
 
 class TRANSPOSE(OpType):
     def __init__(self):
         super().__init__(
             name='transpose', 
             inputs=["x"], 
             constants=["dim0", "dim1"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, dim0, dim1):
         """Performs a (hopefully) virtual transpose on a matrix.
 
         Runtime Signature:
             transpose(x)
@@ -432,15 +441,16 @@
 class RESHAPE(OpType):
     def __init__(self):
         super().__init__(
             name='reshape',
             inputs=["x"], 
             constants=["shape"],
             opcounter=NullCounter(),
-            repr_settings=NodeReprSettings(constants_to_rep=['shape']))
+            repr_settings=NodeReprSettings(constants_to_rep=['shape']),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, shape):
         """Reshape the input tensor
 
         Runtime Signature:
             reshape(x)
@@ -456,15 +466,16 @@
 
 class QUANTIZE(OpType):
     def __init__(self):
         super().__init__(
             name='quantize',
             inputs=["x"], 
             constants=["quanta", "bw"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, quanta, bw):
         """Convert a floating-point tensor into a quantized integer tensor, according to:
 
         Runtime Signature:
             quantize(x)
@@ -487,15 +498,16 @@
 
 class DEQUANTIZE(OpType):
     def __init__(self):
         super().__init__(
             name='dequantize',
             inputs=["x"], 
             constants=["quanta"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, quanta):
         """Convert an integer tensor into a rounded floating-point tensor
 
         Runtime Signature:
             dequantize(x)
@@ -514,15 +526,16 @@
 
 class CHUNK(OpType):
     def __init__(self):
         super().__init__(
             name='chunk', 
             inputs=["x"], 
             constants=["chunks", "dim"],
-            opcounter=CopyCounter())
+            opcounter=CopyCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, chunks, dim):
         """Split a tensor into a tuple of `chunks` tensors along a dimension `dim`.
 
         Runtime Signature:
             chunk(x)
@@ -539,15 +552,16 @@
 
 class SPLIT(OpType):
     def __init__(self):
         super().__init__(
             name='split',
             inputs=["x"],
             constants=["lengths", "dim"],
-            opcounter=CopyCounter())
+            opcounter=CopyCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, lengths, dim):
         """Split a tensor into a tuple of tensors along a dimension `dim`.
 
         Runtime Signature:
             split(x)
@@ -567,15 +581,16 @@
 class CAT(OpType):
     def __init__(self):
         super().__init__(
             name='cat', 
             inputs=["kwargs"], 
             constants=["dim"],
             opcounter=CopyCounter(),
-            repr_settings=NodeReprSettings(use_var_names=False))
+            repr_settings=NodeReprSettings(use_var_names=False),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(dim, **kwargs):
         """Concatenate tensors along `dim`, in order.
 
         Runtime Signature:
             cat(x0, x1, x2, ...)
@@ -595,15 +610,16 @@
 class STACK(OpType):
     def __init__(self):
         super().__init__(
             name='stack', 
             inputs=["kwargs"], 
             constants=["dim"],
             opcounter=CopyCounter(),
-            repr_settings=NodeReprSettings(use_var_names=False))
+            repr_settings=NodeReprSettings(use_var_names=False),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(dim, **kwargs):
         """Stack tensors along dim
 
         Runtime Signature:
             stack(x0, x1, x2, ...)
@@ -622,27 +638,29 @@
 
 class SQUEEZE(OpType):
     def __init__(self):
         super().__init__(
             name='squeeze', 
             inputs=["x"], 
             constants=["dim"], 
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, dim):
         raise NotImplementedError
 
 class ZEROS(OpType):
     def __init__(self):
         super().__init__(
             name='zeros', 
             inputs=[], 
             constants=["shape"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(shape):
         """Init a zeros vector of shape `shape`
 
         Runtime Signature:
             zeros()
@@ -654,15 +672,16 @@
 class CONSTANT(OpType):
     def __init__(self):
         super().__init__(
            name='constant',
             inputs=[], 
             constants=["shape", "value"],
             opcounter=NullCounter(),
-            repr_settings=NodeReprSettings(constants_to_rep=['value']))
+            repr_settings=NodeReprSettings(constants_to_rep=['value']),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(shape, value):
         """Init a constant vector of shape `shape`
 
         Runtime Signature:
             zeros()
@@ -674,15 +693,16 @@
 
 class ASSIGN(OpType):
     def __init__(self):
         super().__init__(
             name='assign',
             inputs=["y", "x"], 
             constants=[],
-            opcounter=CopyCounter())
+            opcounter=CopyCounter(),
+            can_bcast_in=False)
 
     def runtime(self, y, x):
         """Assign y to hold the value stored by x (i.e. y = x)
 
         Runtime Signature:
             assign(y, x)
         Arguments:
@@ -693,15 +713,16 @@
 
 class TEMPORAL_UNFOLD_UNKERNELIZED(OpType):
     def __init__(self):
         super().__init__(
             name='temporal_unfold_unkernelized',
             inputs=["x"], 
             constants=["kernel_size", "dilation", "buffer_length"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     def runtime(self, x, kernel_size, dilation, buffer_length):
         """Internally manages the state of a rolling buffer with a sliding
         dilated temporal window. Returns a concatenation of the in-frame vectors 
         at each time-step.
 
         Runtime Signature:
@@ -719,15 +740,16 @@
 
 class TEMPORAL_UNFOLD(OpType):
     def __init__(self):
         super().__init__(
             name='temporal_unfold',
             inputs=["x", "buffer"], 
             constants=["kernel_size", "dilation", "buffer_length"],
-            opcounter=NullCounter())
+            opcounter=NullCounter(),
+            can_bcast_in=False)
 
     def runtime(self, x, buffer, kernel_size, dilation, buffer_length):
         """Internally manages the state of a rolling buffer with a sliding
         dilated temporal window. Returns a concatenation of the in-frame vectors 
         at each time-step.
 
         Runtime Signature:
@@ -737,15 +759,14 @@
             x: new input frame
             buffer: stateful buffer storing past frames
         Constants:
             kernel_size: kernel size of sliding window
             dilation: dilation of sliding window
             buffer_length: number of vectors stored in buffer
         """
-        print(f'Buffer.shape: {buffer.shape} x.shape: {x.shape}')
         buffer = np.concatenate([buffer, x])
         buffer = buffer.reshape(-1, len(x))
         outs = buffer[::dilation]
         outs = outs.flatten()
         buffer = buffer[1:].flatten()
 
         return {
@@ -755,15 +776,16 @@
 
 class SUM(OpType):
     def __init__(self):
         super().__init__(
             name='sum',
             inputs=["x"], 
             constants=["dim", "keepdim", "shamt_bwred", "bw"],
-            opcounter=ReductionCounter())
+            opcounter=ReductionCounter(),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, dim, keepdim, shamt_bwred, bw):
         """Sum the elements of x along a dim
 
         Runtime Signature:
             sum(x)
@@ -784,15 +806,16 @@
 
 class CONSTANT_LIKE(OpType):
     def __init__(self):
         super().__init__(
             name='constant_like', 
             inputs=["x"], 
             constants=["imm"],
-            opcounter=CopyCounter())
+            opcounter=CopyCounter(),
+            can_bcast_in=False)
     
     @staticmethod
     def runtime(x, imm):
         """Return a tensor of the same shape as the input, filled with constant "imm".
 
         Runtime Signature:
             constant_like(x)
@@ -805,15 +828,16 @@
 
 class COPY(OpType):
     def __init__(self):
         super().__init__(
             name='copy', 
             inputs=["x"], 
             constants=[],
-            opcounter=CopyCounter())
+            opcounter=CopyCounter(),
+            can_bcast_in=False)
     
     @staticmethod
     def runtime(x):
         """Copies a tensor
 
         Runtime Signature:
             copy(x)
@@ -828,15 +852,16 @@
             name='shift',
             inputs=["x"], 
             constants=["shamt", "bw"],
             opcounter=ShiftCounter(),
             repr_settings=NodeReprSettings(
                 # operator_symbol='<<', 
                 constants_to_rep=['shamt'],
-                use_var_names=False)
+                use_var_names=False),
+            can_bcast_in=False
         )
     
     @staticmethod
     def runtime(x, shamt, bw):
         """Shift and saturate a vector
 
         Runtime Signature:
@@ -854,15 +879,16 @@
 
 class GT0(OpType):
     def __init__(self):
         super().__init__(
             name='gt0', 
             inputs=["x"], 
             constants=["bw"],
-            opcounter=VCounter(op=None))
+            opcounter=VCounter(op=None),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, bw):
         """Elementwise greater than zero. Returns a masking tensor of 0/1's.
 
         Runtime Signature:
             gt0(x)
@@ -887,153 +913,23 @@
 
 class PRINT(OpType):
     def __init__(self):
         super().__init__(
             name='print', 
             inputs=["x"], 
             constants=["func"],
-            opcounter=VCounter(op=None))
+            opcounter=VCounter(op=None),
+            can_bcast_in=False)
 
     @staticmethod
     def runtime(x, func):
         """Prints a string given by func(x), where x in a numpy array
         """
         print(func(x))
 
-def conv1d_len_fn(length_in, constants):
-    if isinstance(length_in, (tuple, list)):
-        L = length_in[-1]
-    else:
-        L = length_in
-    p, = constants['padding']
-    if 'dilation' in constants:
-        d, = constants['dilation']
-    else:
-        d = 1
-    k = constants['kernel_size']
-    s, = constants['stride']
-    Lout = math.floor((L + 2*p - d*(k-1) - 1)/s)
-    if isinstance(length_in, (tuple, list)):
-        return tuple([l for l in length_in[:-1]] + [Lout])
-    else:
-        return Lout
-
-class CONV1D(OpType):
-    def __init__(self):
-        super().__init__(
-            name='conv1d',
-            inputs=["x", "weight"], 
-            constants=["shamt_bwred", "bw_out", "stride", "padding", "dilation", "groups", "kernel_size"], 
-            opcounter=ConvCounter(), 
-            seq_length_fn=conv1d_len_fn
-        )
-
-    @staticmethod
-    def runtime(x, weight, shamt_bwred, bw_out, stride, padding, dilation, groups,
-    kernel_size):
-        """Convolution of a 1d signal
-        
-        A placeholder; conv1d will be kernelized later on.
-        """
-        raise NotImplementedError
-
-class AVGPOOL1D(OpType):
-    def __init__(self):
-        super().__init__(
-            name='avgpool1d',
-            inputs=["x"], 
-            constants=["kernel_size", "stride", "padding", "bw_out"], 
-            opcounter=NullCounter(),
-            seq_length_fn=conv1d_len_fn)
-    
-    @staticmethod
-    def runtime(x, kernel_size, stride, padding, bw_out):
-        """AvgPool1d
-
-        A placeholder for now; runtime doesn't do anything
-        """
-        raise NotImplementedError
-
-class MAXPOOL1D(OpType):
-    def __init__(self):
-        super().__init__(
-            name='maxpool1d',
-            inputs=["x"], 
-            constants=["kernel_size", "stride", "padding", "dilation", "bw_out"],
-            opcounter=NullCounter(), 
-            seq_length_fn=conv1d_len_fn)
-    
-    @staticmethod
-    def runtime(x, kernel_size, stride, padding, dilation, bw_out):
-        """MaxPool1d
-
-        A placeholder for now; runtime doesn't do anything
-        """
-        raise NotImplementedError
-
-def conv2d_len_fn(length_in, constants):
-    if isinstance(length_in, (tuple, list)):
-        H, W = length_in[-2], length_in[-1]
-    else:
-        assert False, f'length_in = {length_in} was expected to be tuple or list'
-    if 'padding' in constants:
-        p_h, p_w = constants['padding']
-    else:
-        p_h, p_w = 0, 0
-    if 'dilation' in constants:
-        d_h, d_w = constants['dilation']
-    else:
-        d_h, d_w = 1, 1
-    if 'stride' in constants:
-        s_h, s_w = constants['stride']
-    else:
-        s_h, s_w = 1, 1
-    if 'kernel_size' in constants:
-        k_h, k_w = constants['kernel_size']
-    else:
-        k_h, k_w = 1, 1
-    def len_fn(L, p, k, d, s):
-        Lout = math.floor((L + 2*p - d*(k-1) - 1)/s + 1)
-        return Lout
-    Hp, Wp = len_fn(H, p_h, k_h, d_h, s_h), len_fn(W, p_w, k_w, d_w, s_w)
-    return tuple([l for l in length_in[:-2]] + [Hp, Wp])
-
-class CONV2D(OpType):
-    def __init__(self):
-        super().__init__(
-            name='conv2d',
-            inputs=["input", "weight"], 
-            constants=["bw_out", "stride", "padding", "dilation", "groups", "kernel_size"],
-            opcounter=ConvCounter(), 
-            seq_length_fn=conv2d_len_fn)
-    
-    @staticmethod
-    def runtime(input, weight, bw_out, stride, padding, dilation, groups, kernel_size):
-        raise NotImplementedError
-
-def adaptive_avg_pool2d_len_fn(length_in, constants):
-    if isinstance(length_in, (tuple, list)):
-        H, W = length_in[-2], length_in[-1]
-    else:
-        assert False, f'length_in = {length_in} was expected to be tuple or list'
-    return constants['output_size']
-
-class ADAPTIVEAVGPOOL2D(OpType):
-    def __init__(self):
-        super().__init__(
-            name='adaptive_avg_pool2d', 
-            inputs=["x"], 
-            constants=["output_size", "bw_out"], 
-            opcounter=NullCounter(),
-            seq_length_fn=adaptive_avg_pool2d_len_fn)
-
-    @staticmethod
-    def runtime(x, output_size, bw_out):
-        raise NotImplementedError
-
 class LSTM(OpType):
     def __init__(self):
         super().__init__(
             name='lstm',
             inputs=["x"],
             constants=[
                 "num_layers",
@@ -1041,26 +937,27 @@
                 "hidden_size", 
                 "batch_first", 
                 "sigmoid",
                 "tanh",
                 "layers" # layers contains layer-specific constants
             ],
             opcounter=NullCounter(),
+            can_bcast_in=False
         )
     
     @staticmethod
     def runtime(x, num_layers, input_size, hidden_size, batch_first, sigmoid, tanh, layers):
         raise NotImplementedError
 
-registry_v1 = OpRegistry('fmot_atomics_v1.10')
+registry_v1 = OpRegistry('fmot_atomics_v1.2')
 
 def register(*optypes):
     for optype in optypes:
         op = optype()
         assert isinstance(op, OpType)
         registry_v1.register_op(op)
 
 register(
     VVADD, VIADD, VVSUB, VNEG, VVMUL, VIMUL, MATMUL, ADDMM, RELU, LUT, TRANSPOSE,
     RESHAPE, QUANTIZE, DEQUANTIZE, CHUNK, SPLIT, CAT, STACK, SQUEEZE, ZEROS, CONSTANT, ASSIGN,
-    SUM, CONSTANT_LIKE, COPY, SHIFT, GT0, CONV1D, AVGPOOL1D, MAXPOOL1D, CONV2D,
-    ADAPTIVEAVGPOOL2D, LSTM, TEMPORAL_UNFOLD, TEMPORAL_UNFOLD_UNKERNELIZED, PRINT)
+    SUM, CONSTANT_LIKE, COPY, SHIFT, GT0,
+    LSTM, TEMPORAL_UNFOLD, TEMPORAL_UNFOLD_UNKERNELIZED, PRINT)
```

## fmot/fqir/passes/__init__.py

```diff
@@ -1,16 +1,21 @@
 from .batchdim_removal import remove_batchdim
 from .dimtag_removal import remove_named_dims
 from .kernelize_lstm import kernelize_lstm
 from .kernelize_temporal_unfold import kernelize_temporal_unfold
-from .uniquify_names import uniquify_names
+from .cleanup import uniquify_names, limit_biases, remove_unused_params
+from .kernelize_red_broad import kernelize_sum, kernelize_broadcast
 
 
 PASS_ORDER = [
     kernelize_lstm,
+    kernelize_temporal_unfold,
+    kernelize_sum,
+    kernelize_broadcast,
     uniquify_names,
-    kernelize_temporal_unfold
+    limit_biases,
+    remove_unused_params
 ]
 
 def run_passes(graph):
     for p in PASS_ORDER:
         p(graph)
```

## fmot/fqir/passes/kernelize_lstm.py

```diff
@@ -71,15 +71,15 @@
         weights[name] = proto
     return weights
 
 def get_bw(tensor: TensorProto) -> int:
     return int(tensor.dtype.split('fqint')[1])
 
 def get_matmul(name: str, dtype: str, input_size: int, quanta_out: int, output_size: int, 
-    x: TensorProto, weight: TensorProto, bias: TensorProto=None,
+    x: TensorProto, weight: TensorProto, bias: TensorProto=None, factor: Any=None,
     output: TensorProto=None) -> Tuple[TensorProto, NodeProto]:
     
     if output is None:
         y = TensorProto(f'{name}_output', dtype, [output_size], quanta=quanta_out)
     else:
         y = output
     outputs = [y]
```

## fmot/nn/__init__.py

```diff
@@ -1,12 +1,16 @@
 from .atomics import *
 from .composites import *
 from .sequencer import *
 from .super_structures import BasicRNN, SuperBasic  # SuperStructure
 from .sequenced_rnn import *
 from .conv1d import TemporalConv1d, OverlapAdd
-from . import signal
+from . import signal_processing as signal
+from .signal_processing import EMA
 from .sparsifiers import *
 from .femtornn import *
-from .fft import FFT, RFFT, IRFFT
-from .stft import STFT, OverlapAdd50Pct
-from .sru import SRU
+from .fft import *
+from .stft import STFT, OverlapAdd50Pct, ISTFT
+from .sru import SRU
+from .temporal_unfold import TemporalUnfold1d
+# from .sliding_attention import SlidingSelfAttention
+from .derived_param import *
```

## fmot/nn/atomics.py

```diff
@@ -240,23 +240,14 @@
     def __init__(self, shape):
         super().__init__()
         self.shape = shape
         
     def forward(self, x):
         return torch.reshape(x, self.shape)
 
-class Sum(nn.Module):
-    def __init__(self, dim, keepdim=False):
-        super().__init__()
-        self.dim = dim
-        self.keepdim = keepdim
-
-    def forward(self, x):
-        return torch.sum(x, dim=self.dim, keepdim=self.keepdim)
-
 class Div(nn.Module):
     def forward(self, x, y):
         return x / y
 
 class Mean(nn.Module):
     def __init__(self, dim=0, keepdim=False, biased=False):
         super().__init__()
@@ -358,7 +349,28 @@
 class Squeeze(nn.Module):
     def __init__(self, dim):
         super().__init__()
         self.dim = dim
 
     def forward(self, x):
         return x.squeeze(self.dim)
+
+class Sum(nn.Module):
+    def __init__(self, keepdim: bool, dim=-1):
+        super().__init__()
+        self.dim = dim
+        self.keepdim = keepdim
+
+    def forward(self, x: torch.Tensor):
+        return torch.sum(x, dim=self.dim, keepdim=self.keepdim)
+
+class Expand(nn.Module):
+    def __init__(self, repeats: int, dim=-1):
+        super().__init__()
+        self.repeats = repeats
+        self.dim = dim
+
+    def forward(self, x):
+        assert x.shape[self.dim] == 1
+        repeat_cfg = [-1]*x.ndim
+        repeat_cfg[self.dim] = self.repeats
+        return x.expand(*repeat_cfg)
```

## fmot/nn/composites.py

```diff
@@ -22,15 +22,14 @@
         super().__init__()
         self.matmul = atomics.AddMM()
 
     def forward(self, x, weight, bias):
         weight = weight.t()
         return self.matmul(bias, x, weight)
 
-
 class F_Linear_nb(nn.Module):
     def __init__(self):
         super().__init__()
         self.transpose = atomics.Transpose()
         self.matmul = atomics.Matmul()
 
     def forward(self, x, weight):
@@ -392,14 +391,21 @@
         self.epsilon = epsilon
 
     def forward(self, x, matrix):
         x = torch.matmul(x, matrix)
         return torch.log(x + self.epsilon)
 
 class TuningEpsilon(nn.Module):
+    """Automatically tunes a small +epsilon factor so that it doesn't round to zero
+    after quantization. The value epsilon will be tuned as `eps * running_max`, where
+    `max_abs` is a running maximum input seen by the layer.
+    
+    Arguments:
+        alpha (float): exponential smoothing coefficient, for updating `running_max`
+        eps (float): ratio between max_abs and epsilon"""
     def __init__(self, alpha=0.99, eps=1/128):
         super().__init__()
         self.running_max = 0
         self.alpha = alpha
         self.eps = eps
 
     @torch.jit.ignore()
@@ -415,7 +421,21 @@
         else:
             self.running_max = self.alpha * self.running_max + (1-self.alpha) * xmax
 
     def forward(self, x):
         self.update(x)
         return x + self.epsilon()
 
+class Softmax(nn.Module):
+    def __init__(self, size: int, dim=-1):
+        super().__init__()
+        self.dim = dim 
+        self.sum = atomics.Sum(dim)
+        self.broad = atomics.Expand(size, dim)
+
+    def forward(self, x):
+        e_x = torch.exp(x)
+        den = self.sum(e_x)
+        norm = 1/den
+        norm = self.broad(norm)
+        return e_x * norm
+
```

## fmot/nn/fft.py

```diff
@@ -1,27 +1,33 @@
 import torch
-from torch import nn
+from torch import nn, Tensor
 from fmot.nn import SuperStructure
 import numpy as np
 from typing import *
 
-__all__ = ['FFT', 'RFFT', 'IRFFT']
+__all__ = ['FFT', 'RFFT', 'IRFFT', 'IFFT']
+BASE_RFFT = False
+TWIDDLE_PARALLELISM = 1
+DFT_PARALLELISM = 1
 
 def get_fft_matrices(n_fft, dtype=torch.float32):
     mat = np.fft.fft(np.eye(n_fft))
     m_real = torch.tensor(mat.real, dtype=dtype)
     m_imag = torch.tensor(mat.imag, dtype=dtype)
     return m_real, m_imag
 
-def get_complex_twiddle(n_fft, dtype=torch.float32):
-    w = np.exp(-2j * np.pi / n_fft)
+def get_complex_twiddle(n_fft, dtype=torch.float32, inv=False):
+    sign = -1
+    if inv:
+        sign = 1
+    w = np.exp(sign * 2j * np.pi / n_fft)
     w = np.power(w, np.arange(n_fft//2))
     return torch.tensor(w.real, dtype=dtype), torch.tensor(w.imag, dtype=dtype)
 
-def get_rfft_reverse_matrix(n_fft, dtype=torch.float32):
+def get_reversal_matrix(n_fft, dtype=torch.float32):
     n = n_fft // 2 + 1
     mat = torch.zeros((n_fft - n, n), dtype=dtype)
     for k in range(n_fft - n):
         mat[k, n - k - 1 - ((n_fft+1)%2)] = 1
     return mat
 
 def _get_mod_seq(order):
@@ -33,15 +39,15 @@
         for x in mset:
             new_mset.append(x)
             new_mset.append(x + ord)
         mset = new_mset
 
     return mset
 
-def get_fft_permutation_matrix(N, order, dtype=torch.float32):
+def get_partial_bit_reversal_matrix(N, order, dtype=torch.float32):
     m = np.zeros((N, N))
     perm_set = _get_mod_seq(order)
     base = 2**order
 
     k = 0
     for p in perm_set:
         for j in range(N//base):
@@ -72,32 +78,32 @@
         self.n_fft = n_fft
         self.n = n_fft//2 + 1
         fft_real, fft_imag = get_fft_matrices(n_fft, dtype=torch.float32)
         rfft_real = fft_real[:self.n]
         rfft_imag = fft_imag[:self.n]
         self.rfft_real = nn.Parameter(rfft_real, requires_grad=False)
         self.rfft_imag = nn.Parameter(rfft_imag, requires_grad=False)
-        self.rev = nn.Parameter(get_rfft_reverse_matrix(n_fft), requires_grad=False)
+        self.rev = nn.Parameter(get_reversal_matrix(n_fft), requires_grad=False)
     
     def forward(self, x):
         fwd_real = torch.matmul(x, self.rfft_real.T)
         fwd_imag = torch.matmul(x, self.rfft_imag.T)
 
         rev_real = torch.matmul(fwd_real, self.rev.T)
         rev_imag = torch.matmul(fwd_imag, self.rev.T)
 
         y_real = torch.cat([fwd_real, rev_real], dim=-1)
         y_imag = torch.cat([fwd_imag, -rev_imag], dim=-1)
         return y_real, y_imag
 
 class FFTwiddle(nn.Module):
-    def __init__(self, n_fft: int):
+    def __init__(self, n_fft: int, inv=False):
         super().__init__()
         self.n_fft = n_fft
-        twid_real, twid_imag = get_complex_twiddle(n_fft)
+        twid_real, twid_imag = get_complex_twiddle(n_fft, inv=inv)
         self.twid_real = nn.Parameter(twid_real, requires_grad=False)
         self.twid_imag = nn.Parameter(twid_imag, requires_grad=False)
 
     def forward(self, even_real, even_imag, odd_real, odd_imag):
         todd_real = self.twid_real * odd_real - self.twid_imag * odd_imag
         todd_imag = self.twid_real * odd_imag + self.twid_imag * odd_real
 
@@ -118,69 +124,80 @@
 class FFTPermuter(nn.Module):
     def __init__(self, n_fft, n_stages):
         super().__init__()
         self.n_fft = n_fft
         self.n_stages = n_stages
         self.n_chunks = 2**n_stages
             
-        self.perm = nn.Parameter(get_fft_permutation_matrix(n_fft, n_stages),
+        self.perm = nn.Parameter(get_partial_bit_reversal_matrix(n_fft, n_stages),
                 requires_grad=False)
 
     def forward(self, x):
         y = torch.matmul(x, self.perm)
         return torch.chunk(y, self.n_chunks, dim=-1)
 
 class FFT(SuperStructure):
-    def __init__(self, n_fft, n_stages, dft_parallelism=1, twiddle_parallelism=1,
-        base_rfft=False):
+    """Sparse decomposition of FFT.
+
+    Arguments:
+        n_fft (int): FFT size
+        n_stages (int): number of decomposition stages.
+    """
+    def __init__(self, n_fft: int, n_stages: int):
         super().__init__()
 
-        if base_rfft:
+        if BASE_RFFT:
             dft_class = DFTFromRFFT
         else:
             dft_class = DFT
 
         self.n_fft = n_fft
         self.n_stages = n_stages
         assert n_fft / 2**n_stages % 1 == 0, f'Cannot decompose {n_fft} with {n_stages} power-of-2 stages'
 
-        dft_parallelism = min(2**n_stages, dft_parallelism)
+        dft_parallelism = min(2**n_stages, DFT_PARALLELISM)
         assert dft_parallelism <= 2**n_stages
         self.dft_parallelism = dft_parallelism
-        self.twiddle_parallelism = twiddle_parallelism
+        self.twiddle_parallelism = TWIDDLE_PARALLELISM
 
         self.dfts = nn.ModuleList()
-        for _ in range(dft_parallelism):
+        for _ in range(DFT_PARALLELISM):
             self.dfts.append(dft_class(n_fft//2**n_stages))
 
         if n_stages > 0:
             self.permuter = FFTPermuter(n_fft, n_stages)
             self.twiddle_stages = nn.ModuleList()
 
             stage_size = n_fft//2**(n_stages-1)
             num_calls = n_fft//stage_size
             for _ in range(n_stages):
                 twiddle_list = nn.ModuleList()
-                for j in range(min(num_calls, twiddle_parallelism)):
-                    twiddle_list.append(FFTwiddle(stage_size))
+                for j in range(min(num_calls, TWIDDLE_PARALLELISM)):
+                    twiddle_list.append(FFTwiddle(stage_size, inv=False))
                 self.twiddle_stages.append(twiddle_list)
-                # self.twiddle_stages.append(FFTwiddle(stage_size))
                 stage_size = stage_size * 2
                 num_calls = num_calls//2
 
         else:
             self.permuter = None
             self.twiddle_stages = None
 
         # quantization configs
         self.observe: bool = False
         self.quantize: bool = False
 
     @torch.jit.ignore
-    def forward(self, x):
+    def forward(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        """
+        Arguments:
+            x (Tensor): real-valued tensor of shape (*, n_fft)
+        Returns:
+            - (re, im): two tensors of shape (*, n_fft)
+                The first holds the real-part, and the second holds the imaginary part
+        """
 
         # Fallback to fast implementation of FFT if 
         # not in quantization or observation mode
         if not (self.observe or self.quantize or hasattr(x, 'dimensions')):
             y = torch.fft.fft(x, dim=-1, n=self.n_fft)
             real, imag = y.real, y.imag
             return real, imag
@@ -220,24 +237,20 @@
             return real, imag
                 
     def extra_repr(self) -> str:
         f'n_fft: {self.n_fft} n_stages: {self.n_stages}'
 
 
 class _RFFTDecomp(nn.Module):
-    def __init__(self, n_fft, n_stages, dft_parallelism=1, twiddle_parallelism=1,
-        base_rfft=False):
+    def __init__(self, n_fft, n_stages):
         super().__init__()
         self.n_fft = n_fft
         self.n_stages = n_stages
-        self.dft_parallelism = dft_parallelism
-        self.twiddle_parallelism = twiddle_parallelism
 
-        self.fft = FFT(n_fft, n_stages, dft_parallelism, twiddle_parallelism,
-            base_rfft=base_rfft)
+        self.fft = FFT(n_fft, n_stages)
         self._split0 = int(np.floor(n_fft/2 + 1))
         self._split1 = n_fft - self._split0
 
     def forward(self, x):
         yre, yim = self.fft(x)
         yre, __ = torch.split(yre, [self._split0, self._split1], -1)
         yim, __ = torch.split(yim, [self._split0, self._split1], -1)
@@ -257,52 +270,246 @@
 
     def forward(self, x):
         re = torch.matmul(x, self.rfft_real.T)
         im = torch.matmul(x, self.rfft_imag.T)
         return re, im
 
 class RFFT(nn.Module):
-    def __init__(self, n_fft, n_stages, dft_parallelism=1, twiddle_parallelism=1,
-        base_rfft=False):
+    """Sparse cooley-tukey decomposition of RFFT.
+
+    Arguments:
+        n_fft (int): FFT size
+        n_stages (int): number of decomposition stages.
+    """
+    def __init__(self, n_fft, n_stages):
         super().__init__()
         if n_stages == 0:
             self.rfft = _RFFTDirect(n_fft)
         else:
-            self.rfft = _RFFTDecomp(n_fft, n_stages, dft_parallelism, twiddle_parallelism,
-                base_rfft)
+            self.rfft = _RFFTDecomp(n_fft, n_stages)
         
-    def forward(self, x):
+    def forward(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        """
+        Arguments:
+            x (Tensor): real-valued tensor of shape (*, n_fft)
+        Returns:
+            - (re, im): two tensors of shape (*, n_freq)
+                The first holds the real-part, and the second holds the imaginary part.
+                Here, ``n_freq`` is ``n_fft // 2 + 1``
+        """
         return self.rfft(x)
 
 def get_irfft_matrices(n_fft: int, dtype=torch.float32):
     n = n_fft // 2 + 1
     m_real = np.fft.irfft(np.eye(n))
     m_imag = np.fft.irfft(1j*np.eye(n))
     m_real = torch.tensor(m_real, dtype=dtype)
     m_imag = torch.tensor(m_imag, dtype=dtype)
     return m_real, m_imag
 
+def get_ifft_matrices(n_fft, dtype=torch.float32):
+    mat = np.fft.ifft(np.eye(n_fft))
+    m_real = torch.tensor(mat.real, dtype=dtype)
+    m_imag = torch.tensor(mat.imag, dtype=dtype)
+    return m_real, m_imag
+
 class _IRFFTDirect(nn.Module):
     def __init__(self, n_fft):
         super().__init__()
         self.n_fft = n_fft
         m_real, m_imag = get_irfft_matrices(n_fft, dtype=torch.float32)
 
         self.irfft_real = nn.Parameter(m_real.T, requires_grad=False)
         self.irfft_imag = nn.Parameter(m_imag.T, requires_grad=False)
 
     def forward(self, re, im):
         return torch.matmul(re, self.irfft_real.T) + torch.matmul(im, self.irfft_imag.T)
+    
+class IDFT(nn.Module):
+    def __init__(self, n_fft):
+        super().__init__()
+        self.n_fft = n_fft
+        fft_real, fft_imag = get_ifft_matrices(n_fft, dtype=torch.float32)
+        self.fft_real = nn.Parameter(fft_real, requires_grad=False)
+        self.fft_imag = nn.Parameter(fft_imag, requires_grad=False)
 
-class IRFFT(nn.Module):
+    def forward(self, re, im):
+        y_real = torch.matmul(re, self.fft_real.T) - torch.matmul(im, self.fft_imag.T)
+        y_imag = torch.matmul(re, self.fft_imag.T) + torch.matmul(im, self.fft_real.T)
+        return y_real, y_imag
+    
+class IFFTNormalizer(nn.Module):
+    def __init__(self, n_fft, n_stages):
+        super().__init__()
+        self.n_fft = n_fft
+        self.n_stages = n_stages
+        self.factor = 2**(n_stages)
+
+    def forward(self, x):
+        return x / self.factor
+    
+class IFFT(SuperStructure):
+    def __init__(self, n_fft, n_stages):
+        super().__init__()
+
+        self.n_fft = n_fft
+        self.n_stages = n_stages
+        assert n_fft / 2**n_stages % 1 == 0, f'Cannot decompose {n_fft} with {n_stages} power-of-2 stages'
+
+        dft_parallelism = min(2**n_stages, DFT_PARALLELISM)
+        assert dft_parallelism <= 2**n_stages
+        self.dft_parallelism = dft_parallelism
+        self.twiddle_parallelism = TWIDDLE_PARALLELISM
+
+        self.idfts = nn.ModuleList()
+        for _ in range(dft_parallelism):
+            self.idfts.append(IDFT(n_fft//2**n_stages))
+
+        if n_stages > 0:
+            self.permuter = FFTPermuter(n_fft, n_stages)
+            self.twiddle_stages = nn.ModuleList()
+
+            stage_size = n_fft//2**(n_stages-1)
+            num_calls = n_fft//stage_size
+            for _ in range(n_stages):
+                twiddle_list = nn.ModuleList()
+                for j in range(min(num_calls, self.twiddle_parallelism)):
+                    twiddle_list.append(FFTwiddle(stage_size, inv=True))
+                self.twiddle_stages.append(twiddle_list)
+                stage_size = stage_size * 2
+                num_calls = num_calls//2
+            
+            self.normalizer = IFFTNormalizer(n_fft, n_stages)
+
+        else:
+            self.permuter = None
+            self.twiddle_stages = None
+
+        # quantization configs
+        self.observe: bool = False
+        self.quantize: bool = False
+
+    @torch.jit.ignore
+    def forward(self, re, im):
+
+        if self.permuter is None:
+            return self.idfts[0](re, im)
+
+        else:
+            re_perms = self.permuter(re)
+            im_perms = self.permuter(im)
+
+            sub_dfts = [[],[],[],[]] # stores even_real, even_imag, odd_real, odd_imag sets
+
+            for j, (x_even_re, x_odd_re, x_even_im, x_odd_im) in enumerate(zip(
+                re_perms[::2], re_perms[1::2], im_perms[::2], im_perms[1::2])):
+
+                ev_r, ev_i = self.idfts[2*j % self.dft_parallelism](x_even_re, x_even_im)
+                od_r, od_i = self.idfts[(2*j+1) % self.dft_parallelism](x_odd_re, x_odd_im)
+
+                sub_dfts[0].append(ev_r)
+                sub_dfts[1].append(ev_i)
+                sub_dfts[2].append(od_r)
+                sub_dfts[3].append(od_i)
+
+            for twiddle_list in self.twiddle_stages:
+                new_sub_dfts = [[],[],[],[]]
+                for i, (ev_r, ev_i, od_r, od_i) in enumerate(zip(*sub_dfts)):
+                    twiddler = twiddle_list[i%len(twiddle_list)]
+                    real, imag = twiddler(ev_r, ev_i, od_r, od_i)
+                    if i % 2 == 0:
+                        new_sub_dfts[0].append(real)
+                        new_sub_dfts[1].append(imag)
+                    else:
+                        new_sub_dfts[2].append(real)
+                        new_sub_dfts[3].append(imag)
+                sub_dfts = new_sub_dfts
+            
+            real, imag = sub_dfts[0][0], sub_dfts[1][0]
+
+            real = self.normalizer(real)
+            imag = self.normalizer(imag)
+
+            return real, imag
+                
+    def extra_repr(self) -> str:
+        f'n_fft: {self.n_fft} n_stages: {self.n_stages}'
+
+def get_rfft2fft_matrices(n_fft: int, dtype=torch.float32):
+    """Reconstruct full FFT from RFFT via sparse matrix multiplication.
+
+    Returns 
+        - mat_real: Tensor of shape (n_fft, n_rfft)
+        - mat_imag: Tensor of shape (n_fft, n_rfft)
+
+    Full FFT can be reconstructed from rfft as:
+
+    ```python
+        def rfft2fft(rfft_real, rfft_imag, mat_real, mat_imag):
+            fft_real = torch.matmul(rfft_real, mat_real.t())
+            fft_imag = torch.matmul(rfft_imag, mat_imag.t())
+            return fft_real, fft_imag
+    ```
     """
-    Placeholder for efficient implementation -- for now,
-    just calls the pytorch irfft
+    n_rfft = n_fft // 2 + 1
+
+    mat_real = np.zeros((n_rfft, n_fft))
+    mat_imag = np.zeros((n_rfft, n_fft))
+
+    mat_real[:n_rfft, :n_rfft] = np.eye(n_rfft)
+    mat_imag[:n_rfft, :n_rfft] = np.eye(n_rfft)
+
+    rem = n_fft - n_rfft
+    m_rev = np.eye(rem)[::-1]
+
+    mat_real[1:rem+1, n_rfft:] = m_rev
+    mat_imag[1:rem+1, n_rfft:] = -m_rev
+
+    mat_real = torch.tensor(mat_real.T, dtype=dtype)
+    mat_imag = torch.tensor(mat_imag.T, dtype=dtype)
+    return mat_real, mat_imag
+
+class _IRFFTDecomp(nn.Module):
+    def __init__(self, n_fft: int, n_stages: int):
+        super().__init__()
+        
+        mat_real, mat_imag = get_rfft2fft_matrices(n_fft)
+        self.mat_real = nn.Parameter(mat_real, requires_grad=False)
+        self.mat_imag = nn.Parameter(mat_imag, requires_grad=False)
+
+        self.ifft = IFFT(n_fft, n_stages)
+
+    def forward(self, re, im):
+        re = torch.matmul(re, self.mat_real.t())
+        im = torch.matmul(im, self.mat_imag.t())
+
+        # run and discard the imaginary component
+        y, __ = self.ifft(re, im)
+        return y
+
+class IRFFT(nn.Module):
+    """Sparse cooley-tukey decomposition of IRFFT.
+
+    Arguments:
+        n_fft (int): FFT size
+        n_stages (int): number of decomposition stages.
     """
-    def __init__(self, n_fft):
+    def __init__(self, n_fft, n_stages: int=0):
         super().__init__()
         self.n_fft = n_fft
 
-        self.irfft = _IRFFTDirect(n_fft)
+        if n_stages == 0:
+            self.irfft = _IRFFTDirect(n_fft)
+        else:
+            self.irfft = _IRFFTDecomp(n_fft, n_stages)
 
-    def forward(self, re, im):
+    def forward(self, re: Tensor, im: Tensor) -> Tensor:
+        """Compute the IRFFT given tensors holding the real and imaginary components.
+        
+        Arguments:
+            re (Tensor): real-part of the RFFT to invert, shape ``(*, n_fft//2 + 1)``
+            im (Tensor): imaginary-part of the RFFT to invert, shape ``(*, n_fft//2 + 1)``
+        
+        Returns:
+            Tensor, real-valued inversion of the input RFFT.
+        """
         return self.irfft(re, im)
```

## fmot/nn/sequenced_rnn.py

```diff
@@ -2,14 +2,15 @@
 import math
 from torch import nn
 from ..utils import rsetattr, rgetattr
 from .sequencer import Sequencer, unbind, stack, chunk, cat
 from .super_structures import SuperStructure
 from .atomics import Identity
 from fmot.utils import ActivationCountingReLU
+from fmot import CONFIG
 
 # We need to import these for explicit type annotations
 from typing import List, Tuple, Optional, Any
 from torch import Tensor
 
 # TODO: For Conv1d, Padding (left padding by default now), stride, dilatation, padding_mode
 
@@ -71,14 +72,17 @@
         seq_dim = 1 if batch_first else 0
         super().__init__(state_shapes, batch_dim, seq_dim)
         self.linear_ih = nn.Linear(self.input_size, self.hidden_size, self.bias)
         self.linear_hh = nn.Linear(self.hidden_size, self.hidden_size, self.bias)
 
         if self.nonlinearity == 'tanh':
             self.nonlinearity_layer = torch.nn.Tanh()
+            if CONFIG.rnn_mm_limits:
+                self.linear_ih.limits = (-4, 4)
+                self.linear_hh.limits = (-4, 4)
         elif self.nonlinearity == 'relu':
             self.nonlinearity_layer = torch.nn.ReLU()
         elif self.nonlinearity == 'identity':
             self.nonlinearity_layer = torch.nn.Identity()
         else:
             raise ValueError("Unknown nonlinearity '{}'".format(self.nonlinearity))
 
@@ -120,14 +124,18 @@
         # Base class must be initialized with state-shape and optionally batch_first attributes
         batch_dim = 0 if batch_first else 1
         seq_dim = 1 if batch_first else 0
         super().__init__(state_shapes, batch_dim, seq_dim)
         self.linear_ih = nn.Linear(self.input_size, 4 * self.hidden_size, self.bias)
         self.linear_hh = nn.Linear(self.hidden_size, 4 * self.hidden_size, self.bias)
 
+        if CONFIG.rnn_mm_limits:
+            self.linear_ih.limits = (-8, 8)
+            self.linear_hh.limits = (-8, 8)
+
         self.weight_init()
 
     @torch.jit.export
     def step(self, x_t: Tensor, state: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
         h_t, c_t = state
         stacked_layer = self.linear_ih(x_t) + self.linear_hh(h_t)
 
@@ -146,14 +154,71 @@
     def _from_torchmodule(cls, parent, toplevel=None, inherited_name="", inherited_dict=dict()):
         sequencer = cls(input_size=parent.input_size, hidden_size=parent.hidden_size,
                         bias=parent.bias, batch_first=parent.batch_first, dropout=parent.dropout)
 
         transfer_param(parent, sequencer, inherited_name, inherited_dict)
 
         return sequencer
+    
+class FusedLSTMCell(Sequencer):
+    r'''FusedLSTMCell performs matrix-fusion, combining the forward and recurrent matrices into one
+    matrix. This allows better quantization, since partial ih and hh products are added together at
+    i32 precision, instead of being serialized at i16 or i8 before adding.
+    '''
+
+    def __init__(self, input_size: int, hidden_size: int, bias=True, batch_first=False,
+                 dropout=0):
+        # state_shapes is a list of hidden-state shapes
+        state_shapes = [[hidden_size], [hidden_size]]
+        self.input_size = input_size
+        self.hidden_size = hidden_size
+        self.bias = bias
+        self.batch_first = batch_first
+        self.dropout = dropout
+
+        # Base class must be initialized with state-shape and optionally batch_first attributes
+        batch_dim = 0 if batch_first else 1
+        seq_dim = 1 if batch_first else 0
+        super().__init__(state_shapes, batch_dim, seq_dim)
+        self.linear = nn.Linear(self.input_size + self.hidden_size, 4 * self.hidden_size, self.bias)
+
+        self.linear.limits = (-8, 8)
+
+        self.weight_init()
+
+    @torch.jit.export
+    def step(self, x_t: Tensor, state: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
+        h_t, c_t = state
+        e_t = torch.cat([x_t, h_t], dim=-1)
+        stacked_layer = self.linear(e_t)
+
+        i_t, f_t, g_t, o_t = stacked_layer.chunk(4, 1)
+        i_t = torch.sigmoid(i_t)
+        f_t = torch.sigmoid(f_t)
+        g_t = torch.tanh(g_t)
+        o_t = torch.sigmoid(o_t)
+
+        c_t = f_t * c_t + i_t * g_t
+        h_t = o_t * torch.tanh(c_t)
+
+        return h_t, [h_t, c_t]
+    
+    def transfer_lstm_params(self, parent: torch.nn.LSTM, layer_idx=0):
+        w_ih = getattr(parent, f'weight_ih_l{layer_idx}').data
+        w_hh = getattr(parent, f'weight_hh_l{layer_idx}').data
+        weight = torch.cat([w_ih, w_hh], dim=-1)
+
+        self.linear.weight.data = weight
+
+        if parent.bias:
+            b_ih = getattr(parent, f'bias_ih_l{layer_idx}').data
+            b_hh = getattr(parent, f'bias_hh_l{layer_idx}').data
+            bias = b_ih + b_hh
+
+            self.linear.bias.data = bias
 
 
 class GRUCell(Sequencer):
     r''' Define a logic unit for baseline GRU
     '''
 
     def __init__(self, input_size: int, hidden_size: int, bias=True, batch_first=False,
@@ -168,14 +233,18 @@
         # Base class must be initialized with state-shape and optionally batch_first attributes
         batch_dim = 0 if batch_first else 1
         seq_dim = 1 if batch_first else 0
         super().__init__(state_shapes, batch_dim, seq_dim)
         self.linear_ih = nn.Linear(self.input_size, 3 * self.hidden_size, self.bias)
         self.linear_hh = nn.Linear(self.hidden_size, 3 * self.hidden_size, self.bias)
 
+        if CONFIG.rnn_mm_limits:
+            self.linear_ih.limits = (-8, 8)
+            self.linear_hh.limits = (-8, 8)
+            
         self.weight_init()
 
     @torch.jit.export
     def step(self, x_t: Tensor, state: List[Tensor]) -> Tuple[Tensor, List[Tensor]]:
         h_t, = state
 
         stacked_layer_i = self.linear_ih(x_t)
@@ -193,18 +262,16 @@
 
         return h_t, [h_t]
 
     @classmethod
     def _from_torchmodule(cls, parent, toplevel=None, inherited_name="", inherited_dict=dict()):
         sequencer = cls(input_size=parent.input_size, hidden_size=parent.hidden_size,
                         bias=parent.bias, batch_first=parent.batch_first, dropout=parent.dropout)
-
         transfer_param(parent, sequencer, inherited_name, inherited_dict)
-
-        return sequencer
+        return sequencer    
 
 
 class MultiLayerRNN(SuperStructure):
     def __init__(self, layers: List[Sequencer]):
         r"""MultiLayers RNNs are a super structures from which custom multi-layers RNN should be subclassed. 
         They allow the user to define control-flows in the forward method at training time, but these control 
         flows will be frozem in the final FQIR graph (see FQIR documentation).
@@ -465,18 +532,23 @@
         self.input_size = input_size
         self.hidden_size = hidden_size
         self.num_layers = num_layers
         self.bias = bias
         self.batch_first = batch_first
         self.dropout = dropout
 
+        if CONFIG.fused_lstm:
+            cell_cls = FusedLSTMCell
+        else:
+            cell_cls = LSTMCell
+
         layers = [
-            LSTMCell(self.input_size, self.hidden_size, self.bias, self.batch_first, \
+            cell_cls(self.input_size, self.hidden_size, self.bias, self.batch_first, \
                      self.dropout), \
-            *[LSTMCell(self.hidden_size, self.hidden_size, self.bias, self.batch_first, \
+            *[cell_cls(self.hidden_size, self.hidden_size, self.bias, self.batch_first, \
                        self.dropout) for _ in range(num_layers - 1)]
         ]
 
         super().__init__(layers)
 
     @torch.jit.export
     def forward(self, x, state: Optional[List[Tensor]] = None) -> Tuple[Tensor, List[Tensor]]:
@@ -488,20 +560,24 @@
                 state_tprev_l = [state[2 * l], state[2 * l + 1]]
             x, state_l = layer(x, state_tprev_l)
             state_out.append(state_l[0])
             state_out.append(state_l[1])
         return x, state_out
 
     @classmethod
-    def _from_torchmodule(cls, parent, toplevel=None, inherited_name="", inherited_dict=dict()):
+    def _from_torchmodule(cls, parent: torch.nn.LSTM, toplevel=None, inherited_name="", inherited_dict=dict()):
         multilayer_rnn = cls(input_size=parent.input_size, hidden_size=parent.hidden_size,
                              bias=parent.bias, num_layers=parent.num_layers,
                              batch_first=parent.batch_first, dropout=parent.dropout)
-
-        transfer_param(parent, multilayer_rnn, inherited_name, inherited_dict)
+        if CONFIG.fused_lstm:
+            for idx in range(parent.num_layers):
+                layer: FusedLSTMCell = multilayer_rnn.layers[idx]
+                layer.transfer_lstm_params(parent, idx)
+        else:
+            transfer_param(parent, multilayer_rnn, inherited_name, inherited_dict)
 
         return multilayer_rnn
 
 
 class GRU(MultiLayerRNN):
     r"""Generate a MultiLayerRNN equivalent of a PyTorch multi-layer gated recurrent unit (GRU) RNN. Can be applied
     it to an input sequence. 
@@ -600,17 +676,17 @@
         self.hidden_size = hidden_size
         self.num_layers = num_layers
         self.bias = bias
         self.batch_first = batch_first
         self.dropout = dropout
 
         layers = [
-            GRUCell(self.input_size, self.hidden_size, self.bias, self.batch_first, \
-                    self.dropout), \
-            *[GRUCell(self.hidden_size, self.hidden_size, self.bias, self.batch_first, \
+            GRUCell(self.input_size, self.hidden_size, self.bias, self.batch_first, 
+                    self.dropout), 
+            *[GRUCell(self.hidden_size, self.hidden_size, self.bias, self.batch_first, 
                       self.dropout) for _ in range(num_layers - 1)]
         ]
 
         super().__init__(layers)
 
     @classmethod
     def _from_torchmodule(cls, parent, toplevel=None, inherited_name="", inherited_dict=dict()):
```

## fmot/nn/sequencer.py

```diff
@@ -149,7 +149,14 @@
     def set_streaming(self, stream=True):
         if stream:
             self._streaming = True
         else:
             self._streaming = False
             self.state = None
             self.prev_state = None
+
+    def to(self, device, *args, **kwargs):
+        super().to(device=device, *args, **kwargs)
+        if state is not None:
+            state = [x.to(device) for x in state]
+            print('state to device')
+
```

## fmot/nn/stft.py

```diff
@@ -68,16 +68,25 @@
         super().__init__()
         self.zeros = nn.Parameter(torch.zeros(n), requires_grad=False)
     
     def forward(self, x):
         return torch.cat([x, self.zeros], -1)
 
 class STFT(SuperStructure):
+    """Short-Time Fourier Transform
+
+    Arguments:
+        n_fft (int): size of FFT, in samples
+        hop_size (int): hop size, in samples
+        n_stages (int): number of stages in Cooley-Tukey decomposition of RFFT
+        window_size (int): window size, in samples. If ``None``, defaults to ``n_fft``
+        window_fn (Tensor): Optional window function. Should be a 1D of length ``n_fft``
+    """
     def __init__(self, n_fft: int, hop_size: int, n_stages: int, window_size: int=None,
-        window_fn: Tensor=None, base_rfft=False):
+        window_fn: Tensor=None):
         super().__init__()
         self.n_fft = n_fft
         self.hop_size = hop_size
         if window_size is None:
             window_size = n_fft
         self.window_size = window_size
         self.n_stages = n_stages
@@ -91,18 +100,31 @@
             self.catter = ZeroCatter(n_fft - window_size)
         elif window_size > n_fft:
             raise ValueError('window_size cannot exceed n_fft')
         else:
             self.catter = None
         
         self.buffer = STFTBuffer(window_size, hop_size)
-        self.rfft = RFFT(n_fft, n_stages, base_rfft=base_rfft)
-
-    def forward(self, x):
+        self.rfft = RFFT(n_fft, n_stages)
 
+    def forward(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        """Compute the STFT of a real-valued signal.
+        
+        Arguments:
+            x (Tensor): real-valued input signal, of shape ``(batch, N, hop_size)``
+        
+        Returns:
+            (re, im): real and imaginary parts of the STFT, held in separate real-valued
+                tensors. Each of shape ``(batch, N, n_fft//2 + 1)``
+
+        .. note::
+
+            The input signal must already be separated into non-overlapping ``hop_size``
+            length frames. 
+        """
         # concatenate with previous frames
         x_stack, __ = self.buffer(x)
 
         # optionally apply window_fn:
         if self.window_mul is not None:
             x_stack = self.window_mul(x_stack)
 
@@ -168,23 +190,71 @@
         x_curr, x_next = torch.chunk(x, 2, -1)
         s_curr, = state
         x = x_curr + s_curr
         return x, [x_next]
         
 class OverlapAdd50Pct(nn.Module):
     """50% Overlap-Add Decoding. Takes overlapping waveforms and performs
-    overlap-add, multiplying by a constant/time-varying factor if a window-function
+    overlap-add, multiplying by a constant or time-varying factor if a window-function
     is used.
     """
     def __init__(self, hop_size: int, window: Tensor=None):
         super().__init__()
         if window is not None:
             self.synthesis_window = SynthesisWindow(window)
 
         else:
             self.synthesis_window = ConstantMul(0.5)
         self.ola = _OverlapAdd50pct(hop_size)
 
     def forward(self, x):
         x = self.synthesis_window(x)
         y, __ = self.ola(x)
-        return y
+        return y
+    
+class ISTFT(nn.Module):
+    """Inverse Short-Time Fourier Transform
+
+    Arguments:
+        n_fft (int): size of FFT, in samples
+        hop_size (int): hop size, in samples
+        n_stages (int): number of stages in Cooley-Tukey decomposition of RFFT
+        window_size (int): window size, in samples. If ``None``, defaults to ``n_fft``
+        window_fn (Tensor): Optional window function. Should be a 1D of length ``n_fft``
+
+    .. seealso:
+
+        `scipy.signal.stft <https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.istft.html>`_ has 
+        good documentation explaining OLA (see the Note at the bottom of the page)
+
+    .. warning:
+
+        Presently, restricted to the 50% overlap case where ``n_fft == window_size == 2*hop_size``
+    """
+    def __init__(self, n_fft: int, hop_size: int, n_stages: int, window_size: int=None,
+        window_fn: Tensor=None):
+        super().__init__()
+        self.n_fft = n_fft
+        self.hop_size = hop_size
+        if window_size is None:
+            window_size = n_fft
+        
+        assert window_size == n_fft, 'window_size != n_fft not yet supported in ISTFT'
+        assert window_size == 2 * hop_size, r'ISTFT with overlap other than 50% not yet supported in ISTFT'
+
+        self.irfft = IRFFT(n_fft, n_stages)
+        self.ola = OverlapAdd50Pct(hop_size, window=window_fn)
+
+    def forward(self, re: Tensor, im: Tensor) -> Tensor:
+        """Compute the ISTFT given tensors holding the real and imaginary spectral components.
+        
+        Arguments:
+            re (Tensor): real-part of the STFT to invert, shape ``(batch, N, n_fft//2 + 1)``
+            im (Tensor): imaginary-part of the STFT to invert, shape ``(batch, N, n_fft//2 + 1)``
+        
+        Returns:
+            Tensor, real-valued inversion of the input STFT, with overlap-add inversion.
+            shape: (batch, N, hop_size)
+        """
+        winsig = self.irfft(re, im)
+        olasig = self.ola(winsig)
+        return olasig
```

## fmot/qat/nn/__init__.py

```diff
@@ -3,9 +3,10 @@
 from .quantizers import *
 from .linear import *
 from .sequencer import *
 from .density_matmul import *
 from .quant_wrap import *
 from .luts import *
 from .norm import *
-from .high_level import *
+from .temporal_unfold import TemporalUnfold1d
 from .lstm import LSTM, LSTMConfig
+from .derived_param import *
```

## fmot/qat/nn/atomics.py

```diff
@@ -104,15 +104,16 @@
     def _from_float(cls, parent, bw_conf, interpolate,
         observer=quantizers.DEFAULT_OBSERVERS['default'], **kwargs):
         observer = partial(observer, **kwargs)
         return cls(bitwidth=bw_conf.activations, observer=observer)
 
     def _get_constants(self, x, y):
         z = self.forward(x, y)
-        return _get_add_constants(x, y, z)
+        constants = _get_add_constants(x, y, z)
+        return constants
 
 class VIAdd(AtomicModule):
     def __init__(self, imm, bitwidth, observer=quantizers.DEFAULT_OBSERVERS['default']):
         super().__init__()
         self.imm = nn.Parameter(torch.tensor(imm), requires_grad=False)
         self.imm_quantizer = quantizers.ParameterQuantizer(bitwidth)
         self.quantizer = quantizers.Quantizer(bitwidth, observer=observer)
```

## fmot/qat/nn/composites.py

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 from .quantizers import FixedRangeObserver
 from ._utils import intitem
 from fmot.nn import LUT as LUT_FP
 from .luts import LUT, AddIdentityTLUT, ILUT
 import fmot
 from functools import partial
+from .linear import Linear
 
 class Div(nn.Module):
     def __init__(self, bitwidth, lut_bitwidth, bw_conf, interpolate):
         super().__init__()
         parent = LUT_FP(fmot.LUT_REGISTRY['aten::reciprocal'])
         self.recip = LUT._from_float(parent, bw_conf, interpolate)
         self.mul = atomics.VVMul(bitwidth)
@@ -219,7 +220,11 @@
     @classmethod
     def _from_float(cls, parent, bw_conf, interpolate, 
         observer=quantizers.DEFAULT_OBSERVERS['default'], **observer_kwargs):
         
         observer = partial(observer, **observer_kwargs)
         return cls(bw_conf.activations, running_max=parent.running_max,
             observer=observer, alpha=parent.alpha)
+
+
+
+
```

## fmot/qat/nn/density_matmul.py

```diff
@@ -4,14 +4,15 @@
 import torch
 
 from .atomics import AtomicModule, _get_mul_constants, ACC_BW
 from ._utils import intitem
 from . import quantizers
 from ..annotated_tensors import check_for_annotations, set_dim_annotations, get_dim_annotations, annotate
 from ..fake_quantization import fake_quantize
+from copy import deepcopy
 
 ROUND_NEAREST = False
 
 def is_sparse(*tensors):
     """Returns a boolean list -- whether each tensor has a nonzero average sparsity
     """
     return [x.prev_relu for x in tensors]
@@ -66,37 +67,42 @@
     """
     def __init__(self, matcol_dim=None):
         super().__init__()
         self.matcol_dim = matcol_dim
         self.has_sparse_input = False
 
         # Factors that are updated after forward pass
-        self.delta = None
+        self.register_buffer('delta', None)
         self.nb_iter = None
-        self.mat = None
+        self.register_buffer('mat', None)
         self.batch_dim = None
 
         # Factors that are updated when metrics are computed
-        self._fanout = None
+        self.register_buffer('_fanout', None)
 
-        self.act_density = None
-        self.lookup_density = None
-        self.fanout_density = None
+        self.register_buffer('act_density', None)
+        self.register_buffer('lookup_density', None)
+        self.register_buffer('fanout_density', None)
 
     def _update_factors(self, delta_updt, mat, nb_iter_updt):
         """Private method: updates internal store of factors to
         compute activations density metrics later.
 
         Args:
             delta (tensor): Per-element average vector density,
                 which is a tensor that has same size as the act. vector.
         """
         if self.delta is None:
             self.delta = delta_updt / nb_iter_updt
+            #print(self.delta.device)
         else:
+            # TODO:handle that better. Why is to() method not called from Linear?
+            #print(self.delta.device)
+            #print(delta_updt.device)
+            #self.delta = self.delta.to(delta_updt.device)
             self.delta = (self.nb_iter * self.delta + delta_updt) / (self.nb_iter + nb_iter_updt)
 
         if self.nb_iter is None:
             self.nb_iter = nb_iter_updt
         else:
             self.nb_iter += nb_iter_updt
 
@@ -185,40 +191,43 @@
             return None
         layer_fanout = self.delta.dot(self.fanout()) * self.nb_iter
         layer_weight = self.fanout().sum() * self.nb_iter
         self.lookup_density = layer_fanout / layer_weight
 
         return layer_fanout, layer_weight
 
+
 class Matmul(_MMBase):
     def __init__(self, bitwidth, observer=quantizers.DEFAULT_OBSERVERS['default']):
         super().__init__()
         self.quantizer = quantizers.Quantizer(bitwidth, observer=observer)
 
     @check_for_annotations
     def forward(self, x, y):
         if self._check_for_sparsity(x, y):
             self._register_density_factors(x, y)
         dimensions = get_dim_annotations(x, y)
+
         return self.quantizer(set_dim_annotations(dimensions,
             torch.matmul(x, y)))
 
     @classmethod
     def _from_float(cls, parent, bw_conf, interpolate,
         observer=quantizers.DEFAULT_OBSERVERS['default'], **kwargs):
         observer = partial(observer, **kwargs)
         return cls(bitwidth=bw_conf.activations, observer=observer)
 
     def _get_constants(self, x, y):
         z = self.forward(x, y)
         constants = _get_mul_constants(x, y, z)
+
         if self.quantize:
             constants['bw_out'] = z.bitwidth.bitwidth
             del constants['bw']
-        return constants
+        return deepcopy(constants)
 
 class NoShiftMM(_MMBase):
     def __init__(self, bitwidth):
         super().__init__()
         self.bitwidth = bitwidth
 
     @check_for_annotations
```

## fmot/qat/nn/linear.py

```diff
@@ -1,42 +1,50 @@
 import math
 from functools import partial
 
 import torch
 from torch import nn
-
+from fmot import CONFIG
 from . import atomics, quantizers
 from .density_matmul import AddMM, Matmul
 from ..annotated_tensors import set_dim_annotations
 
 class Linear(torch.nn.Module):
     def __init__(self, in_features, out_features, act_bitwidth, par_bitwidth,
-        bias=True, observer=quantizers.DEFAULT_OBSERVERS['default']):
+        bias=True, observer=quantizers.DEFAULT_OBSERVERS['default'], 
+        mm_limits=None):
         super().__init__()
 
         self.q_group = quantizers.PrecisionConstraint()
 
         self.in_features = in_features
         self.out_features = out_features
+
         self.requant_in = atomics.Requantize(act_bitwidth, observer)
         self.q_group.recursively_add(self.requant_in)
         self.weight = nn.Parameter(torch.Tensor(out_features, in_features))
         self.weight_quant = quantizers.ParameterQuantizer(par_bitwidth,
             observer=quantizers.DEFAULT_OBSERVERS['param'])
         self.q_group.add(self.weight_quant)
         self.weight_transpose = atomics.Transpose()
+
+        if mm_limits is None:
+            mm_observer = observer
+        else:
+            mm_observer = partial(quantizers.FixedRangeObserver, limits=mm_limits)
+
         if bias:
             self.bias = nn.Parameter(torch.Tensor(out_features))
             set_dim_annotations(['F'], self.bias)
-            self.multiplier = AddMM(act_bitwidth, observer=observer)
+            self.multiplier = AddMM(act_bitwidth, observer=mm_observer)
             self.bias_quant = quantizers.ParameterQuantizer(act_bitwidth,
                 observer=quantizers.DEFAULT_OBSERVERS['param'])
         else:
             self.register_parameter('bias', None)
-            self.multiplier = Matmul(act_bitwidth, observer=observer)
+            self.multiplier = Matmul(act_bitwidth, observer=mm_observer)
         self.reset_parameters()
 
     def reset_parameters(self):
         nn.init.kaiming_uniform_(self.weight, a=math.sqrt(5))
         if self.bias is not None:
             fan_in, _ = nn.init._calculate_fan_in_and_fan_out(self.weight)
             bound = 1 / math.sqrt(fan_in)
@@ -61,19 +69,157 @@
             self.multiplier.quantizer.bitwidth, self.weight_quant.bitwidth
         )
 
     @classmethod
     def _from_float(cls, parent, bw_conf, interpolate,
         observer=quantizers.DEFAULT_OBSERVERS['default'], **kwargs):
         observer = partial(observer, **kwargs)
+        limits = None
+        if hasattr(parent, 'limits'):
+            limits = parent.limits
+        kwargs = dict(
+            in_features=parent.in_features,
+            out_features=parent.out_features,
+            act_bitwidth=bw_conf.activations,
+            par_bitwidth=bw_conf.weights,
+            bias=parent.bias is not None,
+            observer=observer,
+            mm_limits=limits
+        )
+        if CONFIG.pow2_linear_scale:
+            model = cls(**kwargs)
+        else:
+            if not CONFIG.perchannel_linear:
+                model = AffineLinear(**kwargs)
+            else:
+                model = PerChannelAffineLinear(**kwargs)
+        model.weight.data = parent.weight.data
+        if model.bias is not None:
+            model.bias.data = parent.bias.data
+        return model
+    
+class AffineLinear(Linear):
+    def __init__(self, in_features, out_features, act_bitwidth, par_bitwidth,
+        bias=True, observer=quantizers.DEFAULT_OBSERVERS['default'], mm_limits=None):
+        if mm_limits is not None:
+            mul_limits = tuple(map(lambda x: 2*x if x is not None else None, mm_limits))
+            vimul_obs = partial(quantizers.FixedRangeObserver, limits=mm_limits)
+        else:
+            mul_limits = None
+            vimul_obs = observer
+        super().__init__(in_features, out_features, act_bitwidth, par_bitwidth,
+            bias, observer, mm_limits=mul_limits)
+        self.vimul = atomics.VIMul(1, act_bitwidth, vimul_obs)
+
+        bw = par_bitwidth.bitwidth
+        self.factor = (2**(bw-1) - 1) / 2**(bw-1)
+
+    def reset_parameters(self):
+        nn.init.kaiming_uniform_(self.weight, a=math.sqrt(5))
+        if self.bias is not None:
+            fan_in, _ = nn.init._calculate_fan_in_and_fan_out(self.weight)
+            bound = 1 / math.sqrt(fan_in)
+            nn.init.uniform_(self.bias, -bound, bound)
+
+    def forward(self, x):
+        x = self.requant_in(x)
+
+        wmax = torch.max(torch.abs(self.weight)) / self.factor
+        with torch.no_grad():
+            p2fact = torch.ceil(torch.log2(wmax))
+        wmax = wmax / 2**(p2fact)
+        w_normed = self.weight / wmax
+        set_dim_annotations(['F', 'F'], w_normed)
+        w_normed = self.weight_quant(w_normed)
+        set_dim_annotations(['F', 'F'], w_normed)
+        w_normed = self.weight_transpose(w_normed)
+        if self.bias is not None:
+            b_normed = self.bias / wmax
+            set_dim_annotations(['F'], b_normed)
+            b_normed = self.bias_quant(b_normed)
+            set_dim_annotations(['F'], b_normed)
+
+            out_normed = self.multiplier(b_normed, x, w_normed)
+
+        else:
+            out_normed = self.multiplier(x, w_normed)
+
+        self.vimul.imm.data = wmax
+        out = self.vimul(out_normed)
+        return out
+
+    def __repr__(self):
+        return 'QuantAffineLinear(in_features={}, out_features={}, bias={}, act_bw={}, par_bw={})'.format(
+            self.in_features, self.out_features, self.bias is not None,
+            self.multiplier.quantizer.bitwidth, self.weight_quant.bitwidth
+        )
+    
+class PerChannelAffineLinear(Linear):
+    def __init__(self, in_features, out_features, act_bitwidth, par_bitwidth,
+        bias=True, observer=quantizers.DEFAULT_OBSERVERS['default'], mm_limits=None):
+        if mm_limits is not None:
+            mul_limits = tuple(map(lambda x: 2*x if x is not None else None, mm_limits))
+            vvmul_obs = partial(quantizers.FixedRangeObserver, limits=mm_limits)
+        else:
+            mul_limits = None
+            vvmul_obs = observer
+        super().__init__(in_features, out_features, act_bitwidth, par_bitwidth, bias, observer,
+                         mm_limits=mul_limits)
+
+        self.norm_quant = quantizers.ParameterQuantizer(act_bitwidth, observer=observer)
+        self.renorm = atomics.VVMul(act_bitwidth, vvmul_obs)
+
+        bw = par_bitwidth.bitwidth
+        self.factor = (2**(bw-1) - 1) / 2**(bw-1)
+
+    def forward(self, x):
+        x = self.requant_in(x)
+
+        max_per_chan, __ = torch.abs(self.weight).max(dim=-1) 
+        max_per_chan = max_per_chan / self.factor + 1e-6
+
+        with torch.no_grad():
+            p2fact = torch.ceil(torch.log2(max_per_chan.max()))
+        max_per_chan = max_per_chan / 2**(p2fact)
+
+        w_normed = self.weight / max_per_chan.unsqueeze(-1)
+        set_dim_annotations(['F', 'F'], w_normed)
+        w_normed = self.weight_quant(w_normed)
+        set_dim_annotations(['F', 'F'], w_normed)
+        w_normed = self.weight_transpose(w_normed)
+        if self.bias is not None:
+            b_normed = self.bias / max_per_chan
+            set_dim_annotations(['F'], b_normed)
+            b_normed = self.bias_quant(b_normed)
+            set_dim_annotations(['F'], b_normed)
+
+            out_normed = self.multiplier(b_normed, x, w_normed)
+
+        else:
+            out_normed = self.multiplier(x, w_normed)
+
+        norm = self.norm_quant(max_per_chan)
+        out = self.renorm(out_normed, norm)
+        return out
+    
+    @classmethod
+    def _from_float(cls, parent, bw_conf, interpolate,
+        observer=quantizers.DEFAULT_OBSERVERS['default'], **kwargs):
+        observer = partial(observer, **kwargs)
         model = cls(
                 in_features=parent.in_features,
                 out_features=parent.out_features,
                 act_bitwidth=bw_conf.activations,
                 par_bitwidth=bw_conf.weights,
                 bias = parent.bias is not None,
                 observer = observer
             )
         model.weight.data = parent.weight.data
         if model.bias is not None:
             model.bias.data = parent.bias.data
         return model
+    
+    def __repr__(self):
+        return 'QuantPerChannelAffineLinear(in_features={}, out_features={}, bias={}, act_bw={}, par_bw={})'.format(
+            self.in_features, self.out_features, self.bias is not None,
+            self.multiplier.quantizer.bitwidth, self.weight_quant.bitwidth
+        )
```

## fmot/qat/nn/lstm.py

```diff
@@ -8,19 +8,18 @@
 from typing import *
 from fmot.qat.bitwidths import fqint4, fqint8, fqint16, Bitwidth, BitwidthConfig
 import math
 from dataclasses import dataclass
 import numpy as np
 from fmot.qat.annotated_tensors import annotate, asint
 from torch.nn.utils.prune import custom_from_mask, remove
+from fmot.configure import CONFIG
 
-LUT_INTERPOLATION = True
 CALIBRATE_CELL = True
 CALIBRATE_MM = True
-PARAM_OBS = GaussianObserver
 MOV_AVG_CALIBRATION = False
 
 def remove_pruning(model: torch.nn.Module):
     r""" Remove the pruning reparametrization from all the
          modules of a model.
 
     Args:
@@ -225,15 +224,15 @@
         
         self.param_quantizers = torch.nn.ModuleDict()
         for (name, param) in parent.named_parameters():
             if param.ndim == 2:
                 bw = self.config.param_bw
             else:
                 bw = self.config.act_bw
-            pq = ParameterQuantizer(bitwidth=bw, observer=PARAM_OBS)
+            pq = ParameterQuantizer(bitwidth=bw, observer=DEFAULT_OBSERVERS['lstm'])
             pq.quantize = self.quantize
             pq.observe = self.quantize
             self.param_quantizers[name] = pq
             self.register_parameter(name, param)
 
 
     def get_weights(self, layer_idx: int) -> Dict[str, Tensor]:
@@ -277,15 +276,15 @@
             b_addr=self.config.lut_bw.bitwidth,
             q_sig_addr=self.config.sigmoid_addr_quanta,
             q_tanh_addr=self.config.tanh_addr_quanta,
             q_unity=self.config.unity_quanta,
             q_mm_ih=q_mm_ih,
             q_mm_hh=q_mm_hh,
             q_c=q_c,
-            interpolate=LUT_INTERPOLATION
+            interpolate=CONFIG.lstm_interpolate
         )
 
     @torch.no_grad()
     def quantize_input(self, x: Tensor, quantize: bool=False) -> Tensor:
         x_maxabs = x.abs().max()
         if self.input_maxabs == 0:
             self.input_maxabs = x_maxabs
@@ -495,15 +494,15 @@
             addr_quanta=self.config.tanh_addr_quanta,
             out_bits=self.config.act_bw.bitwidth,
             out_quanta=self.config.unity_quanta)
         return sigmoid, tanh
 
     def _get_constants(self, x, h=None, c=None) -> dict:
         
-        assert h is None, 'Cannot hanlde initial hidden state yet for LSTM'
+        assert h is None, 'Cannot handle initial hidden state yet for LSTM'
         assert c is None, 'Cannot handle initial cell state yet for LSTM'
 
         sigmoid, tanh = self.get_tables()
         constants = dict(
             num_layers=self.num_layers,
             batch_first=self.batch_first,
             sigmoid=sigmoid,
```

## fmot/qat/nn/luts.py

```diff
@@ -1,10 +1,11 @@
 from .atomics import *
 from . import quantizers
 from functools import partial
+from fmot import CONFIG
 
 class LUT(nn.Module):
     def __init__(self, function, bitwidth, lut_bitwidth, limits=None,
         observer=quantizers.DEFAULT_OBSERVERS['default']):
         super().__init__()
         if limits is None:
             limits = (None, None)
@@ -58,27 +59,30 @@
             else:
                 return cls(**kwargs)
         else:
             return cls(
                 bitwidth=bw_conf.activations, 
                 lut_bitwidth=bw_conf.lut)
 
+
 class ILUT(nn.Module):
     """
     Interpolating Lookup Table
     Technically a composite -- defined here to avoid circular imports
     """
     def __init__(self, function, lut_bitwidth, bitwidth, limits=None,
         observer=quantizers.DEFAULT_OBSERVERS['default']):
         super().__init__()
         if limits is None:
             limits = (None, None)
         self.limits = limits
         lim_obs = partial(quantizers.FixedRangeObserver, limits=limits,
             hard_maximum=True)
+        if CONFIG.ilut_requant:
+            self.requant = Requantize(lut_bitwidth, observer=lim_obs)
         self.shift_down = Requantize(lut_bitwidth, observer=lim_obs)
         self.shift_up = Requantize(bitwidth, observer=lim_obs)
         quantizers.share_observer(self.shift_up, self.shift_down)
         self.obs_in = self.shift_up.quantizer.observer
         self.add_one = VIAdd(0., lut_bitwidth)
         self.lut = BareLUT(function, bitwidth)
         self.rem_sub = VVSub(bitwidth)
@@ -90,14 +94,16 @@
         self.add = VVAdd(bitwidth)
 
         # Group all submodules into a single quantization group
         self.q_group = quantizers.PrecisionConstraint()
         self.q_group.recursively_add(self)
 
     def forward(self, x):
+        if CONFIG.ilut_requant:
+            x = self.requant(x)
         if x.quantized:
             bw = self.shift_down.quantizer.bitwidth.bitwidth
             q_addr = self.obs_in.calculate_quanta(bw)
             self.add_one.imm.data = 2.**(q_addr).detach()
             self.rem_muli.imm.data = 2.**(-q_addr).detach()
         addr = copy_dim_annotations(x, self.shift_down(x))
         addr_p = self.add_one(addr)
@@ -278,14 +284,29 @@
         rem = self.mul_alpha(rem)
         mixed_addr = self.mux_add(self.mux_mul0(addr, is_large), self.mux_mul1(rem, is_small))
         mixed_y = self.lut(mixed_addr)
         to_mul = self.add_multipliers(self.mul_falpha(self.is_small_shift(is_small)))
         unmixed_y = self.demixer(mixed_y, to_mul)
         return unmixed_y
 
+# class AddIdentityTILUT(nn.Module):
+#     """Telescoping & Interpolating Lookup Table, 
+#     for functions that satisfy 
+#     .. math::
+
+#         f(a * b) = f(a) * f(b)
+        
+#     for positive a and b"""
+#     def __init__(self, function, lut_bitwidth, bitwidth, limits=None,
+#                  observer=quantizers.DEFAULT_OBSERVERS['default']):
+#         super().__init__()
+#         self.tele = Shift(-8, bitwidth=bitwidth)
+#         self.gt0 = Gt0(bitwidth)
+
+
 class TILUT(nn.Module):
     """
     Telescoping & Interpolating Lookup Table
     """
     def __init__(self, function, lut_bitwidth, bitwidth, limits=None,
         observer=quantizers.DEFAULT_OBSERVERS['default']):
         super().__init__()
```

## fmot/qat/nn/quantizers.py

```diff
@@ -7,14 +7,15 @@
 from ._utils import intitem
 # from fmot.utils import reset_counters
 from torch import Tensor
 from typing import List, Tuple, Optional
 from torch.jit import Final
 import math
 from functools import partial
+from fmot.configure import CONFIG
 
 EPS = 2**-40
 
 class ObserverBase(nn.Module):
     """Base observer class to be subclassed to implement a particular observer.
 
     All Observers must subclass this base class
@@ -66,14 +67,19 @@
         Args:
             bits (int): bitwidth to be used once the observed tensor is quantized
 
         Returns:
             quanta (int): optimal quanta
         """
         raise NotImplementedError
+    
+    def do_on_fp(self, x):
+        """When quantize = False, this operation is performed to transform input x.
+        By default, x is not modified. Subclasses can overwrite this."""
+        return x
 
 class MinMaxObserver(ObserverBase):
     """MinMaxObserver stores a running minimum and maximum value
 
     The optimal quanta is chosen so that the quantization range barely
     fits the min/max observed activations.
 
@@ -121,14 +127,18 @@
 
         quanta_neg = torch.ceil(torch.log2(-min_val) + 1 - bits)
         quanta_pos = torch.ceil(torch.log2(max_val/(2**(bits-1)-1)))
         if verbose:
             print('qpos:', quanta_pos)
             print('qneg:', quanta_neg)
         quanta = torch.max(quanta_neg, quanta_pos)
+
+        if bits == 16:
+            quanta = quanta + CONFIG.minmax_headroom
+
         return quanta
 
 class MovingAverageMinMaxObserver(MinMaxObserver):
     """Takes an exponential moving average of min and max activation statistics
 
     The optimal quanta is chosen so that the quantization range barely fits the min/max moving
     averages.
@@ -213,14 +223,23 @@
         quanta_neg = torch.ceil(torch.log2(-min_val) + 1 - bits)
         if self.hard_maximum:
             quanta_pos = torch.ceil(torch.log2(max_val/(2**(bits-1)-1)))
         else:
             quanta_pos = torch.ceil(torch.log2(max_val) + 1 - bits)
         quanta = torch.max(quanta_neg, quanta_pos)
         return quanta
+    
+    def do_on_fp(self, x):
+        if CONFIG.sim_fixed_range_fp:
+            if (self.limits[0] is not None) or (self.limits[1] is not None):
+                return torch.clamp(x, *self.limits)
+            else:
+                return x
+        else:
+            return x
 
 class FixedRangeWrappedObserver(ObserverBase):
     """
     hard_maximum -> whether to use asymmetric range [-128, 127] when optimizing
     quanta, or to approximate this with [-128, 128].
     """
     def __init__(self, limits, wrapped, hard_maximum=True):
@@ -252,15 +271,23 @@
         if self.hard_maximum:
             quanta_pos = torch.ceil(torch.log2(vmax/(2**(bits-1)-1)))
         else:
             quanta_pos = torch.ceil(torch.log2(vmax) + 1 - bits)
 
         quanta = torch.max(quanta_neg, quanta_pos)
         return quanta
-
+    
+    def do_on_fp(self, x):
+        if CONFIG.sim_fixed_range_fp:
+            if (self.limits[0] is not None) or (self.limits[1] is not None):
+                return torch.clamp(x, *self.limits)
+            else:
+                return x
+        else:
+            return x
 class GaussianObserver(ObserverBase):
     """
     GaussianObserver fits a normal distribution to the observed tensor.
     Records a running mean and variance. The quanta is chosen to minimize
     the expected value of quantization mean squared error.
 
     Args:
@@ -396,18 +423,38 @@
 
     @staticmethod
     def gaussian_error(bits, quanta, mu, sigma):
         e_trunc = GaussianObserver.truncation_error(bits, quanta, mu, sigma)
         e_round = GaussianObserver.rounding_error(bits, quanta, mu, sigma)
         return e_trunc + e_round
 
-DEFAULT_OBSERVERS = {
-    'default': MinMaxObserver,
-    'param': MinMaxObserver
-}
+class DefObs:
+    def __getitem__(self, key):
+        if key == 'default':
+            return DefObs.get_obs(CONFIG.default_observer)
+        elif key == 'param':
+            return DefObs.get_obs(CONFIG.param_observer)
+        elif key == 'lstm':
+            return DefObs.get_obs(CONFIG.lstm_param_observer)
+        else:
+            raise KeyError(f'Default for {key} not defined')
+
+    @staticmethod
+    def get_obs(key):
+        if key == 'min_max':
+            return MinMaxObserver
+        elif key == 'gaussian':
+            return GaussianObserver
+        elif key == 'moving_min_max':
+            return MovingAverageMinMaxObserver
+        else:
+            raise KeyError(f'Observer {key} not defined')
+
+
+DEFAULT_OBSERVERS = DefObs()
 
 class Quantizer(nn.Module):
     """
     Attributes:
         param: parameter associated to the quantizer (we assume
         that we can only have one to one correspondance)
     """
@@ -426,20 +473,22 @@
 
     def forward(self, x):
         if self.observe:
             self.observer.update_statistics(x)
         quanta = None
         if self.quantize:
             quanta = self.observer.calculate_quanta(self.bitwidth.bitwidth)
+            self.prev_quanta = quanta
+
             if quanta is None:
                 raise ValueError(f'Quanta was None! {self.observer}')
             y = copy_dim_annotations(x, fake_quantize(x, quanta,
                 self.bitwidth.bitwidth, rounded=self.rounded))
         else:
-            y = x
+            y = self.observer.do_on_fp(x)
         try:
             dimensions = x.dimensions
         except:
             warnings.warn('Input dimensions are missing: ' +
                           'dimension information may not propagate correctly')
             dimensions = None
         y = annotate(y, self.bitwidth, quanta, self.quantize, dimensions=dimensions)
@@ -473,30 +522,29 @@
             if len(self.param) != 0:
                 self.param[0].bitwidth = self.bitwidth
 
     def assign_to_group(self, group):
         self.member_of.append(group)
 
 class ParameterQuantizer(Quantizer):
-    def __init__(self, bitwidth, observer=MinMaxObserver,
+    def __init__(self, bitwidth, observer=None,
         rounded=True, dimensions=None, **observer_kwargs):
-        # ignore observer -- always use GaussianObserver
-        # observer = GaussianObserver
+        if observer is None:
+            observer = DEFAULT_OBSERVERS['param']
         super().__init__(bitwidth, observer, rounded, dimensions)
         self.register_buffer('_cache', None)
         self._use_cache = False
         self.param = []
 
     @classmethod
     def _from_float(cls, parent, bw_conf, interpolate,
-        observer=DEFAULT_OBSERVERS['default'], **kwargs):
+        observer=DEFAULT_OBSERVERS['param'], **kwargs):
         observer = partial(observer, **kwargs)
         # TODO: can weights have more than 3 dimensions?
         if parent.is_weight:
-            observer = GaussianObserver
             bw = bw_conf.weights
             dimensions = ['F', 'F']
         else:
             bw = bw_conf.activations
             dimensions = ['F']
         return cls(bitwidth=bw, dimensions=dimensions, observer=observer)
 
@@ -506,15 +554,14 @@
                 y = super().forward(
                         set_dim_annotations(self.dimensions, x))
                 self.param = [y]
                 self.register_buffer('_cache', y)
             return self._cache
         else:
             y = super().forward(set_dim_annotations(self.dimensions, x))
-            #self.param = [y]
             return y
 
     def cache(self):
         self.register_buffer('_cache', None)
         self._use_cache = True
 
     def decache(self):
```

## fmot/sparse/act_pruning.py

```diff
@@ -28,15 +28,15 @@
         model (torch.nn.Module): a PyTorch model
 
     Returns:
         hooks: a list of PyTorch hook. Can be used to remove the hoooks from the model later on.
     """
     hooks = []
     for module in model.modules():
-        if isinstance(module, ThresholdSparsifier):
+        if isinstance(module, ThresholdSparsifier) or isinstance(module, torch.nn.ReLU):
             hooks.append(module.register_forward_hook(actsp_hook_fn))
 
     return hooks
 
 
 def remove_hooks(hooks):
     r"""
```

## fmot/test/test_dim_anno.py

```diff
@@ -68,27 +68,27 @@
         cmodel.quantize(inputs)
 
         x = torch.randn(batch_size, n_features, timesteps)
         output = cmodel(x)
 
         assert(output.dimensions == ['B', 'T', 'F'])
 
-    def test_4d_propag(self):
-        import torch
-        import fmot
-
-        model = torch.nn.Conv2d(1, 16, 2, 2)
-        x = torch.randn(1, 1, 96, 96)
-
-        # convert, quantize
-        named_dims = ['B', 'F', 'H', 'W']
-        cmodel = fmot.ConvertedModel(model, named_dims=named_dims)  # cannot tag dims yet...
-        cmodel.quantize([torch.randn(5, 1, 4, 4) for _ in range(2)])
-        y = cmodel(x)
-        assert y.dimensions == named_dims
+    # def test_4d_propag(self):
+    #     import torch
+    #     import fmot
+
+    #     model = torch.nn.Conv2d(1, 16, 2, 2)
+    #     x = torch.randn(1, 1, 96, 96)
+
+    #     # convert, quantize
+    #     named_dims = ['B', 'F', 'H', 'W']
+    #     cmodel = fmot.ConvertedModel(model, named_dims=named_dims)  # cannot tag dims yet...
+    #     cmodel.quantize([torch.randn(5, 1, 4, 4) for _ in range(2)])
+    #     y = cmodel(x)
+    #     assert y.dimensions == named_dims
 
     def test_torch_1_9(self):
         class Net(nn.Module):
                 def __init__(self):
                     super().__init__()
                     self.linears = nn.ModuleList([nn.Linear(4, 4), nn.Linear(4, 4)])
```

## fmot/test/test_features.py

```diff
@@ -302,73 +302,73 @@
             torch.nn.Linear(4, 2))
         inputs = [torch.randn(4, 4) for __ in range(10)]
         cmodel = ConvertedModel(model, precision='double', batch_dim=0,
                                 interpolate=False)
         cmodel.quantize(inputs)
         _ = generate_param2quantizer(cmodel, inputs[0])
 
-    def test_parameter_table(self):
-        model = torch.nn.Sequential(
-            torch.nn.ReLU(),
-            torch.nn.Linear(4, 2))
-        torch.manual_seed(0)
-        inputs = [torch.randn(4, 4) for __ in range(10)]
-        cmodel = ConvertedModel(model, precision='double', batch_dim=0,
-                                interpolate=False)
-
-        param_table = cmodel.get_parameter_table()
-        for name, _ in cmodel.named_parameters():
-            assert (param_table[name]['memory'] == 'N/A')
-        cmodel.quantize(inputs)
-        param_table = cmodel.get_parameter_table()
-        assert (param_table['model.model.1.weight']['memory'] == 8.)
-
-    def test_set_param_precision(self):
-        model = torch.nn.Sequential(
-            torch.nn.ReLU(),
-            torch.nn.Linear(4, 2))
-        inputs = [torch.randn(4, 4) for __ in range(10)]
-        cmodel = ConvertedModel(model, precision='double', batch_dim=0,
-                                interpolate=False)
-        cmodel.quantize(inputs)
-
-        cmodel.set_param_precision('model.model.1.weight', 'double')
-
-    def test_param2_quant_prunedmodel(self):
-        ''' Tests if param2quant is working as expected on
-            models for which a parameter has been pruned (as pruned
-            parameters are regenerated on-the-fly by PyTorch)
-        '''
-        model = torch.nn.Sequential(
-            torch.nn.ReLU(),
-            torch.nn.Linear(4, 2))
-        inputs = [torch.randn(4, 4) for __ in range(10)]
-        cmodel = ConvertedModel(model, precision='double', batch_dim=0,
-                                interpolate=False)
-        prune.l1_unstructured(cmodel.model.model[1], 'weight', 0.5)
-        cmodel.quantize(inputs)
-        cmodel.modify_precision('standard')
-        assert (str(cmodel.param2quant['model.model.1.weight'].bitwidth) == 'fqint4')
-
-    def test_logic_param2quant(self):
-        ''' Tests on a simple model if the Parameter to Quantizer
-            utilities are working as expected.
-        '''
-        torch.manual_seed(0)
-        model = torch.nn.Sequential(
-            torch.nn.ReLU(),
-            torch.nn.Linear(4, 2))
-        inputs = [torch.randn(4, 4) for __ in range(10)]
-        cmodel = ConvertedModel(model, precision='double', batch_dim=0,
-                                interpolate=False)
-        cmodel.quantize(inputs)
-        table = cmodel.get_parameter_table()
-        assert(table['model.model.1.weight']['density'] == 1.)
-        assert(table['model.model.1.weight']['memory'] == 8 * 8 / 8) # nb_param * bitwidth / 8
-        prune.l1_unstructured(cmodel.model.model[1], 'weight', 0.5)
-        table = cmodel.get_parameter_table()
-        assert(table['model.model.1.weight']['density'] == .5)
-        assert(table['model.model.1.weight']['memory'] == 4.0)
+    # def test_parameter_table(self):
+    #     model = torch.nn.Sequential(
+    #         torch.nn.ReLU(),
+    #         torch.nn.Linear(4, 2))
+    #     torch.manual_seed(0)
+    #     inputs = [torch.randn(4, 4) for __ in range(10)]
+    #     cmodel = ConvertedModel(model, precision='double', batch_dim=0,
+    #                             interpolate=False)
+
+    #     param_table = cmodel.get_parameter_table()
+    #     for name, _ in cmodel.named_parameters():
+    #         assert (param_table[name]['memory'] == 'N/A')
+    #     cmodel.quantize(inputs)
+    #     param_table = cmodel.get_parameter_table()
+    #     assert (param_table['model.model.1.weight']['memory'] == 8.)
+
+    # def test_set_param_precision(self):
+    #     model = torch.nn.Sequential(
+    #         torch.nn.ReLU(),
+    #         torch.nn.Linear(4, 2))
+    #     inputs = [torch.randn(4, 4) for __ in range(10)]
+    #     cmodel = ConvertedModel(model, precision='double', batch_dim=0,
+    #                             interpolate=False)
+    #     cmodel.quantize(inputs)
+
+    #     cmodel.set_param_precision('model.model.1.weight', 'double')
+
+    # def test_param2_quant_prunedmodel(self):
+    #     ''' Tests if param2quant is working as expected on
+    #         models for which a parameter has been pruned (as pruned
+    #         parameters are regenerated on-the-fly by PyTorch)
+    #     '''
+    #     model = torch.nn.Sequential(
+    #         torch.nn.ReLU(),
+    #         torch.nn.Linear(4, 2))
+    #     inputs = [torch.randn(4, 4) for __ in range(10)]
+    #     cmodel = ConvertedModel(model, precision='double', batch_dim=0,
+    #                             interpolate=False)
+    #     prune.l1_unstructured(cmodel.model.model[1], 'weight', 0.5)
+    #     cmodel.quantize(inputs)
+    #     cmodel.modify_precision('standard')
+    #     assert (str(cmodel.param2quant['model.model.1.weight'].bitwidth) == 'fqint4')
+
+    # def test_logic_param2quant(self):
+    #     ''' Tests on a simple model if the Parameter to Quantizer
+    #         utilities are working as expected.
+    #     '''
+    #     torch.manual_seed(0)
+    #     model = torch.nn.Sequential(
+    #         torch.nn.ReLU(),
+    #         torch.nn.Linear(4, 2))
+    #     inputs = [torch.randn(4, 4) for __ in range(10)]
+    #     cmodel = ConvertedModel(model, precision='double', batch_dim=0,
+    #                             interpolate=False)
+    #     cmodel.quantize(inputs)
+    #     table = cmodel.get_parameter_table()
+    #     assert(table['model.model.1.weight']['density'] == 1.)
+    #     assert(table['model.model.1.weight']['memory'] == 8 * 8 / 8) # nb_param * bitwidth / 8
+    #     prune.l1_unstructured(cmodel.model.model[1], 'weight', 0.5)
+    #     table = cmodel.get_parameter_table()
+    #     assert(table['model.model.1.weight']['density'] == .5)
+    #     assert(table['model.model.1.weight']['memory'] == 4.0)
 
 if __name__ == "__main__":
     test = TestFeatures()
     test.test_logic_param2quant()
```

## fmot/test/test_fft.py

```diff
@@ -1,13 +1,28 @@
 import torch
 from fmot.nn import FFT
 import fmot
 import sys
+import numpy as np
+import matplotlib.pyplot as plt
+from fmot.tracing.compare_fqir import run_fqir_autocompare
 sys.setrecursionlimit(10000)
 
 def test_fft():
-    model = FFT(512, 3, dft_parallelism=2,
-        twiddle_parallelism=2)
-    cmodel = fmot.ConvertedModel(model)
+    model = FFT(512, 1)
+    cmodel = fmot.ConvertedModel(model, observer='min_max')
     cmodel.quantize([torch.randn(8, 512) for _ in range(4)])
     graph = cmodel.trace()
-    assert True
+
+    x = torch.randn(1, 512)
+
+    re0, im0 = cmodel(x)
+    re0, im0 = map(lambda x: x.detach().numpy(), [re0, im0])
+    re1, im1 = graph.run(x.numpy(), dequant=True)
+
+    assert np.array_equal(re0, re1)
+    assert np.array_equal(im0, im1)
+
+    print(run_fqir_autocompare(cmodel, graph, [x]))
+
+if __name__ == '__main__':
+    test_fft()
```

## fmot/test/test_sequencers.py

```diff
@@ -7,14 +7,15 @@
 from fmot.nn.conv1d import TemporalConv1d, SequencedTemporalConv1d, DepthWiseTemporalConv1d
 from fmot.nn.conv1d import FmotConv1dWrapper
 from fmot.nn import rsetattr, map_param_name
 from fmot.nn import SuperBasic
 
 from fmot import ConvertedModel
 from fmot import qat as Q
+from fmot import CONFIG
 
 class TestSequencers():
     
     def test_cell_running(self):
         r""" This tests if the step methods for cell unit
              Sequncers are running, and if the shape is correct.
              This does not check if the logic structure is correct
@@ -114,52 +115,52 @@
                     #print(list(torch_rnn.named_parameters()))
                     for name, tensor in torch_net.named_parameters():
                         rsetattr(my_net, map_param_name(name), dict[name])
                     
                     output, h_list = my_net(x,[h for _ in range(num_layers)])
                     assert(torch.sum(torch.abs(torch_output-output)).item() < epsilon)
 
-    def test_unit_logic_lstm(self):
-        batch_size = 5
-        input_size = 3
-        hidden_size = 4
-        time_steps = 2
-        x = torch.randn(batch_size, time_steps, input_size)
-        h = torch.randn(batch_size, hidden_size)
-        c = torch.randn(batch_size, hidden_size)
-        torch.manual_seed(0)
-        
-        epsilon = 10e-6
-        # Check if LSTM logic is correct
-        num_layers_list = [1,3]
-        bias_list = [True, False]
+    # def test_unit_logic_lstm(self):
+    #     batch_size = 5
+    #     input_size = 3
+    #     hidden_size = 4
+    #     time_steps = 2
+    #     x = torch.randn(batch_size, time_steps, input_size)
+    #     h = torch.randn(batch_size, hidden_size)
+    #     c = torch.randn(batch_size, hidden_size)
+    #     torch.manual_seed(0)
+        
+    #     epsilon = 10e-6
+    #     # Check if LSTM logic is correct
+    #     num_layers_list = [1,3]
+    #     bias_list = [True, False]
 
-        for num_layers in num_layers_list:
-            for bias in bias_list:
-                for batch_first in [True, False]:
-                    if batch_first:
-                        x = torch.randn(batch_size, time_steps, input_size)
-                    else:
-                        x = torch.randn(time_steps, batch_size, input_size)
+    #     for num_layers in num_layers_list:
+    #         for bias in bias_list:
+    #             for batch_first in [True, False]:
+    #                 if batch_first:
+    #                     x = torch.randn(batch_size, time_steps, input_size)
+    #                 else:
+    #                     x = torch.randn(time_steps, batch_size, input_size)
                             
-                    torch_net = torch.nn.LSTM(input_size, hidden_size, num_layers = num_layers, bias=True, batch_first=batch_first)
-                    dict = {}       #we can store the weights in this dict for convenience
-                    for name, param in torch_net.named_parameters(): 
-                          nn.init.normal_(param)
-                          dict[name] = param
+    #                 torch_net = torch.nn.LSTM(input_size, hidden_size, num_layers = num_layers, bias=True, batch_first=batch_first)
+    #                 dict = {}       #we can store the weights in this dict for convenience
+    #                 for name, param in torch_net.named_parameters(): 
+    #                       nn.init.normal_(param)
+    #                       dict[name] = param
     
-                    torch_output, h_n = torch_net(x, (torch.cat([h.unsqueeze(0)]*num_layers,0), torch.cat([h.unsqueeze(0)]*num_layers,0)))
-                    torch_output = torch_output.squeeze(1)
-                    my_net = LSTM(input_size,hidden_size,num_layers,bias=True,batch_first=batch_first)
-                    #print(list(torch_rnn.named_parameters()))
-                    for name, tensor in torch_net.named_parameters():
-                        rsetattr(my_net, map_param_name(name), dict[name])
+    #                 torch_output, h_n = torch_net(x, (torch.cat([h.unsqueeze(0)]*num_layers,0), torch.cat([h.unsqueeze(0)]*num_layers,0)))
+    #                 torch_output = torch_output.squeeze(1)
+    #                 my_net = LSTM(input_size,hidden_size,num_layers,bias=True,batch_first=batch_first)
+    #                 #print(list(torch_rnn.named_parameters()))
+    #                 for name, tensor in torch_net.named_parameters():
+    #                     rsetattr(my_net, map_param_name(name), dict[name])
                     
-                    output, h_list = my_net(x,[h for _ in range(2*num_layers)])
-                    assert(torch.sum(torch.abs(torch_output-output)).item() < epsilon)
+    #                 output, h_list = my_net(x,[h for _ in range(2*num_layers)])
+    #                 assert(torch.sum(torch.abs(torch_output-output)).item() < epsilon)
                 
     def test_unit_logic_gru(self):
         batch_size = 5
         input_size = 3
         hidden_size = 4
         time_steps = 2
         x = torch.randn(batch_size, time_steps, input_size)
```

## fmot/test/utm/__init__.py

```diff
@@ -0,0 +1,10 @@
+00000000: 6672 6f6d 202e 726e 6e5f 7465 7374 5f6c  from .rnn_test_l
+00000010: 6962 7261 7279 2069 6d70 6f72 7420 726e  ibrary import rn
+00000020: 6e5f 6c69 6272 6172 790a 6672 6f6d 202e  n_library.from .
+00000030: 6665 6564 666f 7277 6172 645f 7465 7374  feedforward_test
+00000040: 5f6c 6962 7261 7279 2069 6d70 6f72 7420  _library import 
+00000050: 6665 6564 666f 7277 6172 645f 6c69 6272  feedforward_libr
+00000060: 6172 790a 6672 6f6d 202e 6174 6f6d 6963  ary.from .atomic
+00000070: 5f74 6573 745f 6c69 6272 6172 7920 696d  _test_library im
+00000080: 706f 7274 2061 746f 6d69 635f 6c69 6272  port atomic_libr
+00000090: 6172 79                                  ary
```

## fmot/test/utm/feedforward_test_library.py

```diff
@@ -1,10 +1,11 @@
 from .unittest_objects import UTM, TestSet, TestLibrary
 import torch
 from torch import nn
+import fmot
 from torch.nn import functional as F
 from itertools import product as iterprod
 import numpy as np
 
 feedforward_library = TestLibrary('ff')
 
 class LayerNormUTM(UTM):
@@ -139,8 +140,57 @@
         return ba, dc
 
     def _get_random_inputs(self, batch_size):
         return torch.randn(batch_size, self.Din), torch.randn(batch_size, self.Din)
 
 feedforward_library['reordering_cat_chunk'] = TestSet(
     utm=ReorderCatChunkUTM,
-    par_sets=[dict(Din=D) for D in [128, 256, 102, 384, 512, 768]])
+    par_sets=[dict(Din=D) for D in [128, 256, 102, 384, 512, 768]])
+
+class FFTUTM(UTM):
+    def __init__(self, nfft, stages):
+        super().__init__()
+        self.nfft = nfft
+        self.stages = stages
+        self.fft = fmot.nn.FFT(nfft, stages)
+
+    def forward(self, x):
+        return self.fft(x)
+    
+    def _get_random_inputs(self, batch_size):
+        return torch.randn(batch_size, self.nfft)
+    
+feedforward_library['fft'] = TestSet(
+    utm=FFTUTM,
+    par_sets=[dict(nfft=N, stages=S) for N, S in iterprod([256], [0, 1, 2, 3])])
+
+class FCStackReLU(UTM):
+    def __init__(self, Din, gain):
+        super().__init__()
+        self.Din = Din
+        self.gain = gain
+        self.lin0 = nn.Linear(Din, Din)
+        self.lin1 = nn.Linear(Din, Din)
+        self.relu = nn.ReLU()
+
+    def forward(self, x):
+        x = self.lin0(x)
+        x = self.relu(x)
+        x = self.lin1(x)
+        x = torch.sigmoid(x)
+        return x
+    
+    def _get_random_inputs(self, batch_size):
+        return torch.randn(batch_size, self.Din) * self.gain
+    
+feedforward_library['fc_stack_relu'] = TestSet(
+    utm=FCStackReLU,
+    par_sets=[dict(Din=D, gain=G) for D, G in iterprod([256], [32, 64, 128, 256])])
+
+class FCStackReLU6(FCStackReLU):
+    def __init__(self, Din, gain):
+        super().__init__(Din, gain)
+        self.relu = nn.ReLU6()
+    
+feedforward_library['fc_stack_relu6'] = TestSet(
+    utm=FCStackReLU6,
+    par_sets=[dict(Din=D, gain=G) for D, G in iterprod([256], [32, 64, 128, 256])])
```

## fmot/test/utm/quant_tolerances.py

```diff
@@ -1,14 +1,15 @@
 import yaml
 import fmot
 from pathlib import Path
 from fmot.test.utm.get_utms import ALL_UTMS
 from collections import defaultdict
 import tqdm
 from multiprocessing import Pool
+import numpy as np
 from typing import *
 
 TOL_PATH = Path(fmot.__file__).parent / 'test' / 'utm' / 'quantization_tolerance.yaml'
 
 def load_tolerances() -> dict:
     with open(TOL_PATH, 'r') as f:
         tolerances = yaml.safe_load(f)
@@ -88,20 +89,21 @@
                     new_tols[name] = curval
         write_tolerances(new_tols)
 
     elif mode == 'min':
         print('Setting new tolerances as the min of current and new tolerances')
         for name, newval in new_tols.items():
             curval = curr_tols.get(name, None)
+
             if curval is not None:
                 if (
                     newval < curval and 
                     (force or ask_to_continue(f'Lower tolerance of {name} from {curval:.3E} to {newval:.3E}?'))
                 ):
                     pass
                 else:
                     new_tols[name] = curval
         write_tolerances(new_tols)
                     
 
 if __name__ == '__main__':
-    set_tolerances('overwrite', 2, False)
+    set_tolerances('min', 2, False)
```

## fmot/test/utm/rnn_test_library.py

```diff
@@ -153,15 +153,15 @@
               iterprod([6], [32, 64], [32, 64], [1,2], [True, False])]
     )
 rnn_library['lstm'] = lstm_set
 
 class TemporalConv1dUTM(SUTM):
      def __init__(self, nb_timesteps, in_channels, out_channels, kernel_size,
           dilation, stride):
-          super().__init__(batch_dim=0, seq_dim=2)
+          super().__init__(batch_dim=0, seq_dim=2, skip_mixed=True)
           self.nb_timesteps = nb_timesteps
           self.in_channels = in_channels
           self.out_channels = out_channels
           self.kernel_size = kernel_size
           self.dilation = dilation
           self.stride = stride
           self.net = TemporalConv1d(
@@ -227,15 +227,15 @@
           H=H,
           Dout=Dout)
      for T, Din, H, Dout in
      iterprod([16], [64], [128], [64, 128])])
 
 class DWConv1dUTM(SUTM):
     def __init__(self, nb_timesteps, D, kernel_size):
-        super().__init__(batch_dim=0, seq_dim=2)
+        super().__init__(batch_dim=0, seq_dim=2, skip_mixed=True)
         self.nb_timesteps = nb_timesteps
         self.D = D
         self.kernel_size = kernel_size
         self.net = TemporalConv1d(
             in_channels=D,
             out_channels=D,
             groups=D,
@@ -250,15 +250,15 @@
 rnn_library['dw_conv1d'] = TestSet(
     utm=DWConv1dUTM,
     par_sets=[dict(nb_timesteps=T, D=D, kernel_size=K) 
         for T, D, K in iterprod([10], [32], [2,4,8])])
 
 class TCResNetUTM(SUTM):
     def __init__(self, nb_timesteps, input_size, model_fn):
-        super().__init__(batch_dim=0, seq_dim=2)
+        super().__init__(batch_dim=0, seq_dim=2, skip_mixed=True)
         self.nb_timesteps = nb_timesteps
         self.input_size = input_size
         self.net = model_fn(input_size=input_size)
 
     def forward(self, x):
         return self.net(x)
```

## fmot/test/utm/unittest_objects.py

```diff
@@ -6,14 +6,15 @@
 from torch import Tensor, nn
 from typing import List, Tuple, Optional
 import textwrap
 from functools import wraps
 from fmot.qat.annotated_tensors import asint
 from fmot.beta import optimize_mixed_precision
 import warnings
+import pytest
 
 ################################################
 # > Base UTM Class and Test Container Objects
 
 def eval_method(func):
     @wraps(func)
     def new_func(*args, **kwargs):
@@ -28,24 +29,27 @@
 
 class UTM(nn.Module):
     """Unit Test Module
 
     UTMs provide a method to reproducibly generate random inputs
     """
     def __init__(self, batch_dim=0, seq_dim=None, converted_rtol=5e-3,
-        quantized_rtol=1e-2, allow_fqir_offby=1):
+        converted_rms=1e-3, quantized_rtol=1e-2, allow_fqir_offby=1,
+        skip_mixed=False):
         super().__init__()
         self.seed = 0
         self.bw_conf = None
         self.interpolate = None
         self.batch_dim = batch_dim
         self.seq_dim = seq_dim
         self.converted_rtol = converted_rtol
+        self.converted_rms = converted_rms
         self.allow_fqir_offby = allow_fqir_offby
         self.quantized_rtol = quantized_rtol
+        self.skip_mixed = skip_mixed
 
     def get_random_inputs(self, batch_size):
         """Returns a random batch of inputs to the model, incrementing the random seed
 
         UTMs provide reproducible inputs. For the same sequence of get_random_inputs calls,
         the same sequence of inputs will be returned.
 
@@ -159,15 +163,18 @@
         cmodel = self.get_converted_model(bw_conf=bw_conf, interpolate=interpolate)
         x = self.get_random_inputs(B_test)
         y0 = self(*x)
         y1 = cmodel(*x)
         if not (isinstance(y0, tuple) or isinstance(y0, list)):
             y0, y1 = [y0], [y1]
         for yy0, yy1 in zip(y0, y1):
-            np.testing.assert_allclose(yy0.numpy(), yy1.numpy(), rtol=self.converted_rtol)
+            rmse = (yy0 - yy1).square().mean().sqrt() / yy0.square().mean().sqrt()
+            assert rmse < self.converted_rms, f'Normalized RMS error {rmse:.3E} above tolerance {self.converted_rms}'
+
+            # np.testing.assert_allclose(yy0.numpy(), yy1.numpy(), rtol=self.converted_rtol)
 
     @torch.no_grad()
     def get_quantization_nrmse(self, B_test=8, B_quant=8, N_quant=10, bw_conf='double', 
             interpolate=True):
         self.reset_seed()
         qmodel = self.get_quantized_model(B_quant, N_quant, bw_conf, interpolate)
 
@@ -187,15 +194,15 @@
     @torch.no_grad()
     def test_quantization_error(self, tolerance: float,
             B_test=8, B_quant=8, N_quant=10, bw_conf='double', 
             interpolate=True):
         error = self.get_quantization_nrmse(B_test, B_quant, N_quant, bw_conf, interpolate)
 
         if error > tolerance:
-            raise RuntimeError(f'Quant-Error {error} above tolerances: {tolerance}')
+            raise RuntimeError(f'Quant-Error {error:.3E} above tolerances: {tolerance:.3E}')
 
     @staticmethod
     def _test_fqir_runtime(model, graph, x, remove_batchdim=0, offby=0):
         y_torch = model(*x)
         if isinstance(y_torch, torch.Tensor):
             y_torch = [y_torch]
         xq = tuple([xx.numpy() for xx in x])
@@ -228,14 +235,18 @@
         x = self.get_random_inputs(B_test)
         UTM._test_fqir_runtime(qmodel, graph, x, remove_batchdim=remove_batchdim, 
             offby=self.allow_fqir_offby)
 
     @torch.no_grad()
     def test_mixed_precision_fqir_runtime(self, B_test=8, B_quant=8, N_quant=10,
         eta=0.3, remove_batchdim=0):
+
+        if self.skip_mixed:
+            pytest.skip('Skipping mixed-precision testing')
+
         self.reset_seed()
         qmodel = self.get_mixed_precision_model(
             eta=eta, B_quant=B_quant, N_quant=N_quant)
         graph = qmodel.trace()
         self.reset_seed()
         x = self.get_random_inputs(B_test)
         UTM._test_fqir_runtime(qmodel, graph, x, remove_batchdim=remove_batchdim,
@@ -243,17 +254,16 @@
 
 class SUTM(UTM):
     """Sequencer Unit Test Module
 
     A subclass of UTM for modules containing sequencers
     """
     def __init__(self, batch_dim=0, seq_dim=1, input_size=None, nb_timesteps=None, 
-        converted_rtol=5e-3, allow_fqir_offby=1):
-        super().__init__(batch_dim=batch_dim, seq_dim=seq_dim, 
-            converted_rtol=converted_rtol, allow_fqir_offby=allow_fqir_offby)
+        **kwargs):
+        super().__init__(batch_dim=batch_dim, seq_dim=seq_dim, **kwargs)
         self.input_size = input_size
         self.nb_timesteps = nb_timesteps
 
     def forward(self, x):
         # We assume state to be None to avoid KeyError: 'aten::__is__'
         # Rk: We could make SUTM super structures
         assert(hasattr(self, 'net'))
```

## fmot/tracing/oplinks_v1.py

```diff
@@ -21,19 +21,15 @@
     Q.nn.BareCat:           registry_v1['cat'],
     Q.nn.Stack:             registry_v1['stack'],
     Q.nn.Sum:               registry_v1['sum'],
     Q.nn.OnesLike:          registry_v1['constant_like'],
     Q.nn.Shift:             registry_v1['shift'],
     Q.nn.Requantize:        registry_v1['shift'],
     Q.nn.Gt0:               registry_v1['gt0'],
-    Q.nn.FConv1d:           registry_v1['conv1d'],
-    Q.nn.AvgPool1d:         registry_v1['avgpool1d'],
-    Q.nn.MaxPool1d:         registry_v1['maxpool1d'],
-    Q.nn.FConv2d:           registry_v1['conv2d'],
     Q.nn.Squeeze:           registry_v1['squeeze'],
-    Q.nn.AdaptiveAvgPool2d: registry_v1['adaptive_avg_pool2d'],
+    Q.nn.TemporalUnfold1d:  registry_v1['temporal_unfold_unkernelized'],
     Q.nn.LSTM:              registry_v1['lstm']
 }
 
 lut_ops = [Q.nn.LUT, Q.nn.RSqrtPlusEps, Q.nn.PowFrac, Q.nn.BareLUT]
 for op in lut_ops:
     oplinks_v1[op] =    registry_v1['lut']
```

## fmot/tracing/tracing.py

```diff
@@ -12,14 +12,15 @@
 import fmot.qat as Q
 from fmot.qat.annotated_tensors import copy_annotations
 from fmot.nn.conv1d import Conv1dReshaper
 from fmot.tracing.tracing_blacklist import TRACING_BLACKLIST
 from fmot.tracing.oplinks_v1 import oplinks_v1
 from fmot.nn.sequencer import unbind as seq_unbind
 from fmot.nn.sequencer import stack as seq_stack
+from typing import *
 
 logger = logging.getLogger(__name__)
 
 def dimension_index(dim, dims):
     """Extract the index of dim in dims list
 
     Raises:
@@ -42,18 +43,18 @@
             sequential model
     Returns:
         :class:`fqir.GraphProto`: An FQIR graph representation of the model
     """
     if seq_dim is not None:
         if batch_dim is None:
             batch_dim = 0
-        graph = trace_sequential_model(model, *inputs, batch_dim=batch_dim, seq_dim=seq_dim)
+        graph, tsrc_dict = trace_sequential_model(model, *inputs, batch_dim=batch_dim, seq_dim=seq_dim)
     else:
-        graph = trace_feedforward_model(model, *inputs, batch_dim=batch_dim)
-    return graph
+        graph, tsrc_dict = trace_feedforward_model(model, *inputs, batch_dim=batch_dim)
+    return graph, tsrc_dict
 
 COUNT = 0
 
 def get_count():
     global COUNT
     COUNT += 1
     return COUNT
@@ -101,38 +102,42 @@
         if not hasattr(xin, 'proto'):
             xin.proto = TensorProto.from_tensor(xout, f'%p.{get_count()}',
                 store_value=True)
             graph.add_parameter(xin.proto)
         xout.proto = xin.proto
     return module.register_forward_hook(hook_fn)
 
-def register_node(module, graph):
+def register_node(module, graph, tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]]=None):
     """Register a forward hook to add a node to the computational graph if the node is a leaf"""
     hname = get_hierarchical_name(module)
+    module.traced = False
     def hook_fn(module, xin, xout):
         # Get flat list of inputs and outputs
         xin_c = combine_iterators(xin, types=torch.Tensor)
         xout_c = combine_iterators(xout, types=torch.Tensor)
         if not allhaveprotos(xin_c):
             raise ValueError('Inputs to self.{} were not annotated'.format(hname))
 
         # Add a node to the graph if any of the outputs are not annotated with
         # a proto (this indicates that we've reached a leaf module)
         if not allhaveprotos(xout_c):
+            module.traced = True
 
             # Get constants for the node
             if hasattr(module, '_get_constants'):
                 constants = module._get_constants(*xin)
             else:
                 constants = {}
 
             # Create TensorProtos for all of the outputs
-            for x in xout_c:
+            for idx, x in enumerate(xout_c):
                 if not hasattr(x, 'proto'):
                     x.proto = TensorProto.from_tensor(x, f'%x.{get_count()}')
+                    if tsrc_dict is not None:
+                        tsrc_dict[x.proto.name] = (module, idx)
 
             # Get source code reference
             sourceref = ''
             if hasattr(module, '_sourceref'):
                 sourceref = module._sourceref
 
             # Construct an input operand dictionary
@@ -298,33 +303,36 @@
     graph = GraphProto(name='MAIN')
     # Register inputs and outputs
     dequant_graph = GraphProto(name='DEQUANT')
     handles = [register_inputs_immediately(model, graph), \
         register_outputs(model, graph, dequant_graph=dequant_graph),
         attach_subgraph(model, graph, dequant_graph, 'DEQUANT',
             register_inputs=False, register_outputs=False)]
+    
+    # construct a tensor-source-dict for tracing
+    tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]] = {}
 
     # Create a quant/dequant subgraphs if the root node is a QuantWrapper
     if isinstance(model, Q.nn.QuantWrapper):
         # Create and attach a quant subgraph
         qgraph = GraphProto(name='QUANT')
         handles += [attach_subgraph(model.quantizers, graph, qgraph, 'QUANT')]
         # Register quantizers as nodes
-        handles += [register_node(m, qgraph) for m in model.quantizers.quantizers]
+        handles += [register_node(m, qgraph, tsrc_dict) for m in model.quantizers.quantizers]
 
         amodel = model.model
     else:
         amodel = model
     # Create and attach subgraph for arithmetic operations
     agraph = GraphProto(name='ARITH')
     handles += [attach_subgraph(amodel, graph, agraph, 'ARITH')]
     # Register non-blacklisted arithmetic modules and parameters
     for m in list(amodel.modules()) + [amodel]:
         if type(m) not in TRACING_BLACKLIST:
-            handles += [register_node(m, agraph)]
+            handles += [register_node(m, agraph, tsrc_dict)]
         if isinstance(m, Q.nn.ParameterQuantizer):
             handles += [register_param(m, agraph)]
 
     ################################################
     # > CONSTRUCT GRAPH -- just call on test input
     if not(hasattr(inputs[0], 'dimensions')):
         input_dimensions = ['F', 'F', 'F']
@@ -344,15 +352,15 @@
     reset_count()
     clean_params(model)
 
     if remove_batchdim:
         graph = passes.remove_batchdim(graph, dim=batch_dim)
 
     passes.run_passes(graph)
-    return graph
+    return graph, tsrc_dict
 
 def prep_model_for_streaming(model, xin):
     """Set model into streaming mode"""
     for module in [model] + list(model.modules()):
         if isinstance(module, fmot.nn.Sequencer):
             # module.state = module.get_init_state(xin)
             module._streaming = True
@@ -381,14 +389,18 @@
     # > SET RULES FOR GRAPH CONSTRUCTION
     main = GraphProto(name='MAIN')
     init = GraphProto(name='INIT')
     quant = GraphProto(name='QUANT')
     dequant = GraphProto(name='DEQUANT')
     arith = GraphProto(name='ARITH')
 
+    ##########
+    # > Construct a tensor-source dictionary for debugging
+    tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]] = {}
+
     ### MAIN LEVEL
 
     # Register inputs and outputs to MAIN
     handles = []
     handles += [register_inputs_immediately(model, main)]
     handles += [register_outputs(model, main, dequant_graph=dequant)]
 
@@ -405,22 +417,22 @@
     for m in model.modules():
         if isinstance(m, Q.nn.StateInitializer):
             handles += [register_zeros_init(m, init)]
 
     ### LOOP LEVEL
     # QUANT
     handles += [attach_subgraph(model.quantizers, main, quant, 'QUANT')]
-    handles += [register_node(m, quant) for m in model.quantizers.quantizers]
+    handles += [register_node(m, quant, tsrc_dict) for m in model.quantizers.quantizers]
 
     # ARITH
     amodel = model.model
     handles += [attach_subgraph(amodel, main, arith, 'ARITH')]
     for m in amodel.modules():
         if type(m) not in TRACING_BLACKLIST:
-            handles += [register_node(m, arith)]
+            handles += [register_node(m, arith, tsrc_dict)]
         if isinstance(m, fmot.nn.Sequencer):
             handles += [register_state_assign(m, arith)]
         if isinstance(m, Q.nn.ParameterQuantizer):
             handles += [register_param(m, arith)]
 
     ### IN and OUT dimensions
     input_dimensions = ['F', 'F', 'F']
@@ -466,50 +478,52 @@
 
     if batch_dim == 0 and seq_dim == 1:
         main.unbind_dim = 0
     elif batch_dim == 1 and seq_dim == 0:
         main.unbind_dim = 0
     elif seq_dim in (2, -1):
         main.unbind_dim = -1
-    return main
+    return main, tsrc_dict
 
 def prepare_for_tracing(model, x, main_graph):
     for submodule in model.modules():
         if isinstance(submodule, Conv1dReshaper):
             x = submodule.forward(x)
             submodule.tracing_mode = True
             main_graph.register_reshaper(submodule.to_numpy())
         if isinstance(submodule, Q.nn.atomics.FTranspose):
             submodule.tracing_mode = True
     return x
 
-def hook_mixed(model, graph, init_graph):
+def hook_mixed(model, graph, init_graph, tsrc_dict=None):
     handles = []
-    _hook_ff(model, graph, init_graph, handles)
+    _hook_ff(model, graph, init_graph, handles, tsrc_dict)
     return handles
 
-def _hook_ff(module, graph, init_graph, handles):
+def _hook_ff(module, graph, init_graph, handles, 
+             tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]]=None):
     for m in module.children():
         if isinstance(m, fmot.nn.Sequencer):
-            handles += _hook_seq(m, graph, init_graph)
+            handles += _hook_seq(m, graph, init_graph, tsrc_dict)
         elif type(m) not in TRACING_BLACKLIST:
-            handles += [register_node(m, graph)]
+            handles += [register_node(m, graph, tsrc_dict)]
             _hook_ff(m, graph, init_graph, handles)
         if isinstance(m, Q.nn.ParameterQuantizer):
             handles += [register_param(m, graph)]
 
-def _hook_seq(module, graph, init_graph):
+def _hook_seq(module, graph, init_graph, 
+              tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]]=None):
     assert isinstance(module, fmot.nn.Sequencer)
 
     internal_handles = []
     external_handles = []
 
     for m in module.modules():
         if m != module and type(m) not in TRACING_BLACKLIST:
-            internal_handles += [register_node(m,register_node(m, graph))]
+            internal_handles += [register_node(m, register_node(m, graph, tsrc_dict), tsrc_dict)]
         elif isinstance(m, Q.nn.StateInitializer):
             internal_handles += [register_zeros_init(m, init_graph)]
         elif isinstance(m, Q.nn.ParameterQuantizer):
             internal_handles += [register_param(m, graph)]
     internal_handles += [register_state_assign(module, graph)]
 
     def seq_prehook_fn(seq, xin):
@@ -571,14 +585,16 @@
     # > SET RULES FOR GRAPH CONSTRUCTION
     main = GraphProto(name='MAIN')
     init = GraphProto(name='INIT')
     quant = GraphProto(name='QUANT')
     dequant = GraphProto(name='DEQUANT')
     arith = GraphProto(name='ARITH')
 
+    tsrc_dict: Dict[str, Tuple[torch.nn.Module, int]] = {}
+
     ### MAIN LEVEL
 
     # Register inputs and outputs to MAIN
     handles = []
     handles += [register_inputs_immediately(model, main)]
     handles += [register_outputs(model, main, dequant_graph=dequant)]
 
@@ -589,20 +605,20 @@
     # Attach dequant to MAIN
     handles += [attach_subgraph(model, main, dequant, 'DEQUANT',
             register_inputs=False, register_outputs=False)]
 
     ### LOOP LEVEL
     # QUANT
     handles += [attach_subgraph(model.quantizers, main, quant, 'QUANT')]
-    handles += [register_node(m, quant) for m in model.quantizers.quantizers]
+    handles += [register_node(m, quant, tsrc_dict) for m in model.quantizers.quantizers]
 
     # ARITH
     amodel = model.model
     handles += [attach_subgraph(amodel, main, arith, 'ARITH')]
-    handles += hook_mixed(amodel, arith, init)
+    handles += hook_mixed(amodel, arith, init, tsrc_dict)
 
     ### IN and OUT dimensions
     if named_dims is not None:
         input_dimensions = named_dims
     else:
         if seq_dim is not None:
             input_dimensions = ['F', 'F', 'F']
```

## fmot/tracing/tracing_blacklist.py

```diff
@@ -9,9 +9,10 @@
     Q.nn.Quantizer,
     Q.nn.StateQuantizer,
     Q.nn.MinMaxObserver,
     Q.nn.ParameterQuantizer,
     Q.nn.FixedRangeObserver,
     Q.nn.StateInitializer,
     torch.nn.ModuleDict,
-    torch.nn.LSTM
+    torch.nn.LSTM,
+    torch.nn.Unfold
 ]
```

## fmot/utils/saturation_opt.py

```diff
@@ -29,18 +29,22 @@
     fmot.qat.nn.BareCat,
     fmot.qat.nn.Stack,
     fmot.qat.nn.Sum,
     fmot.qat.nn.OnesLike,
     fmot.qat.nn.Shift,
     fmot.qat.nn.Requantize,
     fmot.qat.nn.Gt0,
-    fmot.qat.nn.LUT,
+    fmot.qat.nn.Linear,
+    fmot.qat.nn.AffineLinear,
+    fmot.qat.nn.PerChannelAffineLinear,
+    fmot.qat.nn.ILUT,
     fmot.qat.nn.RSqrtPlusEps,
     fmot.qat.nn.PowFrac,
-    fmot.qat.nn.BareLUT
+    fmot.qat.nn.BareLUT,
+    fmot.qat.nn.Requantize
 ]
 
 # All atomic modules that pass a fixed domain to their predecessors.
 # No multiply or LUT atomics.
 FR_ATOMICS = [
     fmot.qat.nn.VVAdd,
     fmot.qat.nn.VIAdd,
@@ -89,14 +93,21 @@
             return outputs
         else:
             for o in outputs:
                 o.node = module
             return outputs
     return module.register_forward_hook(hook_fn)
 
+def _attach_handles(module: torch.nn.Module, G, handles):
+    if type(module) in ATOMICS:
+        handles.append(hook_layer(module, G))
+    else:
+        for submodule in module.children():
+            _attach_handles(submodule, G, handles)
+
 def trace_graph(model, x):
     """
     Trace an nx.DiGraph with input x. Graph is not guaranteed to be perfect
     (i.e. not good enough to use as a program), but will be good enough
     to recursively backtrack to apply fixed-range observers to the model.
 
     Args:
@@ -105,168 +116,93 @@
 
     Returns:
         - Graph (nx.DiGraph). Nodes are atomic modules, and directed edges denote
             data dependencies
     """
     G = nx.DiGraph()
     handles = []
-    for module in model.modules():
-        if type(module) in ATOMICS:
-            handles.append(hook_layer(module, G))
+    _attach_handles(model, G, handles)
     if isinstance(x, tuple):
         __ = model(*x)
     else:
         __ = model(x)
     for h in handles:
         h.remove()
     return G
 
-def get_vvmul_preds(graph, node, recurse=True):
-    parents = list(graph.predecessors(node))
-    if len(parents) != 2:
-        return []
-
-    lut_parents = [p for p in parents if isinstance(p, fmot.qat.nn.LUT)]
-    nonlut_parents = [p for p in parents if p not in lut_parents]
-    if len(lut_parents) != 1:
-        return []
-
-    lut_parent = lut_parents[0]
-    nonlut_parent = nonlut_parents[0]
-    if lut_parent.function not in [torch.sigmoid, torch.tanh]:
-        return []
-
-    preds = [nonlut_parent]
-    if recurse:
-        preds += get_fixed_range_preds(graph, nonlut_parent, recurse=True,
-            use_vvmul=True)
-    return preds
-
-
-def get_fixed_range_preds(graph, node, recurse=True, use_vvmul=False):
-    """
-    Returns a list of predecessors for a given node in the graph. If 
-    :attr:`recurse=True`, will recursively add predecessors of predecessors,
-    but only recursing through layers in :attr:`FR_ATOMICS` (the set of nodes
-    that passes fixed domains to parents).
-
-    Args:
-        graph (nx.DiGraph): DiGraph representation of the model (i.e. from
-            :attr:`trace_graph()`)
-        node (torch.nn.Module): The node, whose predecessors we want
-        recurse (bool): Whether to recurse, default is :attr:`True`
-    Returns:
-        - Predecessors (list[torch.nn.Module]): A list of all the predecessor
-            nodes
-    """
-    assert node in graph.nodes
-    preds = []
-    for n in graph.predecessors(node):
-        preds.append(n)
-        if recurse:
-            if type(n) in FR_ATOMICS:
-                preds += get_fixed_range_preds(graph, n, recurse=True)
-            elif isinstance(n, fmot.qat.nn.VVMul) and use_vvmul:
-                preds += get_vvmul_preds(graph, n, recurse=True)
-    return preds
-
-def build_limits_dict(graph, use_vvmul=False):
-    """
-    For each LUT layer, recursively backtrack to find candidate limits for
-    predecessor nodes in the graph. Each predecessor node will have one or more
-    candidate limits (more than one if it is predecessor to more than one LUT).
-
-    Args:
-        graph (nx.DiGraph): A directed acyclic graph, output by :attr:`trace_graph()`
-    Returns:
-        A dictionary, connecting predecessor nodes to a list of candidate limits.
-    """
-    candidates = defaultdict(list)
-    for node in graph.nodes:
-        if isinstance(node, fmot.qat.nn.LUT):
-            limits = node.limits
-            preds = get_fixed_range_preds(graph, node, recurse=True,
-                use_vvmul=use_vvmul)
-            for p in preds:
-                candidates[p].append(limits)
-    return candidates
+def find_lin_requant(graph):
+    n = 0
+    for node in graph:
+        if isinstance(node, (fmot.qat.nn.Matmul, fmot.qat.nn.AddMM)):
+            succs = list(graph.successors(node))
+            if len(succs) == 1 and isinstance(succs[0], (fmot.qat.nn.Requantize, fmot.qat.nn.ILUT)):
+                nxt = succs[0]
+                if isinstance(nxt, fmot.qat.nn.ILUT):
+                    requant = nxt.shift_down
+                else:
+                    requant = nxt
+                obs = requant.quantizer.observer
+                if isinstance(obs, fmot.qat.nn.FixedRangeObserver):
+                    old_obs = node.quantizer.observer
+                    node.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=obs.limits, wrapped=old_obs)
+                    n += 1
+        elif isinstance(node, fmot.qat.nn.AffineLinear):
+            succs = list(graph.successors(node))
+            if len(succs) == 1 and isinstance(succs[0], (fmot.qat.nn.Requantize, fmot.qat.nn.ILUT)):
+                nxt = succs[0]
+                if isinstance(nxt, fmot.qat.nn.ILUT):
+                    requant = nxt.shift_down
+                else:
+                    requant = nxt
+                obs = requant.quantizer.observer
+                if isinstance(obs, fmot.qat.nn.FixedRangeObserver):
+                    limits = obs.limits
+                    wide_limits = tuple(map(lambda x: 2*x if x is not None else None, limits))
+                    old_obs = node.multiplier.quantizer.observer
+                    # node.multiplier.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=wide_limits, wrapped=old_obs)
+                    n += 1
+
+                    old_obs = node.vimul.quantizer.observer
+                    node.vimul.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=limits, wrapped=old_obs)
+                    n += 1
+        elif isinstance(node, fmot.qat.nn.PerChannelAffineLinear):
+            succs = list(graph.successors(node))
+            if len(succs) == 1 and isinstance(succs[0], (fmot.qat.nn.Requantize, fmot.qat.nn.ILUT)):
+                nxt = succs[0]
+                if isinstance(nxt, fmot.qat.nn.ILUT):
+                    requant = nxt.shift_down
+                else:
+                    requant = nxt
+                obs = requant.quantizer.observer
+                if isinstance(obs, fmot.qat.nn.FixedRangeObserver):
+                    limits = obs.limits
+                    wide_limits = tuple(map(lambda x: 2*x if x is not None else None, limits))
+                    old_obs = node.multiplier.quantizer.observer
+                    # node.multiplier.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=wide_limits, wrapped=old_obs)
+                    n += 1
+
+                    old_obs = node.renorm.quantizer.observer
+                    node.renorm.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=limits, wrapped=old_obs)
+                    n += 1
+        elif isinstance(node, fmot.qat.nn.Linear):
+            succs = list(graph.successors(node))
+            if len(succs) == 1 and isinstance(succs[0], (fmot.qat.nn.Requantize, fmot.qat.nn.ILUT)):
+                nxt = succs[0]
+                if isinstance(nxt, fmot.qat.nn.ILUT):
+                    requant = nxt.shift_down
+                else:
+                    requant = nxt
+                obs = requant.quantizer.observer
+                if isinstance(obs, fmot.qat.nn.FixedRangeObserver):
+                    old_obs = node.multiplier.quantizer.observer
+                    node.multiplier.quantizer.observer = fmot.qat.nn.FixedRangeWrappedObserver(limits=obs.limits, wrapped=old_obs)
+                    n += 1
+    return n
 
-def arbitrate_limits(candidates):
-    """
-    Finds largest limits among all candidates. If all candidates are 
-    (None, None), will return (None, None)
-
-    Args:
-        candidates (list[tuple]): List of (min, max) limit candidates
-    Returns:
-        limits, a (min, max) tuple. 
-    """
-    l0, l1 = (None, None)
-    for (c0, c1) in candidates:
-        if l0 is None:
-            l0 = c0
-        elif c0 < l0:
-            l0 = c0
-        
-        if l1 is None:
-            l1 = c1
-        elif c1 > l1:
-            l1 = c1
-    return (l0, l1)
-
-def rsetattr(obj, attr, val):
-    pre, _, post = attr.rpartition('.')
-    return setattr(rgetattr(obj, pre) if pre else obj, post, val)
-
-def rgetattr(obj, attr, *args):
-    if attr == '':
-        return obj
-    def _getattr(obj, attr):
-        return getattr(obj, attr, *args)
-    return functools.reduce(_getattr, [obj] + attr.split('.'))
-
-def apply_fixed_ranges(limits_dict, scaling=1., verbose=False):
-    """
-    Apply :attr:`FixedRangeWrappedObserver` layers to all of the predecessor layers.
-
-    For each :attr:`layer: [candidate_limits]` pair in the limits dictionary,
-    arbitrate to find an optimal limits tuple. This limits tuple is used to apply
-    a :attr:`FixedRangeWrappedObserver` to the layer's quantizer/observer.
-
-    The observers are updated in-place, so this function has no returned value.
-
-    Args:
-        limits_dict (dict): A dictionary of :attr:`layer: limits[]` pairs, as
-            output from :attr:`build_limits_dict()`
-        scaling (float): A scaling factor to increase headroom above the saturating
-            range. Should be >= 1, default is :attr:`1`.
-        verbose (bool): If :attr:`True`, will print out details each time an
-            observer is wrapped.
-    """
-    for layer, candidates in limits_dict.items():
-        limits = arbitrate_limits(candidates)
-        if limits != (None, None):
-            # rescale limits
-            l0, l1 = limits
-            if l0 is not None:
-                l0 *= scaling
-            if l1 is not None:
-                l1 *= scaling
-            limits = (l0, l1)
-            # replace observers with fixed-range
-            for name, module in layer.named_modules():
-                if isinstance(module, fmot.qat.nn.ObserverBase):
-                    new_obs = fmot.qat.nn.FixedRangeWrappedObserver(
-                        limits, module, hard_maximum=False)
-                    rsetattr(layer, name, new_obs)
-                    if verbose:
-                        print(f'Applied limits {limits} to {layer}')
-
-def insert_fixed_range_observers(model, x, scaling=1, in_place=True, 
-    verbose=False, use_vvmul=True):
+def insert_fixed_range_observers(model, x):
     """
     Recurse backwards from each saturating nonlinearity to apply fixed-range
     observers to predecessor layers. This restricts dynamic range prior to 
     saturating nonlinearities like sigmoid and tanh, to make the most of 
     dynamic range once the model is quantized.
 
     Args:
@@ -278,18 +214,14 @@
         in_place (bool): Whether to modify the model in-place or to modify a replica.
             Default is False.
         verbose (bool): Print out details about the insertion of 
             :attr:`FixedRangeWrappedObserver` layers.
         use_vvmul (bool): If True, passes fixed range through VVMUL if one of the
             operands is the output of a sigmoid or tanh nonlinearity. Default True.
     """
-    if not in_place:
-        raise NotImplementedError('non-in-place conversion not yet implemented')
     graph = trace_graph(model, x)
-    limits = build_limits_dict(graph, use_vvmul=use_vvmul)
-    apply_fixed_ranges(limits, scaling=scaling, verbose=verbose)
-
+    return find_lin_requant(graph) > 0
```

## fmot/utils/quant_tools/diagnosis.py

```diff
@@ -1,34 +1,39 @@
 import matplotlib.pyplot as plt
+from mpl_toolkits.axes_grid1 import make_axes_locatable
+from mpl_toolkits.axes_grid1 import ImageGrid
 import numpy as np
 import datashader as ds
+from datashader.mpl_ext import dsshow, alpha_colormap
 import pandas as pd
 import colorcet as cc
 from torch import nn
 
 
-def get_diagnosis(model, cmodel, sample_input, to_register=None, kind='output', plot: bool=True):
+def get_diagnosis(model, cmodel, sample_input, to_register=None, kind='output', plot: bool=True,
+                  how='log'):
     ''' Prints a diagnosis for all layers of the model, comparing the activations
         for the torch model and for the ConvertedModel, for a given sample_input.
 
     Args:
         model (torch.nn.Module): a PyTorch Model
         cmodel (fmot.ConvertedModel): its converted/quantized equivalent
         sample_input (torch.Tensor): sample input on which the comparison is carried out
         to_register (set(str)): if None, the comparison will be carried out on all layers.
             If a set of strings is used, the comparison will only be carried out on the
             layer with these names.
         kind (str): 'output' or 'input', so that the comparison will be carried out on outputs
             or inputs of the layers respectively.
         plot (bool): default True, determines whether a plot will be generated for each layer
+        how (str): default True. Can be 'log' or 'linear'. Defines the kind of scale that is used for color-mapping.
     '''
     acts = get_activations(model, sample_input, to_register, kind=kind)
     qacts = get_activations(cmodel, sample_input, to_register=set(acts.keys()), kind=kind)
     if plot:
-        plot_acts(model, acts, qacts, kind=kind)
+        plot_acts(model, acts, qacts, kind=kind, how=how)
 
 
 def act_hook_fn(name: str, activations: dict, kind='output'):
     if kind == 'output':
         def reg_act(model, input, output):
             if type(output) in {tuple, list}:
                 activations[name] = output[0].detach()
@@ -74,28 +79,29 @@
         handle.remove()
 
     # TODO: need to handle substitutions
 
     return activations
 
 
-def plot_acts(net, acts:dict, qacts:dict, kind='output'):
+def plot_acts(net, acts:dict, qacts:dict, kind='output', how='log'):
     for name, layer in net._modules.items():
         if isinstance(layer, nn.Sequential):
             plot_acts(net, acts, qacts)
         else:
             if name in set(acts.keys()):
                 x = acts[name].reshape(1, -1).squeeze().numpy()
                 y = qacts[name].reshape(1, -1).squeeze().numpy()
                 df = pd.DataFrame(data=np.stack([x, y], axis=-1), columns=["x", "y"])
-                width = 500
-                cvs = ds.Canvas(plot_width=width, plot_height=width)
-                agg = cvs.points(df, 'x', 'y')
-                img = ds.tf.set_background(ds.tf.shade(agg, how="log", cmap=cc.fire),
-                                           "black").to_pil()  # create a rasterized image
-                plt.xticks([], [])
-                plt.yticks([], [])
-                plt.imshow(img)
+
+                fig = plt.figure(figsize=(5.5, 5.5))
+                grid = ImageGrid(fig, 111, nrows_ncols=(1, 1), axes_pad=0.5, share_all=True,
+                                 cbar_location="right", cbar_mode="each", cbar_size="5%", cbar_pad="2%")
+
+                artist3 = dsshow(df, ds.Point('x', 'y'), ds.count(), norm=how, cmap='inferno', aspect='equal',
+                                 ax=grid[0])
+                plt.colorbar(artist3, cax=grid.cbar_axes[0])
+                grid[0].set_facecolor('#000000')
+                grid[0].set_title(f'{name}: {kind}')
                 plt.xlabel('acts')
                 plt.ylabel('qacts')
-                plt.title(f'{name}: {kind}')
                 plt.show()
```

## Comparing `fmot-1.3.4.dist-info/METADATA` & `fmot-1.5.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmot
-Version: 1.3.4
+Version: 1.5.6
 Summary: Femtosense Model Optimization Toolkit
 Home-page: https://github.com/femtosense/fmot
 Author: Femtosense
 Author-email: info@femtosense.ai
 Project-URL: Source, https://github.com/femtosense/fmot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: numpy (>=1.18.0)
 Requires-Dist: scipy
 Requires-Dist: python-speech-features
 Requires-Dist: tqdm
 Requires-Dist: networkx
 Requires-Dist: deprecation
 Requires-Dist: tabulate
-Requires-Dist: datashader
+Requires-Dist: datashader (>=0.14.4)
 Requires-Dist: colorcet
 Requires-Dist: matplotlib
 
 ![Build Status](https://codebuild.us-west-2.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiRGpDOFpEOXF1M0prSy9OOVNkZ3F2NkRKM0NNMG8xbmpZU0hZdUp1ejhHOEswdDRhOEZOakMrdWZyaHp1WGVtQ1lVTStzRUpXaFlYeFZPSEJFd21NdjF3PSIsIml2UGFyYW1ldGVyU3BlYyI6InJZYzhuZ3d3a1FUUzBzM0kiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=master)
 
 # fmot
 The Femtosense Model Optimization Toolkit (fmot) quantizes neural network models for deployment on Femtosense hardware.
```

## Comparing `fmot-1.3.4.dist-info/RECORD` & `fmot-1.5.6.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,146 +1,158 @@
 fmot/ENV_REQUIREMENTS.sh,sha256=qMNutpKLRCQMv70HRJhShmXAqDr_wic-NIn5kponsZI,1355
-fmot/PY_REQUIREMENTS,sha256=To16vNwSvyWRRpoHVM86H-qW0yFpAqz_lDm5QNpUkMs,129
-fmot/VERSION,sha256=4KcpQbpy5HHDewvOXowpJlm-_FHb8cfO6jVLJmQsOcM,6
-fmot/__init__.py,sha256=QbUDxXWjcOM_iU5suaJr3opOIXLsL7vi_psOmWVR-5s,581
-fmot/_open_docs.py,sha256=uNkj-I8nLHHKudorzALtbWFBqyKGW7bW59DFXGEyfkA,370
+fmot/PY_REQUIREMENTS,sha256=z2FbJTW3SjQ0E2dCkcq0KPEm_BNn8ndfhHbief-E2Bk,138
+fmot/VERSION,sha256=2rZOBsCBfXe0-IcmGDLLs0ugI8rHx01y2BBoVTZS0MU,6
+fmot/__init__.py,sha256=RjjwgFf7ZUWZxzWp23xViTOM3kfLXjsqWjO8-oAxsUw,648
+fmot/_open_docs.py,sha256=jdnE5Bokv9I7byUaw0fNRq6RqMCD_g4pPKmgBUDSIW4,414
 fmot/_supported_ops.py,sha256=_nWGLwheCOoDAW0hUMiNWX_V7C7q0ROHJWz4ojK9YJw,1611
+fmot/configure.py,sha256=fjW_mDYAmrOSrpd9cNDOJH0NEXRnGhvScKfkCwUSNkI,1654
 fmot/exceptions.py,sha256=k_hnhQvLqQzELA5yV8aDDnik6CxJkAXmfzeHbnaV3mc,929
 fmot/execute_code.py,sha256=eW227iyCxiDMKjCK4ruK5-vd_tYNrgL1a7KkRNJ1Q_U,1821
 fmot/functional.py,sha256=DH98rAmladME98oV5QNtiKicWbMVANGXJgSXGVYb548,61
 fmot/torchscript_utils.py,sha256=lca5a5S3-Wzp-_Lvfp6kHanFc48yG2Qagio3PbpM1jI,4945
 fmot/beta/__init__.py,sha256=LRcqC5g3JZ7ejVWFpadlnU_noRqkKPnDzCku_nq9vww,83
 fmot/beta/amp.py,sha256=OGJAi1h5gLWziv_kk8k9XpFYGRy0v2fRIZYz_0nzjuk,4169
 fmot/beta/auto_multiprecision.py,sha256=BbtXHvvZKeAIw6nu5NDGhk_umUAE7-8CVl9xn8lfkpE,10740
 fmot/beta/quantize_part.py,sha256=YgxUqZnUZCVFCW0Y75vP0Tr3cbmiI8QhXPWn2cT1iEc,1166
 fmot/convert/__init__.py,sha256=WAoTNbpBhUZz1QSCvGLGvv2g0Eyy1tjsYYsofYxCBNQ,200
 fmot/convert/_convert_to_qat.py,sha256=yNhnn3sz2JTQElnipPzFAK8Ba6qHE7LDcGs0JFU9L6w,2900
-fmot/convert/configure.py,sha256=NLB7Sw8mKVRcqYdYJuuKc1hT0FTxj4BsLKJ7ZjdUef4,807
-fmot/convert/conversion_api.py,sha256=saaAtUCRUCl6tbo-KtHwH-_XJqf1NT3yX26Vp4SGheA,15003
-fmot/convert/default_mappings.py,sha256=13g-cHvj2rYYRaq1avaX5RLBXuOFFXBnLmqbiOtF7g8,2496
-fmot/convert/default_patchings.py,sha256=FGTUQP8B9ihJ4i58rSo-NngYogn7VnJcxW4ywHg7zKg,9685
-fmot/convert/default_substitutions.py,sha256=toPPv0cU6TFmkbIPbU8r1gdhBkA3su4yJ2o6qo5iFZA,356
+fmot/convert/conversion_api.py,sha256=LugKItwCxLIANvVidfZSRqXad44-2o1mertYNkBZriw,15168
+fmot/convert/default_mappings.py,sha256=1UfCfsWDqip0S34HMGF1Dnw9ZLtiQI0Vz_odajhV7B8,2410
+fmot/convert/default_patchings.py,sha256=I7s_UHPIsCZvKy-cSmjxTDFg6rqeyKnpK6Vgm4k8ym0,9684
+fmot/convert/default_substitutions.py,sha256=NNMuIMLdzYaWG8KsLRfxgIp9ckptDMcfl08BB3m_abo,547
 fmot/convert/lut_registry.py,sha256=aTOnVsCoeWHorT9P7PyVuGNHc1qNzTMdqWO-NYt7Ezg,4562
-fmot/convert/mapping.py,sha256=wCzjgFeEy5JK09D456wSUifuzqCopM4iOSaE1r3u6o0,3383
+fmot/convert/mapping.py,sha256=XgZDs5MrG1UXwPpkcF-yg0lE3TC-UYdislOzr6my9fs,3998
 fmot/convert/optimizer.py,sha256=VOLVJTJTVdv3vznN0qIAyErzVFD6V36jLJqhe0naxqw,2831
 fmot/convert/param_manager.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fmot/convert/patch_ir.py,sha256=vL6ICASHUpYRNrHxOIAAFXaVIQiik-KqIomggl5npnc,24572
-fmot/convert/patching.py,sha256=-_HEi1-4N157ACyb2n3KalIXLC-5EAFwFf_t-4ceFBE,4116
-fmot/convert/prune_reparametrization.py,sha256=61aBJSqvj1JTFN1H9uE8KUB0UMDHxJO2tr0hj4yw4tw,3234
+fmot/convert/patch_ir.py,sha256=Y29mfiw33ebIBRtaElkiZTwl-UbI92kDedro_73-wxM,24680
+fmot/convert/patching.py,sha256=Nmp9DEfjCnyWfFpIfSLW63Tmf3i45vkLIeYZBr90AVA,4175
+fmot/convert/prune_reparametrization.py,sha256=z_cDRGmCuffym2YNvtz8cifQSWKxSWdU0c3-g4L4L44,3244
 fmot/convert/quantizer_manager.py,sha256=8vCSWq-u_GT1xk4gFV4_W_wP7rlWkeSa7FaMGWuJROU,2963
-fmot/convert/substitution.py,sha256=oaVqoHLvD2_te_eLilz86_ScV5XckCPZLnSWu8qzCiw,2111
+fmot/convert/substitution.py,sha256=XHx-XSdBFBgkdUwlnGYun7w8j9akzo1A3AQnzoZ3EUQ,2121
 fmot/fqir/__init__.py,sha256=FBYLaAL1u5sgX05hVkhnmdEpXb6laAYxllKybjjv0hg,199
 fmot/fqir/utils.py,sha256=nz_dstBc5nRB2Qx1q8-c-eQ_jNlKUU0VwTUEhPzxxNM,660
 fmot/fqir/graph_proto/__init__.py,sha256=Z8uP9WEhcJk5RvoZEVYruJVL_JT4ZgZev3kygnXboDs,35
-fmot/fqir/graph_proto/graph_proto.py,sha256=Pais-UOn2mV-tkvA91-a5hSMZC_YruKxslU4y4wYkOg,13785
-fmot/fqir/graph_proto/graph_runtime.py,sha256=Hy0llEmTeGftoWC-t3B2kMyDKsR6Tvwhyad5k4dtLUI,5214
+fmot/fqir/graph_proto/graph_proto.py,sha256=OYnujquygeIAR8p3_SV3xMefNRCW1NNXzWBM7JBRuBc,13950
+fmot/fqir/graph_proto/graph_runtime.py,sha256=fZekhNLutB5NjhuDlgdwo2bs7fe4FBz4-zB-KIK6ppg,5303
 fmot/fqir/nodes/__init__.py,sha256=03z-NMhbd3OK3navTGGa-fdPdaRhxFTLGfLdwDSoA2U,115
 fmot/fqir/nodes/node_base.py,sha256=p65snA4NXOGXTdGerX0eOrFesUFqNElNDkO-4Rq3F14,5761
-fmot/fqir/nodes/node_proto.py,sha256=gzGE4neuW1S9zrdTtAqiBtINrNz9mDYZplyqzTL-RDI,6731
+fmot/fqir/nodes/node_proto.py,sha256=sxCtGVSLv1LshJUaf-VTSlNAjRYzObDzpUMCJvVCRvA,6920
 fmot/fqir/nodes/opcount.py,sha256=re2PBoxFr35uMdK2HmTWJ04emTzAiF2oYl-nGpLyAtY,2207
 fmot/fqir/nodes/opcounters.py,sha256=jj0g63rXsnIYjOJ3C4jLR4TsK3T6w8BtqbwYg5AEixQ,20518
-fmot/fqir/nodes/optype_base.py,sha256=I_AR_tdkBWmh-ru_8o1d7Hn5OrNVwFBx5WtKBddYYEw,6933
-fmot/fqir/nodes/optypes.py,sha256=1Vqq_IA7Nn02c8KDhOQ2NQKZym89tKLnbROMbw23dRg,33465
-fmot/fqir/passes/__init__.py,sha256=ay7VpHan95VYUbFkplUl9pL4tgEt_HvaoYWlYg9Qxv0,398
+fmot/fqir/nodes/optype_base.py,sha256=OclRVltobcSWpauQ2PPbpagVIXf8u_fkVXXnMLBIdE0,7008
+fmot/fqir/nodes/optypes.py,sha256=FL-YGfU1MDH1uXdy719gjx89B0YdbvCDWOViig0Tg2w,30178
+fmot/fqir/passes/__init__.py,sha256=afwmXU2BFbmvH_3nBqBhBKJ8clovG1yNVljnjXgOjq0,583
 fmot/fqir/passes/batchdim_removal.py,sha256=RzO-0Bx3XjbMwlhwTfiTavz2yi_svJSUmuYsPcWhapY,7322
+fmot/fqir/passes/cleanup.py,sha256=wc4ga3tEPCiBd9Bb9aXb9wxCMN8OkqCCBlFUK_JoPlo,1606
 fmot/fqir/passes/dimtag_removal.py,sha256=8c8DFKAM30ydXPOJmK4K5z7dSosngzEzULIR0ik0cmU,463
 fmot/fqir/passes/helpers.py,sha256=iombb6QFrIBzAXomFyvW4eQD8CEdI1tYqtIZKk6JpOs,1160
-fmot/fqir/passes/kernelize_lstm.py,sha256=h-l4ojm5CbwzapV8mdfqjg1qPF-VmVRzlVbEx3JHt0I,19953
+fmot/fqir/passes/kernelize_lstm.py,sha256=wpURIbcd5KtxWtcNY3UyQKxCFqbF9dhLv1mZ-5FTRKM,19971
+fmot/fqir/passes/kernelize_red_broad.py,sha256=Y9TqT0dVra4p6IpjS78QP7gHOM4cwTkRPpkXYAaTYBc,5496
 fmot/fqir/passes/kernelize_temporal_unfold.py,sha256=ihZcChdCiwC18coYPPnXymx9p2wgWEmIPhj2zTT3qCg,2039
-fmot/fqir/passes/uniquify_names.py,sha256=dSiorlrbXuDMY28ymwQr6l0JOSwogJwowWMjOWGsiO8,657
 fmot/fqir/variables/__init__.py,sha256=24krQW55auJPC_q0hoV71-RD9AOWWiaWyOnazLkrtMM,94
 fmot/fqir/variables/tensor_proto.py,sha256=EvQwq6KJOfx8D1HBTRxio9sEsy71Ny_kkcpARmp9-XQ,6255
 fmot/fqir/variables/variable_base.py,sha256=4d1UdjK0IU4MIaNZqzW7TO3ePZwdZHAURakw5otuB60,2064
-fmot/nn/__init__.py,sha256=Uk_D-DhIlhH4XSsAYMYYnS_lFhrhn36eMwqfw50SNt8,385
-fmot/nn/atomics.py,sha256=vYhmju_YoBkv-1aaNPiF7MgcurGPvkSRq7nWxsMEptY,8315
-fmot/nn/composites.py,sha256=z7yZ0-ZfoKrB05lYxqRrM8QAbkqGiDm6Mzn5QV6xMgk,11515
+fmot/nn/__init__.py,sha256=TI8l3MAV6pa-l3_oHVQ0az0hTES9xgmuPb7JUjOI68g,563
+fmot/nn/atomics.py,sha256=E_FxbKKigyz06vydochdiBRgzyZk8KA-i-fvl9B5xic,8663
+fmot/nn/composites.py,sha256=MkjKot4gqbmOdWDfH5qVkizq3_grqv_2Un5lMUAsqXc,12272
 fmot/nn/conv1d.py,sha256=nPPLo_S2GYHLJhsKbaE0t6QVzSt92I3lnop3uFiSPvk,27568
+fmot/nn/derived_param.py,sha256=wLgyVPScJp0VHsHWRNq5TtgShES2vjZPQDlYtCNZEAo,1844
 fmot/nn/femtornn.py,sha256=T7XtDFWoURSKCMfMBZfJp1WablYNxvbxSNWBzEAdG0M,21993
-fmot/nn/fft.py,sha256=E63C8QbsVETe5PxuSA3Se2EZ_gEKCNDFF45Ns9QVUF4,10431
-fmot/nn/sequenced_rnn.py,sha256=7iqwX6HvbR9H020oYpFkK54r3ohNWVjDbjCXD3xeFxc,31321
-fmot/nn/sequencer.py,sha256=LdZhhfDAqAXhFsiowSDzz8AZ-1f5vNOeiuP936ARfAc,5092
-fmot/nn/signal.py,sha256=cNa6b5qybtcfGS6WCsMywIQMDXuSG_DxekQaWli4MCM,19424
+fmot/nn/fft.py,sha256=J4Rlcko7K_sprpeIT5ptniXzyjsLPEkoqAnzzPNNPhc,17526
+fmot/nn/sequenced_rnn.py,sha256=yO6YpwSyQdxBCELHGFVILFNZmHlp5njYxHOCXW9yKao,34238
+fmot/nn/sequencer.py,sha256=9gCgumIvuO71PajoEfcZbi9XGTzqywTDNeEn62xKTP8,5305
+fmot/nn/signal_processing.py,sha256=_eghECb8TGkaUeLznM9vmCO0MkQNNGVebCUUHexHBqw,11986
+fmot/nn/sliding_attention.py,sha256=Bw-2gno_1IExLnmGqiNVIs2_Ee4z4mDRdevxyHp9B24,3742
 fmot/nn/sparsifiers.py,sha256=iXrs6RgTThGDeXGrEqQzI4cC-VxPdzUdIEKqe9tApFc,9256
 fmot/nn/sru.py,sha256=etnDGB85LxrJsDvN9gecAdOuRB5J2p96dfYIz9tuAos,2294
-fmot/nn/stft.py,sha256=WXjabyXGoOl1LwxamlNk_HYUTd_Ih4ZuR2ORWQPOB1g,6028
+fmot/nn/stft.py,sha256=ycbGfbzDXqCmdjZ1_9f-iPJRHJISMefiJos9f_AtZns,8916
 fmot/nn/super_structures.py,sha256=bzPhxlmmHlgRixm7-BvhPcSnyBvty4UCr1qFLLXf1UI,1525
+fmot/nn/temporal_unfold.py,sha256=uE87sL-CEHcwMmsRcIB_epZyort3AoZG3nz1lt8tp98,1430
 fmot/qat/__init__.py,sha256=GWbiQ7uKgJxaWK4_62Ksx44I-sHWFxH-UKpmGlaAoU4,192
 fmot/qat/annotated_tensors.py,sha256=pKNpd0ujdz27eMy1vrGZDFwdTWC_RHxdw1pnCXVpTnc,4059
 fmot/qat/bitwidths.py,sha256=SONkjQsx0DAB9voBgewMFGbDbx58b5nQou6-8t3GErI,1659
 fmot/qat/control.py,sha256=zqirgQTZraD2xmiBTJh6rOiVDI-CuMy7n2Wuu0ji8lk,4381
 fmot/qat/fake_quantization.py,sha256=jzQJT-FKpg7DHMT0VfsfG2fJ3oOSbRVqxF95Lnafypc,2684
-fmot/qat/nn/__init__.py,sha256=kLUrgQxQo4nncZEnJzfI_6frFTpVXNlANVZd534f1jU,279
+fmot/qat/nn/__init__.py,sha256=MHRSPGRPFuHpdnt75uzJAnBx7NsFvvPDR3_cnnfKSR8,328
 fmot/qat/nn/_utils.py,sha256=ywQLkY7SpR7ES8r07XBHXFVzQOKMcSfMRqmD1t_9q6s,276
 fmot/qat/nn/act_density.py,sha256=zF7GCnKfopSfKEFIXI79W5z9C_X4uVTldgMXTdXJPho,3783
-fmot/qat/nn/atomics.py,sha256=CymNRfa3-yWW7F_f4UbOx44FYlvHhxaPJSeSbJHS6_U,28123
-fmot/qat/nn/composites.py,sha256=oDku4IFXn5A9CxtHt1oi_f3u5qKabX_sufyATwbSCaQ,9167
-fmot/qat/nn/density_matmul.py,sha256=qsdGGWyvXzB3Aj1AQWKIGawdFdsHHeM9xm4a58MZDj4,10426
-fmot/qat/nn/high_level.py,sha256=bmJl8mx_3_EpaReaDBQBGaL0VULIlWdO2YFtFT3fHcM,13703
-fmot/qat/nn/linear.py,sha256=E8Z3EN4F6ZQewpYmhZo1WEhNei7aWfDs5W7RG0l66X4,3210
-fmot/qat/nn/lstm.py,sha256=ydAARWLV4To8xXpSqlWMP-XnC5BUw1Tl0nhQRJ55dwc,19301
-fmot/qat/nn/luts.py,sha256=rGsfKyy5fW5jzEaPzGiNRZjzLKKhXmLxrUynlTAwj2c,13738
+fmot/qat/nn/atomics.py,sha256=2SSK6J_Eikqc5w2AUXSuxQ4bdm7hxXBGEEAWKBrEhTw,28153
+fmot/qat/nn/composites.py,sha256=ZJQoJXGdwMWSI63NJCrb013dV5yDkJvPzK0ZiwTZozE,9198
+fmot/qat/nn/density_matmul.py,sha256=hH7L4s2xg5ZBzV4IWdleW-PlBuJW29V8k04y44yjaGw,10828
+fmot/qat/nn/derived_param.py,sha256=0dnjLzUedGM4ib_1gLAmvHK6446OHq2qyKjKn86vqhA,2102
+fmot/qat/nn/linear.py,sha256=BeQh3-GAnrEVpuWuPjfxE_xe4IRuVhv_GIL02R-kRmU,8923
+fmot/qat/nn/lstm.py,sha256=KIZXGCVp9rcjWilX44KKnJvtRpxBHMbkGwa-mV6gkek,19303
+fmot/qat/nn/luts.py,sha256=FLAV9AdxqqfkAgi6iohuEJFumGiCQq1us4gs6lo_Nsk,14400
 fmot/qat/nn/norm.py,sha256=2BJHcjZO-q9S0kAxlV3uc6lGUj8ZaaSS1tdHLzNcxus,3922
 fmot/qat/nn/quant_wrap.py,sha256=QzS6bOdeOgk6RjG1gXVzSECdEEEQfOLfKAtnFOs_ib4,1350
-fmot/qat/nn/quantizers.py,sha256=WwSV6IqpQm_QaieNrj4RkH-s6Q8LV2aG8C6jXLE6wds,21181
+fmot/qat/nn/quantizers.py,sha256=hWGbOAmX_K_jJTZ4hlikKzljnVoQqmqHoK1NCMEJ5BQ,22679
 fmot/qat/nn/sequencer.py,sha256=wgPQUYOelvWXAIEiUMCnT1gg7F0djejYYbaJqTliav4,1992
+fmot/qat/nn/temporal_unfold.py,sha256=aM-LLxoKbS1h7NWij6PJYzzJf4UAI-UeB_TlB_-whtc,2283
+fmot/qat/nn/tuning_eps.py,sha256=9LJoz8N8hDXNRQOV3vm_flWxkNa72_6t8duCYrIVTUE,1007
 fmot/sparse/__init__.py,sha256=QpJsuYPTkQIXS6w3cTbMNHVlcvo_BMHdJ43UuomqbCM,90
-fmot/sparse/act_pruning.py,sha256=czRaWTuzgJQ9OQSaob_U5MU1jyXYlBH5F5LYD_RAqSU,2657
+fmot/sparse/act_pruning.py,sha256=AVjhbbFsbKyMHEBdhJ6l7QxpTEGgpiq77QVpgvq5hgA,2694
 fmot/sparse/pruning.py,sha256=oC1BXhGhUq-tgmL_96skeuXfnjhPNNjTtg__N8mkB2s,7357
 fmot/sparse/pruning_schedulers.py,sha256=NipSDgmx-EehZmeftBO40yIJyrpUkYPxM1bpgnewZ_Y,4024
 fmot/sparse/pruning_utils.py,sha256=TXpJzk9l1UsxX-KvjQ_sSKRlaYQlp5wlJJvJhU1-yt0,7162
 fmot/test/__init__.py,sha256=zUZZFbzV1lkoUXQIR54JZ9RzN8oRut1_LOu8CbZQrYU,196
 fmot/test/ds_tc_resnet.py,sha256=qG3esRvLHpZoRfFirFrDEioUDOKd0plcatCU0Os6L-A,5861
 fmot/test/kws_test_library.py,sha256=xTHvEgfPQ9EEJTTfnSDIYEuKJAz-6nNdPHaD-NtWl2U,3000
 fmot/test/test_automp.py,sha256=ySoNtmNCuwJNhgi1vX1iF10ftmFePyo7-GE-rpLakws,936
 fmot/test/test_cqt.py,sha256=XviR6eHxQ9WC72RnhbYqW4GnGoXQWodEbo4Oez1QIR0,1373
 fmot/test/test_cuda.py,sha256=Oa8KXn7QFiJoW5eOyOxapBq87keAx3NH2UQWMwdC4rs,1688
 fmot/test/test_density_tracking.py,sha256=jYI2VZm6JNnxd8SWc4Se7GxDWT6hUPNIjDZfIAna4Bg,3878
 fmot/test/test_diagnosis.py,sha256=13dWgNzssiZZrolmPwvGq-DVobIxKgDun3sX135kCkU,1134
-fmot/test/test_dim_anno.py,sha256=jMxy65ZcjTFVppv4OUU7JsLR6dhYBC1c-AbvwRiIAUM,3411
+fmot/test/test_dim_anno.py,sha256=ZKVJo9M2bHlIquxXEfPivXG1ieqzsodzjzwZ5ow6_qA,3433
 fmot/test/test_dropout.py,sha256=0XgNwJ609WHtLrXzqp8PSNZGYjZ9ntaRbATcorJK9NI,958
-fmot/test/test_features.py,sha256=Zbiy16FT9CnQYfUKhcjWWH2_qNrsYmtQWV3pBvbgnIA,14190
-fmot/test/test_fft.py,sha256=3bGECXEBj8XadMaylV6d50JkM156dqAR6SS-YIfaO6Q,323
+fmot/test/test_features.py,sha256=nEunkALbXEqkWLiYJU-SHGV7CdNjNN53jDRffR2BhRY,14304
+fmot/test/test_fft.py,sha256=4TsK2dMlDEEjc9PS1mf-qQbXRRjbz6e_1fd233Hu3b8,722
+fmot/test/test_ifft.py,sha256=FWbgSLr2S-yymWMyn3Tjme7FsCP6DqwaRk00tvE4ymk,1664
+fmot/test/test_layernorm.py,sha256=XPCzKKfeOZW2wwyw7AWHbBFEwk-9cFBhJhGzjl5wi3A,378
+fmot/test/test_lut_grads.py,sha256=4vsB6UvrGSXLO_f4j0KRxvhckXeNarbQuhqSpWyEXVc,1412
 fmot/test/test_nn_stft.py,sha256=Mr1okpY15KvD9HHiZHde5rmd8XKbxf38_jA5UObJd3A,3581
 fmot/test/test_observers.py,sha256=brKTwKQTJUhJgcbxWZRz3QhtoEvmrNwI49XfgMlqikc,2347
 fmot/test/test_package.py,sha256=nGhN_t6QcGI0YYX_bAPPPLO5AmVId3mpJzYhw-jmS7g,310
 fmot/test/test_param_reuse.py,sha256=nq4rU4vQIccL8uYOC7APtOjAGPl1Q2jLUARxmi-LndA,1240
 fmot/test/test_precision_mod.py,sha256=FCKgaUfN6Yw9YN8eOMQQGPb9rpv0q2K0f0BqtdvKCgE,830
 fmot/test/test_pruning.py,sha256=by3oUaiX4fBOLFo2vyIP4wfVqkAwbr6newGx15JGmUA,6440
-fmot/test/test_sequencers.py,sha256=VXkZhrtyXTfDku5X3r7WMoGcP6a5-7po2ho7yeUYj_A,25081
+fmot/test/test_sequencers.py,sha256=Emw6kM_9KqKByGMfaYcauglVS9IH5Sbgu0_5cicVs4k,25171
 fmot/test/test_serialization.py,sha256=WHKtFFXeuVcpk3thhlfFGZMUEqQ20afh2uFcFkAjnkU,2017
+fmot/test/test_stft.py,sha256=VOGUKDZFj47GH0FZG-6NHdN7qD9b-GmStRPKMaCAIwk,4308
+fmot/test/test_temporal_unfold.py,sha256=ONAuazo-2BGjgfdVA-nJjrpmAUG38PbmXBh1kzW9VWA,1322
 fmot/test/test_fqir/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fmot/test/test_fqir/test_opchecks.py,sha256=iXzfg9BCv8NqFh5faSLnbj78LqXxZ3Hwl9Fb8SOdhG8,1657
 fmot/test/test_fqir/test_readme.py,sha256=IJIxJtkoUC3ApIeyyUQTzLv9iBLuU99VkpeYKCNBkgE,1138
 fmot/test/test_fqir/test_single_ops.py,sha256=v0_loWxEUsBWmc-mEa4ohq6-t9iiEJT_0vBfzZE6EeE,15396
-fmot/test/utm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fmot/test/utm/__init__.py,sha256=pgT5r5mbG89As3Q1YGTDB2wI3qcVk8FyNwpGqdpDYjQ,147
 fmot/test/utm/atomic_test_library.py,sha256=InVu5_aJQ5ib24g4YhwmE9SDZgTnO18I9VztZj8fjNU,13543
-fmot/test/utm/feedforward_test_library.py,sha256=3DkrZKFoM8eGw8xmbMVsPTHY1LJxJ59g7-ZruDMijn0,4280
+fmot/test/utm/feedforward_test_library.py,sha256=eUervreGPxJx2jNTFAFtB2aor7Z_2A1gPSks4aRMjrU,5731
 fmot/test/utm/get_utms.py,sha256=T3DQ7IZkVYhsHj9wcPJ4-rjU-IeKojtASLZlKq-6waU,990
 fmot/test/utm/plot_errors.py,sha256=aBQZ3J40HGjGafl-_8fFmcYoZk2fEnylllXBnSL_A5I,2284
-fmot/test/utm/quant_tolerances.py,sha256=cnsERh4YzdzA8lH2Tx3Jm6eBbTWSJpB74MNHp9-lwGw,3589
-fmot/test/utm/rnn_test_library.py,sha256=mo0CZF3LyCAWh2IaXcu4lQIfREnpr5rkcgH_Q2jWazI,9964
+fmot/test/utm/quant_tolerances.py,sha256=d0f3PL3PUjp_lmImOkwaDGFexgFVKr5WWObaqOV3xPU,3603
+fmot/test/utm/rnn_test_library.py,sha256=PbuzdIFylgDU51ixyt3rfOPBk5j-eZjNMY4PDotr0Is,10015
 fmot/test/utm/test_utm_converted_runtime.py,sha256=8Vz3N8xXe3rPnz_9OL4GLijTOrC_hSDr8sZf8hHQZTo,173
 fmot/test/utm/test_utm_fqir_runtime.py,sha256=xgS1Y6PV1LcdXZWBAPTtna4uTJ6zeBwRA103dhNfQkk,340
 fmot/test/utm/test_utm_mixed_precision.py,sha256=cVgnxQi6IBSr64aE9YkKU1kqUVzvnpdHSzKuIkXJJ88,316
 fmot/test/utm/test_utm_quantization_error.py,sha256=L5LkOkZ3wGER7lk9AcvUHmuDIA0qoaoGj94k1klB9Sw,587
-fmot/test/utm/unittest_objects.py,sha256=wxcTGGBRNG0Wd2ov7STNrotEqb822ecX313yz3K2sKg,11995
+fmot/test/utm/unittest_objects.py,sha256=cpJkBOEwFDvAhvEFzBVw3blBOW0ppvbzm4idmfP7YeY,12337
 fmot/tracing/__init__.py,sha256=keA7A6UXMfdgeAXN5XaKgY3z_sTWG8T2f4ypfq9l_vE,90
-fmot/tracing/oplinks_v1.py,sha256=CgcxiC7MJe0V3zjDoBaCcchWDI2ZvPhKx7614ZwhHg4,1743
-fmot/tracing/tracing.py,sha256=-WaV-bHX6k9pb5cfGviIAUTOnyj1JDUqYDzt83U-xhw,22779
-fmot/tracing/tracing_blacklist.py,sha256=iKN2cP26wBSq81MCDaHcPHFqL1K1tcrVmWkfg2y0MAs,344
+fmot/tracing/compare_fqir.py,sha256=qn5gtNxSx95BxMyl7e7zdgX0_m9wuk5hX9vEquqbFK4,2699
+fmot/tracing/oplinks_v1.py,sha256=fFURVJJ7vjWeDcwnBWW-SICEJY5Ulos6y4z9vTm8c7A,1542
+fmot/tracing/tracing.py,sha256=fSL4h-tUiivhNqzMd_30Iii_ldWuahS6J4mpx5B-BT4,23682
+fmot/tracing/tracing_blacklist.py,sha256=7pVYn_Q_WqZ7AiepktYaUMokubGIqhfn-bVvnrl3DT4,365
 fmot/tracing/utils.py,sha256=pep9UWxR4EA6Y-wXzBM16fiYG7ljkh1Ou4x5GpksFZc,2017
 fmot/utils/__init__.py,sha256=Z7iVfecDYakoEW3W0RmZXjjWmUQC8DrVEmvsW1AliNA,325
 fmot/utils/activity.py,sha256=TLJnGKqi-iIWce7S0bHFbvDP5lgaVLPDKyys_bRK1HA,3941
 fmot/utils/conv1d_utils.py,sha256=j79pgm7i6WkdXMHwkeEIHx41BCumxZtilt1ucLkcpZY,3089
 fmot/utils/param_manager.py,sha256=QV-of7kTfhQTrWFSSvkok1FhX_ygeg7R3WIewzCVsIg,2245
 fmot/utils/quant_diagnostic.py,sha256=lafkYJV-51mHOE5lw7sE9x-4hExHIRpSqUrhSRugY9E,6744
 fmot/utils/quantizer_manager.py,sha256=bBicDeeeMrd8Hq4wXN92-53579j1-3feSqkbUTYzFoQ,1792
 fmot/utils/rich_attr.py,sha256=olbVQ0HCx41zcwwvAQUo9yt1PYMia3rUqd0j8XHDcMQ,357
-fmot/utils/saturation_opt.py,sha256=wz_hgSYh8ds9V525SQhA3HVBb4VU_4XWX9W20mE6qJI,9783
+fmot/utils/saturation_opt.py,sha256=uiG3UPuAWq_ehA_lwRh-bVWPLIDam-cBifkpnxNKapA,8372
 fmot/utils/serialization.py,sha256=w_kYDaV_K84RYf9hGuLuhwiV-0s_OBaBIio8t2lNqU4,1986
 fmot/utils/quant_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fmot/utils/quant_tools/diagnosis.py,sha256=9K6tid7qz3ipcaxvSs4nSSXHkjr1JaAA_54vQgYt_XY,4118
-fmot-1.3.4.dist-info/LICENSE,sha256=eN9ZI1xHjUmFvN3TEeop5kBGXRUBfbsl55KBNBYYFqI,36
-fmot-1.3.4.dist-info/METADATA,sha256=WlEPMo1NXVFzQF3I-D7cT9IqaAcIeGkMsMFJZGhk2cc,3657
-fmot-1.3.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fmot-1.3.4.dist-info/top_level.txt,sha256=y0zAp-_TLm8xLv-iKiAhM181teNK64s7Zvp2oshNxY8,5
-fmot-1.3.4.dist-info/RECORD,,
+fmot/utils/quant_tools/diagnosis.py,sha256=Er7vE0XzNv2s8LkTSdeE1h4lzbLCOaax4XinIqm7pU0,4545
+fmot-1.5.6.dist-info/LICENSE,sha256=eN9ZI1xHjUmFvN3TEeop5kBGXRUBfbsl55KBNBYYFqI,36
+fmot-1.5.6.dist-info/METADATA,sha256=yDQSAPnrzBhCLt2HVtl9Ly-yHg42p2GFnT2CWr99wfM,3668
+fmot-1.5.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fmot-1.5.6.dist-info/top_level.txt,sha256=y0zAp-_TLm8xLv-iKiAhM181teNK64s7Zvp2oshNxY8,5
+fmot-1.5.6.dist-info/RECORD,,
```

