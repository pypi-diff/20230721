# Comparing `tmp/neural_compressor-2.2.tar.gz` & `tmp/neural_compressor-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_compressor-2.2.tar", last modified: Wed Jun 21 12:28:59 2023, max compression
+gzip compressed data, was "neural_compressor-2.2.1.tar", last modified: Fri Jul 21 10:57:52 2023, max compression
```

## Comparing `neural_compressor-2.2.tar` & `neural_compressor-2.2.1.tar`

### file list

```diff
@@ -1,577 +1,577 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.632919 neural_compressor-2.2/
--rw-r--r--   0 root         (0) root         (0)    11360 2023-06-21 12:28:42.000000 neural_compressor-2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11139 2023-06-21 12:28:59.632919 neural_compressor-2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10403 2023-06-21 12:28:42.000000 neural_compressor-2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.561916 neural_compressor-2.2/neural_coder/
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/__init__.py
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.568917 neural_compressor-2.2/neural_coder/backends/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/intel_extension_for_transformers.yaml
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/keras_inc.yaml
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1058 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_bf16_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_bf16_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_bf16_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1037 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_fp32_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1032 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_fp32_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_fp32_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_gpu_to_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_int8.yaml
--rw-r--r--   0 root         (0) root         (0)     1057 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1077 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1056 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1044 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_onnxruntime_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_openvino_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1062 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/nano_openvino_int8.yaml
--rw-r--r--   0 root         (0) root         (0)     1082 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/onnx_inc_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1082 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/onnx_inc_static_quant_qdq.yaml
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml
--rw-r--r--   0 root         (0) root         (0)      922 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_aliblade.yaml
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_benchmark.yaml
--rw-r--r--   0 root         (0) root         (0)     1246 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_channels_last.yaml
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1761 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml
--rw-r--r--   0 root         (0) root         (0)     1548 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml
--rw-r--r--   0 root         (0) root         (0)     1719 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_fx.yaml
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     1306 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_ipex_bf16.yaml
--rw-r--r--   0 root         (0) root         (0)     1076 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_ipex_fp32.yaml
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1539 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml
--rw-r--r--   0 root         (0) root         (0)     1260 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_jit_script.yaml
--rw-r--r--   0 root         (0) root         (0)     1234 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_jit_script_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_jit_trace.yaml
--rw-r--r--   0 root         (0) root         (0)     1321 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_jit_trace_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)      860 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_cuda.yaml
--rw-r--r--   0 root         (0) root         (0)      843 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1216 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml
--rw-r--r--   0 root         (0) root         (0)     1250 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml
--rw-r--r--   0 root         (0) root         (0)     1118 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/backends/template.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.569917 neural_compressor-2.2/neural_coder/coders/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.569917 neural_compressor-2.2/neural_coder/coders/autoinc/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/autoinc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26057 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/autoinc/autoinc_harness.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/autoinc/calib_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/autoinc/domain.py
--rw-r--r--   0 root         (0) root         (0)     4793 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/autoinc/eval_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.570917 neural_compressor-2.2/neural_coder/coders/pytorch/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3204 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/batch_size.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/cuda_to_cpu.py
--rw-r--r--   0 root         (0) root         (0)     6755 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)    23101 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/harness.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/lightning.py
--rw-r--r--   0 root         (0) root         (0)     3667 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py
--rw-r--r--   0 root         (0) root         (0)     5291 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/pytorch/reclaim_inputs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.571917 neural_compressor-2.2/neural_coder/coders/tensorflow/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/tensorflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/tensorflow/amp.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/tensorflow/inc.py
--rw-r--r--   0 root         (0) root         (0)     3716 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/coders/transform.py
--rw-r--r--   0 root         (0) root         (0)     3401 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.571917 neural_compressor-2.2/neural_coder/graphers/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11123 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/code_line.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/function.py
--rw-r--r--   0 root         (0) root         (0)    12402 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.572917 neural_compressor-2.2/neural_coder/graphers/preloads/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/preloads/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58208 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/graphers/preloads/transformers.yaml
--rw-r--r--   0 root         (0) root         (0)    52440 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/interface.py
--rw-r--r--   0 root         (0) root         (0)     3722 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.573917 neural_compressor-2.2/neural_coder/utils/
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/cpu_info.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/device.py
--rw-r--r--   0 root         (0) root         (0)     7527 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/handle_user_input.py
--rw-r--r--   0 root         (0) root         (0)     5116 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/line_operation.py
--rw-r--r--   0 root         (0) root         (0)    38671 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/numa_launcher.py
--rw-r--r--   0 root         (0) root         (0)    18664 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/utils/pdf_report.py
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_coder/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.574917 neural_compressor-2.2/neural_compressor/
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.578917 neural_compressor-2.2/neural_compressor/adaptor/
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/adaptor.py
--rw-r--r--   0 root         (0) root         (0)    45064 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.579917 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/conv2d.py
--rw-r--r--   0 root         (0) root         (0)     2861 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/dense.py
--rw-r--r--   0 root         (0) root         (0)     4456 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/pool2d.py
--rw-r--r--   0 root         (0) root         (0)     3950 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/quantizer.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/keras_utils/separable_conv2d.py
--rw-r--r--   0 root         (0) root         (0)    22316 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/mxnet.py
--rw-r--r--   0 root         (0) root         (0)    10620 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/mxnet.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.579917 neural_compressor-2.2/neural_compressor/adaptor/mxnet_utils/
--rw-r--r--   0 root         (0) root         (0)      655 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/mxnet_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31176 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/mxnet_utils/util.py
--rw-r--r--   0 root         (0) root         (0)    77117 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/onnxrt.py
--rw-r--r--   0 root         (0) root         (0)    15262 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/onnxrt.yaml
--rw-r--r--   0 root         (0) root         (0)    15699 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/onnxrt_cuda.yaml
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/onnxrt_trt.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.580917 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/
--rw-r--r--   0 root         (0) root         (0)      656 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36485 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/calibration.py
--rw-r--r--   0 root         (0) root         (0)    15844 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/calibrator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.583917 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5434 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/activation.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/argmax.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/attention.py
--rw-r--r--   0 root         (0) root         (0)     5475 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/binary_op.py
--rw-r--r--   0 root         (0) root         (0)     6055 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/concat.py
--rw-r--r--   0 root         (0) root         (0)    10775 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/conv.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/direct_q8.py
--rw-r--r--   0 root         (0) root         (0)     4360 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py
--rw-r--r--   0 root         (0) root         (0)     5694 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gather.py
--rw-r--r--   0 root         (0) root         (0)     3662 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gavgpool.py
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gemm.py
--rw-r--r--   0 root         (0) root         (0)     5776 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/lstm.py
--rw-r--r--   0 root         (0) root         (0)     8860 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/matmul.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/maxpool.py
--rw-r--r--   0 root         (0) root         (0)     1719 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/norm.py
--rw-r--r--   0 root         (0) root         (0)     5638 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/ops.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/pad.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/pooling.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/reduce.py
--rw-r--r--   0 root         (0) root         (0)     3444 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/resize.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/split.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/unary_op.py
--rw-r--r--   0 root         (0) root         (0)    61182 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/quantizer.py
--rw-r--r--   0 root         (0) root         (0)    30141 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)    20482 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/ox_utils/util.py
--rw-r--r--   0 root         (0) root         (0)   220311 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/pytorch.py
--rw-r--r--   0 root         (0) root         (0)    15795 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/pytorch_cpu.yaml
--rw-r--r--   0 root         (0) root         (0)     2627 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/pytorch_gpu.yaml
--rw-r--r--   0 root         (0) root         (0)     4958 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/pytorch_ipex.yaml
--rw-r--r--   0 root         (0) root         (0)     2384 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/query.py
--rw-r--r--   0 root         (0) root         (0)   113916 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     9968 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tensorflow.yaml
--rw-r--r--   0 root         (0) root         (0)     6941 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tensorflow_itex.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.584917 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42716 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_converter.py
--rw-r--r--   0 root         (0) root         (0)    16274 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.585917 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.585917 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13846 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.590918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3985 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py
--rw-r--r--   0 root         (0) root         (0)     3305 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dequantize_cast_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py
--rw-r--r--   0 root         (0) root         (0)     5522 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3912 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py
--rw-r--r--   0 root         (0) root         (0)    13288 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     7500 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py
--rw-r--r--   0 root         (0) root         (0)     3813 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py
--rw-r--r--   0 root         (0) root         (0)     5035 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py
--rw-r--r--   0 root         (0) root         (0)    17017 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py
--rw-r--r--   0 root         (0) root         (0)    16070 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py
--rw-r--r--   0 root         (0) root         (0)     9885 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py
--rw-r--r--   0 root         (0) root         (0)     5588 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py
--rw-r--r--   0 root         (0) root         (0)     5998 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py
--rw-r--r--   0 root         (0) root         (0)    12728 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py
--rw-r--r--   0 root         (0) root         (0)     5980 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py
--rw-r--r--   0 root         (0) root         (0)    13918 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py
--rw-r--r--   0 root         (0) root         (0)     2219 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py
--rw-r--r--   0 root         (0) root         (0)     3420 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1224 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.592918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py
--rw-r--r--   0 root         (0) root         (0)    18210 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py
--rw-r--r--   0 root         (0) root         (0)     7028 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    39443 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py
--rw-r--r--   0 root         (0) root         (0)     8188 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
--rw-r--r--   0 root         (0) root         (0)    41642 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py
--rw-r--r--   0 root         (0) root         (0)     5409 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     1769 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py
--rw-r--r--   0 root         (0) root         (0)    17254 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.592918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55654 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py
--rw-r--r--   0 root         (0) root         (0)    13537 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py
--rw-r--r--   0 root         (0) root         (0)    22286 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.593918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37367 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py
--rw-r--r--   0 root         (0) root         (0)    40440 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.594918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.595918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8721 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.596918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/
--rw-r--r--   0 root         (0) root         (0)      675 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
--rw-r--r--   0 root         (0) root         (0)     3134 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
--rw-r--r--   0 root         (0) root         (0)    10309 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.597918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13718 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py
--rw-r--r--   0 root         (0) root         (0)    12386 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py
--rw-r--r--   0 root         (0) root         (0)   112996 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py
--rw-r--r--   0 root         (0) root         (0)    27174 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py
--rw-r--r--   0 root         (0) root         (0)     8266 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py
--rw-r--r--   0 root         (0) root         (0)    55564 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py
--rw-r--r--   0 root         (0) root         (0)     6075 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py
--rw-r--r--   0 root         (0) root         (0)     7074 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py
--rw-r--r--   0 root         (0) root         (0)    39207 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py
--rw-r--r--   0 root         (0) root         (0)    13443 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py
--rw-r--r--   0 root         (0) root         (0)     4867 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py
--rw-r--r--   0 root         (0) root         (0)    21256 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py
--rw-r--r--   0 root         (0) root         (0)     5481 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py
--rw-r--r--   0 root         (0) root         (0)    17273 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py
--rw-r--r--   0 root         (0) root         (0)    19188 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph_common.py
--rw-r--r--   0 root         (0) root         (0)    10384 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py
--rw-r--r--   0 root         (0) root         (0)     7752 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py
--rw-r--r--   0 root         (0) root         (0)    14567 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.598918 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/
--rw-r--r--   0 root         (0) root         (0)      662 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6270 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py
--rw-r--r--   0 root         (0) root         (0)     3619 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py
--rw-r--r--   0 root         (0) root         (0)     9682 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py
--rw-r--r--   0 root         (0) root         (0)    15301 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py
--rw-r--r--   0 root         (0) root         (0)    25851 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/tf_utils/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.599918 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/bf16_convert.py
--rw-r--r--   0 root         (0) root         (0)    25631 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/hawq_metric.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)     5472 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/model_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7127 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/pattern_detector.py
--rw-r--r--   0 root         (0) root         (0)    43673 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/symbolic_trace.py
--rw-r--r--   0 root         (0) root         (0)    38166 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/adaptor/torch_utils/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.600918 neural_compressor-2.2/neural_compressor/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/algorithm/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/algorithm/fast_bias_correction.py
--rw-r--r--   0 root         (0) root         (0)     3590 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/algorithm/smooth_quant.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/algorithm/weight_correction.py
--rw-r--r--   0 root         (0) root         (0)    22632 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.600918 neural_compressor-2.2/neural_compressor/compression/
--rw-r--r--   0 root         (0) root         (0)      730 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19938 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.600918 neural_compressor-2.2/neural_compressor/compression/distillation/
--rw-r--r--   0 root         (0) root         (0)      656 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/distillation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65142 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/distillation/criterions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.602918 neural_compressor-2.2/neural_compressor/compression/pruner/
--rw-r--r--   0 root         (0) root         (0)      773 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12467 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/criteria.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.602918 neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5110 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/auto_slim.py
--rw-r--r--   0 root         (0) root         (0)    36319 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py
--rw-r--r--   0 root         (0) root         (0)    17870 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/weight_slim.py
--rw-r--r--   0 root         (0) root         (0)    69780 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/patterns.py
--rw-r--r--   0 root         (0) root         (0)    52361 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/pruners.py
--rw-r--r--   0 root         (0) root         (0)     5094 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/regs.py
--rw-r--r--   0 root         (0) root         (0)     6369 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/schedulers.py
--rw-r--r--   0 root         (0) root         (0)    24017 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/compression/pruner/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.603918 neural_compressor-2.2/neural_compressor/conf/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73446 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/conf/config.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/conf/dotdict.py
--rw-r--r--   0 root         (0) root         (0)    52392 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/conf/pythonic_config.py
--rw-r--r--   0 root         (0) root         (0)    88862 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.603918 neural_compressor-2.2/neural_compressor/contrib/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.603918 neural_compressor-2.2/neural_compressor/contrib/strategy/
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/contrib/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15661 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/contrib/strategy/sigopt.py
--rw-r--r--   0 root         (0) root         (0)    26054 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/contrib/strategy/tpe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.604918 neural_compressor-2.2/neural_compressor/data/
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.605918 neural_compressor-2.2/neural_compressor/data/dataloaders/
--rw-r--r--   0 root         (0) root         (0)      811 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4838 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/base_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6119 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/default_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4892 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/mxnet_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/onnxrt_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/pytorch_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     5097 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/sampler.py
--rw-r--r--   0 root         (0) root         (0)    14844 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/dataloaders/tensorflow_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.606918 neural_compressor-2.2/neural_compressor/data/datasets/
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19629 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    12251 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/coco_dataset.py
--rw-r--r--   0 root         (0) root         (0)    42946 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6584 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/dummy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13461 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/dummy_dataset_v2.py
--rw-r--r--   0 root         (0) root         (0)     9400 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/imagenet_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3650 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/datasets/style_transfer_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.607918 neural_compressor-2.2/neural_compressor/data/filters/
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/filters/coco_filter.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.607918 neural_compressor-2.2/neural_compressor/data/transforms/
--rw-r--r--   0 root         (0) root         (0)     1929 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/coco_transform.py
--rw-r--r--   0 root         (0) root         (0)    17692 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/imagenet_transform.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/postprocess.py
--rw-r--r--   0 root         (0) root         (0)    12109 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/tokenization.py
--rw-r--r--   0 root         (0) root         (0)   106309 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/data/transforms/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.609918 neural_compressor-2.2/neural_compressor/experimental/
--rw-r--r--   0 root         (0) root         (0)     1348 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30413 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.610918 neural_compressor-2.2/neural_compressor/experimental/common/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68967 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/criterion.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/metric.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/model.py
--rw-r--r--   0 root         (0) root         (0)     7839 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/optimizer.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/common/torch_utils.py
--rw-r--r--   0 root         (0) root         (0)    25100 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/component.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.611919 neural_compressor-2.2/neural_compressor/experimental/compression/
--rw-r--r--   0 root         (0) root         (0)      700 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5762 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/compression/pruning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.611919 neural_compressor-2.2/neural_compressor/experimental/contrib/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/contrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.611919 neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14075 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/sigopt.py
--rw-r--r--   0 root         (0) root         (0)    25727 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/tpe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.611919 neural_compressor-2.2/neural_compressor/experimental/data/
--rw-r--r--   0 root         (0) root         (0)     1269 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.613918 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/
--rw-r--r--   0 root         (0) root         (0)      836 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/base_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     1582 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6075 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/default_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/fetcher.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/sampler.py
--rw-r--r--   0 root         (0) root         (0)    14814 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.614919 neural_compressor-2.2/neural_compressor/experimental/data/datasets/
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19430 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/bert_dataset.py
--rw-r--r--   0 root         (0) root         (0)    12163 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/coco_dataset.py
--rw-r--r--   0 root         (0) root         (0)    42301 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/dataset.py
--rw-r--r--   0 root         (0) root         (0)     6561 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/dummy_dataset.py
--rw-r--r--   0 root         (0) root         (0)    13417 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py
--rw-r--r--   0 root         (0) root         (0)     9268 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/imagenet_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/datasets/style_transfer_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.614919 neural_compressor-2.2/neural_compressor/experimental/data/filters/
--rw-r--r--   0 root         (0) root         (0)     1045 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/filters/coco_filter.py
--rw-r--r--   0 root         (0) root         (0)     5962 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.615918 neural_compressor-2.2/neural_compressor/experimental/data/transforms/
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17489 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/transforms/imagenet_transform.py
--rw-r--r--   0 root         (0) root         (0)    12109 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/transforms/tokenization.py
--rw-r--r--   0 root         (0) root         (0)   106216 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/data/transforms/transform.py
--rw-r--r--   0 root         (0) root         (0)    22101 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/distillation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.615918 neural_compressor-2.2/neural_compressor/experimental/export/
--rw-r--r--   0 root         (0) root         (0)      834 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/export/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/export/qlinear2qdq.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/export/tf2onnx.py
--rw-r--r--   0 root         (0) root         (0)     8191 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/export/torch2onnx.py
--rw-r--r--   0 root         (0) root         (0)    20027 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/graph_optimization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.617919 neural_compressor-2.2/neural_compressor/experimental/metric/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4874 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/bleu.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/bleu_util.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/coco_label_map.py
--rw-r--r--   0 root         (0) root         (0)    32578 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/coco_tools.py
--rw-r--r--   0 root         (0) root         (0)     4339 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/evaluate_squad.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/f1.py
--rw-r--r--   0 root         (0) root         (0)    57878 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/metric/metric.py
--rw-r--r--   0 root         (0) root         (0)    10144 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)    15676 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/model_conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.617919 neural_compressor-2.2/neural_compressor/experimental/nas/
--rw-r--r--   0 root         (0) root         (0)      728 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6086 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/basic_nas.py
--rw-r--r--   0 root         (0) root         (0)     4022 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/dynas.py
--rw-r--r--   0 root         (0) root         (0)    15982 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/nas.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/nas_utils.py
--rw-r--r--   0 root         (0) root         (0)     5893 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/nas/search_algorithms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.618919 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/
--rw-r--r--   0 root         (0) root         (0)      995 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12216 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/group_lasso.py
--rw-r--r--   0 root         (0) root         (0)     4565 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/magnitude.py
--rw-r--r--   0 root         (0) root         (0)     2158 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/pattern_lock.py
--rw-r--r--   0 root         (0) root         (0)     4724 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/pruner.py
--rw-r--r--   0 root         (0) root         (0)    22318 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.618919 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.619919 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/pattern.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py
--rw-r--r--   0 root         (0) root         (0)    23225 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pruning_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.620919 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/
--rw-r--r--   0 root         (0) root         (0)      660 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/logger.py
--rw-r--r--   0 root         (0) root         (0)    24675 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/patterns.py
--rw-r--r--   0 root         (0) root         (0)     9285 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/prune_utils.py
--rw-r--r--   0 root         (0) root         (0)    12505 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/pruner.py
--rw-r--r--   0 root         (0) root         (0)     6382 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/pruning.py
--rw-r--r--   0 root         (0) root         (0)     5421 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/scheduler.py
--rw-r--r--   0 root         (0) root         (0)    22544 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/quantization.py
--rw-r--r--   0 root         (0) root         (0)    18510 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.621919 neural_compressor-2.2/neural_compressor/experimental/strategy/
--rw-r--r--   0 root         (0) root         (0)     1023 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7634 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/auto_mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)     9744 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/basic.py
--rw-r--r--   0 root         (0) root         (0)    15658 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/bayesian.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/exhaustive.py
--rw-r--r--   0 root         (0) root         (0)    10490 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/mse.py
--rw-r--r--   0 root         (0) root         (0)    11869 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/mse_v2.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/random.py
--rw-r--r--   0 root         (0) root         (0)    65327 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/strategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.622919 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)    22965 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_sampler.py
--rw-r--r--   0 root         (0) root         (0)    30566 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_space.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_structs.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/experimental/strategy/utils/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.623919 neural_compressor-2.2/neural_compressor/metric/
--rw-r--r--   0 root         (0) root         (0)     1281 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4874 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/bleu.py
--rw-r--r--   0 root         (0) root         (0)     5230 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/bleu_util.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/coco_label_map.py
--rw-r--r--   0 root         (0) root         (0)    32578 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/coco_tools.py
--rw-r--r--   0 root         (0) root         (0)     4339 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/evaluate_squad.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/f1.py
--rw-r--r--   0 root         (0) root         (0)    60811 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/metric/metric.py
--rw-r--r--   0 root         (0) root         (0)     7985 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/mix_precision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.624919 neural_compressor-2.2/neural_compressor/model/
--rw-r--r--   0 root         (0) root         (0)      800 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/base_model.py
--rw-r--r--   0 root         (0) root         (0)     4388 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/keras_model.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/model.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/mxnet_model.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/nets_factory.py
--rw-r--r--   0 root         (0) root         (0)    29905 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/onnx_model.py
--rw-r--r--   0 root         (0) root         (0)    48924 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/tensorflow_model.py
--rw-r--r--   0 root         (0) root         (0)    16394 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/model/torch_model.py
--rw-r--r--   0 root         (0) root         (0)    21247 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/objective.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.624919 neural_compressor-2.2/neural_compressor/profiling/
--rw-r--r--   0 root         (0) root         (0)      663 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.625919 neural_compressor-2.2/neural_compressor/profiling/parser/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.625919 neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/factory.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2202 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.626919 neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/factory.py
--rw-r--r--   0 root         (0) root         (0)     4345 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.626919 neural_compressor-2.2/neural_compressor/profiling/profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.627919 neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/profiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.627919 neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py
--rw-r--r--   0 root         (0) root         (0)     5470 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py
--rw-r--r--   0 root         (0) root         (0)    11891 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/quantization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.629919 neural_compressor-2.2/neural_compressor/strategy/
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4779 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/auto.py
--rw-r--r--   0 root         (0) root         (0)     8664 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/auto_mixed_precision.py
--rw-r--r--   0 root         (0) root         (0)    21817 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/basic.py
--rw-r--r--   0 root         (0) root         (0)    17120 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/bayesian.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/conservative.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/exhaustive.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/hawq_v2.py
--rw-r--r--   0 root         (0) root         (0)    12039 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/mse.py
--rw-r--r--   0 root         (0) root         (0)    11397 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/mse_v2.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/random.py
--rw-r--r--   0 root         (0) root         (0)    86097 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/strategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.630919 neural_compressor-2.2/neural_compressor/strategy/utils/
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)    27701 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/tuning_sampler.py
--rw-r--r--   0 root         (0) root         (0)    32824 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/tuning_space.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/tuning_structs.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/strategy/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)    21592 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/training.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.631919 neural_compressor-2.2/neural_compressor/utils/
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/collect_layer_histogram.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/constant.py
--rw-r--r--   0 root         (0) root         (0)     9668 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/create_obj_from_config.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/kl_divergence.py
--rw-r--r--   0 root         (0) root         (0)    11294 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/load_huggingface.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     4446 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/neural_insights_utils.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/options.py
--rw-r--r--   0 root         (0) root         (0)    18736 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/pytorch.py
--rw-r--r--   0 root         (0) root         (0)    35375 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/utils/weights_details.py
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-21 12:28:42.000000 neural_compressor-2.2/neural_compressor/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 12:28:59.575917 neural_compressor-2.2/neural_compressor.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11139 2023-06-21 12:28:59.000000 neural_compressor-2.2/neural_compressor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26940 2023-06-21 12:28:59.000000 neural_compressor-2.2/neural_compressor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 12:28:59.000000 neural_compressor-2.2/neural_compressor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-21 12:28:59.000000 neural_compressor-2.2/neural_compressor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-21 12:28:59.000000 neural_compressor-2.2/neural_compressor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 12:28:59.632919 neural_compressor-2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3720 2023-06-21 12:28:42.000000 neural_compressor-2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.581252 neural_compressor-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11360 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11141 2023-07-21 10:57:52.581252 neural_compressor-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10403 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.511249 neural_compressor-2.2.1/neural_coder/
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      668 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.518250 neural_compressor-2.2.1/neural_coder/backends/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/intel_extension_for_transformers.yaml
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/keras_inc.yaml
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_bf16_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_bf16_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_bf16_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_fp32_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_fp32_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_fp32_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)      849 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_gpu_to_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_int8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_onnxruntime_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_openvino_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/nano_openvino_int8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/onnx_inc_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/onnx_inc_static_quant_qdq.yaml
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml
+-rw-r--r--   0 root         (0) root         (0)      922 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_aliblade.yaml
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_benchmark.yaml
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_channels_last.yaml
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_fx.yaml
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_bf16.yaml
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_fp32.yaml
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_script.yaml
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_script_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_trace.yaml
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_trace_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)      860 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)      861 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_cuda.yaml
+-rw-r--r--   0 root         (0) root         (0)      843 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/backends/template.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.519250 neural_compressor-2.2.1/neural_coder/coders/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.519250 neural_compressor-2.2.1/neural_coder/coders/autoinc/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/autoinc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26057 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/autoinc/autoinc_harness.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/autoinc/calib_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/autoinc/domain.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/autoinc/eval_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.520250 neural_compressor-2.2.1/neural_coder/coders/pytorch/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/batch_size.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py
+-rw-r--r--   0 root         (0) root         (0)     2992 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/cuda_to_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    23101 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/harness.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/lightning.py
+-rw-r--r--   0 root         (0) root         (0)     3667 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     5291 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/pytorch/reclaim_inputs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.521250 neural_compressor-2.2.1/neural_coder/coders/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/tensorflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/tensorflow/amp.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/tensorflow/inc.py
+-rw-r--r--   0 root         (0) root         (0)     3716 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/coders/transform.py
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.521250 neural_compressor-2.2.1/neural_coder/graphers/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11123 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/code_line.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/function.py
+-rw-r--r--   0 root         (0) root         (0)    12402 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.522250 neural_compressor-2.2.1/neural_coder/graphers/preloads/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/preloads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58208 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/graphers/preloads/transformers.yaml
+-rw-r--r--   0 root         (0) root         (0)    52440 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/interface.py
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.523250 neural_compressor-2.2.1/neural_coder/utils/
+-rw-r--r--   0 root         (0) root         (0)      583 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      900 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/cpu_info.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/device.py
+-rw-r--r--   0 root         (0) root         (0)     7527 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/handle_user_input.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/line_operation.py
+-rw-r--r--   0 root         (0) root         (0)    38671 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/numa_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    18664 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/utils/pdf_report.py
+-rw-r--r--   0 root         (0) root         (0)      604 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_coder/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.524250 neural_compressor-2.2.1/neural_compressor/
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.528250 neural_compressor-2.2.1/neural_compressor/adaptor/
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/adaptor.py
+-rw-r--r--   0 root         (0) root         (0)    45064 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.528250 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/dense.py
+-rw-r--r--   0 root         (0) root         (0)     4456 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/pool2d.py
+-rw-r--r--   0 root         (0) root         (0)     3950 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/separable_conv2d.py
+-rw-r--r--   0 root         (0) root         (0)    22316 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/mxnet.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/mxnet.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.529250 neural_compressor-2.2.1/neural_compressor/adaptor/mxnet_utils/
+-rw-r--r--   0 root         (0) root         (0)      655 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/mxnet_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31176 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/mxnet_utils/util.py
+-rw-r--r--   0 root         (0) root         (0)    77117 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt.py
+-rw-r--r--   0 root         (0) root         (0)    15262 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt.yaml
+-rw-r--r--   0 root         (0) root         (0)    15699 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt_cuda.yaml
+-rw-r--r--   0 root         (0) root         (0)     4872 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt_trt.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.530250 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36485 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/calibration.py
+-rw-r--r--   0 root         (0) root         (0)    15844 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/calibrator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.533250 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5434 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/activation.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/argmax.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/attention.py
+-rw-r--r--   0 root         (0) root         (0)     5475 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/binary_op.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/concat.py
+-rw-r--r--   0 root         (0) root         (0)    10775 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/conv.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/direct_q8.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py
+-rw-r--r--   0 root         (0) root         (0)     5694 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gather.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gavgpool.py
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gemm.py
+-rw-r--r--   0 root         (0) root         (0)     5776 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/lstm.py
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/matmul.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/maxpool.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/norm.py
+-rw-r--r--   0 root         (0) root         (0)     5638 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/ops.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/pad.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/reduce.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/resize.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/split.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/unary_op.py
+-rw-r--r--   0 root         (0) root         (0)    61182 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/quantizer.py
+-rw-r--r--   0 root         (0) root         (0)    30141 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)    20482 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/util.py
+-rw-r--r--   0 root         (0) root         (0)   220311 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)    15795 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_cpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_gpu.yaml
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_ipex.yaml
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/query.py
+-rw-r--r--   0 root         (0) root         (0)   113916 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     9968 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow.yaml
+-rw-r--r--   0 root         (0) root         (0)     6941 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow_itex.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.534250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42716 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_converter.py
+-rw-r--r--   0 root         (0) root         (0)    16274 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.534250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/
+-rw-r--r--   0 root         (0) root         (0)      665 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.535250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13846 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.540250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dequantize_cast_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py
+-rw-r--r--   0 root         (0) root         (0)     5522 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3912 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py
+-rw-r--r--   0 root         (0) root         (0)    13288 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py
+-rw-r--r--   0 root         (0) root         (0)    17017 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py
+-rw-r--r--   0 root         (0) root         (0)    16070 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py
+-rw-r--r--   0 root         (0) root         (0)     9885 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5588 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py
+-rw-r--r--   0 root         (0) root         (0)     5998 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py
+-rw-r--r--   0 root         (0) root         (0)    12728 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py
+-rw-r--r--   0 root         (0) root         (0)    13918 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.542250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/
+-rw-r--r--   0 root         (0) root         (0)      670 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py
+-rw-r--r--   0 root         (0) root         (0)    18210 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    39443 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     8188 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py
+-rw-r--r--   0 root         (0) root         (0)    41642 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py
+-rw-r--r--   0 root         (0) root         (0)     5409 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py
+-rw-r--r--   0 root         (0) root         (0)     5449 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py
+-rw-r--r--   0 root         (0) root         (0)    17254 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.542250 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55654 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py
+-rw-r--r--   0 root         (0) root         (0)    13537 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py
+-rw-r--r--   0 root         (0) root         (0)    22286 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.543251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37367 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    40440 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.544251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.545251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/
+-rw-r--r--   0 root         (0) root         (0)      670 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8721 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.546251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py
+-rw-r--r--   0 root         (0) root         (0)    10309 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.547251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/
+-rw-r--r--   0 root         (0) root         (0)      670 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13718 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py
+-rw-r--r--   0 root         (0) root         (0)    12386 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)   112996 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py
+-rw-r--r--   0 root         (0) root         (0)    27174 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py
+-rw-r--r--   0 root         (0) root         (0)     8266 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py
+-rw-r--r--   0 root         (0) root         (0)    55564 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py
+-rw-r--r--   0 root         (0) root         (0)     7074 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py
+-rw-r--r--   0 root         (0) root         (0)    39207 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py
+-rw-r--r--   0 root         (0) root         (0)    13443 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py
+-rw-r--r--   0 root         (0) root         (0)     4867 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py
+-rw-r--r--   0 root         (0) root         (0)    21256 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py
+-rw-r--r--   0 root         (0) root         (0)    17273 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py
+-rw-r--r--   0 root         (0) root         (0)    19188 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph_common.py
+-rw-r--r--   0 root         (0) root         (0)    10384 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py
+-rw-r--r--   0 root         (0) root         (0)     7752 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py
+-rw-r--r--   0 root         (0) root         (0)    14567 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.548251 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6270 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)     3619 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py
+-rw-r--r--   0 root         (0) root         (0)     9682 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py
+-rw-r--r--   0 root         (0) root         (0)    15301 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py
+-rw-r--r--   0 root         (0) root         (0)    25851 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.549251 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/bf16_convert.py
+-rw-r--r--   0 root         (0) root         (0)    25631 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/hawq_metric.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/model_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/pattern_detector.py
+-rw-r--r--   0 root         (0) root         (0)    43673 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/symbolic_trace.py
+-rw-r--r--   0 root         (0) root         (0)    38166 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.550251 neural_compressor-2.2.1/neural_compressor/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/algorithm/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/algorithm/fast_bias_correction.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/algorithm/smooth_quant.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/algorithm/weight_correction.py
+-rw-r--r--   0 root         (0) root         (0)    22632 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.550251 neural_compressor-2.2.1/neural_compressor/compression/
+-rw-r--r--   0 root         (0) root         (0)      730 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19938 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.550251 neural_compressor-2.2.1/neural_compressor/compression/distillation/
+-rw-r--r--   0 root         (0) root         (0)      656 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/distillation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65142 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/distillation/criterions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.551251 neural_compressor-2.2.1/neural_compressor/compression/pruner/
+-rw-r--r--   0 root         (0) root         (0)      773 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/criteria.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.552251 neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/auto_slim.py
+-rw-r--r--   0 root         (0) root         (0)    36319 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/weight_slim.py
+-rw-r--r--   0 root         (0) root         (0)    69780 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/patterns.py
+-rw-r--r--   0 root         (0) root         (0)    52361 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/pruners.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/regs.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/schedulers.py
+-rw-r--r--   0 root         (0) root         (0)    24017 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/compression/pruner/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.553251 neural_compressor-2.2.1/neural_compressor/conf/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73446 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/conf/config.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/conf/dotdict.py
+-rw-r--r--   0 root         (0) root         (0)    52392 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/conf/pythonic_config.py
+-rw-r--r--   0 root         (0) root         (0)    88862 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.553251 neural_compressor-2.2.1/neural_compressor/contrib/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.553251 neural_compressor-2.2.1/neural_compressor/contrib/strategy/
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/contrib/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/contrib/strategy/sigopt.py
+-rw-r--r--   0 root         (0) root         (0)    26054 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/contrib/strategy/tpe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.553251 neural_compressor-2.2.1/neural_compressor/data/
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.555251 neural_compressor-2.2.1/neural_compressor/data/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)      811 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/base_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6119 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/default_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4892 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/mxnet_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/onnxrt_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/pytorch_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/sampler.py
+-rw-r--r--   0 root         (0) root         (0)    14844 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/dataloaders/tensorflow_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.556251 neural_compressor-2.2.1/neural_compressor/data/datasets/
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19629 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    12251 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/coco_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    42946 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6584 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/dummy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13461 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/dummy_dataset_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9400 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/imagenet_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/datasets/style_transfer_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.556251 neural_compressor-2.2.1/neural_compressor/data/filters/
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/filters/coco_filter.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.557251 neural_compressor-2.2.1/neural_compressor/data/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2031 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/coco_transform.py
+-rw-r--r--   0 root         (0) root         (0)    17692 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/imagenet_transform.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)    12109 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)   106309 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/data/transforms/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.559251 neural_compressor-2.2.1/neural_compressor/experimental/
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30413 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.560251 neural_compressor-2.2.1/neural_compressor/experimental/common/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68967 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/criterion.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/metric.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/model.py
+-rw-r--r--   0 root         (0) root         (0)     7839 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/common/torch_utils.py
+-rw-r--r--   0 root         (0) root         (0)    25100 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/component.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.560251 neural_compressor-2.2.1/neural_compressor/experimental/compression/
+-rw-r--r--   0 root         (0) root         (0)      700 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5762 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/compression/pruning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.560251 neural_compressor-2.2.1/neural_compressor/experimental/contrib/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/contrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.561251 neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/
+-rw-r--r--   0 root         (0) root         (0)      972 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14075 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/sigopt.py
+-rw-r--r--   0 root         (0) root         (0)    25727 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/tpe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.561251 neural_compressor-2.2.1/neural_compressor/experimental/data/
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.562251 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/base_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/default_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/fetcher.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/sampler.py
+-rw-r--r--   0 root         (0) root         (0)    14814 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.563251 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19430 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/bert_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    12163 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/coco_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    42301 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6561 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dummy_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    13417 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9268 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/imagenet_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/style_transfer_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.564251 neural_compressor-2.2.1/neural_compressor/experimental/data/filters/
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/filters/coco_filter.py
+-rw-r--r--   0 root         (0) root         (0)     5962 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/filters/filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.564251 neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17489 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/imagenet_transform.py
+-rw-r--r--   0 root         (0) root         (0)    12109 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)   106216 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/transform.py
+-rw-r--r--   0 root         (0) root         (0)    22101 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/distillation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.565251 neural_compressor-2.2.1/neural_compressor/experimental/export/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/export/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/export/qlinear2qdq.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/export/tf2onnx.py
+-rw-r--r--   0 root         (0) root         (0)     8191 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/export/torch2onnx.py
+-rw-r--r--   0 root         (0) root         (0)    20027 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/graph_optimization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.566251 neural_compressor-2.2.1/neural_compressor/experimental/metric/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4874 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/bleu_util.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/coco_label_map.py
+-rw-r--r--   0 root         (0) root         (0)    32578 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/coco_tools.py
+-rw-r--r--   0 root         (0) root         (0)     4339 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/evaluate_squad.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/f1.py
+-rw-r--r--   0 root         (0) root         (0)    57878 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/metric/metric.py
+-rw-r--r--   0 root         (0) root         (0)    10144 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)    15676 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/model_conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.567252 neural_compressor-2.2.1/neural_compressor/experimental/nas/
+-rw-r--r--   0 root         (0) root         (0)      728 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6086 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/basic_nas.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/dynas.py
+-rw-r--r--   0 root         (0) root         (0)    15982 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/nas.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/nas_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/nas/search_algorithms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.568251 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/
+-rw-r--r--   0 root         (0) root         (0)      995 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12216 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/group_lasso.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/magnitude.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/pattern_lock.py
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/pruner.py
+-rw-r--r--   0 root         (0) root         (0)    22318 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.568251 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.568251 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/pattern.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    23225 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pruning_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.569252 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/logger.py
+-rw-r--r--   0 root         (0) root         (0)    24675 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/patterns.py
+-rw-r--r--   0 root         (0) root         (0)     9285 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/prune_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12505 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/pruner.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/pruning.py
+-rw-r--r--   0 root         (0) root         (0)     5421 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)    22544 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    18510 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.571252 neural_compressor-2.2.1/neural_compressor/experimental/strategy/
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7634 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/auto_mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/bayesian.py
+-rw-r--r--   0 root         (0) root         (0)     2137 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/exhaustive.py
+-rw-r--r--   0 root         (0) root         (0)    10490 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/mse.py
+-rw-r--r--   0 root         (0) root         (0)    11869 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/mse_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/random.py
+-rw-r--r--   0 root         (0) root         (0)    65327 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/strategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.571252 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)    22965 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    30566 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_space.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_structs.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.573252 neural_compressor-2.2.1/neural_compressor/metric/
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4874 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     5230 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/bleu_util.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/coco_label_map.py
+-rw-r--r--   0 root         (0) root         (0)    32578 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/coco_tools.py
+-rw-r--r--   0 root         (0) root         (0)     4339 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/evaluate_squad.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/f1.py
+-rw-r--r--   0 root         (0) root         (0)    60811 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/metric/metric.py
+-rw-r--r--   0 root         (0) root         (0)     7985 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/mix_precision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.574252 neural_compressor-2.2.1/neural_compressor/model/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     4388 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/keras_model.py
+-rw-r--r--   0 root         (0) root         (0)    11263 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/mxnet_model.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/nets_factory.py
+-rw-r--r--   0 root         (0) root         (0)    29905 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/onnx_model.py
+-rw-r--r--   0 root         (0) root         (0)    48924 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/tensorflow_model.py
+-rw-r--r--   0 root         (0) root         (0)    16394 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/model/torch_model.py
+-rw-r--r--   0 root         (0) root         (0)    21247 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/objective.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.574252 neural_compressor-2.2.1/neural_compressor/profiling/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.574252 neural_compressor-2.2.1/neural_compressor/profiling/parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.575252 neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/factory.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.575252 neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/factory.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.576252 neural_compressor-2.2.1/neural_compressor/profiling/profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.576252 neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/profiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.577252 neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py
+-rw-r--r--   0 root         (0) root         (0)     5470 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11891 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/quantization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.578252 neural_compressor-2.2.1/neural_compressor/strategy/
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4779 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/auto.py
+-rw-r--r--   0 root         (0) root         (0)     8664 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/auto_mixed_precision.py
+-rw-r--r--   0 root         (0) root         (0)    21817 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/basic.py
+-rw-r--r--   0 root         (0) root         (0)    17120 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/bayesian.py
+-rw-r--r--   0 root         (0) root         (0)    11122 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/conservative.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/exhaustive.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/hawq_v2.py
+-rw-r--r--   0 root         (0) root         (0)    12039 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/mse.py
+-rw-r--r--   0 root         (0) root         (0)    11397 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/mse_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/random.py
+-rw-r--r--   0 root         (0) root         (0)    86097 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/strategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.579252 neural_compressor-2.2.1/neural_compressor/strategy/utils/
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)    27701 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    32824 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_space.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_structs.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/strategy/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)    21592 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/training.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.581252 neural_compressor-2.2.1/neural_compressor/utils/
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/collect_layer_histogram.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/constant.py
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/create_obj_from_config.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/kl_divergence.py
+-rw-r--r--   0 root         (0) root         (0)    11294 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/load_huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     4446 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/neural_insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/options.py
+-rw-r--r--   0 root         (0) root         (0)    18736 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)    35375 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/utils/weights_details.py
+-rw-r--r--   0 root         (0) root         (0)      766 2023-07-21 10:57:22.000000 neural_compressor-2.2.1/neural_compressor/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 10:57:52.525250 neural_compressor-2.2.1/neural_compressor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11141 2023-07-21 10:57:52.000000 neural_compressor-2.2.1/neural_compressor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26940 2023-07-21 10:57:52.000000 neural_compressor-2.2.1/neural_compressor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 10:57:52.000000 neural_compressor-2.2.1/neural_compressor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-21 10:57:52.000000 neural_compressor-2.2.1/neural_compressor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-21 10:57:52.000000 neural_compressor-2.2.1/neural_compressor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 10:57:52.581252 neural_compressor-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3720 2023-07-21 10:57:23.000000 neural_compressor-2.2.1/setup.py
```

### Comparing `neural_compressor-2.2/LICENSE` & `neural_compressor-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/PKG-INFO` & `neural_compressor-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_compressor
-Version: 2.2
+Version: 2.2.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIA Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural_compressor-2.2/README.md` & `neural_compressor-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/__init__.py` & `neural_compressor-2.2.1/neural_coder/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/__main__.py` & `neural_compressor-2.2.1/neural_coder/__main__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/__init__.py` & `neural_compressor-2.2.1/neural_coder/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/intel_extension_for_transformers.yaml` & `neural_compressor-2.2.1/neural_coder/backends/intel_extension_for_transformers.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/keras_inc.yaml` & `neural_compressor-2.2.1/neural_coder/backends/keras_inc.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_bf16.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_bf16_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_bf16_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_bf16_ipex.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_bf16_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_bf16_ipex_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_bf16_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_fp32_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_fp32_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_fp32_ipex.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_fp32_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_fp32_ipex_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_fp32_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_gpu_to_cpu.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_gpu_to_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_int8.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_int8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_bf16.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_ipex.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_bf16_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_fp32.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_ipex.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_jit_fp32_ipex_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_onnxruntime_fp32.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_onnxruntime_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_onnxruntime_int8_qlinear.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_openvino_fp32.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_openvino_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/nano_openvino_int8.yaml` & `neural_compressor-2.2.1/neural_coder/backends/nano_openvino_int8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/onnx_inc_dynamic_quant.yaml` & `neural_compressor-2.2.1/neural_coder/backends/onnx_inc_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/onnx_inc_static_quant_qdq.yaml` & `neural_compressor-2.2.1/neural_coder/backends/onnx_inc_static_quant_qdq.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml` & `neural_compressor-2.2.1/neural_coder/backends/onnx_inc_static_quant_qlinear.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_aliblade.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_aliblade.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_benchmark.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_benchmark.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_channels_last.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_channels_last.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_bf16.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_dynamic_quant.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_dynamic_quant_fp8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_huggingface_optimum_dynamic.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_huggingface_optimum_static.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_fx.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_fx.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_fx_fp8.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_inc_static_quant_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_ipex_bf16.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_bf16.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_ipex_fp32.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_fp32.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_int8_dynamic_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_ipex_int8_static_quant.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_jit_script.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_script.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_jit_script_ofi.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_script_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_jit_trace.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_trace.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_jit_trace_ofi.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_jit_trace_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_cpu.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_cuda.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_cuda.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_mixed_precision_intel_gpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_script.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_script_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_trace.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml` & `neural_compressor-2.2.1/neural_coder/backends/pytorch_torchdynamo_jit_trace_ofi.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/backends/template.yaml` & `neural_compressor-2.2.1/neural_coder/backends/template.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/__init__.py` & `neural_compressor-2.2.1/neural_coder/coders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/autoinc/__init__.py` & `neural_compressor-2.2.1/neural_coder/coders/autoinc/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/autoinc/autoinc_harness.py` & `neural_compressor-2.2.1/neural_coder/coders/autoinc/autoinc_harness.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/autoinc/calib_dataloader.py` & `neural_compressor-2.2.1/neural_coder/coders/autoinc/calib_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/autoinc/domain.py` & `neural_compressor-2.2.1/neural_coder/coders/autoinc/domain.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/autoinc/eval_func.py` & `neural_compressor-2.2.1/neural_coder/coders/autoinc/eval_func.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/__init__.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/batch_size.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/batch_size.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/change_trainer_to_nlptrainer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/cuda_to_cpu.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/cuda_to_cpu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/dummy_dataloader.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/harness.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/harness.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/lightning.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/lightning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/reclaim_inference_transformers_trainer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/pytorch/reclaim_inputs.py` & `neural_compressor-2.2.1/neural_coder/coders/pytorch/reclaim_inputs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/tensorflow/__init__.py` & `neural_compressor-2.2.1/neural_coder/coders/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/tensorflow/amp.py` & `neural_compressor-2.2.1/neural_coder/coders/tensorflow/amp.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/tensorflow/inc.py` & `neural_compressor-2.2.1/neural_coder/coders/tensorflow/inc.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/coders/transform.py` & `neural_compressor-2.2.1/neural_coder/coders/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/globals.py` & `neural_compressor-2.2.1/neural_coder/globals.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/__init__.py` & `neural_compressor-2.2.1/neural_coder/graphers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/code_line.py` & `neural_compressor-2.2.1/neural_coder/graphers/code_line.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/function.py` & `neural_compressor-2.2.1/neural_coder/graphers/function.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/model.py` & `neural_compressor-2.2.1/neural_coder/graphers/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/preloads/__init__.py` & `neural_compressor-2.2.1/neural_coder/graphers/preloads/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/graphers/preloads/transformers.yaml` & `neural_compressor-2.2.1/neural_coder/graphers/preloads/transformers.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/interface.py` & `neural_compressor-2.2.1/neural_coder/interface.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/launcher.py` & `neural_compressor-2.2.1/neural_coder/launcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/__init__.py` & `neural_compressor-2.2.1/neural_coder/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/common.py` & `neural_compressor-2.2.1/neural_coder/utils/common.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/cpu_info.py` & `neural_compressor-2.2.1/neural_coder/utils/cpu_info.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/device.py` & `neural_compressor-2.2.1/neural_coder/utils/device.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/handle_user_input.py` & `neural_compressor-2.2.1/neural_coder/utils/handle_user_input.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/line_operation.py` & `neural_compressor-2.2.1/neural_coder/utils/line_operation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/numa_launcher.py` & `neural_compressor-2.2.1/neural_coder/utils/numa_launcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/utils/pdf_report.py` & `neural_compressor-2.2.1/neural_coder/utils/pdf_report.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_coder/version.py` & `neural_compressor-2.2.1/neural_coder/version.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/__init__.py` & `neural_compressor-2.2.1/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/adaptor.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/conv2d.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/dense.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/dense.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/pool2d.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/pool2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/quantizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/quantizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/keras_utils/separable_conv2d.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/keras_utils/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/mxnet.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/mxnet.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/mxnet.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/mxnet.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/mxnet_utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/mxnet_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/mxnet_utils/util.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/mxnet_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/onnxrt.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/onnxrt.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/onnxrt_cuda.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt_cuda.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/onnxrt_trt.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/onnxrt_trt.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/calibration.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/calibrator.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/calibrator.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/activation.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/activation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/argmax.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/argmax.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/attention.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/attention.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/binary_op.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/binary_op.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/concat.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/concat.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/conv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/direct_q8.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/direct_q8.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/embed_layernorm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gather.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gather.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gavgpool.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gavgpool.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/gemm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/gemm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/lstm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/lstm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/matmul.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/maxpool.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/maxpool.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/norm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/ops.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/ops.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/pad.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/pad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/pooling.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/reduce.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/reduce.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/resize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/resize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/split.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/split.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/operators/unary_op.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/operators/unary_op.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/quantizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/quantizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/smooth_quant.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/ox_utils/util.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/ox_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/pytorch.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/pytorch.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/pytorch_cpu.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_cpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/pytorch_gpu.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_gpu.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/pytorch_ipex.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/pytorch_ipex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/query.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/query.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tensorflow.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tensorflow.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tensorflow_itex.yaml` & `neural_compressor-2.2.1/neural_compressor/adaptor/tensorflow_itex.yaml`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_converter.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_converter_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/bf16/bf16_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_add_to_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_layout.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_nan_to_random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/convert_placeholder_to_const.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dequantize_cast_optimizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dequantize_cast_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dilated_contraction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/dummy_biasadd.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/expanddims_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fetch_weight_from_reshape.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fold_constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_biasadd_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_column_wise_mul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_conv_with_math.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_decomposed_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_gelu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_layer_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_pad_with_fp32_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/fuse_reshape_transpose.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/graph_cse_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/grappler_pass.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/insert_print_node.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/move_squeeze_after_relu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/pre_optimize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/remove_training_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/rename_batch_norm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/split_shared_input.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_equivalent_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/strip_unused_nodes.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/generic/switch_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_fake_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/freeze_value_without_calib.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_conv_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_redundant_dequantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/fuse_matmul_requantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/meta_op_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_hostconst_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/post_quantized_op_cse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/rnn_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/int8/scale_propagation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_node.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/onnx_schema.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/onnx/tf2onnx_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/insert_qdq_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/merge_duplicated_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_rewriter/qdq/share_qdq_y_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/graph_util.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/graph_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/fake_quantize.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_helper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/optimize_layer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_add.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_layers/quantize_layer_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qat/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_deconv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_in.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/fuse_qdq_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/qdq/optimize_qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_bn.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_concatv2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_conv.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_for_intel_cpu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_matmul.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph/quantize_graph_pooling.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/quantize_graph_common.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/quantize_graph_common.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/smooth_quant_calibration.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/smooth_quant_scaler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/tf2onnx_converter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/bias_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/graph_transform_base.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/insert_logging.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/transform_graph/rerange_quantized_concat.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/tf_utils/util.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/tf_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/bf16_convert.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/bf16_convert.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/hawq_metric.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/hawq_metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/mixed_precision.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/model_wrapper.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/pattern_detector.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/pattern_detector.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/smooth_quant.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/symbolic_trace.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/adaptor/torch_utils/util.py` & `neural_compressor-2.2.1/neural_compressor/adaptor/torch_utils/util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/algorithm/__init__.py` & `neural_compressor-2.2.1/neural_compressor/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/algorithm/algorithm.py` & `neural_compressor-2.2.1/neural_compressor/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/algorithm/fast_bias_correction.py` & `neural_compressor-2.2.1/neural_compressor/algorithm/fast_bias_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/algorithm/smooth_quant.py` & `neural_compressor-2.2.1/neural_compressor/algorithm/smooth_quant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/algorithm/weight_correction.py` & `neural_compressor-2.2.1/neural_compressor/algorithm/weight_correction.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/benchmark.py` & `neural_compressor-2.2.1/neural_compressor/benchmark.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/__init__.py` & `neural_compressor-2.2.1/neural_compressor/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/callbacks.py` & `neural_compressor-2.2.1/neural_compressor/compression/callbacks.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/distillation/__init__.py` & `neural_compressor-2.2.1/neural_compressor/compression/distillation/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/distillation/criterions.py` & `neural_compressor-2.2.1/neural_compressor/compression/distillation/criterions.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/__init__.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/criteria.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/criteria.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/__init__.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/auto_slim.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/auto_slim.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/pattern_analyzer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/model_slim/weight_slim.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/model_slim/weight_slim.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/patterns.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/patterns.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/pruners.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/pruners.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/regs.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/regs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/schedulers.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/schedulers.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/compression/pruner/utils.py` & `neural_compressor-2.2.1/neural_compressor/compression/pruner/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/conf/__init__.py` & `neural_compressor-2.2.1/neural_compressor/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/conf/config.py` & `neural_compressor-2.2.1/neural_compressor/conf/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/conf/dotdict.py` & `neural_compressor-2.2.1/neural_compressor/conf/dotdict.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/conf/pythonic_config.py` & `neural_compressor-2.2.1/neural_compressor/conf/pythonic_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/config.py` & `neural_compressor-2.2.1/neural_compressor/config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/contrib/__init__.py` & `neural_compressor-2.2.1/neural_compressor/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/contrib/strategy/__init__.py` & `neural_compressor-2.2.1/neural_compressor/contrib/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/contrib/strategy/sigopt.py` & `neural_compressor-2.2.1/neural_compressor/contrib/strategy/sigopt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/contrib/strategy/tpe.py` & `neural_compressor-2.2.1/neural_compressor/contrib/strategy/tpe.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/__init__.py` & `neural_compressor-2.2.1/neural_compressor/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/__init__.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/base_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/base_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/default_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/default_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/fetcher.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/fetcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/mxnet_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/mxnet_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/onnxrt_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/onnxrt_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/pytorch_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/pytorch_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/sampler.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/dataloaders/tensorflow_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/data/dataloaders/tensorflow_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/__init__.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/bert_dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/coco_dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/coco_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/dummy_dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/dummy_dataset_v2.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/dummy_dataset_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/imagenet_dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/datasets/style_transfer_dataset.py` & `neural_compressor-2.2.1/neural_compressor/data/datasets/style_transfer_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/filters/__init__.py` & `neural_compressor-2.2.1/neural_compressor/data/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/filters/coco_filter.py` & `neural_compressor-2.2.1/neural_compressor/data/filters/coco_filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/filters/filter.py` & `neural_compressor-2.2.1/neural_compressor/data/filters/filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/__init__.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/coco_transform.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/coco_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/imagenet_transform.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/imagenet_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/postprocess.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/postprocess.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/tokenization.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/tokenization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/data/transforms/transform.py` & `neural_compressor-2.2.1/neural_compressor/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/benchmark.py` & `neural_compressor-2.2.1/neural_compressor/experimental/benchmark.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/criterion.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/criterion.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/metric.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/model.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/optimizer.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/postprocess.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/postprocess.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/common/torch_utils.py` & `neural_compressor-2.2.1/neural_compressor/experimental/common/torch_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/component.py` & `neural_compressor-2.2.1/neural_compressor/experimental/component.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/compression/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/compression/pruning.py` & `neural_compressor-2.2.1/neural_compressor/experimental/compression/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/contrib/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/sigopt.py` & `neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/sigopt.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/contrib/strategy/tpe.py` & `neural_compressor-2.2.1/neural_compressor/experimental/contrib/strategy/tpe.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/base_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/base_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/default_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/default_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/fetcher.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/fetcher.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/mxnet_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/onnxrt_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/pytorch_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/sampler.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/dataloaders/tensorflow_dataloader.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/bert_dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/bert_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/coco_dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/coco_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/dummy_dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/dummy_dataset_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/imagenet_dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/datasets/style_transfer_dataset.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/datasets/style_transfer_dataset.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/filters/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/filters/coco_filter.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/filters/coco_filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/filters/filter.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/filters/filter.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/transforms/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/transforms/imagenet_transform.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/imagenet_transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/transforms/tokenization.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/tokenization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/data/transforms/transform.py` & `neural_compressor-2.2.1/neural_compressor/experimental/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/distillation.py` & `neural_compressor-2.2.1/neural_compressor/experimental/distillation.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/export/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/export/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/export/qlinear2qdq.py` & `neural_compressor-2.2.1/neural_compressor/experimental/export/qlinear2qdq.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/export/tf2onnx.py` & `neural_compressor-2.2.1/neural_compressor/experimental/export/tf2onnx.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/export/torch2onnx.py` & `neural_compressor-2.2.1/neural_compressor/experimental/export/torch2onnx.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/graph_optimization.py` & `neural_compressor-2.2.1/neural_compressor/experimental/graph_optimization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/bleu.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/bleu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/bleu_util.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/bleu_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/coco_label_map.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/coco_label_map.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/coco_tools.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/coco_tools.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/evaluate_squad.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/evaluate_squad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/f1.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/f1.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/metric/metric.py` & `neural_compressor-2.2.1/neural_compressor/experimental/metric/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/mixed_precision.py` & `neural_compressor-2.2.1/neural_compressor/experimental/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/model_conversion.py` & `neural_compressor-2.2.1/neural_compressor/experimental/model_conversion.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/basic_nas.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/basic_nas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/dynas.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/dynas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/nas.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/nas.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/nas_utils.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/nas_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/nas/search_algorithms.py` & `neural_compressor-2.2.1/neural_compressor/experimental/nas/search_algorithms.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/gradient_sensitivity.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/group_lasso.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/group_lasso.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/magnitude.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/magnitude.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/pattern_lock.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/pattern_lock.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruner_legacy/pruner.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruner_legacy/pruner.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/pattern.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning_recipes/patterns/tile_pattern.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pruning_v2.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pruning_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/logger.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/patterns.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/patterns.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/prune_utils.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/prune_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/pruner.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/pruner.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/pruning.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/pruning.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/pytorch_pruner/scheduler.py` & `neural_compressor-2.2.1/neural_compressor/experimental/pytorch_pruner/scheduler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/quantization.py` & `neural_compressor-2.2.1/neural_compressor/experimental/quantization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/scheduler.py` & `neural_compressor-2.2.1/neural_compressor/experimental/scheduler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/auto_mixed_precision.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/auto_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/basic.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/bayesian.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/bayesian.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/exhaustive.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/exhaustive.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/mse.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/mse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/mse_v2.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/mse_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/random.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/strategy.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/constant.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_sampler.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_space.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_space.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/tuning_structs.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/tuning_structs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/experimental/strategy/utils/utility.py` & `neural_compressor-2.2.1/neural_compressor/experimental/strategy/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/__init__.py` & `neural_compressor-2.2.1/neural_compressor/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/bleu.py` & `neural_compressor-2.2.1/neural_compressor/metric/bleu.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/bleu_util.py` & `neural_compressor-2.2.1/neural_compressor/metric/bleu_util.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/coco_label_map.py` & `neural_compressor-2.2.1/neural_compressor/metric/coco_label_map.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/coco_tools.py` & `neural_compressor-2.2.1/neural_compressor/metric/coco_tools.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/evaluate_squad.py` & `neural_compressor-2.2.1/neural_compressor/metric/evaluate_squad.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/f1.py` & `neural_compressor-2.2.1/neural_compressor/metric/f1.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/metric/metric.py` & `neural_compressor-2.2.1/neural_compressor/metric/metric.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/mix_precision.py` & `neural_compressor-2.2.1/neural_compressor/mix_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/__init__.py` & `neural_compressor-2.2.1/neural_compressor/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/base_model.py` & `neural_compressor-2.2.1/neural_compressor/model/base_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/keras_model.py` & `neural_compressor-2.2.1/neural_compressor/model/keras_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/model.py` & `neural_compressor-2.2.1/neural_compressor/model/model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/mxnet_model.py` & `neural_compressor-2.2.1/neural_compressor/model/mxnet_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/nets_factory.py` & `neural_compressor-2.2.1/neural_compressor/model/nets_factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/onnx_model.py` & `neural_compressor-2.2.1/neural_compressor/model/onnx_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/tensorflow_model.py` & `neural_compressor-2.2.1/neural_compressor/model/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/model/torch_model.py` & `neural_compressor-2.2.1/neural_compressor/model/torch_model.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/objective.py` & `neural_compressor-2.2.1/neural_compressor/objective.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/onnx_parser/parser.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/onnx_parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/parser.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/result.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/result.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/parser/tensorflow_parser/parser.py` & `neural_compressor-2.2.1/neural_compressor/profiling/parser/tensorflow_parser/parser.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/onnxrt_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/profiler.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/factory.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py` & `neural_compressor-2.2.1/neural_compressor/profiling/profiler/tensorflow_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/quantization.py` & `neural_compressor-2.2.1/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/__init__.py` & `neural_compressor-2.2.1/neural_compressor/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/auto.py` & `neural_compressor-2.2.1/neural_compressor/strategy/auto.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/auto_mixed_precision.py` & `neural_compressor-2.2.1/neural_compressor/strategy/auto_mixed_precision.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/basic.py` & `neural_compressor-2.2.1/neural_compressor/strategy/basic.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/bayesian.py` & `neural_compressor-2.2.1/neural_compressor/strategy/bayesian.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/conservative.py` & `neural_compressor-2.2.1/neural_compressor/strategy/conservative.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/exhaustive.py` & `neural_compressor-2.2.1/neural_compressor/strategy/exhaustive.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/hawq_v2.py` & `neural_compressor-2.2.1/neural_compressor/strategy/hawq_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/mse.py` & `neural_compressor-2.2.1/neural_compressor/strategy/mse.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/mse_v2.py` & `neural_compressor-2.2.1/neural_compressor/strategy/mse_v2.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/random.py` & `neural_compressor-2.2.1/neural_compressor/strategy/random.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/strategy.py` & `neural_compressor-2.2.1/neural_compressor/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/constant.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/tuning_sampler.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/tuning_space.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_space.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/tuning_structs.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/tuning_structs.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/strategy/utils/utility.py` & `neural_compressor-2.2.1/neural_compressor/strategy/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/training.py` & `neural_compressor-2.2.1/neural_compressor/training.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/__init__.py` & `neural_compressor-2.2.1/neural_compressor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/collect_layer_histogram.py` & `neural_compressor-2.2.1/neural_compressor/utils/collect_layer_histogram.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/constant.py` & `neural_compressor-2.2.1/neural_compressor/utils/constant.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/create_obj_from_config.py` & `neural_compressor-2.2.1/neural_compressor/utils/create_obj_from_config.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/kl_divergence.py` & `neural_compressor-2.2.1/neural_compressor/utils/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/load_huggingface.py` & `neural_compressor-2.2.1/neural_compressor/utils/load_huggingface.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/logger.py` & `neural_compressor-2.2.1/neural_compressor/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/neural_insights_utils.py` & `neural_compressor-2.2.1/neural_compressor/utils/neural_insights_utils.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/options.py` & `neural_compressor-2.2.1/neural_compressor/utils/options.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/pytorch.py` & `neural_compressor-2.2.1/neural_compressor/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/utility.py` & `neural_compressor-2.2.1/neural_compressor/utils/utility.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/utils/weights_details.py` & `neural_compressor-2.2.1/neural_compressor/utils/weights_details.py`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/neural_compressor/version.py` & `neural_compressor-2.2.1/neural_compressor/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Intel® Neural Compressor: An open-source Python library supporting popular model compression techniques."""
-__version__ = "2.2"
+__version__ = "2.2.1"
```

### Comparing `neural_compressor-2.2/neural_compressor.egg-info/PKG-INFO` & `neural_compressor-2.2.1/neural_compressor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-compressor
-Version: 2.2
+Version: 2.2.1
 Summary: Repository of Intel® Neural Compressor
 Home-page: https://github.com/intel/neural-compressor
 Author: Intel AIA Team
 Author-email: feng.tian@intel.com, haihao.shen@intel.com, suyue.chen@intel.com
 License: Apache 2.0
 Keywords: quantization,auto-tuning,post-training static quantization,post-training dynamic quantization,quantization-aware training
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neural_compressor-2.2/neural_compressor.egg-info/SOURCES.txt` & `neural_compressor-2.2.1/neural_compressor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_compressor-2.2/setup.py` & `neural_compressor-2.2.1/setup.py`

 * *Files identical despite different names*

