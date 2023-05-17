# Comparing `tmp/rime_sdk-2.1.0rc2.tar.gz` & `tmp/rime_sdk-2.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.1.0rc2.tar", last modified: Mon May  8 22:34:21 2023, max compression
+gzip compressed data, was "rime_sdk-2.1.0rc3.tar", last modified: Wed May 17 05:16:26 2023, max compression
```

## Comparing `rime_sdk-2.1.0rc2.tar` & `rime_sdk-2.1.0rc3.tar`

### file list

```diff
@@ -1,477 +1,487 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.382819 rime_sdk-2.1.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 22:34:21.382819 rime_sdk-2.1.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.298816 rime_sdk-2.1.0rc2/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60447 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.298816 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24295 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.302816 rime_sdk-2.1.0rc2/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    59344 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24987 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.302816 rime_sdk-2.1.0rc2/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.302816 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    45262 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.306816 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54931 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.382819 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43323 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/tags_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-05-08 22:34:17.000000 rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:34:21.298816 rime_sdk-2.1.0rc2/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31362 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-08 22:34:21.000000 rime_sdk-2.1.0rc2/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:34:21.382819 rime_sdk-2.1.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 22:33:37.000000 rime_sdk-2.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.863933 rime_sdk-2.1.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 05:16:26.859933 rime_sdk-2.1.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60633 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24471 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61023 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.779933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    46345 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.783933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28249 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26924 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64351 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.859933 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    44319 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11045 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/tags_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-17 05:16:22.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-05-17 05:16:23.000000 rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:16:26.775933 rime_sdk-2.1.0rc3/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32082 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 05:16:26.000000 rime_sdk-2.1.0rc3/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:16:26.863933 rime_sdk-2.1.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-17 05:15:36.000000 rime_sdk-2.1.0rc3/setup.py
```

### Comparing `rime_sdk-2.1.0rc2/LICENSE` & `rime_sdk-2.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/PKG-INFO` & `rime_sdk-2.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc2/README.md` & `rime_sdk-2.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/__init__.py` & `rime_sdk-2.1.0rc3/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/client.py` & `rime_sdk-2.1.0rc3/rime_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,30 +387,32 @@
             if general_access_role != "ACTOR_ROLE_NONE":
                 role_pairs = [
                     RimeParentRoleSubjectRolePair(
                         parent_role=RimeActorRole.ADMIN,
                         subject_role=general_access_role,
                     ),
                     RimeParentRoleSubjectRolePair(
-                        parent_role=RimeActorRole.VP, subject_role=general_access_role,
+                        parent_role=RimeActorRole.VP,
+                        subject_role=general_access_role,
                     ),
                     RimeParentRoleSubjectRolePair(
                         parent_role=RimeActorRole.USER,
                         subject_role=general_access_role,
                     ),
                     # Workspace viewers can receive only a viewer role through
                     # general access as per the RBAC spec.
                     RimeParentRoleSubjectRolePair(
                         parent_role=RimeActorRole.VIEWER,
                         subject_role=RimeActorRole.VIEWER,
                     ),
                 ]
                 workspace_role_body = RoleWorkspaceBody(role_pairs=role_pairs)
                 api.project_service_update_workspace_roles_for_project(
-                    project_id_uuid=response.project.id.uuid, body=workspace_role_body,
+                    project_id_uuid=response.project.id.uuid,
+                    body=workspace_role_body,
                 )
             return Project(self._api_client, response.project.id.uuid)
 
     def get_project(self, project_id: str) -> Project:
         """Get Project by ID.
 
         Args:
@@ -626,15 +628,16 @@
         except ApiException as e:
             if e.status == HTTPStatus.NOT_FOUND:
                 raise ValueError(f"Docker image with name {name} does not exist.")
             raise ValueError(e.reason) from None
 
     @staticmethod
     def pip_requirement(
-        name: str, version_specifier: Optional[str] = None,
+        name: str,
+        version_specifier: Optional[str] = None,
     ) -> ManagedImagePipRequirement:
         """Construct a PipRequirement object for use in ``create_managed_image()``."""
         if not isinstance(name, str) or (
             version_specifier is not None and not isinstance(version_specifier, str)
         ):
             raise ValueError(
                 (
@@ -648,15 +651,16 @@
         res = ManagedImagePipRequirement(name=name)
         if version_specifier is not None:
             res.version_specifier = version_specifier
         return res
 
     @staticmethod
     def os_requirement(
-        name: str, version_specifier: Optional[str] = None,
+        name: str,
+        version_specifier: Optional[str] = None,
     ) -> ManagedImagePackageRequirement:
         """Construct a PackageRequirement object for ``create_managed_image()``."""
         if (
             not isinstance(name, str)
             or (
                 version_specifier is not None and not isinstance(version_specifier, str)
             )
@@ -678,15 +682,16 @@
         )
         if version_specifier is not None:
             res.version_specifier = version_specifier
         return res
 
     @staticmethod
     def pip_library_filter(
-        name: str, fixed_version: Optional[str] = None,
+        name: str,
+        fixed_version: Optional[str] = None,
     ) -> ListImagesRequestPipLibraryFilter:
         """Construct a PipLibraryFilter object for use in ``list_managed_images()``."""
         if not isinstance(name, str) or (
             fixed_version is not None and not isinstance(fixed_version, str)
         ):
             raise ValueError(
                 (
@@ -761,15 +766,16 @@
 
         # Iterate through the pages of images and break at the last page.
         api = swagger_client.ImageRegistryApi(self._api_client)
         page_token = ""
         while True:
             if page_token == "":
                 body = RimeListImagesRequest(
-                    pip_libraries=pip_library_filters, page_size=20,
+                    pip_libraries=pip_library_filters,
+                    page_size=20,
                 )
             else:
                 body = RimeListImagesRequest(page_token=page_token, page_size=20)
             with RESTErrorHandler():
                 # This function hits the additional REST binding on the RPC endpoint.
                 # The method sends a POST request instead of a GET since it is
                 # the only way to encode multiple custom messages (pip_libraries).
@@ -780,15 +786,17 @@
             # If we've reached the last page token
             if page_token == res.next_page_token:
                 break
 
             # Move to the next page
             page_token = res.next_page_token
 
-    def list_agents(self,) -> Iterator[Dict]:
+    def list_agents(
+        self,
+    ) -> Iterator[Dict]:
         """List all Agents available to the user.
 
         Returns:
             Iterator[Dict]:
                 An iterator of dictionaries, each dictionary represents a single Agent.
 
         Raises:
@@ -826,15 +834,17 @@
             # If we've reached the last page token
             if not res.has_more:
                 break
 
             # Move to the next page
             page_token = res.next_page_token
 
-    def list_projects(self,) -> Iterator[Project]:
+    def list_projects(
+        self,
+    ) -> Iterator[Project]:
         """List all Projects.
 
         Returns:
             Iterator[Project]:
                 An iterator of Projects.
 
         Raises:
@@ -964,15 +974,16 @@
                 experimental_fields=exp_fields if exp_fields else None,
             )
             Client._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_stress_test(
-                body=req, project_id_uuid=project_id,
+                body=req,
+                project_id_uuid=project_id,
             ).job
         return Job(self._api_client, job.job_id)
 
     def get_test_run(self, test_run_id: str) -> TestRun:
         """Get a TestRun object with the specified test_run_id.
 
         Checks to see if the test_run_id exists, then returns TestRun object.
@@ -1255,15 +1266,17 @@
         if upload_path is not None and upload_path == "":
             raise ValueError("specified upload_path must not be an empty string")
         if isinstance(dir_path, str):
             dir_path = Path(dir_path)
         with RESTErrorHandler():
             fum = FileUploadModule(self._api_client)
             return fum.upload_model_directory(
-                dir_path, upload_hidden=upload_hidden, upload_path=upload_path,
+                dir_path,
+                upload_hidden=upload_hidden,
+                upload_path=upload_path,
             )
 
     def list_uploaded_file_urls(self) -> Iterator[str]:
         """Return an iterator of file paths that have been uploaded using ``client.upload_file``.
 
         Returns:
             Iterator[str]:
@@ -1408,15 +1421,17 @@
             )
 
         if cpu_request_millicores is not None and cpu_request_millicores <= 0:
             raise ValueError(
                 "The requested number of millicores of CPU must be positive"
             )
         model_info = model_info_from_dict(model_file_info)
-        req = RimeStartFileScanRequest(file_info=model_info,)
+        req = RimeStartFileScanRequest(
+            file_info=model_info,
+        )
 
         req.run_time_info = RuntimeinfoRunTimeInfo()
         if cpu_request_millicores:
             req.run_time_info.resource_request.cpu_request_millicores = (
                 cpu_request_millicores
             )
         if ram_request_megabytes:
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/data_collector.py` & `rime_sdk-2.1.0rc3/rime_sdk/data_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 def convert_input_to_datapoint(
     input_data: Dict,
     timestamp: Optional[datetime] = None,
     label: Optional[Union[Dict, int, float]] = None,
     query_id: Optional[Union[str, float, int]] = None,
 ) -> DatacollectorDatapointRow:
     """Convert input data to a datapoint."""
-    datapoint = DatacollectorDatapointRow(input_data=json_serialize(input_data),)
+    datapoint = DatacollectorDatapointRow(
+        input_data=json_serialize(input_data),
+    )
     if label is not None:
         datapoint.label = json_serialize(label)
     if query_id is not None:
         datapoint.query_id = json_serialize(query_id)
     if timestamp is not None:
         datapoint.timestamp = serialize_datetime_to_proto_timestamp(timestamp)
     return datapoint
@@ -114,15 +116,16 @@
             str:
                 The ID of the registered data stream.
         """
         req = DatastreamProjectIdUuidBody(project_id=RimeUUID(self._project_id))
         with RESTErrorHandler():
             api = swagger_client.DataCollectorApi(self._api_client)
             res = api.data_collector_register_data_stream(
-                body=req, project_id_uuid=self._project_id,
+                body=req,
+                project_id_uuid=self._project_id,
             )
         return res.data_stream_id.uuid
 
     def _upload_datapoints_with_buffer(
         self, data_stream_id: str, datapoints: Iterator[DatacollectorDatapointRow]
     ) -> List[str]:
         """Upload a list of Data Collector datapoints, buffering message size."""
@@ -143,26 +146,28 @@
                 if bytes_counter + sys.getsizeof(datapoint) > GRPC_MAX_BYTES_SIZE:
                     req = DataDataStreamIdUuidBody(
                         data_stream_id=RimeUUID(data_stream_id),
                         datapoints=datapoint_list,
                     )
                     with RESTErrorHandler():
                         resp = api.data_collector_store_datapoints(
-                            data_stream_id_uuid=data_stream_id, body=req,
+                            data_stream_id_uuid=data_stream_id,
+                            body=req,
                         )
                         datapoint_ids.extend(resp.datapoint_ids)
                     datapoint_list = []
                     bytes_counter = 0
 
                 datapoint_list.append(datapoint)
                 bytes_counter += sys.getsizeof(datapoint)
             # Upload remaining datapoints
             if len(datapoint_list) > 0:
                 req = DataDataStreamIdUuidBody(
-                    data_stream_id=RimeUUID(data_stream_id), datapoints=datapoint_list,
+                    data_stream_id=RimeUUID(data_stream_id),
+                    datapoints=datapoint_list,
                 )
                 with RESTErrorHandler():
                     resp = api.data_collector_store_datapoints(
                         data_stream_id_uuid=data_stream_id, body=req
                     )
                     datapoint_ids.extend(resp.datapoint_ids)
         return [datapoint_id.uuid for datapoint_id in datapoint_ids]
@@ -231,15 +236,20 @@
         print("Logging datapoints...")
 
         # Easier for looping through options
         it_timestamps: Iterable[Any] = timestamps or itertools.repeat(None)
         it_labels: Iterable[Any] = labels or itertools.repeat(None)
         it_queries: Iterable[Any] = query_ids or itertools.repeat(None)
 
-        data_vals = zip(inputs, it_labels, it_timestamps, it_queries,)
+        data_vals = zip(
+            inputs,
+            it_labels,
+            it_timestamps,
+            it_queries,
+        )
         datapoint_iterator = DatapointIterator(iter(data_vals))
         return self._upload_datapoints_with_buffer(data_stream_id, datapoint_iterator)
 
     def log_predictions(
         self, model_id: str, datapoint_ids: List[str], predictions: List[Dict]
     ) -> None:
         """Log predictions to the Data Collector.
@@ -288,23 +298,27 @@
                 prediction=json_serialize(prediction),
             )
             preds_list.append(pred)
             bytes_counter += sys.getsizeof(pred)
             if bytes_counter + sys.getsizeof(pred) > GRPC_MAX_BYTES_SIZE:
                 with RESTErrorHandler():
                     req = PredictionsModelIdUuidBody(
-                        model_id=RimeUUID(model_id), predictions=preds_list,
+                        model_id=RimeUUID(model_id),
+                        predictions=preds_list,
                     )
                     api.data_collector_store_predictions(
-                        body=req, model_id_uuid=model_id,
+                        body=req,
+                        model_id_uuid=model_id,
                     )
 
                 preds_list = []
                 bytes_counter = 0
         if len(preds_list) > 0:
             with RESTErrorHandler():
                 req = PredictionsModelIdUuidBody(
-                    model_id=RimeUUID(model_id), predictions=preds_list,
+                    model_id=RimeUUID(model_id),
+                    predictions=preds_list,
                 )
                 api.data_collector_store_predictions(
-                    body=req, model_id_uuid=model_id,
+                    body=req,
+                    model_id_uuid=model_id,
                 )
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/nlp_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 INPUT_TYPES = set([INPUT_PREDS_INCLUDED, INPUT_PREDS_SEPARATE, PREDS])
 
 ERROR_UNKNOWN_TASK = "Unrecognized NLP task: '{task}'. Task must be one of {tasks}"
 ERROR_UNKNOWN_INPUT = (
     "Unrecognized input type: '{input_type}'. Input type must be one of {accepted}"
 )
 
+
 # NLP Data loading methods
 def _load_data_from_file_object(file_object: IO, file_name: str) -> Iterable[dict]:
     path = Path(file_name)
     try:
         if path.suffix == ".json":
             yield from json.load(file_object)
         elif path.suffix == ".jsonl":
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.1.0rc3/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/detection_event.py` & `rime_sdk-2.1.0rc3/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/firewall.py` & `rime_sdk-2.1.0rc3/rime_sdk/firewall.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,16 @@
                 ref_data_id=ref_data_id,
                 scheduled_ct_info=scheduled_ct_info,
             ),
             mask=",".join(field_mask_list),
         )
         with RESTErrorHandler():
             resp = api.firewall_service_update_firewall(
-                firewall_firewall_id_uuid=self._firewall_id, body=req,
+                firewall_firewall_id_uuid=self._firewall_id,
+                body=req,
             )
         print(f"Firewall {self._firewall_id} updated successfully.")
         return resp
 
     def activate_ct_scheduling(
         self,
         data_info: dict,
@@ -271,15 +272,17 @@
         }
         return convert_dict_to_html(info)
 
     def get_link(self) -> str:
         """Return a URL to the Firewall."""
         api = swagger_client.FirewallServiceApi(self._api_client)
         with RESTErrorHandler():
-            resp = api.firewall_service_get_url(firewall_id_uuid=self._firewall_id,)
+            resp = api.firewall_service_get_url(
+                firewall_id_uuid=self._firewall_id,
+            )
         return resp.url.url
 
     def get_bin_size(self) -> timedelta:
         """Return the bin size of this Firewall."""
         firewall = self._get_firewall()
         return rest_to_timedelta(firewall.bin_size)
 
@@ -329,15 +332,17 @@
 
     def _get_firewall(self) -> FirewallFirewall:
         api = swagger_client.FirewallServiceApi(self._api_client)
         with RESTErrorHandler():
             res = api.firewall_service_get_firewall(firewall_id_uuid=self._firewall_id)
         return res.firewall
 
-    def get_events_df(self,) -> pd.DataFrame:
+    def get_events_df(
+        self,
+    ) -> pd.DataFrame:
         """Get a dataframe of Detected Events for the given Firewall.
 
         Monitors detect Events when degradations occur.
         For example, a Monitor for the metric "Accuracy" will detect an Event
         when the value of the model performance metric drops below a threshold.
         """
         # TODO [Wombat]: allow user to specify a time interval to query over.
@@ -441,15 +446,16 @@
             else:
                 kwargs["first_page_req_included_monitor_types"] = swagger_monitor_types
                 kwargs[
                     "first_page_req_included_risk_category_types"
                 ] = swagger_risk_types
             with RESTErrorHandler():
                 res = api.monitor_service_list_monitors(
-                    firewall_id_uuid=self._firewall_id, **kwargs,
+                    firewall_id_uuid=self._firewall_id,
+                    **kwargs,
                 )
             for monitor in res.monitors:
                 yield Monitor(
                     self._api_client, monitor.id.uuid, self._firewall_id, project_id
                 )
             next_page_token = res.next_page_token
             has_more = res.has_more
@@ -540,23 +546,28 @@
                     random_seed=random_seed,
                 ),
             ),
             override_existing_bins=override_existing_bins,
             experimental_fields=exp_fields if exp_fields else None,
         )
         if custom_image:
-            req.test_run_incremental_config.run_time_info.custom_image = RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
-                custom_image=custom_image
+            req.test_run_incremental_config.run_time_info.custom_image = (
+                RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
+                    custom_image=custom_image
+                )
             )
         if rime_managed_image:
-            req.test_run_incremental_config.run_time_info.custom_image = RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
-                managed_image_name=rime_managed_image
+            req.test_run_incremental_config.run_time_info.custom_image = (
+                RuntimeinfoCustomImageType(  # pylint: disable=line-too-long
+                    managed_image_name=rime_managed_image
+                )
             )
         with RESTErrorHandler():
             Firewall._throttler.throttle(  # pylint: disable=W0212
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_continuous_test(
-                body=req, firewall_id_uuid=self._firewall_id,
+                body=req,
+                firewall_id_uuid=self._firewall_id,
             ).job
         return ContinuousTestJob(self._api_client, job.job_id)
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/image_builder.py` & `rime_sdk-2.1.0rc3/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/config_parser.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/config_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 import functools
 import inspect
 import json
 from copy import deepcopy
 from typing import Any, Callable, Optional, Set, Tuple, Union, cast
 
 from rime_sdk.swagger.swagger_client.models import (
-    DataInfoParamsFeatureIntersection,
-    DataInfoParamsRankingInfo,
-    ModelHuggingFaceModelInfo,
-    ModelModelInfo,
-    ModelModelPathInfo,
+    DataParamsFeatureIntersection,
+    DataParamsRankingInfo,
+    RegistryConnectionInfo,
+    RegistryDataCollectorInfo,
+    RegistryDataFileInfo,
+    RegistryDataLoadingInfo,
+    RegistryDataParams,
+    RegistryDeltaLakeInfo,
+    RegistryHuggingFaceDataInfo,
+    RegistryHuggingFaceModelInfo,
+    RegistryModelInfo,
+    RegistryModelPathInfo,
+    RegistryPredictionParams,
+    RegistryPredInfo,
     RimeUUID,
-    TestrunConnectionInfo,
-    TestrunDataCollectorInfo,
-    TestrunDataFileInfo,
-    TestrunDataInfoParams,
-    TestrunDataLoadingInfo,
-    TestrunDeltaLakeInfo,
-    TestrunHuggingFaceDataInfo,
-    TestrunPredictionParams,
-    TestrunPredInfo,
-    TestrunSingleDataInfo,
+    SchemaregistryDataInfo,
 )
 
 DEFAULT_DO_SAMPLING = True
 CONNECTION_INFO_TYPE_SWAGGER = Union[
-    TestrunDataFileInfo,
-    TestrunDataLoadingInfo,
-    TestrunDataCollectorInfo,
-    TestrunDeltaLakeInfo,
-    TestrunHuggingFaceDataInfo,
+    RegistryDataFileInfo,
+    RegistryDataLoadingInfo,
+    RegistryDataCollectorInfo,
+    RegistryDeltaLakeInfo,
+    RegistryHuggingFaceDataInfo,
 ]
 VALID_CONNECTION_TYPES = [
     "data_file",
     "data_loading",
     "data_collector",
     "delta_lake",
     "hugging_face",
@@ -67,37 +67,37 @@
 # NOTE: whenever changing any of convert_single_pred_info_to_swagger,
 # convert_single_data_info_to_swagger, convert_model_info_to_swagger, or any of their
 # helper functions, be sure to copy those changes over to rime/core/config_parser.py.
 # This is needed for the mock registry used in rime-engine ete tests.
 @validate_types
 def convert_pred_params_to_swagger(
     pred_params: dict,
-) -> Optional[TestrunPredictionParams]:
+) -> Optional[RegistryPredictionParams]:
     """Convert prediction params dictionary to swagger."""
     _config = deepcopy(pred_params)
-    proto_names = TestrunPredictionParams.swagger_types
+    proto_names = RegistryPredictionParams.swagger_types
     param_config = {
         name: _config.pop(name) for name in proto_names if name in pred_params
     }
     if len(param_config) == 0:
         return None
     if _config:
         raise ValueError(
             f"Unknown prediction params: {list(_config)}"
             f"\nExpected: {list(proto_names)}"
         )
-    return TestrunPredictionParams(**param_config)
+    return RegistryPredictionParams(**param_config)
 
 
 @validate_types
 def convert_data_params_to_swagger(
     data_params: dict,
-) -> Optional[TestrunDataInfoParams]:
+) -> Optional[RegistryDataParams]:
     """Convert data params dictionary to swagger."""
-    field_names = TestrunDataInfoParams.swagger_types
+    field_names = RegistryDataParams.swagger_types
     _config = deepcopy(data_params)
     param_config = {
         name: _config.pop(name) for name in field_names if name in data_params
     }
     if "sample" not in param_config:
         param_config["sample"] = DEFAULT_DO_SAMPLING
     if len(param_config) == 0:
@@ -107,46 +107,46 @@
             "Found parameters in the data_params config that do"
             f" not belong: {list(_config)}"
             f"\nExpected: {list(field_names)}"
         )
     if "loading_kwargs" in param_config and param_config["loading_kwargs"] is not None:
         param_config["loading_kwargs"] = json.dumps(param_config["loading_kwargs"])
     if "ranking_info" in param_config and param_config["ranking_info"] is not None:
-        param_config["ranking_info"] = DataInfoParamsRankingInfo(
+        param_config["ranking_info"] = DataParamsRankingInfo(
             **param_config["ranking_info"]
         )
     if "intersections" in param_config and param_config["intersections"] is not None:
         intersections = param_config["intersections"]
         param_config["intersections"] = [
-            DataInfoParamsFeatureIntersection(features=i.get("features", []))
+            DataParamsFeatureIntersection(features=i.get("features", []))
             for i in intersections
         ]
     for param in ["text_features", "image_features"]:
         unstructured_feats = param_config.get(param)
         if unstructured_feats is not None and not isinstance(unstructured_feats, list):
             raise ValueError(
                 f"`{param}` must be type `List[str]`. Got '{unstructured_feats}'."
             )
-    return TestrunDataInfoParams(**param_config)
+    return RegistryDataParams(**param_config)
 
 
 @validate_types
 def _mutate_data_file_conn_info_to_swag(
     connection_info: dict, path: str
-) -> TestrunDataFileInfo:
+) -> RegistryDataFileInfo:
     """Process data file connection info into a connection swagger."""
     required_keys = {"path"}
     _check_required_keys_exist(connection_info, required_keys, path)
-    return TestrunDataFileInfo(path=connection_info.pop("path"))
+    return RegistryDataFileInfo(path=connection_info.pop("path"))
 
 
 @validate_types
 def _mutate_data_loader_conn_info_to_swag(
     connection_info: dict, path: str
-) -> TestrunDataLoadingInfo:
+) -> RegistryDataLoadingInfo:
     """Process data loader connection info into a connection swagger."""
     required_keys = {"path", "load_func_name"}
     _check_required_keys_exist(connection_info, required_keys, path)
     loader_kwargs_json = ""
     if "loader_kwargs" in connection_info and "loader_kwargs_json" in connection_info:
         raise ValueError(
             "Got both loader_kwargs and loader_kwargs_json, "
@@ -160,50 +160,50 @@
     elif "loader_kwargs_json" in connection_info:
         # This can be None, but we don't want to set, so check first.
         _val = connection_info.pop("loader_kwargs_json")
         if _val is not None:
             loader_kwargs_json = _val
     else:
         pass
-    return TestrunDataLoadingInfo(
+    return RegistryDataLoadingInfo(
         path=connection_info.pop("path"),
         load_func_name=connection_info.pop("load_func_name"),
         loader_kwargs_json=loader_kwargs_json,
     )
 
 
 @validate_types
 def _mutate_data_collector_conn_info_to_swag(
     connection_info: dict, path: str
-) -> TestrunDataCollectorInfo:
+) -> RegistryDataCollectorInfo:
     """Process data collector connection info into a connection info swagger."""
     required_keys = {"data_stream_id"}
     _check_required_keys_exist(connection_info, required_keys, path)
     data_stream_id = RimeUUID(connection_info.pop("data_stream_id"))
-    return TestrunDataCollectorInfo(data_stream_id=data_stream_id)
+    return RegistryDataCollectorInfo(data_stream_id=data_stream_id)
 
 
 @validate_types
 def _mutate_delta_lake_conn_info_to_swag(
     connection_info: dict, path: str
-) -> TestrunDeltaLakeInfo:
+) -> RegistryDeltaLakeInfo:
     """Process delta lake connection info into a connection info swagger."""
     required_keys = {"table_name"}
     _check_required_keys_exist(connection_info, required_keys, path)
-    return TestrunDeltaLakeInfo(table_name=connection_info.pop("table_name"))
+    return RegistryDeltaLakeInfo(table_name=connection_info.pop("table_name"))
 
 
 @validate_types
 def _mutate_huggingface_conn_info_to_swag(
     connection_info: dict, path: str
-) -> TestrunHuggingFaceDataInfo:
+) -> RegistryHuggingFaceDataInfo:
     """Process huggingface connection info into a connection info swagger."""
     required_keys = {"dataset_uri", "split_name"}
     _check_required_keys_exist(connection_info, required_keys, path)
-    return TestrunHuggingFaceDataInfo(
+    return RegistryHuggingFaceDataInfo(
         dataset_uri=connection_info.pop("dataset_uri"),
         split_name=connection_info.pop("split_name", None),
         loading_params_json=json.dumps(connection_info.pop("loading_params", None)),
     )
 
 
 def _check_required_keys_exist(
@@ -241,31 +241,33 @@
             f" that do not belong: {list(_config)}."
             f" Expected parameters: {expected_field_names}."
         )
     return cast(CONNECTION_INFO_TYPE_SWAGGER, swagger)
 
 
 @validate_types
-def convert_single_pred_info_to_swagger(pred_config: dict) -> Optional[TestrunPredInfo]:
+def convert_single_pred_info_to_swagger(
+    pred_config: dict,
+) -> Optional[RegistryPredInfo]:
     """Convert a dictionary to single pred info swagger message."""
     _config = deepcopy(pred_config)
     if "connection_info" not in _config:
         raise ValueError(
             "Missing required key 'connection_info' in prediction info config."
             f"\nGot: {list(_config)}."
         )
     connection_info = _config.pop("connection_info")
     pred_params_dict = _config.pop("pred_params", {})
     pred_params = convert_pred_params_to_swagger(pred_params_dict)
     connection_swagger, field = _process_connection_info_dict_swagger(
         connection_info, "pred_config"
     )
-    connection_info = TestrunConnectionInfo()
+    connection_info = RegistryConnectionInfo()
     setattr(connection_info, field, connection_swagger)
-    return TestrunPredInfo(pred_params=pred_params, connection_info=connection_info)
+    return RegistryPredInfo(pred_params=pred_params, connection_info=connection_info)
 
 
 @validate_types
 def _process_connection_info_dict_swagger(
     connection_info: dict, path: str
 ) -> Tuple[CONNECTION_INFO_TYPE_SWAGGER, str]:
     """Process the connection info dictionary."""
@@ -288,16 +290,16 @@
     connection_swagger = process_connection_info_to_swagger(
         connection_info, config_type, _path
     )
     return connection_swagger, config_type
 
 
 @validate_types
-def convert_single_data_info_to_swagger(data_config: dict) -> TestrunSingleDataInfo:
-    """Convert a dictionary to a `SingleDataInfo` Swagger message."""
+def convert_single_data_info_to_swagger(data_config: dict) -> SchemaregistryDataInfo:
+    """Convert a dictionary to a `DataInfo` Swagger message."""
     _config = deepcopy(data_config)
     if "connection_info" not in _config:
         raise ValueError(
             "Missing required key `connection_info` in data info config."
             f"\nGot: {list(_config)}"
         )
     connection_info = _config.pop("connection_info")
@@ -307,59 +309,60 @@
     )
     params_dict = _config.pop("data_params", {})
     data_params = convert_data_params_to_swagger(params_dict)
     if _config:
         raise ValueError(
             f"Found parameters in the data info config for {path} that do not"
             f" belong: {list(_config)}."
-            f" Expected parameters: {list(TestrunSingleDataInfo.swagger_types)}."
+            f" Expected parameters: {list(SchemaregistryDataInfo.swagger_types)}."
         )
-    connection_info = TestrunConnectionInfo()
+    connection_info = RegistryConnectionInfo()
     setattr(connection_info, field, connection_swagger)
-    return TestrunSingleDataInfo(
-        data_params=data_params, connection_info=connection_info,
+    return SchemaregistryDataInfo(
+        data_params=data_params,
+        connection_info=connection_info,
     )
 
 
 @validate_types
-def convert_model_info_to_swagger(model_config: dict) -> ModelModelInfo:
+def convert_model_info_to_swagger(model_config: dict) -> RegistryModelInfo:
     """Convert a dictionary to model info swagger message."""
     _config = deepcopy(model_config)
-    valid_model_infos = list(ModelModelInfo.swagger_types)
+    valid_model_infos = list(RegistryModelInfo.swagger_types)
     if len(_config) != 1:
         raise ValueError(
             "Must specify exactly one valid model_info type in config. "
             f"Valid model_info types are: {valid_model_infos}. "
             f"Got: {list(_config)}."
         )
     model_type, model_info = next(iter(_config.items()))
     if not isinstance(model_info, dict):
         raise ValueError(
             f"model_info must be a dictionary. Got: {type(model_info)}."
             f"\nFull config: {model_config}"
         )
     try:
         if model_type == "model_path":
-            model_info_swagger = ModelModelInfo(
-                model_path=ModelModelPathInfo(path=model_info.pop("path"))
+            model_info_swagger = RegistryModelInfo(
+                model_path=RegistryModelPathInfo(path=model_info.pop("path"))
             )
         elif model_type == "hugging_face":
             model_uri = model_info.pop("model_uri")
             config_d = model_info.pop("kwargs", {})
             if isinstance(config_d, dict):
                 config_str = json.dumps(config_d)
             elif isinstance(config_d, str):
                 config_str = config_d
             else:
                 raise ValueError(
                     f"Invalid type for `kwargs` in hugging_face model_info."
                     f" Expected `dict` or json `str`. Got: {type(config_d)}"
                 )
-            model_info_swagger = ModelModelInfo(
-                hugging_face=ModelHuggingFaceModelInfo(
+            model_info_swagger = RegistryModelInfo(
+                hugging_face=RegistryHuggingFaceModelInfo(
                     model_uri=model_uri, kwargs=config_str
                 )
             )
         else:
             raise ValueError(
                 f"model_info type in config should be one of {valid_model_infos}. "
                 f"Got {model_type}."
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/constants.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/decorators.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/file_upload.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/file_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
     def __init__(self, api_client: ApiClient):
         """Create a FileUploadModule for the `file_upload_client`."""
         self._api_client = api_client
         self._file_upload_client = FileUploadApi(self._api_client)
 
     def upload_dataset_file(
-        self, file_path: Path, upload_path: Optional[str] = None,
+        self,
+        file_path: Path,
+        upload_path: Optional[str] = None,
     ) -> str:
         """Upload dataset file ``file_path`` to RIME's blobstore via a FileUploadStub.
 
         The uploaded file is placed within the blobstore using its file name.
 
         Args:
             file_path: Path
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,16 @@
         set(all_test_run_columns).difference(set(default_test_run_columns))
     )
     ordered_index = pd.Index(default_test_run_columns + sorted(non_default_cols))
     return full_df.reindex(ordered_index, axis=1)
 
 
 def parse_test_batch_result(
-    raw_result: TestrunresultTestBatchResult, unpack_metrics: bool = False,
+    raw_result: TestrunresultTestBatchResult,
+    unpack_metrics: bool = False,
 ) -> pd.Series:
     """Parse test batch result into a series."""
     result_dict = raw_result.to_dict()
     del result_dict["metrics"]
     if unpack_metrics:
         _add_metric_cols(result_dict, raw_result)
 
@@ -222,30 +223,33 @@
                         if getter is not None:
                             metric_value = getter
                             break
                 result_dict[f"{category_string}:{metric.metric}"] = metric_value
 
 
 def parse_summary_test_result(
-    raw_result: RimeCategoryTestResult, unpack_metrics: bool = False,
+    raw_result: RimeCategoryTestResult,
+    unpack_metrics: bool = False,
 ) -> dict:
     """Parse swagger summary test result to pythonic form."""
     raw_dict = raw_result.to_dict()
     for key in SUMMARY_TEST_KEYS_TO_HIDE:
         raw_dict.pop(key, None)
     if unpack_metrics:
         for metric in raw_result.category_metrics:
             raw_dict[metric.name] = metric.value
     severity_count_dict = raw_dict.pop("severity_counts")
     for key in severity_count_dict:
         raw_dict[key] = int(severity_count_dict[key])
     return raw_dict
 
 
-def parse_events_to_df(events: List[DetectionDetectionEvent],) -> pd.DataFrame:
+def parse_events_to_df(
+    events: List[DetectionDetectionEvent],
+) -> pd.DataFrame:
     """Parse a list of Detection Events to a pandas DateFrame."""
     event_dicts = [event.to_dict() for event in events]
     df = pd.json_normalize(event_dicts, sep=DF_FLATTEN_SEPARATOR)
 
     intersect_df = df[df.columns.intersection(EVENT_COLUMNS_TO_SHOW)]
     intersect_df = intersect_df.rename({"event_object_id": "monitor_id"}, axis=1)
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/throttle_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,13 +57,13 @@
         # contribution of this delay is
         #    T = DI * sum_{t=1}{N} 2^-t
         #      < DI * sum_{t=1}{inf} 2^-t
         #      = DI
         # where DI is the desired interval and N is the desired events per epoch.
         # Thus, there will be at most 1 unit of desired interval in delays before
         # full throttling is applied.
-        time.sleep(self._desired_interval * 2.0 ** excess_events)
+        time.sleep(self._desired_interval * 2.0**excess_events)
 
         # Record the latest event in the circular queue.
         self._timestamp_queue[self._timestamp_index] = time.time()
         self._timestamp_index = (self._timestamp_index + 1) % len(self._timestamp_queue)
         return throttled
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/internal/utils.py` & `rime_sdk-2.1.0rc3/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/job.py` & `rime_sdk-2.1.0rc3/rime_sdk/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,16 @@
         with RESTErrorHandler():
             job: RimeJobMetadata = api.job_reader_get_job(
                 job_id=self._job_id, view=RimeJobView.FULL
             ).job
         if verbose:
             print(
                 "Job '{}' started at {}".format(
-                    job.job_id, datetime.fromtimestamp(job.creation_time.timestamp()),
+                    job.job_id,
+                    datetime.fromtimestamp(job.creation_time.timestamp()),
                 )
             )
 
         # Do not repeat if the job is finished or blocking is disabled.
         while wait_until_finish and job.status not in (
             StatedbJobStatus.SUCCEEDED,
             StatedbJobStatus.FAILED,
@@ -460,7 +461,17 @@
 
     _job_type = RimeJobType.FILE_SCAN
 
     def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
         """Pretty print the progress of the test run."""
         # TODO: find a good way to pretty print the progress of a FileScanJob
         return None
+
+
+class CrossPlaneTask(BaseJob):
+    """This object provides an interface for monitoring a CrossPlaneTasks in the RI platform."""
+
+    _job_type = RimeJobType.CROSS_PLANE_TASK
+
+    def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
+        """Pretty print the progress of the job."""
+        return None
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/monitor.py` & `rime_sdk-2.1.0rc3/rime_sdk/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     """An interface to a Monitor object.
 
     Monitors track important model events over time including metric degradations or
     attacks on your model.
     """
 
     def __init__(
-        self, api_client: ApiClient, monitor_id: str, firewall_id: str, project_id: str,
+        self,
+        api_client: ApiClient,
+        monitor_id: str,
+        firewall_id: str,
+        project_id: str,
     ) -> None:
         """Initialize a new Monitor object.
 
         Args:
             api_client: ApiClient
                 The client used to query for the up-to-date status of the Monitor.
             monitor_id: str
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/project.py` & `rime_sdk-2.1.0rc3/rime_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Library defining the interface to a Project."""
 import json
-from datetime import timedelta
+from datetime import datetime, timedelta
 from http import HTTPStatus
 from typing import Any, Dict, Iterator, List, NamedTuple, Optional
 
+from deprecated import deprecated
 from google.protobuf.field_mask_pb2 import FieldMask
 from google.protobuf.json_format import MessageToDict
 
 from rime_sdk.data_collector import DataCollector
 from rime_sdk.firewall import Firewall
 from rime_sdk.internal.config_parser import (
     _get_individual_tests_config_swagger,
@@ -18,15 +19,15 @@
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.swagger_utils import parse_str_to_uuid, timedelta_to_rest
 from rime_sdk.internal.utils import (
     convert_dict_to_html,
     get_swagger_field_mask,
     make_link,
 )
-from rime_sdk.job import Job
+from rime_sdk.job import CrossPlaneTask, Job
 from rime_sdk.registry import Registry
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
     CreateFirewallRequestScheduledCTParameters,
     RimeCreateFirewallRequest,
     RimeUUID,
@@ -47,14 +48,23 @@
     RimeJobType,
     RimeLicenseLimit,
     RimeLimitStatusStatus,
     RimeListNotificationsResponse,
     SchemanotificationConfig,
     StatedbJobStatus,
 )
+from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import (
+    RimeGetFooTaskStatusResponse,
+)
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import (
+    RimeStartFooTaskRequest,
+)
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import (
+    RimeStartFooTaskResponse,
+)
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import (
     TestrunProfilingConfig,
 )
 from rime_sdk.swagger.swagger_client.rest import ApiException
 from rime_sdk.test_run import TestRun
 
 NOTIFICATION_TYPE_JOB_ACTION_STR: str = "Job_Action"
@@ -190,14 +200,41 @@
                 A ``Project`` object.
         """
         api = swagger_client.ProjectServiceApi(self._api_client)
         with RESTErrorHandler():
             response = api.project_service_get_project(self._project_id)
             return response.project.project
 
+    @deprecated
+    def foo_example_cross_plane_task(self) -> Optional[datetime]:
+        """Do the Foo toy example for the given project.
+
+        This makes a CrossPlane call to the DataPlane and returns the current
+        time on the agent side.
+        This may fail at certain times :)
+        """
+        # TODO(RAT-1738): remove this method, only for internal testing.
+        api = swagger_client.FooXPInterfaceApi(self._api_client)
+        with RESTErrorHandler():
+            req = RimeStartFooTaskRequest(project_id=RimeUUID(self._project_id))
+            res: RimeStartFooTaskResponse = api.foo_xp_interface_start_foo_task(req)
+            job_id: str = res.job_id.uuid
+            job = CrossPlaneTask(self._api_client, job_id)
+            status = job.get_status(
+                verbose=True, wait_until_finish=True, poll_rate_sec=1
+            )
+
+            if status.get("status") == StatedbJobStatus.SUCCEEDED:
+                get_res: RimeGetFooTaskStatusResponse = (
+                    api.foo_xp_interface_get_foo_task_status(job_id)
+                )
+                return get_res.res.receive_time
+
+            return None
+
     @property
     def info(self) -> ProjectInfo:
         """Return description, use case and ethical consideration of the Project."""
         project = self._get_project()
         return ProjectInfo(
             self._project_id,
             project.name,
@@ -226,15 +263,16 @@
 
     @property
     def description(self) -> str:
         """Return the description of this Project."""
         return self.info.description
 
     def list_stress_testing_jobs(
-        self, status_filters: Optional[List[str]] = None,
+        self,
+        status_filters: Optional[List[str]] = None,
     ) -> Iterator[Job]:
         """Get list of Stress Testing Jobs for the Project filtered by status.
 
         Note that this only returns jobs from the last two days, because the
         time-to-live of job objects in the cluster is set at two days.
 
         Args:
@@ -280,15 +318,17 @@
                 kwargs: Dict[str, Any] = {}
                 if page_token is None:
                     kwargs["first_page_query_selected_statuses"] = selected_statuses
                     kwargs["first_page_query_selected_types"] = selected_types
                 else:
                     kwargs["page_token"] = page_token
                 res = api.job_reader_list_jobs_for_project(
-                    project_id_uuid=self.project_id, page_size=20, **kwargs,
+                    project_id_uuid=self.project_id,
+                    page_size=20,
+                    **kwargs,
                 )
                 for job in res.jobs:
                     yield Job(self._api_client, job.job_id)
                 if not res.has_more:
                     break
                 page_token = res.next_page_token
 
@@ -591,15 +631,16 @@
                     notif_setting.webhooks.append(webhook_config)
                 with RESTErrorHandler():
                     # Note: the FieldMask object is not a Swagger model so we must
                     # serialize it to a dictionary before invoking Swagger API methods.
                     serialized_mask = MessageToDict(mask)
                     body = {"notification": notif_setting, "mask": serialized_mask}
                     api.notification_setting_update_notification(
-                        body=body, notification_id_uuid=notif_setting.id.uuid,
+                        body=body,
+                        notification_id_uuid=notif_setting.id.uuid,
                     )
                     return
         # Notification setting does not exist for the notif_type.
         req = RimeCreateNotificationRequest(
             object_type=NotificationObjectType.PROJECT,
             object_id=self.project_id,
             config=SchemanotificationConfig(),
@@ -672,15 +713,16 @@
                             # API methods.
                             serialized_mask = MessageToDict(mask)
                             body = {
                                 "notification": notif_setting,
                                 "mask": serialized_mask,
                             }
                             api.notification_setting_update_notification(
-                                body=body, notification_id_uuid=notif_setting.id.uuid,
+                                body=body,
+                                notification_id_uuid=notif_setting.id.uuid,
                             )
                         return
         notif_entry_str = ""
         if email is not None:
             notif_entry_str = "Email " + email
         elif webhook_config is not None:
             notif_entry_str = "Webhook " + webhook_config.webhook
@@ -1211,15 +1253,17 @@
             for role_pair in response.role_pairs:
                 workspace_role = "Workspace Role: " + role_pair.parent_role
                 project_role = "Project Role:" + role_pair.subject_role
                 roles_map[workspace_role] = project_role
             return roles_map
 
     def list_predictions(
-        self, model_id: Optional[str] = None, dataset_id: Optional[str] = None,
+        self,
+        model_id: Optional[str] = None,
+        dataset_id: Optional[str] = None,
     ) -> Iterator[Dict]:
         """Return a list of predictions.
 
         Args:
             model_id: Optional[str] = None
                 The ID of the model to which the prediction sets belong.
             dataset_id: Optional[str] = None
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/registry.py` & `rime_sdk-2.1.0rc3/rime_sdk/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,16 @@
                 end_time=serialize_datetime_to_proto_timestamp(ct_info["end_time"]),
                 ct_dataset_type=DatasetCTDatasetType.USER_SPECIFIED,
             )
 
         with RESTErrorHandler():
             api = swagger_client.RegistryServiceApi(self._api_client)
             res = api.registry_service_register_dataset(
-                body=req, project_id_uuid=project_id,
+                body=req,
+                project_id_uuid=project_id,
             )
 
             res = cast(RimeRegisterDatasetResponse, res)
 
         return res.dataset_id
 
     def register_model(
@@ -191,15 +192,18 @@
                         }
                     },
                     tags=[MODEL_TAG],
                     metadata={KEY: VALUE},
                     external_id=EXTERNAL_ID,
                 )
         """
-        req = ProjectIdUuidModelBody(project_id=RimeUUID(uuid=project_id), name=name,)
+        req = ProjectIdUuidModelBody(
+            project_id=RimeUUID(uuid=project_id),
+            name=name,
+        )
 
         if model_config is not None:
             # When the `model_path` key is provided to the dictionary, the value
             # must be a dictionary whose `path` value points to a python
             # file that holds a `predict_dict` or `predict_df` function.
             # When the `model_loading` key is provided to the dictionary, the value
             # must be a dictionary whose `path` value points to a python
@@ -222,15 +226,16 @@
             req.external_id = external_id
         if integration_id is not None:
             req.integration_id = RimeUUID(uuid=integration_id)
 
         with RESTErrorHandler():
             api = swagger_client.RegistryServiceApi(self._api_client)
             res = api.registry_service_register_model(
-                body=req, project_id_uuid=project_id,
+                body=req,
+                project_id_uuid=project_id,
             )
 
             res = cast(RimeRegisterModelResponse, res)
 
         return cast(RimeUUID, res.model_id).uuid
 
     def register_predictions(
@@ -435,26 +440,29 @@
         # Iterate through the pages of datasets and break at the last page.
         page_token = ""
         # pylint: disable=line-too-long
         with RESTErrorHandler():
             while True:
                 if page_token == "":
                     if model_id is not None:
-                        res: RimeListPredictionSetsResponse = api.registry_service_list_prediction_sets(
-                            project_id_uuid=project_id,
-                            first_page_req_model_id=model_id,
+                        res: RimeListPredictionSetsResponse = (
+                            api.registry_service_list_prediction_sets(
+                                project_id_uuid=project_id,
+                                first_page_req_model_id=model_id,
+                            )
                         )
                     else:
                         res = api.registry_service_list_prediction_sets(
                             project_id_uuid=project_id,
                             first_page_req_dataset_id=dataset_id,
                         )
                 else:
                     res = api.registry_service_list_prediction_sets(
-                        project_id_uuid=project_id, page_token=page_token,
+                        project_id_uuid=project_id,
+                        page_token=page_token,
                     )
                 if res.predictions is not None:
                     for prediction in res.predictions:
                         yield prediction.to_dict()
                 # Advance to the next page of predictions.
                 page_token = res.next_page_token
                 # we've reached the last page of predictions.
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
+from rime_sdk.swagger.swagger_client.api.foo_xp_interface_api import FooXPInterfaceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
 from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
 from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
 from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
 from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
 from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
 from rime_sdk.swagger.swagger_client.api.notification_setting_api import NotificationSettingApi
@@ -50,16 +51,16 @@
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
-from rime_sdk.swagger.swagger_client.models.data_info_params_feature_intersection import DataInfoParamsFeatureIntersection
-from rime_sdk.swagger.swagger_client.models.data_info_params_ranking_info import DataInfoParamsRankingInfo
+from rime_sdk.swagger.swagger_client.models.data_params_feature_intersection import DataParamsFeatureIntersection
+from rime_sdk.swagger.swagger_client.models.data_params_ranking_info import DataParamsRankingInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_column_type_info import DataProfilingColumnTypeInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_feature_relationship_info import DataProfilingFeatureRelationshipInfo
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint import DatacollectorDatapoint
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint_row import DatacollectorDatapointRow
 from rime_sdk.swagger.swagger_client.models.dataset_ct_dataset_type import DatasetCTDatasetType
 from rime_sdk.swagger.swagger_client.models.dataset_ct_info import DatasetCTInfo
 from rime_sdk.swagger.swagger_client.models.dataset_dataset import DatasetDataset
@@ -82,14 +83,17 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
+from rime_sdk.swagger.swagger_client.models.fooexample_foo_request import FooexampleFooRequest
+from rime_sdk.swagger.swagger_client.models.fooexample_foo_response import FooexampleFooResponse
+from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
@@ -111,18 +115,15 @@
 from rime_sdk.swagger.swagger_client.models.list_summary_tests_request_list_summary_tests_query import ListSummaryTestsRequestListSummaryTestsQuery
 from rime_sdk.swagger.swagger_client.models.list_test_cases_request_list_test_cases_query import ListTestCasesRequestListTestCasesQuery
 from rime_sdk.swagger.swagger_client.models.managed_image_package_requirement import ManagedImagePackageRequirement
 from rime_sdk.swagger.swagger_client.models.managed_image_package_type import ManagedImagePackageType
 from rime_sdk.swagger.swagger_client.models.managed_image_pip_library import ManagedImagePipLibrary
 from rime_sdk.swagger.swagger_client.models.managed_image_pip_requirement import ManagedImagePipRequirement
 from rime_sdk.swagger.swagger_client.models.managed_image_role_type import ManagedImageRoleType
-from rime_sdk.swagger.swagger_client.models.model_hugging_face_model_info import ModelHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.model_model import ModelModel
-from rime_sdk.swagger.swagger_client.models.model_model_info import ModelModelInfo
-from rime_sdk.swagger.swagger_client.models.model_model_path_info import ModelModelPathInfo
 from rime_sdk.swagger.swagger_client.models.modelcards_model_card_model_card_id_uuid_body import ModelcardsModelCardModelCardIdUuidBody
 from rime_sdk.swagger.swagger_client.models.monitor_aggregation import MonitorAggregation
 from rime_sdk.swagger.swagger_client.models.monitor_aggregation_type import MonitorAggregationType
 from rime_sdk.swagger.swagger_client.models.monitor_anomaly_config import MonitorAnomalyConfig
 from rime_sdk.swagger.swagger_client.models.monitor_artifact_identifier import MonitorArtifactIdentifier
 from rime_sdk.swagger.swagger_client.models.monitor_difference_from_target import MonitorDifferenceFromTarget
 from rime_sdk.swagger.swagger_client.models.monitor_excluded_transforms import MonitorExcludedTransforms
@@ -167,15 +168,27 @@
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
 from rime_sdk.swagger.swagger_client.models.rca_feature_cause import RcaFeatureCause
 from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
 from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
 from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
+from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
+from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
+from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
+from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
+from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
+from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
+from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
+from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
 from rime_sdk.swagger.swagger_client.models.registry_validity_status import RegistryValidityStatus
 from rime_sdk.swagger.swagger_client.models.registryprediction_prediction import RegistrypredictionPrediction
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
@@ -231,14 +244,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flag_jwt_response import RimeGetFeatureFlagJwtResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flags_response import RimeGetFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_firewall_response import RimeGetFirewallResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import RimeGetFooTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_image_response import RimeGetImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_integration_response import RimeGetIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_job_response import RimeGetJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_latest_logs_response import RimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_limit_status_response import RimeGetLimitStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_card_response import RimeGetModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_directory_upload_urls_response import RimeGetModelDirectoryUploadURLsResponse
@@ -256,14 +270,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
 from rime_sdk.swagger.swagger_client.models.rime_job_type import RimeJobType
 from rime_sdk.swagger.swagger_client.models.rime_job_view import RimeJobView
+from rime_sdk.swagger.swagger_client.models.rime_language import RimeLanguage
 from rime_sdk.swagger.swagger_client.models.rime_license_feature import RimeLicenseFeature
 from rime_sdk.swagger.swagger_client.models.rime_license_limit import RimeLicenseLimit
 from rime_sdk.swagger.swagger_client.models.rime_limit_status import RimeLimitStatus
 from rime_sdk.swagger.swagger_client.models.rime_limit_status_status import RimeLimitStatusStatus
 from rime_sdk.swagger.swagger_client.models.rime_list_api_tokens_response import RimeListAPITokensResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_agents_response import RimeListAgentsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
@@ -314,14 +329,17 @@
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import RimeStartFooTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import RimeStartFooTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_generative_stress_test_response import RimeStartGenerativeStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
@@ -367,42 +385,34 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
+from rime_sdk.swagger.swagger_client.models.schemaregistry_data_info import SchemaregistryDataInfo
+from rime_sdk.swagger.swagger_client.models.schematestrun_data_info import SchematestrunDataInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
-from rime_sdk.swagger.swagger_client.models.testrun_connection_info import TestrunConnectionInfo
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
-from rime_sdk.swagger.swagger_client.models.testrun_data_collector_info import TestrunDataCollectorInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_file_info import TestrunDataFileInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_info import TestrunDataInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_info_params import TestrunDataInfoParams
-from rime_sdk.swagger.swagger_client.models.testrun_data_loading_info import TestrunDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
-from rime_sdk.swagger.swagger_client.models.testrun_delta_lake_info import TestrunDeltaLakeInfo
-from rime_sdk.swagger.swagger_client.models.testrun_hugging_face_data_info import TestrunHuggingFaceDataInfo
+from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
-from rime_sdk.swagger.swagger_client.models.testrun_pred_info import TestrunPredInfo
-from rime_sdk.swagger.swagger_client.models.testrun_prediction_params import TestrunPredictionParams
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
-from rime_sdk.swagger.swagger_client.models.testrun_single_data_info import TestrunSingleDataInfo
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
+from rime_sdk.swagger.swagger_client.api.foo_xp_interface_api import FooXPInterfaceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
 from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
 from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
 from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
 from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
 from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
 from rime_sdk.swagger.swagger_client.api.notification_setting_api import NotificationSettingApi
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -320,15 +320,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def image_registry_list_images(self, **kwargs):  # noqa: E501
         """ListImages  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_list_images(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
@@ -343,15 +343,15 @@
         else:
             (data) = self.image_registry_list_images_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def image_registry_list_images_with_http_info(self, **kwargs):  # noqa: E501
         """ListImages  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_list_images_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
@@ -415,15 +415,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def image_registry_list_images2(self, body, **kwargs):  # noqa: E501
         """ListImages  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_list_images2(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeListImagesRequest body: (required)
@@ -437,15 +437,15 @@
         else:
             (data) = self.image_registry_list_images2_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
     def image_registry_list_images2_with_http_info(self, body, **kwargs):  # noqa: E501
         """ListImages  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.image_registry_list_images2_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param RimeListImagesRequest body: (required)
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def job_reader_list_jobs_for_project(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListJobsForProject  # noqa: E501
 
-        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
+        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
@@ -442,15 +442,15 @@
         else:
             (data) = self.job_reader_list_jobs_for_project_with_http_info(project_id_uuid, **kwargs)  # noqa: E501
             return data
 
     def job_reader_list_jobs_for_project_with_http_info(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListJobsForProject  # noqa: E501
 
-        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers)     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['jobs'])     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
+        Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project_with_http_info(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -230,14 +230,121 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def model_testing_start_generative_stress_test(self, body, project_id_uuid, **kwargs):  # noqa: E501
+        """StartGenerativeStressTest  # noqa: E501
+
+        Starts a Generative Stress Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_testing_start_generative_stress_test(body, project_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param GenerativestresstestsProjectIdUuidBody body: (required)
+        :param str project_id_uuid: Unique object ID. (required)
+        :return: RimeStartGenerativeStressTestResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.model_testing_start_generative_stress_test_with_http_info(body, project_id_uuid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.model_testing_start_generative_stress_test_with_http_info(body, project_id_uuid, **kwargs)  # noqa: E501
+            return data
+
+    def model_testing_start_generative_stress_test_with_http_info(self, body, project_id_uuid, **kwargs):  # noqa: E501
+        """StartGenerativeStressTest  # noqa: E501
+
+        Starts a Generative Stress Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_testing_start_generative_stress_test_with_http_info(body, project_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param GenerativestresstestsProjectIdUuidBody body: (required)
+        :param str project_id_uuid: Unique object ID. (required)
+        :return: RimeStartGenerativeStressTestResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'project_id_uuid']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method model_testing_start_generative_stress_test" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `model_testing_start_generative_stress_test`")  # noqa: E501
+        # verify the required parameter 'project_id_uuid' is set
+        if ('project_id_uuid' not in params or
+                params['project_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `project_id_uuid` when calling `model_testing_start_generative_stress_test`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'project_id_uuid' in params:
+            path_params['projectId.uuid'] = params['project_id_uuid']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/internal/generative-stress-tests/{projectId.uuid}', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeStartGenerativeStressTestResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def model_testing_start_stress_test(self, body, project_id_uuid, **kwargs):  # noqa: E501
         """StartStressTest  # noqa: E501
 
         Starts a Stress Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.model_testing_start_stress_test(body, project_id_uuid, async_req=True)
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -538,15 +538,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def results_reader_list_batch_results(self, **kwargs):  # noqa: E501
         """ListBatchResults  # noqa: E501
 
-        Returns a paginated list of batch results from a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of batch results from a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_batch_results(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str test_run_id: The ID of the Test Run associated with batch results. Specify exactly one of the pageToken field or this field.
@@ -563,15 +563,15 @@
         else:
             (data) = self.results_reader_list_batch_results_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def results_reader_list_batch_results_with_http_info(self, **kwargs):  # noqa: E501
         """ListBatchResults  # noqa: E501
 
-        Returns a paginated list of batch results from a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of batch results from a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_batch_results_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str test_run_id: The ID of the Test Run associated with batch results. Specify exactly one of the pageToken field or this field.
@@ -641,15 +641,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def results_reader_list_feature_results(self, **kwargs):  # noqa: E501
         """ListFeatureResults  # noqa: E501
 
-        List all feature results from a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all feature results from a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_feature_results(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str test_run_id: The ID of the Test Run associated with feature results. Specify exactly one of the page_token field or this field.
@@ -666,15 +666,15 @@
         else:
             (data) = self.results_reader_list_feature_results_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def results_reader_list_feature_results_with_http_info(self, **kwargs):  # noqa: E501
         """ListFeatureResults  # noqa: E501
 
-        List all feature results from a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        List all feature results from a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_feature_results_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str test_run_id: The ID of the Test Run associated with feature results. Specify exactly one of the page_token field or this field.
@@ -744,15 +744,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def results_reader_list_summary_tests(self, **kwargs):  # noqa: E501
         """ListSummaryTests  # noqa: E501
 
-        Returns a paginated list of the summary tests of a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of the summary tests of a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_summary_tests(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str query_test_run_id: The ID of the test run associated with summary tests. Specify exactly one of the page_token field or this field.
@@ -768,15 +768,15 @@
         else:
             (data) = self.results_reader_list_summary_tests_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def results_reader_list_summary_tests_with_http_info(self, **kwargs):  # noqa: E501
         """ListSummaryTests  # noqa: E501
 
-        Returns a paginated list of the summary tests of a test run.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of the summary tests of a test run.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_summary_tests_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str query_test_run_id: The ID of the test run associated with summary tests. Specify exactly one of the page_token field or this field.
@@ -843,15 +843,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def results_reader_list_test_cases(self, **kwargs):  # noqa: E501
         """ListTestCases  # noqa: E501
 
-        Returns a paginated list of the test cases in a test run. Specify a set of test types to filter the list by test types.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of the test cases in a test run. Specify a set of test types to filter the list by test types.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_cases(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str list_test_cases_query_test_run_id: Uniquely specifies a Test Run associated with test cases. Specify exactly one of the page_token field or this field.
@@ -870,15 +870,15 @@
         else:
             (data) = self.results_reader_list_test_cases_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def results_reader_list_test_cases_with_http_info(self, **kwargs):  # noqa: E501
         """ListTestCases  # noqa: E501
 
-        Returns a paginated list of the test cases in a test run. Specify a set of test types to filter the list by test types.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Returns a paginated list of the test cases in a test run. Specify a set of test types to filter the list by test types.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_cases_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str list_test_cases_query_test_run_id: Uniquely specifies a Test Run associated with test cases. Specify exactly one of the page_token field or this field.
@@ -956,15 +956,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def results_reader_list_test_runs(self, **kwargs):  # noqa: E501
         """ListTestRuns  # noqa: E501
 
-        Lists all test runs belonging to a project.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Lists all test runs belonging to a project.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_runs(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id: The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
@@ -980,15 +980,15 @@
         else:
             (data) = self.results_reader_list_test_runs_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def results_reader_list_test_runs_with_http_info(self, **kwargs):  # noqa: E501
         """ListTestRuns  # noqa: E501
 
-        Lists all test runs belonging to a project.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Lists all test runs belonging to a project.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_list_test_runs_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id: The ID of the project containing the requested test runs. Specify exactly one of the page_token field or this field.
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
-from rime_sdk.swagger.swagger_client.models.data_info_params_feature_intersection import DataInfoParamsFeatureIntersection
-from rime_sdk.swagger.swagger_client.models.data_info_params_ranking_info import DataInfoParamsRankingInfo
+from rime_sdk.swagger.swagger_client.models.data_params_feature_intersection import DataParamsFeatureIntersection
+from rime_sdk.swagger.swagger_client.models.data_params_ranking_info import DataParamsRankingInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_column_type_info import DataProfilingColumnTypeInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_feature_relationship_info import DataProfilingFeatureRelationshipInfo
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint import DatacollectorDatapoint
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint_row import DatacollectorDatapointRow
 from rime_sdk.swagger.swagger_client.models.dataset_ct_dataset_type import DatasetCTDatasetType
 from rime_sdk.swagger.swagger_client.models.dataset_ct_info import DatasetCTInfo
 from rime_sdk.swagger.swagger_client.models.dataset_dataset import DatasetDataset
@@ -56,14 +56,17 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
+from rime_sdk.swagger.swagger_client.models.fooexample_foo_request import FooexampleFooRequest
+from rime_sdk.swagger.swagger_client.models.fooexample_foo_response import FooexampleFooResponse
+from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
@@ -85,18 +88,15 @@
 from rime_sdk.swagger.swagger_client.models.list_summary_tests_request_list_summary_tests_query import ListSummaryTestsRequestListSummaryTestsQuery
 from rime_sdk.swagger.swagger_client.models.list_test_cases_request_list_test_cases_query import ListTestCasesRequestListTestCasesQuery
 from rime_sdk.swagger.swagger_client.models.managed_image_package_requirement import ManagedImagePackageRequirement
 from rime_sdk.swagger.swagger_client.models.managed_image_package_type import ManagedImagePackageType
 from rime_sdk.swagger.swagger_client.models.managed_image_pip_library import ManagedImagePipLibrary
 from rime_sdk.swagger.swagger_client.models.managed_image_pip_requirement import ManagedImagePipRequirement
 from rime_sdk.swagger.swagger_client.models.managed_image_role_type import ManagedImageRoleType
-from rime_sdk.swagger.swagger_client.models.model_hugging_face_model_info import ModelHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.model_model import ModelModel
-from rime_sdk.swagger.swagger_client.models.model_model_info import ModelModelInfo
-from rime_sdk.swagger.swagger_client.models.model_model_path_info import ModelModelPathInfo
 from rime_sdk.swagger.swagger_client.models.modelcards_model_card_model_card_id_uuid_body import ModelcardsModelCardModelCardIdUuidBody
 from rime_sdk.swagger.swagger_client.models.monitor_aggregation import MonitorAggregation
 from rime_sdk.swagger.swagger_client.models.monitor_aggregation_type import MonitorAggregationType
 from rime_sdk.swagger.swagger_client.models.monitor_anomaly_config import MonitorAnomalyConfig
 from rime_sdk.swagger.swagger_client.models.monitor_artifact_identifier import MonitorArtifactIdentifier
 from rime_sdk.swagger.swagger_client.models.monitor_difference_from_target import MonitorDifferenceFromTarget
 from rime_sdk.swagger.swagger_client.models.monitor_excluded_transforms import MonitorExcludedTransforms
@@ -141,15 +141,27 @@
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
 from rime_sdk.swagger.swagger_client.models.rca_feature_cause import RcaFeatureCause
 from rime_sdk.swagger.swagger_client.models.rca_rca_result import RcaRCAResult
 from rime_sdk.swagger.swagger_client.models.rca_rca_role import RcaRCARole
 from rime_sdk.swagger.swagger_client.models.rca_test_case_cause import RcaTestCaseCause
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
+from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
+from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
+from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
+from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
+from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
+from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
+from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
+from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
 from rime_sdk.swagger.swagger_client.models.registry_validity_status import RegistryValidityStatus
 from rime_sdk.swagger.swagger_client.models.registryprediction_prediction import RegistrypredictionPrediction
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
@@ -205,14 +217,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flag_jwt_response import RimeGetFeatureFlagJwtResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flags_response import RimeGetFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_firewall_response import RimeGetFirewallResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import RimeGetFooTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_image_response import RimeGetImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_integration_response import RimeGetIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_job_response import RimeGetJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_latest_logs_response import RimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_limit_status_response import RimeGetLimitStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_card_response import RimeGetModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_directory_upload_urls_response import RimeGetModelDirectoryUploadURLsResponse
@@ -230,14 +243,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
 from rime_sdk.swagger.swagger_client.models.rime_job_type import RimeJobType
 from rime_sdk.swagger.swagger_client.models.rime_job_view import RimeJobView
+from rime_sdk.swagger.swagger_client.models.rime_language import RimeLanguage
 from rime_sdk.swagger.swagger_client.models.rime_license_feature import RimeLicenseFeature
 from rime_sdk.swagger.swagger_client.models.rime_license_limit import RimeLicenseLimit
 from rime_sdk.swagger.swagger_client.models.rime_limit_status import RimeLimitStatus
 from rime_sdk.swagger.swagger_client.models.rime_limit_status_status import RimeLimitStatusStatus
 from rime_sdk.swagger.swagger_client.models.rime_list_api_tokens_response import RimeListAPITokensResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_agents_response import RimeListAgentsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
@@ -288,14 +302,17 @@
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import RimeStartFooTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import RimeStartFooTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_generative_stress_test_response import RimeStartGenerativeStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
@@ -341,42 +358,34 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
+from rime_sdk.swagger.swagger_client.models.schemaregistry_data_info import SchemaregistryDataInfo
+from rime_sdk.swagger.swagger_client.models.schematestrun_data_info import SchematestrunDataInfo
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
 from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
-from rime_sdk.swagger.swagger_client.models.testrun_connection_info import TestrunConnectionInfo
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
-from rime_sdk.swagger.swagger_client.models.testrun_data_collector_info import TestrunDataCollectorInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_file_info import TestrunDataFileInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_info import TestrunDataInfo
-from rime_sdk.swagger.swagger_client.models.testrun_data_info_params import TestrunDataInfoParams
-from rime_sdk.swagger.swagger_client.models.testrun_data_loading_info import TestrunDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.testrun_data_profiling import TestrunDataProfiling
-from rime_sdk.swagger.swagger_client.models.testrun_delta_lake_info import TestrunDeltaLakeInfo
-from rime_sdk.swagger.swagger_client.models.testrun_hugging_face_data_info import TestrunHuggingFaceDataInfo
+from rime_sdk.swagger.swagger_client.models.testrun_generative_test_run_config import TestrunGenerativeTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
-from rime_sdk.swagger.swagger_client.models.testrun_pred_info import TestrunPredInfo
-from rime_sdk.swagger.swagger_client.models.testrun_prediction_params import TestrunPredictionParams
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
-from rime_sdk.swagger.swagger_client.models.testrun_single_data_info import TestrunSingleDataInfo
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,17 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'eval_data_integration_id': 'RimeUUID',
-        'eval_data_info': 'TestrunSingleDataInfo',
+        'eval_data_info': 'SchemaregistryDataInfo',
         'eval_pred_integration_id': 'RimeUUID',
-        'eval_pred_info': 'TestrunPredInfo',
+        'eval_pred_info': 'RegistryPredInfo',
         'rolling_window': 'str'
     }
 
     attribute_map = {
         'eval_data_integration_id': 'evalDataIntegrationId',
         'eval_data_info': 'evalDataInfo',
         'eval_pred_integration_id': 'evalPredIntegrationId',
@@ -85,25 +85,25 @@
 
     @property
     def eval_data_info(self):
         """Gets the eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
 
 
         :return: The eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :rtype: TestrunSingleDataInfo
+        :rtype: SchemaregistryDataInfo
         """
         return self._eval_data_info
 
     @eval_data_info.setter
     def eval_data_info(self, eval_data_info):
         """Sets the eval_data_info of this CreateFirewallRequestScheduledCTParameters.
 
 
         :param eval_data_info: The eval_data_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :type: TestrunSingleDataInfo
+        :type: SchemaregistryDataInfo
         """
 
         self._eval_data_info = eval_data_info
 
     @property
     def eval_pred_integration_id(self):
         """Gets the eval_pred_integration_id of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
@@ -127,25 +127,25 @@
 
     @property
     def eval_pred_info(self):
         """Gets the eval_pred_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
 
 
         :return: The eval_pred_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :rtype: TestrunPredInfo
+        :rtype: RegistryPredInfo
         """
         return self._eval_pred_info
 
     @eval_pred_info.setter
     def eval_pred_info(self, eval_pred_info):
         """Sets the eval_pred_info of this CreateFirewallRequestScheduledCTParameters.
 
 
         :param eval_pred_info: The eval_pred_info of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
-        :type: TestrunPredInfo
+        :type: RegistryPredInfo
         """
 
         self._eval_pred_info = eval_pred_info
 
     @property
     def rolling_window(self):
         """Gets the rolling_window of this CreateFirewallRequestScheduledCTParameters.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class DataInfoParamsFeatureIntersection(object):
+class DataParamsFeatureIntersection(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'features': 'features'
     }
 
     def __init__(self, features=None):  # noqa: E501
-        """DataInfoParamsFeatureIntersection - a model defined in Swagger"""  # noqa: E501
+        """DataParamsFeatureIntersection - a model defined in Swagger"""  # noqa: E501
         self._features = None
         self.discriminator = None
         if features is not None:
             self.features = features
 
     @property
     def features(self):
-        """Gets the features of this DataInfoParamsFeatureIntersection.  # noqa: E501
+        """Gets the features of this DataParamsFeatureIntersection.  # noqa: E501
 
 
-        :return: The features of this DataInfoParamsFeatureIntersection.  # noqa: E501
+        :return: The features of this DataParamsFeatureIntersection.  # noqa: E501
         :rtype: list[str]
         """
         return self._features
 
     @features.setter
     def features(self, features):
-        """Sets the features of this DataInfoParamsFeatureIntersection.
+        """Sets the features of this DataParamsFeatureIntersection.
 
 
-        :param features: The features of this DataInfoParamsFeatureIntersection.  # noqa: E501
+        :param features: The features of this DataParamsFeatureIntersection.  # noqa: E501
         :type: list[str]
         """
 
         self._features = features
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DataInfoParamsFeatureIntersection, dict):
+        if issubclass(DataParamsFeatureIntersection, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DataInfoParamsFeatureIntersection):
+        if not isinstance(other, DataParamsFeatureIntersection):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class DataInfoParamsRankingInfo(object):
+class DataParamsRankingInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,15 +38,15 @@
         'query_col': 'queryCol',
         'nqueries': 'nqueries',
         'nrows_per_query': 'nrowsPerQuery',
         'drop_query_id': 'dropQueryId'
     }
 
     def __init__(self, query_col=None, nqueries=None, nrows_per_query=None, drop_query_id=None):  # noqa: E501
-        """DataInfoParamsRankingInfo - a model defined in Swagger"""  # noqa: E501
+        """DataParamsRankingInfo - a model defined in Swagger"""  # noqa: E501
         self._query_col = None
         self._nqueries = None
         self._nrows_per_query = None
         self._drop_query_id = None
         self.discriminator = None
         if query_col is not None:
             self.query_col = query_col
@@ -55,99 +55,99 @@
         if nrows_per_query is not None:
             self.nrows_per_query = nrows_per_query
         if drop_query_id is not None:
             self.drop_query_id = drop_query_id
 
     @property
     def query_col(self):
-        """Gets the query_col of this DataInfoParamsRankingInfo.  # noqa: E501
+        """Gets the query_col of this DataParamsRankingInfo.  # noqa: E501
 
         Name of column in dataset that contains the query ids.  # noqa: E501
 
-        :return: The query_col of this DataInfoParamsRankingInfo.  # noqa: E501
+        :return: The query_col of this DataParamsRankingInfo.  # noqa: E501
         :rtype: str
         """
         return self._query_col
 
     @query_col.setter
     def query_col(self, query_col):
-        """Sets the query_col of this DataInfoParamsRankingInfo.
+        """Sets the query_col of this DataParamsRankingInfo.
 
         Name of column in dataset that contains the query ids.  # noqa: E501
 
-        :param query_col: The query_col of this DataInfoParamsRankingInfo.  # noqa: E501
+        :param query_col: The query_col of this DataParamsRankingInfo.  # noqa: E501
         :type: str
         """
 
         self._query_col = query_col
 
     @property
     def nqueries(self):
-        """Gets the nqueries of this DataInfoParamsRankingInfo.  # noqa: E501
+        """Gets the nqueries of this DataParamsRankingInfo.  # noqa: E501
 
         Number of queries to consider. If null, will use all queries.  # noqa: E501
 
-        :return: The nqueries of this DataInfoParamsRankingInfo.  # noqa: E501
+        :return: The nqueries of this DataParamsRankingInfo.  # noqa: E501
         :rtype: str
         """
         return self._nqueries
 
     @nqueries.setter
     def nqueries(self, nqueries):
-        """Sets the nqueries of this DataInfoParamsRankingInfo.
+        """Sets the nqueries of this DataParamsRankingInfo.
 
         Number of queries to consider. If null, will use all queries.  # noqa: E501
 
-        :param nqueries: The nqueries of this DataInfoParamsRankingInfo.  # noqa: E501
+        :param nqueries: The nqueries of this DataParamsRankingInfo.  # noqa: E501
         :type: str
         """
 
         self._nqueries = nqueries
 
     @property
     def nrows_per_query(self):
-        """Gets the nrows_per_query of this DataInfoParamsRankingInfo.  # noqa: E501
+        """Gets the nrows_per_query of this DataParamsRankingInfo.  # noqa: E501
 
         Number of rows to use per query. If null, will use all rows.  # noqa: E501
 
-        :return: The nrows_per_query of this DataInfoParamsRankingInfo.  # noqa: E501
+        :return: The nrows_per_query of this DataParamsRankingInfo.  # noqa: E501
         :rtype: str
         """
         return self._nrows_per_query
 
     @nrows_per_query.setter
     def nrows_per_query(self, nrows_per_query):
-        """Sets the nrows_per_query of this DataInfoParamsRankingInfo.
+        """Sets the nrows_per_query of this DataParamsRankingInfo.
 
         Number of rows to use per query. If null, will use all rows.  # noqa: E501
 
-        :param nrows_per_query: The nrows_per_query of this DataInfoParamsRankingInfo.  # noqa: E501
+        :param nrows_per_query: The nrows_per_query of this DataParamsRankingInfo.  # noqa: E501
         :type: str
         """
 
         self._nrows_per_query = nrows_per_query
 
     @property
     def drop_query_id(self):
-        """Gets the drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
+        """Gets the drop_query_id of this DataParamsRankingInfo.  # noqa: E501
 
         Whether to drop the query ID column from the dataset to avoid passing as a feature to the model.  # noqa: E501
 
-        :return: The drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
+        :return: The drop_query_id of this DataParamsRankingInfo.  # noqa: E501
         :rtype: bool
         """
         return self._drop_query_id
 
     @drop_query_id.setter
     def drop_query_id(self, drop_query_id):
-        """Sets the drop_query_id of this DataInfoParamsRankingInfo.
+        """Sets the drop_query_id of this DataParamsRankingInfo.
 
         Whether to drop the query ID column from the dataset to avoid passing as a feature to the model.  # noqa: E501
 
-        :param drop_query_id: The drop_query_id of this DataInfoParamsRankingInfo.  # noqa: E501
+        :param drop_query_id: The drop_query_id of this DataParamsRankingInfo.  # noqa: E501
         :type: bool
         """
 
         self._drop_query_id = drop_query_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -166,15 +166,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(DataInfoParamsRankingInfo, dict):
+        if issubclass(DataParamsRankingInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -182,15 +182,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DataInfoParamsRankingInfo):
+        if not isinstance(other, DataParamsRankingInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'name': 'str',
         'dataset_id': 'str',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'user_metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'data_info': 'TestrunSingleDataInfo',
+        'data_info': 'SchemaregistryDataInfo',
         'ct_info': 'DatasetCTInfo',
         'validity_status': 'RegistryValidityStatus',
         'marked_for_delete_at': 'datetime'
     }
 
     attribute_map = {
         'name': 'name',
@@ -245,25 +245,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this DatasetDataset.  # noqa: E501
 
 
         :return: The data_info of this DatasetDataset.  # noqa: E501
-        :rtype: TestrunSingleDataInfo
+        :rtype: SchemaregistryDataInfo
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this DatasetDataset.
 
 
         :param data_info: The data_info of this DatasetDataset.  # noqa: E501
-        :type: TestrunSingleDataInfo
+        :type: SchemaregistryDataInfo
         """
 
         self._data_info = data_info
 
     @property
     def ct_info(self):
         """Gets the ct_info of this DatasetDataset.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'model_id': 'object',
         'metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'pred_info': 'TestrunPredInfo'
+        'pred_info': 'RegistryPredInfo'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'model_id': 'modelId',
         'metadata': 'metadata',
         'integration_id': 'integrationId',
@@ -152,25 +152,25 @@
 
     @property
     def pred_info(self):
         """Gets the pred_info of this DatasetIdPredictionBody.  # noqa: E501
 
 
         :return: The pred_info of this DatasetIdPredictionBody.  # noqa: E501
-        :rtype: TestrunPredInfo
+        :rtype: RegistryPredInfo
         """
         return self._pred_info
 
     @pred_info.setter
     def pred_info(self, pred_info):
         """Sets the pred_info of this DatasetIdPredictionBody.
 
 
         :param pred_info: The pred_info of this DatasetIdPredictionBody.  # noqa: E501
-        :type: TestrunPredInfo
+        :type: RegistryPredInfo
         """
 
         self._pred_info = pred_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,17 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'eval_data_integration_id': 'RimeUUID',
-        'eval_data_info': 'TestrunSingleDataInfo',
+        'eval_data_info': 'SchemaregistryDataInfo',
         'eval_pred_integration_id': 'RimeUUID',
-        'eval_pred_info': 'TestrunPredInfo',
+        'eval_pred_info': 'RegistryPredInfo',
         'rolling_window': 'str',
         'last_ct_scheduled': 'datetime',
         'activated_time': 'datetime',
         'disable_scheduled_ct': 'bool'
     }
 
     attribute_map = {
@@ -100,25 +100,25 @@
 
     @property
     def eval_data_info(self):
         """Gets the eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
 
 
         :return: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :rtype: TestrunSingleDataInfo
+        :rtype: SchemaregistryDataInfo
         """
         return self._eval_data_info
 
     @eval_data_info.setter
     def eval_data_info(self, eval_data_info):
         """Sets the eval_data_info of this FirewallScheduledCTInfo.
 
 
         :param eval_data_info: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :type: TestrunSingleDataInfo
+        :type: SchemaregistryDataInfo
         """
 
         self._eval_data_info = eval_data_info
 
     @property
     def eval_pred_integration_id(self):
         """Gets the eval_pred_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
@@ -142,25 +142,25 @@
 
     @property
     def eval_pred_info(self):
         """Gets the eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
 
 
         :return: The eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :rtype: TestrunPredInfo
+        :rtype: RegistryPredInfo
         """
         return self._eval_pred_info
 
     @eval_pred_info.setter
     def eval_pred_info(self, eval_pred_info):
         """Sets the eval_pred_info of this FirewallScheduledCTInfo.
 
 
         :param eval_pred_info: The eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
-        :type: TestrunPredInfo
+        :type: RegistryPredInfo
         """
 
         self._eval_pred_info = eval_pred_info
 
     @property
     def rolling_window(self):
         """Gets the rolling_window of this FirewallScheduledCTInfo.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ModelHuggingFaceModelInfo(object):
+class RegistryHuggingFaceModelInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,62 +34,62 @@
 
     attribute_map = {
         'model_uri': 'modelUri',
         'kwargs': 'kwargs'
     }
 
     def __init__(self, model_uri=None, kwargs=None):  # noqa: E501
-        """ModelHuggingFaceModelInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryHuggingFaceModelInfo - a model defined in Swagger"""  # noqa: E501
         self._model_uri = None
         self._kwargs = None
         self.discriminator = None
         if model_uri is not None:
             self.model_uri = model_uri
         if kwargs is not None:
             self.kwargs = kwargs
 
     @property
     def model_uri(self):
-        """Gets the model_uri of this ModelHuggingFaceModelInfo.  # noqa: E501
+        """Gets the model_uri of this RegistryHuggingFaceModelInfo.  # noqa: E501
 
 
-        :return: The model_uri of this ModelHuggingFaceModelInfo.  # noqa: E501
+        :return: The model_uri of this RegistryHuggingFaceModelInfo.  # noqa: E501
         :rtype: str
         """
         return self._model_uri
 
     @model_uri.setter
     def model_uri(self, model_uri):
-        """Sets the model_uri of this ModelHuggingFaceModelInfo.
+        """Sets the model_uri of this RegistryHuggingFaceModelInfo.
 
 
-        :param model_uri: The model_uri of this ModelHuggingFaceModelInfo.  # noqa: E501
+        :param model_uri: The model_uri of this RegistryHuggingFaceModelInfo.  # noqa: E501
         :type: str
         """
 
         self._model_uri = model_uri
 
     @property
     def kwargs(self):
-        """Gets the kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
+        """Gets the kwargs of this RegistryHuggingFaceModelInfo.  # noqa: E501
 
         We are currently in the process of adding extra huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
 
-        :return: The kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
+        :return: The kwargs of this RegistryHuggingFaceModelInfo.  # noqa: E501
         :rtype: str
         """
         return self._kwargs
 
     @kwargs.setter
     def kwargs(self, kwargs):
-        """Sets the kwargs of this ModelHuggingFaceModelInfo.
+        """Sets the kwargs of this RegistryHuggingFaceModelInfo.
 
         We are currently in the process of adding extra huggingface params and separating use cases into tabular and nlp. Use a serialized json dictionary for other variables right now to ensure maximum flexibility.  # noqa: E501
 
-        :param kwargs: The kwargs of this ModelHuggingFaceModelInfo.  # noqa: E501
+        :param kwargs: The kwargs of this RegistryHuggingFaceModelInfo.  # noqa: E501
         :type: str
         """
 
         self._kwargs = kwargs
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ModelHuggingFaceModelInfo, dict):
+        if issubclass(RegistryHuggingFaceModelInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ModelHuggingFaceModelInfo):
+        if not isinstance(other, RegistryHuggingFaceModelInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'name': 'str',
         'model_id': 'RimeUUID',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'external_id': 'str',
         'user_metadata': 'RegistryMetadata',
-        'model_info': 'ModelModelInfo',
+        'model_info': 'RegistryModelInfo',
         'validity_status': 'RegistryValidityStatus',
         'integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'name': 'name',
         'model_id': 'modelId',
@@ -242,25 +242,25 @@
 
     @property
     def model_info(self):
         """Gets the model_info of this ModelModel.  # noqa: E501
 
 
         :return: The model_info of this ModelModel.  # noqa: E501
-        :rtype: ModelModelInfo
+        :rtype: RegistryModelInfo
         """
         return self._model_info
 
     @model_info.setter
     def model_info(self, model_info):
         """Sets the model_info of this ModelModel.
 
 
         :param model_info: The model_info of this ModelModel.  # noqa: E501
-        :type: ModelModelInfo
+        :type: RegistryModelInfo
         """
 
         self._model_info = model_info
 
     @property
     def validity_status(self):
         """Gets the validity_status of this ModelModel.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,84 +11,84 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ModelModelInfo(object):
+class RegistryModelInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'model_path': 'ModelModelPathInfo',
-        'hugging_face': 'ModelHuggingFaceModelInfo'
+        'model_path': 'RegistryModelPathInfo',
+        'hugging_face': 'RegistryHuggingFaceModelInfo'
     }
 
     attribute_map = {
         'model_path': 'modelPath',
         'hugging_face': 'huggingFace'
     }
 
     def __init__(self, model_path=None, hugging_face=None):  # noqa: E501
-        """ModelModelInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryModelInfo - a model defined in Swagger"""  # noqa: E501
         self._model_path = None
         self._hugging_face = None
         self.discriminator = None
         if model_path is not None:
             self.model_path = model_path
         if hugging_face is not None:
             self.hugging_face = hugging_face
 
     @property
     def model_path(self):
-        """Gets the model_path of this ModelModelInfo.  # noqa: E501
+        """Gets the model_path of this RegistryModelInfo.  # noqa: E501
 
 
-        :return: The model_path of this ModelModelInfo.  # noqa: E501
-        :rtype: ModelModelPathInfo
+        :return: The model_path of this RegistryModelInfo.  # noqa: E501
+        :rtype: RegistryModelPathInfo
         """
         return self._model_path
 
     @model_path.setter
     def model_path(self, model_path):
-        """Sets the model_path of this ModelModelInfo.
+        """Sets the model_path of this RegistryModelInfo.
 
 
-        :param model_path: The model_path of this ModelModelInfo.  # noqa: E501
-        :type: ModelModelPathInfo
+        :param model_path: The model_path of this RegistryModelInfo.  # noqa: E501
+        :type: RegistryModelPathInfo
         """
 
         self._model_path = model_path
 
     @property
     def hugging_face(self):
-        """Gets the hugging_face of this ModelModelInfo.  # noqa: E501
+        """Gets the hugging_face of this RegistryModelInfo.  # noqa: E501
 
 
-        :return: The hugging_face of this ModelModelInfo.  # noqa: E501
-        :rtype: ModelHuggingFaceModelInfo
+        :return: The hugging_face of this RegistryModelInfo.  # noqa: E501
+        :rtype: RegistryHuggingFaceModelInfo
         """
         return self._hugging_face
 
     @hugging_face.setter
     def hugging_face(self, hugging_face):
-        """Sets the hugging_face of this ModelModelInfo.
+        """Sets the hugging_face of this RegistryModelInfo.
 
 
-        :param hugging_face: The hugging_face of this ModelModelInfo.  # noqa: E501
-        :type: ModelHuggingFaceModelInfo
+        :param hugging_face: The hugging_face of this RegistryModelInfo.  # noqa: E501
+        :type: RegistryHuggingFaceModelInfo
         """
 
         self._hugging_face = hugging_face
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ModelModelInfo, dict):
+        if issubclass(RegistryModelInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ModelModelInfo):
+        if not isinstance(other, RegistryModelInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/model_model_path_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ModelModelPathInfo(object):
+class RegistryModelPathInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'path': 'path'
     }
 
     def __init__(self, path=None):  # noqa: E501
-        """ModelModelPathInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryModelPathInfo - a model defined in Swagger"""  # noqa: E501
         self._path = None
         self.discriminator = None
         if path is not None:
             self.path = path
 
     @property
     def path(self):
-        """Gets the path of this ModelModelPathInfo.  # noqa: E501
+        """Gets the path of this RegistryModelPathInfo.  # noqa: E501
 
 
-        :return: The path of this ModelModelPathInfo.  # noqa: E501
+        :return: The path of this RegistryModelPathInfo.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
-        """Sets the path of this ModelModelPathInfo.
+        """Sets the path of this RegistryModelPathInfo.
 
 
-        :param path: The path of this ModelModelPathInfo.  # noqa: E501
+        :param path: The path of this RegistryModelPathInfo.  # noqa: E501
         :type: str
         """
 
         self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ModelModelPathInfo, dict):
+        if issubclass(RegistryModelPathInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ModelModelPathInfo):
+        if not isinstance(other, RegistryModelPathInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'data_info': 'TestrunSingleDataInfo',
+        'data_info': 'SchemaregistryDataInfo',
         'ct_info': 'DatasetCTInfo'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
@@ -158,25 +158,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
 
 
         :return: The data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
-        :rtype: TestrunSingleDataInfo
+        :rtype: SchemaregistryDataInfo
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this ProjectIdUuidDatasetBody.
 
 
         :param data_info: The data_info of this ProjectIdUuidDatasetBody.  # noqa: E501
-        :type: TestrunSingleDataInfo
+        :type: SchemaregistryDataInfo
         """
 
         self._data_info = data_info
 
     @property
     def ct_info(self):
         """Gets the ct_info of this ProjectIdUuidDatasetBody.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'external_id': 'str',
-        'model_info': 'ModelModelInfo',
+        'model_info': 'RegistryModelInfo',
         'integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
@@ -160,25 +160,25 @@
 
     @property
     def model_info(self):
         """Gets the model_info of this ProjectIdUuidModelBody.  # noqa: E501
 
 
         :return: The model_info of this ProjectIdUuidModelBody.  # noqa: E501
-        :rtype: ModelModelInfo
+        :rtype: RegistryModelInfo
         """
         return self._model_info
 
     @model_info.setter
     def model_info(self, model_info):
         """Sets the model_info of this ProjectIdUuidModelBody.
 
 
         :param model_info: The model_info of this ProjectIdUuidModelBody.  # noqa: E501
-        :type: ModelModelInfo
+        :type: RegistryModelInfo
         """
 
         self._model_info = model_info
 
     @property
     def integration_id(self):
         """Gets the integration_id of this ProjectIdUuidModelBody.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'dataset_id': 'str',
         'model_id': 'RimeUUID',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'user_metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'pred_info': 'TestrunPredInfo',
+        'pred_info': 'RegistryPredInfo',
         'validity_status': 'RegistryValidityStatus',
         'marked_for_delete_at': 'datetime'
     }
 
     attribute_map = {
         'dataset_id': 'datasetId',
         'model_id': 'modelId',
@@ -240,25 +240,25 @@
 
     @property
     def pred_info(self):
         """Gets the pred_info of this RegistrypredictionPrediction.  # noqa: E501
 
 
         :return: The pred_info of this RegistrypredictionPrediction.  # noqa: E501
-        :rtype: TestrunPredInfo
+        :rtype: RegistryPredInfo
         """
         return self._pred_info
 
     @pred_info.setter
     def pred_info(self, pred_info):
         """Sets the pred_info of this RegistrypredictionPrediction.
 
 
         :param pred_info: The pred_info of this RegistrypredictionPrediction.  # noqa: E501
-        :type: TestrunPredInfo
+        :type: RegistryPredInfo
         """
 
         self._pred_info = pred_info
 
     @property
     def validity_status(self):
         """Gets the validity_status of this RegistrypredictionPrediction.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     allowed enum values
     """
     UNSPECIFIED = "JOB_TYPE_UNSPECIFIED"
     MODEL_STRESS_TEST = "JOB_TYPE_MODEL_STRESS_TEST"
     IMAGE_BUILDER = "JOB_TYPE_IMAGE_BUILDER"
     FIREWALL_BATCH_TEST = "JOB_TYPE_FIREWALL_BATCH_TEST"
     FILE_SCAN = "JOB_TYPE_FILE_SCAN"
+    CROSS_PLANE_TASK = "JOB_TYPE_CROSS_PLANE_TASK"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     BINARY_CLASSIFICATION = "MODEL_TASK_BINARY_CLASSIFICATION"
     MULTICLASS_CLASSIFICATION = "MODEL_TASK_MULTICLASS_CLASSIFICATION"
     NAMED_ENTITY_RECOGNITION = "MODEL_TASK_NAMED_ENTITY_RECOGNITION"
     RANKING = "MODEL_TASK_RANKING"
     OBJECT_DETECTION = "MODEL_TASK_OBJECT_DETECTION"
     NATURAL_LANGUAGE_INFERENCE = "MODEL_TASK_NATURAL_LANGUAGE_INFERENCE"
     FILL_MASK = "MODEL_TASK_FILL_MASK"
+    QUESTION_ANSWERING = "MODEL_TASK_QUESTION_ANSWERING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/tags_name_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/tags_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataCollectorInfo(object):
+class RegistryDataCollectorInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'data_stream_id': 'dataStreamId'
     }
 
     def __init__(self, data_stream_id=None):  # noqa: E501
-        """TestrunDataCollectorInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDataCollectorInfo - a model defined in Swagger"""  # noqa: E501
         self._data_stream_id = None
         self.discriminator = None
         if data_stream_id is not None:
             self.data_stream_id = data_stream_id
 
     @property
     def data_stream_id(self):
-        """Gets the data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
+        """Gets the data_stream_id of this RegistryDataCollectorInfo.  # noqa: E501
 
 
-        :return: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
+        :return: The data_stream_id of this RegistryDataCollectorInfo.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._data_stream_id
 
     @data_stream_id.setter
     def data_stream_id(self, data_stream_id):
-        """Sets the data_stream_id of this TestrunDataCollectorInfo.
+        """Sets the data_stream_id of this RegistryDataCollectorInfo.
 
 
-        :param data_stream_id: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
+        :param data_stream_id: The data_stream_id of this RegistryDataCollectorInfo.  # noqa: E501
         :type: RimeUUID
         """
 
         self._data_stream_id = data_stream_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataCollectorInfo, dict):
+        if issubclass(RegistryDataCollectorInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataCollectorInfo):
+        if not isinstance(other, RegistryDataCollectorInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataFileInfo(object):
+class RegistryDataFileInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,37 +32,37 @@
     }
 
     attribute_map = {
         'path': 'path'
     }
 
     def __init__(self, path=None):  # noqa: E501
-        """TestrunDataFileInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDataFileInfo - a model defined in Swagger"""  # noqa: E501
         self._path = None
         self.discriminator = None
         self.path = path
 
     @property
     def path(self):
-        """Gets the path of this TestrunDataFileInfo.  # noqa: E501
+        """Gets the path of this RegistryDataFileInfo.  # noqa: E501
 
         The path to the data file.  # noqa: E501
 
-        :return: The path of this TestrunDataFileInfo.  # noqa: E501
+        :return: The path of this RegistryDataFileInfo.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
-        """Sets the path of this TestrunDataFileInfo.
+        """Sets the path of this RegistryDataFileInfo.
 
         The path to the data file.  # noqa: E501
 
-        :param path: The path of this TestrunDataFileInfo.  # noqa: E501
+        :param path: The path of this RegistryDataFileInfo.  # noqa: E501
         :type: str
         """
         if path is None:
             raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
         self._path = path
 
@@ -83,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataFileInfo, dict):
+        if issubclass(RegistryDataFileInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataFileInfo):
+        if not isinstance(other, RegistryDataFileInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataInfo(object):
+class SchematestrunDataInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,64 +34,64 @@
 
     attribute_map = {
         'ref_dataset_id': 'refDatasetId',
         'eval_dataset_id': 'evalDatasetId'
     }
 
     def __init__(self, ref_dataset_id=None, eval_dataset_id=None):  # noqa: E501
-        """TestrunDataInfo - a model defined in Swagger"""  # noqa: E501
+        """SchematestrunDataInfo - a model defined in Swagger"""  # noqa: E501
         self._ref_dataset_id = None
         self._eval_dataset_id = None
         self.discriminator = None
         self.ref_dataset_id = ref_dataset_id
         self.eval_dataset_id = eval_dataset_id
 
     @property
     def ref_dataset_id(self):
-        """Gets the ref_dataset_id of this TestrunDataInfo.  # noqa: E501
+        """Gets the ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
 
         Uniquely specifies a reference Dataset.  # noqa: E501
 
-        :return: The ref_dataset_id of this TestrunDataInfo.  # noqa: E501
+        :return: The ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
         :rtype: str
         """
         return self._ref_dataset_id
 
     @ref_dataset_id.setter
     def ref_dataset_id(self, ref_dataset_id):
-        """Sets the ref_dataset_id of this TestrunDataInfo.
+        """Sets the ref_dataset_id of this SchematestrunDataInfo.
 
         Uniquely specifies a reference Dataset.  # noqa: E501
 
-        :param ref_dataset_id: The ref_dataset_id of this TestrunDataInfo.  # noqa: E501
+        :param ref_dataset_id: The ref_dataset_id of this SchematestrunDataInfo.  # noqa: E501
         :type: str
         """
         if ref_dataset_id is None:
             raise ValueError("Invalid value for `ref_dataset_id`, must not be `None`")  # noqa: E501
 
         self._ref_dataset_id = ref_dataset_id
 
     @property
     def eval_dataset_id(self):
-        """Gets the eval_dataset_id of this TestrunDataInfo.  # noqa: E501
+        """Gets the eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
 
         Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :return: The eval_dataset_id of this TestrunDataInfo.  # noqa: E501
+        :return: The eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
         :rtype: str
         """
         return self._eval_dataset_id
 
     @eval_dataset_id.setter
     def eval_dataset_id(self, eval_dataset_id):
-        """Sets the eval_dataset_id of this TestrunDataInfo.
+        """Sets the eval_dataset_id of this SchematestrunDataInfo.
 
         Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :param eval_dataset_id: The eval_dataset_id of this TestrunDataInfo.  # noqa: E501
+        :param eval_dataset_id: The eval_dataset_id of this SchematestrunDataInfo.  # noqa: E501
         :type: str
         """
         if eval_dataset_id is None:
             raise ValueError("Invalid value for `eval_dataset_id`, must not be `None`")  # noqa: E501
 
         self._eval_dataset_id = eval_dataset_id
 
@@ -112,15 +112,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataInfo, dict):
+        if issubclass(SchematestrunDataInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -128,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataInfo):
+        if not isinstance(other, SchematestrunDataInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataLoadingInfo(object):
+class RegistryDataLoadingInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,92 +36,92 @@
     attribute_map = {
         'path': 'path',
         'load_func_name': 'loadFuncName',
         'loader_kwargs_json': 'loaderKwargsJson'
     }
 
     def __init__(self, path=None, load_func_name=None, loader_kwargs_json=None):  # noqa: E501
-        """TestrunDataLoadingInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDataLoadingInfo - a model defined in Swagger"""  # noqa: E501
         self._path = None
         self._load_func_name = None
         self._loader_kwargs_json = None
         self.discriminator = None
         self.path = path
         self.load_func_name = load_func_name
         if loader_kwargs_json is not None:
             self.loader_kwargs_json = loader_kwargs_json
 
     @property
     def path(self):
-        """Gets the path of this TestrunDataLoadingInfo.  # noqa: E501
+        """Gets the path of this RegistryDataLoadingInfo.  # noqa: E501
 
         The path to the data file.  # noqa: E501
 
-        :return: The path of this TestrunDataLoadingInfo.  # noqa: E501
+        :return: The path of this RegistryDataLoadingInfo.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
-        """Sets the path of this TestrunDataLoadingInfo.
+        """Sets the path of this RegistryDataLoadingInfo.
 
         The path to the data file.  # noqa: E501
 
-        :param path: The path of this TestrunDataLoadingInfo.  # noqa: E501
+        :param path: The path of this RegistryDataLoadingInfo.  # noqa: E501
         :type: str
         """
         if path is None:
             raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
         self._path = path
 
     @property
     def load_func_name(self):
-        """Gets the load_func_name of this TestrunDataLoadingInfo.  # noqa: E501
+        """Gets the load_func_name of this RegistryDataLoadingInfo.  # noqa: E501
 
         The name of the function that loads the data.  # noqa: E501
 
-        :return: The load_func_name of this TestrunDataLoadingInfo.  # noqa: E501
+        :return: The load_func_name of this RegistryDataLoadingInfo.  # noqa: E501
         :rtype: str
         """
         return self._load_func_name
 
     @load_func_name.setter
     def load_func_name(self, load_func_name):
-        """Sets the load_func_name of this TestrunDataLoadingInfo.
+        """Sets the load_func_name of this RegistryDataLoadingInfo.
 
         The name of the function that loads the data.  # noqa: E501
 
-        :param load_func_name: The load_func_name of this TestrunDataLoadingInfo.  # noqa: E501
+        :param load_func_name: The load_func_name of this RegistryDataLoadingInfo.  # noqa: E501
         :type: str
         """
         if load_func_name is None:
             raise ValueError("Invalid value for `load_func_name`, must not be `None`")  # noqa: E501
 
         self._load_func_name = load_func_name
 
     @property
     def loader_kwargs_json(self):
-        """Gets the loader_kwargs_json of this TestrunDataLoadingInfo.  # noqa: E501
+        """Gets the loader_kwargs_json of this RegistryDataLoadingInfo.  # noqa: E501
 
         This is a JSON-serialized string from a map.  # noqa: E501
 
-        :return: The loader_kwargs_json of this TestrunDataLoadingInfo.  # noqa: E501
+        :return: The loader_kwargs_json of this RegistryDataLoadingInfo.  # noqa: E501
         :rtype: str
         """
         return self._loader_kwargs_json
 
     @loader_kwargs_json.setter
     def loader_kwargs_json(self, loader_kwargs_json):
-        """Sets the loader_kwargs_json of this TestrunDataLoadingInfo.
+        """Sets the loader_kwargs_json of this RegistryDataLoadingInfo.
 
         This is a JSON-serialized string from a map.  # noqa: E501
 
-        :param loader_kwargs_json: The loader_kwargs_json of this TestrunDataLoadingInfo.  # noqa: E501
+        :param loader_kwargs_json: The loader_kwargs_json of this RegistryDataLoadingInfo.  # noqa: E501
         :type: str
         """
 
         self._loader_kwargs_json = loader_kwargs_json
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -140,15 +140,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataLoadingInfo, dict):
+        if issubclass(RegistryDataLoadingInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -156,15 +156,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataLoadingInfo):
+        if not isinstance(other, RegistryDataLoadingInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDeltaLakeInfo(object):
+class RegistryDeltaLakeInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,37 +32,37 @@
     }
 
     attribute_map = {
         'table_name': 'tableName'
     }
 
     def __init__(self, table_name=None):  # noqa: E501
-        """TestrunDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
         self._table_name = None
         self.discriminator = None
         self.table_name = table_name
 
     @property
     def table_name(self):
-        """Gets the table_name of this TestrunDeltaLakeInfo.  # noqa: E501
+        """Gets the table_name of this RegistryDeltaLakeInfo.  # noqa: E501
 
         The database table name to use.  # noqa: E501
 
-        :return: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
+        :return: The table_name of this RegistryDeltaLakeInfo.  # noqa: E501
         :rtype: str
         """
         return self._table_name
 
     @table_name.setter
     def table_name(self, table_name):
-        """Sets the table_name of this TestrunDeltaLakeInfo.
+        """Sets the table_name of this RegistryDeltaLakeInfo.
 
         The database table name to use.  # noqa: E501
 
-        :param table_name: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
+        :param table_name: The table_name of this RegistryDeltaLakeInfo.  # noqa: E501
         :type: str
         """
         if table_name is None:
             raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
 
         self._table_name = table_name
 
@@ -83,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDeltaLakeInfo, dict):
+        if issubclass(RegistryDeltaLakeInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDeltaLakeInfo):
+        if not isinstance(other, RegistryDeltaLakeInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunHuggingFaceDataInfo(object):
+class RegistryHuggingFaceDataInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,92 +36,92 @@
     attribute_map = {
         'dataset_uri': 'datasetUri',
         'split_name': 'splitName',
         'loading_params_json': 'loadingParamsJson'
     }
 
     def __init__(self, dataset_uri=None, split_name=None, loading_params_json=None):  # noqa: E501
-        """TestrunHuggingFaceDataInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryHuggingFaceDataInfo - a model defined in Swagger"""  # noqa: E501
         self._dataset_uri = None
         self._split_name = None
         self._loading_params_json = None
         self.discriminator = None
         self.dataset_uri = dataset_uri
         self.split_name = split_name
         if loading_params_json is not None:
             self.loading_params_json = loading_params_json
 
     @property
     def dataset_uri(self):
-        """Gets the dataset_uri of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        """Gets the dataset_uri of this RegistryHuggingFaceDataInfo.  # noqa: E501
 
         The unique identifier of the dataset.  # noqa: E501
 
-        :return: The dataset_uri of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :return: The dataset_uri of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :rtype: str
         """
         return self._dataset_uri
 
     @dataset_uri.setter
     def dataset_uri(self, dataset_uri):
-        """Sets the dataset_uri of this TestrunHuggingFaceDataInfo.
+        """Sets the dataset_uri of this RegistryHuggingFaceDataInfo.
 
         The unique identifier of the dataset.  # noqa: E501
 
-        :param dataset_uri: The dataset_uri of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :param dataset_uri: The dataset_uri of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :type: str
         """
         if dataset_uri is None:
             raise ValueError("Invalid value for `dataset_uri`, must not be `None`")  # noqa: E501
 
         self._dataset_uri = dataset_uri
 
     @property
     def split_name(self):
-        """Gets the split_name of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        """Gets the split_name of this RegistryHuggingFaceDataInfo.  # noqa: E501
 
         The string that represents the name of a predefined subset of data.  # noqa: E501
 
-        :return: The split_name of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :return: The split_name of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :rtype: str
         """
         return self._split_name
 
     @split_name.setter
     def split_name(self, split_name):
-        """Sets the split_name of this TestrunHuggingFaceDataInfo.
+        """Sets the split_name of this RegistryHuggingFaceDataInfo.
 
         The string that represents the name of a predefined subset of data.  # noqa: E501
 
-        :param split_name: The split_name of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :param split_name: The split_name of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :type: str
         """
         if split_name is None:
             raise ValueError("Invalid value for `split_name`, must not be `None`")  # noqa: E501
 
         self._split_name = split_name
 
     @property
     def loading_params_json(self):
-        """Gets the loading_params_json of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        """Gets the loading_params_json of this RegistryHuggingFaceDataInfo.  # noqa: E501
 
         This is a JSON-serialized string from a map.  # noqa: E501
 
-        :return: The loading_params_json of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :return: The loading_params_json of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :rtype: str
         """
         return self._loading_params_json
 
     @loading_params_json.setter
     def loading_params_json(self, loading_params_json):
-        """Sets the loading_params_json of this TestrunHuggingFaceDataInfo.
+        """Sets the loading_params_json of this RegistryHuggingFaceDataInfo.
 
         This is a JSON-serialized string from a map.  # noqa: E501
 
-        :param loading_params_json: The loading_params_json of this TestrunHuggingFaceDataInfo.  # noqa: E501
+        :param loading_params_json: The loading_params_json of this RegistryHuggingFaceDataInfo.  # noqa: E501
         :type: str
         """
 
         self._loading_params_json = loading_params_json
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -140,15 +140,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunHuggingFaceDataInfo, dict):
+        if issubclass(RegistryHuggingFaceDataInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -156,15 +156,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunHuggingFaceDataInfo):
+        if not isinstance(other, RegistryHuggingFaceDataInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunPredInfo(object):
+class UserFavoriteProjects(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection_info': 'TestrunConnectionInfo',
-        'pred_params': 'TestrunPredictionParams'
+        'workspace_id': 'RimeUUID',
+        'project_ids': 'list[RimeUUID]'
     }
 
     attribute_map = {
-        'connection_info': 'connectionInfo',
-        'pred_params': 'predParams'
+        'workspace_id': 'workspaceId',
+        'project_ids': 'projectIds'
     }
 
-    def __init__(self, connection_info=None, pred_params=None):  # noqa: E501
-        """TestrunPredInfo - a model defined in Swagger"""  # noqa: E501
-        self._connection_info = None
-        self._pred_params = None
+    def __init__(self, workspace_id=None, project_ids=None):  # noqa: E501
+        """UserFavoriteProjects - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
+        self._project_ids = None
         self.discriminator = None
-        if connection_info is not None:
-            self.connection_info = connection_info
-        if pred_params is not None:
-            self.pred_params = pred_params
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
+        if project_ids is not None:
+            self.project_ids = project_ids
 
     @property
-    def connection_info(self):
-        """Gets the connection_info of this TestrunPredInfo.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this UserFavoriteProjects.  # noqa: E501
 
 
-        :return: The connection_info of this TestrunPredInfo.  # noqa: E501
-        :rtype: TestrunConnectionInfo
+        :return: The workspace_id of this UserFavoriteProjects.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._connection_info
+        return self._workspace_id
 
-    @connection_info.setter
-    def connection_info(self, connection_info):
-        """Sets the connection_info of this TestrunPredInfo.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this UserFavoriteProjects.
 
 
-        :param connection_info: The connection_info of this TestrunPredInfo.  # noqa: E501
-        :type: TestrunConnectionInfo
+        :param workspace_id: The workspace_id of this UserFavoriteProjects.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._connection_info = connection_info
+        self._workspace_id = workspace_id
 
     @property
-    def pred_params(self):
-        """Gets the pred_params of this TestrunPredInfo.  # noqa: E501
+    def project_ids(self):
+        """Gets the project_ids of this UserFavoriteProjects.  # noqa: E501
 
 
-        :return: The pred_params of this TestrunPredInfo.  # noqa: E501
-        :rtype: TestrunPredictionParams
+        :return: The project_ids of this UserFavoriteProjects.  # noqa: E501
+        :rtype: list[RimeUUID]
         """
-        return self._pred_params
+        return self._project_ids
 
-    @pred_params.setter
-    def pred_params(self, pred_params):
-        """Sets the pred_params of this TestrunPredInfo.
+    @project_ids.setter
+    def project_ids(self, project_ids):
+        """Sets the project_ids of this UserFavoriteProjects.
 
 
-        :param pred_params: The pred_params of this TestrunPredInfo.  # noqa: E501
-        :type: TestrunPredictionParams
+        :param project_ids: The project_ids of this UserFavoriteProjects.  # noqa: E501
+        :type: list[RimeUUID]
         """
 
-        self._pred_params = pred_params
+        self._project_ids = project_ids
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunPredInfo, dict):
+        if issubclass(UserFavoriteProjects, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunPredInfo):
+        if not isinstance(other, UserFavoriteProjects):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,91 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunPredictionParams(object):
+class UsersUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'pred_col': 'str',
-        'timestamp_col': 'str'
+        'user': 'V1usersuserIdUuidUser',
+        'mask': 'RimeUserWriteMask'
     }
 
     attribute_map = {
-        'pred_col': 'predCol',
-        'timestamp_col': 'timestampCol'
+        'user': 'user',
+        'mask': 'mask'
     }
 
-    def __init__(self, pred_col=None, timestamp_col=None):  # noqa: E501
-        """TestrunPredictionParams - a model defined in Swagger"""  # noqa: E501
-        self._pred_col = None
-        self._timestamp_col = None
+    def __init__(self, user=None, mask=None):  # noqa: E501
+        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._mask = None
         self.discriminator = None
-        if pred_col is not None:
-            self.pred_col = pred_col
-        if timestamp_col is not None:
-            self.timestamp_col = timestamp_col
+        if user is not None:
+            self.user = user
+        if mask is not None:
+            self.mask = mask
 
     @property
-    def pred_col(self):
-        """Gets the pred_col of this TestrunPredictionParams.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
 
-        Column used for predictions.  # noqa: E501
 
-        :return: The pred_col of this TestrunPredictionParams.  # noqa: E501
-        :rtype: str
+        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: V1usersuserIdUuidUser
         """
-        return self._pred_col
+        return self._user
 
-    @pred_col.setter
-    def pred_col(self, pred_col):
-        """Sets the pred_col of this TestrunPredictionParams.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserIdUuidBody.
 
-        Column used for predictions.  # noqa: E501
 
-        :param pred_col: The pred_col of this TestrunPredictionParams.  # noqa: E501
-        :type: str
+        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :type: V1usersuserIdUuidUser
         """
 
-        self._pred_col = pred_col
+        self._user = user
 
     @property
-    def timestamp_col(self):
-        """Gets the timestamp_col of this TestrunPredictionParams.  # noqa: E501
+    def mask(self):
+        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
 
-        Column used for CT timestamp.  # noqa: E501
 
-        :return: The timestamp_col of this TestrunPredictionParams.  # noqa: E501
-        :rtype: str
+        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: RimeUserWriteMask
         """
-        return self._timestamp_col
+        return self._mask
 
-    @timestamp_col.setter
-    def timestamp_col(self, timestamp_col):
-        """Sets the timestamp_col of this TestrunPredictionParams.
+    @mask.setter
+    def mask(self, mask):
+        """Sets the mask of this UsersUserIdUuidBody.
 
-        Column used for CT timestamp.  # noqa: E501
 
-        :param timestamp_col: The timestamp_col of this TestrunPredictionParams.  # noqa: E501
-        :type: str
+        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :type: RimeUserWriteMask
         """
 
-        self._timestamp_col = timestamp_col
+        self._mask = mask
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunPredictionParams, dict):
+        if issubclass(UsersUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunPredictionParams):
+        if not isinstance(other, UsersUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,84 +11,84 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunSingleDataInfo(object):
+class SchemaregistryDataInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'connection_info': 'TestrunConnectionInfo',
-        'data_params': 'TestrunDataInfoParams'
+        'connection_info': 'RegistryConnectionInfo',
+        'data_params': 'RegistryDataParams'
     }
 
     attribute_map = {
         'connection_info': 'connectionInfo',
         'data_params': 'dataParams'
     }
 
     def __init__(self, connection_info=None, data_params=None):  # noqa: E501
-        """TestrunSingleDataInfo - a model defined in Swagger"""  # noqa: E501
+        """SchemaregistryDataInfo - a model defined in Swagger"""  # noqa: E501
         self._connection_info = None
         self._data_params = None
         self.discriminator = None
         if connection_info is not None:
             self.connection_info = connection_info
         if data_params is not None:
             self.data_params = data_params
 
     @property
     def connection_info(self):
-        """Gets the connection_info of this TestrunSingleDataInfo.  # noqa: E501
+        """Gets the connection_info of this SchemaregistryDataInfo.  # noqa: E501
 
 
-        :return: The connection_info of this TestrunSingleDataInfo.  # noqa: E501
-        :rtype: TestrunConnectionInfo
+        :return: The connection_info of this SchemaregistryDataInfo.  # noqa: E501
+        :rtype: RegistryConnectionInfo
         """
         return self._connection_info
 
     @connection_info.setter
     def connection_info(self, connection_info):
-        """Sets the connection_info of this TestrunSingleDataInfo.
+        """Sets the connection_info of this SchemaregistryDataInfo.
 
 
-        :param connection_info: The connection_info of this TestrunSingleDataInfo.  # noqa: E501
-        :type: TestrunConnectionInfo
+        :param connection_info: The connection_info of this SchemaregistryDataInfo.  # noqa: E501
+        :type: RegistryConnectionInfo
         """
 
         self._connection_info = connection_info
 
     @property
     def data_params(self):
-        """Gets the data_params of this TestrunSingleDataInfo.  # noqa: E501
+        """Gets the data_params of this SchemaregistryDataInfo.  # noqa: E501
 
 
-        :return: The data_params of this TestrunSingleDataInfo.  # noqa: E501
-        :rtype: TestrunDataInfoParams
+        :return: The data_params of this SchemaregistryDataInfo.  # noqa: E501
+        :rtype: RegistryDataParams
         """
         return self._data_params
 
     @data_params.setter
     def data_params(self, data_params):
-        """Sets the data_params of this TestrunSingleDataInfo.
+        """Sets the data_params of this SchemaregistryDataInfo.
 
 
-        :param data_params: The data_params of this TestrunSingleDataInfo.  # noqa: E501
-        :type: TestrunDataInfoParams
+        :param data_params: The data_params of this SchemaregistryDataInfo.  # noqa: E501
+        :type: RegistryDataParams
         """
 
         self._data_params = data_params
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunSingleDataInfo, dict):
+        if issubclass(SchemaregistryDataInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunSingleDataInfo):
+        if not isinstance(other, SchemaregistryDataInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'run_name': 'str',
         'model_id': 'RimeUUID',
-        'data_info': 'TestrunDataInfo',
+        'data_info': 'SchematestrunDataInfo',
         'run_time_info': 'RuntimeinfoRunTimeInfo',
         'profiling_config': 'TestrunProfilingConfig',
         'test_suite_config': 'TestrunTestSuiteConfig',
         'categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
@@ -119,25 +119,25 @@
 
     @property
     def data_info(self):
         """Gets the data_info of this TestrunTestRunConfig.  # noqa: E501
 
 
         :return: The data_info of this TestrunTestRunConfig.  # noqa: E501
-        :rtype: TestrunDataInfo
+        :rtype: SchematestrunDataInfo
         """
         return self._data_info
 
     @data_info.setter
     def data_info(self, data_info):
         """Sets the data_info of this TestrunTestRunConfig.
 
 
         :param data_info: The data_info of this TestrunTestRunConfig.  # noqa: E501
-        :type: TestrunDataInfo
+        :type: SchematestrunDataInfo
         """
         if data_info is None:
             raise ValueError("Invalid value for `data_info`, must not be `None`")  # noqa: E501
 
         self._data_info = data_info
 
     @property
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserFavoriteProjects(object):
+class UsersUserUserIdUuidBody1(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'workspace_id': 'RimeUUID',
-        'project_ids': 'list[RimeUUID]'
+        'workspace_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'project_ids': 'projectIds'
+        'user': 'user'
     }
 
-    def __init__(self, workspace_id=None, project_ids=None):  # noqa: E501
-        """UserFavoriteProjects - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._project_ids = None
+        self._user = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        if project_ids is not None:
-            self.project_ids = project_ids
+        if user is not None:
+            self.user = user
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this UserFavoriteProjects.  # noqa: E501
+        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UserFavoriteProjects.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UserFavoriteProjects.
+        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UserFavoriteProjects.  # noqa: E501
-        :type: RimeUUID
+        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def project_ids(self):
-        """Gets the project_ids of this UserFavoriteProjects.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
 
 
-        :return: The project_ids of this UserFavoriteProjects.  # noqa: E501
-        :rtype: list[RimeUUID]
+        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._project_ids
+        return self._user
 
-    @project_ids.setter
-    def project_ids(self, project_ids):
-        """Sets the project_ids of this UserFavoriteProjects.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody1.
 
 
-        :param project_ids: The project_ids of this UserFavoriteProjects.  # noqa: E501
-        :type: list[RimeUUID]
+        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._project_ids = project_ids
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserFavoriteProjects, dict):
+        if issubclass(UsersUserUserIdUuidBody1, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserFavoriteProjects):
+        if not isinstance(other, UsersUserUserIdUuidBody1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserIdUuidBody(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'user': 'V1usersuserIdUuidUser',
-        'mask': 'RimeUserWriteMask'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'user': 'user',
-        'mask': 'mask'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, user=None, mask=None):  # noqa: E501
-        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
-        self._user = None
-        self._mask = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if user is not None:
-            self.user = user
-        if mask is not None:
-            self.mask = mask
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: V1usersuserIdUuidUser
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: object
         """
-        return self._user
+        return self._user_id
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserIdUuidBody.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :type: V1usersuserIdUuidUser
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: object
         """
 
-        self._user = user
+        self._user_id = user_id
 
     @property
-    def mask(self):
-        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: RimeUserWriteMask
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._mask
+        return self._user_role
 
-    @mask.setter
-    def mask(self, mask):
-        """Sets the mask of this UsersUserIdUuidBody.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :type: RimeUserWriteMask
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._mask = mask
+        self._user_role = user_role
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserIdUuidBody, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserIdUuidBody):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,89 +11,92 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody1(object):
+class WorkspaceIdUuidTagsBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'name': 'str'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'user': 'user'
+        'name': 'name'
     }
 
-    def __init__(self, workspace_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, name=None):  # noqa: E501
+        """WorkspaceIdUuidTagsBody - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._user = None
+        self._name = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        if user is not None:
-            self.user = user
+        self.name = name
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        """Gets the workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
         :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
+        """Sets the workspace_id of this WorkspaceIdUuidTagsBody.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
         :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def name(self):
+        """Gets the name of this WorkspaceIdUuidTagsBody.  # noqa: E501
 
+        Name of the tag.  # noqa: E501
 
-        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :rtype: str
         """
-        return self._user
+        return self._name
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody1.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this WorkspaceIdUuidTagsBody.
 
+        Name of the tag.  # noqa: E501
 
-        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param name: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._user = user
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +111,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody1, dict):
+        if issubclass(WorkspaceIdUuidTagsBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +127,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody1):
+        if not isinstance(other, WorkspaceIdUuidTagsBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,92 +11,91 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WorkspaceIdUuidTagsBody(object):
+class WorkspaceIdUuidUsersBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'object',
-        'name': 'str'
+        'users': 'list[RimeUserWithRole]'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'name': 'name'
+        'users': 'users'
     }
 
-    def __init__(self, workspace_id=None, name=None):  # noqa: E501
-        """WorkspaceIdUuidTagsBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, users=None):  # noqa: E501
+        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._name = None
+        self._users = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        self.name = name
+        if users is not None:
+            self.users = users
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this WorkspaceIdUuidTagsBody.
+        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def name(self):
-        """Gets the name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+    def users(self):
+        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
-        Name of the tag.  # noqa: E501
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :return: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
-        :rtype: str
+        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :rtype: list[RimeUserWithRole]
         """
-        return self._name
+        return self._users
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this WorkspaceIdUuidTagsBody.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this WorkspaceIdUuidUsersBody.
 
-        Name of the tag.  # noqa: E501
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :param name: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
-        :type: str
+        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :type: list[RimeUserWithRole]
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._users = users
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -111,15 +110,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkspaceIdUuidTagsBody, dict):
+        if issubclass(WorkspaceIdUuidUsersBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -127,15 +126,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkspaceIdUuidTagsBody):
+        if not isinstance(other, WorkspaceIdUuidUsersBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.1.0rc3/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/test_batch.py` & `rime_sdk-2.1.0rc3/rime_sdk/test_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,17 @@
                     9. summary_counts.total
                     10. summary_counts.pass
                     11. summary_counts.fail
                     12. summary_counts.warning
                     13. summary_counts.skip
         """
         res = get_batch_result_response(
-            self._test_run_id, self._test_type, self._api_client,
+            self._test_run_id,
+            self._test_type,
+            self._api_client,
         )
         return parse_test_batch_result(
             res.test_batch, unpack_metrics=show_batch_metrics
         )
 
     def get_test_cases_df(self) -> pd.DataFrame:
         """Return all Test Cases in the Test Batch as a Pandas DataFrame.
@@ -113,15 +115,16 @@
                     res = api.results_reader_list_test_cases(
                         list_test_cases_query_test_run_id=self._test_run_id,
                         list_test_cases_query_test_types=[self._test_type],
                         page_size=20,
                     )
                 else:
                     res = api.results_reader_list_test_cases(
-                        page_token=page_token, page_size=20,
+                        page_token=page_token,
+                        page_size=20,
                     )
             if res.test_cases:
                 tc_dicts = [
                     parse_test_case_result(tc, unpack_metrics=True)
                     for tc in res.test_cases
                 ]
                 # Concatenate the list of Test Case dictionaries.
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk/test_run.py` & `rime_sdk-2.1.0rc3/rime_sdk/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,16 @@
                 if page_token == "":
                     res = api.results_reader_list_test_cases(
                         page_size=20,
                         list_test_cases_query_test_run_id=self._test_run_id,
                     )
                 else:
                     res = api.results_reader_list_test_cases(
-                        page_size=20, page_token=page_token,
+                        page_size=20,
+                        page_token=page_token,
                     )
             if res.test_cases:
                 tc_dicts = [
                     parse_test_case_result(tc, unpack_metrics=show_test_case_metrics)
                     for tc in res.test_cases
                 ]
                 # Concatenate the list of Test Case dictionaries.
@@ -208,33 +209,36 @@
         api = swagger_client.ResultsReaderApi(self._api_client)
         # Iterate through the pages of Test Cases and break at the last page.
         page_token = ""
         while True:
             with RESTErrorHandler():
                 if page_token == "":
                     res = api.results_reader_list_batch_results(
-                        page_size=20, test_run_id=self._test_run_id,
+                        page_size=20,
+                        test_run_id=self._test_run_id,
                     )
                 else:
                     res = api.results_reader_list_batch_results(
-                        page_size=20, page_token=page_token,
+                        page_size=20,
+                        page_token=page_token,
                     )
             if res.test_batches:
                 for test_batch in res.test_batches:
                     yield TestBatch(
                         self._api_client, self._test_run_id, test_batch.test_type
                     )
             # Advance to the next page of Test Cases.
             page_token = res.next_page_token
             # we've reached the last page of Test Cases.
             if not res.has_more:
                 break
 
     def get_summary_tests_df(
-        self, show_summary_test_metrics: bool = False,
+        self,
+        show_summary_test_metrics: bool = False,
     ) -> pd.DataFrame:
         """Get summary tests for a completed stress Test Run in a dataframe.
 
         This gives you the ability to perform granular queries on summary tests.
         This only works on stress test jobs that have succeeded.
 
         Returns:
@@ -265,24 +269,27 @@
         all_summary_tests = []
         # Iterate through the pages of Test Cases and break at the last page.
         page_token = ""
         while True:
             with RESTErrorHandler():
                 if page_token == "":
                     res = api.results_reader_list_summary_tests(
-                        page_size=20, query_test_run_id=self._test_run_id,
+                        page_size=20,
+                        query_test_run_id=self._test_run_id,
                     )
                 else:
                     res = api.results_reader_list_summary_tests(
-                        page_size=20, page_token=page_token,
+                        page_size=20,
+                        page_token=page_token,
                     )
             if res.summary_test_results:
                 for summary_test_result in res.summary_test_results:
                     parsed_result = parse_summary_test_result(
-                        summary_test_result, unpack_metrics=show_summary_test_metrics,
+                        summary_test_result,
+                        unpack_metrics=show_summary_test_metrics,
                     )
                     all_summary_tests.append(parsed_result)
             # Advance to the next page of Test Cases.
             page_token = res.next_page_token
             # we've reached the last page of Test Cases.
             if not res.has_more:
                 break
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.1.0rc3/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc2/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.1.0rc3/rime_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 rime_sdk/swagger/swagger_client/api/config_validator_api.py
 rime_sdk/swagger/swagger_client/api/data_collector_api.py
 rime_sdk/swagger/swagger_client/api/detection_api.py
 rime_sdk/swagger/swagger_client/api/feature_flag_api.py
 rime_sdk/swagger/swagger_client/api/file_scanning_api.py
 rime_sdk/swagger/swagger_client/api/file_upload_api.py
 rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
 rime_sdk/swagger/swagger_client/api/image_registry_api.py
 rime_sdk/swagger/swagger_client/api/integration_service_api.py
 rime_sdk/swagger/swagger_client/api/job_reader_api.py
 rime_sdk/swagger/swagger_client/api/model_card_service_api.py
 rime_sdk/swagger/swagger_client/api/model_testing_api.py
 rime_sdk/swagger/swagger_client/api/monitor_service_api.py
 rime_sdk/swagger/swagger_client/api/notification_setting_api.py
@@ -74,16 +75,16 @@
 rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
 rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
 rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
 rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
 rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
 rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
-rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
-rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
+rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
 rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
 rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
 rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
 rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
 rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
 rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
 rime_sdk/swagger/swagger_client/models/dataset_dataset.py
@@ -106,14 +107,17 @@
 rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
+rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
+rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
 rime_sdk/swagger/swagger_client/models/integration_integration_type.py
 rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
@@ -135,18 +139,15 @@
 rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
 rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
 rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
 rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
 rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
 rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
 rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
-rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/model_model.py
-rime_sdk/swagger/swagger_client/models/model_model_info.py
-rime_sdk/swagger/swagger_client/models/model_model_path_info.py
 rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
 rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
 rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
 rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
 rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
 rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
@@ -191,15 +192,27 @@
 rime_sdk/swagger/swagger_client/models/protobuf_any.py
 rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
 rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
 rime_sdk/swagger/swagger_client/models/rca_rca_result.py
 rime_sdk/swagger/swagger_client/models/rca_rca_role.py
 rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
 rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_params.py
+rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
+rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_metadata.py
+rime_sdk/swagger/swagger_client/models/registry_model_info.py
+rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
 rime_sdk/swagger/swagger_client/models/registry_validity_status.py
 rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
 rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
 rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/rime_actor_role.py
 rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_agent.py
@@ -255,14 +268,15 @@
 rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
@@ -280,14 +294,15 @@
 rime_sdk/swagger/swagger_client/models/rime_image_reference.py
 rime_sdk/swagger/swagger_client/models/rime_int_list.py
 rime_sdk/swagger/swagger_client/models/rime_integration_info.py
 rime_sdk/swagger/swagger_client/models/rime_job_data.py
 rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
 rime_sdk/swagger/swagger_client/models/rime_job_type.py
 rime_sdk/swagger/swagger_client/models/rime_job_view.py
+rime_sdk/swagger/swagger_client/models/rime_language.py
 rime_sdk/swagger/swagger_client/models/rime_license_feature.py
 rime_sdk/swagger/swagger_client/models/rime_license_limit.py
 rime_sdk/swagger/swagger_client/models/rime_limit_status.py
 rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
 rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
@@ -338,14 +353,17 @@
 rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
 rime_sdk/swagger/swagger_client/models/rime_severity.py
 rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
 rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
 rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
+rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
+rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
 rime_sdk/swagger/swagger_client/models/rime_str_list.py
 rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
 rime_sdk/swagger/swagger_client/models/rime_subject_type.py
@@ -391,42 +409,34 @@
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
 rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
 rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
 rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
 rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+rime_sdk/swagger/swagger_client/models/schemaregistry_data_info.py
+rime_sdk/swagger/swagger_client/models/schematestrun_data_info.py
 rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
 rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
 rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/statedb_job_status.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
 rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/tags_name_body.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
 rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
-rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
 rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
-rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
-rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
-rime_sdk/swagger/swagger_client/models/testrun_data_info.py
-rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
-rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
 rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
-rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
-rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
+rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
-rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
-rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
 rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
-rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
 rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
 rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
```

### Comparing `rime_sdk-2.1.0rc2/setup.py` & `rime_sdk-2.1.0rc3/setup.py`

 * *Files identical despite different names*

