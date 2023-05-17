# Comparing `tmp/olive_ai-0.1.0-py3-none-any.whl.zip` & `tmp/olive_ai-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,129 +1,210 @@
-Zip file size: 139307 bytes, number of entries: 127
--rw-rw-r--  2.0 unx      608 b- defN 23-Mar-24 00:27 olive/__init__.py
--rw-rw-r--  2.0 unx     4035 b- defN 23-Mar-24 00:27 olive/cache.py
--rw-rw-r--  2.0 unx      945 b- defN 23-Mar-24 00:27 olive/constants.py
--rw-rw-r--  2.0 unx    19004 b- defN 23-Mar-24 00:27 olive/engine.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Mar-24 00:27 olive/logging.py
--rw-rw-r--  2.0 unx    14118 b- defN 23-Mar-24 00:27 olive/model.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/common/__init__.py
--rw-rw-r--  2.0 unx     3453 b- defN 23-Mar-24 00:27 olive/common/auto_config.py
--rw-rw-r--  2.0 unx     6812 b- defN 23-Mar-24 00:27 olive/common/config_utils.py
--rw-rw-r--  2.0 unx     1468 b- defN 23-Mar-24 00:27 olive/common/import_lib.py
--rw-rw-r--  2.0 unx     1783 b- defN 23-Mar-24 00:27 olive/common/user_module_loader.py
--rw-rw-r--  2.0 unx     4527 b- defN 23-Mar-24 00:27 olive/common/utils.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/evaluator/__init__.py
--rw-rw-r--  2.0 unx     3356 b- defN 23-Mar-24 00:27 olive/evaluator/accuracy.py
--rw-rw-r--  2.0 unx    12347 b- defN 23-Mar-24 00:27 olive/evaluator/evaluation.py
--rw-rw-r--  2.0 unx     4787 b- defN 23-Mar-24 00:27 olive/evaluator/metric.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Mar-24 00:27 olive/evaluator/metric_config.py
--rw-rw-r--  2.0 unx     1787 b- defN 23-Mar-24 00:27 olive/evaluator/olive_evaluator.py
--rw-rw-r--  2.0 unx      575 b- defN 23-Mar-24 00:27 olive/passes/__init__.py
--rw-rw-r--  2.0 unx     9563 b- defN 23-Mar-24 00:27 olive/passes/olive_pass.py
--rw-rw-r--  2.0 unx     3770 b- defN 23-Mar-24 00:27 olive/passes/pass_config.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Mar-24 00:27 olive/passes/onnx/__init__.py
--rw-rw-r--  2.0 unx     6015 b- defN 23-Mar-24 00:27 olive/passes/onnx/conversion.py
--rw-rw-r--  2.0 unx     5261 b- defN 23-Mar-24 00:27 olive/passes/onnx/model_optimizer.py
--rw-rw-r--  2.0 unx    11199 b- defN 23-Mar-24 00:27 olive/passes/onnx/perf_tuning.py
--rw-rw-r--  2.0 unx    13072 b- defN 23-Mar-24 00:27 olive/passes/onnx/quantization.py
--rw-rw-r--  2.0 unx     3734 b- defN 23-Mar-24 00:27 olive/passes/onnx/transformer_optimization.py
--rw-rw-r--  2.0 unx      448 b- defN 23-Mar-24 00:27 olive/passes/openvino/__init__.py
--rw-rw-r--  2.0 unx     3676 b- defN 23-Mar-24 00:27 olive/passes/openvino/conversion.py
--rw-rw-r--  2.0 unx     4202 b- defN 23-Mar-24 00:27 olive/passes/openvino/quantization.py
--rw-rw-r--  2.0 unx      375 b- defN 23-Mar-24 00:27 olive/passes/pytorch/__init__.py
--rw-rw-r--  2.0 unx     7068 b- defN 23-Mar-24 00:27 olive/passes/pytorch/cluster.py
--rw-rw-r--  2.0 unx      974 b- defN 23-Mar-24 00:27 olive/passes/pytorch/pytorch_lightning_utils.py
--rw-rw-r--  2.0 unx     8154 b- defN 23-Mar-24 00:27 olive/passes/pytorch/qat_utils.py
--rw-rw-r--  2.0 unx     6237 b- defN 23-Mar-24 00:27 olive/passes/pytorch/quantization_aware_training.py
--rw-rw-r--  2.0 unx      501 b- defN 23-Mar-24 00:27 olive/passes/snpe/__init__.py
--rw-rw-r--  2.0 unx     4651 b- defN 23-Mar-24 00:27 olive/passes/snpe/conversion.py
--rw-rw-r--  2.0 unx     3491 b- defN 23-Mar-24 00:27 olive/passes/snpe/quantization.py
--rw-rw-r--  2.0 unx     2007 b- defN 23-Mar-24 00:27 olive/passes/snpe/snpe_to_onnx.py
--rw-rw-r--  2.0 unx      432 b- defN 23-Mar-24 00:27 olive/snpe/__init__.py
--rw-rw-r--  2.0 unx     2496 b- defN 23-Mar-24 00:27 olive/snpe/configure.py
--rw-rw-r--  2.0 unx     1079 b- defN 23-Mar-24 00:27 olive/snpe/constants.py
--rw-rw-r--  2.0 unx     1046 b- defN 23-Mar-24 00:27 olive/snpe/copy_libcdsprpc.ps1
--rw-rw-r--  2.0 unx     1142 b- defN 23-Mar-24 00:27 olive/snpe/create_python36_env.sh
--rw-rw-r--  2.0 unx     8306 b- defN 23-Mar-24 00:27 olive/snpe/data_loader.py
--rw-rw-r--  2.0 unx     3908 b- defN 23-Mar-24 00:27 olive/snpe/snpe.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/snpe/tools/__init__.py
--rw-rw-r--  2.0 unx    10335 b- defN 23-Mar-24 00:27 olive/snpe/tools/dev.py
--rw-rw-r--  2.0 unx    17791 b- defN 23-Mar-24 00:27 olive/snpe/tools/inference.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-24 00:27 olive/snpe/utils/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Mar-24 00:27 olive/snpe/utils/adb.py
--rw-rw-r--  2.0 unx     8643 b- defN 23-Mar-24 00:27 olive/snpe/utils/input_list.py
--rw-rw-r--  2.0 unx     4867 b- defN 23-Mar-24 00:27 olive/snpe/utils/local.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/strategy/__init__.py
--rw-rw-r--  2.0 unx     5563 b- defN 23-Mar-24 00:27 olive/strategy/search_parameter.py
--rw-rw-r--  2.0 unx     7415 b- defN 23-Mar-24 00:27 olive/strategy/search_results.py
--rw-rw-r--  2.0 unx     4654 b- defN 23-Mar-24 00:27 olive/strategy/search_space.py
--rw-rw-r--  2.0 unx    10002 b- defN 23-Mar-24 00:27 olive/strategy/search_strategy.py
--rw-rw-r--  2.0 unx     4076 b- defN 23-Mar-24 00:27 olive/strategy/utils.py
--rw-rw-r--  2.0 unx      598 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/__init__.py
--rw-rw-r--  2.0 unx     1153 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/exhaustive.py
--rw-rw-r--  2.0 unx     4070 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/optuna_sampler.py
--rw-rw-r--  2.0 unx     2480 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/random_sampler.py
--rw-rw-r--  2.0 unx     2307 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/search_algorithm.py
--rw-rw-r--  2.0 unx     1864 b- defN 23-Mar-24 00:27 olive/strategy/search_algorithm/tpe_sampler.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/systems/__init__.py
--rw-rw-r--  2.0 unx     2020 b- defN 23-Mar-24 00:27 olive/systems/common.py
--rw-rw-r--  2.0 unx     1743 b- defN 23-Mar-24 00:27 olive/systems/local.py
--rw-rw-r--  2.0 unx     1282 b- defN 23-Mar-24 00:27 olive/systems/olive_system.py
--rw-rw-r--  2.0 unx     2094 b- defN 23-Mar-24 00:27 olive/systems/system_config.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Mar-24 00:27 olive/systems/utils.py
--rw-rw-r--  2.0 unx      411 b- defN 23-Mar-24 00:27 olive/systems/azureml/__init__.py
--rw-rw-r--  2.0 unx     1968 b- defN 23-Mar-24 00:27 olive/systems/azureml/aml_evaluation_runner.py
--rw-rw-r--  2.0 unx     3844 b- defN 23-Mar-24 00:27 olive/systems/azureml/aml_pass_runner.py
--rw-rw-r--  2.0 unx    19463 b- defN 23-Mar-24 00:27 olive/systems/azureml/aml_system.py
--rw-rw-r--  2.0 unx      662 b- defN 23-Mar-24 00:27 olive/systems/docker/Dockerfile
--rw-rw-r--  2.0 unx      407 b- defN 23-Mar-24 00:27 olive/systems/docker/__init__.py
--rw-rw-r--  2.0 unx     6055 b- defN 23-Mar-24 00:27 olive/systems/docker/docker_system.py
--rw-rw-r--  2.0 unx     2196 b- defN 23-Mar-24 00:27 olive/systems/docker/eval.py
--rw-rw-r--  2.0 unx     4403 b- defN 23-Mar-24 00:27 olive/systems/docker/utils.py
--rw-rw-r--  2.0 unx      287 b- defN 23-Mar-24 00:27 olive/workflows/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/workflows/run/__init__.py
--rw-rw-r--  2.0 unx      540 b- defN 23-Mar-24 00:27 olive/workflows/run/__main__.py
--rw-rw-r--  2.0 unx     2971 b- defN 23-Mar-24 00:27 olive/workflows/run/config.py
--rw-rw-r--  2.0 unx     2661 b- defN 23-Mar-24 00:27 olive/workflows/run/run.py
--rw-rw-r--  2.0 unx      388 b- defN 23-Mar-24 00:27 olive/workflows/snpe/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/workflows/snpe/convertquantize/__init__.py
--rw-rw-r--  2.0 unx     1339 b- defN 23-Mar-24 00:27 olive/workflows/snpe/convertquantize/__main__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Mar-24 00:27 olive/workflows/snpe/convertquantize/convertquantize.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 olive/workflows/snpe/evaluate/__init__.py
--rw-rw-r--  2.0 unx      955 b- defN 23-Mar-24 00:27 olive/workflows/snpe/evaluate/__main__.py
--rw-rw-r--  2.0 unx     2854 b- defN 23-Mar-24 00:27 olive/workflows/snpe/evaluate/evaluate.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/integ_test/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/azureml_eval/__init__.py
--rw-rw-r--  2.0 unx     1650 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/azureml_eval/test_aml_evaluation.py
--rw-rw-r--  2.0 unx      555 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/azureml_eval/user_script.py
--rw-rw-r--  2.0 unx     4465 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/azureml_eval/utils.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/docker_eval/__init__.py
--rw-rw-r--  2.0 unx     2013 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/docker_eval/test_docker_evaluation.py
--rw-rw-r--  2.0 unx      646 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/docker_eval/user_script.py
--rw-rw-r--  2.0 unx     3760 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/docker_eval/utils.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/local_eval/__init__.py
--rw-rw-r--  2.0 unx     1750 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/local_eval/test_local_evaluation.py
--rw-rw-r--  2.0 unx     3518 b- defN 23-Mar-24 00:27 test/integ_test/evaluator/local_eval/utils.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/unit_test/__init__.py
--rw-rw-r--  2.0 unx      485 b- defN 23-Mar-24 00:27 test/unit_test/conftest.py
--rw-rw-r--  2.0 unx     2560 b- defN 23-Mar-24 00:27 test/unit_test/test_cache.py
--rw-rw-r--  2.0 unx     4500 b- defN 23-Mar-24 00:27 test/unit_test/test_engine.py
--rw-rw-r--  2.0 unx     2889 b- defN 23-Mar-24 00:27 test/unit_test/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Mar-24 00:27 test/unit_test/common/__init__.py
--rw-rw-r--  2.0 unx     3560 b- defN 23-Mar-24 00:27 test/unit_test/common/test_import_lib.py
--rw-rw-r--  2.0 unx     1247 b- defN 23-Mar-24 00:27 test/unit_test/common/test_retry.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/unit_test/evaluator/__init__.py
--rw-rw-r--  2.0 unx     3353 b- defN 23-Mar-24 00:27 test/unit_test/evaluator/test_accuracy.py
--rw-rw-r--  2.0 unx     4380 b- defN 23-Mar-24 00:27 test/unit_test/evaluator/test_evaluation.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/unit_test/systems/__init__.py
--rw-rw-r--  2.0 unx     3006 b- defN 23-Mar-24 00:27 test/unit_test/systems/test_local.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/unit_test/systems/azureml/__init__.py
--rw-rw-r--  2.0 unx    10706 b- defN 23-Mar-24 00:27 test/unit_test/systems/azureml/test_aml_system.py
--rw-rw-r--  2.0 unx      247 b- defN 23-Mar-24 00:27 test/unit_test/systems/docker/__init__.py
--rw-rw-r--  2.0 unx     7442 b- defN 23-Mar-24 00:27 test/unit_test/systems/docker/test_docker_system.py
--rw-rw-r--  2.0 unx     1141 b- defN 23-Mar-24 00:31 olive_ai-0.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2049 b- defN 23-Mar-24 00:31 olive_ai-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-24 00:31 olive_ai-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-24 00:31 olive_ai-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    11429 b- defN 23-Mar-24 00:31 olive_ai-0.1.0.dist-info/RECORD
-127 files, 434492 bytes uncompressed, 121063 bytes compressed:  72.1%
+Zip file size: 330328 bytes, number of entries: 208
+-rw-rw-r--  2.0 unx     1147 b- defN 23-May-17 12:12 olive/__init__.py
+-rw-rw-r--  2.0 unx     6064 b- defN 23-May-17 12:12 olive/cache.py
+-rw-rw-r--  2.0 unx      989 b- defN 23-May-17 12:12 olive/constants.py
+-rw-rw-r--  2.0 unx      469 b- defN 23-May-17 12:12 olive/extra_dependencies.json
+-rw-rw-r--  2.0 unx     3758 b- defN 23-May-17 12:12 olive/hf_utils.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-May-17 12:12 olive/logging.py
+-rw-rw-r--  2.0 unx    37681 b- defN 23-May-17 12:12 olive/model.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/azureml/__init__.py
+-rw-rw-r--  2.0 unx     3383 b- defN 23-May-17 12:12 olive/azureml/azureml_client.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/common/__init__.py
+-rw-rw-r--  2.0 unx     3453 b- defN 23-May-17 12:12 olive/common/auto_config.py
+-rw-rw-r--  2.0 unx     7158 b- defN 23-May-17 12:12 olive/common/config_utils.py
+-rw-rw-r--  2.0 unx     1468 b- defN 23-May-17 12:12 olive/common/import_lib.py
+-rw-rw-r--  2.0 unx     2809 b- defN 23-May-17 12:12 olive/common/ort_inference.py
+-rw-rw-r--  2.0 unx     1783 b- defN 23-May-17 12:12 olive/common/user_module_loader.py
+-rw-rw-r--  2.0 unx     5298 b- defN 23-May-17 12:12 olive/common/utils.py
+-rw-rw-r--  2.0 unx      345 b- defN 23-May-17 12:12 olive/data/__init__.py
+-rw-rw-r--  2.0 unx     7641 b- defN 23-May-17 12:12 olive/data/config.py
+-rw-rw-r--  2.0 unx     1452 b- defN 23-May-17 12:12 olive/data/constants.py
+-rw-rw-r--  2.0 unx     7887 b- defN 23-May-17 12:12 olive/data/registry.py
+-rw-rw-r--  2.0 unx      342 b- defN 23-May-17 12:12 olive/data/component/__init__.py
+-rw-rw-r--  2.0 unx     1595 b- defN 23-May-17 12:12 olive/data/component/dataloader.py
+-rw-rw-r--  2.0 unx     2398 b- defN 23-May-17 12:12 olive/data/component/load_dataset.py
+-rw-rw-r--  2.0 unx      948 b- defN 23-May-17 12:12 olive/data/component/post_process_data.py
+-rw-rw-r--  2.0 unx     2103 b- defN 23-May-17 12:12 olive/data/component/pre_process_data.py
+-rw-rw-r--  2.0 unx      318 b- defN 23-May-17 12:12 olive/data/container/__init__.py
+-rw-rw-r--  2.0 unx     2734 b- defN 23-May-17 12:12 olive/data/container/data_container.py
+-rw-rw-r--  2.0 unx     1044 b- defN 23-May-17 12:12 olive/data/container/huggingface_container.py
+-rw-rw-r--  2.0 unx      345 b- defN 23-May-17 12:12 olive/engine/__init__.py
+-rw-rw-r--  2.0 unx    35473 b- defN 23-May-17 12:12 olive/engine/engine.py
+-rw-rw-r--  2.0 unx    14347 b- defN 23-May-17 12:12 olive/engine/footprint.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/engine/packaging/__init__.py
+-rw-rw-r--  2.0 unx      598 b- defN 23-May-17 12:12 olive/engine/packaging/packaging_config.py
+-rw-rw-r--  2.0 unx    11341 b- defN 23-May-17 12:12 olive/engine/packaging/packaging_generator.py
+-rw-rw-r--  2.0 unx     1588 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
+-rw-rw-r--  2.0 unx     4990 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
+-rw-rw-r--  2.0 unx     1590 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/cs/README.md
+-rw-rw-r--  2.0 unx     4214 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
+-rw-rw-r--  2.0 unx     2304 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/python/README.md
+-rw-rw-r--  2.0 unx     2531 b- defN 23-May-17 12:12 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/evaluator/__init__.py
+-rw-rw-r--  2.0 unx     3386 b- defN 23-May-17 12:12 olive/evaluator/accuracy.py
+-rw-rw-r--  2.0 unx     4829 b- defN 23-May-17 12:12 olive/evaluator/metric.py
+-rw-rw-r--  2.0 unx     3255 b- defN 23-May-17 12:12 olive/evaluator/metric_config.py
+-rw-rw-r--  2.0 unx    18538 b- defN 23-May-17 12:12 olive/evaluator/olive_evaluator.py
+-rw-rw-r--  2.0 unx      575 b- defN 23-May-17 12:12 olive/passes/__init__.py
+-rw-rw-r--  2.0 unx    16976 b- defN 23-May-17 12:12 olive/passes/olive_pass.py
+-rw-rw-r--  2.0 unx     5315 b- defN 23-May-17 12:12 olive/passes/pass_config.py
+-rw-rw-r--  2.0 unx     1506 b- defN 23-May-17 12:12 olive/passes/onnx/__init__.py
+-rw-rw-r--  2.0 unx     4512 b- defN 23-May-17 12:12 olive/passes/onnx/append_pre_post_processing_ops.py
+-rw-rw-r--  2.0 unx     6086 b- defN 23-May-17 12:12 olive/passes/onnx/common.py
+-rw-rw-r--  2.0 unx     4818 b- defN 23-May-17 12:12 olive/passes/onnx/conversion.py
+-rw-rw-r--  2.0 unx     2861 b- defN 23-May-17 12:12 olive/passes/onnx/float16_conversion.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-May-17 12:12 olive/passes/onnx/inc_quantization.py
+-rw-rw-r--  2.0 unx     6355 b- defN 23-May-17 12:12 olive/passes/onnx/insert_beam_search.py
+-rw-rw-r--  2.0 unx     7114 b- defN 23-May-17 12:12 olive/passes/onnx/mixed_precision.py
+-rw-rw-r--  2.0 unx     5367 b- defN 23-May-17 12:12 olive/passes/onnx/model_optimizer.py
+-rw-rw-r--  2.0 unx    12799 b- defN 23-May-17 12:12 olive/passes/onnx/perf_tuning.py
+-rw-rw-r--  2.0 unx    20463 b- defN 23-May-17 12:12 olive/passes/onnx/quantization.py
+-rw-rw-r--  2.0 unx    11428 b- defN 23-May-17 12:12 olive/passes/onnx/transformer_optimization.py
+-rw-rw-r--  2.0 unx    11387 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai_quantization.py
+-rw-rw-r--  2.0 unx      449 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/calibrate.py
+-rw-rw-r--  2.0 unx     7724 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/qdq_quantizer.py
+-rw-rw-r--  2.0 unx     4044 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/quant_utils.py
+-rw-rw-r--  2.0 unx    10774 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/quantize.py
+-rw-rw-r--  2.0 unx    18375 b- defN 23-May-17 12:12 olive/passes/onnx/vitis_ai/refine.py
+-rw-rw-r--  2.0 unx      448 b- defN 23-May-17 12:12 olive/passes/openvino/__init__.py
+-rw-rw-r--  2.0 unx     3901 b- defN 23-May-17 12:12 olive/passes/openvino/conversion.py
+-rw-rw-r--  2.0 unx     4206 b- defN 23-May-17 12:12 olive/passes/openvino/quantization.py
+-rw-rw-r--  2.0 unx      375 b- defN 23-May-17 12:12 olive/passes/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     7068 b- defN 23-May-17 12:12 olive/passes/pytorch/cluster.py
+-rw-rw-r--  2.0 unx      974 b- defN 23-May-17 12:12 olive/passes/pytorch/pytorch_lightning_utils.py
+-rw-rw-r--  2.0 unx     8272 b- defN 23-May-17 12:12 olive/passes/pytorch/qat_utils.py
+-rw-rw-r--  2.0 unx     5827 b- defN 23-May-17 12:12 olive/passes/pytorch/quantization_aware_training.py
+-rw-rw-r--  2.0 unx      501 b- defN 23-May-17 12:12 olive/passes/snpe/__init__.py
+-rw-rw-r--  2.0 unx     4670 b- defN 23-May-17 12:12 olive/passes/snpe/conversion.py
+-rw-rw-r--  2.0 unx     3521 b- defN 23-May-17 12:12 olive/passes/snpe/quantization.py
+-rw-rw-r--  2.0 unx     2299 b- defN 23-May-17 12:12 olive/passes/snpe/snpe_to_onnx.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/passes/utils/__init__.py
+-rw-rw-r--  2.0 unx    10242 b- defN 23-May-17 12:12 olive/passes/utils/whisper_prepost.py
+-rw-rw-r--  2.0 unx      432 b- defN 23-May-17 12:12 olive/snpe/__init__.py
+-rw-rw-r--  2.0 unx     2496 b- defN 23-May-17 12:12 olive/snpe/configure.py
+-rw-rw-r--  2.0 unx     1079 b- defN 23-May-17 12:12 olive/snpe/constants.py
+-rw-rw-r--  2.0 unx     1046 b- defN 23-May-17 12:12 olive/snpe/copy_libcdsprpc.ps1
+-rw-rw-r--  2.0 unx     1142 b- defN 23-May-17 12:12 olive/snpe/create_python36_env.sh
+-rw-rw-r--  2.0 unx     8306 b- defN 23-May-17 12:12 olive/snpe/data_loader.py
+-rw-rw-r--  2.0 unx     3908 b- defN 23-May-17 12:12 olive/snpe/snpe.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/snpe/tools/__init__.py
+-rw-rw-r--  2.0 unx    10382 b- defN 23-May-17 12:12 olive/snpe/tools/dev.py
+-rw-rw-r--  2.0 unx    17791 b- defN 23-May-17 12:12 olive/snpe/tools/inference.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-17 12:12 olive/snpe/utils/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-May-17 12:12 olive/snpe/utils/adb.py
+-rw-rw-r--  2.0 unx     8643 b- defN 23-May-17 12:12 olive/snpe/utils/input_list.py
+-rw-rw-r--  2.0 unx     4867 b- defN 23-May-17 12:12 olive/snpe/utils/local.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/strategy/__init__.py
+-rw-rw-r--  2.0 unx    11885 b- defN 23-May-17 12:12 olive/strategy/search_parameter.py
+-rw-rw-r--  2.0 unx     5731 b- defN 23-May-17 12:12 olive/strategy/search_results.py
+-rw-rw-r--  2.0 unx     4876 b- defN 23-May-17 12:12 olive/strategy/search_space.py
+-rw-rw-r--  2.0 unx    10608 b- defN 23-May-17 12:12 olive/strategy/search_strategy.py
+-rw-rw-r--  2.0 unx     2911 b- defN 23-May-17 12:12 olive/strategy/utils.py
+-rw-rw-r--  2.0 unx      598 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/__init__.py
+-rw-rw-r--  2.0 unx     1153 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/exhaustive.py
+-rw-rw-r--  2.0 unx     4403 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/optuna_sampler.py
+-rw-rw-r--  2.0 unx     2498 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/random_sampler.py
+-rw-rw-r--  2.0 unx     2429 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/search_algorithm.py
+-rw-rw-r--  2.0 unx     1876 b- defN 23-May-17 12:12 olive/strategy/search_algorithm/tpe_sampler.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/systems/__init__.py
+-rw-rw-r--  2.0 unx     2079 b- defN 23-May-17 12:12 olive/systems/common.py
+-rw-rw-r--  2.0 unx     1535 b- defN 23-May-17 12:12 olive/systems/local.py
+-rw-rw-r--  2.0 unx     1192 b- defN 23-May-17 12:12 olive/systems/olive_system.py
+-rw-rw-r--  2.0 unx     3618 b- defN 23-May-17 12:12 olive/systems/system_config.py
+-rw-rw-r--  2.0 unx     1507 b- defN 23-May-17 12:12 olive/systems/utils.py
+-rw-rw-r--  2.0 unx      411 b- defN 23-May-17 12:12 olive/systems/azureml/__init__.py
+-rw-rw-r--  2.0 unx     2076 b- defN 23-May-17 12:12 olive/systems/azureml/aml_evaluation_runner.py
+-rw-rw-r--  2.0 unx     4179 b- defN 23-May-17 12:12 olive/systems/azureml/aml_pass_runner.py
+-rw-rw-r--  2.0 unx    21637 b- defN 23-May-17 12:12 olive/systems/azureml/aml_system.py
+-rw-rw-r--  2.0 unx      697 b- defN 23-May-17 12:12 olive/systems/docker/Dockerfile
+-rw-rw-r--  2.0 unx      407 b- defN 23-May-17 12:12 olive/systems/docker/__init__.py
+-rw-rw-r--  2.0 unx      651 b- defN 23-May-17 12:12 olive/systems/docker/dev_mount_cleanup.py
+-rw-rw-r--  2.0 unx     7426 b- defN 23-May-17 12:12 olive/systems/docker/docker_system.py
+-rw-rw-r--  2.0 unx     1776 b- defN 23-May-17 12:12 olive/systems/docker/eval.py
+-rw-rw-r--  2.0 unx     5352 b- defN 23-May-17 12:12 olive/systems/docker/utils.py
+-rw-rw-r--  2.0 unx      381 b- defN 23-May-17 12:12 olive/systems/python_environment/__init__.py
+-rw-rw-r--  2.0 unx      874 b- defN 23-May-17 12:12 olive/systems/python_environment/available_eps.py
+-rw-rw-r--  2.0 unx     4050 b- defN 23-May-17 12:12 olive/systems/python_environment/inference_runner.py
+-rw-rw-r--  2.0 unx     1485 b- defN 23-May-17 12:12 olive/systems/python_environment/is_valid_ep.py
+-rw-rw-r--  2.0 unx    11513 b- defN 23-May-17 12:12 olive/systems/python_environment/python_environment_system.py
+-rw-rw-r--  2.0 unx      287 b- defN 23-May-17 12:12 olive/workflows/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/workflows/run/__init__.py
+-rw-rw-r--  2.0 unx      634 b- defN 23-May-17 12:12 olive/workflows/run/__main__.py
+-rw-rw-r--  2.0 unx     7204 b- defN 23-May-17 12:12 olive/workflows/run/config.py
+-rw-rw-r--  2.0 unx     6319 b- defN 23-May-17 12:12 olive/workflows/run/run.py
+-rw-rw-r--  2.0 unx      388 b- defN 23-May-17 12:12 olive/workflows/snpe/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/workflows/snpe/convertquantize/__init__.py
+-rw-rw-r--  2.0 unx     1339 b- defN 23-May-17 12:12 olive/workflows/snpe/convertquantize/__main__.py
+-rw-rw-r--  2.0 unx     4322 b- defN 23-May-17 12:12 olive/workflows/snpe/convertquantize/convertquantize.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 olive/workflows/snpe/evaluate/__init__.py
+-rw-rw-r--  2.0 unx      955 b- defN 23-May-17 12:12 olive/workflows/snpe/evaluate/__main__.py
+-rw-rw-r--  2.0 unx     2879 b- defN 23-May-17 12:12 olive/workflows/snpe/evaluate/evaluate.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/integ_test/__init__.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-17 12:12 test/integ_test/evaluator/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/integ_test/evaluator/azureml_eval/__init__.py
+-rw-rw-r--  2.0 unx     1587 b- defN 23-May-17 12:12 test/integ_test/evaluator/azureml_eval/test_aml_evaluation.py
+-rw-rw-r--  2.0 unx      555 b- defN 23-May-17 12:12 test/integ_test/evaluator/azureml_eval/user_script.py
+-rw-rw-r--  2.0 unx     4649 b- defN 23-May-17 12:12 test/integ_test/evaluator/azureml_eval/utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/integ_test/evaluator/docker_eval/__init__.py
+-rw-rw-r--  2.0 unx     2141 b- defN 23-May-17 12:12 test/integ_test/evaluator/docker_eval/test_docker_evaluation.py
+-rw-rw-r--  2.0 unx     1787 b- defN 23-May-17 12:12 test/integ_test/evaluator/docker_eval/user_script.py
+-rw-rw-r--  2.0 unx     4033 b- defN 23-May-17 12:12 test/integ_test/evaluator/docker_eval/utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/integ_test/evaluator/local_eval/__init__.py
+-rw-rw-r--  2.0 unx     1942 b- defN 23-May-17 12:12 test/integ_test/evaluator/local_eval/test_local_evaluation.py
+-rw-rw-r--  2.0 unx     5153 b- defN 23-May-17 12:12 test/integ_test/evaluator/local_eval/utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/__init__.py
+-rw-rw-r--  2.0 unx      549 b- defN 23-May-17 12:12 test/unit_test/conftest.py
+-rw-rw-r--  2.0 unx     4266 b- defN 23-May-17 12:12 test/unit_test/test_cache.py
+-rw-rw-r--  2.0 unx     5840 b- defN 23-May-17 12:12 test/unit_test/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-17 12:12 test/unit_test/common/__init__.py
+-rw-rw-r--  2.0 unx     3560 b- defN 23-May-17 12:12 test/unit_test/common/test_import_lib.py
+-rw-rw-r--  2.0 unx     1247 b- defN 23-May-17 12:12 test/unit_test/common/test_retry.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/data_container/__init__.py
+-rw-rw-r--  2.0 unx     1266 b- defN 23-May-17 12:12 test/unit_test/data_container/test_config.py
+-rw-rw-r--  2.0 unx     1899 b- defN 23-May-17 12:12 test/unit_test/data_container/test_data_container.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-17 12:12 test/unit_test/engine/__init__.py
+-rw-rw-r--  2.0 unx    12138 b- defN 23-May-17 12:12 test/unit_test/engine/test_engine.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-May-17 12:12 test/unit_test/engine/test_footprint.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/engine/packaging/__init__.py
+-rw-rw-r--  2.0 unx     4141 b- defN 23-May-17 12:12 test/unit_test/engine/packaging/test_packaging_generator.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/evaluator/__init__.py
+-rw-rw-r--  2.0 unx     3348 b- defN 23-May-17 12:12 test/unit_test/evaluator/test_accuracy.py
+-rw-rw-r--  2.0 unx     4442 b- defN 23-May-17 12:12 test/unit_test/evaluator/test_olive_evaluator.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/hf_utils/__init__.py
+-rw-rw-r--  2.0 unx     1021 b- defN 23-May-17 12:12 test/unit_test/hf_utils/test_hf_utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/model/__init__.py
+-rw-rw-r--  2.0 unx     3040 b- defN 23-May-17 12:12 test/unit_test/model/test_pytorch_model.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/common/__init__.py
+-rw-rw-r--  2.0 unx     1353 b- defN 23-May-17 12:12 test/unit_test/passes/common/test_user_script.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/inc/__init__.py
+-rw-rw-r--  2.0 unx     4669 b- defN 23-May-17 12:12 test/unit_test/passes/inc/test_inc_quantization.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/__init__.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_insert_beam_search.py
+-rw-rw-r--  2.0 unx      632 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_mixed_precision.py
+-rw-rw-r--  2.0 unx      866 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_model_optimizer.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_perf_tuning.py
+-rw-rw-r--  2.0 unx     3327 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_pre_post_processing_op.py
+-rw-rw-r--  2.0 unx     2044 b- defN 23-May-17 12:12 test/unit_test/passes/onnx/test_transformer_optimization.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/openvino/__init__.py
+-rw-rw-r--  2.0 unx     2062 b- defN 23-May-17 12:12 test/unit_test/passes/openvino/test_openvino_conversion.py
+-rw-rw-r--  2.0 unx     4362 b- defN 23-May-17 12:12 test/unit_test/passes/openvino/test_openvino_quantization.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/pytorch/__init__.py
+-rw-rw-r--  2.0 unx      985 b- defN 23-May-17 12:12 test/unit_test/passes/pytorch/test_quantization_aware_training.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/passes/vitis_ai/__init__.py
+-rw-rw-r--  2.0 unx     2245 b- defN 23-May-17 12:12 test/unit_test/passes/vitis_ai/test_vitis_ai_quantization.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/systems/__init__.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-May-17 12:12 test/unit_test/systems/test_local.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/systems/azureml/__init__.py
+-rw-rw-r--  2.0 unx    11185 b- defN 23-May-17 12:12 test/unit_test/systems/azureml/test_aml_system.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/systems/docker/__init__.py
+-rw-rw-r--  2.0 unx     7650 b- defN 23-May-17 12:12 test/unit_test/systems/docker/test_docker_system.py
+-rw-rw-r--  2.0 unx      247 b- defN 23-May-17 12:12 test/unit_test/systems/python_environment/__init__.py
+-rw-rw-r--  2.0 unx     3625 b- defN 23-May-17 12:12 test/unit_test/systems/python_environment/test_python_environment_system.py
+-rw-rw-r--  2.0 unx     1141 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2700 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx   760804 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/NOTICE.txt
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    19492 b- defN 23-May-17 12:13 olive_ai-0.2.0.dist-info/RECORD
+208 files, 1570783 bytes uncompressed, 299002 bytes compressed:  81.0%
```

## zipnote {}

```diff
@@ -3,48 +3,129 @@
 
 Filename: olive/cache.py
 Comment: 
 
 Filename: olive/constants.py
 Comment: 
 
-Filename: olive/engine.py
+Filename: olive/extra_dependencies.json
+Comment: 
+
+Filename: olive/hf_utils.py
 Comment: 
 
 Filename: olive/logging.py
 Comment: 
 
 Filename: olive/model.py
 Comment: 
 
+Filename: olive/azureml/__init__.py
+Comment: 
+
+Filename: olive/azureml/azureml_client.py
+Comment: 
+
 Filename: olive/common/__init__.py
 Comment: 
 
 Filename: olive/common/auto_config.py
 Comment: 
 
 Filename: olive/common/config_utils.py
 Comment: 
 
 Filename: olive/common/import_lib.py
 Comment: 
 
+Filename: olive/common/ort_inference.py
+Comment: 
+
 Filename: olive/common/user_module_loader.py
 Comment: 
 
 Filename: olive/common/utils.py
 Comment: 
 
-Filename: olive/evaluator/__init__.py
+Filename: olive/data/__init__.py
 Comment: 
 
-Filename: olive/evaluator/accuracy.py
+Filename: olive/data/config.py
+Comment: 
+
+Filename: olive/data/constants.py
+Comment: 
+
+Filename: olive/data/registry.py
+Comment: 
+
+Filename: olive/data/component/__init__.py
+Comment: 
+
+Filename: olive/data/component/dataloader.py
+Comment: 
+
+Filename: olive/data/component/load_dataset.py
+Comment: 
+
+Filename: olive/data/component/post_process_data.py
 Comment: 
 
-Filename: olive/evaluator/evaluation.py
+Filename: olive/data/component/pre_process_data.py
+Comment: 
+
+Filename: olive/data/container/__init__.py
+Comment: 
+
+Filename: olive/data/container/data_container.py
+Comment: 
+
+Filename: olive/data/container/huggingface_container.py
+Comment: 
+
+Filename: olive/engine/__init__.py
+Comment: 
+
+Filename: olive/engine/engine.py
+Comment: 
+
+Filename: olive/engine/footprint.py
+Comment: 
+
+Filename: olive/engine/packaging/__init__.py
+Comment: 
+
+Filename: olive/engine/packaging/packaging_config.py
+Comment: 
+
+Filename: olive/engine/packaging/packaging_generator.py
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/cs/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/python/README.md
+Comment: 
+
+Filename: olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
+Comment: 
+
+Filename: olive/evaluator/__init__.py
+Comment: 
+
+Filename: olive/evaluator/accuracy.py
 Comment: 
 
 Filename: olive/evaluator/metric.py
 Comment: 
 
 Filename: olive/evaluator/metric_config.py
 Comment: 
@@ -60,29 +141,68 @@
 
 Filename: olive/passes/pass_config.py
 Comment: 
 
 Filename: olive/passes/onnx/__init__.py
 Comment: 
 
+Filename: olive/passes/onnx/append_pre_post_processing_ops.py
+Comment: 
+
+Filename: olive/passes/onnx/common.py
+Comment: 
+
 Filename: olive/passes/onnx/conversion.py
 Comment: 
 
+Filename: olive/passes/onnx/float16_conversion.py
+Comment: 
+
+Filename: olive/passes/onnx/inc_quantization.py
+Comment: 
+
+Filename: olive/passes/onnx/insert_beam_search.py
+Comment: 
+
+Filename: olive/passes/onnx/mixed_precision.py
+Comment: 
+
 Filename: olive/passes/onnx/model_optimizer.py
 Comment: 
 
 Filename: olive/passes/onnx/perf_tuning.py
 Comment: 
 
 Filename: olive/passes/onnx/quantization.py
 Comment: 
 
 Filename: olive/passes/onnx/transformer_optimization.py
 Comment: 
 
+Filename: olive/passes/onnx/vitis_ai_quantization.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/__init__.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/calibrate.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/qdq_quantizer.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/quant_utils.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/quantize.py
+Comment: 
+
+Filename: olive/passes/onnx/vitis_ai/refine.py
+Comment: 
+
 Filename: olive/passes/openvino/__init__.py
 Comment: 
 
 Filename: olive/passes/openvino/conversion.py
 Comment: 
 
 Filename: olive/passes/openvino/quantization.py
@@ -111,14 +231,20 @@
 
 Filename: olive/passes/snpe/quantization.py
 Comment: 
 
 Filename: olive/passes/snpe/snpe_to_onnx.py
 Comment: 
 
+Filename: olive/passes/utils/__init__.py
+Comment: 
+
+Filename: olive/passes/utils/whisper_prepost.py
+Comment: 
+
 Filename: olive/snpe/__init__.py
 Comment: 
 
 Filename: olive/snpe/configure.py
 Comment: 
 
 Filename: olive/snpe/constants.py
@@ -225,23 +351,41 @@
 
 Filename: olive/systems/docker/Dockerfile
 Comment: 
 
 Filename: olive/systems/docker/__init__.py
 Comment: 
 
+Filename: olive/systems/docker/dev_mount_cleanup.py
+Comment: 
+
 Filename: olive/systems/docker/docker_system.py
 Comment: 
 
 Filename: olive/systems/docker/eval.py
 Comment: 
 
 Filename: olive/systems/docker/utils.py
 Comment: 
 
+Filename: olive/systems/python_environment/__init__.py
+Comment: 
+
+Filename: olive/systems/python_environment/available_eps.py
+Comment: 
+
+Filename: olive/systems/python_environment/inference_runner.py
+Comment: 
+
+Filename: olive/systems/python_environment/is_valid_ep.py
+Comment: 
+
+Filename: olive/systems/python_environment/python_environment_system.py
+Comment: 
+
 Filename: olive/workflows/__init__.py
 Comment: 
 
 Filename: olive/workflows/run/__init__.py
 Comment: 
 
 Filename: olive/workflows/run/__main__.py
@@ -318,36 +462,126 @@
 
 Filename: test/unit_test/conftest.py
 Comment: 
 
 Filename: test/unit_test/test_cache.py
 Comment: 
 
-Filename: test/unit_test/test_engine.py
-Comment: 
-
 Filename: test/unit_test/utils.py
 Comment: 
 
 Filename: test/unit_test/common/__init__.py
 Comment: 
 
 Filename: test/unit_test/common/test_import_lib.py
 Comment: 
 
 Filename: test/unit_test/common/test_retry.py
 Comment: 
 
+Filename: test/unit_test/data_container/__init__.py
+Comment: 
+
+Filename: test/unit_test/data_container/test_config.py
+Comment: 
+
+Filename: test/unit_test/data_container/test_data_container.py
+Comment: 
+
+Filename: test/unit_test/engine/__init__.py
+Comment: 
+
+Filename: test/unit_test/engine/test_engine.py
+Comment: 
+
+Filename: test/unit_test/engine/test_footprint.py
+Comment: 
+
+Filename: test/unit_test/engine/packaging/__init__.py
+Comment: 
+
+Filename: test/unit_test/engine/packaging/test_packaging_generator.py
+Comment: 
+
 Filename: test/unit_test/evaluator/__init__.py
 Comment: 
 
 Filename: test/unit_test/evaluator/test_accuracy.py
 Comment: 
 
-Filename: test/unit_test/evaluator/test_evaluation.py
+Filename: test/unit_test/evaluator/test_olive_evaluator.py
+Comment: 
+
+Filename: test/unit_test/hf_utils/__init__.py
+Comment: 
+
+Filename: test/unit_test/hf_utils/test_hf_utils.py
+Comment: 
+
+Filename: test/unit_test/model/__init__.py
+Comment: 
+
+Filename: test/unit_test/model/test_pytorch_model.py
+Comment: 
+
+Filename: test/unit_test/passes/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/common/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/common/test_user_script.py
+Comment: 
+
+Filename: test/unit_test/passes/inc/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/inc/test_inc_quantization.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_insert_beam_search.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_mixed_precision.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_model_optimizer.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_perf_tuning.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_pre_post_processing_op.py
+Comment: 
+
+Filename: test/unit_test/passes/onnx/test_transformer_optimization.py
+Comment: 
+
+Filename: test/unit_test/passes/openvino/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/openvino/test_openvino_conversion.py
+Comment: 
+
+Filename: test/unit_test/passes/openvino/test_openvino_quantization.py
+Comment: 
+
+Filename: test/unit_test/passes/pytorch/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/pytorch/test_quantization_aware_training.py
+Comment: 
+
+Filename: test/unit_test/passes/vitis_ai/__init__.py
+Comment: 
+
+Filename: test/unit_test/passes/vitis_ai/test_vitis_ai_quantization.py
 Comment: 
 
 Filename: test/unit_test/systems/__init__.py
 Comment: 
 
 Filename: test/unit_test/systems/test_local.py
 Comment: 
@@ -360,23 +594,32 @@
 
 Filename: test/unit_test/systems/docker/__init__.py
 Comment: 
 
 Filename: test/unit_test/systems/docker/test_docker_system.py
 Comment: 
 
-Filename: olive_ai-0.1.0.dist-info/LICENSE
+Filename: test/unit_test/systems/python_environment/__init__.py
+Comment: 
+
+Filename: test/unit_test/systems/python_environment/test_python_environment_system.py
+Comment: 
+
+Filename: olive_ai-0.2.0.dist-info/LICENSE
+Comment: 
+
+Filename: olive_ai-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: olive_ai-0.1.0.dist-info/METADATA
+Filename: olive_ai-0.2.0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: olive_ai-0.1.0.dist-info/WHEEL
+Filename: olive_ai-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: olive_ai-0.1.0.dist-info/top_level.txt
+Filename: olive_ai-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: olive_ai-0.1.0.dist-info/RECORD
+Filename: olive_ai-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## olive/__init__.py

```diff
@@ -10,8 +10,25 @@
 
 _sc = logging.StreamHandler(stream=sys.stdout)
 _formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)d:%(funcName)s] %(message)s")
 _sc.setFormatter(_formatter)
 _logger.addHandler(_sc)
 _logger.propagate = False
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
+
+
+def set_default_logger_severity(level):
+    """
+    Set log level for olive package.
+
+    :param level: 0: DEBUG, 1: INFO, 2: WARNING, 3: ERROR, 4: CRITICAL
+    """
+    # mapping from level to logging level
+    level_map = {0: logging.DEBUG, 1: logging.INFO, 2: logging.WARNING, 3: logging.ERROR, 4: logging.CRITICAL}
+
+    # check if level is valid
+    if level not in level_map:
+        raise ValueError(f"Invalid level {level}, should be one of {list(level_map.keys())}")
+
+    # set logger level
+    _logger.setLevel(level_map[level])
```

## olive/cache.py

```diff
@@ -4,14 +4,16 @@
 # --------------------------------------------------------------------------
 import json
 import logging
 import shutil
 from pathlib import Path
 from typing import Union
 
+from olive.common.config_utils import serialize_to_json
+from olive.model import ModelStorageKind, ONNXModel
 from olive.passes import REGISTRY as PASS_REGISTRY
 
 logger = logging.getLogger(__name__)
 
 
 def get_cache_sub_dirs(cache_dir: Union[str, Path] = ".olive-cache"):
     """
@@ -52,30 +54,21 @@
 
 
 def _delete_model(model_number: str, cache_dir: Union[str, Path] = ".olive-cache"):
     """
     Deletes the model and all associated runs and evaluations.
     """
     model_cache_dir, run_cache_dir, evaluation_cache_dir = get_cache_sub_dirs(cache_dir)
-    model_jsons = list(model_cache_dir.glob(f"{model_number}_*.json"))
-    for model_json in model_jsons:
-        try:
-            model_data = json.load(open(model_json, "r"))
-            if model_data != {}:
-                model_file = Path(json.load(open(model_json, "r"))["model_path"])
-                model_file_number = model_file.stem.split("_")[0]
-                if model_file_number == model_number:
-                    if model_file.is_dir():
-                        shutil.rmtree(model_file, ignore_errors=True)
-                    elif model_file.is_file():
-                        model_file.unlink()
-        except Exception as e:
-            logger.exception(e)
-        finally:
-            model_json = model_json.unlink()
+    # delete all model files that start with model_number
+    model_files = list(model_cache_dir.glob(f"{model_number}_*"))
+    for model_file in model_files:
+        if model_file.is_dir():
+            shutil.rmtree(model_file, ignore_errors=True)
+        elif model_file.is_file():
+            model_file.unlink()
 
     evaluation_jsons = list(evaluation_cache_dir.glob(f"{model_number}_*.json"))
     for evaluation_json in evaluation_jsons:
         evaluation_json.unlink()
 
     run_jsons = list(run_cache_dir.glob(f"*-{model_number}-*.json"))
     for run_json in run_jsons:
@@ -85,15 +78,16 @@
 def _delete_run(run_id: str, cache_dir: Union[str, Path] = ".olive-cache"):
     """
     Deletes the run and all associated models and evaluations.
     """
     run_cache_dir = get_cache_sub_dirs(cache_dir)[1]
     run_json = run_cache_dir / f"{run_id}.json"
     try:
-        run_data = json.load(open(run_json, "r"))
+        with run_json.open("r") as f:
+            run_data = json.load(f)
         # output model and children
         output_model_number = run_data["output_model_id"].split("_")[0]
         _delete_model(output_model_number, cache_dir)
     except Exception as e:
         logger.exception(e)
     finally:
         run_json.unlink()
@@ -109,7 +103,65 @@
 
     run_cache_dir = get_cache_sub_dirs(cache_dir)[1]
 
     # cached runs for pass
     run_jsons = list(run_cache_dir.glob(f"{pass_type}-*.json"))
     for run_json in run_jsons:
         _delete_run(run_json.stem, cache_dir)
+
+
+def save_model(
+    model_number: str,
+    output_dir: Union[str, Path] = None,
+    output_name: Union[str, Path] = None,
+    cache_dir: Union[str, Path] = ".olive-cache",
+):
+    """
+    Saves a model from the cache to a given path.
+    """
+    model_number = model_number.split("_")[0]
+    output_dir = Path(output_dir) if output_dir else Path.cwd()
+    output_dir.mkdir(parents=True, exist_ok=True)
+    output_name = output_name if output_name else "model"
+
+    model_cache_dir = get_cache_sub_dirs(cache_dir)[0]
+    model_jsons = list(model_cache_dir.glob(f"{model_number}_*.json"))
+    assert len(model_jsons) == 1, f"No model found for {model_number}"
+
+    with model_jsons[0].open("r") as f:
+        model_json = serialize_to_json(json.load(f))
+
+    if model_json["type"].lower() == "compositeonnxmodel":
+        logger.warning("Saving composite ONNX models is not supported yet.")
+        return
+
+    # save model file/folder
+    model_path = model_json["config"]["model_path"]
+    if model_path is not None and Path(model_path).exists():
+        if (
+            model_json["type"].lower() == "onnxmodel"
+            and model_json["config"]["model_storage_kind"] == ModelStorageKind.LocalFolder
+        ):
+            # onnx model has external data
+            output_path = ONNXModel.resolve_path(output_dir / output_name)
+            # copy the .onnx file along with external data files
+            shutil.copytree(Path(model_path).parent, Path(output_path).parent, dirs_exist_ok=True)
+            # rename the .onnx file to the output_path
+            (Path(output_path).parent / Path(model_path).name).rename(output_path)
+        else:
+            model_path = Path(model_path)
+            output_path = (output_dir / output_name).resolve()
+            if model_path.is_dir():
+                shutil.copytree(model_path, output_path, dirs_exist_ok=True)
+            elif model_path.is_file():
+                output_path = output_path.with_suffix(model_path.suffix)
+                shutil.copy(model_path, output_path)
+            output_path = str(output_path)
+    else:
+        output_path = model_path
+
+    # save model json
+    model_json["config"]["model_path"] = output_path
+    with open(output_dir / f"{output_name}.json", "w") as f:
+        json.dump(model_json, f, indent=4)
+
+    return model_json
```

## olive/constants.py

```diff
@@ -22,11 +22,12 @@
     Given a framework, there might be 1 or more on-disk model file format(s), model save/Load logic may differ.
     """
 
     ONNX = "ONNX"
     PYTORCH_ENTIRE_MODEL = "PyTorch.EntireModel"
     PYTORCH_STATE_DICT = "PyTorch.StateDict"
     PYTORCH_TORCH_SCRIPT = "PyTorch.TorchScript"
+    PYTORCH_MLFLOW_MODEL = "PyTorch.MLflow"
     TENSORFLOW_PROTOBUF = "TensorFlow.Protobuf"
     TENSORFLOW_SAVED_MODEL = "TensorFlow.SavedModel"
-    SNEP_DLC = "SNPE.DLC"
+    SNPE_DLC = "SNPE.DLC"
     OPENVINO_IR = "OpenVINO.IR"
```

## olive/model.py

```diff
@@ -1,33 +1,56 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
+import os
+import shutil
+import tempfile
 from abc import ABC, abstractmethod
+from copy import deepcopy
+from enum import Enum
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import onnx
-import onnxruntime as ort
 import torch
-import transformers
+import yaml
+from onnx import AttributeProto, GraphProto
 from pydantic import validator
 
-from olive.common.config_utils import ConfigBase, serialize_to_json
+if TYPE_CHECKING:
+    from azure.ai.ml import MLClient
+from olive.common.config_utils import ConfigBase, serialize_to_json, validate_config
+from olive.common.ort_inference import get_ort_inference_session
 from olive.common.user_module_loader import UserModuleLoader
-from olive.constants import Framework
+from olive.constants import Framework, ModelFileFormat
+from olive.hf_utils import (
+    get_hf_model_config,
+    huggingface_model_loader,
+    load_huggingface_model_from_model_class,
+    load_huggingface_model_from_task,
+)
 from olive.snpe import SNPEDevice, SNPEInferenceSession, SNPESessionOptions
 from olive.snpe.tools.dev import get_dlc_metrics
 from olive.systems.common import Device
 
 REGISTRY = {}
 logger = logging.getLogger(__name__)
 
 
+class ModelStorageKind(str, Enum):
+    LocalFile = "file"
+    LocalFolder = "folder"
+    AzureMLModel = "azureml"
+
+    def __str__(self) -> str:
+        return self.value
+
+
 class OliveModel(ABC):
     """
     Abstraction for logical "Model", it contains model path and related metadata.
     Each technique accepts Model as input, return Model as output.
     """
 
     @classmethod
@@ -35,61 +58,95 @@
         """Register the model."""
         super().__init_subclass__(**kwargs)
         REGISTRY[cls.__name__.lower()] = cls
 
     def __init__(
         self,
         framework: Framework,
+        model_file_format: ModelFileFormat,
         model_path: Optional[Union[Path, str]] = None,
         name: Optional[str] = None,
         version: Optional[int] = None,
-        is_file: bool = False,
-        is_aml_model: bool = False,
+        aml_storage_name: Optional[str] = None,
+        model_storage_kind: ModelStorageKind = ModelStorageKind.LocalFile,
     ):
-        if is_aml_model:
+        if isinstance(model_storage_kind, str):
+            model_storage_kind = ModelStorageKind(model_storage_kind)
+
+        assert isinstance(model_storage_kind, ModelStorageKind)
+
+        if model_storage_kind == ModelStorageKind.AzureMLModel:
             if not name:
                 raise Exception("Please specify model 'name' for Azure ML model")
             if not version:
                 raise Exception("Please specify model 'version' for Azure ML model")
             self.model_path = f"azureml:{name}:{version}"
         else:
             self.model_path = model_path
         self.version = version
         self.framework = framework
+        self.model_file_format = model_file_format
         self.name = name
-        self.is_file = is_file
-        self.is_aml_model = is_aml_model
+        self.aml_storage_name = aml_storage_name
+        self.composite_parent = None
+        self.model_storage_kind = model_storage_kind
 
     @abstractmethod
-    def load_model(self) -> object:
+    def load_model(self, rank: int = None) -> object:
         """
         Load model from disk, return in-memory model object
         Derived class should implement its specific logic if needed.
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def prepare_session(self, inference_settings: Optional[Dict[str, Any]] = None, device: Device = Device.CPU):
+    def prepare_session(
+        self, inference_settings: Optional[Dict[str, Any]] = None, device: Device = Device.CPU, rank: int = None
+    ):
         """
         Prepare inference session for Olive model, return in-memory inference session.
         Derived class should implement its specific logic if needed.
         """
         raise NotImplementedError()
 
+    def download_from_azureml(self, ml_client: "MLClient", download_path: Union[Path, str]):
+        if ml_client is None:
+            raise Exception("Azure ML client is not initialized")
+        if self.model_storage_kind != ModelStorageKind.AzureMLModel:
+            raise Exception("Only Azure ML model can be downloaded from Azure ML workspace")
+        if not self.aml_storage_name:
+            logger.error(
+                f"Error to download model {self.model_path} from Azure ML workspace: aml_storage_name is not specified"
+            )
+            raise Exception("Please specify model 'aml_storage_name' for Azure ML model")
+        try:
+            ml_client.models.download(name=self.name, version=self.version, download_path=download_path)
+        except Exception as e:
+            logger.error(f"Failed to downloafd model {self.name} from Azure ML workspace, error: {e}")
+            raise e
+
+        model_path = Path(download_path) / self.name / self.aml_storage_name
+        return model_path
+
+    def set_composite_parent(self, cp):
+        self.composite_parent = cp
+
+    def get_composite_parent(self):
+        return self.composite_parent
+
     def to_json(self, check_object: bool = False):
         model_path = self.model_path
         if model_path and Path(model_path).exists():
             model_path = Path(model_path)
         config = {
             "type": self.__class__.__name__,
             "config": {
                 "model_path": model_path,
                 "name": self.name,
-                "is_file": self.is_file,
-                "is_aml_model": self.is_aml_model,
+                "model_storage_kind": self.model_storage_kind.value,
                 "version": self.version,
             },
         }
         return serialize_to_json(config, check_object)
 
 
 class ModelConfig(ConfigBase):
@@ -102,202 +159,591 @@
             raise ValueError(f"Unknown model type {v}")
         return v
 
     def create_model(self):
         return REGISTRY[self.type.lower()](**self.config)
 
 
-class ONNXModel(OliveModel):
+class IOConfig(ConfigBase):
+    # TODO remove input names, shapes and types, turn to use olive dataset conifg.
+    input_names: List[str]
+    input_shapes: List[List[int]] = None
+    input_types: List[str] = None
+    output_names: List[str]
+    output_shapes: List[List[int]] = None
+    output_types: List[str] = None
+    dynamic_axes: Dict[str, Dict[int, str]] = None
+    # ONNX exporter might mark dimension like 'Transposepresent_value_self_1_dim_2' in shape inference
+    # even though we want the dimension to be a constant int.
+    # We use a workaround here: first use dim_param like "1" to represent the dimension, and then
+    # convert it to int in the onnx model.
+    string_to_int_dim_params: List[str] = None
+
+    @validator("input_shapes", "input_types")
+    def check_input_shapes(cls, v, values):
+        if not v:
+            return v
+
+        if "input_names" not in values:
+            raise ValueError("Invalid input_names")
+        if len(v) != len(values["input_names"]):
+            raise ValueError("input_names and input_shapes must have the same length")
+        return v
+
+    @validator("output_shapes", "output_types")
+    def check_output_shapes(cls, v, values):
+        if not v:
+            return v
+
+        if "output_names" not in values:
+            raise ValueError("Invalid output_names")
+        if len(v) != len(values["output_names"]):
+            raise ValueError("output_names and output_shapes must have the same length")
+        return v
+
+    @validator("dynamic_axes")
+    def convert_dynamic_axes(cls, v):
+        if not v:
+            return v
+
+        dynamic_axes = v
+        for k, v in dynamic_axes.items():
+            dynamic_axes[k] = {int(kk): vv for kk, vv in v.items()}
+        return dynamic_axes
+
+    @validator("string_to_int_dim_params")
+    def check_string_to_int_dim_params(cls, v):
+        if not v:
+            return v
+
+        for dim_param in v:
+            try:
+                int(dim_param)
+            except ValueError:
+                raise ValueError(f"Invalid string_to_int_dim_params: {dim_param}. Must be castable to int.")
+        return v
+
+
+class HFComponent(ConfigBase):
+    name: str
+    io_config: IOConfig = None
+    dummy_inputs_func: Union[str, Callable] = None
+
+
+class HFConfig(ConfigBase):
+    model_name: str = None
+    task: str = None
+    # TODO: remove model_class and only use task
+    model_class: str = None
+    use_ort_implementation: bool = False
+    components: List[HFComponent] = None
+    dataset: Dict[str, Any] = None
+
+    @validator("model_class", always=True)
+    def task_or_model_class_required(cls, v, values):
+        if values["model_name"]:
+            if not v and not values.get("task", None):
+                raise ValueError("Either task or model_class must be specified")
+            return v
+
+
+class ONNXModelBase(OliveModel):
+    """
+    Abstract class to manage ONNX models
+    """
+
+    def __init__(
+        self,
+        model_path: str = None,
+        name: Optional[str] = None,
+        version: Optional[int] = None,
+        aml_storage_name: Optional[str] = None,
+        model_storage_kind: Union[str, ModelStorageKind] = ModelStorageKind.LocalFile,
+        inference_settings: Optional[dict] = None,
+        use_ort_extensions: bool = False,
+    ):
+        super().__init__(
+            framework=Framework.ONNX,
+            model_file_format=ModelFileFormat.ONNX,
+            model_path=model_path,
+            name=name,
+            version=version,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=model_storage_kind,
+        )
+        self.inference_settings = inference_settings
+        self.use_ort_extensions = use_ort_extensions
+
+    def _is_valid_ep(self, filepath: str, ep: str = None):
+        # TODO: should be remove if future accelerators is implemented
+        # It should be a bug for onnxruntime where the execution provider is not be fallback.
+        import onnxruntime as ort
+
+        try:
+            sess_options = ort.SessionOptions()
+            if self.use_ort_extensions:
+                # register custom ops for onnxruntime-extensions
+                from onnxruntime_extensions import get_library_path
+
+                sess_options.register_custom_ops_library(get_library_path())
+
+            ort.InferenceSession(filepath, sess_options, providers=[ep])
+        except Exception as e:
+            logger.warning(
+                f"Error: {e}Olive will ignore this {ep}."
+                + f"Please make sure the environment with {ep} has the required dependencies."
+            )
+            return False
+        return True
+
+    @abstractmethod
+    def get_default_execution_providers(self, device: Device):
+        """
+        Returns a list of supported default execution providers
+        """
+        return ["CPUExecutionProvider"]
+
 
+class ONNXModel(ONNXModelBase):
     # device type definition: https://github.com/pytorch/pytorch/blob/master/c10/core/DeviceType.h
     EXECUTION_PROVIDERS = {
         "cpu": ["CPUExecutionProvider", "OpenVINOExecutionProvider"],
         "gpu": [
+            "DmlExecutionProvider",
             "CUDAExecutionProvider",
             "OpenVINOExecutionProvider",
             "TensorrtExecutionProvider",
             "CPUExecutionProvider",
         ],
+        "npu": ["QNNExecutionProvider", "CPUExecutionProvider"],
     }
 
     def __init__(
         self,
         model_path: str = None,
         name: Optional[str] = None,
         version: Optional[int] = None,
-        is_file: bool = True,
-        is_aml_model: bool = False,
+        aml_storage_name: Optional[str] = None,
+        model_storage_kind: Union[str, ModelStorageKind] = ModelStorageKind.LocalFile,
         inference_settings: Optional[dict] = None,
+        use_ort_extensions: bool = False,
+        hf_config: Union[Dict[str, Any], HFConfig] = None,
     ):
         super().__init__(
-            framework=Framework.ONNX,
             model_path=model_path,
             name=name,
             version=version,
-            is_file=is_file,
-            is_aml_model=is_aml_model,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=model_storage_kind,
+            inference_settings=inference_settings,
+            use_ort_extensions=use_ort_extensions,
         )
-        self.inference_settings = inference_settings
+        self.io_config = None
+        self.graph = None
+        self.all_graphs: Optional[List[GraphProto]] = None
+        # huggingface config
+        self.hf_config = validate_config(hf_config, HFConfig) if hf_config else None
+
+    @staticmethod
+    def resolve_path(file_or_dir_path: str, model_filename: str = "model.onnx") -> str:
+        """
+        The engine provides output paths to ONNX passes that do not contain .onnx
+        extension (these paths are generally locations in the cache). This function
+        will convert such paths to absolute file paths and also ensure the parent
+        directories exist. If the input path is already an ONNX file it is simply
+        returned. Examples:
+
+        resolve_path("c:/foo/bar.onnx") -> c:/foo/bar.onnx
+
+        resolve_path("c:/foo/bar") -> c:/foo/bar/model.onnx
+        """
+        path = Path(file_or_dir_path)
+        if path.suffix != ".onnx":
+            path = path / model_filename
+            parent_dir = path.parent
+            if not parent_dir.exists():
+                parent_dir.mkdir(parents=True, exist_ok=True)
+        return str(path)
 
-    def load_model(self) -> onnx.ModelProto:
+    def load_model(self, rank: int = None) -> onnx.ModelProto:
         # HACK: ASSUME no external data
         return onnx.load(self.model_path)
 
-    def prepare_session(self, inference_settings: Dict[str, Any], device: Device):
-        sess_options = ort.SessionOptions()
-        execution_provider = None
-        ort_inference_settings = inference_settings or self.inference_settings
-        if ort_inference_settings:
-            execution_provider = ort_inference_settings.get("execution_provider")
-            session_options = ort_inference_settings.get("session_options")
-            inter_op_num_threads = session_options.get("inter_op_num_threads")
-            intra_op_num_threads = session_options.get("intra_op_num_threads")
-            execution_mode = session_options.get("execution_mode")
-            graph_optimization_level = session_options.get("graph_optimization_level")
-            extra_session_config = session_options.get("extra_session_config")
-            if inter_op_num_threads:
-                sess_options.inter_op_num_threads = inter_op_num_threads
-            if intra_op_num_threads:
-                sess_options.intra_op_num_threads = intra_op_num_threads
-            if execution_mode:
-                if execution_mode == 0:
-                    sess_options.execution_mode = ort.ExecutionMode.ORT_SEQUENTIAL
-                elif execution_mode == 1:
-                    sess_options.execution_mode = ort.ExecutionMode.ORT_PARALLEL
-            if graph_optimization_level:
-                sess_options.graph_optimization_level = ort.GraphOptimizationLevel(graph_optimization_level)
-            if extra_session_config:
-                for key, value in extra_session_config.items():
-                    sess_options.add_session_config_entry(key, value)
-
-        if not execution_provider:
-            execution_provider = self.get_execution_providers(device)
-        elif isinstance(execution_provider, tuple):
-            execution_provider = execution_provider
-        elif isinstance(execution_provider, str):
-            execution_provider = [execution_provider]
-
-        return ort.InferenceSession(self.model_path, sess_options, providers=execution_provider)
+    def prepare_session(self, inference_settings: Dict[str, Any], device: Device, rank: int = None):
+        # user provided inference_settings > model's inference_settings > default settings
+        inference_settings = inference_settings or self.inference_settings or {}
+        # deep copy to avoid modifying the original settings
+        inference_settings = deepcopy(inference_settings)
+
+        # if user doesn't not provide ep list, use default value([ep]). Otherwise, use the user's ep list
+        if not inference_settings.get("execution_provider"):
+            inference_settings["execution_provider"] = self.get_default_execution_providers(device)
+
+        return get_ort_inference_session(self.model_path, inference_settings, self.use_ort_extensions)
+
+    def nodes(self):
+        for graph in self.get_all_graphs():
+            for node in graph.node:
+                yield node
+
+    def get_graph(self):
+        if self.graph is not None:
+            return self.graph
+        self.graph = self.load_model().graph
+        return self.graph
+
+    def get_all_graphs(self):
+        if self.all_graphs is not None:
+            return self.all_graphs
+        self.all_graphs = []
+        graph_queue = [self.get_graph()]
+        while graph_queue:
+            graph = graph_queue.pop(0)
+            self.all_graphs.append(graph)
+            for node in graph.node:
+                for attr in node.attribute:
+                    if attr.type == AttributeProto.AttributeType.GRAPH:
+                        assert isinstance(attr.g, GraphProto)
+                        graph_queue.append(attr.g)
+                    if attr.type == AttributeProto.AttributeType.GRAPHS:
+                        for g in attr.graphs:
+                            assert isinstance(g, GraphProto)
+                            graph_queue.append(g)
+        return self.all_graphs
+
+    def output_name_to_node(self):
+        output_name_to_node = {}
+        for node in self.nodes():
+            for output_name in node.output:
+                if output_name:  # could be empty when it is optional
+                    output_name_to_node[output_name] = node
+        return output_name_to_node
+
+    def get_initializer(self, name):
+        for graph in self.get_all_graphs():
+            for tensor in graph.initializer:
+                if tensor.name == name:
+                    return tensor
+        return None
 
     def to_json(self, check_object: bool = False):
         config = super().to_json(check_object)
-        config["config"].update({"inference_settings": self.inference_settings})
+        config["config"].update(
+            {
+                "inference_settings": self.inference_settings,
+                "use_ort_extensions": self.use_ort_extensions,
+                "hf_config": self.hf_config,
+            }
+        )
         return serialize_to_json(config, check_object)
 
-    def get_execution_providers(self, device: Device):
+    def get_default_execution_providers(self, device: Device):
+        # return firstly available ep as ort default ep
+        available_providers = ONNXModel.get_execution_providers(device)
+        for ep in available_providers:
+            if self._is_valid_ep(self.model_path, ep):
+                return [ep]
+        return super().get_default_execution_providers(device)
+
+    @staticmethod
+    def get_execution_providers(device: Device):
+        import onnxruntime as ort
+
         available_providers = ort.get_available_providers()
-        eps_per_device = self.EXECUTION_PROVIDERS.get(device)
+        eps_per_device = ONNXModel.EXECUTION_PROVIDERS.get(device)
 
         eps = []
         if eps_per_device:
             for ep in available_providers:
                 if ep in eps_per_device:
                     eps.append(ep)
 
         return eps if eps else available_providers
 
+    def get_io_config(self):
+        """
+        Get input/output names, shapes, types of the onnx model without creating an ort session.
+        This function loads the onnx model and parses the graph to get the io config.
+        """
+        if self.io_config:
+            return self.io_config
+
+        try:
+            from onnx.helper import tensor_dtype_to_np_dtype
+        except ImportError:
+            from onnx.mapping import TENSOR_TYPE_TO_NP_TYPE
+
+            def tensor_dtype_to_np_dtype(tensor_type):
+                return TENSOR_TYPE_TO_NP_TYPE[tensor_type]
+
+        # external data is not needed for io config parsing
+        # the .onnx model already contains all of the graph information
+        # this method works whether the external data is in the same directory or not
+        model = onnx.load(self.model_path, load_external_data=False)
+        io_config = {
+            "input_names": [],
+            "input_shapes": [],
+            "input_types": [],
+            "output_names": [],
+            "output_shapes": [],
+            "output_types": [],
+        }
+        for prefix, ios in [("input", model.graph.input), ("output", model.graph.output)]:
+            for io in ios:
+                # get name, type, shape
+                name = io.name
+                tensor_type = io.type.tensor_type
+                if tensor_type.elem_type == 0:
+                    # sequence type
+                    # TODO: add support for different types
+                    # refer to https://github.com/lutzroeder/netron/blob/main/source/onnx.js#L1424
+                    tensor_type = io.type.sequence_type.elem_type.tensor_type
+                data_type = str(tensor_dtype_to_np_dtype(tensor_type.elem_type))
+                shape = [dim.dim_param if dim.dim_param else dim.dim_value for dim in tensor_type.shape.dim]
+
+                # append to io_config
+                io_config[f"{prefix}_names"].append(name)
+                io_config[f"{prefix}_types"].append(data_type)
+                io_config[f"{prefix}_shapes"].append(shape)
+
+        # save io_config
+        self.io_config = io_config
+
+        return io_config
+
 
 class PyTorchModel(OliveModel):
     def __init__(
         self,
         model_path: str = None,
+        model_file_format: ModelFileFormat = ModelFileFormat.PYTORCH_ENTIRE_MODEL,
         name: Optional[str] = None,
         version: Optional[int] = None,
-        is_file: bool = False,
-        is_aml_model: bool = False,
-        model_loader=None,
-        model_script=None,
-        script_dir=None,
+        aml_storage_name: Optional[str] = None,
+        model_storage_kind: Union[str, ModelStorageKind] = ModelStorageKind.LocalFolder,
+        model_loader: Union[str, Callable] = None,
+        model_script: Union[str, Path] = None,
+        script_dir: Union[str, Path] = None,
+        io_config: Union[Dict[str, Any], IOConfig] = None,
+        dummy_inputs_func: Union[str, Callable] = None,
+        hf_config: Union[Dict[str, Any], HFConfig] = None,
     ):
         if not (
             isinstance(model_loader, Callable)
             or (isinstance(model_loader, str) and model_script)
             or model_path
-            or is_aml_model
+            or model_storage_kind == ModelStorageKind.AzureMLModel
+            or hf_config
         ):
             raise ValueError(
-                "model_path or is_aml_model is required "
+                "model_path or model_storage_kind/AzureMLModel is required "
                 "since model_loader is not callable or model_script is not provided"
             )
 
         self.model_loader = model_loader
         self.model_script = model_script
         self.script_dir = script_dir
         self.model = None
         super().__init__(
             framework=Framework.PYTORCH,
+            model_file_format=model_file_format,
             model_path=model_path,
             name=name,
             version=version,
-            is_file=is_file,
-            is_aml_model=is_aml_model,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=model_storage_kind,
         )
 
-    def load_model(self) -> torch.nn.Module:
+        # io config for conversion to onnx
+        self.io_config = validate_config(io_config, IOConfig) if io_config else None
+        self.dummy_inputs_func = dummy_inputs_func
+
+        self.dummy_inputs = None
+
+        # huggingface config
+        self.hf_config = validate_config(hf_config, HFConfig) if hf_config else None
+
+    def load_model(self, rank: int = None) -> torch.nn.Module:
         if self.model is not None:
             return self.model
 
         if self.model_loader is not None:
             user_module_loader = UserModuleLoader(self.model_script, self.script_dir)
             model = user_module_loader.call_object(self.model_loader, self.model_path)
+        elif self.hf_config and (self.hf_config.model_class or self.hf_config.task):
+            input_model = self.model_path or self.hf_config.model_name
+            if self.hf_config.task:
+                model = load_huggingface_model_from_task(self.hf_config.task, input_model)
+            else:
+                model = load_huggingface_model_from_model_class(
+                    self.hf_config.model_class, input_model, self.hf_config.use_ort_implementation
+                )
         else:
-            try:
+            if self.model_file_format == ModelFileFormat.PYTORCH_ENTIRE_MODEL:
                 model = torch.load(self.model_path)
-            except (RuntimeError, ModuleNotFoundError):
+            elif self.model_file_format == ModelFileFormat.PYTORCH_TORCH_SCRIPT:
                 model = torch.jit.load(self.model_path)
+            elif self.model_file_format == ModelFileFormat.PYTORCH_MLFLOW_MODEL:
+                model = self.load_mlflow_model()
+            elif self.model_file_format == ModelFileFormat.PYTORCH_STATE_DICT:
+                raise ValueError("Please use customized model loader to load state dict model.")
+            else:
+                raise ValueError(f"Unsupported model file format: {self.model_file_format}")
+
         self.model = model
 
         return model
 
-    def prepare_session(self, inference_settings: Dict[str, Any], device: Device):
+    def load_mlflow_model(self):
+        tmp_dir = tempfile.TemporaryDirectory(prefix="mlflow_tmp")
+        tmp_dir_path = Path(tmp_dir.name)
+
+        shutil.copytree(os.path.join(self.model_path, "data/model"), tmp_dir_path, dirs_exist_ok=True)
+        shutil.copytree(os.path.join(self.model_path, "data/config"), tmp_dir_path, dirs_exist_ok=True)
+        shutil.copytree(os.path.join(self.model_path, "data/tokenizer"), tmp_dir_path, dirs_exist_ok=True)
+
+        with open(os.path.join(self.model_path, "MLmodel"), "r") as fp:
+            mlflow_data = yaml.safe_load(fp)
+            hf_pretrained_class = mlflow_data["flavors"]["hftransformers"]["hf_pretrained_class"]
+
+        model_loader = huggingface_model_loader(hf_pretrained_class)
+        loaded_model = model_loader(tmp_dir_path)
+        loaded_model.eval()
+
+        tmp_dir.cleanup()
+
+        return loaded_model
+
+    def prepare_session(self, inference_settings: Dict[str, Any], device: Device, rank: int = None):
         return self.load_model().eval()
 
+    # TODO: remove this method once we have olive datasets implemented.
+    # The dataset should be able to provide the dummy inputs.
+    def get_dummy_inputs(self):
+        """
+        Return a dummy input for the model.
+        """
+        if self.dummy_inputs is not None:
+            return self.dummy_inputs
+
+        assert self.dummy_inputs_func or (
+            self.io_config and self.io_config.input_shapes
+        ), "dummy_inputs_func or io_config.input_shapes must be provided to get dummy input"
+
+        if self.dummy_inputs_func is not None:
+            user_module_loader = UserModuleLoader(self.model_script, self.script_dir)
+            dummy_inputs = user_module_loader.call_object(self.dummy_inputs_func, self)
+        else:
+            str_to_type = {
+                "float32": torch.float32,
+                "float16": torch.float16,
+                "int32": torch.int32,
+                "int64": torch.int64,
+                "int8": torch.int8,
+                "bool": torch.bool,
+            }
+            input_types = self.io_config.input_types or ["float32"] * len(self.io_config.input_shapes)
+            dummy_inputs = []
+            for shape, dtype in zip(self.io_config.input_shapes, input_types):
+                dummy_inputs.append(torch.zeros(shape, dtype=str_to_type[dtype]))
+            dummy_inputs = tuple(dummy_inputs) if len(dummy_inputs) > 1 else dummy_inputs[0]
+
+        self.dummy_inputs = dummy_inputs
+
+        return dummy_inputs
+
+    def get_model_config(self):
+        if self.hf_config is None:
+            raise Exception("HF model_config is not available")
+        return get_hf_model_config(self.hf_config.model_name)
+
+    @property
+    def components(self) -> List[str]:
+        """
+        Names of the components of the model.
+        """
+        if not self.hf_config or not self.hf_config.components:
+            return None
+
+        return [component.name for component in self.hf_config.components]
+
+    def get_component(self, component_name: str) -> "PyTorchModel":
+        """
+        Get a component of the model as a PyTorchModel.
+        """
+        assert self.components, "hf_config.components must be provided to get component"
+        assert component_name in self.components, f"component {component_name} not found in hf_config"
+
+        model = self.load_model()
+        model_component = getattr(model, component_name)
+
+        # get the component from hf_config
+        components_dict = {component.name: component for component in self.hf_config.components}
+        hf_component = components_dict[component_name]
+
+        def model_loader(_):
+            return model_component
+
+        return PyTorchModel(
+            model_loader=model_loader,
+            name=hf_component.name,
+            io_config=hf_component.io_config,
+            dummy_inputs_func=hf_component.dummy_inputs_func,
+            model_script=self.model_script,
+            script_dir=self.script_dir,
+        )
+
     def to_json(self, check_object: bool = False):
         config = super().to_json(check_object)
         config["config"].update(
             {
                 "model_loader": self.model_loader,
                 "model_script": Path(self.model_script) if self.model_script else None,
                 "script_dir": Path(self.script_dir) if self.script_dir else None,
+                "io_config": self.io_config,
+                "dummy_inputs_func": self.dummy_inputs_func,
+                "hf_config": self.hf_config,
             }
         )
         return serialize_to_json(config, check_object)
 
 
 class SNPEModel(OliveModel):
     def __init__(
         self,
         input_names: List[str],
         input_shapes: List[List[int]],
         output_names: List[str],
         output_shapes: List[List[int]],
         model_path: str = None,
-        is_aml_model: bool = False,
+        model_storage_kind=ModelStorageKind.LocalFile,
         name: Optional[str] = None,
         version: Optional[int] = None,
     ):
         super().__init__(
             framework=Framework.SNPE,
+            model_file_format=ModelFileFormat.SNPE_DLC,
             model_path=model_path,
             name=name,
             version=version,
-            is_file=True,
-            is_aml_model=is_aml_model,
+            model_storage_kind=model_storage_kind,
         )
         self.io_config = {
             "input_names": input_names,
             "input_shapes": input_shapes,
             "output_names": output_names,
             "output_shapes": output_shapes,
         }
 
-    def load_model(self):
+    def load_model(self, rank: int = None):
         raise NotImplementedError()
 
-    def prepare_session(self, inference_settings: Dict[str, Any], device: Device) -> SNPEInferenceSession:
+    def prepare_session(
+        self, inference_settings: Dict[str, Any], device: Device, rank: int = None
+    ) -> SNPEInferenceSession:
         session_options = SNPESessionOptions(**inference_settings) if inference_settings else None
         if device == Device.NPU:
             device = SNPEDevice.DSP
         session_options.device = device
         return SNPEInferenceSession(self.model_path, self.io_config, session_options)
 
     def to_json(self, check_object: bool = False):
@@ -307,43 +753,52 @@
 
     def get_dlc_metrics(self) -> dict:
         return get_dlc_metrics(self.model_path)
 
 
 class TensorFlowModel(OliveModel):
     def __init__(
-        self, model_path: str = None, name: Optional[str] = None, is_file: bool = False, is_aml_model: bool = False
+        self,
+        model_path: str = None,
+        model_file_format: ModelFileFormat = ModelFileFormat.TENSORFLOW_SAVED_MODEL,
+        name: Optional[str] = None,
+        model_storage_kind=ModelStorageKind.LocalFolder,
     ):
         super().__init__(
-            model_path=model_path, framework=Framework.TENSORFLOW, name=name, is_file=is_file, is_aml_model=is_aml_model
+            model_path=model_path,
+            framework=Framework.TENSORFLOW,
+            model_file_format=model_file_format,
+            name=name,
+            model_storage_kind=model_storage_kind,
         )
 
-    def load_model(self):
+    def load_model(self, rank: int = None):
         raise NotImplementedError()
 
-    def prepare_session(self, inference_settings: Dict[str, Any], device: Device):
+    def prepare_session(self, inference_settings: Dict[str, Any], device: Device, rank: int = None):
         raise NotImplementedError()
 
 
 class OpenVINOModel(OliveModel):
     def __init__(
         self,
         model_path: str,
         name: str = None,
-        is_file=False,
+        model_storage_kind=ModelStorageKind.LocalFolder,
         version: Optional[int] = None,
-        is_aml_model: bool = False,
+        aml_storage_name: Optional[str] = None,
     ):
         super().__init__(
             model_path=model_path,
             framework=Framework.OPENVINO,
+            model_file_format=ModelFileFormat.OPENVINO_IR,
             name=name,
-            is_file=is_file,
             version=version,
-            is_aml_model=is_aml_model,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=model_storage_kind,
         )
 
         if len(list(Path(model_path).glob("*.xml"))) == 0 or len(list(Path(model_path).glob("*.bin"))) == 0:
             raise Exception(f"No OpenVINO model found in {model_path}")
         if len(list(Path(model_path).glob("*.xml"))) > 1 or len(list(Path(model_path).glob("*.bin"))) > 1:
             raise Exception(f"More than 1 OpenVINO models are found in {model_path}")
 
@@ -354,39 +809,186 @@
 
         self.model_config = {
             "model_name": name if name else ov_model.stem,
             "model": str(ov_model.resolve()),
             "weights": str(ov_weights.resolve()),
         }
 
-    def load_model(self):
+    def load_model(self, rank: int = None):
         try:
             from openvino.tools.pot import load_model
         except ImportError:
-            raise ImportError("Please install olive[openvino] to use OpenVINO model")
+            raise ImportError("Please install olive-ai[openvino] to use OpenVINO model")
         return load_model(self.model_config)
 
-    def prepare_session(self, inference_settings: Dict[str, Any], device: Device):
+    def prepare_session(self, inference_settings: Dict[str, Any], device: Device, rank: int = None):
         try:
             from openvino.runtime import Core
         except ImportError:
-            raise ImportError("Please install olive[openvino] to use OpenVINO model")
+            raise ImportError("Please install olive-ai[openvino] to use OpenVINO model")
         ie = Core()
         model_pot = ie.read_model(model=self.model_config["model"])
         if device == Device.INTEL_MYRIAD:
             device = "MYRIAD"
         compiled_model = ie.compile_model(model=model_pot, device_name=device.upper())
         return compiled_model
 
 
-def huggingface_model_loader(model_loader):
-    if model_loader is None:
-        model_loader = "AutoModel"
-    if isinstance(model_loader, str):
-        try:
-            model_loader = getattr(transformers, model_loader)
-        except AttributeError:
-            raise AttributeError(f"{model_loader} is not found in transformers")
-    elif not isinstance(model_loader, Callable):
-        raise ValueError("model_loader must be a callable or a string defined in transformers")
+class DistributedOnnxModel(ONNXModelBase):
+    EXECUTION_PROVIDERS = {
+        "cpu": ["CPUExecutionProvider"],
+        "gpu": ["CUDAExecutionProvider", "CPUExecutionProvider"],
+    }
+
+    def __init__(
+        self,
+        model_filepaths: List[str],
+        name: Optional[str] = None,
+        version: Optional[int] = None,
+        aml_storage_name: Optional[str] = None,
+        inference_settings: Optional[dict] = None,
+        use_ort_extensions: bool = False,
+    ):
+        super().__init__(
+            model_path=None,
+            name=name,
+            version=version,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=ModelStorageKind.LocalFolder,
+            inference_settings=inference_settings,
+            use_ort_extensions=use_ort_extensions,
+        )
+        self.model_filepaths = model_filepaths
+
+    @property
+    def ranks(self):
+        return len(self.model_filepaths)
+
+    def load_model(self, rank: int) -> ONNXModel:
+        return ONNXModel(self.model_filepaths[rank], inference_settings=self.inference_settings)
+
+    def prepare_session(
+        self, inference_settings: Optional[Dict[str, Any]] = None, device: Device = Device.GPU, rank: int = 0
+    ):
+        # user provided inference_settings > model's inference_settings > default settings
+        inference_settings = inference_settings or self.inference_settings or {}
+        # deep copy to avoid modifying the original settings
+        inference_settings = deepcopy(inference_settings)
+
+        # if user doesn't not provide ep list, use default value([ep]). Otherwise, use the user's ep list
+        execution_providers = inference_settings.get("execution_provider")
+        if not execution_providers:
+            execution_providers = self.get_default_execution_providers(device)
+            inference_settings["execution_provider"] = execution_providers
+
+        if not inference_settings.get("provider_options"):
+            inference_settings["provider_options"] = [
+                {"device_id": str(rank)} if ep == "CUDAExecutionProvider" else {} for ep in execution_providers
+            ]
+
+        return get_ort_inference_session(self.model_filepaths[rank], inference_settings)
+
+    def get_default_execution_providers(self, filepath: str, device: Device):
+        # return firstly available ep as ort default ep
+        available_providers = DistributedOnnxModel.get_execution_providers(device)
+        for ep in available_providers:
+            if self._is_valid_ep(filepath, ep):
+                return [ep]
+
+        return ["CUDAExecutionProvider", "CPUExecutionProvider"]
+
+    @staticmethod
+    def get_execution_providers(device: Device):
+        import onnxruntime as ort
+
+        available_providers = ort.get_available_providers()
+        eps_per_device = DistributedOnnxModel.EXECUTION_PROVIDERS.get(device)
+
+        eps = []
+        if eps_per_device:
+            for ep in available_providers:
+                if ep in eps_per_device:
+                    eps.append(ep)
+
+        return eps if eps else available_providers
+
+    def to_json(self, check_object: bool = False):
+        config = {
+            "type": self.__class__.__name__,
+            "config": {
+                "model_filepaths": self.model_filepaths,
+                "name": self.name,
+                "version": self.version,
+                "inference_settings": self.inference_settings,
+                "use_ort_extensions": self.use_ort_extensions,
+            },
+        }
+        return serialize_to_json(config, check_object=check_object)
+
+
+class CompositeOnnxModel(ONNXModelBase):
+    """
+    CompositeOnnxModel represents multi component models. Whisper is an example composite
+    model that has encoder and decoder components. CompositeOnnxModel is a collection of
+    OnnxModels.
+    """
+
+    def __init__(
+        self,
+        model_components: List[str],
+        name: Optional[str] = None,
+        version: Optional[int] = None,
+        aml_storage_name: Optional[str] = None,
+        hf_config: Union[Dict[str, Any], HFConfig] = None,
+    ):
+        super().__init__(
+            model_path=None,
+            name=name,
+            version=version,
+            aml_storage_name=aml_storage_name,
+            model_storage_kind=ModelStorageKind.LocalFolder,
+        )
+
+        if isinstance(model_components[0], dict):
+            assert all(
+                [m.get("type").lower() == "onnxmodel" for m in model_components]
+            ), "All components must be ONNXModel"
+            self.model_components = [ONNXModel(**m.get("config", {})) for m in model_components]
+        else:
+            assert all([isinstance(m, ONNXModel) for m in model_components]), "All components must be ONNXModel"
+            self.model_components = model_components
+
+        for m in self.model_components:
+            m.set_composite_parent(self)
+
+        self.hf_config = validate_config(hf_config, HFConfig) if hf_config else None
+
+    def load_model(self, rank: int = None):
+        raise NotImplementedError()
+
+    def prepare_session(self, inference_settings: Dict[str, Any], device: Device, rank: int = None):
+        raise NotImplementedError()
+
+    def get_default_execution_providers(self, device: Device):
+        raise NotImplementedError()
+
+    def get_model_components(self):
+        return self.model_components
+
+    def get_model_component(self, idx):
+        return self.model_components[idx]
+
+    def get_model_config(self):
+        if self.hf_config is None:
+            raise Exception("HF model_config is not available")
+        return get_hf_model_config(self.hf_config.model_name)
+
+    def to_json(self, check_object: bool = False):
+        json_dict = {
+            "type": self.__class__.__name__,
+            "config": {"name": self.name, "version": self.version, "hf_config": self.hf_config},
+        }
+        json_dict["config"]["model_components"] = []
+        for m in self.model_components:
+            json_dict["config"]["model_components"].append(m.to_json(check_object))
 
-    return model_loader.from_pretrained
+        return serialize_to_json(json_dict, check_object)
```

## olive/common/config_utils.py

```diff
@@ -1,22 +1,25 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import inspect
 import json
+import logging
 from functools import partial
 from pathlib import Path
 from types import FunctionType, MethodType
 from typing import Any, Callable, Dict, Optional, Union
 
 from pydantic import BaseModel, create_model, validator
 
 from olive.common.utils import hash_function, hash_object
 
+logger = logging.getLogger(__name__)
+
 
 def serialize_function(function: Union[FunctionType, MethodType]) -> dict:
     """
     Serialize a function into a dictionary.
     """
     return {
         "olive_parameter_type": "Function",
@@ -115,15 +118,15 @@
 class ConfigParam(ConfigBase):
     """
     Dataclass for pass configuration parameters.
     """
 
     type_: Any
     required: bool = False
-    default: Any = None
+    default_value: Any = None
     is_object: bool = False
     description: str = None
 
     def __repr__(self):
         repr_list = []
         booleans = ["required", "is_object"]
         for k, v in self.__dict__.items():
@@ -175,35 +178,41 @@
             validators[validator_name] = validator(param, allow_reuse=True)(validate_object)
 
         type_ = param_config.type_
         if param_config.required:
             config[param] = (type_, ...)
             continue
 
-        config[param] = (type_, param_config.default)
+        config[param] = (Optional[type_], param_config.default_value)
 
     return create_model(class_name, **config, __base__=base, __validators__=validators)
 
 
 def validate_config(
-    config: Union[Dict[str, Any], ConfigBase, None], base_class: ConfigBase, instance_class: Optional[ConfigBase] = None
+    config: Union[Dict[str, Any], ConfigBase, None],
+    base_class: ConfigBase,
+    instance_class: Optional[ConfigBase] = None,
+    warn_unused_keys: bool = True,
 ):
     """
     Validate a config dictionary or object against a base class and instance class.
     instance class is a subclass of base class.
     """
     config = config or {}
 
     if instance_class is None:
         instance_class = base_class
 
-    if config is None:
-        config = instance_class()
-    elif isinstance(config, dict):
+    if isinstance(config, dict):
+        user_keys = set(config.keys())
         config = instance_class(**config)
+        config_keys = set(config.dict().keys())
+        unused_keys = user_keys - config_keys
+        if unused_keys and warn_unused_keys:
+            logger.warning(f"Keys {unused_keys} are not part of {instance_class.__name__}. Ignoring them.")
     elif isinstance(config, base_class) and config.__class__.__name__ == instance_class.__name__:
         pass
     else:
         raise ValueError(
             f"Invalid config class. Expected {instance_class.__name__} but got {config.__class__.__name__}"
         )
     return config
```

## olive/common/utils.py

```diff
@@ -32,14 +32,20 @@
     stderr = out.stderr.decode("utf-8")
     if check and returncode != 0:
         raise RuntimeError(f"Command '{cmd}' failed with return code {returncode} and error: {stderr}")
 
     return returncode, stdout, stderr
 
 
+def hash_string(string):  # pragma: no cover
+    md5_hash = hashlib.md5()
+    md5_hash.update(string.encode())
+    return md5_hash.hexdigest()
+
+
 def hash_io_stream(f):  # pragma: no cover
     md5_hash = hashlib.md5()
     # Read and update hash in chunks of 4K
     for byte_block in iter(lambda: f.read(4096), b""):
         md5_hash.update(byte_block)
     return md5_hash.hexdigest()
 
@@ -132,7 +138,27 @@
             num_tries += 1
             if num_tries == max_tries:
                 logger.error(f"Failed with error: {e}")
                 raise e
             logger.debug(f"Failed. Retrying in {sleep_time} seconds...")
             time.sleep(sleep_time)
             sleep_time *= backoff
+
+
+def tensor_data_to_device(data, device: str):
+    if device is None:
+        return data
+
+    from torch import Tensor
+
+    if isinstance(data, Tensor):
+        return data.to(device)
+    elif isinstance(data, dict):
+        return {k: tensor_data_to_device(v, device) for k, v in data.items()}
+    elif isinstance(data, list):
+        return [tensor_data_to_device(v, device) for v in data]
+    elif isinstance(data, tuple):
+        return tuple(tensor_data_to_device(v, device) for v in data)
+    elif isinstance(data, set):
+        return set(tensor_data_to_device(v, device) for v in data)
+    else:
+        return data
```

## olive/evaluator/accuracy.py

```diff
@@ -25,77 +25,77 @@
     def __init__(self, config: Union[ConfigBase, Dict[str, Any]] = None) -> None:
         super().__init__(config)
 
     @staticmethod
     def _default_config() -> Dict[str, ConfigParam]:
         return {
             "num_classes": ConfigParam(type_=int),
-            "threshold": ConfigParam(type_=float, default=0.5),
-            "average": ConfigParam(type_=str, default="micro"),
-            "ignore_index": ConfigParam(type_=list, default=None),
-            "top_k": ConfigParam(type_=int, default=None),
-            "mdmc_average": ConfigParam(type_=str, default="global"),
+            "threshold": ConfigParam(type_=float, default_value=0.5),
+            "average": ConfigParam(type_=str, default_value="micro"),
+            "ignore_index": ConfigParam(type_=list, default_value=None),
+            "top_k": ConfigParam(type_=int, default_value=None),
+            "mdmc_average": ConfigParam(type_=str, default_value="global"),
         }
 
     @abstractmethod
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         raise NotImplementedError()
 
 
 class AccuracyScore(AccuracyBase):
     name: str = "accuracy_score"
 
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         preds_tensor = torch.tensor(preds, dtype=torch.int)
         target_tensor = torch.tensor(target, dtype=torch.int)
         accuracy = torchmetrics.Accuracy(**self.config.dict())
         result = accuracy(preds_tensor, target_tensor)
         return result.item()
 
 
 class F1Score(AccuracyBase):
     name: str = "f1_score"
 
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         preds_tensor = torch.tensor(preds, dtype=torch.int)
         target_tensor = torch.tensor(target, dtype=torch.int)
         f1 = torchmetrics.F1Score(**self.config.dict())
         result = f1(preds_tensor, target_tensor)
         return result.item()
 
 
 class Precision(AccuracyBase):
     name: str = "precision"
 
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         preds_tensor = torch.tensor(preds, dtype=torch.int)
         target_tensor = torch.tensor(target, dtype=torch.int)
         precision = torchmetrics.Precision(**self.config.dict())
         result = precision(preds_tensor, target_tensor)
         return result.item()
 
 
 class Recall(AccuracyBase):
     name: str = "recall"
 
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         preds_tensor = torch.tensor(preds, dtype=torch.int)
         target_tensor = torch.tensor(target, dtype=torch.int)
         recall = torchmetrics.Recall(**self.config.dict())
         result = recall(preds_tensor, target_tensor)
         return result.item()
 
 
 class AUC(AccuracyBase):
     name: str = "auc"
 
     @staticmethod
     def _default_config():
-        return {"reorder": ConfigParam(type_=bool, default=False)}
+        return {"reorder": ConfigParam(type_=bool, default_value=False)}
 
-    def evaluate(self, preds, target):
+    def measure(self, preds, target):
         preds = np.array(preds).flatten()
         target = np.array(target).flatten()
         preds_tensor = torch.tensor(preds, dtype=torch.int)
         target_tensor = torch.tensor(target, dtype=torch.int)
         result = torchmetrics.functional.auc(preds_tensor, target_tensor, self.config.reorder)
         return result.item()
```

## olive/evaluator/metric.py

```diff
@@ -1,17 +1,18 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from enum import Enum
-from typing import List, Union
+from typing import Union
 
-from pydantic import BaseModel, validator
+from pydantic import validator
 
 from olive.common.config_utils import ConfigBase, validate_config
+from olive.data.config import DataConfig
 from olive.evaluator.accuracy import AccuracyBase
 from olive.evaluator.metric_config import LatencyMetricConfig, MetricGoal, get_user_config_class
 
 
 class MetricType(str, Enum):
     ACCURACY = "accuracy"
     LATENCY = "latency"
@@ -37,25 +38,27 @@
     P99 = "p99"
     P999 = "p999"
 
 
 # TODO: support multiple subtypes at the same type for the same type
 # Otherwise it's a waste of compute and time if we have to evaluate a model for different subtypes
 # names, subtypes: Union[str, List[str]]
-# However accurcacy metric poses a slight problem since AUC has a different config. Need to resolve this
+# However accuracy metric poses a slight problem since AUC has a different config. Need to resolve this
 # so that we get a single metric config for a single type
 # This way, the user can return multiple metrics at once
 class Metric(ConfigBase):
     name: str
     type: MetricType
     sub_type: Union[AccuracySubType, LatencySubType] = None
     higher_is_better: bool = True
+    priority_rank: int = 1
     goal: MetricGoal = None
     metric_config: ConfigBase = None
-    user_config: ConfigBase
+    user_config: ConfigBase = None
+    data_config: DataConfig = DataConfig()
 
     @validator("sub_type", always=True, pre=True)
     def validate_sub_type(cls, v, values):
         if "type" not in values:
             raise ValueError("Invalid type")
 
         if values["type"] == MetricType.CUSTOM:
@@ -129,11 +132,7 @@
         valid_range = ranges[(v.type, higher_is_better)]
         if not valid_range[0] < v.value < valid_range[1]:
             raise ValueError(
                 f"Invalid goal value {v.value} for {v.type} and higher_is_better={higher_is_better}. Valid range is"
                 f" {valid_range}"
             )
         return v
-
-
-class MetricList(BaseModel):
-    __root__: List[Metric]
```

## olive/evaluator/metric_config.py

```diff
@@ -1,40 +1,43 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from pathlib import Path
-from typing import Callable, Union
+from typing import Callable, List, Union
 
 from pydantic import validator
 
 from olive.common.config_utils import ConfigBase, ConfigParam, create_config_class
 
 WARMUP_NUM = 10
 REPEAT_TEST_NUM = 20
 SLEEP_NUM = 0
 
 
 _common_user_config = {
     "script_dir": ConfigParam(type_=Union[Path, str]),
     "user_script": ConfigParam(type_=Union[Path, str]),
     "data_dir": ConfigParam(type_=Union[Path, str]),
-    "batch_size": ConfigParam(type_=int, default=1),
+    "batch_size": ConfigParam(type_=int, default_value=1),
+    "input_names": ConfigParam(type_=List),
+    "input_shapes": ConfigParam(type_=List),
+    "input_types": ConfigParam(type_=List),
 }
 
 _common_user_config_validators = {}
 
 _type_to_user_config = {
     "latency": {
-        "dataloader_func": ConfigParam(type_=Union[Callable, str], required=True, is_object=True),
+        "dataloader_func": ConfigParam(type_=Union[Callable, str], is_object=True),
         "inference_settings": ConfigParam(type_=dict),
-        "io_bind": ConfigParam(type_=bool, default=False),
+        "io_bind": ConfigParam(type_=bool, default_value=False),
     },
     "accuracy": {
-        "dataloader_func": ConfigParam(type_=Union[Callable, str], required=True, is_object=True),
+        "dataloader_func": ConfigParam(type_=Union[Callable, str], is_object=True),
         "post_processing_func": ConfigParam(type_=Union[Callable, str], is_object=True),
         "inference_settings": ConfigParam(type_=dict),
     },
     "custom": {
         "evaluate_func": ConfigParam(type_=Union[Callable, str], required=True, is_object=True),
     },
 }
@@ -46,14 +49,20 @@
     default_config = _common_user_config.copy()
     default_config.update(_type_to_user_config[metric_type])
     validators = _common_user_config_validators.copy()
     validators.update(_type_to_user_config_validators.get(metric_type, {}))
     return create_config_class(f"{metric_type.title()}UserConfig", default_config, ConfigBase, validators)
 
 
+def get_properties_from_metric_type(metric_type):
+    user_config_class = get_user_config_class(metric_type)
+    # avoid to use schema() to get the fields, because it will skip the ones with object type
+    return list(user_config_class.__fields__)
+
+
 # TODO: automate latency metric config also we standardize accuracy metric config
 class LatencyMetricConfig(ConfigBase):
     warmup_num: int = WARMUP_NUM
     repeat_test_num: int = REPEAT_TEST_NUM
     sleep_num: int = SLEEP_NUM
```

## olive/evaluator/olive_evaluator.py

```diff
@@ -1,49 +1,437 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
-from typing import Dict, List
+import time
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List
 
+import numpy as np
+import torch
 from pydantic import validator
+from torch.utils.data import Dataset
 
 from olive.common.config_utils import ConfigBase
-from olive.evaluator.metric import Metric
-from olive.model import OliveModel
-from olive.systems.common import SystemType
-from olive.systems.local import LocalSystem
-from olive.systems.olive_system import OliveSystem
-from olive.systems.system_config import SystemConfig
+from olive.common.user_module_loader import UserModuleLoader
+from olive.common.utils import tensor_data_to_device
+from olive.constants import Framework
+from olive.evaluator.accuracy import AUC, AccuracyScore, F1Score, Precision, Recall
+from olive.evaluator.metric import AccuracySubType, LatencySubType, Metric, MetricType
+from olive.model import OliveModel, ONNXModel, OpenVINOModel, PyTorchModel, SNPEModel
+from olive.systems.common import Device
 
 logger = logging.getLogger(__name__)
 
 
-class OliveEvaluator:
-    def __init__(self, metrics: List[Metric], target: OliveSystem = None):
-        metric_names = set([metric.name for metric in metrics])
-        assert len(metric_names) == len(metrics), "Metric names must be unique"
-        self.metrics = metrics
-        self.target = target or LocalSystem()
-
-    def get_metric(self, metric_name: str) -> Metric:
-        for metric in self.metrics:
-            if metric.name == metric_name:
-                return metric
-        raise ValueError(f"Metric {metric_name} not found")
-
-    def evaluate(self, model: OliveModel) -> Dict:
-        return self.target.evaluate_model(model, self.metrics)
+class DummyDataloader(Dataset):
+    def __init__(self, input_names, input_shapes, input_types):
+        self.input_names = input_names
+        self.input_shapes = input_shapes
+        self.input_types = input_types
+
+    def __len__(self):
+        return 100
+
+    def __getitem__(self, index):
+        str_to_type = {"float32": torch.float32, "float16": torch.float16, "int32": torch.int32, "int64": torch.int64}
+        input_types = []
+        if self.input_types:
+            for input_type in self.input_types:
+                input_types.append(str_to_type[input_type])
+        else:
+            for _ in range(len(self.input_names)):
+                input_types.append(torch.float32)
+        if len(self.input_names) == 1:
+            dummy_inputs = torch.ones(self.input_shapes[0], dtype=input_types[0])
+        else:
+            dummy_inputs = {}
+            for input_name, input_shape, input_type in zip(self.input_names, self.input_shapes, input_types):
+                dummy_inputs.update({input_name: torch.ones(input_shape, dtype=input_type)})
+        label = 0
+        return dummy_inputs, label
+
+
+class OliveEvaluator(ABC):
+    registry: Dict[str, "OliveEvaluator"] = {}
+
+    @classmethod
+    def __init_subclass__(cls, framework: Framework, **kwargs) -> None:
+        super().__init_subclass__(**kwargs)
+        cls.framework = framework
+        cls.registry[str(framework).lower()] = cls
+
+    def __init__(self):
+        pass
+
+    def get_inference_settings(self, metric: Metric) -> Dict[str, Any]:
+        # user.config.inference_settings > model.inference_settings > default inference_settings
+        # when user.config.inference_settings is None, the model.inference_settings
+        # will be used in model.prepare_session(..)
+        return (
+            metric.user_config.inference_settings.get(self.framework.lower())
+            if metric.user_config.inference_settings
+            else None
+        )
+
+    @abstractmethod
+    def _evaluate_accuracy(
+        self, model: OliveModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        raise NotImplementedError()
+
+    @abstractmethod
+    def _evaluate_latency(
+        self, model: OliveModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        raise NotImplementedError()
+
+    def _evaluate_custom(
+        self,
+        model: OliveModel,
+        metric: Metric,
+        dataloader: Dataset,
+        eval_func,
+        device: Device = Device.CPU,
+        post_func=None,
+    ) -> Dict[str, Any]:
+        # TODO: Change the evaluate function to accept the metric rather than
+        # breaking it into multiple arguments
+        # return eval_func(model, metric, dataloader, device, post_func)
+        return eval_func(model, metric.user_config.data_dir, metric.user_config.batch_size, device)
+
+    def evaluate(self, model: OliveModel, metrics: List[Metric], device: Device = Device.CPU) -> Dict[str, Any]:
+        metrics_res = {}
+        for metric in metrics:
+            dataloader, eval_func, post_func = OliveEvaluator.get_user_config(metric)
+
+            if metric.type == MetricType.ACCURACY:
+                metrics_res[metric.name] = self._evaluate_accuracy(model, metric, dataloader, device, post_func)
+            elif metric.type == MetricType.LATENCY:
+                metrics_res[metric.name] = self._evaluate_latency(model, metric, dataloader, device, post_func)
+            elif metric.type == MetricType.CUSTOM:
+                metrics_res[metric.name] = self._evaluate_custom(
+                    model, metric, dataloader, eval_func, device, post_func
+                )
+            else:
+                raise TypeError(f"{metric.type} is not a supported metric type")
+        return metrics_res
+
+    @staticmethod
+    def get_user_config(metric: Metric):
+        user_module = UserModuleLoader(metric.user_config.user_script, metric.user_config.script_dir)
+
+        post_processing_func = getattr(metric.user_config, "post_processing_func", None)
+        post_func = user_module.load_object(post_processing_func)
+
+        dataloader_func = getattr(metric.user_config, "dataloader_func", None)
+        dataloader = user_module.call_object(
+            dataloader_func, metric.user_config.data_dir, metric.user_config.batch_size
+        )
+
+        evaluate_func = getattr(metric.user_config, "evaluate_func", None)
+        eval_func = user_module.load_object(evaluate_func)
+
+        if metric.user_config.input_names and metric.user_config.input_shapes and not dataloader and not eval_func:
+            dataloader = DummyDataloader(
+                metric.user_config.input_names, metric.user_config.input_shapes, metric.user_config.input_types
+            )
+
+        if not dataloader or not post_func:
+            dc = metric.data_config.to_data_container()
+
+            # TODO remove user_scripts dataloader: we should respect user scripts
+            # dataloder to meet back compatibility for time being.
+            dataloader = dataloader or dc.create_dataloader()
+            post_func = post_func or dc.config.post_process
+
+        return dataloader, eval_func, post_func
+
+    @staticmethod
+    def compute_accuracy(metric: Metric, preds: Any, targets: Any) -> Dict[str, Any]:
+        """
+        Compute accuracy metrics
+        """
+        if metric.sub_type == AccuracySubType.ACCURACY_SCORE:
+            return AccuracyScore(metric.metric_config).measure(preds, targets)
+        elif metric.sub_type == AccuracySubType.F1_SCORE:
+            return F1Score(metric.metric_config).measure(preds, targets)
+        elif metric.sub_type == AccuracySubType.PRECISION:
+            return Precision(metric.metric_config).measure(preds, targets)
+        elif metric.sub_type == AccuracySubType.RECALL:
+            return Recall(metric.metric_config).measure(preds, targets)
+        elif metric.sub_type == AccuracySubType.AUC:
+            return AUC(metric.metric_config).measure(preds, targets)
+        else:
+            raise TypeError(f"{metric.sub_type} is not a supported accuracy metric")
+
+    @staticmethod
+    def compute_latency(metric: Metric, latencies: Any) -> float:
+        """
+        Compute latency metrics
+        """
+        if metric.sub_type == LatencySubType.AVG:
+            return round(sum(latencies) / len(latencies) * 1000, 5)
+        elif metric.sub_type == LatencySubType.MAX:
+            return round(max(latencies) * 1000, 5)
+        elif metric.sub_type == LatencySubType.MIN:
+            return round(min(latencies) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P50:
+            return round(np.percentile(latencies, 50) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P75:
+            return round(np.percentile(latencies, 75) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P90:
+            return round(np.percentile(latencies, 90) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P95:
+            return round(np.percentile(latencies, 95) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P99:
+            return round(np.percentile(latencies, 99) * 1000, 5)
+        elif metric.sub_type == LatencySubType.P999:
+            return round(np.percentile(latencies, 99.9) * 1000, 5)
+        else:
+            raise TypeError(f"{metric.sub_type} is not a supported latency metric")
+
+
+class OnnxEvaluator(OliveEvaluator, framework=Framework.ONNX):
+    def __init__(self):
+        super().__init__()
+
+    @staticmethod
+    def format_input(input_data, io_config):
+        """
+        Format input data to ONNX input format.
+        """
+        input_names = io_config["input_names"]
+        name_to_type = {k: v for k, v in zip(io_config["input_names"], io_config["input_types"])}
+        if not isinstance(input_data, dict):
+            input_data = dict(zip(input_names, [input_data]))
+        input_dict = {
+            k: np.ascontiguousarray(
+                input_data[k].cpu().numpy() if isinstance(input_data[k], torch.Tensor) else input_data[k],
+                dtype=name_to_type[k],
+            )
+            for k in input_data.keys()
+            if k in input_names
+        }
+        return input_dict
+
+    def _evaluate_accuracy(
+        self, model: ONNXModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+        io_config = model.get_io_config()
+
+        preds = []
+        targets = []
+        output_names = io_config["output_names"]
+        for input_data, labels in dataloader:
+            input_dict = OnnxEvaluator.format_input(input_data, io_config)
+            res = session.run(input_feed=input_dict, output_names=None)
+            result = torch.Tensor(res[0]) if len(output_names) == 1 else torch.Tensor(res)
+            outputs = post_func(result) if post_func else result
+            preds.extend(outputs.tolist())
+            targets.extend(labels.data.tolist())
+
+        return OliveEvaluator.compute_accuracy(metric, preds, targets)
+
+    def _evaluate_latency(
+        self, model: OliveModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        warmup_num = metric.metric_config.warmup_num
+        repeat_test_num = metric.metric_config.repeat_test_num
+        sleep_num = metric.metric_config.sleep_num
+
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+        io_config = model.get_io_config()
+
+        input_data, _ = next(iter(dataloader))
+        input_dict = OnnxEvaluator.format_input(input_data, io_config)
+
+        if metric.user_config.io_bind:
+            io_bind_op = session.io_binding()
+            io_bind_device = "cuda" if device == "gpu" else "cpu"
+            for k, v in input_dict.items():
+                io_bind_op.bind_cpu_input(k, v)
+            for item in session.get_outputs():
+                io_bind_op.bind_output(item.name, io_bind_device)
+
+        for _ in range(warmup_num):
+            if metric.user_config.io_bind:
+                session.run_with_iobinding(io_bind_op)
+            else:
+                session.run(input_feed=input_dict, output_names=None)
+
+        latencies = []
+        for _ in range(repeat_test_num):
+            if metric.user_config.io_bind:
+                t = time.perf_counter()
+                session.run_with_iobinding(io_bind_op)
+                latencies.append(time.perf_counter() - t)
+            else:
+                t = time.perf_counter()
+                session.run(input_feed=input_dict, output_names=None)
+                latencies.append(time.perf_counter() - t)
+            time.sleep(sleep_num)
+
+        return OliveEvaluator.compute_latency(metric, latencies)
+
+
+class PyTorchEvaluator(OliveEvaluator, framework=Framework.PYTORCH):
+    def __init__(self):
+        super().__init__()
+
+    @staticmethod
+    def _device_string_to_torch_device(device: Device):
+        return torch.device("cuda") if device == Device.GPU else torch.device(device)
+
+    def _evaluate_accuracy(
+        self, model: PyTorchModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        preds = []
+        targets = []
+        device = PyTorchEvaluator._device_string_to_torch_device(device)
+        if device:
+            session.to(device)
+        for input_data, labels in dataloader:
+            input_data = tensor_data_to_device(input_data, device)
+            result = session(**input_data) if isinstance(input_data, dict) else session(input_data)
+            outputs = post_func(result) if post_func else result
+            # use the list.extend instead of list.append to avoid the different sub-array has different size when
+            # batch size is greater than 2 so that the residue array has different size with the batch size,
+            # which will result the exception like:
+            #  ValueError: expected sequence of length 128 at dim 1 (got 3)
+            preds.extend(outputs.tolist())
+            targets.extend(labels.data.tolist())
+
+        return OliveEvaluator.compute_accuracy(metric, preds, targets)
+
+    def _evaluate_latency(
+        self, model: PyTorchModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        warmup_num = metric.metric_config.warmup_num
+        repeat_test_num = metric.metric_config.repeat_test_num
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        input_data, _ = next(iter(dataloader))
+        device = PyTorchEvaluator._device_string_to_torch_device(device)
+        if device:
+            session.to(device)
+            input_data = tensor_data_to_device(input_data, device)
+
+        latencies = []
+        if isinstance(input_data, dict):
+            for _ in range(warmup_num):
+                session(**input_data)
+            for _ in range(repeat_test_num):
+                t = time.perf_counter()
+                session(**input_data)
+                latencies.append(time.perf_counter() - t)
+        else:
+            for _ in range(warmup_num):
+                session(input_data)
+            for _ in range(repeat_test_num):
+                t = time.perf_counter()
+                session(input_data)
+                latencies.append(time.perf_counter() - t)
+
+        return OliveEvaluator.compute_latency(metric, latencies)
+
+
+class SNPEEvaluator(OliveEvaluator, framework=Framework.SNPE):
+    def __init__(self):
+        super().__init__()
+
+    def _evaluate_accuracy(
+        self, model: SNPEModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        preds = []
+        targets = []
+        for data_dir, input_list, labels in dataloader:
+            result = session(input_list, data_dir)
+            if post_func:
+                outputs = post_func(result)
+            else:
+                raise ValueError("Post processing function is required for SNPE model")
+            preds.extend(outputs.tolist())
+            targets.extend(labels.tolist())
+
+        return OliveEvaluator.compute_accuracy(metric, preds, targets)
+
+    def _evaluate_latency(
+        self, model: SNPEModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        data_dir, input_data, _ = next(iter(dataloader))
+        total_runs = metric.metric_config.warmup_num + metric.metric_config.repeat_test_num
+        results = session(input_data, data_dir, runs=total_runs, sleep=metric.metric_config.sleep_num)
+        latencies = results["latencies"]["total_inference_time"][metric.metric_config.warmup_num:]  # fmt: skip
+
+        return OliveEvaluator.compute_latency(metric, latencies)
+
+
+class OpenVINOEvaluator(OliveEvaluator, framework=Framework.OPENVINO):
+    def __init__(self):
+        super().__init__()
+
+    def _evaluate_accuracy(
+        self, model: OpenVINOModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        preds = []
+        targets = []
+        for input_data, labels in dataloader:
+            result = session.infer_new_request({0: input_data})
+            outputs = post_func(result) if post_func else result
+            if not isinstance(labels, list):
+                labels = [labels]
+            preds.extend(outputs)
+            targets.extend(labels)
+
+        return OliveEvaluator.compute_accuracy(metric, preds, targets)
+
+    def _evaluate_latency(
+        self, model: OpenVINOModel, metric: Metric, dataloader: Dataset, device: Device = Device.CPU, post_func=None
+    ) -> Dict[str, Any]:
+        session = model.prepare_session(inference_settings=self.get_inference_settings(metric), device=device)
+
+        latencies = []
+        for input_data, _ in dataloader:
+            t = time.perf_counter()
+            session(input_data)
+            latencies.append(time.perf_counter() - t)
+
+        return OliveEvaluator.compute_latency(metric, latencies)
+
+
+class OliveEvaluatorFactory:
+    @staticmethod
+    def create_evaluator_for_model(model: OliveModel) -> OliveEvaluator:
+        evaluator_cls = OliveEvaluator.registry[str(model.framework).lower()]
+        return evaluator_cls()
 
 
 class OliveEvaluatorConfig(ConfigBase):
-    metrics: List[Metric]
-    target: SystemConfig = SystemConfig(type=SystemType.Local)
+    metrics: List[Metric] = []
 
     @validator("metrics")
     def validate_metrics(cls, v):
+        metric_len = len(v)
+        if metric_len == 1:
+            return v
+
         metric_names = set([metric.name for metric in v])
-        assert len(metric_names) == len(v), "Metric names must be unique"
-        return v
+        assert len(metric_names) == metric_len, "Metric names must be unique"
 
-    def create_evaluator(self):
-        return OliveEvaluator(self.metrics, self.target.create_system())
+        rank_set = set([metric.priority_rank for metric in v])
+        expected_rank_set = set(range(1, metric_len + 1))
+        # Check if all ranks are present
+        if rank_set != expected_rank_set:
+            raise ValueError(f"Priority ranks must be unique and in the range 1 to {metric_len}")
+
+        return v
```

## olive/passes/olive_pass.py

```diff
@@ -1,160 +1,298 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from abc import abstractmethod
+import inspect
+import logging
+from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 
 from pydantic import validator
 
-from olive.common.auto_config import AutoConfigClass
 from olive.common.config_utils import ConfigBase, validate_config
 from olive.common.user_module_loader import UserModuleLoader
-from olive.model import OliveModel
+from olive.data.config import DataConfig
+from olive.model import CompositeOnnxModel, DistributedOnnxModel, OliveModel
 from olive.passes.pass_config import (
     PassConfigBase,
     PassConfigParam,
     PassParamDefault,
     create_config_class,
+    get_data_config,
     get_user_script_config,
 )
-from olive.strategy.search_parameter import Conditional, SearchParameter
-from olive.strategy.utils import cyclic_search_space
+from olive.strategy.search_parameter import (
+    Categorical,
+    Conditional,
+    ConditionalDefault,
+    SearchParameter,
+    SpecialParamValue,
+)
+from olive.strategy.search_space import SearchSpace
+from olive.strategy.utils import cyclic_search_space, order_search_parameters
+
+logger = logging.getLogger(__name__)
 
 
-class Pass(AutoConfigClass):
+class Pass(ABC):
     """
     Base class for pass configuration.
     Each pass should derive its own configuration class that contains all information it needs to execute.
     """
 
     registry: Dict[str, "Pass"] = {}
     # True if pass configuration requires user script for non-local host support
     _requires_user_script: bool = False
+    # True if pass configuration requires data configuration which will leverage data container for pass execution
+    _requires_data_config: bool = False
+    # True if the pass processes a composite model at once. Otherwise, the components of the
+    # composite model will be processed individually.
+    _accepts_composite_model: bool = False
 
-    def __init__(self, config: Union[Dict[str, Any], PassConfigBase], default_to_search: Optional[bool] = False):
+    @classmethod
+    def __init_subclass__(cls, **kwargs) -> None:
+        """Register the Pass."""
+        super().__init_subclass__(**kwargs)
+        if not inspect.isabstract(cls):
+            cls.registry[cls.__name__.lower()] = cls
+
+    def __init__(self, config_class: Type[PassConfigBase], config: Dict[str, Any]):
+        """Initialize the pass.
+
+        :param config_class: the PassConfig class with the default value or default search values.
+        :type config_class: Type[PassConfigBase]
+        :param config: the configuration representing search space.
+        :type config: Dict[str, Any]
         """
-        Initialize the pass.
-        default_to_search: If True, use default search parameters, if any, for parameters that are not specified
-        in the config. Only applies when the config is a dictionary.
-        """
-        self._config_class = self.get_config_class(default_to_search)
-        self._config = validate_config(config, PassConfigBase, self._config_class)
-        self._config = self._config.dict()
-        self._config = self._resolve_defaults(self._config)
+        self._config_class = config_class
+        self._config = config
         if self._requires_user_script:
             self._user_module_loader = UserModuleLoader(self._config["user_script"], self._config["script_dir"])
-            self._config = self._validate_user_script(self._config, self._user_module_loader)
-
-        self._fixed_params, self._search_space = self._init_fixed_and_search_params(self._config)
+        if self._requires_data_config:
+            data_config = self._config["data_config"] or {}
+            self._data_config = DataConfig(**data_config)
+
+        self._fixed_params = {}
+        self._search_space = {}
+        for k, v in self._config.items():
+            if isinstance(v, SearchParameter):
+                self._search_space[k] = v
+            else:
+                self._fixed_params[k] = v
 
         # Params that are paths [(param_name, required)]
         self.path_params = []
-        for param, param_config in self.default_config().items():
+        for param, param_config in self._config_class._default_config.items():
             if param_config.is_path:
                 self.path_params.append((param, param_config.required))
 
         self._initialized = False
 
     @classmethod
-    def get_config_class(cls, default_to_search: Optional[bool] = False) -> Type[PassConfigBase]:
+    def requires_data_config(cls):
+        return cls._requires_data_config
+
+    @classmethod
+    def generate_search_space(
+        cls, config: Optional[Union[Dict[str, Any], PassConfigBase]] = None, disable_search: Optional[bool] = False
+    ) -> Tuple[Type[PassConfigBase], Dict[str, Any]]:
+        """
+        Generate search space for the pass.
+        """
+        default_config = cls.default_config()
+        # Get the config class with default value or default search value
+        config_class = cls.get_config_class(default_config, disable_search)
+        # Generate the search space by using both default value and default search value and user provided config
+        config = cls._resolve_config(config_class, config, default_config)
+        config = cls._init_fixed_and_search_params(config, default_config)
+        return config_class, config
+
+    @classmethod
+    def get_config_class(
+        cls, default_config: Dict[str, PassConfigParam], disable_search: Optional[bool] = False
+    ) -> Type[PassConfigBase]:
         """
         Get the configuration class for the pass.
         """
-        return create_config_class(cls.__name__, cls.default_config(), default_to_search, cls._validators())
+        return create_config_class(cls.__name__, default_config, disable_search, cls._validators())
 
     @classmethod
     def default_config(cls) -> Dict[str, PassConfigParam]:
         """
         Get the default configuration for the pass.
         """
         config = {}
         if cls._requires_user_script:
             config.update(get_user_script_config())
+        if cls.requires_data_config():
+            config.update(get_data_config())
         return {**config, **cls._default_config()}
 
     @staticmethod
+    def _validators() -> Dict[str, Callable]:
+        """
+        pydantic validators for config params
+        """
+        return {}
+
+    @staticmethod
     @abstractmethod
     def _default_config() -> Dict[str, PassConfigParam]:
         """
         Get the default configuration for the pass. Doesn't include user_script and script_dir.
+
+        Example:
+            return {
+                # required parameter
+                "param1": PassConfigParam(type_=int, required=True, description="param1 description"),
+                # optional parameter with default value
+                "param2": PassConfigParam(type_=int, default_value=1, description="param2 description"),
+                # optional parameter with default value and searchable values
+                "param3": PassConfigParam(
+                    type_=int,
+                    default_value=1,
+                    searchable_values=Categorical([1, 2, 3]),
+                    description="param3 description",
+                ),
+                # optional parameter with `is_object` set to True
+                # the value of this parameter can be a string or a function that takes a string and returns the object,
+                # say a class ObjectClass
+                "param4": PassConfigParam(
+                    type_=Union[str, Callable[[str], Pass]], is_object=True, description="param4 description"
+                ),
+                # optional parameter with default_value that depends on another parameter value
+                "param5": PassConfigParam(
+                    type_=int,
+                    default_value=ConditionalDefault(parents="param2", support={(1,): 2, (2,): 3}, default=4),
+                    description="param5 description",
+                ),
+                # optional parameter with searchable_values that depends on other parameter values
+                "param6": PassConfigParam(
+                    type_=int,
+                    default_value=1,
+                    searchable_values=Conditional(
+                        parents=("param2", "param3"),
+                        # invalid if (param2, param3) not in [(1, 1), (1, 2)]
+                        support={
+                            (1, 1): Categorical([1, 2, 3]),
+                            (1, 2): Categorical([4, 5, 6]),
+                        },
+                    ),
+                    description="param6 description",
+                ),
+            }
         """
         raise NotImplementedError()
 
-    def _resolve_defaults(self, config: Dict[str, Any]) -> Dict[str, Any]:
+    @classmethod
+    def _resolve_defaults(cls, config: Dict[str, Any], default_config: Dict[str, PassConfigParam]) -> Dict[str, Any]:
         """
         Resolve default values.
         """
-        default_config = self.default_config()
         for key, value in config.items():
-            if value == PassParamDefault.DEFAULT:
-                config[key] = default_config[key].default
-            elif value == PassParamDefault.DEFAULT_SEARCH:
-                default_search = default_config[key].default_search
-                assert default_search is not None, f"Parameter {key} does not have a default search."
-                config[key] = default_search
+            if value == PassParamDefault.DEFAULT_VALUE:
+                config[key] = default_config[key].default_value
+            elif value == PassParamDefault.SEARCHABLE_VALUES:
+                value = default_config[key].searchable_values
+                if value is None:
+                    logger.warning(f"Parameter {key} does not have searchable values. Using default value instead.")
+                    value = default_config[key].default_value
+                config[key] = value
         return config
 
-    def _validate_user_script(self, config: Dict[str, Any], user_module_loader: UserModuleLoader) -> Dict[str, Any]:
+    @classmethod
+    def _validate_user_script(
+        cls, config: Dict[str, Any], user_module_loader: UserModuleLoader, default_config: Dict[str, PassConfigParam]
+    ) -> Dict[str, Any]:
         """
         Validate callables in the config.
         """
-        default_config = self.default_config()
         for key, value in config.items():
             if default_config[key].is_object and isinstance(value, str):
-                assert user_module_loader is not None, f"'user_script' must be specified if a {key} is a string."
+                assert user_module_loader.user_script, f"'user_script' must be specified if a {key} is a string."
         # TODO: once convention for user_script and script dir is finalized, let config class handle
         # the resolution during serialization
         if config["user_script"] is not None:
             config["user_script"] = str(Path(config["user_script"]).resolve())
         if config["script_dir"] is not None:
             config["script_dir"] = str(Path(config["script_dir"]).resolve())
         return config
 
+    @classmethod
     def _init_fixed_and_search_params(
-        self, config: Dict[str, Any]
+        cls, config: Dict[str, Any], default_config: Dict[str, PassConfigParam]
     ) -> Tuple[Dict[str, Any], Dict[str, SearchParameter]]:
         """
         Get the fixed and search parameters from the config.
         """
-        default_config = self.default_config()
+        param_order = order_search_parameters(config)
 
         # fixed parameters
         fixed_params = {}
-        for key, value in config.items():
-            if isinstance(value, SearchParameter):
-                continue
-            if default_config[key].is_path and value is not None:
-                value = str(Path(value).resolve())
-            fixed_params[key] = value
-
-        # search parameters
         search_space = {}
-        for key, value in config.items():
+        for key in param_order:
+            value = config[key]
+            if isinstance(value, SearchParameter):
+                # resolve conditional parameters
+                # if categorical with single choice, use that choice directly
+                value = cls._resolve_search_parameter(value, fixed_params)
+            if value == SpecialParamValue.INVALID:
+                # TODO: better error message, e.g. what the parent values were, how it was invalid
+                raise ValueError(
+                    f"Invalid value for parameter '{key}'. Either the parameter or its parents are not fixed."
+                )
             if isinstance(value, SearchParameter):
-                search_space[key] = self._resolve_search_parameter(value, fixed_params)
+                search_space[key] = value
+            else:
+                if default_config[key].is_path and value is not None:
+                    value = str(Path(value).resolve())
+                fixed_params[key] = value
         assert not cyclic_search_space(search_space), "Search space is cyclic."
+        # TODO: better error message, e.g. which parameters are invalid, how they are invalid
+        assert SearchSpace({"search_space": search_space}).size() > 0, "There are no valid points in the search space."
 
-        return fixed_params, search_space
+        return {**fixed_params, **search_space}
 
-    def _resolve_search_parameter(self, param: SearchParameter, fixed_params: Dict[str, Any]) -> Any:
+    @classmethod
+    def _resolve_search_parameter(cls, param: SearchParameter, fixed_params: Dict[str, Any]) -> Any:
         """
         Resolve a search parameter.
         """
         if isinstance(param, Conditional):
             # if value is conditional and one/more parents are fixed, use the condition to get new value
             parent_values = {parent: fixed_params[parent] for parent in param.parents if parent in fixed_params}
-            if len(parent_values) == 0:
-                return param
-            else:
-                return param.condition(parent_values)
-        else:
-            return param
+            if len(parent_values) > 0:
+                param = param.condition(parent_values)
+            if isinstance(param, ConditionalDefault):
+                # if there are still searchable parents, convert to conditional
+                param = ConditionalDefault.conditional_default_to_conditional(param)
+        if isinstance(param, Categorical) and len(param.get_support()) == 1:
+            # if there is only one choice, use that choice
+            param = param.get_support()[0]
+        return param
+
+    @classmethod
+    def _resolve_config(
+        cls,
+        config_class: Type[PassConfigBase],
+        input_config: Union[Dict[str, Any], PassConfigBase],
+        default_config: Dict[str, PassConfigParam],
+    ) -> Dict[str, Any]:
+        """
+        Resolve config to PassConfigBase.
+        """
+        config = validate_config(input_config, PassConfigBase, config_class)
+        config = config.dict()
+        config = cls._resolve_defaults(config, default_config)
+        if cls._requires_user_script:
+            user_module_loader = UserModuleLoader(config["user_script"], config["script_dir"])
+            config = cls._validate_user_script(config, user_module_loader, default_config)
+        return config
 
     def _initialize(self):
         """
         Initialize the pass. Pass specific initialization should be done here.
         """
         pass
 
@@ -176,14 +314,20 @@
 
     def validate_search_point(self, search_point: Dict[str, Any]) -> bool:
         """
         Validate the search point for the pass.
         """
         return True
 
+    def filter_ignored_params(self, config: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Filter out ignored parameters.
+        """
+        return {key: value for key, value in config.items() if value != SpecialParamValue.IGNORED}
+
     @abstractmethod
     def _run_for_config(self, model: OliveModel, config: Dict[str, Any], output_model_path: str) -> OliveModel:
         """
         Run the pass on the model with the given configuration.
         """
         raise NotImplementedError()
 
@@ -194,48 +338,67 @@
         point = point or {}
         config = self.config_at_search_point(point)
 
         if not self._initialized:
             self._initialize()
             self._initialized = True
 
+        # Optimization pass still works on individual graphs.
+        if isinstance(model, DistributedOnnxModel):
+            output_filepaths = []
+            for rank in range(0, model.ranks):
+                input_rank_model = model.load_model(rank)
+                rank_output_path = Path(output_model_path).with_suffix("") / str(rank)
+                output_rank_model = self._run_for_config(input_rank_model, config, rank_output_path)
+                output_filepaths.append(output_rank_model.model_path)
+            return DistributedOnnxModel(
+                output_filepaths, model.name, version=model.version, inference_settings=model.inference_settings
+            )
+        elif isinstance(model, CompositeOnnxModel) and not self._accepts_composite_model:
+            components = []
+            for cidx, child in enumerate(model.get_model_components()):
+                component_output_path = Path(output_model_path).with_suffix("") / str(cidx)
+                components.append(self._run_for_config(child, config, str(component_output_path)))
+            return CompositeOnnxModel(components, model.name, hf_config=model.hf_config)
+
         return self._run_for_config(model, config, output_model_path)
 
     def serialize_config(self, config: Dict[str, Any], check_objects: bool = False) -> str:
         """
         Serialize the configuration.
         """
         return self._config_class(**config).to_json(check_objects)
 
     def to_json(self, check_objects: bool = False) -> Dict[str, Any]:
         """
         Convert the pass to json.
         """
-        return {"type": self.__class__.__name__, "config": self.serialize_config(self._config, check_objects)}
+        return {
+            "type": self.__class__.__name__,
+            "disable_search": True,
+            "config": self.serialize_config(self._config, check_objects),
+        }
 
 
 # TODO rename. We are using FullPassConfig since PassConfigBase already refers to inner config
 class FullPassConfig(ConfigBase):
     type: str
-    default_to_search: bool = False
-    config: PassConfigBase = None
+    disable_search: bool = False
+    config: Dict[str, Any] = None
 
     @validator("type")
     def validate_type(cls, v):
         if v.lower() not in Pass.registry:
             raise ValueError(f"Unknown pass type {v}")
         return v
 
-    @validator("config", pre=True, always=True)
-    def validate_config(cls, v, values):
-        if "type" not in values:
-            raise ValueError("Invalid type")
-        if "default_to_search" not in values:
-            raise ValueError("Invalid default_to_search")
-
-        pass_type = values["type"].lower()
-        default_to_search = values["default_to_search"]
-        config_class = Pass.registry[pass_type].get_config_class(default_to_search)
-        return validate_config(v, PassConfigBase, config_class)
-
     def create_pass(self):
-        return Pass.registry[self.type.lower()](self.config, self.default_to_search)
+        pass_cls = Pass.registry[self.type.lower()]
+        return create_pass_from_dict(pass_cls, self.config, self.disable_search)
+
+
+def create_pass_from_dict(pass_cls: Type[Pass], config: Dict[str, Any] = None, disable_search=False) -> Pass:
+    """
+    Create a pass from a dictionary.
+    """
+    config_class, config = pass_cls.generate_search_space(config, disable_search)
+    return pass_cls(config_class, config)
```

## olive/passes/pass_config.py

```diff
@@ -5,32 +5,46 @@
 from enum import Enum
 from pathlib import Path
 from typing import Callable, Dict, Optional, Type, Union
 
 from pydantic import create_model, validator
 
 from olive.common.config_utils import ConfigBase, ConfigParam, validate_object
+from olive.data.config import DataConfig
 from olive.strategy.search_parameter import SearchParameter, json_to_search_parameter
 
 
 class PassParamDefault(str, Enum):
     """
     Default values for passes.
     """
 
-    DEFAULT = "DEFAULT"
-    DEFAULT_SEARCH = "DEFAULT_SEARCH"
+    DEFAULT_VALUE = "DEFAULT_VALUE"
+    SEARCHABLE_VALUES = "SEARCHABLE_VALUES"
 
 
 class PassConfigParam(ConfigParam):
     """
     Dataclass for pass configuration parameters.
+
+    Parameters
+    ----------
+    type_ : type of the parameter
+    required : whether the parameter is required
+    is_object : whether the parameter is an object/function. If so, this parameter accepts the object or a string with
+        the name of the object/function in the user script. The type must include str.
+    is_path : whether the parameter is a path. If so, this file/folder will be uploaded to the host system.
+    description : description of the parameter
+    default_value: default value for the parameter. This value is used if search is disabled or there are no searchable
+        values. Must be the same type as the parameter or a ConditionalDefault SearchParameter.
+    searchable_values: default searchable values for the parameter. This value is used if search is enabled.
+        Must be a Categorical or Conditional SearchParameter.
     """
 
-    default_search: SearchParameter = None
+    searchable_values: SearchParameter = None
     is_path: bool = False
 
     def __repr__(self):
         repr_list = []
         booleans = ["required", "is_path", "is_object"]
         for k, v in self.__dict__.items():
             if k in booleans:
@@ -62,14 +76,28 @@
                 " be imported from this script."
             ),
         ),
     }
     return user_script_config
 
 
+def get_data_config(required: Optional[bool] = False):
+    data_config = {
+        "data_config": PassConfigParam(
+            type_=Union[DataConfig, str],
+            required=required,
+            description="""
+                Data config for calibration, required if quant_mode is 'static'.
+                If not provided, a default DataConfig will be used.
+            """,
+        )
+    }
+    return data_config
+
+
 class PassConfigBase(ConfigBase):
     @validator("*", pre=True)
     def _validate_default_str(cls, v, field):
         try:
             v = PassParamDefault(v)
         finally:
             if field.required and isinstance(v, PassParamDefault):
@@ -82,15 +110,15 @@
             return json_to_search_parameter(v)
         return v
 
 
 def create_config_class(
     pass_type: str,
     default_config: Dict[str, PassConfigParam],
-    default_to_search: Optional[bool] = True,
+    disable_search: Optional[bool] = False,
     validators: Dict[str, Callable] = None,
 ) -> Type[PassConfigBase]:
     """
     Create a Pydantic model class from a configuration dictionary.
     """
     config = {}
     validators = validators.copy() if validators else {}
@@ -99,14 +127,17 @@
             validators[f"validate_{param}"] = validator(param, allow_reuse=True)(validate_object)
 
         type_ = param_config.type_
         if param_config.required:
             config[param] = (type_, ...)
             continue
 
-        type_ = Union[type_, SearchParameter, PassParamDefault]
-        if default_to_search and param_config.default_search is not None:
-            config[param] = (type_, param_config.default_search)
+        type_ = Optional[Union[type_, SearchParameter, PassParamDefault]]
+        if not disable_search and param_config.searchable_values is not None:
+            config[param] = (type_, param_config.searchable_values)
         else:
-            config[param] = (type_, param_config.default)
+            config[param] = (type_, param_config.default_value)
+
+    class PassConfigBaseDefaultConfig(PassConfigBase):
+        _default_config = default_config  # store default config as a class attribute, not included in json
 
-    return create_model(f"{pass_type}Config", **config, __base__=PassConfigBase, __validators__=validators)
+    return create_model(f"{pass_type}Config", **config, __base__=PassConfigBaseDefaultConfig, __validators__=validators)
```

## olive/passes/onnx/__init__.py

```diff
@@ -1,19 +1,33 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
+from olive.passes.onnx.append_pre_post_processing_ops import AppendPrePostProcessingOps
 from olive.passes.onnx.conversion import OnnxConversion
+from olive.passes.onnx.float16_conversion import OnnxFloatToFloat16
+from olive.passes.onnx.inc_quantization import IncDynamicQuantization, IncQuantization, IncStaticQuantization
+from olive.passes.onnx.insert_beam_search import InsertBeamSearch
+from olive.passes.onnx.mixed_precision import OrtMixedPrecision
 from olive.passes.onnx.model_optimizer import OnnxModelOptimizer
 from olive.passes.onnx.perf_tuning import OrtPerfTuning
 from olive.passes.onnx.quantization import OnnxDynamicQuantization, OnnxQuantization, OnnxStaticQuantization
 from olive.passes.onnx.transformer_optimization import OrtTransformersOptimization
+from olive.passes.onnx.vitis_ai_quantization import VitisAIQuantization
 
 __all__ = [
+    "AppendPrePostProcessingOps",
     "OnnxConversion",
     "OnnxDynamicQuantization",
     "OnnxQuantization",
     "OnnxStaticQuantization",
+    "IncDynamicQuantization",
+    "IncQuantization",
+    "IncStaticQuantization",
     "OrtPerfTuning",
     "OrtTransformersOptimization",
     "OnnxModelOptimizer",
+    "OnnxFloatToFloat16",
+    "InsertBeamSearch",
+    "OrtMixedPrecision",
+    "VitisAIQuantization",
 ]
```

## olive/passes/onnx/conversion.py

```diff
@@ -1,18 +1,22 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
+import tempfile
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Dict, Union
 
+import onnx
 import torch
 
-from olive.model import ONNXModel, PyTorchModel
+from olive.common.utils import tensor_data_to_device
+from olive.model import CompositeOnnxModel, ONNXModel, PyTorchModel
 from olive.passes import Pass
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 
 
 class TraceModelWrapper(torch.nn.Module):
     def __init__(self, model: torch.nn.Module):
         super().__init__()
         self.model = model
@@ -25,112 +29,87 @@
 
 class OnnxConversion(Pass):
     """Convert a PyTorch model to ONNX model using torch.onnx.export."""
 
     _requires_user_script = True
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
-        return {
-            "input_names": PassConfigParam(type_=List[str], required=True, description="List of input names."),
-            # required for if input_tensors_func is not provided
-            "input_shapes": PassConfigParam(
-                type_=List[List[int]],
-                default=None,
-                description=(
-                    "List of input shapes. Must be provided if input_tensor_func is not provided. It is used to create"
-                    " dummy inputs for the model during onnx export."
-                ),
-            ),
-            "input_types": PassConfigParam(
-                type_=List[str],
-                default=None,
-                description=(
-                    "List of input types. If provided, must be the same length as input_shapes. Otherwise, defaults to"
-                    " float32 for all inputs. Used with input_shapes to create dummy inputs for the model during onnx"
-                    " export."
-                ),
-            ),
-            "input_tensor_func": PassConfigParam(
-                type_=Union[Callable, str],
-                default=None,
-                is_object=True,
-                description=(
-                    "Function (no input) to create dummy inputs for the model. Can be a function (local use) or name of"
-                    " a function to be imported from user script. If provided, input_shapes and input_types will be"
-                    " ignored. Refer to 'args' at https://pytorch.org/docs/stable/onnx.html#torch.onnx.export for more"
-                    " details."
-                ),
-            ),
-            "output_names": PassConfigParam(type_=List[str], required=True, description="List of output names."),
-            "dynamic_axes": PassConfigParam(
-                type_=dict,
-                default=None,
-                description=(
-                    "Dynamic axes for the model. Refer to 'dynamic_axes' at"
-                    " https://pytorch.org/docs/stable/onnx.html#torch.onnx.export for more details."
-                ),
-            ),
+    def _default_config() -> Dict[str, PassConfigParam]:
+        config = {
             "target_opset": PassConfigParam(
-                type_=int, default=14, description="The version of the default (ai.onnx) opset to target."
-            ),
+                type_=int, default_value=14, description="The version of the default (ai.onnx) opset to target."
+            )
         }
+        config.update(get_external_data_config())
+        return config
 
-    def _initialize(self):
-        # input shapes
-        self._fixed_params["input_shapes"] = self._fixed_params["input_shapes"] or []
-
-        # input types
-        str_to_type = {"float32": torch.float32, "float16": torch.float16, "int32": torch.int32, "int64": torch.int64}
-        input_types = []
-        if self._fixed_params["input_types"] is not None:
-            for input_type in self._fixed_params["input_types"]:
-                input_types.append(str_to_type[input_type])
-        else:
-            input_types = [str_to_type["float32"] for _ in self._fixed_params["input_shapes"]]
-
-        assert not (
-            self._fixed_params["input_tensor_func"] and self._fixed_params["input_shapes"]
-        ), "Either input_tensor_func or input_shapes must be provided."
-
-        # dummy inputs
-        self._dummy_inputs = []
-        if self._fixed_params["input_tensor_func"] is not None:
-            self._dummy_inputs = self._user_module_loader.call_object(self._fixed_params["input_tensor_func"])
-        else:
-            for input_shape, input_type in zip(self._fixed_params["input_shapes"], input_types):
-                self._dummy_inputs.append(torch.zeros(input_shape, dtype=input_type))
-            self._dummy_inputs = tuple(self._dummy_inputs) if len(self._dummy_inputs) > 1 else self._dummy_inputs[0]
-
-        # dynamic axes
-        self._dynamic_axes = {}
-        if self._fixed_params["dynamic_axes"] is not None:
-            for name in self._fixed_params["dynamic_axes"]:
-                self._dynamic_axes[name] = {
-                    int(key): value for key, value in self._fixed_params["dynamic_axes"][name].items()
-                }
-        else:
-            self._dynamic_axes = None
+    def _run_for_config(
+        self, model: PyTorchModel, config: Dict[str, Any], output_model_path: str
+    ) -> Union[ONNXModel, CompositeOnnxModel]:
+        # check if the model has components
+        if model.components:
+            onnx_models = []
+            for component_name in model.components:
+                component_model = model.get_component(component_name)
+                component_output_path = Path(output_model_path).with_suffix("") / component_name
+                onnx_models.append(self._run_for_config(component_model, config, str(component_output_path)))
+            return CompositeOnnxModel(onnx_models, hf_config=model.hf_config)
+
+        # get dummy inputs
+        dummy_inputs = model.get_dummy_inputs()
+
+        # get input and output names, and dynamic axes
+        assert model.io_config, "Model IO config is not set."
+        input_names = model.io_config.input_names
+        output_names = model.io_config.output_names
+        dynamic_axes = model.io_config.dynamic_axes
 
-    def _run_for_config(self, model: PyTorchModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
+        # convert the model
         pytorch_model = model.load_model()
         pytorch_model.eval()
+
+        # TODO: add e2e test for model on cpu but data on gpu; model on gpu but data on cpu
+        # put pytorch_model and dummy_inputs at the same device
+        pytorch_model.to("cpu")
+        dummy_inputs = tensor_data_to_device(dummy_inputs, "cpu")
         if isinstance(pytorch_model, torch.jit.RecursiveScriptModule):
             pytorch_model = TraceModelWrapper(pytorch_model)
 
-        if Path(output_model_path).suffix != ".onnx":
-            output_model_path += ".onnx"
+        output_model_path = ONNXModel.resolve_path(output_model_path)
+
+        # there might be multiple files created during export, so we need to track the dir
+        # if there are other processes writing to the same dir, we might end up deleting files created by
+        # other processes
+        tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp")
+        tmp_dir_path = Path(tmp_dir.name)
+        tmp_model_path = str(tmp_dir_path / Path(output_model_path).name)
 
         torch.onnx.export(
             pytorch_model,
-            # TODO: support custom input tensor. Will implement once we decide how to handle non-hashable config params
-            self._dummy_inputs,
-            output_model_path,
+            dummy_inputs,
+            tmp_model_path,
             export_params=True,
             opset_version=config["target_opset"],
-            input_names=config["input_names"],
-            output_names=config["output_names"],
-            dynamic_axes=self._dynamic_axes,
+            input_names=input_names,
+            output_names=output_names,
+            dynamic_axes=dynamic_axes,
         )
 
-        model = ONNXModel(output_model_path, model.name)
-        return model
+        # load the model
+        onnx_model = onnx.load(tmp_model_path)
+        # the model is loaded into memory, so it's safe to delete previously exported file(s)
+        tmp_dir.cleanup()
+
+        # Workaround as described under IOConfig.string_to_int_dim_params: change numeric dim_param to dim_value
+        if model.io_config.string_to_int_dim_params:
+            for tensor in onnx_model.graph.output:
+                for dim_proto in tensor.type.tensor_type.shape.dim:
+                    if (
+                        dim_proto.HasField("dim_param")
+                        and dim_proto.dim_param in model.io_config.string_to_int_dim_params
+                    ):
+                        dim_value = int(dim_proto.dim_param)
+                        dim_proto.Clear()
+                        dim_proto.dim_value = dim_value
+
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(onnx_model, output_model_path, config, model.name)
```

## olive/passes/onnx/model_optimizer.py

```diff
@@ -1,29 +1,30 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from pathlib import Path
 from typing import Any, Dict
 
 import numpy as np
 import onnx
-from onnxruntime.transformers.onnx_model import OnnxModel as TransformersOnnxModel
 
 from olive.model import ONNXModel
 from olive.passes import Pass
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
+from olive.passes.pass_config import PassConfigParam
 
 
 class ModelOptimizer:
-    def __init__(self, source_model_path, target_model_path):
+    def __init__(self, source_model_path):
         self.source_model_path = str(source_model_path)
-        self.target_model_path = str(target_model_path)
         self.prepare()
 
     def prepare(self):
+        from onnxruntime.transformers.onnx_model import OnnxModel as TransformersOnnxModel
+
         self.model = onnx.load(self.source_model_path)
         self.onnx_model = TransformersOnnxModel(self.model)
         self.graph = self.onnx_model.graph()
 
         node_idx = 0
         self.node_name2module = dict()
 
@@ -56,16 +57,14 @@
 
                     self.remove_nodes(self.graph, [node, dequant_node, x_node, x_scale_node, x_zero_point_node])
                     new_dequant, x, x_scale, x_zero_point = self.create_dequantizelinear_node(
                         new_x_val, x_scale_val, x_zero_point_val, new_dequant_node_output, node_index
                     )
                     self.add_nodes(self.graph, [new_dequant, x, x_scale, x_zero_point], node_index)
 
-        onnx.save(self.onnx_model.model, self.target_model_path)
-
     def create_dequantizelinear_node(self, x_val, x_scale_val, x_zero_point_val, outputs, node_name_suffix):
         x_tensor = onnx.helper.make_tensor(
             name="const_tensor",
             data_type=onnx.TensorProto.DataType.INT8,
             dims=x_val.shape,
             vals=x_val.flatten().tobytes(),
             raw=True,
@@ -115,17 +114,19 @@
             graph.node.insert(node_index, node)
 
 
 class OnnxModelOptimizer(Pass):
     """Optimize ONNX model by fusing nodes."""
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
-        return {}
+    def _default_config() -> Dict[str, PassConfigParam]:
+        return get_external_data_config()
 
     def _run_for_config(self, model: ONNXModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
-        if Path(output_model_path).suffix != ".onnx":
-            output_model_path += ".onnx"
+        output_model_path = ONNXModel.resolve_path(output_model_path)
 
-        model_optimizer = ModelOptimizer(model.model_path, output_model_path)
+        # optimize model
+        model_optimizer = ModelOptimizer(model.model_path)
         model_optimizer.optimize()
-        return ONNXModel(output_model_path, model.name)
+
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(model_optimizer.model, output_model_path, config, model.name)
```

## olive/passes/onnx/perf_tuning.py

```diff
@@ -2,65 +2,78 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import copy
 import itertools
 import logging
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable, Dict, Union
 
-import onnxruntime as ort
-import psutil
-
-from olive.evaluator.evaluation import evaluate_latency
 from olive.evaluator.metric import LatencySubType, Metric, MetricType
+from olive.evaluator.metric_config import get_properties_from_metric_type
 from olive.model import ONNXModel
 from olive.passes import Pass
 from olive.passes.pass_config import PassConfigParam
 
 logger = logging.getLogger(__name__)
 
 
-def generate_tuning_combos(config):
-    providers_list = config.providers_list if config.providers_list else ort.get_available_providers()
+def generate_tuning_combos(model, config):
+    import onnxruntime as ort
+
+    providers_list = config.providers_list if config.providers_list else model.get_execution_providers(config.device)
     execution_mode_list = (
         config.execution_mode_list
         if config.execution_mode_list
         else [ort.ExecutionMode.ORT_SEQUENTIAL.value, ort.ExecutionMode.ORT_PARALLEL.value]
     )
     opt_level_list = config.opt_level_list if config.opt_level_list else [99]
 
-    io_bind_list = None
-    if isinstance(config.io_bind, list):
-        io_bind_list = config.io_bind
-    elif isinstance(config.io_bind, bool):
-        io_bind_list = [config.io_bind]
-    else:
-        io_bind_list = [False]
+    io_bind_list = [True, False] if config.io_bind else [False]
 
     tuning_combos = itertools.product(providers_list, execution_mode_list, opt_level_list, io_bind_list)
     yield from tuning_combos
 
 
+def valid_config(tuning_combos):
+    # the order of combos: "provider", "execution_mode", "ort_opt_level", "io_bind"
+
+    # Parallel execution mode does not support the CUDA Execution Provider.
+    # So ORT will make the execution mode sequential when it uses the CUDA Execution Provider.
+
+    # if the first combo is CPUExecutionProvider, then the io_bind should not be True
+    if tuning_combos[0] == "CPUExecutionProvider" and tuning_combos[3]:
+        logger.info("[Skipped] Because EPs is CPUExecutionProvider, the io_bind should not be True")
+        return False
+    return True
+
+
 def tune_onnx_model(model, config):
-    latency_user_config = config.dict()
-    latency_user_config.pop("io_bind")
+    latency_user_config = {}
+    # which should be the same as the config in the metric
+    config_dict = config.dict()
+    for eval_config in get_properties_from_metric_type(MetricType.LATENCY):
+        if eval_config in config_dict:
+            latency_user_config[eval_config] = config_dict.get(eval_config)
     latency_metric = Metric(
         name="latency", type=MetricType.LATENCY, sub_type=LatencySubType.AVG, user_config=latency_user_config
     )
 
     pretuning_inference_result = get_benchmark(model, latency_metric, config)
 
     tuning_results = []
-    for tuning_combo in generate_tuning_combos(config):
-        logger.info("Run tuning for: {}".format(tuning_combo))
-        if tuning_combo[0] == "CPUExecutionProvider" and tuning_combo[3]:
+    for tuning_combo in generate_tuning_combos(model, config):
+        tuning_item = ["provider", "execution_mode", "ort_opt_level", "io_bind"]
+        logger.info("Run tuning for: {}".format(list(zip(tuning_item, tuning_combo))))
+        if not valid_config(tuning_combo):
             continue
         tuning_results.extend(threads_num_tuning(model, latency_metric, config, tuning_combo))
-        logger.info("Current tuning results: {}".format(tuning_results[-1]["latency_ms"]))
+
+    for tuning_result in tuning_results:
+        logger.debug("Tuning result: {}".format(tuning_result["latency_ms"]))
 
     best_result = parse_tuning_result(*tuning_results, pretuning_inference_result)
     logger.info("Best result: {}".format(best_result))
     if best_result.get("test_name") != "pretuning":
         optimized_model = copy.copy(model)
         optimized_model.inference_settings = {
             "execution_provider": best_result.get("execution_provider"),
@@ -106,14 +119,17 @@
         logging.error("Optimization failed for tuning combo {}".format(tuning_combo))
         pass
 
     return tuning_results
 
 
 def threads_num_binary_search(model, latency_metric, config, test_params, tuning_results):
+    import onnxruntime as ort
+    import psutil
+
     if test_params["session_options"].get("extra_session_config"):
         extra_session_config = test_params["session_options"].get("extra_session_config")
         if extra_session_config.get("session.intra_op_thread_affinities"):
             affinity_str = extra_session_config.get("session.intra_op_thread_affinities")
             test_params["session_options"]["intra_op_num_threads"] = get_thread_affinity_nums(affinity_str) + 1
             threads_names = ["inter_op_num_threads"]
     elif test_params["session_options"].get("execution_mode") == ort.ExecutionMode.ORT_SEQUENTIAL:
@@ -172,14 +188,16 @@
         test_name = "_".join(["_".join([str(v) for v in i]) for i in test_params.items()])
     else:
         test_name = "pretuning"
     return test_name
 
 
 def get_benchmark(model, latency_metric, config, test_params=None):
+    from olive.evaluator.olive_evaluator import OliveEvaluatorFactory
+
     test_result = {}
     session_name = generate_test_name(test_params)
     test_result["test_name"] = session_name
 
     if test_params:
         # params starts with _ are not used in inference setting, we need add special handling for io_bind
         io_bind = test_params.pop("_io_bind", False)
@@ -188,15 +206,16 @@
         latency_metric.user_config.inference_settings = {"onnx": test_params}
         test_result["execution_provider"] = test_params.get("execution_provider")
         test_result["session_options"] = test_params.get("session_options").copy()
         test_result["io_bind"] = io_bind
 
         # add the io_bind back to test_params
         test_params["_io_bind"] = io_bind
-    test_result["latency_ms"] = evaluate_latency(model, latency_metric, config.device)
+    evaluator = OliveEvaluatorFactory.create_evaluator_for_model(model)
+    test_result["latency_ms"] = evaluator.evaluate(model, [latency_metric], config.device)[latency_metric.name]
     return test_result
 
 
 def parse_tuning_result(*tuning_results):
     best_result = min(tuning_results, key=lambda x: x["latency_ms"])
     return best_result
 
@@ -206,56 +225,71 @@
     return len(affinities)
 
 
 class OrtPerfTuning(Pass):
     """Optimize ONNX Runtime inference settings."""
 
     _requires_user_script = True
+    _requires_data_config = True
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         return {
             "data_dir": PassConfigParam(
                 type_=Union[Path, str], is_path=True, description="Directory of sample inference data."
             ),
             "dataloader_func": PassConfigParam(
                 type_=Union[Callable, str],
-                required=True,
                 is_object=True,
                 description="Dataloader function to load data from given data_dir with given batch size.",
             ),
-            "batch_size": PassConfigParam(type_=int, required=True, description="Batch size for inference."),
-            "device": PassConfigParam(type_=str, default="cpu", description="Device selected for tuning process."),
-            "cpu_cores": PassConfigParam(type_=int, default=None, description="CPU cores used for thread tuning."),
+            "batch_size": PassConfigParam(type_=int, description="Batch size for inference."),
+            "input_names": PassConfigParam(
+                type_=list, default_value=None, description="Input names list for ONNX model."
+            ),
+            "input_shapes": PassConfigParam(
+                type_=list, default_value=None, description="Input shapes list for ONNX model."
+            ),
+            "input_types": PassConfigParam(
+                type_=list, default_value=None, description="Input types list for ONNX model."
+            ),
+            "device": PassConfigParam(
+                type_=str, default_value="cpu", description="Device selected for tuning process."
+            ),
+            "cpu_cores": PassConfigParam(
+                type_=int, default_value=None, description="CPU cores used for thread tuning."
+            ),
             "io_bind": PassConfigParam(
-                type_=Union[bool, List[bool]],
-                default=False,
-                description="Whether enable IOBingding for ONNX Runimte infernece.",
+                type_=bool,
+                default_value=False,
+                description="Whether enable IOBinding Search for ONNX Runtime inference.",
             ),
             "providers_list": PassConfigParam(
-                type_=list, default=None, description="Execution providers framework list to execute the ONNX models."
+                type_=list,
+                default_value=None,
+                description="Execution providers framework list to execute the ONNX models.",
             ),
             "execution_mode_list": PassConfigParam(
-                type_=list, default=None, description="Parallelism list between operators."
+                type_=list, default_value=None, description="Parallelism list between operators."
             ),
             "opt_level_list": PassConfigParam(
-                type_=list, default=None, description="Optimization level list for ONNX model."
+                type_=list, default_value=None, description="Optimization level list for ONNX model."
             ),
             "trt_fp16_enable": PassConfigParam(
-                type_=bool, default=False, description="Whether enable FP16 mode for TensorRT execution provider."
+                type_=bool, default_value=False, description="Whether enable FP16 mode for TensorRT execution provider."
             ),
             "intra_thread_num_list": PassConfigParam(
-                type_=list, default=[None], description="List of intra thread number for test."
+                type_=list, default_value=[None], description="List of intra thread number for test."
             ),
             "inter_thread_num_list": PassConfigParam(
-                type_=list, default=[None], description="List of inter thread number for test."
+                type_=list, default_value=[None], description="List of inter thread number for test."
             ),
             "extra_session_config": PassConfigParam(
                 type_=Dict[str, Any],
-                default=None,
+                default_value=None,
                 description="Extra customized session options during tuning process.",
             ),
         }
 
     def _run_for_config(self, model: ONNXModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
         config = self._config_class(**config)
         # TODO: decide on whether to ignore the output_model_path
```

## olive/passes/onnx/quantization.py

```diff
@@ -2,106 +2,140 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 import tempfile
 from copy import deepcopy
 from pathlib import Path
-from shutil import copyfile
 from typing import Any, Callable, Dict, Union
 
-from onnxruntime.quantization import QuantFormat, QuantType, quantize_dynamic, quantize_static
-from onnxruntime.quantization.calibrate import CalibrationMethod
-from onnxruntime.quantization.preprocess import quant_pre_process
+import onnx
 
-from olive.model import ONNXModel
+from olive.common.utils import hash_string
+from olive.model import ModelStorageKind, ONNXModel
 from olive.passes import Pass
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_file, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
-from olive.strategy.search_parameter import Boolean, Categorical, Conditional
+from olive.strategy.search_parameter import Boolean, Categorical, Conditional, ConditionalDefault
 
 logger = logging.getLogger(__name__)
 
 # common config for both static and dynamic quantization
 _onnx_quantization_config = {
     "weight_type": PassConfigParam(
         type_=str,
-        default="QInt8",
-        default_search=Categorical(["QInt8", "QUInt8"]),
+        default_value="QInt8",
+        searchable_values=Categorical(["QInt8", "QUInt8"]),
         description="""
             Data type for quantizing weights which is used both in dynamic
             and static quantization. 'QInt8' for signed 8-bit integer,
             'QUInt8' for unsigned 8-bit integer.
         """,
     ),
     "op_types_to_quantize": PassConfigParam(
         type_=list,
-        default=None,
+        default_value=None,
         description="""
             List of operator types to quantize. If None, all quantizable.
         """,
     ),
     "nodes_to_quantize": PassConfigParam(
         type_=list,
-        default=None,
+        default_value=None,
         description="""
             List of node names to quantize. If None, all quantizable.
         """,
     ),
     "nodes_to_exclude": PassConfigParam(
         type_=list,
-        default=None,
+        default_value=None,
         description="""
             List of node names to exclude from quantization. If None, all quantizable.
         """,
     ),
     "per_channel": PassConfigParam(
         type_=bool,
-        default=False,
-        default_search=Boolean(),
+        default_value=False,
+        searchable_values=Boolean(),
         description="""
             Quantize weights per channel.
             Tips: When to use reduce_range and per-channel quantization:
             https://onnxruntime.ai/docs/performance/quantization.html#when-to-use-reduce-range-and-per-channel-quantization
         """,
     ),
     "reduce_range": PassConfigParam(
         type_=bool,
-        default=False,
-        default_search=Boolean(),
+        default_value=False,
+        searchable_values=Boolean(),
         description="""
             Quantize weights with 7-bits. It may improve the accuracy for
             some models running on non-VNNI machine, especially for per-channel mode.
             Tips: When to use reduce_range and per-channel quantization:
             https://onnxruntime.ai/docs/performance/quantization.html#when-to-use-reduce-range-and-per-channel-quantization
         """,
     ),
     "optimize_model": PassConfigParam(
         type_=bool,
-        default=False,
-        default_search=Boolean(),
+        default_value=False,
+        searchable_values=Boolean(),
         description="""
             Deprecating Soon in ONNX! Optimize model before quantization. NOT recommended, optimization will
             change the computation graph, making debugging of quantization loss difficult.
         """,
     ),
-    # TODO: enable search if we support onnx external data format
-    "use_external_data_format": PassConfigParam(
+    "quant_preprocess": PassConfigParam(
         type_=bool,
-        default=False,
+        default_value=True,
+        searchable_values=Boolean(),
         description="""
-            option used for large size (>2GB) model. Set to False by default.
+            Shape inference and model optimization, in preparation for quantization.
+            https://onnxruntime.ai/docs/performance/quantization.html#pre-processing
         """,
     ),
-    "quant_preprocess": PassConfigParam(
+}
+
+_exposed_extra_options_config = {
+    "extra.Sigmoid.nnapi": PassConfigParam(type_=bool, default_value=False, description=""),
+    "ActivationSymmetric": PassConfigParam(
+        type_=bool, default_value=False, description="symmetrize calibration data for activations"
+    ),
+    "WeightSymmetric": PassConfigParam(
+        type_=bool, default_value=True, description="symmetrize calibration data for weights"
+    ),
+    "EnableSubgraph": PassConfigParam(
+        type_=bool,
+        default_value=False,
+        description="If enabled, subgraph will be quantized. Dynamic mode currently is supported.",
+    ),
+    "ForceQuantizeNoInputCheck": PassConfigParam(
         type_=bool,
-        default=True,
-        default_search=Boolean(),
+        default_value=False,
         description="""
-            Shape inference and model optimization, in preparation for quantization.
-            https://onnxruntime.ai/docs/performance/quantization.html#pre-processing
+            By default, some latent operators like maxpool, transpose, do not quantize if their input is not
+            quantized already. Setting to True to force such operator always quantize input and so generate
+            quantized output. Also the True behavior could be disabled per node using the nodes_to_exclude.
+        """,
+    ),
+    "MatMulConstBOnly": PassConfigParam(
+        type_=bool,
+        default_value=ConditionalDefault(parents=("quant_mode",), support={("dynamic",): True, ("static",): False}),
+        description="If enabled, only MatMul with const B will be quantized.",
+    ),
+}
+
+_extra_options_config = {
+    "extra_options": PassConfigParam(
+        type_=dict,
+        default_value=None,
+        description=f"""
+            Key value pair dictionary for `extra_options` in quantization. Please refer to
+            https://github.com/microsoft/onnxruntime/blob/main/onnxruntime/python/tools/quantization/quantize.py
+            for details about the supported options. If an option is one of
+            {list(_exposed_extra_options_config.keys())}, it will be overwritten by the corresponding config parameter
+            value.
         """,
     ),
 }
 
 # static quantization specific config
 _static_dataloader_config = {
     "data_dir": PassConfigParam(
@@ -110,55 +144,65 @@
         description="""
             Path to the directory containing the dataset.
             For local data, it is required if quant_mode is 'static'.
         """,
     ),
     "batch_size": PassConfigParam(
         type_=int,
-        default=1,
+        default_value=1,
         description="""
             Batch size for calibration, required if quant_mode is 'static'.
         """,
     ),
+    # TODO: remove this option once we have a data config ready
     "dataloader_func": PassConfigParam(
         type_=Union[Callable, str],
-        required=True,
+        required=False,
         is_object=True,
         description="""
             Function/function name to generate dataloader for calibration,
             required if quant_mode is 'static'
         """,
     ),
 }
 
 _static_optional_config = {
     "calibrate_method": PassConfigParam(
         type_=str,
-        default="MinMax",
-        default_search=Categorical(["MinMax", "Entropy", "Percentile"]),
+        default_value="MinMax",
+        searchable_values=Categorical(["MinMax", "Entropy", "Percentile"]),
         description="""
             Current calibration methods supported are MinMax and Entropy,
             Please use CalibrationMethod.MinMax or CalibrationMethod.Entropy as options.
         """,
     ),
     "quant_format": PassConfigParam(
         type_=str,
-        default="QDQ",
-        default_search=Categorical(["QOperator", "QDQ"]),
+        default_value="QDQ",
+        searchable_values=Categorical(["QOperator", "QDQ"]),
         description="""
             QOperator format quantizes the model with quantized operators directly.
             QDQ format quantize the model by inserting QuantizeLinear/DeQuantizeLinear on the tensor.
         """,
     ),
     "activation_type": PassConfigParam(
         type_=str,
-        default="QInt8",
-        default_search=Conditional(
-            parents=("quant_format",),
-            support={("QDQ",): Categorical(["QInt8", "QUInt8"]), ("QOperator",): Categorical(["QInt8"])},
+        default_value="QInt8",
+        # the search space is conditional on quant_format and weight_type
+        # the equivalent joint search space for (quant_format, weight_type, activation) is
+        # {(QDQ, QInt8, QInt8), (QDQ, QUInt8, QUInt8), (QOperator, QUInt8, QUInt8)}
+        searchable_values=Conditional(
+            parents=("quant_format", "weight_type"),
+            support={
+                ("QDQ", "QInt8"): Categorical(["QInt8"]),
+                ("QDQ", "QUInt8"): Categorical(["QUInt8"]),
+                ("QOperator", "QUInt8"): Categorical(["QUInt8"]),
+                # invalid choice for QOperator, QInt8
+                ("QOperator", "QInt8"): Conditional.get_invalid_choice(),
+            },
         ),
         description="""
             Quantization data type of activation. Please refer to
             https://onnxruntime.ai/docs/performance/quantization.html for more details on data type selection
         """,
     ),
 }
@@ -167,55 +211,75 @@
 class OnnxQuantization(Pass):
     """
     Quantize ONNX model with onnxruntime where we can search for
     best parameters for static/dynamic quantization at same time.
     """
 
     _requires_user_script = True
+    _requires_data_config = True
 
     def _initialize(self):
         super()._initialize()
-        self.tmp_dir = tempfile.TemporaryDirectory()
+        self.tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp")
 
     @staticmethod
-    def _default_config() -> Dict[str, Any]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         config = {
             "quant_mode": PassConfigParam(
                 type_=str,
-                default="static",
-                default_search=Categorical(["dynamic", "static"]),
+                default_value="static",
+                searchable_values=Categorical(["dynamic", "static"]),
                 description="""
                     Onnx Quantization mode. 'dynamic' for dynamic quantization,
                     'static' for static quantization.
                 """,
             )
         }
 
         # common quantization config
         config.update(deepcopy(_onnx_quantization_config))
 
         # static quantization config
         config.update(deepcopy(_static_dataloader_config))
         static_optional_config = deepcopy(_static_optional_config)
         for _, value in static_optional_config.items():
-            if isinstance(value.default_search, Categorical):
-                value.default_search = Conditional(
+            # default value is conditional on quant_mode
+            # if quant_mode is static, use the default value in static_optional_config
+            # if quant_mode is dynamic, set default value as ignored. dynamic quantization doesn't use this parameter
+            value.default_value = ConditionalDefault(
+                parents=("quant_mode",),
+                support={("static",): value.default_value, ("dynamic",): ConditionalDefault.get_ignored_choice()},
+            )
+            if isinstance(value.searchable_values, Categorical):
+                # ignore the parameter if quant_mode is dynamic
+                # if quant_mode is static, use the searchable_values in static_optional_config by making it conditional
+                value.searchable_values = Conditional(
                     parents=("quant_mode",),
-                    support={("static",): value.default_search},
-                    default=Categorical(["Invalid"]),
+                    support={("static",): value.searchable_values},
+                    default=Conditional.get_ignored_choice(),
                 )
-            elif isinstance(value.default_search, Conditional):
-                value.default_search = Conditional(
-                    parents=("quant_mode",) + value.default_search.parents,
+            elif isinstance(value.searchable_values, Conditional):
+                # ignore the parameter if quant_mode is dynamic
+                # if quant_mode is static, use the searchable_values in static_optional_config by expanding the parents
+                value.searchable_values = Conditional(
+                    parents=("quant_mode",) + value.searchable_values.parents,
                     support={
-                        ("static",) + key: value.default_search.support[key] for key in value.default_search.support
+                        ("static",) + key: value.searchable_values.support[key]
+                        for key in value.searchable_values.support
                     },
-                    default=Categorical(["Invalid"]),
+                    default=Conditional.get_ignored_choice(),
                 )
         config.update(static_optional_config)
+
+        # exposed extra options config
+        config.update(deepcopy(_exposed_extra_options_config))
+        config.update(deepcopy(_extra_options_config))
+
+        # external data config
+        config.update(get_external_data_config())
         return config
 
     def validate_search_point(self, search_point: Dict[str, Any]) -> bool:
         config = self.config_at_search_point(search_point)
         if config["quant_mode"] == "static":
             if (
                 config["weight_type"] == "QInt8"
@@ -223,116 +287,194 @@
                 and config["quant_format"] == "QOperator"
             ):
                 logger.info("QOperator is not supported for QInt8 activation and weight.")
                 return False
             if config["weight_type"] != config["activation_type"]:
                 logger.info("Weight type and activation type must be the same.")
                 return False
+            if config["EnableSubgraph"] is True:
+                logger.info("EnabaleSubgraph is not supported for static quantization.")
+                return False
         return True
 
     def _run_for_config(self, model: ONNXModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
+        from onnxruntime.quantization import QuantFormat, QuantType, quantize_dynamic, quantize_static
+        from onnxruntime.quantization.calibrate import CalibrationMethod
+
         # start with a copy of the config
         run_config = deepcopy(config)
         is_static = run_config["quant_mode"] == "static"
 
-        # add onnx extension if not present
-        if Path(output_model_path).suffix != ".onnx":
-            output_model_path += ".onnx"
+        output_model_path = ONNXModel.resolve_path(output_model_path)
+
+        # extra config
+        extra_options = deepcopy(config["extra_options"]) if config["extra_options"] else {}
+        # keys in extra_options that are already exposed
+        intersection = set(extra_options.keys()).intersection(set(_exposed_extra_options_config.keys()))
+        if intersection:
+            message = (
+                f"Extra config keys {intersection} are already exposed in the pass config. They will be overwritten by"
+                " the corresponding pass config parameter values."
+            )
+            logger.warning(message)
+        for key in _exposed_extra_options_config:
+            extra_options[key] = run_config[key]
+            del run_config[key]
 
         # preprocess the model
-        preprocessed_temp_model_path = Path(self.tmp_dir.name) / f"{Path(model.model_path).stem}_preprocessed.onnx"
+        # we hash the entire path of the input model to ensure we are not accidentally using a preprocessed model
+        # from a different model
+        preprocessed_temp_model_path = (
+            Path(self.tmp_dir.name) / f"{hash_string(str(Path(model.model_path).resolve()))}" / "preprocessed.onnx"
+        )
+        preprocessed_temp_model_path.parent.mkdir(exist_ok=True, parents=True)
         if run_config["quant_preprocess"]:
             if not preprocessed_temp_model_path.exists():
                 # overwrite the model path with the preprocessed model path
                 logger.info("Preprocessing model for quantization")
                 model = self._quant_preprocess(model, preprocessed_temp_model_path)
             else:
                 logger.info("Already processed model for quantization, skipping preprocessing")
-                model = ONNXModel(preprocessed_temp_model_path)
+                model = ONNXModel(
+                    preprocessed_temp_model_path, model.name, model_storage_kind=ModelStorageKind.LocalFolder
+                )
 
         # keys not needed for quantization
-        to_delete = ["quant_mode", "script_dir", "user_script", "quant_preprocess"]
+        to_delete = ["quant_mode", "script_dir", "user_script", "quant_preprocess", "data_config"]
+        to_delete += list(get_external_data_config().keys())
 
         # update string values to enum values
         if is_static:
             to_delete += list(_static_dataloader_config.keys())
             run_config.update(
                 {
                     "calibrate_method": CalibrationMethod[run_config["calibrate_method"]],
                     "quant_format": QuantFormat[run_config["quant_format"]],
                     "activation_type": QuantType[run_config["activation_type"]],
                     "weight_type": QuantType[run_config["weight_type"]],
-                    "extra_options": {},
+                    "extra_options": extra_options,
                 }
             )
         else:
             to_delete += list(_static_dataloader_config.keys())
             to_delete += list(_static_optional_config.keys())
             run_config.update(
                 {
                     "weight_type": QuantType[run_config["weight_type"]],
-                    "extra_options": {},
+                    "extra_options": extra_options,
                 }
             )
         # remove keys not needed for quantization
         for key in to_delete:
             if key in run_config:
                 del run_config[key]
-        # add extra options to the extra options dictionary
-        for key, value in config.items():
-            if key.startswith("eo_"):
-                run_config["extra_options"][key] = value
-                del run_config[key]
+
+        # to be safe, run the quantizer with use_external_data_format set to `True` and
+        # `model_output` to a temporary directory
+        # reload the model and save to output_model_path using the external data config
+        # TODO: don't default to use_external_data_format=True if the loading and saving model makes
+        # the pass inefficient
+        tmp_dir = tempfile.TemporaryDirectory(prefix="olive_tmp")
+        tmp_dir_path = Path(tmp_dir.name)
+        tmp_model_path = str(tmp_dir_path / Path(output_model_path).name)
 
         if is_static:
             # get the dataloader
-            dataloader = self._user_module_loader.call_object(
-                self._fixed_params["dataloader_func"], self._fixed_params["data_dir"], self._fixed_params["batch_size"]
-            )
+            # TODO: only use data config
+            if self._user_module_loader.user_module:
+                dataloader = self._user_module_loader.call_object(
+                    self._fixed_params["dataloader_func"],
+                    self._fixed_params["data_dir"],
+                    self._fixed_params["batch_size"],
+                )
+            elif self._data_config:
+                dataloader = self._data_config.to_data_container().create_calibration_dataloader()
             quantize_static(
                 model_input=model.model_path,
-                model_output=output_model_path,
+                model_output=tmp_model_path,
                 calibration_data_reader=dataloader,
+                use_external_data_format=True,
                 **run_config,
             )
         else:
-            quantize_dynamic(model_input=model.model_path, model_output=output_model_path, **run_config)
+            quantize_dynamic(
+                model_input=model.model_path, model_output=tmp_model_path, use_external_data_format=True, **run_config
+            )
+
+        # load the model
+        onnx_model = onnx.load(tmp_model_path)
+        # the model is loaded into memory, so it's safe to delete previously exported files
+        tmp_dir.cleanup()
 
-        return ONNXModel(output_model_path, model.name)
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(onnx_model, output_model_path, config, model.name)
 
     def _quant_preprocess(self, model: ONNXModel, output_model_path: str) -> ONNXModel:
+        from onnxruntime.quantization.preprocess import quant_pre_process
+
         try:
             quant_pre_process(input_model_path=model.model_path, output_model_path=output_model_path, auto_merge=True)
+            has_external_data = False
         except Exception as e:
-            logger.warning(f"failed to run quantization preprocessing with error of {e}")
-            copyfile(model.model_path, output_model_path)
+            # TODO: try with `skip_optimization = True`
+            # quantization preprocessing will fail if the model is too large and `skip_optimization = False`
+            # there are some problems with the path to where the external data is saved
+            # need to find out why before enabling this
+
+            logger.warning(f"Failed to run quantization preprocessing with error of {e}. Using original model.")
+            # save original model to output path
+            onnx_model = onnx.load(model.model_path)
+            model_proto_to_file(
+                onnx_model,
+                output_model_path,
+                save_as_external_data=True,  # always save as external data to avoid failures due to large models
+            )
+            has_external_data = True
 
-        return ONNXModel(output_model_path)
+        return ONNXModel(
+            output_model_path,
+            model.name,
+            model_storage_kind=ModelStorageKind.LocalFolder if has_external_data else ModelStorageKind.LocalFile,
+        )
 
 
 class OnnxDynamicQuantization(OnnxQuantization):
     """ONNX Dynamic Quantization Pass"""
 
     _requires_user_script = False
 
     @staticmethod
-    def _default_config() -> Dict[str, Any]:
-        config = {"quant_mode": PassConfigParam(type_=str, default="dynamic", description="dynamic quantization mode")}
+    def _default_config() -> Dict[str, PassConfigParam]:
+        config = {
+            "quant_mode": PassConfigParam(type_=str, default_value="dynamic", description="dynamic quantization mode")
+        }
         # common quantization config
         config.update(deepcopy(_onnx_quantization_config))
+        # exposed extra options config
+        config.update(deepcopy(_exposed_extra_options_config))
+        config.update(deepcopy(_extra_options_config))
+        # external data config
+        config.update(get_external_data_config())
         return config
 
 
 class OnnxStaticQuantization(OnnxQuantization):
     """ONNX Static Quantization Pass"""
 
     _requires_user_script = True
 
     @staticmethod
-    def _default_config() -> Dict[str, Any]:
-        config = {"quant_mode": PassConfigParam(type_=str, default="static", description="static quantization mode")}
+    def _default_config() -> Dict[str, PassConfigParam]:
+        config = {
+            "quant_mode": PassConfigParam(type_=str, default_value="static", description="static quantization mode")
+        }
         # common quantization config
         config.update(deepcopy(_onnx_quantization_config))
         # static quantization specific config
         config.update(deepcopy(_static_dataloader_config))
         config.update(deepcopy(_static_optional_config))
+        # exposed extra options config
+        config.update(deepcopy(_exposed_extra_options_config))
+        config.update(deepcopy(_extra_options_config))
+        # external data config
+        config.update(get_external_data_config())
         return config
```

## olive/passes/onnx/transformer_optimization.py

```diff
@@ -1,80 +1,239 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from copy import deepcopy
-from pathlib import Path
-from typing import Any, Dict
+from typing import Any, Dict, List, Union
+
+from packaging import version
 
 from olive.model import ONNXModel
 from olive.passes import Pass
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 
 
 class OrtTransformersOptimization(Pass):
     """Optimize transformer based models in scenarios where ONNX Runtime does not apply the optimization at load time.
     It is based on onnxruntime.transformers.optimizer."""
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         # TODO: add default search if supported
-        return {
+        from onnxruntime.transformers.fusion_options import FusionOptions
+
+        config = {
             "model_type": PassConfigParam(
                 type_=str,
                 required=True,
                 description=(
-                    "Transformer based model type, includig bert (exported by PyTorch), gpt2 (exported by PyTorch), "
-                    "bert_tf (BERT exported by tf2onnx), bert_keras (BERT exported by keras2onnx)."
+                    "Transformer based model type, including bert (exported by PyTorch), gpt2 (exported by PyTorch), "
+                    "bert_tf (BERT exported by tf2onnx), bert_keras (BERT exported by keras2onnx), and "
+                    "unet/vae/clip (stable diffusion)."
                 ),
             ),
-            "num_heads": PassConfigParam(type_=int, default=0, description="Number of attention heads."),
-            "hidden_size": PassConfigParam(type_=int, default=0, description="Number of hidden nodes."),
+            "num_heads": PassConfigParam(type_=int, default_value=0, description="Number of attention heads."),
+            "hidden_size": PassConfigParam(type_=int, default_value=0, description="Number of hidden nodes."),
             # TODO: Figure out what the expected type is
             "optimization_options": PassConfigParam(
-                type_=Any, default=None, description="Optimization options that turn on/off some fusions."
+                type_=Union[Dict[str, Any], FusionOptions],
+                default_value=None,
+                description="Optimization options that turn on/off some fusions.",
             ),
             "opt_level": PassConfigParam(
                 type_=Any,
-                default=None,
+                default_value=None,
                 description=(
                     "Graph optimization level of Onnx Runtime: "
                     "0 - disable all (default), 1 - basic, 2 - extended, 99 - all."
                 ),
             ),
-            "use_gpu": PassConfigParam(type_=bool, default=False, description="Flag for GPU inference."),
+            "use_gpu": PassConfigParam(type_=bool, default_value=False, description="Flag for GPU inference."),
             "only_onnxruntime": PassConfigParam(
                 type_=bool,
-                default=False,
+                default_value=False,
                 description="Whether only use onnxruntime to optimize model, and no python fusion.",
             ),
             "float16": PassConfigParam(
-                type_=bool, default=False, description="Whether half-precision float will be used."
+                type_=bool, default_value=False, description="Whether half-precision float will be used."
             ),
             "input_int32": PassConfigParam(
-                type_=bool, default=False, description="Whether int32 tensors will be used as input."
+                type_=bool, default_value=False, description="Whether int32 tensors will be used as input."
+            ),
+            "keep_io_types": PassConfigParam(
+                type_=bool,
+                default_value=True,
+                description="Keep input and output tensors in their original data type",
             ),
-            "use_external_data_format": PassConfigParam(
-                type_=bool, default=False, description="Whether use external data format to store large model (>2GB)"
+            "force_fp32_ops": PassConfigParam(
+                type_=List[str], default_value=None, description="Operators that are forced to run in float32"
+            ),
+            "target_provider": PassConfigParam(
+                type_=str,
+                default_value=None,
+                description=(
+                    "Target execution provider. This parameter will be removed when "
+                    "accelerators/targets are visible to passes."
+                ),
             ),
         }
+        config.update(get_external_data_config())
+        return config
+
+    @staticmethod
+    def _set_fusion_options(run_config: Dict[str, Any]):
+        from onnxruntime.transformers.fusion_options import FusionOptions
+
+        fusion_options = FusionOptions(run_config["model_type"])
+        fusion_options.__dict__.update(run_config["optimization_options"])
+        run_config["optimization_options"] = fusion_options
+
+    @staticmethod
+    def sd_model_types():
+        """Returns model types in the stable diffusion pipeline recognized by the ORT transformer optimizer"""
+        return ("unet", "vae", "clip")
+
+    @staticmethod
+    def _set_sd_fusion_options(run_config: Dict[str, Any], pass_config: Dict[str, Any]):
+        """Configures fusion options for stable diffusion models"""
+        import onnxruntime as ort
+
+        ort_version = version.parse(ort.__version__)
+        is_ort_1_13_or_older = ort_version < version.parse("1.14.0")
+        # is_ort_1_14 = ort_version >= version.parse("1.14.0") and ort_version < version.parse("1.15.0")
+
+        # default to no specific fusion options in earlier releases of ORT
+        if is_ort_1_13_or_older:
+            return
+
+        is_ort_1_15_0_or_newer = ort_version >= version.parse("1.15.0")
+        is_ort_1_15_1_or_newer = ort_version >= version.parse("1.15.1")
+
+        input_model_type = run_config["model_type"]
+        if not is_ort_1_15_0_or_newer and input_model_type != "unet":
+            # 'vae' and 'clip' are only recognized in ORT v1.15+. earlier versions of ORT stable diffusion
+            # optimization simply use "unet" for these model types.
+            run_config["model_type"] = "unet"
+
+        from onnxruntime.transformers.fusion_options import FusionOptions
+
+        fusion_options = FusionOptions(run_config["model_type"])
+
+        # TODO: remove dml_future when ORT 1.15.1 with future version of DML is released
+        # This "provider" value is simply a way to test in-development changes without having
+        # to bump the ORT version.
+        dml_future = pass_config["target_provider"] == "directml_future"
+
+        if pass_config["target_provider"] == "directml" or dml_future:
+            # Some of these fusions are disabled because they provide no performance advantage,
+            # and it's preferable to limit ops outside the ONNX domain.
+            fusion_options.enable_gelu = is_ort_1_15_0_or_newer
+            fusion_options.enable_layer_norm = is_ort_1_15_0_or_newer
+            fusion_options.enable_attention = is_ort_1_15_1_or_newer or dml_future
+            fusion_options.use_multi_head_attention = is_ort_1_15_1_or_newer or dml_future
+            fusion_options.enable_skip_layer_norm = False
+            fusion_options.enable_embed_layer_norm = is_ort_1_15_0_or_newer
+            fusion_options.enable_bias_skip_layer_norm = False
+            fusion_options.enable_bias_gelu = is_ort_1_15_0_or_newer
+            fusion_options.enable_gelu_approximation = False
+            fusion_options.enable_qordered_matmul = False
+            fusion_options.enable_shape_inference = is_ort_1_15_0_or_newer
+            fusion_options.enable_gemm_fast_gelu = False
+            fusion_options.enable_nhwc_conv = False
+            fusion_options.enable_group_norm = is_ort_1_15_1_or_newer or dml_future
+            fusion_options.enable_bias_splitgelu = False
+            fusion_options.enable_packed_qkv = pass_config["float16"] and is_ort_1_15_0_or_newer
+            fusion_options.enable_packed_kv = pass_config["float16"] and is_ort_1_15_0_or_newer
+            fusion_options.enable_bias_add = False
+        else:
+            if input_model_type == "unet":
+                fusion_options.enable_packed_kv = pass_config["float16"]
+                fusion_options.enable_packed_qkv = pass_config["float16"] and is_ort_1_15_0_or_newer
+                fusion_options.enable_bias_add = is_ort_1_15_0_or_newer
+
+        run_config["optimization_options"] = fusion_options
+
+    @staticmethod
+    def _get_op_block_list(config: Dict[str, Any]):
+        import onnxruntime as ort
+
+        op_block_list = []
+
+        if config["float16"]:
+            if config["model_type"] in OrtTransformersOptimization.sd_model_types():
+                if version.parse(ort.__version__) < version.parse("1.15.0"):
+                    op_block_list += ["RandomNormalLike", "Resize", "GroupNorm"]
+                else:
+                    op_block_list += ["RandomNormalLike"]
+            if config["force_fp32_ops"]:
+                op_block_list += config["force_fp32_ops"]
+
+        return op_block_list if len(op_block_list) > 0 else None
+
+    @staticmethod
+    def _run_without_optimization(model: ONNXModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
+        """Fallback/pass-through path that skips onnxruntime.transformers.optimizer and simply copies the model
+        or converts it to FP16 without performing transformer-specific optimizations. This fallback exists so
+        that a pass configuration can be used with multiple ORT versions, some of which may not support optimization.
+        """
+
+        if not config["float16"]:
+            return model
+
+        import onnx
+        from onnxconverter_common import float16
+
+        # stable diffusion unet is too large for the converter to handle with shape inference
+        disable_shape_infer = config["model_type"] == "unet"
+
+        op_block_list = OrtTransformersOptimization._get_op_block_list(config)
+
+        model_fp32 = onnx.load(str(model.model_path))
+        model_fp16 = float16.convert_float_to_float16(
+            model_fp32,
+            keep_io_types=config["keep_io_types"],
+            op_block_list=op_block_list,
+            disable_shape_infer=disable_shape_infer,
+        )
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(model_fp16, output_model_path, config, model.name)
 
     def _run_for_config(self, model: ONNXModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
+        import onnxruntime as ort
         from onnxruntime.transformers import optimizer as transformers_optimizer
 
         # start with a copy of the config
         run_config = deepcopy(config)
-        del run_config["float16"], run_config["input_int32"], run_config["use_external_data_format"]
+        del (
+            run_config["float16"],
+            run_config["input_int32"],
+            run_config["keep_io_types"],
+            run_config["force_fp32_ops"],
+            run_config["target_provider"],
+        )
+        for key in get_external_data_config():
+            del run_config[key]
+
+        output_model_path = ONNXModel.resolve_path(output_model_path)
+
+        if config["model_type"] in OrtTransformersOptimization.sd_model_types():
+            # stable diffusion optimization only applies to the CUDA EP in ORT 1.14 and earlier.
+            if config["target_provider"] != "cuda" and version.parse(ort.__version__) < version.parse("1.15.0"):
+                return self._run_without_optimization(model, config, output_model_path)
+
+            if config["optimization_options"] is None:
+                self._set_sd_fusion_options(run_config, config)
+        elif config["optimization_options"]:
+            self._set_fusion_options(run_config)
 
         optimizer = transformers_optimizer.optimize_model(input=model.model_path, **run_config)
+
         if config["float16"]:
-            optimizer.convert_float_to_float16(keep_io_types=True)
+            op_block_list = self._get_op_block_list(config)
+            optimizer.convert_float_to_float16(keep_io_types=config["keep_io_types"], op_block_list=op_block_list)
+
         if config["input_int32"]:
             optimizer.change_graph_inputs_to_int32()
 
-        # add onnx extension if not present
-        if Path(output_model_path).suffix != ".onnx":
-            output_model_path += ".onnx"
-
-        optimizer.save_model_to_file(output_model_path, config["use_external_data_format"])
-
-        return ONNXModel(output_model_path, model.name)
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(optimizer.model, output_model_path, config, model.name)
```

## olive/passes/openvino/conversion.py

```diff
@@ -2,26 +2,26 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from pathlib import Path
 from typing import Any, Dict, List, Tuple, Union
 
 from olive.constants import Framework
-from olive.model import ONNXModel, OpenVINOModel, PyTorchModel
+from olive.model import ModelStorageKind, ONNXModel, OpenVINOModel, PyTorchModel
 from olive.passes import Pass
 from olive.passes.pass_config import PassConfigParam
 
 
 class OpenVINOConversion(Pass):
     """
     Converts PyTorch, ONNX or TensorFlow Model to OpenVino Model.
     """
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         return {
             "input": PassConfigParam(
                 type_=List[Tuple],
                 required=False,
                 description=(
                     "Input can be set by passing a list of tuples. "
                     "Each tuple should contain input name and optionally input type or input shape."
@@ -34,15 +34,15 @@
                     "Input shape(s) that should be fed to an input node(s) of the model."
                     " Shape is defined as a comma-separated list of integer numbers"
                     " enclosed in parentheses or square brackets, for example [1,3,227,227]."
                 ),
             ),
             "extra_config": PassConfigParam(
                 type_=Dict,
-                default=None,
+                default_value=None,
                 required=False,
                 description=(
                     "Extra configurations for OpenVINO model conversion. extra_config can be set by"
                     " passing a dictionary where key is the parameter name, and the value is the parameter value."
                     " Please check 'mo' command usage instruction for available parameters:"
                     " https://docs.openvino.ai/latest/openvino_docs_MO_DG_Deep_Learning_Model_Optimizer_DevGuide.html"
                 ),
@@ -54,27 +54,32 @@
     ) -> OpenVINOModel:
         import torch
 
         try:
             from openvino.runtime import serialize
             from openvino.tools.mo import convert_model
         except ImportError:
-            raise ImportError("Please install olive[openvino] to use OpenVINO model")
+            raise ImportError("Please install olive-ai[openvino] to use OpenVINO model")
 
         model_name = model.name if model.name else "ov_model"
 
         model_input_param = "input_model"
         input_model = model.model_path
-        if model.framework == Framework.TENSORFLOW and not model.is_file:
+        if model.framework == Framework.TENSORFLOW and model.model_storage_kind == ModelStorageKind.LocalFolder:
             model_input_param = "saved_model_dir"
         if model.framework == Framework.PYTORCH:
             input_model = model.load_model()
 
-        extra_config = config["extra_config"] or {}
-        if not extra_config.get("example_input") and config.get("input_shape"):
+        if config.get("extra_config") is None:
+            config["extra_config"] = {}
+
+        extra_config = config["extra_config"]
+        example_input = extra_config.get("example_input")
+        input_shape = config.get("input_shape")
+        if example_input is None and input_shape:
             extra_config["example_input"] = torch.randn(config["input_shape"])
         args = {model_input_param: input_model, "model_name": model_name, **extra_config}
 
         # OpenVINO Python API document: https://docs.openvino.ai/latest/openvino_docs_MO_DG_Python_API.html
         ov_model = convert_model(**args)
         output_dir = Path(output_model_path) / model_name
```

## olive/passes/openvino/quantization.py

```diff
@@ -16,39 +16,39 @@
     Post-training quantization for OpenVINO model.
     Please refer to https://docs.openvino.ai/latest/pot_introduction.html for more details.
     """
 
     _requires_user_script = True
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         return {
             "engine_config": PassConfigParam(
                 type_=Dict,
                 required=True,
                 description=(
                     "Specific config for openvino.tools.pot.IEEngine. 'engine_config' can be set"
-                    " by passing a dictonary, for example engine_config = {'device': 'CPU'}"
+                    " by passing a dictonary, for example engine_config: {'device': 'CPU'}"
                 ),
             ),
             "dataloader_func": PassConfigParam(
                 type_=Union[Callable, str],
                 required=False,
                 is_object=True,
                 description=(
                     "A callable function or a str of the function name from 'user_script'"
                     " for the instance of the dataloader."
                 ),
             ),
             "data_dir": PassConfigParam(
                 type_=Union[Path, str],
                 is_path=True,
-                description=("Dataset path. 'data_dir' can be by a str or Pathlib.Path."),
+                description="Dataset path. 'data_dir' can be by a str or Pathlib.Path.",
             ),
-            "batch_size": PassConfigParam(type_=int, default=1, description=("Batch size for the dataloader.")),
+            "batch_size": PassConfigParam(type_=int, default_value=1, description="Batch size for the dataloader."),
             "metric_func": PassConfigParam(
                 type_=Union[Callable, str],
                 required=False,
                 is_object=True,
                 description=(
                     "A callable function or a str of the function name from 'user_script'"
                     " for Metric instance to calculate the accuracy metric of the model."
@@ -56,26 +56,26 @@
             ),
             "algorithms": PassConfigParam(
                 type_=List[Dict],
                 required=True,
                 description=(
                     "A list defining optimization algorithms and their parameters included"
                     " in the optimization pipeline. The order in which they are applied to the model"
-                    " in the optimization pipeline is determined by the order in the list. example: algorithms = "
+                    " in the optimization pipeline is determined by the order in the list. example: algorithms: "
                     " [{'name': 'DefaultQuantization', 'params': {'preset': 'performance', 'stat_subset_size': 500},}]"
                 ),
             ),
         }
 
     def _run_for_config(self, model: OpenVINOModel, config: Dict[str, Any], output_model_path: str) -> OpenVINOModel:
 
         try:
             from openvino.tools.pot import IEEngine, compress_model_weights, create_pipeline, save_model
         except ImportError:
-            raise ImportError("Please install olive[openvino] to use OpenVINO model")
+            raise ImportError("Please install olive-ai[openvino] to use OpenVINO model")
 
         model_name = model.name if model.name else "ov_model"
 
         loader = UserModuleLoader(user_script=config["user_script"], script_dir=config["script_dir"])
         data_loader = loader.call_object(config["dataloader_func"], config["data_dir"], config["batch_size"])
         metric = loader.load_object(config["metric_func"])
         engine = IEEngine(config=config["engine_config"], data_loader=data_loader, metric=metric)
```

## olive/passes/pytorch/qat_utils.py

```diff
@@ -1,19 +1,22 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import copy
 
+import pytorch_lightning
 import torch
 import torch.quantization.quantization_mappings as tqqm
+from packaging import version
 from pytorch_lightning import LightningModule, seed_everything
 from torch.ao.quantization.fake_quantize import FakeQuantize, MovingAverageMinMaxObserver
 
-from olive.model import PyTorchModel
+from olive.constants import ModelFileFormat
+from olive.model import ModelStorageKind, PyTorchModel
 from olive.passes.pytorch.cluster import barrier, create_cluster, is_master_proc
 from olive.passes.pytorch.pytorch_lightning_utils import create_ddp_strategy, create_trainer
 
 
 class QuantizedModule(torch.nn.Module):
     def __init__(self, model: torch.nn.Module):
         super().__init__()
@@ -35,15 +38,15 @@
         self.output_model_path = output_model_path
 
     def execute_local(self) -> PyTorchModel:
         seed_everything(self.config.seed)
         cluster_environment = create_cluster()
         run_on_gpus = cluster_environment is not None or torch.cuda.is_available()
         input_model = self.model.load_model()
-        model_input_tensor = self.create_dummy_input()
+        model_input_tensor = self.model.get_dummy_inputs()
 
         if self.config.qconfig_func:
             qconfig = self.config.qconfig_func()
         else:
             default_fake_quant = FakeQuantize.with_args(
                 observer=MovingAverageMinMaxObserver,
                 quant_min=0,
@@ -75,15 +78,18 @@
 
             kwargs = {}
             if run_on_gpus:
                 num_gpus = self.config.gpus if self.config.gpus is not None else torch.cuda.device_count()
                 ddp = create_ddp_strategy(cluster=cluster_environment, accelerator="gpu")
                 kwargs["strategy"] = ddp
                 kwargs["devices"] = num_gpus
-                kwargs["replace_sampler_ddp"] = False
+                if version.parse(pytorch_lightning.__version__) >= version.parse("1.9.0"):
+                    kwargs["use_distributed_sampler"] = False
+                else:
+                    kwargs["replace_sampler_ddp"] = False
 
             trainer = create_trainer(
                 max_epochs=self.config.num_epochs, max_steps=self.config.num_steps, logger=self.config.logger, **kwargs
             )
 
             trainer.fit(ptl_module, datamodule=ptl_data_module)
 
@@ -106,16 +112,29 @@
     def post_qat(self, model: torch.nn.Module, model_input_tensor) -> torch.nn.Module:
         model.apply(torch.quantization.disable_observer)
         model_converted = torch.ao.quantization.convert(model.eval(), inplace=False)
         traced_model_converted = torch.jit.trace(model_converted, model_input_tensor, strict=False)
         if is_master_proc():
             torch.jit.save(traced_model_converted, self.output_model_path)
         barrier()
+        # preserve the io_config, dummy_inputs_func, model_script, script_dir
+        # from the original model
+        original_config = self.model.to_json()["config"]
+        to_keep = ["io_config", "dummy_inputs_func"]
+        if isinstance(original_config["dummy_inputs_func"], str):
+            to_keep += ["model_script", "script_dir"]
+        config_to_keep = {k: original_config[k] for k in to_keep}
         # TODO: Add PyTorch model type flag
-        qat_pytorch_model = PyTorchModel(model_path=self.output_model_path, name="pytorch_qat_model", is_file=True)
+        qat_pytorch_model = PyTorchModel(
+            model_path=self.output_model_path,
+            name="pytorch_qat_model",
+            model_file_format=ModelFileFormat.PYTORCH_TORCH_SCRIPT,
+            model_storage_kind=ModelStorageKind.LocalFile,
+            **config_to_keep
+        )
         return qat_pytorch_model
 
     def fuse_modules(self, model: torch.nn.Module):
         if self.config.modules_to_fuse:
             for group in self.config.modules_to_fuse:
                 if self._check_feasible_fuse(model, group):
                     torch.quantization.fuse_modules(model, [group], inplace=True)
@@ -152,30 +171,14 @@
         return state and hasattr(obj, attribs)
 
     def _check_feasible_fuse(self, model, group):
         if not all(self._recursive_hasattr(model, m) for m in group):
             return False
         return True
 
-    def create_dummy_input(self):
-        str_to_type = {"float32": torch.float32, "float16": torch.float16, "int32": torch.int32, "int64": torch.int64}
-        input_types = []
-        if self.config.input_types is not None:
-            for input_type in self.config.input_types:
-                input_types.append(str_to_type[input_type])
-        else:
-            input_types = [str_to_type["float32"] for _ in self.config.input_shapes]
-
-        # dummy inputs
-        dummy_inputs = []
-        for input_shape, input_type in zip(self.config.input_shapes, input_types):
-            dummy_inputs.append(torch.zeros(input_shape, dtype=input_type))
-        dummy_inputs = tuple(dummy_inputs) if len(dummy_inputs) > 1 else dummy_inputs[0]
-        return dummy_inputs
-
 
 class DefaultPTLModule(LightningModule):
     def __init__(self, model, training_dataloader):
         super().__init__()
         self.save_hyperparameters()
         self.model = model
         self.training_dataloader = training_dataloader
```

## olive/passes/pytorch/quantization_aware_training.py

```diff
@@ -12,15 +12,15 @@
 
 class QuantizationAwareTraining(Pass):
     """Run quantization aware training on PyTorch model."""
 
     _requires_user_script = True
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         import pytorch_lightning
         from packaging import version
 
         if version.parse(pytorch_lightning.__version__) >= version.parse("1.9.0"):
             from pytorch_lightning.loggers import Logger
         else:
             from pytorch_lightning.loggers import LightningLoggerBase as Logger
@@ -53,51 +53,43 @@
                     "LightningDataModule for PyTorch Lightning trainer. It is a way of encapsulating all the "
                     "data-related logic for training, validation, and testing of a PyTorch model. Please refer to "
                     "https://pytorch-lightning.readthedocs.io/en/stable/data/datamodule.html for more details."
                 ),
             ),
             "train_batch_size": PassConfigParam(type_=int, description="Batch size for training."),
             "num_epochs": PassConfigParam(type_=int, description="Maximum number of epochs for training."),
-            "num_steps": PassConfigParam(type_=int, default=-1, description="Maximum number of steps for training."),
+            "num_steps": PassConfigParam(
+                type_=int, default_value=-1, description="Maximum number of steps for training."
+            ),
             "do_validate": PassConfigParam(
                 type_=bool,
-                default=False,
+                default_value=False,
                 description="Whether perform one evaluation epoch over the validation set after training.",
             ),
             "modules_to_fuse": PassConfigParam(
-                type_=List[List[str]], default=None, description="List of list of module names to fuse."
-            ),
-            "input_shapes": PassConfigParam(
-                type_=List[List[int]],
-                required=True,
-                description="List ot input shapes. It is used to create dummy input for PyTorch model tracing.",
-            ),
-            "input_types": PassConfigParam(
-                type_=List[str],
-                default=None,
-                description="List ot input types. It is used to create dummy input for PyTorch model tracing.",
+                type_=List[List[str]], default_value=None, description="List of list of module names to fuse."
             ),
             "qconfig_func": PassConfigParam(
                 type_=Union[Callable, str],
-                default=None,
+                default_value=None,
                 is_object=True,
                 description=(
                     "Customized function to create a QConfig for QAT. Please refer to "
                     "https://pytorch.org/docs/stable/generated/torch.quantization.qconfig.QConfig.html for details."
                 ),
             ),
             "logger": PassConfigParam(
                 type_=Union[Logger, Iterable[Logger], Callable, bool],
                 required=False,
-                default=False,
+                default_value=False,
                 is_object=True,
                 description="Logger for training.",
             ),
             "gpus": PassConfigParam(type_=int, description="Number of GPUs to use."),
-            "seed": PassConfigParam(type_=int, default=None, description="Random seed for training."),
+            "seed": PassConfigParam(type_=int, default_value=None, description="Random seed for training."),
         }
 
     def _run_for_config(self, model: PyTorchModel, config: Dict[str, Any], output_model_path: str) -> PyTorchModel:
         from olive.passes.pytorch.qat_utils import QatTrainer
 
         qat_trainer_config = self._config_class(**config)
         if Path(output_model_path).suffix != ".pt":
```

## olive/passes/snpe/conversion.py

```diff
@@ -40,15 +40,15 @@
 class SNPEConversion(Pass):
     """
     Convert ONNX or TensorFlow model to SNPE DLC.
     Uses snpe-tensorflow-to-dlc or snpe-onnx-to-dlc tools from the SNPE SDK.
     """
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
+    def _default_config() -> Dict[str, PassConfigParam]:
         return {
             "input_names": PassConfigParam(type_=List[str], required=True, description="List of input names."),
             "input_shapes": PassConfigParam(
                 type_=List[List[int]],
                 required=True,
                 description="List of input shapes. Must be the same length as input_names.",
             ),
@@ -56,33 +56,33 @@
             "output_shapes": PassConfigParam(
                 type_=List[List[int]],
                 required=True,
                 description="List of output shapes. Must be the same length as output_names.",
             ),
             "input_types": PassConfigParam(
                 type_=List[Union[str, None]],
-                default=None,
+                default_value=None,
                 description=(
                     "List of input types. If not None, it must be a list of the same length as input_names. List"
                     " members can be None to use default value. Refer to olive.snpe.constants.InputType for valid"
                     " values."
                 ),
             ),
             "input_layouts": PassConfigParam(
                 type_=List[Union[str, None]],
-                default=None,
+                default_value=None,
                 description=(
                     "List of input layouts. If not None, it must be a list of the same length as input_names. List"
                     " members can be None to use infered value. Refer to olive.snpe.constants.InputLayout for valid"
                     " values."
                 ),
             ),
             "extra_args": PassConfigParam(
                 type_=str,
-                default=None,
+                default_value=None,
                 description=(
                     "Extra arguments to pass to snpe conversion tool. Refer to snpe-onnx-to-dlc and"
                     " snpe-tensorflow-to-dlc at https://developer.qualcomm.com/sites/default/files/docs/snpe/tools.html"
                     " for more additional arguments. Must be a dictionary of the form: {'arg_name': 'arg_value'}."
                 ),
             ),
         }
```

## olive/passes/snpe/quantization.py

```diff
@@ -34,34 +34,34 @@
                 description=(
                     "Function or function name to create dataloader for quantization. Function should take data"
                     " directory as an argument and return a olive.snpe.SNPEDataLoader object."
                 ),
             ),
             "use_enhanced_quantizer": PassConfigParam(
                 type_=bool,
-                default=False,
-                default_search=Boolean(),
+                default_value=False,
+                searchable_values=Boolean(),
                 description=(
                     "Use the enhanced quantizer feature when quantizing the model. Uses an algorithm to determine"
                     " optimal range instead of min and max range of data.  It can be useful for quantizing models that"
                     " have long tails in the distribution of the data being quantized."
                 ),
             ),
             "enable_htp": PassConfigParam(
                 type_=bool,
-                default=False,
-                default_search=Boolean(),
+                default_value=False,
+                searchable_values=Boolean(),
                 description="Pack HTP information in quantized DLC.",
             ),
             "htp_socs": PassConfigParam(
-                type_=List[str], default=None, description="List of SoCs to generate HTP Offline cache for."
+                type_=List[str], default_value=None, description="List of SoCs to generate HTP Offline cache for."
             ),
             "extra_args": PassConfigParam(
                 type_=str,
-                default=None,
+                default_value=None,
                 description=(
                     "Extra arguments to pass to snpe conversion tool. Refer to"
                     " https://developer.qualcomm.com/sites/default/files/docs/snpe/tools.html#tools_snpe-dlc-quantize"
                     " for more additional arguments. Must be a dictionary of the form: {'arg_name': 'arg_value'}."
                 ),
             ),
         }
```

## olive/passes/snpe/snpe_to_onnx.py

```diff
@@ -1,18 +1,18 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from pathlib import Path
 from typing import Any, Callable, Dict
 
 from pydantic import validator
 
 from olive.model import ONNXModel, SNPEModel
 from olive.passes.olive_pass import Pass
+from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 from olive.snpe import SNPEDevice
 from olive.snpe.tools.dev import dlc_to_onnx
 
 
 def _validate_target_device(v):
     valid_devices = [d.value for d in SNPEDevice]
@@ -24,31 +24,35 @@
 class SNPEtoONNXConversion(Pass):
     """
     Convert a SNPE DLC to ONNX to use with SNPE Execution Provider.
     Creates a ONNX graph with the SNPE DLC as a node.
     """
 
     @staticmethod
-    def _default_config() -> Dict[str, Dict[str, Any]]:
-        return {
+    def _default_config() -> Dict[str, PassConfigParam]:
+        config = {
             "target_device": PassConfigParam(
                 type_=str,
-                default="cpu",
+                default_value="cpu",
                 description="Target device for the ONNX model. Refer to olive.snpe.SNPEDevice for valid values.",
             ),
-            "target_opset": PassConfigParam(type_=int, default=12, description="Target ONNX opset version."),
+            "target_opset": PassConfigParam(type_=int, default_value=12, description="Target ONNX opset version."),
         }
+        config.update(get_external_data_config())
+        return config
 
     @staticmethod
     def _validators() -> Dict[str, Callable]:
         return {
             "validate_target_device": validator("target_device", allow_reuse=True)(_validate_target_device),
         }
 
     def _run_for_config(self, model: SNPEModel, config: Dict[str, Any], output_model_path: str) -> ONNXModel:
         config = self._config_class(**config)
 
-        if Path(output_model_path).suffix != ".onnx":
-            output_model_path += ".onnx"
+        output_model_path = ONNXModel.resolve_path(output_model_path)
+
+        # create a onnx model that wraps the dlc binary in a node
+        onnx_model = dlc_to_onnx(model.model_path, config.dict(), **model.io_config)
 
-        dlc_to_onnx(model.model_path, config.dict(), output_model_path, **model.io_config)
-        return ONNXModel(output_model_path, name=model.name)
+        # save the model to the output path and return the model
+        return model_proto_to_olive_model(onnx_model, output_model_path, config.dict(), model.name)
```

## olive/snpe/tools/dev.py

```diff
@@ -212,23 +212,30 @@
     _, stderr = run_snpe_command(cmd, dev=True)
 
     # check if quantization succeeded
     if not ("Writing quantized model" in stderr or "Saved quantized dlc" in stderr):
         raise Exception(stderr)
 
 
-def dlc_to_onnx(dlc_path, config, output_file, input_names, input_shapes, output_names, output_shapes):
+def dlc_to_onnx(
+    dlc_path: str,
+    config: dict,
+    input_names: List[str],
+    input_shapes: List[List[int]],
+    output_names: List[str],
+    output_shapes: List[List[int]],
+) -> onnx.ModelProto:
     """
     Convert a SNPE DLC to ONNX. The DLC is wrapped in a ONNX model for use with onnxruntime SNPE EP.
+    Returns an ONNX ModelProto.
 
     dlc_path: path to the DLC file.
     config: Config dict with the following keys:
         target_device: str = target device for the ONNX-wrapped SNPE model.
         target_opset: int = target ONNX opset for the ONNX-wrapped SNPE model.
-    output_file: path to the output ONNX file.
     input_names: List[str] = list of input names.
     input_shapes: List[List[int]] = list of input shapes.
     output_names: List[str] = list of output names.
     output_shapes: List[List[int]] = list of output shapes.
     """
     # get the SNPE version used to create the DLC
     snpe_version = get_dlc_snpe_version(dlc_path)
@@ -269,9 +276,8 @@
     # Create the graph
     graph_def = helper.make_graph([snpe_node], model_name, inputs_tensor_val, outputs_tensor_val)
 
     op = onnx.OperatorSetIdProto()
     op.version = config["target_opset"]
     model_def = helper.make_model(graph_def, producer_name="Olive", opset_imports=[op])
 
-    # Save the model
-    onnx.save(model_def, output_file)
+    return model_def
```

## olive/strategy/search_parameter.py

```diff
@@ -1,12 +1,13 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from abc import ABC, abstractmethod
+from enum import Enum
 from typing import Any, Dict, List, Tuple, Union
 
 from olive.common.utils import flatten_dict, unflatten_dict
 
 
 class SearchParameter(ABC):
     """
@@ -29,17 +30,33 @@
         raise NotImplementedError()
 
     @abstractmethod
     def to_json(self):
         raise NotImplementedError()
 
 
+class SpecialParamValue(str, Enum):
+    """
+    Special values for parameters.
+
+    IGNORED: the parameter gets the value "OLIVE_IGNORED_PARAM_VALUE". The pass might ignore this parameter.
+    INVALID: Any seach point with this value is invalid. The search algorithm will not suggest such a search point.
+    """
+
+    IGNORED = "OLIVE_IGNORED_PARAM_VALUE"
+    INVALID = "OLIVE_INVALID_PARAM_VALUE"
+
+
 class Categorical(SearchParameter):
     """
     Search parameter that supports a list of values
+
+    Examples
+    --------
+    >>> Categorical([1, 2, 3])
     """
 
     def __init__(self, support: Union[List[str], List[int], List[float], List[bool]]):
         self.support = support
 
     def get_support(self) -> Union[List[str], List[int], List[float], List[bool]]:
         """
@@ -53,34 +70,74 @@
     def to_json(self):
         return {"olive_parameter_type": "SearchParameter", "type": "Categorical", "support": self.support}
 
 
 class Boolean(Categorical):
     """
     Search parameter that supports a boolean value
+
+    Examples
+    --------
+    >>> Boolean()
     """
 
     def __init__(self):
         super().__init__([True, False])
 
 
 class Conditional(SearchParameter):
     """
     Conditional search parameter
+
+    Examples
+    --------
+    # conditional search parameter with one parent
+    # when parent1 is value1, the support is [1, 2, 3],
+    # when parent1 is value2, the support is [4, 5, 6],
+    # otherwise the support is [7, 8, 9]
+    >>> Conditional(
+            parents=("parent1",),
+            support={
+                ("value1",): Categorical([1, 2, 3]),
+                ("value2",): Categorical([4, 5, 6])
+            },
+            default=Categorical([4, 5, 6])
+        )
+
+    # conditional search parameter with two parents
+    # when parent1 is value1 and parent2 is value2, the support is [1, 2, 3], otherwise the support is Invalid
+    >>> Conditional(parents=("parent1", "parent2"), support={("value1", "value2"): Categorical([1, 2, 3])})
+
+    # when parent1 is value1 and parent2 is value2, the support is [1, 2, 3],
+    # when parent1 is value1 and parent2 is value3, the support is Invalid,
+    # otherwise the support is Ignored
+    >>> Conditional(
+            parents=("parent1", "parent2"),
+            support={
+                ("value1", "value2"): Categorical([1, 2, 3]),
+                ("value1", "value3"): Conditional.get_invalid_choice()
+            },
+            default=Conditional.get_ignored_choice()
+        )
     """
 
     def __init__(
         self,
         parents: Tuple[str],
         support: Dict[Tuple[Any], SearchParameter],
         default: SearchParameter = None,
     ):
+        assert isinstance(parents, tuple), "parents must be a tuple"
+        for key in support:
+            assert isinstance(key, tuple), "support key must be a tuple"
+            assert len(key) == len(parents), "support key length must match the number of parents"
+
         self.parents = parents
         self.support = support
-        self.default = default or Categorical([None])
+        self.default = default or self.get_invalid_choice()
 
     def get_support(self, parent_values: Dict[str, Any]) -> Union[List[str], List[int], List[float], List[bool]]:
         """
         get the support for the search parameter for a given parent value
         """
         assert parent_values.keys() == set(self.parents), "parent values keys do not match the parents"
         parent_values = tuple([parent_values[parent] for parent in self.parents])
@@ -133,25 +190,137 @@
             "olive_parameter_type": "SearchParameter",
             "type": "Conditional",
             "parents": self.parents,
             "support": support,
             "default": self.default.to_json(),
         }
 
+    @staticmethod
+    def get_invalid_choice():
+        """
+        Return a categorical search parameter with the invalid choice
+        """
+        return Categorical([SpecialParamValue.INVALID])
+
+    @staticmethod
+    def get_ignored_choice():
+        """
+        Return a categorical search parameter with the ignored choice
+        """
+        return Categorical([SpecialParamValue.IGNORED])
+
+
+class ConditionalDefault(Conditional):
+    """
+    Parameter with conditional default value
+
+    Examples
+    --------
+    # conditional default with one parent
+    # when parent1 is value1, the default is 1,
+    # when parent1 is value2, the default is 2,
+    # otherwise the default is 3
+    >>> ConditionalDefault(
+            parents=("parent1",),
+            support={
+                ("value1",): 1,
+                ("value2",): 2
+            },
+            default=3
+        )
+
+    # conditional default with two parents
+    # when parent1 is value1 and parent2 is value2, the default is 1,
+    # otherwise the default is Invalid
+    >>> ConditionalDefault(
+            parents=("parent1", "parent2"),
+            support={("value1", "value2"): 1}
+        )
+    """
+
+    def __init__(self, parents: Tuple[str], support: Dict[Tuple[Any], Any], default: Any = SpecialParamValue.INVALID):
+        support = {key: Categorical([value]) for key, value in support.items()}
+        default = Categorical([default])
+        super().__init__(parents, support, default)
+
+    def get_support(self, parent_values: Dict[str, Any]) -> Union[bool, int, float, str]:
+        """
+        get the support for the search parameter for a given parent value
+        """
+        return super().get_support(parent_values)[0]
+
+    def condition(self, parent_values: Dict[str, Any]) -> Union[bool, int, float, str, "ConditionalDefault"]:
+        """
+        Fix the parent value and return a new search parameter
+        """
+        value = super().condition(parent_values)
+        if isinstance(value, Categorical):
+            return value.get_support()[0]
+        if isinstance(value, Conditional):
+            return self.conditional_to_conditional_default(value)
+
+    @staticmethod
+    def conditional_to_conditional_default(conditional: Conditional) -> "ConditionalDefault":
+        """
+        Convert a conditional to a conditional default
+        """
+        support = {}
+        for key, value in conditional.support.items():
+            assert isinstance(value, Categorical), "Conditional support must be categorical"
+            assert len(value.get_support()) == 1, "Conditional support must have only one value"
+            support[key] = value.get_support()[0]
+        assert isinstance(conditional.default, Categorical), "Conditional default must be categorical"
+        assert len(conditional.default.get_support()) == 1, "Conditional default must have only one value"
+        return ConditionalDefault(conditional.parents, support, conditional.default.get_support()[0])
+
+    @staticmethod
+    def conditional_default_to_conditional(conditional_default: "ConditionalDefault") -> Conditional:
+        """
+        Convert a conditional default to a conditional
+        """
+        return Conditional(conditional_default.parents, conditional_default.support, conditional_default.default)
+
+    def __repr__(self):
+        support = {key: value.get_support()[0] for key, value in self.support.items()}
+        default = self.default.get_support()[0]
+        return f"ConditionalDefault(parents: {self.parents}, support: {support}, default: {default})"
+
+    def to_json(self):
+        json_data = super().to_json()
+        json_data["type"] = "ConditionalDefault"
+        return json_data
+
+    @staticmethod
+    def get_invalid_choice():
+        """
+        Return a categorical search parameter with the invalid choice
+        """
+        return SpecialParamValue.INVALID
+
+    @staticmethod
+    def get_ignored_choice():
+        """
+        Return a categorical search parameter with the ignored choice
+        """
+        return SpecialParamValue.IGNORED
+
 
 def json_to_search_parameter(json: Dict[str, Any]) -> SearchParameter:
     """
     Convert a json to a search parameter
     """
     assert json["olive_parameter_type"] == "SearchParameter", "Not a search parameter"
     search_parameter_type = json["type"]
     if search_parameter_type == "Categorical":
         return Categorical(json["support"])
-    if search_parameter_type == "Conditional":
+    if search_parameter_type == "Conditional" or search_parameter_type == "ConditionalDefault":
         stop_condition = lambda x: (  # noqa: E731
             isinstance(x, dict) and x.get("olive_parameter_type") == "SearchParameter"
         )
         support = flatten_dict(json["support"], stop_condition=stop_condition)
         for key, value in support.items():
             support[key] = json_to_search_parameter(value)
-        return Conditional(json["parents"], support, json_to_search_parameter(json["default"]))
+        conditional = Conditional(json["parents"], support, json_to_search_parameter(json["default"]))
+        if search_parameter_type == "ConditionalDefault":
+            return ConditionalDefault.conditional_to_conditional_default(conditional)
+        return conditional
     raise ValueError(f"Unknown search parameter type {search_parameter_type}")
```

## olive/strategy/search_results.py

```diff
@@ -2,18 +2,16 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from copy import deepcopy
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
-import pandas as pd
 
 from olive.common.utils import hash_dict
-from olive.strategy.utils import find_pareto_frontier_points
 
 
 class SearchResults:
     """
     This class stores the results of a search.
     """
 
@@ -51,87 +49,46 @@
         Report the result of a configuration.
         """
         search_point_hash = hash_dict(search_point)
         self.search_point_hash_table[search_point_hash] = deepcopy(search_point)
         self.results[search_point_hash] = deepcopy(result)
         self.model_ids[search_point_hash] = model_ids
 
-    def get_pareto_frontier(self, objectives: List[str] = None, apply_goals: bool = False) -> List[str]:
-        """
-        Return the pareto frontier of the search results.
-
-        If objectives is None, use all objectives.
-        If apply_goals is True, only return results that satisfy the goals.
-        """
-        search_point_hashes, results = self._get_results_list(objectives, apply_goals)
-
-        pareto_frontier_points = find_pareto_frontier_points(np.array(results))
-        pareto_frontier_hashes = [search_point_hashes[i] for i in pareto_frontier_points]
-
-        return [self.model_ids[point_hash][-1].split("_")[0] for point_hash in pareto_frontier_hashes]
-
-    def get_results_df(self, show_search_points: bool = False):
-        """
-        Return the results as a dataframe.
-        """
-        pareto_frontier = self.get_pareto_frontier(apply_constraints=False)["model_numbers"]
-
-        headers_1 = ["model_number"] + self.metrics + ["constraint_met", "is_pareto"]
-        if show_search_points:
-            search_point = self.search_point_hash_table[list(self.search_point_hash_table.keys())[0]]
-            for pass_name in search_point:
-                for pass_param in search_point[pass_name]:
-                    headers_1.append(f"{pass_name}:{pass_param}")
-
-        df = pd.DataFrame(columns=headers_1)
-        for search_point_hash, result in self.results.items():
-            if result == {}:
-                continue
-            model_id = self.model_ids[search_point_hash][-1]
-            model_number = model_id.split("_")[0]
-            row = [model_number] + [result.get(metric, "") for metric in self.metrics]
-            row.append(self.check_constraints(result))
-            row.append(model_number in pareto_frontier)
-            if show_search_points:
-                search_point = self.search_point_hash_table[search_point_hash]
-                for pass_name in search_point:
-                    for pass_param in search_point[pass_name]:
-                        row.append(search_point[pass_name][pass_param])
-            df.loc[len(df)] = row
-
-        return df
-
     def check_goals(self, result: Dict[str, Union[float, int]]) -> bool:
         """
         Check if the result satisfies the constraints.
         """
+        # if goals are not set, return True always
         if self.goals == {}:
-            return False
+            return True
 
         for obj, goal in self.goals.items():
             if self.obj_mul[obj] * result[obj] < self.obj_mul[obj] * goal:
                 return False
         return True
 
     def sort_search_points(self, objectives: List[str] = None, apply_goals: bool = False) -> List[str]:
         """
         Return the search points sorted by the objectives.
         """
+        # TODO this function only works for pass-by-pass execution order, but only return with the first model
+        # with the best latency results which is not correct. One pass may generate multiple models.
         if objectives is None:
             objectives = self.objectives
         else:
             assert set(objectives).issubset(self.objectives)
 
         results, search_point_hashes = self._get_results_list(objectives, apply_goals)
         if not results:
             return None, None, None
 
-        # sort by objectives
-        results = np.array(results)
-        results *= np.array([self.obj_mul[obj] for obj in objectives])
+        # sort by objectives, left most objective has highest priority
+        # flip the order of the objectives since np.lexsort prioritizes the last column
+        # negate the results since np.lexsort sorts in ascending order
+        results = -np.flip(np.array(results), 1)
         sorted_indices = np.lexsort(results.T)
         sorted_hashes = [search_point_hashes[i] for i in sorted_indices]
 
         # get model numbers
         sorted_model_ids = [self.model_ids[point_hash] for point_hash in sorted_hashes]
         sorted_results = [self.results[point_hash] for point_hash in sorted_hashes]
         # TODO: this will be done using helper later
@@ -139,14 +96,16 @@
         return sorted_model_ids, sorted_search_points, sorted_results
 
     def _get_results_list(
         self, objectives: List[str] = None, apply_goals: bool = False
     ) -> Tuple[List[List[float]], List[str]]:
         """
         Return the results as a list of lists.
+
+        Values are multiplied by the objective multiplier so that higher is better for all objectives.
         """
         if objectives is None:
             objectives = self.objectives
         else:
             assert set(objectives).issubset(self.objectives)
 
         search_point_hashes = []
```

## olive/strategy/search_space.py

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from copy import deepcopy
 from random import Random
 from typing import Any, Dict, List, Optional, Tuple
 
-from olive.strategy.search_parameter import Categorical, Conditional, SearchParameter
+from olive.strategy.search_parameter import Categorical, Conditional, SearchParameter, SpecialParamValue
 from olive.strategy.utils import order_search_parameters
 
 
 class SearchSpace:
     """
     Search space for a search algorithm.
     """
@@ -59,14 +59,16 @@
             param = self._search_space[space_name][param_name]
             if isinstance(param, Conditional):
                 parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
                 options = param.get_support(parent_vals)
             elif isinstance(param, Categorical):
                 options = param.get_support()
             search_point[space_name][param_name] = self.rng.choice(options)
+            if search_point[space_name][param_name] == SpecialParamValue.INVALID:
+                return self.random_sample()
 
         return search_point
 
     def _iterate_util(
         self, full_iter_order: List[Tuple[str, str]], search_point: Dict[str, Dict[str, Any]], index: int
     ):
         if index == len(full_iter_order):
@@ -78,14 +80,16 @@
 
         if isinstance(param, Conditional):
             parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
             options = param.get_support(parent_vals)
         elif isinstance(param, Categorical):
             options = param.get_support()
         for option in options:
+            if option == SpecialParamValue.INVALID:
+                continue
             search_point[space_name][param_name] = option
             yield from self._iterate_util(full_iter_order, search_point, index + 1)
 
     def iterate(self) -> Dict[str, Dict[str, Any]]:
         """
         Iterate over all possible configurations in the search space.
         """
```

## olive/strategy/search_strategy.py

```diff
@@ -19,14 +19,15 @@
 _VALID_EXECUTION_ORDERS = ["joint", "pass-by-pass"]
 
 
 class SearchStrategyConfig(ConfigBase):
     execution_order: str
     search_algorithm: str
     search_algorithm_config: ConfigBase = None
+    output_model_num: int = None
     stop_when_goals_met: bool = False
     max_iter: int = None
     max_time: int = None
 
     @validator("execution_order", pre=True)
     def _validate_execution_order(cls, v):
         if v not in _VALID_EXECUTION_ORDERS:
@@ -81,23 +82,23 @@
         """
         self._objective_dict = objective_dict
 
         # search spaces
         self._spaces_order = [search_space[0] for search_space in search_spaces_list]
         self._spaces_dict = {search_space[0]: search_space[1] for search_space in search_spaces_list}
 
-        # search space dictionaries for pass are grouped based on exection_order
+        # search space dictionaries for pass are grouped based on execution_order
         self._spaces_groups = self._group_search_spaces(self._spaces_order)
         self._done_spaces_groups = []
         self._active_spaces_group = None
 
         # state
-        self._searchers = {}
-        self._search_results = {}
-        self._init_model_ids = {}
+        self._searchers: Dict[Any, SearchAlgorithm] = {}
+        self._search_results: Dict[Any, SearchResults] = {}
+        self._init_model_ids: Dict[Any, str] = {}
         self._best_search_points = {}
 
         # initialize the first search space
         self._next_search_group(init_model_id)
 
         self._initialized = True
 
@@ -116,30 +117,48 @@
 
         return search_spaces_groups
 
     def _next_search_group(self, init_model_id: Optional[str] = None) -> Optional[SearchAlgorithm]:
         """
         Get the next search space group and initialize the search algorithm.
         """
-        # TODO: organize the state better and make exection order more flexible using a graph
+        # TODO: organize the state better and make execution order more flexible using a graph
         if self._active_spaces_group is not None:
             self._done_spaces_groups.append(self._active_spaces_group)
             # legacy, will update once search results has info function
             sorted_model_ids, sorted_search_points, sorted_results = self._search_results[
                 tuple(self._active_spaces_group)
-            ].sort_search_points()
+            ].sort_search_points(apply_goals=True)
+            if sorted_model_ids is None:
+                logger.warning(
+                    f"No models in this search group {self._active_spaces_group} met the goals. Sorting the models"
+                    " without applying goals..."
+                )
+                sorted_model_ids, sorted_search_points, sorted_results = self._search_results[
+                    tuple(self._active_spaces_group)
+                ].sort_search_points(apply_goals=False)
+            # TODO: this is a hack to get the best search point for the current search space group
+            #      it totally work for joint execution order, but not for pass-by-pass
             if sorted_search_points and sorted_results:
                 best_search_point = (sorted_search_points[0], list(sorted_results[0].values()), sorted_model_ids[0])
                 self._best_search_points[tuple(self._active_spaces_group)] = best_search_point
                 init_model_id = best_search_point[2][-1]
 
         if len(self._spaces_groups) == 0:
             self._active_spaces_group = None
             return None
 
+        if init_model_id is None and self._active_spaces_group is None:
+            raise ValueError("init_model_id must be provided for the first search group")
+        if init_model_id is None and self._active_spaces_group is not None:
+            raise ValueError(
+                f"The previous search group {self._active_spaces_group} has no output models that were created and"
+                " evaluated successfully. Cannot continue."
+            )
+
         self._active_spaces_group = self._spaces_groups.pop(0)
         self._searchers[tuple(self._active_spaces_group)] = self._create_searcher(self._active_spaces_group)
         self._search_results[tuple(self._active_spaces_group)] = SearchResults(self._objective_dict)
         self._init_model_ids[tuple(self._active_spaces_group)] = init_model_id
 
         return self._active_spaces_group
 
@@ -201,14 +220,17 @@
         self._searchers[tuple(self._active_spaces_group)].report(search_point, signal, should_prune)
 
     def check_exit_criteria(self, iter_num, time_diff, metric_signal):
         """
         Check if the olive search_strategy should exit.
         """
         self.exit_criteria_met = False
+        if not self._config.stop_when_goals_met:
+            # stop early stopping when stop_when_goals_met is False, but still apply goals check without stopping
+            return
         # early exit is not supported for pass-by-pass execution order currently
         if self._config.execution_order == "pass-by-pass":
             return
         if self._config.max_iter is not None and iter_num > self._config.max_iter:
             self.exit_criteria_met = True
             return
         if self._config.max_time is not None and time_diff > self._config.max_time:
@@ -216,30 +238,9 @@
             return
         if metric_signal == {}:
             return
         self.exit_criteria_met = self._config.stop_when_goals_met and self._search_results[
             tuple(self._active_spaces_group)
         ].check_goals(metric_signal)
 
-    def get_best_execution(self) -> Dict[str, Any]:
-        """
-        Get the best execution found so far.
-        """
-        best_search_points = {}
-        best_metric = None
-        best_model_ids = []
-
-        # legacy will update once search results has info function
-        for spaces_group in self._done_spaces_groups:
-            annotated_search_point = self._best_search_points.get(tuple(spaces_group), None)
-            if not annotated_search_point:
-                continue
-            for space_name in spaces_group:
-                best_search_points[space_name] = annotated_search_point[0][space_name]
-            best_metric = annotated_search_point[1]
-            best_model_ids += annotated_search_point[2]
-
-        return {
-            "search_points": best_search_points,
-            "metric": best_metric,
-            "model_ids": best_model_ids,
-        }
+    def get_output_model_num(self):
+        return self._config.output_model_num
```

## olive/strategy/utils.py

```diff
@@ -1,15 +1,13 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from typing import Dict, List, Set, Tuple
 
-import numpy as np
-
 from olive.strategy.search_parameter import Conditional, SearchParameter
 
 
 class DirectedGraph:
     def __init__(self, vertices: List[str], edges: List[Tuple[str, str]] = None):
         self.vertices = vertices
         self.graph = {v: [] for v in vertices}
@@ -89,38 +87,7 @@
 
 def order_search_parameters(search_space: Dict[str, SearchParameter]) -> List[str]:
     """
     Order the search parameters in a topological order.
     """
     graph = _search_space_graph(search_space)
     return graph.topological_sort()
-
-
-def find_pareto_frontier_points(points: np.ndarray) -> List[int]:
-    """
-    Find the pareto frontier points in a set of points.
-    """
-    assert points.ndim == 2, "Points must be a 2D array."
-    # assert points.shape[1] > 1, "Points must have more than 1 dimension."
-
-    # Find the pareto frontier points
-    pareto_frontier_points = np.array([])
-    for idx, point in enumerate(points):
-        if len(pareto_frontier_points) == 0:
-            pareto_frontier_points = np.append(pareto_frontier_points, idx)
-            continue
-
-        frontier = points[pareto_frontier_points.astype(int)]
-
-        # check if point is dominated by another point on the pareto front
-        is_dominated = np.all(point <= frontier, axis=1)
-        if np.any(is_dominated):
-            continue
-
-        # remove points from the pareto front dominated by point
-        dominates = np.all(point >= frontier, axis=1)
-        pareto_frontier_points = pareto_frontier_points[~dominates]
-
-        # add point to the pareto front
-        pareto_frontier_points = np.append(pareto_frontier_points, idx)
-
-    return pareto_frontier_points.astype(int).tolist()
```

## olive/strategy/search_algorithm/optuna_sampler.py

```diff
@@ -6,31 +6,31 @@
 from typing import Any, Dict, Tuple, Union
 
 import optuna
 
 from olive.common.config_utils import ConfigParam
 from olive.common.utils import hash_dict
 from olive.strategy.search_algorithm.search_algorithm import SearchAlgorithm
-from olive.strategy.search_parameter import Categorical, Conditional
+from olive.strategy.search_parameter import Categorical, Conditional, SpecialParamValue
 
 optuna.logging.set_verbosity(optuna.logging.WARNING)
 
 
 class OptunaSearchAlgorithm(SearchAlgorithm):
     """
     Optuna sampler for search algorithms.
     """
 
     name = "optuna_sampler"
 
     @staticmethod
     def _default_config() -> Dict[str, ConfigParam]:
         return {
-            "num_samples": ConfigParam(type_=int, default=1, description="Number of samples to suggest."),
-            "seed": ConfigParam(type_=int, default=1, description="Seed for the rng."),
+            "num_samples": ConfigParam(type_=int, default_value=1, description="Number of samples to suggest."),
+            "seed": ConfigParam(type_=int, default_value=1, description="Seed for the rng."),
         }
 
     def initialize(self):
         """
         Initialize the searcher.
         """
         self._sampler = self._create_sampler()
@@ -57,15 +57,18 @@
     def suggest(self) -> Dict[str, Dict[str, Any]]:
         """
         Suggest a new configuration to try.
         """
         if self.should_stop():
             return None
 
-        trial, search_point = self._get_trial()
+        trial, search_point, invalid = self._get_trial()
+        if invalid:
+            self._study.tell(trial.number, state=optuna.trial.TrialState.PRUNED)
+            return self.suggest()
 
         # save history
         search_point_hash = hash_dict(search_point)
         self._trial_ids[search_point_hash] = trial.number
 
         self._num_samples_suggested += 1
 
@@ -73,29 +76,31 @@
 
     def _get_trial(self) -> Tuple[optuna.trial.Trial, Dict[str, Dict[str, Any]]]:
         """
         Get a trial from the study.
         """
         trial = self._study.ask()
         search_point = self._search_space.empty_search_point()
+        invalid_trial = False
         for space_name, param_name, param in self._search_space.iter_params():
             if space_name not in search_point:
                 search_point[space_name] = {}
             suggestion_name = f"{space_name}___{param_name}"
             if isinstance(param, Categorical):
                 search_point[space_name][param_name] = trial.suggest_categorical(suggestion_name, param.get_support())
             elif isinstance(param, Conditional):
                 parent_vals = {parent: search_point[space_name][parent] for parent in param.parents}
                 options = param.get_support(parent_vals)
                 parent_vals_name = "_".join([f"{v}" for _, v in parent_vals.items()])
                 suggestion_name = f"{space_name}___{param_name}___{parent_vals_name}"
                 search_point[space_name][param_name] = trial.suggest_categorical(suggestion_name, options)
             else:
                 raise ValueError(f"Unsupported parameter type: {type(param)}")
-        return trial, search_point
+            invalid_trial = invalid_trial or (search_point[space_name][param_name] == SpecialParamValue.INVALID)
+        return trial, search_point, invalid_trial
 
     def report(
         self, search_point: Dict[str, Dict[str, Any]], result: Dict[str, Union[float, int]], should_prune: bool = False
     ):
         search_point_hash = hash_dict(search_point)
         trial_id = self._trial_ids[search_point_hash]
         if should_prune:
```

## olive/strategy/search_algorithm/random_sampler.py

```diff
@@ -14,17 +14,17 @@
     """
 
     name = "random"
 
     @staticmethod
     def _default_config() -> Dict[str, ConfigParam]:
         return {
-            "num_samples": ConfigParam(type_=int, default=1, description="Number of samples to suggest."),
-            "seed": ConfigParam(type_=int, default=1, description="Seed for the rng."),
-            "with_replacement": ConfigParam(type_=bool, default=False, description="Sample with replacement."),
+            "num_samples": ConfigParam(type_=int, default_value=1, description="Number of samples to suggest."),
+            "seed": ConfigParam(type_=int, default_value=1, description="Seed for the rng."),
+            "with_replacement": ConfigParam(type_=bool, default_value=False, description="Sample with replacement."),
         }
 
     def initialize(self):
         """
         Initialize the searcher.
         """
         self._search_space.set_seed(self._config.seed)
```

## olive/strategy/search_algorithm/search_algorithm.py

```diff
@@ -29,14 +29,16 @@
         search_space: Dict[str, Dict[str, SearchParameter]],
         objectives: Optional[List[str]] = None,
         higher_is_betters: Optional[List[bool]] = None,
         config: Optional[Union[Dict[str, Any], ConfigBase]] = None,
     ):
         # search space
         self._search_space = SearchSpace(search_space)
+        if self._search_space.size() == 0:
+            raise ValueError("There are no valid points in the search space.")
 
         # objectives and directions
         objectives = objectives or []
         higher_is_betters = higher_is_betters or []
         assert len(objectives) == len(higher_is_betters), "Number of objectives must match number of higher_is_betters"
         self._objectives = objectives
         self._higher_is_betters = higher_is_betters
```

## olive/strategy/search_algorithm/tpe_sampler.py

```diff
@@ -21,19 +21,19 @@
     name = "tpe"
 
     @staticmethod
     def _default_config() -> Dict[str, ConfigParam]:
         return {
             **OptunaSearchAlgorithm._default_config(),
             "multivariate": ConfigParam(
-                type_=bool, default=True, description="Use multivariate TPE when suggesting parameters."
+                type_=bool, default_value=True, description="Use multivariate TPE when suggesting parameters."
             ),
             "group": ConfigParam(
                 type_=bool,
-                default=True,
+                default_value=True,
                 description=(
                     "If this and multivariate are True, the multivariate TPE with the group decomposed search space is"
                     " used when suggesting parameters. Refer to 'group' at"
                     " https://optuna.readthedocs.io/en/stable/reference/samplers/generated/"
                     "optuna.samplers.TPESampler.html for more information."
                 ),
             ),
```

## olive/systems/common.py

```diff
@@ -11,14 +11,15 @@
 from olive.common.config_utils import ConfigBase
 
 
 class SystemType(str, Enum):
     Docker = "Docker"
     Local = "LocalSystem"
     AzureML = "AzureML"
+    PythonEnvironment = "PythonEnvironment"
 
 
 class Device(str, Enum):
     CPU = "cpu"
     GPU = "gpu"
     NPU = "npu"
     INTEL_MYRIAD = "intel_myriad"
@@ -48,14 +49,14 @@
     dockerfile: Optional[str] = None
     build_context_path: Optional[Union[Path, str]] = None
     build_args: Optional[dict] = None
     run_params: Optional[dict] = None
 
     @validator("build_context_path", "requirements_file_path")
     def _get_abspath(cls, v):
-        return str(Path(v).resolve())
+        return str(Path(v).resolve()) if v else None
 
     @validator("dockerfile", always=True)
     def _validate_one_of_dockerfile_or_base_image(cls, v, values):
         if v is None and values.get("requirements_file_path") is None:
             raise ValueError("One of build_context_path/dockerfile or requirements_file_path must be provided")
         return v
```

## olive/systems/local.py

```diff
@@ -1,26 +1,27 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from typing import Any, Dict, List, Optional
 
-from olive.evaluator.evaluation import evaluate_accuracy, evaluate_custom_metric, evaluate_latency
-from olive.evaluator.metric import Metric, MetricType
-from olive.model import OliveModel
+from olive.evaluator.metric import Metric
+from olive.evaluator.olive_evaluator import OliveEvaluator, OliveEvaluatorFactory
+from olive.model import CompositeOnnxModel, OliveModel
 from olive.passes.olive_pass import Pass
 from olive.systems.common import Device, SystemType
 from olive.systems.olive_system import OliveSystem
 
 
 class LocalSystem(OliveSystem):
     system_type = SystemType.Local
 
     def __init__(self, device: Device = Device.CPU):
-        super().__init__(device)
+        self.device = device
+        super().__init__()
 
     def run_pass(
         self,
         the_pass: Pass,
         model: OliveModel,
         output_model_path: str,
         point: Optional[Dict[str, Any]] = None,
@@ -30,16 +31,12 @@
         """
         return the_pass.run(model, output_model_path, point)
 
     def evaluate_model(self, model: OliveModel, metrics: List[Metric]) -> Dict[str, Any]:
         """
         Evaluate the model
         """
-        metrics_res = {}
-        for metric in metrics:
-            if metric.type == MetricType.ACCURACY:
-                metrics_res[metric.name] = evaluate_accuracy(model, metric, self.device)
-            elif metric.type == MetricType.LATENCY:
-                metrics_res[metric.name] = evaluate_latency(model, metric, self.device)
-            else:
-                metrics_res[metric.name] = evaluate_custom_metric(model, metric, self.device)
-        return metrics_res
+        if isinstance(model, CompositeOnnxModel):
+            raise NotImplementedError()
+
+        evaluator: OliveEvaluator = OliveEvaluatorFactory.create_evaluator_for_model(model)
+        return evaluator.evaluate(model, metrics, device=self.device)
```

## olive/systems/olive_system.py

```diff
@@ -5,25 +5,23 @@
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional
 
 from olive.evaluator.metric import Metric
 from olive.model import OliveModel
 from olive.passes.olive_pass import Pass
-from olive.systems.common import Device, SystemType
+from olive.systems.common import SystemType
 
 logger = logging.getLogger(__name__)
 
 
 class OliveSystem(ABC):
     system_type: SystemType
 
-    def __init__(self, device: Device):
-        # device arg will be removed
-        self.device = device
+    def __init__(self):
         self.accelerators = []
 
     @abstractmethod
     def run_pass(
         self,
         the_pass: Pass,
         model: OliveModel,
```

## olive/systems/system_config.py

```diff
@@ -1,51 +1,81 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import importlib
+import shutil
 from pathlib import Path
-from typing import Union
+from typing import Dict, List, Union
 
 from pydantic import validator
 
+from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.common.config_utils import ConfigBase, validate_config
 from olive.systems.common import AzureMLDockerConfig, Device, LocalDockerConfig, SystemType
 
 
 class TargetUserConfig(ConfigBase):
-    device: Device = Device.CPU
+    pass
 
 
 class LocalTargetUserConfig(TargetUserConfig):
-    pass
+    device: Device = Device.CPU
 
 
 class DockerTargetUserConfig(TargetUserConfig):
     local_docker_config: LocalDockerConfig
+    is_dev: bool = False
 
 
 class AzureMLTargetUserConfig(TargetUserConfig):
-    aml_config_path: Union[Path, str]
+    azureml_client_config: AzureMLClientConfig = None
     aml_compute: str
     aml_docker_config: AzureMLDockerConfig
     instance_count: int = 1
     is_dev: bool = False
 
 
+class PythonEnvironmentTargetUserConfig(TargetUserConfig):
+    device: Device = Device.CPU
+    python_environment_path: Union[
+        Path, str
+    ]  # path to the python environment, e.g. /home/user/anaconda3/envs/myenv, /home/user/.virtualenvs/myenv
+    environment_variables: Dict[str, str] = None  # os.environ will be updated with these variables
+    prepend_to_path: List[str] = None  # paths to prepend to os.environ["PATH"]
+
+    @validator("python_environment_path", "prepend_to_path", pre=True, each_item=True)
+    def _get_abspath(cls, v):
+        return str(Path(v).resolve()) if v else None
+
+    @validator("python_environment_path")
+    def _validate_python_environment_path(cls, v):
+        # check if the path exists
+        if not Path(v).exists():
+            raise ValueError(f"Python path {v} does not exist")
+
+        # check if python exists in the path
+        python_path = shutil.which("python", path=v)
+        if not python_path:
+            raise ValueError(f"Python executable not found in the path {v}")
+        return v
+
+
 _type_to_config = {
     SystemType.Local: LocalTargetUserConfig,
     SystemType.AzureML: AzureMLTargetUserConfig,
     SystemType.Docker: DockerTargetUserConfig,
+    SystemType.PythonEnvironment: PythonEnvironmentTargetUserConfig,
 }
 
 _type_to_system_path = {
     SystemType.Local: "olive.systems.local.LocalSystem",
     SystemType.AzureML: "olive.systems.azureml.AzureMLSystem",
     SystemType.Docker: "olive.systems.docker.DockerSystem",
+    SystemType.PythonEnvironment: "olive.systems.python_environment.PythonEnvironmentSystem",
 }
 
 
 def import_system_from_type(system_type: SystemType):
     system_path = _type_to_system_path[system_type]
     module_path, class_name = system_path.rsplit(".", 1)
     module = importlib.import_module(module_path)
@@ -63,8 +93,10 @@
 
         system_type = values["type"]
         config_class = _type_to_config[system_type]
         return validate_config(v, config_class)
 
     def create_system(self):
         system_class = import_system_from_type(self.type)
+        if system_class.system_type == SystemType.AzureML and not self.config.azureml_client_config:
+            raise ValueError("azureml_client is required for AzureML system")
         return system_class(**self.config.dict())
```

## olive/systems/utils.py

```diff
@@ -1,13 +1,16 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import argparse
 import json
+from pathlib import Path
+
+from olive.model import ModelStorageKind
 
 
 def parse_common_args(raw_args):
     parser = argparse.ArgumentParser("Olive model args")
 
     # model args
     parser.add_argument("--model_config", type=str, help="model config", required=True)
@@ -19,14 +22,20 @@
     # model output args
     parser.add_argument("--pipeline_output", type=str, help="pipeline output path", required=True)
 
     return parser.parse_known_args(raw_args)
 
 
 def get_model_config(common_args):
-    model_json = json.load(open(common_args.model_config))
+    with open(common_args.model_config) as f:
+        model_json = json.load(f)
 
     for key, value in common_args.__dict__.items():
         if value and key in model_json["config"]:
             model_json["config"][key] = value
+    if (
+        model_json["type"].lower() == "onnxmodel"
+        and model_json["config"]["model_storage_kind"] == ModelStorageKind.LocalFolder
+    ):
+        model_json["config"]["model_path"] = str(Path(model_json["config"]["model_path"]) / "model.onnx")
 
     return model_json
```

## olive/systems/azureml/aml_evaluation_runner.py

```diff
@@ -3,57 +3,61 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import argparse
 import json
 from pathlib import Path
 
 from olive.evaluator.metric import Metric
-from olive.evaluator.olive_evaluator import OliveEvaluator
 from olive.model import ModelConfig
+from olive.systems.local import LocalSystem
+from olive.systems.olive_system import OliveSystem
 from olive.systems.utils import get_model_config, parse_common_args
 
 
 def parse_metric_args(raw_args):
     parser = argparse.ArgumentParser("Metric config")
 
     parser.add_argument("--metric_config", type=str, help="pass config", required=True)
-    parser.add_argument("--metric_user_script", type=str, help="metric user script", required=True)
+    parser.add_argument("--metric_user_script", type=str, help="metric user script")
     parser.add_argument("--metric_script_dir", type=str, help="metric script dir")
     parser.add_argument("--metric_data_dir", type=str, help="metric data dir")
 
     return parser.parse_args(raw_args)
 
 
 def create_metric(metric_config, metric_args):
     for key, value in vars(metric_args).items():
+        if key == "metric_config":
+            continue
         if value is not None:
             key = key.replace("metric_", "")
             metric_config["user_config"][key] = value
 
     p = Metric.from_json(metric_config)
     return p
 
 
 def main(raw_args=None):
     common_args, extra_args = parse_common_args(raw_args)
     metric_args = parse_metric_args(extra_args)
 
+    # load metric
+    with open(metric_args.metric_config) as f:
+        metric_config = json.load(f)
+    metric = create_metric(metric_config, metric_args)
+
     # load model
     model_config = get_model_config(common_args)
     model = ModelConfig.from_json(model_config).create_model()
 
-    # load metric
-    metric_config = json.load(open(metric_args.metric_config))
-    metric = create_metric(metric_config, metric_args)
-
-    # create_evaluator
-    evaluator = OliveEvaluator([metric])
+    target: OliveSystem = LocalSystem()
 
     # metric result
-    metric_result = evaluator.evaluate(model)
+    metric_result = target.evaluate_model(model, [metric])
 
     # save metric result json
-    json.dump(metric_result, open(Path(common_args.pipeline_output) / "metric_result.json", "w"))
+    with open(Path(common_args.pipeline_output) / "metric_result.json", "w") as f:
+        json.dump(metric_result, f)
 
 
 if __name__ == "__main__":
     main()
```

## olive/systems/azureml/aml_pass_runner.py

```diff
@@ -24,14 +24,15 @@
 
 
 def parse_pass_args(pass_type, raw_args):
     pass_class = PASS_REGISTRY[pass_type]
 
     parser = argparse.ArgumentParser(f"{pass_type} pass args")
 
+    # TODO: get accelerator specs from args when it is implemented
     # parse pass args
     for param, param_config in pass_class.default_config().items():
         if param_config.is_path:
             parser.add_argument(f"--pass_{param}", type=str, help=f"pass {param}", required=param_config.required)
 
     return parser.parse_args(raw_args)
 
@@ -47,30 +48,31 @@
 
 
 def main(raw_args=None):
     common_args, extra_args = parse_common_args(raw_args)
     pass_config_arg, extra_args = parse_pass_config_arg(extra_args)
 
     # pass config
-    pass_config = json.load(open(pass_config_arg.pass_config))
+    with open(pass_config_arg.pass_config) as f:
+        pass_config = json.load(f)
     pass_type = pass_config["type"].lower()
 
     # TODO: contact ort team for a workaround
     # Some passes create temporary files in the same directory as the model
     # original directory for model path is read only, so we need to copy the model to a temp directory
     # TODO: test if sym link solves it
     if common_args.model_path is not None:
         tmp_dir = tempfile.TemporaryDirectory()
         old_path = Path(common_args.model_path).resolve()
         new_path = Path(tmp_dir.name).resolve() / old_path.name
         if old_path.is_file():
             shutil.copy(old_path, new_path)
         else:
             new_path.mkdir(parents=True, exist_ok=True)
-            shutil.copytree(old_path, new_path)
+            shutil.copytree(old_path, new_path, dirs_exist_ok=True)
         common_args.model_path = str(new_path)
 
     # pass specific args
     pass_args = parse_pass_args(pass_type, extra_args)
 
     # load input_model
     input_model_config = get_model_config(common_args)
@@ -84,21 +86,27 @@
     output_model_path = str(Path(common_args.pipeline_output) / "output_model")
 
     # run pass
     output_model = p.run(input_model, output_model_path)
 
     # save model json
     model_json = output_model.to_json()
+
+    # Replace output model HF config with input model HF config
+    if input_model_config["config"].get("hf_config"):
+        model_json["config"]["hf_config"] = input_model_config["config"]["hf_config"]
+
     # this is to handle passes like OrtPerfTuning that use the same model file as input
     model_json["same_model_path_as_input"] = False
     if model_json["config"]["model_path"] is not None:
         model_path = str(Path(model_json["config"]["model_path"]).resolve())
         if model_path == input_model_path:
             model_json["config"]["model_path"] = None
             model_json["same_model_path_as_input"] = True
         else:
             model_json["config"]["model_path"] = str(Path(model_path).relative_to(Path(common_args.pipeline_output)))
-    json.dump(model_json, open(Path(common_args.pipeline_output) / "output_model_config.json", "w"), indent=4)
+    with open(Path(common_args.pipeline_output) / "output_model_config.json", "w") as f:
+        json.dump(model_json, f, indent=4)
 
 
 if __name__ == "__main__":
     main()
```

## olive/systems/azureml/aml_system.py

```diff
@@ -5,176 +5,182 @@
 import json
 import logging
 import shutil
 import tempfile
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from azure.ai.ml import Input, MLClient, Output, command
+from azure.ai.ml import Input, Output, command
 from azure.ai.ml.constants import AssetTypes
 from azure.ai.ml.dsl import pipeline
 from azure.ai.ml.entities import BuildContext, Environment
 from azure.core.exceptions import HttpResponseError, ServiceResponseError
-from azure.identity import AzureCliCredential, DefaultAzureCredential, InteractiveBrowserCredential
 
+from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.common.config_utils import validate_config
 from olive.common.utils import retry_func
 from olive.constants import Framework
 from olive.evaluator.metric import Metric
-from olive.model import ModelConfig, OliveModel
+from olive.model import ModelConfig, ModelStorageKind, OliveModel, ONNXModel
 from olive.passes.olive_pass import Pass
-from olive.systems.common import AzureMLDockerConfig, Device, SystemType
+from olive.systems.common import AzureMLDockerConfig, SystemType
 from olive.systems.olive_system import OliveSystem
 
 logger = logging.getLogger(__name__)
 
 
 class AzureMLSystem(OliveSystem):
     system_type = SystemType.AzureML
 
     def __init__(
         self,
-        aml_config_path: str,
+        azureml_client_config: AzureMLClientConfig,
         aml_compute: str,
         aml_docker_config: Union[Dict[str, Any], AzureMLDockerConfig],
-        device: Device = Device.CPU,
         instance_count: int = 1,
         is_dev: bool = False,
     ):
-        super().__init__(device)
+        super().__init__()
         self._assert_not_none(aml_docker_config)
         aml_docker_config = validate_config(aml_docker_config, AzureMLDockerConfig)
-        self.device = device
-        self.ml_client = MLClient.from_config(self._get_credentials(), path=aml_config_path)
+        azureml_client_config = validate_config(azureml_client_config, AzureMLClientConfig)
+        self.azureml_client_config = azureml_client_config
         self.compute = aml_compute
         self.environment = self._create_environment(aml_docker_config)
         self.instance_count = instance_count
         self.is_dev = is_dev
 
     def _create_environment(self, docker_config: AzureMLDockerConfig):
         if docker_config.build_context_path:
             return Environment(
                 build=BuildContext(dockerfile_path=docker_config.dockerfile, path=docker_config.build_context_path)
             )
         if docker_config.base_image:
             return Environment(image=docker_config.base_image, conda_file=docker_config.conda_file_path)
         raise Exception("Please specify DockerConfig.")
 
-    def _get_credentials(self):
-        try:
-            credential = AzureCliCredential()
-            credential.get_token("https://management.azure.com/.default")
-        except Exception:
-            try:
-                credential = DefaultAzureCredential()
-                # Check if given credential can get token successfully.
-                credential.get_token("https://management.azure.com/.default")
-            except Exception:
-                # Fall back to InteractiveBrowserCredential in case DefaultAzureCredential not work
-                credential = InteractiveBrowserCredential()
-
-        return credential
-
     def _assert_not_none(self, object):
         if object is None:
             raise Exception(f"{object.__class__.__name__} is missing in the inputs!")
 
     def run_pass(
         self,
         the_pass: Pass,
         model: OliveModel,
         output_model_path: str,
         point: Optional[Dict[str, Any]] = None,
     ) -> OliveModel:
         """
         Run the pass on the model at a specific point in the search space.
         """
+        ml_client = self.azureml_client_config.create_client()
         point = point or {}
         config = the_pass.config_at_search_point(point)
         pass_config = the_pass.to_json(check_objects=True)
         pass_config["config"].update(the_pass.serialize_config(config, check_objects=True))
 
         with tempfile.TemporaryDirectory() as tempdir:
             pipeline_job = self._create_pipeline_for_pass(tempdir, model, pass_config, the_pass.path_params)
 
             # submit job
             logger.debug("Submitting pipeline")
             job = retry_func(
-                self.ml_client.jobs.create_or_update,
+                ml_client.jobs.create_or_update,
                 [pipeline_job],
                 {"experiment_name": "olive-pass", "tags": {"Pass": pass_config["type"]}},
                 max_tries=3,
                 delay=5,
                 exceptions=HttpResponseError,
             )
             logger.info(f"Pipeline submitted. Job name: {job.name}. Job link: {job.studio_url}")
-            self.ml_client.jobs.stream(job.name)
+            ml_client.jobs.stream(job.name)
 
             # get output
             output_dir = Path(tempdir) / "pipeline_output"
             output_dir.mkdir(parents=True, exist_ok=True)
             logger.debug(f"Downloading pipeline output to {output_dir}")
             retry_func(
-                self.ml_client.jobs.download,
+                ml_client.jobs.download,
                 [job.name],
                 {"output_name": "pipeline_output", "download_path": output_dir},
                 max_tries=3,
                 delay=5,
                 exceptions=ServiceResponseError,
             )
 
             pipeline_output_path = output_dir / "named-outputs" / "pipeline_output"
 
             return self._load_model(model, output_model_path, pipeline_output_path)
 
-    def _create_model_inputs(self, is_aml_model: bool):
+    def _create_model_inputs(self, model_storage_kind: ModelStorageKind):
         return {
             "model_config": Input(type=AssetTypes.URI_FILE),
             # aml supports uploading file/folder even though model_path is typed as URI_FOLDER
             "model_path": Input(type=AssetTypes.CUSTOM_MODEL)
-            if is_aml_model
+            if model_storage_kind == ModelStorageKind.AzureMLModel
             else Input(type=AssetTypes.URI_FOLDER, optional=True),
             "model_script": Input(type=AssetTypes.URI_FILE, optional=True),
             "model_script_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
         }
 
     def _create_model_args(self, model_json: dict, tmp_dir: Path):
-        # TODO: consider symlinkinking model_script and model_script_dir also when we decide
+        # TODO: consider symlinking model_script and model_script_dir also when we decide
         # the relationship between the two
         model_script = None
         if model_json["config"].get("model_script"):
             model_script = Input(type=AssetTypes.URI_FILE, path=model_json["config"]["model_script"])
             model_json["config"]["model_script"] = None
 
         model_script_dir = None
         if model_json["config"].get("script_dir"):
             model_script_dir = Input(type=AssetTypes.URI_FOLDER, path=model_json["config"]["script_dir"])
             model_json["config"]["script_dir"] = None
 
         model_path = None
-        if model_json["config"]["is_aml_model"] is True:
+        if model_json["config"]["model_storage_kind"] == ModelStorageKind.AzureMLModel:
             model_path = Input(
                 type=AssetTypes.CUSTOM_MODEL,
                 path=model_json["config"]["model_path"],
             )
-            model_json["config"]["is_aml_model"] = False
+            model_json["config"]["model_storage_kind"] = str(ModelStorageKind.LocalFile)
             model_json["config"]["version"] = None
         else:
             if model_json["config"].get("model_path"):
                 original_model_path = Path(model_json["config"]["model_path"]).resolve()
+                if (
+                    model_json["type"].lower() == "onnxmodel"
+                    and model_json["config"]["model_storage_kind"] == ModelStorageKind.LocalFolder
+                ):
+                    # onnx model with external data
+                    # need to upload the parent directory of .onnx file
+                    original_model_path = original_model_path.parent
+                # use common name "model" for model_path
                 tmp_model_path = (tmp_dir / "model").with_suffix(original_model_path.suffix)
-                tmp_model_path.symlink_to(original_model_path)
+                if original_model_path.is_dir():
+                    # copy model directory
+                    # symlink doesn't work for directory
+                    shutil.copytree(original_model_path, tmp_model_path, symlinks=True)
+                    if model_json["type"].lower() == "onnxmodel":
+                        # rename .onnx file to model.onnx
+                        onnx_model_file = Path(model_json["config"]["model_path"]).resolve().name
+                        (tmp_model_path / onnx_model_file).rename(tmp_model_path / "model.onnx")
+                else:
+                    # symlink model file
+                    tmp_model_path.symlink_to(original_model_path)
                 model_path = Input(
-                    type=AssetTypes.URI_FILE if model_json["config"].get("is_file") else AssetTypes.URI_FOLDER,
+                    type=AssetTypes.URI_FILE
+                    if model_json["config"].get("model_storage_kind") == ModelStorageKind.LocalFile
+                    else AssetTypes.URI_FOLDER,
                     path=tmp_model_path,
                 )
         model_json["config"]["model_path"] = None
 
         model_config_path = tmp_dir / "model_config.json"
-        json.dump(model_json, model_config_path.open("w"), sort_keys=True)
+        with model_config_path.open("w") as f:
+            json.dump(model_json, f, sort_keys=True)
         model_config = Input(type=AssetTypes.URI_FILE, path=model_config_path)
 
         return {
             "model_config": model_config,
             "model_path": model_path,
             "model_script": model_script,
             "model_script_dir": model_script_dir,
@@ -196,15 +202,16 @@
             pass_args[f"pass_{param}"] = Input(
                 type=AssetTypes.URI_FILE if Path(pass_config["config"][param]).is_file() else AssetTypes.URI_FOLDER,
                 path=pass_config["config"][param],
             )
             pass_config["config"][param] = None
 
         pass_config_path = tmp_dir / "pass_config.json"
-        json.dump(pass_config, pass_config_path.open("w"), sort_keys=True)
+        with pass_config_path.open("w") as f:
+            json.dump(pass_config, f, sort_keys=True)
 
         return {"pass_config": Input(type=AssetTypes.URI_FILE, path=pass_config_path), **pass_args}
 
     def _create_step(
         self, name, display_name, description, aml_environment, code, compute, instance_count, inputs, script_name
     ):
         parameters = []
@@ -253,15 +260,15 @@
                 "This mode is only enabled for CI pipeline! "
                 + "It will overwrite the Olive package in AML computer with latest code."
             )
             project_folder = cur_dir.parent.parent
             shutil.copytree(project_folder, code_root / "olive", ignore=shutil.ignore_patterns("__pycache__"))
 
         # prepare inputs
-        inputs = {**self._create_model_inputs(model.is_aml_model), **self._create_pass_inputs(pass_path_params)}
+        inputs = {**self._create_model_inputs(model.model_storage_kind), **self._create_pass_inputs(pass_path_params)}
 
         # pass type
         pass_type = pass_config["type"]
 
         # aml command object
         cmd = self._create_step(
             name=pass_type,
@@ -293,40 +300,63 @@
 
         pipeline_job = pass_runner_pipeline()
 
         return pipeline_job
 
     def _load_model(self, input_model, output_model_path, pipeline_output_path):
         model_json_path = pipeline_output_path / "output_model_config.json"
-        model_json = json.load(open(model_json_path, "r"))
+        with model_json_path.open("r") as f:
+            model_json = json.load(f)
 
         # resolve model path
         # this is to handle passes like OrtPerfTuning that use the same model file as input
         same_model_path_as_input = model_json.pop("same_model_path_as_input")
         model_path = None
         if same_model_path_as_input:
             model_path = input_model.model_path
             model_json["config"].update(
-                {"name": input_model.name, "version": input_model.version, "is_aml_model": input_model.is_aml_model}
+                {
+                    "name": input_model.name,
+                    "version": input_model.version,
+                    "model_storage_kind": input_model.model_storage_kind,
+                }
             )
         elif model_json["config"]["model_path"] is not None:
             downloaded_model_path = pipeline_output_path / model_json["config"]["model_path"]
-            if Path(output_model_path).suffix != Path(downloaded_model_path).suffix:
-                output_model_path += Path(downloaded_model_path).suffix
-            # TODO: handle cases where output_model_path is a directory
-            shutil.copy(downloaded_model_path, output_model_path)
+            if model_json["type"].lower() == "onnxmodel":
+                # onnx model can have external data
+                output_model_path = ONNXModel.resolve_path(output_model_path)
+                if model_json["config"]["model_storage_kind"] == ModelStorageKind.LocalFolder:
+                    # has external data
+                    # copy the .onnx file along with external data files
+                    shutil.copytree(downloaded_model_path.parent, Path(output_model_path).parent, dirs_exist_ok=True)
+                    # rename the .onnx file to the output_model_path, the downloaded model has "model.onnx" name
+                    (Path(output_model_path).parent / downloaded_model_path.name).rename(output_model_path)
+                else:
+                    # no external data
+                    # just copy over the .onnx file
+                    shutil.copy(downloaded_model_path, output_model_path)
+            else:
+                # handle other model types
+                if Path(output_model_path).suffix != Path(downloaded_model_path).suffix:
+                    output_model_path += Path(downloaded_model_path).suffix
+                if downloaded_model_path.is_file():
+                    # model is a file
+                    shutil.copy(downloaded_model_path, output_model_path)
+                else:
+                    # model is a directory
+                    shutil.copytree(downloaded_model_path, output_model_path, dirs_exist_ok=True)
             model_path = output_model_path
-            model_json["config"]["is_aml_model"] = False
         model_json["config"]["model_path"] = model_path
         return ModelConfig(**model_json).create_model()
 
     def _create_metric_inputs(self):
         return {
             "metric_config": Input(type=AssetTypes.URI_FILE),
-            "metric_user_script": Input(type=AssetTypes.URI_FILE),
+            "metric_user_script": Input(type=AssetTypes.URI_FILE, optional=True),
             "metric_script_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
             "metric_data_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
         }
 
     def _create_metric_args(self, metric_config: dict, tmp_dir: Path) -> Tuple[List[str], dict]:
         metric_config["name"] = "result"
         metric_config.pop("goal", None)
@@ -342,64 +372,66 @@
 
         metric_data_dir = metric_config["user_config"]["data_dir"]
         if metric_data_dir:
             metric_data_dir = Input(type=AssetTypes.URI_FOLDER, path=metric_data_dir)
             metric_config["user_config"]["data_dir"] = None
 
         metric_config_path = tmp_dir / "metric_config.json"
-        json.dump(metric_config, open(metric_config_path, "w"), sort_keys=True)
+        with metric_config_path.open("w") as f:
+            json.dump(metric_config, f, sort_keys=True)
         metric_config = Input(type=AssetTypes.URI_FILE, path=metric_config_path)
 
         return {
             "metric_config": metric_config,
             "metric_user_script": metric_user_script,
             "metric_script_dir": metric_script_dir,
             "metric_data_dir": metric_data_dir,
         }
 
     def evaluate_model(self, model: OliveModel, metrics: List[Metric]) -> Dict[str, Any]:
-
         if model.framework == Framework.SNPE:
             raise NotImplementedError("SNPE model does not support azureml evaluation")
         if model.framework == Framework.OPENVINO:
             raise NotImplementedError("OpenVINO model does not support azureml evaluation")
 
         with tempfile.TemporaryDirectory() as tempdir:
+            ml_client = self.azureml_client_config.create_client()
             pipeline_job = self._create_pipeline_for_evaluation(tempdir, model, metrics)
 
             # submit job
             logger.debug("Submitting pipeline")
             job = retry_func(
-                self.ml_client.jobs.create_or_update,
+                ml_client.jobs.create_or_update,
                 [pipeline_job],
                 {"experiment_name": "olive-evaluation"},
                 max_tries=3,
                 delay=5,
                 exceptions=HttpResponseError,
             )
             logger.info(f"Pipeline submitted. Job name: {job.name}. Job link: {job.studio_url}")
-            self.ml_client.jobs.stream(job.name)
+            ml_client.jobs.stream(job.name)
 
             # get output
             output_dir = Path(tempdir) / "pipeline_output"
             output_dir.mkdir(parents=True, exist_ok=True)
             retry_func(
-                self.ml_client.jobs.download,
+                ml_client.jobs.download,
                 [job.name],
                 {"download_path": output_dir, "all": True},
                 max_tries=3,
                 delay=5,
                 exceptions=ServiceResponseError,
             )
 
             metric_results = {}
             for metric in metrics:
                 metric_json = output_dir / "named-outputs" / metric.name / "metric_result.json"
                 if metric_json.is_file():
-                    metric_results[metric.name] = json.load(open(metric_json))["result"]
+                    with metric_json.open() as f:
+                        metric_results[metric.name] = json.load(f)["result"]
 
             return metric_results
 
     def _create_pipeline_for_evaluation(self, tmp_dir: str, model: OliveModel, metrics: List[Metric]):
         tmp_dir = Path(tmp_dir)
 
         # model json
@@ -409,24 +441,28 @@
         model_args = self._create_model_args(model_json, tmp_dir)
 
         @pipeline
         def evaluate_pipeline():
             outputs = {}
             for metric in metrics:
                 metric_tmp_dir = tmp_dir / metric.name
-                metric_component = self._create_metric_component(metric_tmp_dir, metric, model_args, model.is_aml_model)
+                metric_component = self._create_metric_component(
+                    metric_tmp_dir, metric, model_args, model.model_storage_kind
+                )
                 outputs[metric.name] = metric_component.outputs.pipeline_output
             return outputs
 
         pipeline_job = evaluate_pipeline()
         pipeline_job.settings.default_compute = self.compute
 
         return pipeline_job
 
-    def _create_metric_component(self, tmp_dir: Path, metric: Metric, model_args: Dict[str, Input], is_aml_model: bool):
+    def _create_metric_component(
+        self, tmp_dir: Path, metric: Metric, model_args: Dict[str, Input], model_storage_kind: ModelStorageKind
+    ):
         metric_json = metric.to_json(check_objects=True)
 
         # prepare code
         script_name = "aml_evaluation_runner.py"
         cur_dir = Path(__file__).resolve().parent
         code_file = cur_dir / script_name
         code_root = tmp_dir / "code"
@@ -437,15 +473,15 @@
                 "This mode is only enabled for CI pipeline! "
                 + "It will overwrite the Olive package in AML computer with latest code."
             )
             project_folder = cur_dir.parent.parent
             shutil.copytree(project_folder, code_root / "olive", ignore=shutil.ignore_patterns("__pycache__"))
 
         # prepare inputs
-        inputs = {**self._create_model_inputs(is_aml_model), **self._create_metric_inputs()}
+        inputs = {**self._create_model_inputs(model_storage_kind), **self._create_metric_inputs()}
 
         # metric type
         metric_type = metric_json["type"]
         if metric_json["sub_type"] is not None:
             metric_type = f"{metric_type}-{metric_json['sub_type']}"
 
         # aml command object
```

## olive/systems/docker/Dockerfile

```diff
@@ -8,13 +8,14 @@
             azure-identity \
             azureml-defaults \
             azureml-dataprep \
             onnxruntime \
             openvino \
             openvino-dev[tensorflow,onnx] \
             tensorflow \
-            olive-ai==0.1.0
+            onnxconverter_common \
+            olive-ai==0.2.0
 
 ADD requirements.txt requirements.txt
 RUN pip install -r requirements.txt
 
 WORKDIR /olive
```

## olive/systems/docker/docker_system.py

```diff
@@ -24,17 +24,18 @@
 
 
 class DockerSystem(OliveSystem):
     system_type = SystemType.Docker
 
     BASE_DOCKERFILE = "Dockerfile"
 
-    def __init__(self, local_docker_config: Union[Dict[str, Any], LocalDockerConfig]):
+    def __init__(self, local_docker_config: Union[Dict[str, Any], LocalDockerConfig], is_dev: bool = False):
         logger.info("Initializing Docker System...")
         local_docker_config = validate_config(local_docker_config, LocalDockerConfig)
+        self.is_dev = is_dev
         self.docker_client = docker.from_env()
         self.run_params = local_docker_config.run_params
         try:
             self.image = self.docker_client.images.get(local_docker_config.image_name)
             logger.info(f"Image {local_docker_config.image_name} found")
 
         except docker.errors.ImageNotFound:
@@ -75,15 +76,15 @@
         """
         Run the pass on the model at a specific point in the search space.
         """
         logger.warning("DockerSystem.run_pass is not implemented yet.")
         raise NotImplementedError()
 
     def evaluate_model(self, model: OliveModel, metrics: List[Metric]) -> Dict[str, Any]:
-        container_root_path = Path("/olive/")
+        container_root_path = Path("/olive-ws/")
         with tempfile.TemporaryDirectory() as tempdir:
             metrics_res = {}
             metric_json = self._run_container(tempdir, model, metrics, container_root_path)
             if metric_json.is_file():
                 with metric_json.open() as f:
                     metrics_res = json.load(f)
             return metrics_res
@@ -92,19 +93,25 @@
         eval_output_path = "eval_output"
         eval_output_name = "eval_res.json"
 
         volumes_list = []
         eval_file_mount_path, eval_file_mount_str = docker_utils.create_eval_script_mount(container_root_path)
         volumes_list.append(eval_file_mount_str)
 
+        if self.is_dev:
+            dev_mount_path, dev_mount_str = docker_utils.create_dev_mount(tempdir, container_root_path)
+            volumes_list.append(dev_mount_str)
+
         model_copy = copy.deepcopy(model)
-        model_mount_path, model_mount_str_list = docker_utils.create_model_mount(
-            model=model_copy, container_root_path=container_root_path
-        )
-        volumes_list += model_mount_str_list
+        model_mount_path = None
+        if model_copy.model_path:
+            model_mount_path, model_mount_str_list = docker_utils.create_model_mount(
+                model=model_copy, container_root_path=container_root_path
+            )
+            volumes_list += model_mount_str_list
 
         metrics_copy = copy.deepcopy(metrics)
         volumes_list = docker_utils.create_metric_volumes_list(
             metrics=metrics_copy,
             container_root_path=container_root_path,
             mount_list=volumes_list,
         )
@@ -127,13 +134,31 @@
             config_path=config_mount_path,
             output_path=output_mount_path,
             output_name=eval_output_name,
         )
 
         run_command = docker_utils.create_run_command(run_params=self.run_params)
 
-        logger.info(f"The volumes list is {volumes_list}")
-
-        self.docker_client.containers.run(image=self.image, command=eval_command, volumes=volumes_list, **run_command)
+        try:
+            logger.debug(f"Running container with eval command: {eval_command}")
+            logger.debug(f"The volumes list is {volumes_list}")
+            container = self.docker_client.containers.run(
+                image=self.image, command=eval_command, volumes=volumes_list, detach=True, **run_command
+            )
+            for line in container.logs(stream=True):
+                print(line.strip().decode())
+            logger.debug("Docker container evaluation completed successfully")
+        finally:
+            # clean up dev mount regardless of whether the run was successful or not
+            # otherwise __pycache__ will be created in the dev mount and will cause issues
+            if self.is_dev:
+                clean_up_mount_path, clean_up_mount_str = docker_utils.create_dev_cleanup_mount(container_root_path)
+                logger.debug("Cleaning up dev mount")
+                self.docker_client.containers.run(
+                    image=self.image,
+                    command=f"python {clean_up_mount_path} --dev_mount_path {dev_mount_path}",
+                    volumes=[dev_mount_str, clean_up_mount_str],
+                )
+                logger.debug("Dev mount cleaned up successfully")
 
         metric_json = Path(output_local_path) / f"{eval_output_name}"
         return metric_json
```

## olive/systems/docker/eval.py

```diff
@@ -4,40 +4,32 @@
 # --------------------------------------------------------------------------
 import argparse
 import json
 import logging
 import os
 import sys
 
-from olive.evaluator.evaluation import evaluate_accuracy, evaluate_custom_metric, evaluate_latency
-from olive.evaluator.metric import MetricList, MetricType
+from olive.evaluator.olive_evaluator import OliveEvaluator, OliveEvaluatorConfig, OliveEvaluatorFactory
 from olive.model import ModelConfig
 
-logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(module)s - %(levelname)s - %(message)s")
-logger = logging.getLogger()
+logger = logging.getLogger(__name__)
 
 
 def evaluate_entry(config, model_path, output_path, output_name):
     with open(config, "r") as f:
         config_json = json.load(f)
-    metric_list = MetricList(__root__=json.loads(config_json["metrics"])).__root__
-    logger.info(f"Evaluation metric list: {metric_list}")
-
+    evaluator_config = OliveEvaluatorConfig(metrics=config_json["metrics"])
     model_json = config_json["model"]
-    model_json["config"]["model_path"] = model_path
+
+    if model_path != "None":
+        model_json["config"]["model_path"] = model_path
     model = ModelConfig.from_json(model_json).create_model()
 
-    metrics_res = {}
-    for metric in metric_list:
-        if metric.name == MetricType.ACCURACY:
-            metrics_res[MetricType.ACCURACY] = evaluate_accuracy(model, metric)
-        elif metric.name == MetricType.LATENCY:
-            metrics_res[MetricType.LATENCY] = evaluate_latency(model, metric)
-        else:
-            metrics_res[metric.name] = evaluate_custom_metric(model, metric)
+    evaluator: OliveEvaluator = OliveEvaluatorFactory.create_evaluator_for_model(model)
+    metrics_res = evaluator.evaluate(model, evaluator_config.metrics)
 
     with open(os.path.join(output_path, f"{output_name}"), "w") as f:
         json.dump(metrics_res, f)
     logger.info(f"Metric result: {metrics_res}")
 
 
 if __name__ == "__main__":
```

## olive/systems/docker/utils.py

```diff
@@ -1,29 +1,29 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import json
 import logging
+import shutil
 from pathlib import Path
 from typing import List
 
 from olive.constants import Framework
-from olive.evaluator.metric import Metric, MetricList
+from olive.evaluator.metric import Metric
 from olive.model import OliveModel
 
 logger = logging.getLogger(__name__)
 
 
 def create_config_file(tempdir, model: OliveModel, metrics: List[Metric], container_root_path: Path):
     model_json = model.to_json(check_object=True)
 
     config_file_path = Path(tempdir) / "config.json"
-    metric_json_list = MetricList(__root__=metrics).json()
-    data = {"metrics": metric_json_list, "model": model_json}
+    data = {"metrics": [k.dict() for k in metrics], "model": model_json}
 
     # the config yaml file saved to local disk
     with config_file_path.open("w") as f:
         json.dump(data, f)
     config_mount_path = str(container_root_path / "config.json")
     config_file_mount_str = f"{config_file_path}:{config_mount_path}"
     return config_mount_path, config_file_mount_str
@@ -76,15 +76,15 @@
             metric.user_config.data_dir = str(metric_path / "data_dir")
 
     return mount_list
 
 
 def create_model_mount(model: OliveModel, container_root_path: Path):
     model_mount_path = str(container_root_path / Path(model.model_path).name)
-    model_mount_str = f"{model.model_path}:{model_mount_path}"
+    model_mount_str = f"{str(Path(model.model_path).resolve())}:{model_mount_path}"
     model.model_path = model_mount_path
     model_mount_str_list = [model_mount_str]
 
     if model.framework == Framework.PYTORCH:
         if model.script_dir:
             script_dir_mount = f"{model.script_dir}:{container_root_path}"
             model.script_dir = container_root_path
@@ -95,13 +95,36 @@
 def create_eval_script_mount(container_root_path: Path):
     eval_file_mount_path = str(container_root_path / "eval.py")
     current_dir = Path(__file__).resolve().parent
     eval_file_mount_str = f"{str(current_dir / 'eval.py')}:{eval_file_mount_path}"
     return eval_file_mount_path, eval_file_mount_str
 
 
+def create_dev_mount(tempdir: Path, container_root_path: Path):
+    logger.warning(
+        "This mode is only enabled for CI pipeline! "
+        + "It will overwrite the Olive package in docker container with latest code."
+    )
+    tempdir = Path(tempdir)
+
+    # copy the whole project folder to tempdir
+    project_folder = Path(__file__).resolve().parent.parent.parent
+    shutil.copytree(project_folder, tempdir / "olive", ignore=shutil.ignore_patterns("__pycache__"))
+
+    project_folder_mount_path = str(container_root_path / "olive")
+    project_folder_mount_str = f"{tempdir / 'olive'}:{project_folder_mount_path}"
+    return project_folder_mount_path, project_folder_mount_str
+
+
+def create_dev_cleanup_mount(container_root_path: Path):
+    mount_path = str(container_root_path / "dev_mount_cleanup.py")
+    current_dir = Path(__file__).resolve().parent
+    mount_str = f"{str(current_dir / 'dev_mount_cleanup.py')}:{mount_path}"
+    return mount_path, mount_str
+
+
 def create_output_mount(tempdir, docker_eval_output_path: str, container_root_path: Path):
     output_local_path = Path(tempdir) / docker_eval_output_path
     output_local_path.mkdir(parents=True, exist_ok=True)
     output_mount_path = str(container_root_path / docker_eval_output_path)
     output_mount_str = f"{output_local_path}:{output_mount_path}"
     return output_local_path, output_mount_path, output_mount_str
```

## olive/workflows/run/__main__.py

```diff
@@ -5,11 +5,12 @@
 import argparse
 
 from olive.workflows import run
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser("Olive Workflow: Custom Run")
     parser.add_argument("--config", type=str, help="Path to json config file", required=True)
+    parser.add_argument("--setup", help="Whether run environment setup", action="store_true")
 
     args = parser.parse_args()
 
     run(**vars(args))
```

## olive/workflows/run/config.py

```diff
@@ -1,84 +1,180 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from typing import Dict
+from pathlib import Path
+from typing import Dict, Union
 
 from pydantic import validator
 
-from olive.common.config_utils import ConfigBase
-from olive.engine import EngineConfig
+from olive.azureml.azureml_client import AzureMLClientConfig
+from olive.common.config_utils import ConfigBase, validate_config
+from olive.data.config import DataConfig
+from olive.data.constants import DEFAULT_HF_DATA_CONTAINER_NAME, DefaultDataContainer
+from olive.data.container.huggingface_container import HuggingfaceContainer
+from olive.engine import Engine, EngineConfig
+from olive.engine.packaging.packaging_config import PackagingConfig
 from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
 from olive.model import ModelConfig
-from olive.passes import FullPassConfig
+from olive.passes import FullPassConfig, Pass
 from olive.systems.system_config import SystemConfig
 
 
 class RunPassConfig(FullPassConfig):
     host: SystemConfig = None
     evaluator: OliveEvaluatorConfig = None
     clean_run_cache: bool = False
 
 
+class RunEngineConfig(EngineConfig):
+    evaluation_only: bool = False
+    output_dir: Union[Path, str] = None
+    output_name: str = None
+    packaging_config: PackagingConfig = None
+    log_severity_level: int = 1
+    ort_log_severity_level: int = 3
+
+    def create_engine(self):
+        config = self.dict()
+        to_del = [
+            "evaluation_only",
+            "output_dir",
+            "output_name",
+            "packaging_config",
+            "log_severity_level",
+            "ort_log_severity_level",
+        ]
+        for key in to_del:
+            del config[key]
+        return Engine(config)
+
+
 class RunConfig(ConfigBase):
     verbose: bool = False
+    azureml_client: AzureMLClientConfig = None
     input_model: ModelConfig
     systems: Dict[str, SystemConfig] = None
+    data_config: Dict[str, DataConfig] = {
+        DefaultDataContainer.DATA_CONTAINER.value: DataConfig(),
+        DEFAULT_HF_DATA_CONTAINER_NAME: DataConfig(
+            name=DEFAULT_HF_DATA_CONTAINER_NAME,
+            type=HuggingfaceContainer.__name__,
+        ),
+    }
     evaluators: Dict[str, OliveEvaluatorConfig] = None
+    engine: RunEngineConfig
     passes: Dict[str, RunPassConfig]
-    engine: EngineConfig
+
+    @validator("data_config", pre=True, each_item=True, always=True)
+    def validate_data_config(cls, v, values):
+        hf_config = values["input_model"].dict()["config"].get("hf_config", {})
+
+        if isinstance(v, DataConfig):
+            # clean up default components before config validation
+            v.components = None if hf_config.get("dataset", None) else v.components
+            v = v.dict()
+
+        if v["type"] == HuggingfaceContainer.__name__:
+            if hf_config:
+                v["params_config"]["model_name"] = hf_config.get("model_name", None)
+                v["params_config"]["task"] = hf_config.get("task", None)
+                v["params_config"].update(hf_config.get("dataset", {}))
+        return validate_config(v, DataConfig)
 
     @validator("evaluators", pre=True, each_item=True)
     def validate_evaluators(cls, v, values):
-        return _resolve_system(v, values, "target")
+        v = _resolve_system(v, values, "target")
+        for idx, metric in enumerate(v.get("metrics", [])):
+            v["metrics"][idx] = _resolve_data_config(metric, values, "data_config")
+        return v
 
-    @validator("passes", pre=True, each_item=True)
-    def validate_passes(cls, v, values):
+    @validator("engine", pre=True)
+    def validate_engine(cls, v, values):
         v = _resolve_system(v, values, "host")
+        v = _resolve_system(v, values, "target")
         return _resolve_evaluator(v, values)
 
-    @validator("engine", pre=True)
-    def validate_engine(cls, v, values):
-        search_strategy = None
-        if isinstance(v, dict):
-            search_strategy = v.get("search_strategy")
-        elif isinstance(v, EngineConfig):
-            search_strategy = v.search_strategy
-        if search_strategy is None:
-            raise ValueError("search_strategy must be specified in engine config")
+    @validator("engine")
+    def validate_evaluation_only(cls, v):
+        if v.evaluation_only and v.evaluator is None:
+            raise ValueError("Evaluation only requires evaluator")
+        return v
+
+    @validator("passes", pre=True, each_item=True)
+    def validate_pass_host_evaluator(cls, v, values):
         v = _resolve_system(v, values, "host")
         return _resolve_evaluator(v, values)
 
+    @validator("passes", pre=True, each_item=True)
+    def validate_pass_search(cls, v, values):
+        if "engine" not in values:
+            raise ValueError("Invalid engine")
+
+        if not values["engine"].search_strategy:
+            # disable search if search_strategy is None/False/{}, user cannot override
+            disable_search = True
+        else:
+            # disable search if user explicitly set disable_search to True
+            disable_search = v.get("disable_search", False)
+
+        v["disable_search"] = disable_search
+        pass_cls = Pass.registry.get(v["type"].lower(), None)
+        if pass_cls and pass_cls.requires_data_config():
+            v["config"] = _resolve_data_config(v.get("config", {}), values, "data_config")
+        return v
+
 
-def _resolve_system(v, values, system_alias):
+def _resolve_config_str(v, values, alias, component_name):
     if not isinstance(v, dict):
         return v
 
-    system = v.get(system_alias)
-    if not isinstance(system, str):
+    sub_component = v.get(alias)
+    if not isinstance(sub_component, str):
         return v
 
-    # resolve system name to systems member config
-    if "systems" not in values:
-        raise ValueError("Invalid systems")
-    systems = values["systems"] or {}
-    if system not in systems:
-        raise ValueError(f"{system_alias} {system} not found in systems")
-    v[system_alias] = systems[system]
+    # resolve component name to component config
+    if component_name not in values:
+        raise ValueError(f"Invalid {component_name}")
+    components = values[component_name] or {}
+    if sub_component not in components:
+        raise ValueError(f"{alias} {sub_component} not found in {components}")
+    v[alias] = components[sub_component]
     return v
 
 
+def _resolve_system(v, values, system_alias, component_name="systems"):
+    v = _resolve_config_str(v, values, system_alias, component_name=component_name)
+    if system_alias in v:
+        v[system_alias] = validate_config(v[system_alias], SystemConfig)
+        if v[system_alias].type == "AzureML":
+            if not values["azureml_client"]:
+                raise ValueError("AzureML client config is required for AzureML system")
+            v[system_alias].config.azureml_client_config = values["azureml_client"]
+    return v
+
+
+def _resolve_data_config(v, values, system_alias, component_name="data_config"):
+    data_container_config = v.get("data_config", None)
+    hf_data_config = values["input_model"].dict()["config"].get("hf_config", {}).get("dataset", None)
+    if not data_container_config and hf_data_config:
+        # if data_container is None, we need to update the config to use HuggingfaceContainer
+        v["data_config"] = DEFAULT_HF_DATA_CONTAINER_NAME
+    return _resolve_config_str(v, values, system_alias, component_name=component_name)
+
+
 def _resolve_evaluator(v, values):
     if not isinstance(v, dict):
         return v
 
     evaluator = v.get("evaluator")
     if isinstance(evaluator, dict):
         v["evaluator"] = _resolve_system(evaluator, values, "target")
+        for metrics in v["evaluator"].get("metrics", []):
+            metrics = _resolve_data_config(metrics, values, "data_config")
         return v
     elif not isinstance(evaluator, str):
         return v
 
     # resolve evaluator name to evaluators member config
     if "evaluators" not in values:
         raise ValueError("Invalid evaluators")
```

## olive/workflows/run/run.py

```diff
@@ -1,73 +1,164 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import json
 import logging
+import os
+import subprocess
 from pathlib import Path
 from typing import Union
 
-from olive.engine import Engine
+import onnxruntime as ort
+
+from olive import set_default_logger_severity
+from olive.passes import Pass
+from olive.systems.common import Device, SystemType
 from olive.workflows.run.config import RunConfig
 
 logger = logging.getLogger(__name__)
 
 
-def automatically_insert_passes(engine, config):
+def automatically_insert_passes(config):
     new_config_dict = json.loads(config.json())
     new_passes = {}
 
-    # insert onnx coverter
+    # insert onnx converter
     oc_config = {"type": "OnnxConversion"}
-    oc_config["config"] = config.engine.model_io_config
     new_passes["conversion"] = oc_config
 
     # insert transformer opt
-    to_config = {"type": "OnnxTransformersOptimization"}
+    to_config = {"type": "OrtTransformersOptimization"}
     to_config["config"] = {"model_type": "bert"}
     new_passes["transformers_optimization"] = to_config
 
     # insert quantization
     q_config = {"type": "OnnxDynamicQuantization"}
-    q_config["config"] = {"per_channel": "DEFAULT_SEARCH", "reduce_range": "DEFAULT_SEARCH"}
+    q_config["config"] = {"per_channel": "SEARCHABLE_VALUES", "reduce_range": "SEARCHABLE_VALUES"}
     q_config["clean_run_cache"] = False
     new_passes["dynamic_quantization"] = q_config
 
-    # insert thread_tuning
-    t_config = {"type": "OnnxThreadTuning"}
+    # insert perf_tuning
+    t_config = {"type": "OrtPerfTuning"}
     t_config["config"] = {"user_script": "user_script.py", "dataloader_func": "create_dataloader", "batch_size": 1}
-    new_passes["thread_tuning"] = t_config
+    new_passes["perf_tuning"] = t_config
 
     new_config_dict["passes"] = new_passes
     new_config = RunConfig.parse_obj(new_config_dict)
-    new_engine = Engine(new_config.engine)
+    new_engine = new_config.engine.create_engine()
 
     return new_engine, new_config
 
 
-def run(config: Union[str, Path, dict]):
+def dependency_setup(config):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with open(os.path.join(here, "../../extra_dependencies.json"), "r") as f:
+        EXTRAS = json.load(f)
+    DEPENDENCY_MAPPING = {
+        "device": {
+            SystemType.AzureML: EXTRAS.get("azureml"),
+            SystemType.Docker: EXTRAS.get("docker"),
+            SystemType.Local: {Device.CPU: EXTRAS.get("cpu"), Device.GPU: EXTRAS.get("gpu")},
+        },
+        "pass": {
+            "OnnxFloatToFloat16": ["onnxconverter-common"],
+            "OrtPerfTuning": ["psutil"],
+            "QuantizationAwareTraining": ["pytorch-lightning"],
+            "OpenVINOConversion": EXTRAS.get("openvino"),
+            "OpenVINOQuantization": EXTRAS.get("openvino"),
+            "IncQuantization": EXTRAS.get("inc"),
+            "IncDynamicQuantization": EXTRAS.get("inc"),
+            "IncStaticQuantization": EXTRAS.get("inc"),
+        },
+    }
+
+    local_packages = []
+    remote_packages = []
+
+    # add dependencies for passes
+    for _, pass_config in config.passes.items():
+        host = pass_config.host or config.engine.host
+        if (host and host.type == SystemType.Local) or not host:
+            local_packages.extend(DEPENDENCY_MAPPING["pass"].get(pass_config.type, []))
+        else:
+            remote_packages.extend(DEPENDENCY_MAPPING["pass"].get(pass_config.type, []))
+        if pass_config.type in ["SNPEConversion", "SNPEQuantization", "SNPEtoONNXConversion"]:
+            logger.info(
+                "Please refer to https://microsoft.github.io/Olive/tutorials/passes/snpe.html                 to"
+                " install SNPE Prerequisites for pass {}".format(pass_config.type)
+            )
+
+    # add dependencies for engine
+    if config.engine.host and config.engine.host.type == SystemType.Local:
+        local_packages.extend(DEPENDENCY_MAPPING["device"][SystemType.Local][config.engine.host.config.device])
+    elif not config.engine.host:
+        local_packages.extend(DEPENDENCY_MAPPING["device"][SystemType.Local]["cpu"])
+    else:
+        local_packages.extend(DEPENDENCY_MAPPING["device"][config.engine.host.type])
+
+    # install packages to local or tell user to install packages in their environment
+    logger.info("The following packages will be installed: {}".format(" ".join(local_packages)))
+    for package in set(local_packages):
+        try:
+            __import__(package)
+        except ImportError:
+            subprocess.check_call(["python", "-m", "pip", "install", "{}".format(package)])
+    if remote_packages:
+        logger.info(
+            "Please make sure the following packages are installed in {} environment: {}".format(
+                config.engine.host.type, remote_packages
+            )
+        )
+
+
+def run(config: Union[str, Path, dict], setup: bool = False):
     # we use parse_file and parse_obj to be safe. If implemented as expected, both should be equivalent.
     if isinstance(config, str) or isinstance(config, Path):
         config = RunConfig.parse_file(config)
     else:
         config = RunConfig.parse_obj(config)
 
+    # set ort log level
+    set_default_logger_severity(config.engine.log_severity_level)
+    ort.set_default_logger_severity(config.engine.ort_log_severity_level)
+
     # input model
     input_model = config.input_model.create_model()
 
+    # Azure ML Client
+    if config.azureml_client:
+        config.engine.azureml_client_config = config.azureml_client
+
     # engine
-    engine = Engine(config.engine)
+    engine = config.engine.create_engine()
 
-    if config.passes is None or not config.passes:
-        engine, config = automatically_insert_passes(engine, config)
-    # passes
-    for pass_name, pass_config in config.passes.items():
-        p = pass_config.create_pass()
-        host = pass_config.host.create_system() if pass_config.host is not None else None
-        evaluator = pass_config.evaluator.create_evaluator() if pass_config.evaluator is not None else None
-        engine.register(p, pass_name, host, evaluator, pass_config.clean_run_cache)
-
-    # run
-    best_execution = engine.run(input_model, config.verbose)
-    logger.info(best_execution)
-    return best_execution
+    if (config.passes is None or not config.passes) and (not config.engine.evaluation_only):
+        # TODO enhance this logic for more passes templates
+        engine, config = automatically_insert_passes(config)
+
+    if setup:
+        dependency_setup(config)
+    else:
+        # passes
+        for pass_name, pass_config in config.passes.items():
+            host = pass_config.host.create_system() if pass_config.host is not None else None
+            engine.register(
+                Pass.registry[pass_config.type.lower()],
+                config=pass_config.config,
+                disable_search=pass_config.disable_search,
+                name=pass_name,
+                host=host,
+                evaluator_config=pass_config.evaluator,
+                clean_run_cache=pass_config.clean_run_cache,
+            )
+
+        # run
+        best_execution = engine.run(
+            input_model,
+            config.engine.packaging_config,
+            config.verbose,
+            config.engine.output_dir,
+            config.engine.output_name,
+            config.engine.evaluation_only,
+        )
+        return best_execution
```

## olive/workflows/snpe/convertquantize/convertquantize.py

```diff
@@ -5,14 +5,15 @@
 import json
 import logging
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from olive.model import ONNXModel, TensorFlowModel
 from olive.passes import SNPEConversion, SNPEQuantization, SNPEtoONNXConversion
+from olive.passes.olive_pass import create_pass_from_dict
 from olive.snpe import SNPEDevice, SNPEProcessedDataLoader
 
 logger = logging.getLogger(__name__)
 
 
 def convertquantize(
     model: str,
@@ -32,15 +33,16 @@
         output_dir (str, optional): Path to the output directory. Optional if it is the same as model directory.
         output_name (str, optional): Name of the output model (without extension). Optional if same as model name.
     """
     models_dir = Path(model).resolve().parent if output_dir is None else Path(output_dir).resolve()
     data_dir = Path(data).resolve()
     name = Path(model).resolve().stem if output_name is None else output_name
     if type(config) is str:
-        config = json.load(open(Path(config).resolve()))
+        with open(Path(config).resolve()) as f:
+            config = json.load(f)
 
     # ------------------------------------------------------------------
     model_file = Path(model).resolve()
     if model_file.suffix == ".onnx":
         logger.info("Loading model...")
         model = ONNXModel(model_file, name)
     elif model_file.suffix == ".pb":
@@ -50,39 +52,47 @@
         raise Exception(f"Unsupported model format: {model_file.suffix}")
 
     # ------------------------------------------------------------------
     # SNPE model
     logger.info("Converting model to SNPE...")
     snpe_model_file = str(models_dir / f"{name}.dlc")
 
-    snpe_conversion = SNPEConversion({**config["io_config"], **config["convert_options"]})
+    snpe_conversion = create_pass_from_dict(
+        SNPEConversion, {**config["io_config"], **config["convert_options"]}, disable_search=True
+    )
     snpe_model = snpe_conversion.run(model, snpe_model_file)
     assert Path(snpe_model.model_path).is_file()
-    json.dump(snpe_model.io_config, open(str(models_dir / f"{name}.dlc_io_config.json"), "w"))
+    with open(str(models_dir / f"{name}.dlc_io_config.json"), "w") as f:
+        json.dump(snpe_model.io_config, f)
 
     # ------------------------------------------------------------------
     # SNPE Quantized model
     logger.info("Quantizing SNPE model...")
     snpe_quantized_model_file = str(models_dir / f"{name}.quant.dlc")
     dataloader_func = lambda data_dir: SNPEProcessedDataLoader(data_dir, input_list_file=input_list_file)  # noqa: E731
 
-    snpe_quantization = SNPEQuantization(
-        {"data_dir": str(data_dir), "dataloader_func": dataloader_func, **config["quantize_options"]}
+    snpe_quantization = create_pass_from_dict(
+        SNPEQuantization,
+        {"data_dir": str(data_dir), "dataloader_func": dataloader_func, **config["quantize_options"]},
+        disable_search=True,
     )
     snpe_quantized_model = snpe_quantization.run(snpe_model, snpe_quantized_model_file)
     assert Path(snpe_quantized_model.model_path).is_file()
-    json.dump(snpe_quantized_model.io_config, open(str(models_dir / f"{name}.quant.dlc_io_config.json"), "w"))
+    with open(str(models_dir / f"{name}.quant.dlc_io_config.json"), "w") as f:
+        json.dump(snpe_quantized_model.io_config, f)
 
     # ------------------------------------------------------------------
     # SNPE Quantized ONNX model
     save_to_onnx = config.get("save_to_onnx", False)
     if not save_to_onnx:
         return
 
     logger.info("Converting SNPE Quantized model to ONNX...")
     snpe_quantized_onnx_model_file = str(models_dir / f"{name}.quant.onnx")
 
-    snpe_to_onnx_conversion = SNPEtoONNXConversion(
-        {"target_device": config["quantize_options"].get("target_device", SNPEDevice.CPU)}
+    snpe_to_onnx_conversion = create_pass_from_dict(
+        SNPEtoONNXConversion,
+        {"target_device": config["quantize_options"].get("target_device", SNPEDevice.CPU)},
+        disable_search=True,
     )
     snpe_quantized_onnx_model = snpe_to_onnx_conversion.run(snpe_quantized_model, snpe_quantized_onnx_model_file)
     assert Path(snpe_quantized_onnx_model.model_path).is_file()
```

## olive/workflows/snpe/evaluate/evaluate.py

```diff
@@ -25,15 +25,16 @@
         config (str): Either the path of json config file or an already loaded json file as a `dict`.
         data (str): Path to the evaluation data.
         input_list_file (str, optional): Name of input list file. Optional if it is 'input_list.txt'.
     """
     data_dir = Path(data).resolve()
     name = Path(model).resolve().stem
     if type(config) is str:
-        config = json.load(open(Path(config).resolve()))
+        with open(Path(config).resolve()) as f:
+            config = json.load(f)
 
     # SNPE Model
     model = SNPEModel(model_path=model, name=name, **config["io_config"])
 
     # Devices to evaluate on
     devices = [Device.CPU]
     if get_snpe_target_arch() == "ARM64-Windows":
```

## test/integ_test/evaluator/azureml_eval/test_aml_evaluation.py

```diff
@@ -12,16 +12,15 @@
     get_latency_metric,
     get_onnx_model,
     get_pytorch_model,
 )
 
 import pytest
 
-from olive.evaluator.olive_evaluator import OliveEvaluator
-from olive.model import ONNXModel, PyTorchModel
+from olive.model import ModelStorageKind, ONNXModel, PyTorchModel
 
 
 class TestAMLEvaluation:
     @pytest.fixture(scope="class", autouse=True)
     def setup(self):
         get_directories()
         download_models()
@@ -38,11 +37,10 @@
 
     @pytest.mark.parametrize(
         "model_cls,model_path,metric,expected_res",
         EVALUATION_TEST_CASE,
     )
     def test_evaluate_model(self, model_cls, model_path, metric, expected_res):
         aml_target = get_aml_target()
-        olive_model = model_cls(model_path=model_path, is_file=True)
-        evaluator = OliveEvaluator(metrics=[metric], target=aml_target)
-        actual_res = evaluator.evaluate(olive_model)[metric.name]
+        olive_model = model_cls(model_path=model_path, model_storage_kind=ModelStorageKind.LocalFile)
+        actual_res = aml_target.evaluate_model(olive_model, [metric])[metric.name]
         assert actual_res >= expected_res
```

## test/integ_test/evaluator/azureml_eval/utils.py

```diff
@@ -7,14 +7,15 @@
 import shutil
 from pathlib import Path
 
 from azure.storage.blob import BlobClient
 from torchvision import datasets
 from torchvision.transforms import ToTensor
 
+from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.evaluator.metric import AccuracySubType, LatencySubType, Metric, MetricType
 from olive.systems.azureml import AzureMLDockerConfig, AzureMLSystem
 
 
 def get_directories():
     current_dir = Path(__file__).resolve().parent
 
@@ -110,20 +111,24 @@
 
 def get_aml_target():
     aml_compute = "cpu-cluster"
     current_path = Path(__file__).absolute().parent
     conda_file_location = current_path / "conda.yaml"
     config_file_location = current_path / "olive-workspace-config.json"
     generate_olive_workspace_config(config_file_location)
+    azureml_client_config = AzureMLClientConfig(aml_config_path=str(config_file_location))
     docker_config = AzureMLDockerConfig(
         base_image="mcr.microsoft.com/azureml/openmpi4.1.0-ubuntu20.04",
         conda_file_path=conda_file_location,
     )
     return AzureMLSystem(
-        aml_config_path=config_file_location, aml_compute=aml_compute, aml_docker_config=docker_config, is_dev=True
+        azureml_client_config=azureml_client_config,
+        aml_compute=aml_compute,
+        aml_docker_config=docker_config,
+        is_dev=True,
     )
 
 
 def generate_olive_workspace_config(workspace_config_path):
     subscription_id = os.environ.get("WORKSPACE_SUBSCRIPTION_ID")
     if subscription_id is None:
         raise Exception("Please set the environment variable WORKSPACE_SUBSCRIPTION_ID")
```

## test/integ_test/evaluator/docker_eval/test_docker_evaluation.py

```diff
@@ -6,23 +6,23 @@
 from test.integ_test.evaluator.docker_eval.utils import (
     delete_directories,
     download_data,
     download_models,
     get_accuracy_metric,
     get_directories,
     get_docker_target,
+    get_huggingface_model,
     get_latency_metric,
     get_onnx_model,
     get_openvino_model,
     get_pytorch_model,
 )
 
 import pytest
 
-from olive.evaluator.olive_evaluator import OliveEvaluator
 from olive.model import ONNXModel, OpenVINOModel, PyTorchModel
 
 
 class TestDockerEvaluation:
     @pytest.fixture(scope="class", autouse=True)
     def setup(self):
         get_directories()
@@ -30,24 +30,25 @@
         download_data()
         yield
         delete_directories()
 
     EVALUATION_TEST_CASE = [
         (PyTorchModel, get_pytorch_model(), get_accuracy_metric("post_process"), 0.99),
         (PyTorchModel, get_pytorch_model(), get_latency_metric(), 0.001),
+        (PyTorchModel, get_huggingface_model(), get_accuracy_metric("hf_post_process", "create_hf_dataloader"), 0.1),
+        (PyTorchModel, get_huggingface_model(), get_latency_metric("create_hf_dataloader"), 0.001),
         (ONNXModel, get_onnx_model(), get_accuracy_metric("post_process"), 0.99),
         (ONNXModel, get_onnx_model(), get_latency_metric(), 0.001),
         (OpenVINOModel, get_openvino_model(), get_accuracy_metric("openvino_post_process"), 0.99),
         (OpenVINOModel, get_openvino_model(), get_latency_metric(), 0.001),
     ]
 
     @pytest.mark.parametrize(
-        "model_cls,model_path,metric,expected_res",
+        "model_cls,model_config,metric,expected_res",
         EVALUATION_TEST_CASE,
     )
     @pytest.mark.skipif(platform.system() == "Windows", reason="Docker target does not support windows")
-    def test_evaluate_model(self, model_cls, model_path, metric, expected_res):
+    def test_evaluate_model(self, model_cls, model_config, metric, expected_res):
         docker_target = get_docker_target()
-        olive_model = model_cls(model_path=model_path)
-        evaluator = OliveEvaluator(metrics=[metric], target=docker_target)
-        actual_res = evaluator.evaluate(olive_model)[metric.name]
+        olive_model = model_cls(**model_config)
+        actual_res = docker_target.evaluate_model(olive_model, [metric])[metric.name]
         assert actual_res >= expected_res
```

## test/integ_test/evaluator/docker_eval/user_script.py

```diff
@@ -15,7 +15,45 @@
     dataset = datasets.MNIST(data_dir, transform=ToTensor())
     return torch.utils.data.DataLoader(dataset, batch_size)
 
 
 def openvino_post_process(res):
     res = list(res.values())[0]
     return res.argmax(1)
+
+
+def hf_post_process(res):
+    _, preds = torch.max(res[0], dim=1)
+    return preds
+
+
+def create_hf_dataloader(data_dir, batch_size):
+    from datasets import load_dataset
+    from torch.utils.data import Dataset
+    from transformers import AutoTokenizer
+
+    tokenizer = AutoTokenizer.from_pretrained("prajjwal1/bert-tiny")
+    dataset = load_dataset("glue", "mrpc", split="validation")
+
+    class BaseData(Dataset):
+        def __init__(self, data):
+            self.data = data
+
+        def __len__(self):
+            return 10
+
+        def __getitem__(self, idx):
+            data = {k: v for k, v in self.data[idx].items() if k != "label"}
+            return data, self.data[idx]["label"]
+
+    def _map(examples):
+        t_input = tokenizer(examples["sentence1"], examples["sentence2"], truncation=True, padding=True)
+        t_input["label"] = examples["label"]
+        return t_input
+
+    dataset = dataset.map(
+        _map,
+        batched=True,
+        remove_columns=dataset.column_names,
+    )
+    dataset.set_format(type="torch", output_all_columns=True)
+    return torch.utils.data.DataLoader(BaseData(dataset), batch_size)
```

## test/integ_test/evaluator/docker_eval/utils.py

```diff
@@ -27,35 +27,35 @@
     return current_dir, models_dir, data_dir
 
 
 current_dir, models_dir, data_dir = get_directories()
 user_script = str(current_dir / "user_script.py")
 
 
-def get_accuracy_metric(post_process):
+def get_accuracy_metric(post_process, dataloader_func="create_dataloader"):
     accuracy_metric_config = {
         "user_script": user_script,
         "post_processing_func": post_process,
         "data_dir": data_dir,
-        "dataloader_func": "create_dataloader",
+        "dataloader_func": dataloader_func,
     }
     accuracy_metric = Metric(
         name="accuracy",
         type=MetricType.ACCURACY,
         sub_type=AccuracySubType.ACCURACY_SCORE,
         user_config=accuracy_metric_config,
     )
     return accuracy_metric
 
 
-def get_latency_metric():
+def get_latency_metric(dataloader_func="create_dataloader"):
     latency_metric_config = {
         "user_script": user_script,
         "data_dir": data_dir,
-        "dataloader_func": "create_dataloader",
+        "dataloader_func": dataloader_func,
     }
     latency_metric = Metric(
         name="latency",
         type=MetricType.LATENCY,
         sub_type=LatencySubType.AVG,
         user_config=latency_metric_config,
     )
@@ -89,24 +89,28 @@
     return str(models_dir / "openvino")
 
 
 def download_data():
     datasets.MNIST(data_dir, download=True, transform=ToTensor())
 
 
+def get_huggingface_model():
+    return {"hf_config": {"model_class": "AutoModelForSequenceClassification", "model_name": "prajjwal1/bert-tiny"}}
+
+
 def get_pytorch_model():
-    return str(models_dir / "model.pt")
+    return {"model_path": str(models_dir / "model.pt")}
 
 
 def get_onnx_model():
-    return str(models_dir / "model.onnx")
+    return {"model_path": str(models_dir / "model.onnx")}
 
 
 def get_openvino_model():
-    return str(models_dir / "openvino")
+    return {"model_path": str(models_dir / "openvino")}
 
 
 def download_azure_blob(container, blob, download_path):
     try:
         conn_str = os.environ["OLIVEWHEELS_STORAGE_CONNECTION_STRING"]
     except KeyError:
         raise Exception("Please set the environment variable OLIVEWHEELS_STORAGE_CONNECTION_STRING")
@@ -125,8 +129,8 @@
 
 def get_docker_target():
     local_docker_config = LocalDockerConfig(
         image_name="olive",
         build_context_path=str(current_dir / "dockerfile"),
         dockerfile="Dockerfile",
     )
-    return DockerSystem(local_docker_config=local_docker_config)
+    return DockerSystem(local_docker_config=local_docker_config, is_dev=True)
```

## test/integ_test/evaluator/local_eval/test_local_evaluation.py

```diff
@@ -2,46 +2,50 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from test.integ_test.evaluator.local_eval.utils import (
     delete_directories,
     get_accuracy_metric,
     get_directories,
+    get_hf_accuracy_metric,
+    get_hf_latency_metric,
+    get_huggingface_model,
     get_latency_metric,
     get_onnx_model,
     get_openvino_model,
     get_pytorch_model,
     openvino_post_process,
     post_process,
 )
 
 import pytest
 
-from olive.evaluator.olive_evaluator import OliveEvaluator
 from olive.model import ONNXModel, OpenVINOModel, PyTorchModel
+from olive.systems.local import LocalSystem
 
 
 class TestLocalEvaluation:
     @pytest.fixture(scope="class", autouse=True)
     def setup(self):
         get_directories()
         yield
         delete_directories()
 
     EVALUATION_TEST_CASE = [
         (PyTorchModel, get_pytorch_model(), get_accuracy_metric(post_process), 0.99),
         (PyTorchModel, get_pytorch_model(), get_latency_metric(), 0.001),
+        (PyTorchModel, get_huggingface_model(), get_hf_accuracy_metric(), 0.1),
+        (PyTorchModel, get_huggingface_model(), get_hf_latency_metric(), 0.001),
         (ONNXModel, get_onnx_model(), get_accuracy_metric(post_process), 0.99),
         (ONNXModel, get_onnx_model(), get_latency_metric(), 0.001),
         (OpenVINOModel, get_openvino_model(), get_accuracy_metric(openvino_post_process), 0.99),
         (OpenVINOModel, get_openvino_model(), get_latency_metric(), 0.001),
     ]
 
     @pytest.mark.parametrize(
-        "model_cls,model_path,metric,expected_res",
+        "model_cls,model_config,metric,expected_res",
         EVALUATION_TEST_CASE,
     )
-    def test_evaluate_model(self, model_cls, model_path, metric, expected_res):
-        olive_model = model_cls(model_path=model_path)
-        evaluator = OliveEvaluator(metrics=[metric])
-        actual_res = evaluator.evaluate(olive_model)[metric.name]
+    def test_evaluate_model(self, model_cls, model_config, metric, expected_res):
+        olive_model = model_cls(**model_config)
+        actual_res = LocalSystem().evaluate_model(olive_model, [metric])[metric.name]
         assert actual_res >= expected_res
```

## test/integ_test/evaluator/local_eval/utils.py

```diff
@@ -40,76 +40,126 @@
 
 
 def create_dataloader(data_dir, batch_size):
     dataset = datasets.MNIST(data_dir, train=True, download=True, transform=ToTensor())
     return torch.utils.data.DataLoader(dataset, batch_size)
 
 
-def get_accuracy_metric(post_process):
+def hf_post_process(res):
+    _, preds = torch.max(res[0], dim=1)
+    return preds
+
+
+def create_hf_dataloader(data_dir, batch_size):
+    from datasets import load_dataset
+    from torch.utils.data import Dataset
+    from transformers import AutoTokenizer
+
+    tokenizer = AutoTokenizer.from_pretrained("prajjwal1/bert-tiny")
+    dataset = load_dataset("glue", "mrpc", split="validation")
+
+    class BaseData(Dataset):
+        def __init__(self, data):
+            self.data = data
+
+        def __len__(self):
+            return 10
+
+        def __getitem__(self, idx):
+            data = {k: v for k, v in self.data[idx].items() if k != "label"}
+            return data, self.data[idx]["label"]
+
+    def _map(examples):
+        t_input = tokenizer(examples["sentence1"], examples["sentence2"], truncation=True, padding=True)
+        t_input["label"] = examples["label"]
+        return t_input
+
+    dataset = dataset.map(
+        _map,
+        batched=True,
+        remove_columns=dataset.column_names,
+    )
+    dataset.set_format(type="torch", output_all_columns=True)
+    return torch.utils.data.DataLoader(BaseData(dataset), batch_size)
+
+
+def get_accuracy_metric(post_process, dataloader=create_dataloader):
     accuracy_metric_config = {
         "post_processing_func": post_process,
         "data_dir": data_dir,
-        "dataloader_func": create_dataloader,
+        "dataloader_func": dataloader,
     }
     accuracy_metric = Metric(
         name="accuracy",
         type=MetricType.ACCURACY,
         sub_type=AccuracySubType.ACCURACY_SCORE,
         user_config=accuracy_metric_config,
     )
     return accuracy_metric
 
 
-def get_latency_metric():
+def get_latency_metric(dataloader=create_dataloader):
     latency_metric_config = {
         "data_dir": data_dir,
-        "dataloader_func": create_dataloader,
+        "dataloader_func": dataloader,
     }
     latency_metric = Metric(
         name="latency",
         type=MetricType.LATENCY,
         sub_type=LatencySubType.AVG,
         user_config=latency_metric_config,
     )
     return latency_metric
 
 
+def get_hf_accuracy_metric(post_process=hf_post_process, dataloader=create_hf_dataloader):
+    return get_accuracy_metric(post_process, dataloader)
+
+
+def get_hf_latency_metric(dataloader=create_hf_dataloader):
+    return get_latency_metric(dataloader)
+
+
 def get_pytorch_model():
     download_path = models_dir / "model.pt"
     pytorch_model_config = {
         "container": "olivetest",
         "blob": "models/model.pt",
         "download_path": download_path,
     }
     download_azure_blob(**pytorch_model_config)
-    return str(download_path)
+    return {"model_path": str(download_path)}
+
+
+def get_huggingface_model():
+    return {"hf_config": {"model_class": "AutoModelForSequenceClassification", "model_name": "prajjwal1/bert-tiny"}}
 
 
 def get_onnx_model():
     download_path = models_dir / "model.onnx"
     onnx_model_config = {
         "container": "olivetest",
         "blob": "models/model.onnx",
         "download_path": download_path,
     }
     download_azure_blob(**onnx_model_config)
-    return str(download_path)
+    return {"model_path": str(download_path)}
 
 
 def get_openvino_model():
     download_path = models_dir / "openvino.zip"
     openvino_model_config = {
         "container": "olivetest",
         "blob": "models/openvino.zip",
         "download_path": download_path,
     }
     download_azure_blob(**openvino_model_config)
     with ZipFile(download_path) as zip_ref:
         zip_ref.extractall(models_dir)
-    return str(models_dir / "openvino")
+    return {"model_path": str(models_dir / "openvino")}
 
 
 def download_azure_blob(container, blob, download_path):
     try:
         conn_str = os.environ["OLIVEWHEELS_STORAGE_CONNECTION_STRING"]
     except KeyError:
         raise Exception("Please set the environment variable OLIVEWHEELS_STORAGE_CONNECTION_STRING")
```

## test/unit_test/conftest.py

```diff
@@ -5,10 +5,13 @@
 from test.unit_test.utils import create_onnx_model_file, delete_onnx_model_files
 
 import pytest
 
 
 @pytest.fixture(scope="session", autouse=True)
 def setup_onnx_model():
+    from datasets import disable_caching
+
+    disable_caching()
     create_onnx_model_file()
     yield
     delete_onnx_model_files()
```

## test/unit_test/test_cache.py

```diff
@@ -1,67 +1,109 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
+import json
 import os
 import platform
 import shutil
 from pathlib import Path
 
 import pytest
 
-from olive.cache import clean_pass_run_cache
+from olive.cache import clean_pass_run_cache, create_cache, get_cache_sub_dirs, save_model
 
 
 class TestCache:
     @pytest.mark.parametrize(
         "model_path",
         ["0_model_folder", "0_model.onnx"],
     )
     def test_clean_pass_run_cache(self, model_path):
         # setup
         pass_type = "onnxconversion"
         cache_dir = Path("cache_dir")
         cache_dir.mkdir(parents=True, exist_ok=True)
+        create_cache(cache_dir)
+        model_cache_dir, run_cache_dir, evaluation_cache_dir = get_cache_sub_dirs(cache_dir)
 
         if model_path == "0_model_folder":
-            model_folder = cache_dir / model_path
+            model_folder = model_cache_dir / model_path
             model_folder.mkdir(parents=True, exist_ok=True)
             model_p = str(model_folder)
         else:
-            model_p = str(cache_dir / model_path)
-            open(str(cache_dir / model_path), "w")
+            model_p = str(model_cache_dir / model_path)
+            open(model_p, "w")
 
-        run_cache_dir = cache_dir / "runs"
-        run_cache_dir.mkdir(parents=True, exist_ok=True)
         run_cache_file_path = str((run_cache_dir / f"{pass_type}-p(･◡･)p.json").resolve())
         with open(run_cache_file_path, "w") as run_cache_file:
             run_data = (
                 '{"pass_name": "OnnxConversion", "input_model_id": "0", "output_model_id": "0_OnnxConversion-0-1"}'
             )
             run_cache_file.write(run_data)
 
-        model_cache_dir = cache_dir / "models"
-        model_cache_dir.mkdir(parents=True, exist_ok=True)
         model_cache_file_path = str((model_cache_dir / "0_p(･◡･)p.json").resolve())
         with open(model_cache_file_path, "w") as model_cache_file:
             model_data = f'{{"model_path": "{model_p}"}}'
             if platform.system() == "Windows":
                 model_data = model_data.replace("\\", "//")
             model_cache_file.write(model_data)
 
-        evaluation_cache_dir = cache_dir / "evaluations"
-        evaluation_cache_dir.mkdir(parents=True, exist_ok=True)
         evaluation_cache_file_path = str((evaluation_cache_dir / "0_p(･◡･)p.json").resolve())
         open(evaluation_cache_file_path, "w")
 
         # execute
         clean_pass_run_cache(pass_type, cache_dir)
 
         # assert
         assert not os.path.exists(model_p)
         assert not os.path.exists(run_cache_file_path)
         assert not os.path.exists(model_cache_file_path)
         assert not os.path.exists(evaluation_cache_file_path)
 
         # cleanup
         shutil.rmtree(cache_dir)
+
+    @pytest.mark.parametrize(
+        "model_path",
+        ["0_model_folder", "0_model.onnx"],
+    )
+    def test_save_model(self, model_path):
+        # setup
+        cache_dir = Path("cache_dir")
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        create_cache(cache_dir)
+        model_cache_dir, _, _ = get_cache_sub_dirs(cache_dir)
+
+        if model_path == "0_model_folder":
+            model_folder = model_cache_dir / model_path
+            model_folder.mkdir(parents=True, exist_ok=True)
+            model_p = str(model_folder)
+        else:
+            model_p = str(model_cache_dir / model_path)
+            open(model_p, "w")
+
+        # cache model to cache_dir
+        model_id = "0"
+        model_cache_dir = cache_dir / "models"
+        model_cache_dir.mkdir(parents=True, exist_ok=True)
+        model_cache_file_path = str((model_cache_dir / f"{model_id}_p(･◡･)p.json").resolve())
+        model_json = {"type": "onnx", "config": {"model_path": model_p}}
+        json.dump(model_json, open(model_cache_file_path, "w"))
+
+        # output model to output_dir
+        output_dir = cache_dir / "output"
+        shutil.rmtree(output_dir, ignore_errors=True)
+        output_name = "test_model"
+        output_json = save_model(model_id, output_dir, output_name, cache_dir)
+
+        # assert
+        output_model_path = (output_dir / f"{output_name}").with_suffix(Path(model_p).suffix).resolve()
+        output_model_path = str(output_model_path.resolve())
+        output_json_path = output_dir / f"{output_name}.json"
+        assert output_model_path == output_json["config"]["model_path"]
+        assert os.path.exists(output_model_path)
+        assert os.path.exists(output_json_path)
+        assert output_model_path == json.load(open(output_json_path))["config"]["model_path"]
+
+        # cleanup
+        shutil.rmtree(cache_dir)
```

## test/unit_test/utils.py

```diff
@@ -1,58 +1,83 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import os
 from pathlib import Path
 
+import numpy as np
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader, Dataset
 
+from olive.data.config import DataComponentConfig, DataConfig
+from olive.data.registry import Registry
 from olive.evaluator.metric import Metric, MetricType
 from olive.evaluator.metric_config import MetricGoal
 from olive.model import ONNXModel, PyTorchModel
-from olive.passes.onnx.conversion import OnnxConversion
+from olive.passes.olive_pass import create_pass_from_dict
+from olive.passes.onnx import OnnxConversion, OnnxDynamicQuantization
 
 ONNX_MODEL_PATH = Path(__file__).absolute().parent / "dummy_model.onnx"
 
 
 class DummyModel(nn.Module):
     def __init__(self):
         super(DummyModel, self).__init__()
-        self.fc1 = nn.Linear(10, 10)
+        self.fc1 = nn.Linear(1, 10)
 
     def forward(self, x):
         x = torch.relu(self.fc1(x))
         return x
 
 
 class DummyDataset(Dataset):
     def __init__(self, size):
         self.size = size
 
     def __getitem__(self, idx):
-        return torch.randn(10), 1
+        return torch.randn(1), torch.rand(10)
+
+    def __len__(self):
+        return self.size
+
+
+class FixedDummyDataset(Dataset):
+    def __init__(self, size):
+        self.size = size
+        self.rng = np.random.default_rng(0)
+        self.data = torch.tensor(self.rng.random((size, 1)))
+
+    def __getitem__(self, idx):
+        return self.data[idx], torch.rand(10)
 
     def __len__(self):
         return self.size
 
 
 def pytorch_model_loader(model_path):
     return DummyModel().eval()
 
 
 def get_pytorch_model():
-    return PyTorchModel(model_loader=pytorch_model_loader, model_path=None)
+    return PyTorchModel(
+        model_loader=pytorch_model_loader,
+        model_path=None,
+        io_config={"input_names": ["input"], "output_names": ["output"], "input_shapes": [(1, 1)]},
+    )
+
+
+def get_pytorch_model_dummy_input():
+    return torch.randn(1, 1)
 
 
 def create_onnx_model_file():
     pytorch_model = pytorch_model_loader(model_path=None)
-    dummy_input = torch.randn(1, 10)
+    dummy_input = get_pytorch_model_dummy_input()
     torch.onnx.export(
         pytorch_model, dummy_input, ONNX_MODEL_PATH, opset_version=10, input_names=["input"], output_names=["output"]
     )
 
 
 def get_onnx_model():
     return ONNXModel(model_path=str(ONNX_MODEL_PATH))
@@ -60,20 +85,25 @@
 
 def delete_onnx_model_files():
     if os.path.exists(ONNX_MODEL_PATH):
         os.remove(ONNX_MODEL_PATH)
 
 
 def create_dataloader(datadir, batchsize):
-    dataloader = DataLoader(DummyDataset(10))
+    dataloader = DataLoader(DummyDataset(1))
+    return dataloader
+
+
+def create_fixed_dataloader(datadir, batchsize):
+    dataloader = DataLoader(FixedDummyDataset(1))
     return dataloader
 
 
-def get_accuracy_metric(acc_subtype):
-    accuracy_metric_config = {"dataloader_func": create_dataloader}
+def get_accuracy_metric(acc_subtype, random_dataloader=True):
+    accuracy_metric_config = {"dataloader_func": create_dataloader if random_dataloader else create_fixed_dataloader}
     accuracy_metric = Metric(
         name="accuracy",
         type=MetricType.ACCURACY,
         sub_type=acc_subtype,
         goal=MetricGoal(type="threshold", value=0.99),
         user_config=accuracy_metric_config,
     )
@@ -96,14 +126,87 @@
         type=MetricType.LATENCY,
         sub_type=lat_subtype,
         user_config=latency_metric_config,
     )
     return latency_metric
 
 
-def get_onnxconversion_pass():
-    onnx_conversion_config = {
-        "input_names": ["input"],
-        "output_names": ["output"],
-    }
-    p = OnnxConversion(onnx_conversion_config)
+def get_onnxconversion_pass(ignore_pass_config=True):
+    onnx_conversion_config = {}
+    p = create_pass_from_dict(OnnxConversion, onnx_conversion_config)
+    if ignore_pass_config:
+        return p
+    pass_config = p.config_at_search_point({})
+    pass_config = p.serialize_config(pass_config)
+    return p, pass_config
+
+
+def get_onnx_dynamic_quantization_pass(disable_search=False):
+    p = create_pass_from_dict(OnnxDynamicQuantization, disable_search=disable_search)
     return p
+
+
+def get_data_config():
+    @Registry.register_dataset("test_dataset")
+    def _test_dataset(test_value):
+        ...
+
+    @Registry.register_dataloader()
+    def _test_dataloader(test_value):
+        ...
+
+    @Registry.register_pre_process()
+    def _pre_process(test_value):
+        ...
+
+    @Registry.register_post_process()
+    def _post_process(test_value):
+        ...
+
+    return DataConfig(
+        components={
+            "load_dataset": {
+                "name": "test_dataset",
+                "type": "test_dataset",
+                "params": {"test_value": "test_value"},
+            },
+            "dataloader": {
+                "name": "test_dataloader",
+                "type": "_test_dataloader",  # This is the key to get dataloader
+                "params": {"test_value": "test_value"},
+            },
+        }
+    )
+
+
+def get_glue_huggingface_data_config():
+    return DataConfig(
+        type="HuggingfaceContainer",
+        params_config={
+            "task": "text-classification",
+            "model_name": "bert-base-uncased",
+            "data_name": "glue",
+            "subset": "mrpc",
+            "split": "validation",
+            "input_cols": ["sentence1", "sentence2"],
+            "label_cols": ["label"],
+            "batch_size": 1,
+        },
+    )
+
+
+def get_dc_params_config():
+    return DataConfig(
+        params_config={
+            "data_dir": "./params_config",
+            "batch_size": 1,
+            "label_cols": ["label_from_params_config"],
+        },
+        components={
+            "load_dataset": DataComponentConfig(
+                params={
+                    "data_dir": "./params",
+                    "batch_size": 10,
+                }
+            )
+        },
+    )
```

## test/unit_test/evaluator/test_accuracy.py

```diff
@@ -16,15 +16,15 @@
     targets = [1, 1, 1, 1]
     expected_res = 0.99
     mock_res = MagicMock()
     mock_res.item.return_value = expected_res
     mock_torchmetrics.Accuracy().return_value = mock_res
 
     # execute
-    actual_res = acc.evaluate(preds, targets)
+    actual_res = acc.measure(preds, targets)
 
     # assert
     mock_torch.tensor.called_once_with(preds)
     mock_torch.tensor.called_once_with(targets)
     assert actual_res == expected_res
 
 
@@ -37,15 +37,15 @@
     targets = [1, 1, 1, 1]
     expected_res = 0.99
     mock_res = MagicMock()
     mock_res.item.return_value = expected_res
     mock_torchmetrics.F1Score().return_value = mock_res
 
     # execute
-    actual_res = acc.evaluate(preds, targets)
+    actual_res = acc.measure(preds, targets)
 
     # assert
     mock_torch.tensor.called_once_with(preds)
     mock_torch.tensor.called_once_with(targets)
     assert actual_res == expected_res
 
 
@@ -58,15 +58,15 @@
     targets = [1, 1, 1, 1]
     expected_res = 0.99
     mock_res = MagicMock()
     mock_res.item.return_value = expected_res
     mock_torchmetrics.Precision().return_value = mock_res
 
     # execute
-    actual_res = acc.evaluate(preds, targets)
+    actual_res = acc.measure(preds, targets)
 
     # assert
     mock_torch.tensor.called_once_with(preds)
     mock_torch.tensor.called_once_with(targets)
     assert actual_res == expected_res
 
 
@@ -79,15 +79,15 @@
     targets = [1, 1, 1, 1]
     expected_res = 0.99
     mock_res = MagicMock()
     mock_res.item.return_value = expected_res
     mock_torchmetrics.Recall().return_value = mock_res
 
     # execute
-    actual_res = acc.evaluate(preds, targets)
+    actual_res = acc.measure(preds, targets)
 
     # assert
     mock_torch.tensor.called_once_with(preds)
     mock_torch.tensor.called_once_with(targets)
     assert actual_res == expected_res
 
 
@@ -100,13 +100,13 @@
     targets = [1, 1, 1, 1]
     expected_res = 0.99
     mock_res = MagicMock()
     mock_res.item.return_value = expected_res
     mock_torchmetrics.functional.auc.return_value = mock_res
 
     # execute
-    actual_res = acc.evaluate(preds, targets)
+    actual_res = acc.measure(preds, targets)
 
     # assert
     mock_torch.tensor.called_once_with(preds)
     mock_torch.tensor.called_once_with(targets)
     assert actual_res == expected_res
```

## test/unit_test/systems/test_local.py

```diff
@@ -3,31 +3,32 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from test.unit_test.utils import get_accuracy_metric, get_custom_metric, get_latency_metric
 from unittest.mock import MagicMock, patch
 
 import pytest
 
+from olive.constants import Framework
 from olive.evaluator.metric import AccuracySubType, LatencySubType, MetricType
 from olive.systems.local import LocalSystem
 
 
 class TestLocalSystem:
     @pytest.fixture(autouse=True)
     def setup(self):
-        self.local_system = LocalSystem()
+        self.system = LocalSystem()
 
     def test_run_pass(self):
         # setup
         p = MagicMock()
         olive_model = MagicMock()
         output_model_path = "output_model_path"
 
         # execute
-        self.local_system.run_pass(p, olive_model, output_model_path)
+        self.system.run_pass(p, olive_model, output_model_path)
 
         # assert
         p.run.called_once_with(olive_model, output_model_path, None)
 
     METRIC_TEST_CASE = [
         (get_accuracy_metric(AccuracySubType.ACCURACY_SCORE)),
         (get_accuracy_metric(AccuracySubType.F1_SCORE)),
@@ -46,29 +47,35 @@
         (get_custom_metric()),
     ]
 
     @pytest.mark.parametrize(
         "metric",
         METRIC_TEST_CASE,
     )
-    @patch("olive.systems.local.evaluate_accuracy")
-    @patch("olive.systems.local.evaluate_latency")
-    @patch("olive.systems.local.evaluate_custom_metric")
-    def test_evaluate_model(self, mock_evaluate_custom_metric, mock_evaluate_latency, mock_evaluate_accuracy, metric):
+    @patch("olive.evaluator.olive_evaluator.OliveEvaluator.get_user_config")
+    @patch("olive.evaluator.olive_evaluator.OnnxEvaluator._evaluate_accuracy")
+    @patch("olive.evaluator.olive_evaluator.OnnxEvaluator._evaluate_latency")
+    @patch("olive.evaluator.olive_evaluator.OnnxEvaluator._evaluate_custom")
+    def test_evaluate_model(
+        self, mock_evaluate_custom, mock_evaluate_latency, mock_evaluate_accuracy, mock_get_user_config, metric
+    ):
         # setup
         olive_model = MagicMock()
+        olive_model.framework = Framework.ONNX
         expected_res = "0.382715310"
-        mock_evaluate_custom_metric.return_value = expected_res
+        mock_evaluate_custom.return_value = expected_res
         mock_evaluate_latency.return_value = expected_res
         mock_evaluate_accuracy.return_value = expected_res
+        mock_get_user_config.return_value = (None, None, None)
 
         # execute
-        actual_res = self.local_system.evaluate_model(olive_model, [metric])
+        actual_res = self.system.evaluate_model(olive_model, [metric])[metric.name]
 
         # assert
         if metric.type == MetricType.ACCURACY:
-            mock_evaluate_accuracy.called_once_with(olive_model, metric, self.local_system.device)
-        if metric.type == MetricType.LATENCY:
-            mock_evaluate_latency.called_once_with(olive_model, metric, self.local_system.device)
-        if metric.type == MetricType.CUSTOM:
-            mock_evaluate_custom_metric.called_once_with(olive_model, metric, self.local_system.device)
-        assert actual_res[metric.name] == expected_res
+            mock_evaluate_accuracy.called_once_with(olive_model, metric, None, self.system.device, None)
+        elif metric.type == MetricType.LATENCY:
+            mock_evaluate_latency.called_once_with(olive_model, metric, None, self.system.device, None)
+        elif metric.type == MetricType.CUSTOM:
+            mock_evaluate_custom.called_once_with(olive_model, metric, None, None, self.system.device, None)
+
+        assert actual_res == expected_res
```

## test/unit_test/systems/azureml/test_aml_system.py

```diff
@@ -2,37 +2,39 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import os
 import tempfile
 from pathlib import Path
 from test.unit_test.utils import get_accuracy_metric, get_latency_metric, get_pytorch_model
-from unittest.mock import MagicMock, patch
+from unittest.mock import MagicMock, Mock, patch
 
 import pytest
 from azure.ai.ml import Input, Output
 from azure.ai.ml.constants import AssetTypes
 
+from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.evaluator.metric import AccuracySubType, LatencySubType
-from olive.model import ONNXModel
+from olive.model import ModelStorageKind, ONNXModel
+from olive.passes.olive_pass import create_pass_from_dict
 from olive.passes.onnx.conversion import OnnxConversion
 from olive.systems.azureml.aml_system import AzureMLSystem
 from olive.systems.common import AzureMLDockerConfig
 
 
 class TestAzureMLSystem:
     @pytest.fixture(autouse=True)
-    @patch("olive.systems.azureml.aml_system.MLClient.from_config")
     @patch("olive.systems.azureml.aml_system.Environment")
-    def setup(self, mock_env, mock_from_config):
+    def setup(self, mock_env):
         docker_config = AzureMLDockerConfig(
             base_image="base_image",
             conda_file_path="conda_file_path",
         )
-        self.aml_system = AzureMLSystem("dummy", "dummy", docker_config)
+        mock_azureml_client_config = Mock(spec=AzureMLClientConfig)
+        self.system = AzureMLSystem(mock_azureml_client_config, "dummy", docker_config)
 
     METRIC_TEST_CASE = [
         (get_accuracy_metric(AccuracySubType.ACCURACY_SCORE)),
         (get_accuracy_metric(AccuracySubType.F1_SCORE)),
         (get_accuracy_metric(AccuracySubType.PRECISION)),
         (get_accuracy_metric(AccuracySubType.RECALL)),
         (get_accuracy_metric(AccuracySubType.AUC)),
@@ -55,94 +57,95 @@
     @patch("olive.systems.azureml.aml_system.AzureMLSystem._create_pipeline_for_evaluation")
     @patch("olive.systems.azureml.aml_system.tempfile.TemporaryDirectory")
     def test_evaluate_model(self, mock_tempdir, mock_create_pipeline, mock_retry_func, metric):
         # setup
         olive_model = get_pytorch_model()
         output_folder = Path(__file__).absolute().parent / "output_metrics"
         mock_tempdir.return_value.__enter__.return_value = output_folder
+        ml_client = MagicMock()
+        self.system.azureml_client_config.create_client.return_value = ml_client
 
         # execute
-        res = self.aml_system.evaluate_model(olive_model, [metric])
+        res = self.system.evaluate_model(olive_model, [metric])[metric.name]
 
         # assert
         mock_create_pipeline.assert_called_once_with(output_folder, olive_model, [metric])
-        self.aml_system.ml_client.jobs.stream.assert_called_once()
+        ml_client.jobs.stream.assert_called_once()
         assert mock_retry_func.call_count == 2
         if metric.name == "accuracy":
-            assert res[metric.name] == 0.99618
+            assert res == 0.99618
         if metric.name == "latency":
-            assert res[metric.name] == 0.031415
+            assert res == 0.031415
 
     @patch("olive.systems.azureml.aml_system.shutil.copy")
     @patch("olive.systems.azureml.aml_system.retry_func")
     @patch("olive.systems.azureml.aml_system.AzureMLSystem._create_pipeline_for_pass")
     @patch("olive.systems.azureml.aml_system.tempfile.TemporaryDirectory")
     def test_run_pass(self, mock_tempdir, mock_create_pipeline, mock_retry_func, mock_copy):
         # setup
-        onnx_conversion_config = {
-            "input_names": ["input"],
-            "output_names": ["output"],
-        }
-        p = OnnxConversion(onnx_conversion_config)
+        onnx_conversion_config = {}
+        p = create_pass_from_dict(OnnxConversion, onnx_conversion_config)
         olive_model = get_pytorch_model()
         output_model_path = "output_model_path"
         output_folder = Path(__file__).absolute().parent / "output_pass"
         mock_tempdir.return_value.__enter__.return_value = output_folder
-        expected_model = ONNXModel(model_path=f"{output_model_path}.onnx", name="test_model")
+        expected_model = ONNXModel(model_path=ONNXModel.resolve_path(output_model_path), name="test_model")
+        ml_client = MagicMock()
+        self.system.azureml_client_config.create_client.return_value = ml_client
 
         # execute
-        actual_res = self.aml_system.run_pass(p, olive_model, output_model_path)
+        actual_res = self.system.run_pass(p, olive_model, output_model_path)
 
         # assert
         mock_create_pipeline.assert_called_once_with(output_folder, olive_model, p.to_json(), p.path_params)
         assert mock_retry_func.call_count == 2
-        self.aml_system.ml_client.jobs.stream.assert_called_once()
+        ml_client.jobs.stream.assert_called_once()
         assert expected_model.to_json() == actual_res.to_json()
 
     @pytest.mark.parametrize(
-        "is_aml_model",
-        [True, False],
+        "model_storage_kind",
+        [ModelStorageKind.AzureMLModel, ModelStorageKind.LocalFile],
     )
-    def test__create_model_args(self, is_aml_model):
+    def test__create_model_args(self, model_storage_kind):
         # setup
         temp_model = tempfile.NamedTemporaryFile(dir=".", suffix=".onnx", prefix="model_0")
         model_json = {
+            "type": "onnxmodel",
             "config": {
                 "model_script": "model_script",
                 "script_dir": "script_dir",
                 "model_path": temp_model.name,
-                "is_file": True,
-            }
+                "model_storage_kind": model_storage_kind,
+            },
         }
-        model_json["config"].update({"is_aml_model": is_aml_model})
         tem_dir = Path(".")
         model_config_path = tem_dir / "model_config.json"
         model_path = tem_dir / "model.onnx"
-        if is_aml_model:
+        if model_storage_kind == ModelStorageKind.AzureMLModel:
             expected_model_path = Input(type=AssetTypes.CUSTOM_MODEL, path=temp_model.name)
         else:
             expected_model_path = Input(type=AssetTypes.URI_FILE, path=model_path)
         expected_model_script = Input(type=AssetTypes.URI_FILE, path="model_script")
         expected_model_script_dir = Input(type=AssetTypes.URI_FOLDER, path="script_dir")
         expected_model_config = Input(type=AssetTypes.URI_FILE, path=model_config_path)
         expected_res = {
             "model_config": expected_model_config,
             "model_path": expected_model_path,
             "model_script": expected_model_script,
             "model_script_dir": expected_model_script_dir,
         }
 
         # execute
-        actual_res = self.aml_system._create_model_args(model_json, tem_dir)
+        actual_res = self.system._create_model_args(model_json, tem_dir)
 
         # assert
         assert actual_res == expected_res
         assert model_json["config"]["model_script"] is None
         assert model_json["config"]["script_dir"] is None
-        assert model_json["config"]["is_aml_model"] is False
+        assert model_json["config"]["model_storage_kind"] != ModelStorageKind.AzureMLModel
         assert model_json["config"]["model_path"] is None
 
         # cleanup
         if os.path.exists(model_path):
             os.remove(model_path)
         if os.path.exists(model_config_path):
             os.remove(model_config_path)
@@ -167,75 +170,75 @@
             "metric_config": expected_metric_config,
             "metric_user_script": expected_metric_user_script,
             "metric_script_dir": expected_metric_script_dir,
             "metric_data_dir": expected_metric_data_dir,
         }
 
         # execute
-        actual_res = self.aml_system._create_metric_args(metric_config, tem_dir)
+        actual_res = self.system._create_metric_args(metric_config, tem_dir)
 
         # assert
         assert actual_res == expected_res
         assert metric_config["user_config"]["user_script"] is None
         assert metric_config["user_config"]["script_dir"] is None
         assert metric_config["user_config"]["data_dir"] is None
 
         # cleanup
         if os.path.exists(metric_config_path):
             os.remove(metric_config_path)
 
     @pytest.mark.parametrize(
-        "is_aml_model",
-        [True, False],
+        "model_storage_kind",
+        [ModelStorageKind.AzureMLModel, ModelStorageKind.LocalFile],
     )
     @patch("olive.systems.azureml.aml_system.shutil.copy")
     @patch("olive.systems.azureml.aml_system.command")
     @patch("olive.systems.azureml.aml_system.AzureMLSystem._create_metric_args")
-    def test__create_metric_component(self, mock_create_metric_args, mock_command, mock_copy, is_aml_model):
+    def test__create_metric_component(self, mock_create_metric_args, mock_command, mock_copy, model_storage_kind):
         # setup
         tem_dir = Path(".")
         code_path = tem_dir / "code"
         metric = get_accuracy_metric(AccuracySubType.ACCURACY_SCORE)
         metric.user_config = {}
         model_args = {"input": Input(type=AssetTypes.URI_FILE, path="path")}
         metric_type = f"{metric.type}-{metric.sub_type}"
         model_inputs = {
             "model_config": Input(type=AssetTypes.URI_FILE),
             "model_path": Input(type=AssetTypes.CUSTOM_MODEL)
-            if is_aml_model
+            if model_storage_kind == ModelStorageKind.AzureMLModel
             else Input(type=AssetTypes.URI_FOLDER, optional=True),
             "model_script": Input(type=AssetTypes.URI_FILE, optional=True),
             "model_script_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
         }
         metric_inputs = {
             "metric_config": Input(type=AssetTypes.URI_FILE),
-            "metric_user_script": Input(type=AssetTypes.URI_FILE),
+            "metric_user_script": Input(type=AssetTypes.URI_FILE, optional=True),
             "metric_script_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
             "metric_data_dir": Input(type=AssetTypes.URI_FOLDER, optional=True),
         }
         inputs = {**model_inputs, **metric_inputs}
         expected_res = MagicMock()
         mock_command.return_value.return_value = expected_res
 
         # execute
-        actual_res = self.aml_system._create_metric_component(tem_dir, metric, model_args, is_aml_model)
+        actual_res = self.system._create_metric_component(tem_dir, metric, model_args, model_storage_kind)
 
         # assert
         assert actual_res == expected_res
         mock_command.assert_called_once_with(
             name=metric_type,
             display_name=metric_type,
             description=f"Run olive {metric_type} evaluation",
             command=self.create_command(inputs),
-            environment=self.aml_system.environment,
+            environment=self.system.environment,
             code=code_path,
             inputs=inputs,
             outputs=dict(pipeline_output=Output(type=AssetTypes.URI_FOLDER)),
             instance_count=1,
-            compute=self.aml_system.compute,
+            compute=self.system.compute,
         )
 
         # cleanup
         if os.path.exists(code_path):
             os.rmdir(code_path)
 
     def create_command(self, inputs):
```

## test/unit_test/systems/docker/test_docker_system.py

```diff
@@ -1,34 +1,41 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
+import tempfile
 from pathlib import Path
 from test.unit_test.utils import get_accuracy_metric, get_pytorch_model
 from unittest.mock import MagicMock, patch
 
+import pytest
+
 from olive.evaluator.metric import AccuracySubType
 from olive.systems.common import LocalDockerConfig
 from olive.systems.docker.docker_system import DockerSystem
 
 
 class TestDockerSystem:
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.tmp_dir = tempfile.TemporaryDirectory()
+
     @patch("olive.systems.docker.docker_system.docker.from_env")
     def test__init_image_exist(self, mock_from_env):
         # setup
         mock_docker_client = MagicMock()
         mock_from_env.return_value = mock_docker_client
         mock_image = MagicMock()
         mock_docker_client.images.get.return_value = mock_image
         docker_config = LocalDockerConfig(
             image_name="image_name", build_context_path="build_context_path", dockerfile="dockerfile"
         )
 
         # execute
-        docker_system = DockerSystem(docker_config)
+        docker_system = DockerSystem(docker_config, is_dev=True)
 
         # assert
         assert docker_system.image == mock_image
         mock_docker_client.images.get.called_once_with(docker_config.image_name)
 
     @patch("olive.systems.docker.docker_system.docker.from_env")
     def test__init_image_dockerfile_build(self, mock_from_env):
@@ -40,15 +47,15 @@
         docker_config = LocalDockerConfig(
             image_name="image_name", build_context_path="build_context_path", dockerfile="dockerfile"
         )
         mock_docker_client.images.get.side_effect = docker.errors.ImageNotFound("msg")
         mock_docker_client.images.build = MagicMock()
 
         # execute
-        DockerSystem(docker_config)
+        DockerSystem(docker_config, is_dev=True)
 
         # assert
         mock_docker_client.images.build.called_once_with(
             docker_config.build_context_path,
             docker_config.dockerfile,
             docker_config.image_name,
             docker_config.build_args,
@@ -57,27 +64,27 @@
     @patch("olive.systems.docker.docker_system.shutil.copy2")
     @patch("olive.systems.docker.docker_system.docker.from_env")
     @patch("olive.systems.docker.docker_system.tempfile.TemporaryDirectory")
     def test__init_image_requirements_file_build(self, mock_tempdir, mock_from_env, mock_copy):
         # setup
         import docker
 
-        tempdir = "tempdir"
+        tempdir = self.tmp_dir.name
         mock_tempdir.return_value.__enter__.return_value = tempdir
         mock_docker_client = MagicMock()
         mock_from_env.return_value = mock_docker_client
         docker_config = LocalDockerConfig(
             image_name="image_name",
             requirements_file_path="requirements_file_path",
         )
         mock_docker_client.images.get.side_effect = docker.errors.ImageNotFound("msg")
         mock_docker_client.images.build = MagicMock()
 
         # execute
-        docker_system = DockerSystem(docker_config)
+        docker_system = DockerSystem(docker_config, is_dev=True)
 
         # assert
         mock_docker_client.images.build.called_once_with(
             tempdir, docker_system.BASE_DOCKERFILE, docker_config.image_name, docker_config.build_args
         )
 
     @patch("olive.systems.docker.docker_system.copy.deepcopy")
@@ -102,22 +109,22 @@
         mock_create_evaluate_command,
         mock_create_run_command,
         mock_copy,
     ):
         # setup
         mock_docker_client = MagicMock()
         mock_from_env.return_value = mock_docker_client
-        tempdir = "tempdir"
+        tempdir = self.tmp_dir.name
         mock_tempdir.return_value.__enter__.return_value = tempdir
         olive_model = get_pytorch_model()
         metric = get_accuracy_metric(AccuracySubType.ACCURACY_SCORE)
         docker_config = LocalDockerConfig(
             image_name="image_name", build_context_path="build_context_path", dockerfile="dockerfile"
         )
-        docker_system = DockerSystem(docker_config)
+        docker_system = DockerSystem(docker_config, is_dev=True)
         container_root_path = Path("/olive/")
         eval_output_path = "eval_output"
         eval_output_name = "eval_res.json"
         mock_copy = MagicMock()
         mock_copy.return_value = mock_copy
 
         eval_file_mount_path = "eval_file_mount_path"
@@ -143,15 +150,15 @@
         eval_command = "eval_command"
         mock_create_evaluate_command.return_value = eval_command
 
         run_command = {"key": "val"}
         mock_create_run_command.return_value = run_command
 
         # execute
-        actual_res = docker_system.evaluate_model(olive_model, [metric])
+        actual_res = docker_system.evaluate_model(olive_model, [metric])[metric.name]
 
         # assert
         mock_create_eval_script_mount.called_once_with(container_root_path)
         mock_create_model_mount.called_once_with(mock_copy, container_root_path)
         vol_list = [eval_file_mount_str] + model_mount_str_list
         mock_create_metric_volumes_list.called_once_with(mock_copy, container_root_path, vol_list)
         mock_create_config_file.called_once_with(tempdir, mock_copy, mock_copy, container_root_path)
@@ -160,8 +167,8 @@
             eval_file_mount_path, model_mount_path, config_mount_path, output_mount_path, eval_output_name
         )
         mock_create_run_command.called_once_with(docker_system.run_params)
         volumes_list.append(config_file_mount_str)
         volumes_list.append(output_mount_str)
         mock_docker_client.containers.run.call_once_with(docker_system.image, eval_command, volumes_list, **run_command)
 
-        assert actual_res[metric.name] == 0.99618
+        assert actual_res == 0.99618
```

## Comparing `test/unit_test/evaluator/test_evaluation.py` & `test/unit_test/evaluator/test_olive_evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,77 +3,80 @@
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from test.unit_test.utils import get_accuracy_metric, get_latency_metric, get_onnx_model, get_pytorch_model
 from unittest.mock import patch
 
 import pytest
 
-from olive.evaluator.evaluation import evaluate_accuracy, evaluate_latency
 from olive.evaluator.metric import AccuracySubType, LatencySubType
+from olive.systems.local import LocalSystem
 
 
-class TestEvaluation:
+class TestOliveEvaluator:
+    @pytest.fixture(autouse=True)
+    def setup(self):
+        self.system = LocalSystem()
 
     ACCURACY_TEST_CASE = [
         (
             get_pytorch_model(),
             get_accuracy_metric(AccuracySubType.ACCURACY_SCORE),
-            "olive.evaluator.evaluation.AccuracyScore",
+            "olive.evaluator.accuracy.AccuracyScore",
             0.99,
         ),
         (
             get_pytorch_model(),
             get_accuracy_metric(AccuracySubType.F1_SCORE),
-            "olive.evaluator.evaluation.F1Score",
+            "olive.evaluator.accuracy.F1Score",
             0.99,
         ),
         (
             get_pytorch_model(),
             get_accuracy_metric(AccuracySubType.PRECISION),
-            "olive.evaluator.evaluation.Precision",
+            "olive.evaluator.accuracy.Precision",
             0.99,
         ),
-        (get_pytorch_model(), get_accuracy_metric(AccuracySubType.RECALL), "olive.evaluator.evaluation.Recall", 0.99),
-        (get_pytorch_model(), get_accuracy_metric(AccuracySubType.AUC), "olive.evaluator.evaluation.AUC", 0.99),
+        (get_pytorch_model(), get_accuracy_metric(AccuracySubType.RECALL), "olive.evaluator.accuracy.Recall", 0.99),
+        (get_pytorch_model(), get_accuracy_metric(AccuracySubType.AUC), "olive.evaluator.accuracy.AUC", 0.99),
         (
             get_onnx_model(),
             get_accuracy_metric(AccuracySubType.ACCURACY_SCORE),
-            "olive.evaluator.evaluation.AccuracyScore",
+            "olive.evaluator.accuracy.AccuracyScore",
             0.99,
         ),
         (
             get_onnx_model(),
             get_accuracy_metric(AccuracySubType.F1_SCORE),
-            "olive.evaluator.evaluation.F1Score",
+            "olive.evaluator.accuracy.F1Score",
             0.99,
         ),
         (
             get_onnx_model(),
             get_accuracy_metric(AccuracySubType.PRECISION),
-            "olive.evaluator.evaluation.Precision",
+            "olive.evaluator.accuracy.Precision",
             0.99,
         ),
-        (get_onnx_model(), get_accuracy_metric(AccuracySubType.RECALL), "olive.evaluator.evaluation.Recall", 0.99),
-        (get_onnx_model(), get_accuracy_metric(AccuracySubType.AUC), "olive.evaluator.evaluation.AUC", 0.99),
+        (get_onnx_model(), get_accuracy_metric(AccuracySubType.RECALL), "olive.evaluator.accuracy.Recall", 0.99),
+        (get_onnx_model(), get_accuracy_metric(AccuracySubType.AUC), "olive.evaluator.accuracy.AUC", 0.99),
     ]
 
     @pytest.mark.parametrize(
         "olive_model,metric,acc_subtype,expected_res",
         ACCURACY_TEST_CASE,
     )
     def test_evaluate_accuracy(self, olive_model, metric, acc_subtype, expected_res):
         # setup
-        with patch(acc_subtype) as mock_acc:
-            mock_acc.return_value.evaluate.return_value = expected_res
+        with patch(f"{acc_subtype}.measure") as mock_acc:
+            mock_acc.return_value = expected_res
 
             # execute
-            actual_res = evaluate_accuracy(olive_model, metric)
+            actual_res = self.system.evaluate_model(olive_model, [metric])[metric.name]
 
             # assert
-            mock_acc.return_value.evaluate.assert_called_once()
+            mock_acc.assert_called_once()
             assert expected_res == actual_res
 
     LATENCY_TEST_CASE = [
         (get_pytorch_model(), get_latency_metric(LatencySubType.AVG), 1),
         (get_pytorch_model(), get_latency_metric(LatencySubType.MAX), 1),
         (get_pytorch_model(), get_latency_metric(LatencySubType.MIN), 1),
         (get_pytorch_model(), get_latency_metric(LatencySubType.P50), 1),
@@ -95,11 +98,11 @@
 
     @pytest.mark.parametrize(
         "olive_model,metric,expected_res",
         LATENCY_TEST_CASE,
     )
     def test_evaluate_latency(self, olive_model, metric, expected_res):
         # execute
-        actual_res = evaluate_latency(olive_model, metric)
+        actual_res = self.system.evaluate_model(olive_model, [metric])[metric.name]
 
         # assert
         assert expected_res > actual_res
```

## Comparing `olive_ai-0.1.0.dist-info/LICENSE` & `olive_ai-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

