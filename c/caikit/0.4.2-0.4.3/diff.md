# Comparing `tmp/caikit-0.4.2.tar.gz` & `tmp/caikit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.4.2.tar` & `caikit-0.4.3.tar`

### file list

```diff
@@ -1,312 +1,315 @@
--rw-r--r--   0        0        0       60 2023-05-15 18:00:15.868723 caikit-0.4.2/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1272 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-15 18:00:15.868723 caikit-0.4.2/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      212 2023-05-15 18:00:15.868723 caikit-0.4.2/.gitignore
--rw-r--r--   0        0        0      324 2023-05-15 18:00:15.868723 caikit-0.4.2/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-15 18:00:15.868723 caikit-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-15 18:00:15.868723 caikit-0.4.2/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-15 18:00:15.868723 caikit-0.4.2/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-15 18:00:15.868723 caikit-0.4.2/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-15 18:00:15.868723 caikit-0.4.2/.whitesource
--rw-r--r--   0        0        0      336 2023-05-15 18:00:15.868723 caikit-0.4.2/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-15 18:00:15.868723 caikit-0.4.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-15 18:00:15.868723 caikit-0.4.2/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-15 18:00:15.868723 caikit-0.4.2/README.md
--rw-r--r--   0        0        0      152 2023-05-15 18:00:15.868723 caikit-0.4.2/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit-overview.png
--rw-r--r--   0        0        0      419 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/__init__.py
--rw-r--r--   0        0        0     5392 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/config.py
--rw-r--r--   0        0        0     6488 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/config/config.yml
--rw-r--r--   0        0        0     1819 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1026 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    28986 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    12390 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4736 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40248 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21916 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/model_manager.py
--rw-r--r--   0        0        0    41505 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module.py
--rw-r--r--   0        0        0     7074 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4716 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2769 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5715 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_meta.py
--rw-r--r--   0        0        0    14929 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/module_type.py
--rw-r--r--   0        0        0      709 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1246 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/resources/base.py
--rw-r--r--   0        0        0     5391 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32204 2023-05-15 18:00:15.872723 caikit-0.4.2/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9332 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16693 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5845 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13249 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12814 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10744 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8232 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9473 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15316 2023-05-15 18:00:15.876723 caikit-0.4.2/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6797 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17900 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-15 18:00:15.880723 caikit-0.4.2/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-15 18:00:15.880723 caikit-0.4.2/code-of-conduct.md
--rw-r--r--   0        0        0     1610 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-15 18:00:15.880723 caikit-0.4.2/docs/architecture_club/README.md
--rw-r--r--   0        0        0      837 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      671 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      643 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3061 2023-05-15 18:00:15.880723 caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
--rw-r--r--   0        0        0     1157 2023-05-15 18:00:22.136702 caikit-0.4.2/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-05-15 18:00:15.880723 caikit-0.4.2/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-15 18:00:15.880723 caikit-0.4.2/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0     3572 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/config/__init__.py
--rw-r--r--   0        0        0     4345 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/config/test_configs.py
--rw-r--r--   0        0        0     9076 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    11661 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26454 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13147 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    19621 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     1104 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4291 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0      521 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_imports.py
--rw-r--r--   0        0        0    22165 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    13348 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_module.py
--rw-r--r--   0        0        0     7667 2023-05-15 18:00:15.880723 caikit-0.4.2/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8080 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     3773 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_module_type.py
--rw-r--r--   0        0        0     1038 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2456 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4972 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    14659 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5542 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      337 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      646 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2456 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1306 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2713 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      410 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-15 18:00:15.884723 caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14146 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10454 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17866 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8668 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3768 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1372 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7848 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15426 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30064 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11070 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26122 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-15 18:00:15.888723 caikit-0.4.2/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1115 2023-05-15 18:00:15.888723 caikit-0.4.2/tox.ini
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-17 19:45:34.757668 caikit-0.4.3/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1272 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-17 19:45:34.757668 caikit-0.4.3/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-05-17 19:45:34.757668 caikit-0.4.3/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-17 19:45:34.757668 caikit-0.4.3/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-17 19:45:34.757668 caikit-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-17 19:45:34.757668 caikit-0.4.3/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-17 19:45:34.757668 caikit-0.4.3/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-17 19:45:34.757668 caikit-0.4.3/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-17 19:45:34.757668 caikit-0.4.3/.whitesource
+-rw-r--r--   0        0        0      368 2023-05-17 19:45:34.757668 caikit-0.4.3/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-17 19:45:34.757668 caikit-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-17 19:45:34.757668 caikit-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3626 2023-05-17 19:45:34.757668 caikit-0.4.3/README.md
+-rw-r--r--   0        0        0      152 2023-05-17 19:45:34.757668 caikit-0.4.3/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit-overview.png
+-rw-r--r--   0        0        0      419 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/config.py
+-rw-r--r--   0        0        0     6554 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/config/config.yml
+-rw-r--r--   0        0        0     1838 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1026 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    28986 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    12390 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40248 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21916 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    41505 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module.py
+-rw-r--r--   0        0        0     6062 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4716 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2769 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6293 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_meta.py
+-rw-r--r--   0        0        0    14929 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/module_type.py
+-rw-r--r--   0        0        0      709 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     5391 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32204 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9332 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-17 19:45:34.761668 caikit-0.4.3/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16693 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5845 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13249 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7155 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12818 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0      666 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10744 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4794 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8232 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9473 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15316 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6797 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17900 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-17 19:45:34.765668 caikit-0.4.3/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-17 19:45:34.765668 caikit-0.4.3/code-of-conduct.md
+-rw-r--r--   0        0        0     1610 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-17 19:45:34.765668 caikit-0.4.3/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      837 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1425 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      671 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-17 19:45:34.765668 caikit-0.4.3/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      643 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3061 2023-05-17 19:45:34.769668 caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py
+-rw-r--r--   0        0        0     1157 2023-05-17 19:45:37.989673 caikit-0.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0      639 2023-05-17 19:45:34.769668 caikit-0.4.3/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-05-17 19:45:34.769668 caikit-0.4.3/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-17 19:45:34.769668 caikit-0.4.3/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     3572 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/config/test_configs.py
+-rw-r--r--   0        0        0     9171 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    11661 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26454 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13147 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    19621 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     1104 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4291 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0      521 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21985 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    13348 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module.py
+-rw-r--r--   0        0        0     6950 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8080 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     3773 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_module_type.py
+-rw-r--r--   0        0        0     1038 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     2456 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4972 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    14622 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5542 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-17 19:45:34.769668 caikit-0.4.3/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      337 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1875 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      646 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2456 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1306 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2713 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      410 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14146 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10454 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17908 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     5398 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8668 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3768 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1716 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1372 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7848 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15426 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30097 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11070 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26122 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-17 19:45:34.773668 caikit-0.4.3/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1301 2023-05-17 19:45:34.773668 caikit-0.4.3/tox.ini
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 caikit-0.4.3/PKG-INFO
```

### Comparing `caikit-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.4.3/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/.github/workflows/build-library.yml` & `caikit-0.4.3/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/.github/workflows/lint-code.yml` & `caikit-0.4.3/.github/workflows/lint-code.yml`

 * *Files 18% similar despite different names*

```diff
@@ -33,8 +33,11 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r setup_requirements.txt
       - name: Check Formatting
         run: tox -e fmt
       - name: Run pylint
         run: tox -e lint
-
+      - name: Setup Graphviz # `graphviz/dot` is required for the import checker
+        uses: ts-graphviz/setup-graphviz@v1
+      - name: Enforce import rules
+        run: tox -e imports
```

### Comparing `caikit-0.4.2/.github/workflows/publish-library.yml` & `caikit-0.4.3/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/.pylintrc` & `caikit-0.4.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/CONTRIBUTING.md` & `caikit-0.4.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/LICENSE` & `caikit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/README.md` & `caikit-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit-overview.png` & `caikit-0.4.3/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/config/__init__.py` & `caikit-0.4.3/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/config/config.py` & `caikit-0.4.3/caikit/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 # limitations under the License.
 
 
 """Config methods for the `caikit` library. Mainly interacts with `config.yml`.
 """
 
 # Standard
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 import os
-import threading
 
 # First Party
 import aconfig
 import alog
 
 log = alog.use_channel("CONFIG")
 
@@ -31,15 +30,16 @@
     os.path.join(os.path.dirname(__file__), "config.yml")
 )
 
 # The core config object that is continually merged into
 _CONFIG: aconfig.Config = aconfig.Config({})
 # An immutable view into the core config object, to be passed to callers
 _IMMUTABLE_CONFIG: aconfig.ImmutableConfig = aconfig.ImmutableConfig({})
-_CONFIG_LOCK: threading.Lock = threading.Lock()
+# Little helper type for signatures
+_CONFIG_TYPE = Union[dict, aconfig.Config]
 
 
 def get_config() -> aconfig.Config:
     """Get the caikit configuration"""
     return _IMMUTABLE_CONFIG
 
 
@@ -67,34 +67,35 @@
     """
     if not config_yml_path and not config_dict:
         log.error("<CFG43273054E>", "No config_file or config_dict provided")
         raise ValueError("No config_file or config_dict provided")
 
     cfg = aconfig.Config(_CONFIG)
     if config_yml_path:
-        cfg = merge_configs(cfg, aconfig.Config.from_yaml(config_yml_path))
-    if config_dict:
-        cfg = merge_configs(cfg, aconfig.Config(config_dict))
+        new_config = aconfig.Config.from_yaml(config_yml_path)
+    else:
+        new_config = aconfig.Config(config_dict)
+
+    cfg = merge_configs(cfg, new_config, _get_merge_strategy(new_config))
 
     cfg = _merge_extra_files(cfg)
     _update_global_config(cfg)
 
 
 def _update_global_config(cfg: aconfig.Config):
-    """Updates the caikit config and creates a new immutable view of it to be shared via
+    """Replaces the caikit config and creates a new immutable view of it to be shared via
     get_config().
-    Locked because who the heck knows if merge_configs() is threadsafe.
     """
     # pylint: disable=global-statement
     global _IMMUTABLE_CONFIG
-    # Update the config by merging the new updates over the existing config
-    with _CONFIG_LOCK:
-        # Locked just in case `configure()` is called concurrently for any reason
-        merge_configs(_CONFIG, cfg)
-        _IMMUTABLE_CONFIG = aconfig.ImmutableConfig(_CONFIG, override_env_vars=False)
+    # pylint: disable=global-statement
+    global _CONFIG
+    _CONFIG = cfg
+    # Set override_env_vars=False because we want the immutable config to be an exact copy
+    _IMMUTABLE_CONFIG = aconfig.ImmutableConfig(_CONFIG, override_env_vars=False)
 
 
 def _merge_extra_files(config: aconfig.Config) -> aconfig.Config:
     """Looks at the `config_files` configuration item and merges those files into the config,
     left to right"""
     if config.config_files:
         extra_config_files = [
@@ -107,48 +108,69 @@
             log.info(
                 {
                     "log_code": "<RUN17612094I>",
                     "message": "Loading config file '%s'" % file,
                 }
             )
             new_overrides = aconfig.Config.from_yaml(file, override_env_vars=True)
-            config = merge_configs(config, new_overrides)
+            config = merge_configs(
+                config, new_overrides, _get_merge_strategy(new_overrides)
+            )
     return config
 
 
-def merge_configs(base: Optional[dict], overrides: Optional[dict]) -> dict:
+def merge_configs(
+    base: Optional[_CONFIG_TYPE],
+    overrides: Optional[_CONFIG_TYPE],
+    merge_strategy: str = "merge",
+) -> _CONFIG_TYPE:
     """Helper to perform a deep merge of the overrides into the base. The merge
     is done in place, but the resulting dict is also returned for convenience.
     The merge logic is quite simple: If both the base and overrides have a key
     and the type of the key for both is a dict, recursively merge, otherwise
     set the base value to the override value.
     Args:
         base: Optional[dict]
             The base config that will be updated with the overrides
         overrides: Optional[dict]
             The override config
+        merge_strategy: str
+            The merging strategy, either `merge` or `override`
+            `override` will replace values in base with those from overrides
+            `merge` will deep-merge dictionaries and prepend-merge lists
     Returns:
         merged: dict
             The merged results of overrides merged onto base
     """
     # Handle none args
     if base is None:
         return overrides or {}
     if overrides is None:
         return base or {}
 
+    if merge_strategy == "override":
+        base.update(overrides)
+        return base
+
     # Do the deep merge
     for key, value in overrides.items():
         if (
             key not in base
-            or not isinstance(base[key], dict)
-            or not isinstance(value, dict)
+            or not isinstance(base[key], (dict, list))
+            or not isinstance(value, (dict, list))
         ):
             base[key] = value
+        elif isinstance(value, list):
+            # merge lists by prepending new one
+            base[key] = value + base[key]
         else:
-            base[key] = merge_configs(base[key], value)
+            base[key] = merge_configs(base[key], value, merge_strategy)
 
     return base
 
 
+def _get_merge_strategy(cfg: _CONFIG_TYPE) -> str:
+    return cfg.get("merge_strategy", "merge")
+
+
 # Run initial configuration with the base config
 configure(BASE_CONFIG_PATH)
```

### Comparing `caikit-0.4.2/caikit/config/config.yml` & `caikit-0.4.3/caikit/config/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # User can set comma-separated string of config file locations to read
 config_files: ""
+# merge_strategy can be either `merge` which will merge lists and dicts,
+# or `override` which will set the values directly
+merge_strategy: "merge"
 
 # Global config switch for runtime check functions (type_check, value_check, file_check...)
 enable_error_checks: true
 # Maximum number of times that a single exception is logged
 max_exception_log_messages: 4
 load_path: null
 
 # Configuration for training/loading via module backends
 module_backends:
-    # Local is always enabled unless explicitly disabled
-    disable_local: false
     # Configuration for distributed loading and training. Each has an ordered
     # list of backends in priority order. Each entry is a mapping with a "type"
     # field and optionally a "config" field that maps to a blob of config for
     # the backend instance. Entries may also have a "name" field that must be
     # unique among entries, allowing for multiple instances of the same type.
     # For example:
     #
```

### Comparing `caikit-0.4.2/caikit/core/__init__.py` & `caikit-0.4.3/caikit/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 """Caikit Core AI Framework library.  This is the base framework for core AI/ML libraries.
 """
 
 # the import order cannot adhere to the linter here because we must do things like
 # disable warnings, initialize the JVM and configure logging in a specific order
 # pylint: disable=wrong-import-position,wrong-import-order
 
+# NOTE: There are cyclic imports due to the "import *"s here, when modules then
+# "import core"
+
 # Standard
 # We're filtering (most) warnings for now
 import warnings as _warnings
 
 _warnings.filterwarnings("ignore")
 
 # Local
-# must import toolkit first since we need alog to be set up before it is used
 from . import blocks, data_model, module, module_config, resources, toolkit, workflows
 from .blocks.base import BlockBase, block
 from .data_model import DataObjectBase, dataobject
 from .model_manager import *
 from .module import *
 from .module_backend_config import configure as backend_configure
 from .module_backends import *
```

### Comparing `caikit-0.4.2/caikit/core/augmentors/__init__.py` & `caikit-0.4.3/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/base.py` & `caikit-0.4.3/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.4.3/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.4.3/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/schemes/base.py` & `caikit-0.4.3/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.4.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.4.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/blocks/__init__.py` & `caikit-0.4.3/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/blocks/base.py` & `caikit-0.4.3/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/__init__.py` & `caikit-0.4.3/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/base.py` & `caikit-0.4.3/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.4.3/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/data_backends/base.py` & `caikit-0.4.3/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.4.3/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/dataobject.py` & `caikit-0.4.3/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/enums.py` & `caikit-0.4.3/caikit/core/data_model/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 # First Party
 import alog
 
 # Local
 from ..toolkit.errors import error_handler
 from ..toolkit.isa import isprotobufenum
-from . import protobufs
 
 log = alog.use_channel("DATAM")
 error = error_handler.get(log)
 
 
 @classmethod
 def to_dict(cls) -> Dict[str, int]:
@@ -82,15 +81,18 @@
     if not isprotobufenum(proto_enum):
         error(
             "<COR71783964E>",
             AttributeError(f"`{proto_enum}` is not a valid protobuf enumeration"),
         )
 
     name = proto_enum.DESCRIPTOR.name
-    enum_class = enum_class or Enum._create_(name, proto_enum.items())
+    log.debug2("Importing enum named %s", name)
+    if enum_class is None:
+        log.debug2("Creating Enum class for %s", name)
+        enum_class = Enum._create_(name, proto_enum.items())
 
     # Add extra utility functions
     setattr(enum_class, "to_dict", to_dict)
     setattr(enum_class, "to_munch", to_munch)
 
     globals()[name] = enum_class
     rev_name = name + "Rev"
@@ -126,13 +128,14 @@
     # caller = inspect.stack()[1]
     # caller_module = inspect.getmodule(caller[0])
     # current_globals = caller_module.__dict__
 
     # Add the str->int (EnumBase) and int->str (EnumRevBase) mapping for each enum
     # to the calling module's symbol table, then update __all__ to include the names
     # for the added objects.
-    all_enum_names = getattr(current_globals.get("protobufs"), "all_enum_names", [])
+    protobufs = current_globals.get("protobufs")
+    all_enum_names = getattr(protobufs, "all_enum_names", [])
     for name in all_enum_names:
         proto_enum = getattr(protobufs, name)
         name, rev_name = import_enum(proto_enum)
         current_globals[name] = globals()[name]
         current_globals[rev_name] = globals()[rev_name]
```

### Comparing `caikit-0.4.2/caikit/core/data_model/producer.py` & `caikit-0.4.3/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.4.3/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/__init__.py` & `caikit-0.4.3/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/converter.py` & `caikit-0.4.3/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.4.3/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/data_stream.py` & `caikit-0.4.3/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/resolver.py` & `caikit-0.4.3/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/data_model/streams/validator.py` & `caikit-0.4.3/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/model_manager.py` & `caikit-0.4.3/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module.py` & `caikit-0.4.3/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_backend_config.py` & `caikit-0.4.3/caikit/core/module_backend_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 # Standard
 from typing import List
 import copy
 
 # First Party
-import aconfig
 import alog
 
 # Local
 from .module import MODULE_BACKEND_REGISTRY
 from .module_backends.backend_types import (
     MODULE_BACKEND_CONFIG_FUNCTIONS,
     MODULE_BACKEND_TYPES,
@@ -71,39 +70,14 @@
     for backend_priority, registry, registry_name in [
         (config_object.load_priority, _CONFIGURED_LOAD_BACKENDS, "load"),
         (config_object.train_priority, _CONFIGURED_TRAIN_BACKENDS, "train"),
     ]:
         backend_priority = backend_priority or []
         error.type_check("<COR46006487E>", list, backend_priority=backend_priority)
 
-        # Check if disable_local is set
-        disable_local_backend = config_object.disable_local or False
-
-        # Add local at the end of priority by default
-        backend_priority_types = [cfg.get("type") for cfg in backend_priority]
-        error.value_check(
-            "<COR92038969E>",
-            not (
-                disable_local_backend
-                and MODULE_BACKEND_TYPES.LOCAL in backend_priority_types
-            ),
-            "Invalid configuration with {} in the priority list and disable_local set",
-            MODULE_BACKEND_TYPES.LOCAL,
-        )
-        if not disable_local_backend and (
-            MODULE_BACKEND_TYPES.LOCAL not in backend_priority_types
-        ):
-            log.debug3("Adding fallback priority to [%s]", MODULE_BACKEND_TYPES.LOCAL)
-            backend_priority.append(
-                aconfig.Config(
-                    {"type": MODULE_BACKEND_TYPES.LOCAL},
-                    override_env_vars=False,
-                )
-            )
-
         # Configure each backend instance
         for i, backend_config in enumerate(backend_priority):
             error.value_check(
                 "<COR48633635E>",
                 "type" in backend_config,
                 "All backend priority configs must have a 'type' field",
             )
```

### Comparing `caikit-0.4.2/caikit/core/module_backends/__init__.py` & `caikit-0.4.3/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_backends/backend_types.py` & `caikit-0.4.3/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_backends/base.py` & `caikit-0.4.3/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_backends/local_backend.py` & `caikit-0.4.3/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_config.py` & `caikit-0.4.3/caikit/core/module_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright The Caikit Authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 # Standard
 import os
 
 # First Party
 import aconfig
 import alog
```

### Comparing `caikit-0.4.2/caikit/core/module_meta.py` & `caikit-0.4.3/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/module_type.py` & `caikit-0.4.3/caikit/core/module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/resources/__init__.py` & `caikit-0.4.3/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/resources/base.py` & `caikit-0.4.3/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/task.py` & `caikit-0.4.3/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/__init__.py` & `caikit-0.4.3/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/compatibility.py` & `caikit-0.4.3/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/errors/__init__.py` & `caikit-0.4.3/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.4.3/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.4.3/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/fileio.py` & `caikit-0.4.3/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/isa.py` & `caikit-0.4.3/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/logging.py` & `caikit-0.4.3/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.4.3/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/serializers.py` & `caikit-0.4.3/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/toolkit/wip_decorator.py` & `caikit-0.4.3/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/workflows/__init__.py` & `caikit-0.4.3/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/core/workflows/base.py` & `caikit-0.4.3/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/__init__.py` & `caikit-0.4.3/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/common/__init__.py` & `caikit-0.4.3/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.4.3/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/common/data_model/producer.py` & `caikit-0.4.3/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/runtime/__init__.py` & `caikit-0.4.3/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.4.3/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.4.3/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/__init__.py` & `caikit-0.4.3/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/dump_services.py` & `caikit-0.4.3/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/grpc_server.py` & `caikit-0.4.3/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/interceptors/__init__.py` & `caikit-0.4.3/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.4.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/metrics/__init__.py` & `caikit-0.4.3/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.4.3/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/__init__.py` & `caikit-0.4.3/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/batcher.py` & `caikit-0.4.3/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/loaded_model.py` & `caikit-0.4.3/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/model_loader.py` & `caikit-0.4.3/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/model_manager.py` & `caikit-0.4.3/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/model_sizer.py` & `caikit-0.4.3/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/model_management/training_manager.py` & `caikit-0.4.3/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/__init__.py` & `caikit-0.4.3/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.4.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.4.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.4.3/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.4.3/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.4.3/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.4.3/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.4.3/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_factory.py` & `caikit-0.4.3/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.4.3/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.4.3/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/create_service.py` & `caikit-0.4.3/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.4.3/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/primitives.py` & `caikit-0.4.3/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/rpcs.py` & `caikit-0.4.3/caikit/runtime/service_generation/rpcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             triple[1]: Annotated[Optional[triple[0]], FieldNumber(triple[2])]
             for triple in self.request.triples
             if triple[1] in self.request.default_map
         }
         attrs = copy.copy(self.request.default_map)
         attrs["__annotations__"] = {**properties, **optional_properties}
 
-        if not properties and optional_properties:
+        if not properties and not optional_properties:
             log.warning(
                 "No arguments found for request %s. Cannot generate rpc",
                 self.request.name,
             )
             return None
 
         decorator = dataobject(package=package_name)
```

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.4.3/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.4.3/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/__init__.py` & `caikit-0.4.3/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.4.3/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.4.3/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.4.3/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.4.3/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.4.3/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/types/__init__.py` & `caikit-0.4.3/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/types/aborted_exception.py` & `caikit-0.4.3/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.4.3/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.4.3/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/utils/__init__.py` & `caikit-0.4.3/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/utils/import_util.py` & `caikit-0.4.3/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/utils/servicer_util.py` & `caikit-0.4.3/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/work_management/__init__.py` & `caikit-0.4.3/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/work_management/abortable_action.py` & `caikit-0.4.3/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/work_management/call_aborter.py` & `caikit-0.4.3/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.4.3/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/docs/adrs/010-data-model-definition.md` & `caikit-0.4.3/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/docs/adrs/015-runtime-service-generation.md` & `caikit-0.4.3/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/docs/adrs/018-shared-backends.md` & `caikit-0.4.3/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/docs/adrs/019-loader-stack.md` & `caikit-0.4.3/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/docs/architecture_club/04-25-23.md` & `caikit-0.4.3/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/start_runtime_with_sample_lib.py` & `caikit-0.4.3/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/README.md` & `caikit-0.4.3/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/client.py` & `caikit-0.4.3/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.4.3/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/start_runtime.py` & `caikit-0.4.3/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py` & `caikit-0.4.3/examples/text-sentiment/text_sentiment/runtime_model/hf_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/pyproject.toml` & `caikit-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.4.2"
+version = "0.4.3"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -17,15 +17,15 @@
     "alchemy-config>=1.1.1,<2.0.0",
     "alchemy-logging>=1.0.4,<2.0.0",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1,<0.16.0",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.3.0",
-    "munch>=2.5.0,<3.0",
+    "munch>=2.5.0,<4.0",
     "protobuf>=3.19.0,<5",
     "prometheus_client>=0.12.0,<1.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
```

### Comparing `caikit-0.4.2/scripts/fmt.sh` & `caikit-0.4.3/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/__init__.py` & `caikit-0.4.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/base.py` & `caikit-0.4.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/conftest.py` & `caikit-0.4.3/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,24 +182,25 @@
     yield model_id
 
     # teardown
     model_manager.unload_model(model_id)
 
 
 @contextmanager
-def temp_config(config_overrides: dict):
+def temp_config(config_overrides: dict, merge_strategy="override"):
     """Temporarily edit the caikit config in a mock context"""
     existing_config = copy.deepcopy(getattr(caikit.config.config, "_CONFIG"))
     # Patch out the internal config, starting with a fresh copy of the current config
     with patch.object(caikit.config.config, "_CONFIG", existing_config):
         # Patch the immutable view of the config as well
         # This is required otherwise the updated immutable view will persist after the test
         with patch.object(caikit.config.config, "_IMMUTABLE_CONFIG", None):
             # Run our config overrides inside the patch
             if config_overrides:
+                config_overrides["merge_strategy"] = merge_strategy
                 caikit.configure(config_dict=config_overrides)
             else:
                 # or just slap some random uuids in there. Barf, but we need to call `.configure()`
                 caikit.configure(config_dict={str(uuid.uuid4()): str(uuid.uuid4())})
             # Yield to the test with the new overridden config
             yield get_config()
```

### Comparing `caikit-0.4.2/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.4.3/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.4.3/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/blocks/__init__.py` & `caikit-0.4.3/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/blocks/test_base.py` & `caikit-0.4.3/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.4.3/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/streams/test_converter.py` & `caikit-0.4.3/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.4.3/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.4.3/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/streams/test_resolver.py` & `caikit-0.4.3/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/streams/test_validator.py` & `caikit-0.4.3/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/test_base.py` & `caikit-0.4.3/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/test_dataobject.py` & `caikit-0.4.3/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/data_model/test_producer.py` & `caikit-0.4.3/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/helpers.py` & `caikit-0.4.3/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/module_backends/test_backend_types.py` & `caikit-0.4.3/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_imports.py` & `caikit-0.4.3/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_model_manager.py` & `caikit-0.4.3/tests/core/test_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,16 +318,15 @@
     """Test that backend specific model can be loaded as a singleton"""
 
     _, DummyBar = setup_saved_model(MockBackend)
     # Configure backend
     with temp_config(
         {
             "module_backends": {
-                "priority": [backend_types.MOCK],
-                "configs": {"mock": {}},
+                "load_priority": [{"type": backend_types.MOCK}],
             }
         }
     ):
         configure()
 
         dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
         model1 = caikit.core.load(dummy_model_path, load_singleton=True)
@@ -355,16 +354,15 @@
     """Test singleton cache doesn't stop different backend models"""
 
     _, _ = setup_saved_model(MockBackend)
     # Configure backend
     with temp_config(
         {
             "module_backends": {
-                "priority": [backend_types.MOCK],
-                "configs": {"mock": {}},
+                "load_priority": [{"type": backend_types.MOCK}],
             }
         }
     ):
         configure()
 
         dummy_model_path = os.path.join(TEST_DATA_PATH, DUMMY_BACKEND_MODEL_NAME)
         _ = caikit.core.load(dummy_model_path, load_singleton=True)
@@ -399,28 +397,26 @@
     """
     with temp_saved_model(NonDistributedBlock()) as model_path:
         model = caikit.core.load(model_path)
 
     assert isinstance(model, NonDistributedBlock)
 
 
-def test_no_local_if_disabled(reset_globals):
-    """Make sure that if LOCAL is disabled and a given module doesn't have any
-    registered backends, loading fails.
+def test_load_fails_on_no_supported_backend(reset_globals):
+    """Make sure if a given module doesn't have any registered backends,
+    loading fails.
     """
     _ = setup_saved_model(MockBackend)
-    # 🌶️ TODO: remove the `disable_local` flag
-    # ...if LOCAL can always be supplied in the caikit base config
     with temp_config(
         {
+            "merge_strategy": "override",
             "module_backends": {
                 "load_priority": [{"type": backend_types.MOCK}],
                 "train_priority": [],
-                "disable_local": True,
-            }
+            },
         }
     ):
         configure()
         with temp_saved_model(NonDistributedBlock()) as model_path:
             with pytest.raises(ValueError):
                 caikit.core.load(model_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `caikit-0.4.2/tests/core/test_module.py` & `caikit-0.4.3/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_module_backend_config.py` & `caikit-0.4.3/tests/core/test_module_backend_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,34 +128,14 @@
             }
         }
     ):
         with pytest.raises(ValueError):
             configure()
 
 
-def test_disabling_local_backend(reset_globals):
-    """Test that disabling local backend does not add it to priority automatically"""
-    with temp_config(
-        {
-            "module_backends": {
-                "disable_local": True,
-                "load_priority": [{"type": backend_types.MOCK}],
-                "train_priority": [{"type": backend_types.MOCK}],
-            }
-        }
-    ):
-        configure()
-        assert get_load_backend(backend_types.MOCK)
-        assert get_train_backend(backend_types.MOCK)
-        with pytest.raises(AssertionError):
-            get_load_backend(backend_types.LOCAL)
-        with pytest.raises(AssertionError):
-            get_train_backend(backend_types.LOCAL)
-
-
 def test_duplicate_config_raises(reset_globals):
     """Test that duplicate configuration of a backend raises"""
     with temp_config(
         {
             "module_backends": {
                 "load_priority": [
                     {"type": backend_types.MOCK},
```

### Comparing `caikit-0.4.2/tests/core/test_module_metadata.py` & `caikit-0.4.3/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_module_type.py` & `caikit-0.4.3/tests/core/test_module_type.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_no_write_permissions.py` & `caikit-0.4.3/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/test_task.py` & `caikit-0.4.3/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_compatibility.py` & `caikit-0.4.3/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_error_handler.py` & `caikit-0.4.3/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_fileio.py` & `caikit-0.4.3/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.4.3/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_serializers.py` & `caikit-0.4.3/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.4.3/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/workflows/__init__.py` & `caikit-0.4.3/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/core/workflows/test_base.py` & `caikit-0.4.3/tests/core/workflows/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 # Standard
 import os
 import tempfile
 
 # Local
-from caikit.config import get_config
 from caikit.core.workflows import workflow
 from caikit.core.workflows.base import WorkflowLoader, WorkflowSaver
 
 # pylint: disable=import-error
 from sample_lib.blocks.sample_task import SampleBlock
 from sample_lib.data_model.sample import SampleInputType, SampleTask
 from sample_lib.workflows.sample_task import SampleWorkflow
```

### Comparing `caikit-0.4.2/tests/data_model_helpers.py` & `caikit-0.4.3/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/config/config.yml` & `caikit-0.4.3/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.4.3/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_block.zip` & `caikit-0.4.3/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_block/config.yml` & `caikit-0.4.3/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.4.3/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_resource.zip` & `caikit-0.4.3/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_workflow.zip` & `caikit-0.4.3/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.4.3/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/fixtures.py` & `caikit-0.4.3/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/invalid.zip` & `caikit-0.4.3/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/linux.txt` & `caikit-0.4.3/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/primitive_party.proto` & `caikit-0.4.3/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.4.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.4.3/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.4.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.4.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.4.3/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.4.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/generated/__init__.py` & `caikit-0.4.3/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/metrics/__init__.py` & `caikit-0.4.3/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.4.3/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/model_management/__init__.py` & `caikit-0.4.3/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/model_management/test_batcher.py` & `caikit-0.4.3/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/model_management/test_model_loader.py` & `caikit-0.4.3/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/model_management/test_model_manager.py` & `caikit-0.4.3/tests/runtime/model_management/test_model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 # Standard
 from tempfile import TemporaryDirectory
 from unittest.mock import MagicMock, patch
 import os
 import shutil
 import unittest
-import uuid
 
 # Third Party
 import grpc
 
 # Local
 from caikit import get_config
 from caikit.core.blocks.base import BlockBase
@@ -84,15 +83,17 @@
                 Fixtures.get_good_model_path(), os.path.join(tempdir, "model1")
             )
             shutil.copy(
                 Fixtures.get_good_model_archive_path(),
                 os.path.join(tempdir, "model2.zip"),
             )
             ModelManager._ModelManager__instance = None
-            with temp_config({"runtime": {"local_models_dir": tempdir}}):
+            with temp_config(
+                {"runtime": {"local_models_dir": tempdir}}, merge_strategy="merge"
+            ):
                 self.model_manager = ModelManager()
 
                 self.assertEqual(len(self.model_manager.loaded_models), 2)
                 self.assertIn("model1", self.model_manager.loaded_models.keys())
                 self.assertIn("model2.zip", self.model_manager.loaded_models.keys())
                 self.assertNotIn(
                     "model-does-not-exist.zip", self.model_manager.loaded_models.keys()
```

### Comparing `caikit-0.4.2/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.4.3/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/model_management/test_training_manager.py` & `caikit-0.4.3/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.4.3/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/test_create_service.py` & `caikit-0.4.3/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.4.3/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/test_primitives.py` & `caikit-0.4.3/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.4.3/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/__init__.py` & `caikit-0.4.3/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.4.3/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.4.3/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.4.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.4.3/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.4.3/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/test_grpc_server.py` & `caikit-0.4.3/tests/runtime/test_grpc_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,15 +739,16 @@
     free_high_port = RuntimeGRPCServer._find_port(50000, 60000)
     with temp_config(
         {
             "runtime": {
                 "port": free_high_port,
                 "find_available_port": False,
             }
-        }
+        },
+        merge_strategy="merge",
     ):
         with RuntimeGRPCServer(
             inference_service=sample_inference_service,
             training_service=None,
         ) as server:
             _assert_connection(grpc.insecure_channel(f"localhost:{free_high_port}"))
```

### Comparing `caikit-0.4.2/tests/runtime/test_service_factory.py` & `caikit-0.4.3/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/utils/__init__.py` & `caikit-0.4.3/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/utils/test_import_util.py` & `caikit-0.4.3/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/utils/test_servicer_util.py` & `caikit-0.4.3/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/work_management/__init__.py` & `caikit-0.4.3/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.4.3/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.4.3/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.4.3/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.4.2/tox.ini` & `caikit-0.4.3/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 skip_install = True # Skip package install since fmt doesn't need to execute code, for ⚡⚡⚡
 
 [testenv:lint]
 description = lint with pylint
 deps = pylint>=2.16.2,<3.0
 commands = pylint caikit
 
+[testenv:imports]
+description = enforce internal import rules
+deps = pydeps==1.12.3
+commands = ./scripts/check_deps.sh
+allowlist_externals = ./scripts/check_deps.sh
+skip_install = True
+
 [testenv:publish]
 description = publish wheel to pypi
 deps = flit==3.8
 passenv =
     FLIT_PASSWORD
 setenv =
     FLIT_USERNAME = __token__
```

### Comparing `caikit-0.4.2/PKG-INFO` & `caikit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.4.2
+Version: 0.4.3
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.16.0
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
-Requires-Dist: munch>=2.5.0,<3.0
+Requires-Dist: munch>=2.5.0,<4.0
 Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: prometheus_client>=0.12.0,<1.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
```

