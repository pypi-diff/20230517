# Comparing `tmp/humanloop-0.4.0.tar.gz` & `tmp/humanloop-0.4.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanloop-0.4.0.tar", max compression
+gzip compressed data, was "humanloop-0.4.0a4.tar", max compression
```

## Comparing `humanloop-0.4.0.tar` & `humanloop-0.4.0a4.tar`

### file list

```diff
@@ -1,371 +1,371 @@
--rw-r--r--   0        0        0     1081 2023-05-17 00:32:28.110883 humanloop-0.4.0/LICENSE
--rw-r--r--   0        0        0     8180 2023-05-17 00:32:28.161333 humanloop-0.4.0/README.md
--rw-r--r--   0        0        0     1059 2023-05-17 00:32:27.984855 humanloop-0.4.0/humanloop/__init__.py
--rw-r--r--   0        0        0    73009 2023-05-17 00:32:27.985162 humanloop-0.4.0/humanloop/api_client.py
--rw-r--r--   0        0        0      663 2023-05-17 00:32:27.985345 humanloop-0.4.0/humanloop/api_response.py
--rw-r--r--   0        0        0      214 2023-05-17 00:32:27.985504 humanloop-0.4.0/humanloop/apis/__init__.py
--rw-r--r--   0        0        0     5316 2023-05-17 00:32:27.985681 humanloop-0.4.0/humanloop/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-17 00:32:27.985862 humanloop-0.4.0/humanloop/apis/paths/__init__.py
--rw-r--r--   0        0        0       88 2023-05-17 00:32:27.986014 humanloop-0.4.0/humanloop/apis/paths/apps.py
--rw-r--r--   0        0        0       93 2023-05-17 00:32:27.986180 humanloop-0.4.0/humanloop/apis/paths/apps_id.py
--rw-r--r--   0        0        0      110 2023-05-17 00:32:27.986345 humanloop-0.4.0/humanloop/apis/paths/apps_id_sessions.py
--rw-r--r--   0        0        0       91 2023-05-17 00:32:27.986496 humanloop-0.4.0/humanloop/apis/paths/chat.py
--rw-r--r--   0        0        0      108 2023-05-17 00:32:27.986674 humanloop-0.4.0/humanloop/apis/paths/chat_deployed.py
--rw-r--r--   0        0        0      112 2023-05-17 00:32:27.986839 humanloop-0.4.0/humanloop/apis/paths/chat_experiment.py
--rw-r--r--   0        0        0      115 2023-05-17 00:32:27.987024 humanloop-0.4.0/humanloop/apis/paths/chat_model_config.py
--rw-r--r--   0        0        0      103 2023-05-17 00:32:27.987208 humanloop-0.4.0/humanloop/apis/paths/completion.py
--rw-r--r--   0        0        0      120 2023-05-17 00:32:27.987371 humanloop-0.4.0/humanloop/apis/paths/completion_deployed.py
--rw-r--r--   0        0        0      124 2023-05-17 00:32:27.987520 humanloop-0.4.0/humanloop/apis/paths/completion_experiment.py
--rw-r--r--   0        0        0      127 2023-05-17 00:32:27.987674 humanloop-0.4.0/humanloop/apis/paths/completion_model_config.py
--rw-r--r--   0        0        0      226 2023-05-17 00:32:27.987836 humanloop-0.4.0/humanloop/apis/paths/experiments_experiment_id.py
--rw-r--r--   0        0        0      152 2023-05-17 00:32:27.987984 humanloop-0.4.0/humanloop/apis/paths/experiments_experiment_id_model_config.py
--rw-r--r--   0        0        0       99 2023-05-17 00:32:27.988082 humanloop-0.4.0/humanloop/apis/paths/feedback.py
--rw-r--r--   0        0        0       91 2023-05-17 00:32:27.988190 humanloop-0.4.0/humanloop/apis/paths/logs.py
--rw-r--r--   0        0        0      108 2023-05-17 00:32:27.988329 humanloop-0.4.0/humanloop/apis/paths/model_configs.py
--rw-r--r--   0        0        0      110 2023-05-17 00:32:27.988470 humanloop-0.4.0/humanloop/apis/paths/model_configs_id.py
--rw-r--r--   0        0        0      165 2023-05-17 00:32:27.988608 humanloop-0.4.0/humanloop/apis/paths/projects.py
--rw-r--r--   0        0        0      176 2023-05-17 00:32:27.988830 humanloop-0.4.0/humanloop/apis/paths/projects_id.py
--rw-r--r--   0        0        0      144 2023-05-17 00:32:27.989063 humanloop-0.4.0/humanloop/apis/paths/projects_id_active_experiment.py
--rw-r--r--   0        0        0      147 2023-05-17 00:32:28.001771 humanloop-0.4.0/humanloop/apis/paths/projects_id_active_model_config.py
--rw-r--r--   0        0        0      117 2023-05-17 00:32:28.002080 humanloop-0.4.0/humanloop/apis/paths/projects_id_export.py
--rw-r--r--   0        0        0      135 2023-05-17 00:32:28.002213 humanloop-0.4.0/humanloop/apis/paths/projects_id_feedback_types.py
--rw-r--r--   0        0        0      125 2023-05-17 00:32:28.002326 humanloop-0.4.0/humanloop/apis/paths/projects_id_model_config.py
--rw-r--r--   0        0        0      127 2023-05-17 00:32:28.002438 humanloop-0.4.0/humanloop/apis/paths/projects_id_model_configs.py
--rw-r--r--   0        0        0      231 2023-05-17 00:32:28.002544 humanloop-0.4.0/humanloop/apis/paths/projects_project_id_experiments.py
--rw-r--r--   0        0        0       99 2023-05-17 00:32:28.002641 humanloop-0.4.0/humanloop/apis/paths/sessions.py
--rw-r--r--   0        0        0      101 2023-05-17 00:32:28.002755 humanloop-0.4.0/humanloop/apis/paths/sessions_id.py
--rw-r--r--   0        0        0      114 2023-05-17 00:32:28.002870 humanloop-0.4.0/humanloop/apis/paths/sessions_id_events.py
--rw-r--r--   0        0        0     1642 2023-05-17 00:32:28.002987 humanloop-0.4.0/humanloop/apis/tag_to_api.py
--rw-r--r--   0        0        0      568 2023-05-17 00:32:28.003108 humanloop-0.4.0/humanloop/apis/tags/__init__.py
--rw-r--r--   0        0        0      839 2023-05-17 00:32:28.003250 humanloop-0.4.0/humanloop/apis/tags/apps_api.py
--rw-r--r--   0        0        0     1006 2023-05-17 00:32:28.003424 humanloop-0.4.0/humanloop/apis/tags/chats_api.py
--rw-r--r--   0        0        0     1020 2023-05-17 00:32:28.003580 humanloop-0.4.0/humanloop/apis/tags/completions_api.py
--rw-r--r--   0        0        0     1091 2023-05-17 00:32:28.024050 humanloop-0.4.0/humanloop/apis/tags/experiments_api.py
--rw-r--r--   0        0        0      721 2023-05-17 00:32:28.024396 humanloop-0.4.0/humanloop/apis/tags/feedback_api.py
--rw-r--r--   0        0        0      707 2023-05-17 00:32:28.024792 humanloop-0.4.0/humanloop/apis/tags/logs_api.py
--rw-r--r--   0        0        0      803 2023-05-17 00:32:28.025036 humanloop-0.4.0/humanloop/apis/tags/model_configurations_api.py
--rw-r--r--   0        0        0     1519 2023-05-17 00:32:28.025190 humanloop-0.4.0/humanloop/apis/tags/projects_api.py
--rw-r--r--   0        0        0      854 2023-05-17 00:32:28.025308 humanloop-0.4.0/humanloop/apis/tags/sessions_api.py
--rw-r--r--   0        0        0    27541 2023-05-17 00:32:28.025538 humanloop-0.4.0/humanloop/client.py
--rw-r--r--   0        0        0    27541 2023-05-17 00:32:28.025829 humanloop-0.4.0/humanloop/client.pyi
--rw-r--r--   0        0        0     7106 2023-05-17 00:42:45.818667 humanloop-0.4.0/humanloop/client_custom.py
--rw-r--r--   0        0        0    18309 2023-05-17 00:32:28.026078 humanloop-0.4.0/humanloop/configuration.py
--rw-r--r--   0        0        0     7678 2023-05-17 00:32:28.026250 humanloop-0.4.0/humanloop/exceptions.py
--rw-r--r--   0        0        0     2274 2023-05-17 00:32:28.026399 humanloop-0.4.0/humanloop/exceptions_base.py
--rw-r--r--   0        0        0      343 2023-05-17 00:32:28.026602 humanloop-0.4.0/humanloop/model/__init__.py
--rw-r--r--   0        0        0     6379 2023-05-17 00:32:28.026751 humanloop-0.4.0/humanloop/model/base_metric_response.py
--rw-r--r--   0        0        0     6379 2023-05-17 00:32:28.026912 humanloop-0.4.0/humanloop/model/base_metric_response.pyi
--rw-r--r--   0        0        0     5150 2023-05-17 00:32:28.027058 humanloop-0.4.0/humanloop/model/categorical_feedback_label.py
--rw-r--r--   0        0        0     5150 2023-05-17 00:32:28.027213 humanloop-0.4.0/humanloop/model/categorical_feedback_label.pyi
--rw-r--r--   0        0        0     8957 2023-05-17 00:32:28.027390 humanloop-0.4.0/humanloop/model/chat_data_response.py
--rw-r--r--   0        0        0     8957 2023-05-17 00:32:28.027809 humanloop-0.4.0/humanloop/model/chat_data_response.pyi
--rw-r--r--   0        0        0     9998 2023-05-17 00:32:28.028017 humanloop-0.4.0/humanloop/model/chat_deployed_request.py
--rw-r--r--   0        0        0     9998 2023-05-17 00:32:28.028282 humanloop-0.4.0/humanloop/model/chat_deployed_request.pyi
--rw-r--r--   0        0        0    10659 2023-05-17 00:32:28.028502 humanloop-0.4.0/humanloop/model/chat_experiment_request.py
--rw-r--r--   0        0        0    10659 2023-05-17 00:32:28.028846 humanloop-0.4.0/humanloop/model/chat_experiment_request.pyi
--rw-r--r--   0        0        0     3702 2023-05-17 00:32:28.029149 humanloop-0.4.0/humanloop/model/chat_message.py
--rw-r--r--   0        0        0     3702 2023-05-17 00:32:28.030165 humanloop-0.4.0/humanloop/model/chat_message.pyi
--rw-r--r--   0        0        0    10693 2023-05-17 00:32:28.030383 humanloop-0.4.0/humanloop/model/chat_model_config_request.py
--rw-r--r--   0        0        0    10693 2023-05-17 00:32:28.030596 humanloop-0.4.0/humanloop/model/chat_model_config_request.pyi
--rw-r--r--   0        0        0    12556 2023-05-17 00:32:28.030804 humanloop-0.4.0/humanloop/model/chat_request.py
--rw-r--r--   0        0        0    12556 2023-05-17 00:32:28.031073 humanloop-0.4.0/humanloop/model/chat_request.pyi
--rw-r--r--   0        0        0    11076 2023-05-17 00:32:28.031285 humanloop-0.4.0/humanloop/model/chat_response.py
--rw-r--r--   0        0        0    11076 2023-05-17 00:32:28.031504 humanloop-0.4.0/humanloop/model/chat_response.pyi
--rw-r--r--   0        0        0     1446 2023-05-17 00:32:28.031696 humanloop-0.4.0/humanloop/model/chat_role.py
--rw-r--r--   0        0        0     1285 2023-05-17 00:32:28.031844 humanloop-0.4.0/humanloop/model/chat_role.pyi
--rw-r--r--   0        0        0     9674 2023-05-17 00:32:28.031994 humanloop-0.4.0/humanloop/model/completion_deployed_request.py
--rw-r--r--   0        0        0     9674 2023-05-17 00:32:28.032155 humanloop-0.4.0/humanloop/model/completion_deployed_request.pyi
--rw-r--r--   0        0        0    10340 2023-05-17 00:32:28.032487 humanloop-0.4.0/humanloop/model/completion_experiment_request.py
--rw-r--r--   0        0        0    10340 2023-05-17 00:32:28.032710 humanloop-0.4.0/humanloop/model/completion_experiment_request.pyi
--rw-r--r--   0        0        0    10376 2023-05-17 00:32:28.032937 humanloop-0.4.0/humanloop/model/completion_model_config_request.py
--rw-r--r--   0        0        0    10376 2023-05-17 00:32:28.033079 humanloop-0.4.0/humanloop/model/completion_model_config_request.pyi
--rw-r--r--   0        0        0    12258 2023-05-17 00:32:28.033373 humanloop-0.4.0/humanloop/model/completion_request.py
--rw-r--r--   0        0        0    12258 2023-05-17 00:32:28.033602 humanloop-0.4.0/humanloop/model/completion_request.pyi
--rw-r--r--   0        0        0    11017 2023-05-17 00:32:28.033840 humanloop-0.4.0/humanloop/model/completion_response.py
--rw-r--r--   0        0        0    11017 2023-05-17 00:32:28.034047 humanloop-0.4.0/humanloop/model/completion_response.pyi
--rw-r--r--   0        0        0     6280 2023-05-17 00:32:28.034171 humanloop-0.4.0/humanloop/model/create_experiment_request.py
--rw-r--r--   0        0        0     6280 2023-05-17 00:32:28.034299 humanloop-0.4.0/humanloop/model/create_experiment_request.pyi
--rw-r--r--   0        0        0     3199 2023-05-17 00:32:28.034443 humanloop-0.4.0/humanloop/model/create_log_response.py
--rw-r--r--   0        0        0     3199 2023-05-17 00:32:28.034566 humanloop-0.4.0/humanloop/model/create_log_response.pyi
--rw-r--r--   0        0        0     4266 2023-05-17 00:32:28.034707 humanloop-0.4.0/humanloop/model/create_project_request.py
--rw-r--r--   0        0        0     4266 2023-05-17 00:32:28.034858 humanloop-0.4.0/humanloop/model/create_project_request.pyi
--rw-r--r--   0        0        0     2649 2023-05-17 00:32:28.034976 humanloop-0.4.0/humanloop/model/create_session_request.py
--rw-r--r--   0        0        0     2649 2023-05-17 00:32:28.035104 humanloop-0.4.0/humanloop/model/create_session_request.pyi
--rw-r--r--   0        0        0     7455 2023-05-17 00:32:28.035237 humanloop-0.4.0/humanloop/model/data_response.py
--rw-r--r--   0        0        0     7455 2023-05-17 00:32:28.035379 humanloop-0.4.0/humanloop/model/data_response.pyi
--rw-r--r--   0        0        0     9235 2023-05-17 00:32:28.035542 humanloop-0.4.0/humanloop/model/experiment_model_config_response.py
--rw-r--r--   0        0        0     9235 2023-05-17 00:32:28.035746 humanloop-0.4.0/humanloop/model/experiment_model_config_response.pyi
--rw-r--r--   0        0        0    12947 2023-05-17 00:32:28.035899 humanloop-0.4.0/humanloop/model/experiment_response.py
--rw-r--r--   0        0        0    12947 2023-05-17 00:32:28.036019 humanloop-0.4.0/humanloop/model/experiment_response.pyi
--rw-r--r--   0        0        0     1376 2023-05-17 00:32:28.036346 humanloop-0.4.0/humanloop/model/experiment_status.py
--rw-r--r--   0        0        0     1229 2023-05-17 00:32:28.036478 humanloop-0.4.0/humanloop/model/experiment_status.pyi
--rw-r--r--   0        0        0     1685 2023-05-17 00:32:28.036615 humanloop-0.4.0/humanloop/model/experiments_list_response.py
--rw-r--r--   0        0        0     1685 2023-05-17 00:32:28.036732 humanloop-0.4.0/humanloop/model/experiments_list_response.pyi
--rw-r--r--   0        0        0     6681 2023-05-17 00:32:28.036869 humanloop-0.4.0/humanloop/model/feedback.py
--rw-r--r--   0        0        0     6681 2023-05-17 00:32:28.036983 humanloop-0.4.0/humanloop/model/feedback.pyi
--rw-r--r--   0        0        0     1463 2023-05-17 00:32:28.037126 humanloop-0.4.0/humanloop/model/feedback_class.py
--rw-r--r--   0        0        0     1296 2023-05-17 00:32:28.037301 humanloop-0.4.0/humanloop/model/feedback_class.pyi
--rw-r--r--   0        0        0     3334 2023-05-17 00:32:28.037516 humanloop-0.4.0/humanloop/model/feedback_label_request.py
--rw-r--r--   0        0        0     3334 2023-05-17 00:32:28.037687 humanloop-0.4.0/humanloop/model/feedback_label_request.pyi
--rw-r--r--   0        0        0     7189 2023-05-17 00:32:28.037864 humanloop-0.4.0/humanloop/model/feedback_request.py
--rw-r--r--   0        0        0     7189 2023-05-17 00:32:28.038432 humanloop-0.4.0/humanloop/model/feedback_request.pyi
--rw-r--r--   0        0        0     7141 2023-05-17 00:32:28.038658 humanloop-0.4.0/humanloop/model/feedback_response.py
--rw-r--r--   0        0        0     7141 2023-05-17 00:32:28.038860 humanloop-0.4.0/humanloop/model/feedback_response.pyi
--rw-r--r--   0        0        0     3200 2023-05-17 00:32:28.039071 humanloop-0.4.0/humanloop/model/feedback_submit_request.py
--rw-r--r--   0        0        0     3200 2023-05-17 00:32:28.039272 humanloop-0.4.0/humanloop/model/feedback_submit_request.pyi
--rw-r--r--   0        0        0     3210 2023-05-17 00:32:28.039450 humanloop-0.4.0/humanloop/model/feedback_submit_response.py
--rw-r--r--   0        0        0     3210 2023-05-17 00:32:28.039620 humanloop-0.4.0/humanloop/model/feedback_submit_response.pyi
--rw-r--r--   0        0        0     1690 2023-05-17 00:32:28.039792 humanloop-0.4.0/humanloop/model/feedback_type.py
--rw-r--r--   0        0        0     1459 2023-05-17 00:32:28.039966 humanloop-0.4.0/humanloop/model/feedback_type.pyi
--rw-r--r--   0        0        0     6161 2023-05-17 00:32:28.040131 humanloop-0.4.0/humanloop/model/feedback_type_model.py
--rw-r--r--   0        0        0     6161 2023-05-17 00:32:28.040291 humanloop-0.4.0/humanloop/model/feedback_type_model.pyi
--rw-r--r--   0        0        0     6289 2023-05-17 00:32:28.040449 humanloop-0.4.0/humanloop/model/feedback_type_request.py
--rw-r--r--   0        0        0     6289 2023-05-17 00:32:28.040616 humanloop-0.4.0/humanloop/model/feedback_type_request.pyi
--rw-r--r--   0        0        0     1659 2023-05-17 00:32:28.040784 humanloop-0.4.0/humanloop/model/feedback_types.py
--rw-r--r--   0        0        0     1659 2023-05-17 00:32:28.040923 humanloop-0.4.0/humanloop/model/feedback_types.pyi
--rw-r--r--   0        0        0    24518 2023-05-17 00:32:28.041126 humanloop-0.4.0/humanloop/model/get_model_config_response.py
--rw-r--r--   0        0        0    24518 2023-05-17 00:32:28.041383 humanloop-0.4.0/humanloop/model/get_model_config_response.pyi
--rw-r--r--   0        0        0     3611 2023-05-17 00:32:28.041586 humanloop-0.4.0/humanloop/model/http_validation_error.py
--rw-r--r--   0        0        0     3611 2023-05-17 00:32:28.041743 humanloop-0.4.0/humanloop/model/http_validation_error.pyi
--rw-r--r--   0        0        0     1667 2023-05-17 00:32:28.041864 humanloop-0.4.0/humanloop/model/label_sentiment.py
--rw-r--r--   0        0        0     1468 2023-05-17 00:32:28.041971 humanloop-0.4.0/humanloop/model/label_sentiment.pyi
--rw-r--r--   0        0        0     3156 2023-05-17 00:32:28.042086 humanloop-0.4.0/humanloop/model/log_datapoint_request.py
--rw-r--r--   0        0        0     3156 2023-05-17 00:32:28.042352 humanloop-0.4.0/humanloop/model/log_datapoint_request.pyi
--rw-r--r--   0        0        0    14677 2023-05-17 00:32:28.042601 humanloop-0.4.0/humanloop/model/log_request.py
--rw-r--r--   0        0        0    14677 2023-05-17 00:32:28.042833 humanloop-0.4.0/humanloop/model/log_request.pyi
--rw-r--r--   0        0        0    18636 2023-05-17 00:32:28.043092 humanloop-0.4.0/humanloop/model/log_response.py
--rw-r--r--   0        0        0    18636 2023-05-17 00:32:28.043349 humanloop-0.4.0/humanloop/model/log_response.pyi
--rw-r--r--   0        0        0     3205 2023-05-17 00:32:28.043558 humanloop-0.4.0/humanloop/model/logs_log_response.py
--rw-r--r--   0        0        0     3205 2023-05-17 00:32:28.043750 humanloop-0.4.0/humanloop/model/logs_log_response.pyi
--rw-r--r--   0        0        0    16246 2023-05-17 00:32:28.043934 humanloop-0.4.0/humanloop/model/model_config_chat_request.py
--rw-r--r--   0        0        0    16246 2023-05-17 00:32:28.044183 humanloop-0.4.0/humanloop/model/model_config_chat_request.pyi
--rw-r--r--   0        0        0    15386 2023-05-17 00:32:28.044433 humanloop-0.4.0/humanloop/model/model_config_completion_request.py
--rw-r--r--   0        0        0    15386 2023-05-17 00:32:28.044672 humanloop-0.4.0/humanloop/model/model_config_completion_request.pyi
--rw-r--r--   0        0        0     1460 2023-05-17 00:32:28.044880 humanloop-0.4.0/humanloop/model/model_endpoints.py
--rw-r--r--   0        0        0     1305 2023-05-17 00:32:28.045025 humanloop-0.4.0/humanloop/model/model_endpoints.pyi
--rw-r--r--   0        0        0     1695 2023-05-17 00:32:28.045126 humanloop-0.4.0/humanloop/model/model_providers.py
--rw-r--r--   0        0        0     1468 2023-05-17 00:32:28.045270 humanloop-0.4.0/humanloop/model/model_providers.pyi
--rw-r--r--   0        0        0     5144 2023-05-17 00:32:28.045432 humanloop-0.4.0/humanloop/model/paginated_data_log_response.py
--rw-r--r--   0        0        0     5144 2023-05-17 00:32:28.045581 humanloop-0.4.0/humanloop/model/paginated_data_log_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-17 00:32:28.045812 humanloop-0.4.0/humanloop/model/paginated_data_project_response.py
--rw-r--r--   0        0        0     5180 2023-05-17 00:32:28.047730 humanloop-0.4.0/humanloop/model/paginated_data_project_response.pyi
--rw-r--r--   0        0        0     3143 2023-05-17 00:32:28.047957 humanloop-0.4.0/humanloop/model/positive_label.py
--rw-r--r--   0        0        0     3143 2023-05-17 00:32:28.048127 humanloop-0.4.0/humanloop/model/positive_label.pyi
--rw-r--r--   0        0        0    18363 2023-05-17 00:32:28.048349 humanloop-0.4.0/humanloop/model/project_model_config_request.py
--rw-r--r--   0        0        0    18363 2023-05-17 00:32:28.048611 humanloop-0.4.0/humanloop/model/project_model_config_request.pyi
--rw-r--r--   0        0        0    13460 2023-05-17 00:32:28.048843 humanloop-0.4.0/humanloop/model/project_response.py
--rw-r--r--   0        0        0    13460 2023-05-17 00:32:28.049080 humanloop-0.4.0/humanloop/model/project_response.pyi
--rw-r--r--   0        0        0     1471 2023-05-17 00:32:28.049288 humanloop-0.4.0/humanloop/model/project_sort_by.py
--rw-r--r--   0        0        0     1300 2023-05-17 00:32:28.049446 humanloop-0.4.0/humanloop/model/project_sort_by.pyi
--rw-r--r--   0        0        0     3795 2023-05-17 00:32:28.049596 humanloop-0.4.0/humanloop/model/project_user_response.py
--rw-r--r--   0        0        0     3795 2023-05-17 00:32:28.049752 humanloop-0.4.0/humanloop/model/project_user_response.pyi
--rw-r--r--   0        0        0     2004 2023-05-17 00:32:28.049927 humanloop-0.4.0/humanloop/model/projects_get_model_configs_response.py
--rw-r--r--   0        0        0     2004 2023-05-17 00:32:28.050110 humanloop-0.4.0/humanloop/model/projects_get_model_configs_response.pyi
--rw-r--r--   0        0        0     1715 2023-05-17 00:32:28.050393 humanloop-0.4.0/humanloop/model/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1715 2023-05-17 00:32:28.050592 humanloop-0.4.0/humanloop/model/projects_update_feedback_types_request.pyi
--rw-r--r--   0        0        0     4150 2023-05-17 00:32:28.050771 humanloop-0.4.0/humanloop/model/provider_api_keys.py
--rw-r--r--   0        0        0     4150 2023-05-17 00:32:28.050958 humanloop-0.4.0/humanloop/model/provider_api_keys.pyi
--rw-r--r--   0        0        0     3675 2023-05-17 00:32:28.051186 humanloop-0.4.0/humanloop/model/session_app_response.py
--rw-r--r--   0        0        0     3675 2023-05-17 00:32:28.051419 humanloop-0.4.0/humanloop/model/session_app_response.pyi
--rw-r--r--   0        0        0     4394 2023-05-17 00:32:28.051627 humanloop-0.4.0/humanloop/model/session_response.py
--rw-r--r--   0        0        0     4394 2023-05-17 00:32:28.051832 humanloop-0.4.0/humanloop/model/session_response.pyi
--rw-r--r--   0        0        0     1309 2023-05-17 00:32:28.052006 humanloop-0.4.0/humanloop/model/sort_order.py
--rw-r--r--   0        0        0     1192 2023-05-17 00:32:28.052223 humanloop-0.4.0/humanloop/model/sort_order.pyi
--rw-r--r--   0        0        0    17927 2023-05-17 00:32:28.052461 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0    17927 2023-05-17 00:32:28.052719 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi
--rw-r--r--   0        0        0     4889 2023-05-17 00:32:28.052956 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-17 00:32:28.053330 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0    24036 2023-05-17 00:32:28.053691 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0    24036 2023-05-17 00:32:28.054055 humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi
--rw-r--r--   0        0        0    17927 2023-05-17 00:32:28.054474 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py
--rw-r--r--   0        0        0    17927 2023-05-17 00:32:28.054745 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi
--rw-r--r--   0        0        0     4889 2023-05-17 00:32:28.055084 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-17 00:32:28.055329 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0    24036 2023-05-17 00:32:28.055624 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0    24036 2023-05-17 00:32:28.055956 humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi
--rw-r--r--   0        0        0     4232 2023-05-17 00:32:28.056195 humanloop-0.4.0/humanloop/model/tool_result_response.py
--rw-r--r--   0        0        0     4232 2023-05-17 00:32:28.056356 humanloop-0.4.0/humanloop/model/tool_result_response.pyi
--rw-r--r--   0        0        0     7302 2023-05-17 00:32:28.056518 humanloop-0.4.0/humanloop/model/update_experiment_request.py
--rw-r--r--   0        0        0     7302 2023-05-17 00:32:28.056671 humanloop-0.4.0/humanloop/model/update_experiment_request.pyi
--rw-r--r--   0        0        0     5125 2023-05-17 00:32:28.056831 humanloop-0.4.0/humanloop/model/update_project_request.py
--rw-r--r--   0        0        0     5125 2023-05-17 00:32:28.056979 humanloop-0.4.0/humanloop/model/update_project_request.pyi
--rw-r--r--   0        0        0     4118 2023-05-17 00:32:28.057125 humanloop-0.4.0/humanloop/model/usage.py
--rw-r--r--   0        0        0     4118 2023-05-17 00:32:28.057282 humanloop-0.4.0/humanloop/model/usage.pyi
--rw-r--r--   0        0        0     6805 2023-05-17 00:32:28.057429 humanloop-0.4.0/humanloop/model/validation_error.py
--rw-r--r--   0        0        0     6805 2023-05-17 00:32:28.057597 humanloop-0.4.0/humanloop/model/validation_error.pyi
--rw-r--r--   0        0        0     5725 2023-05-17 00:32:28.057772 humanloop-0.4.0/humanloop/models/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-17 00:32:28.057943 humanloop-0.4.0/humanloop/paths/__init__.py
--rw-r--r--   0        0        0      285 2023-05-17 00:32:28.058085 humanloop-0.4.0/humanloop/paths/apps/__init__.py
--rw-r--r--   0        0        0    12735 2023-05-17 00:32:28.058250 humanloop-0.4.0/humanloop/paths/apps/get.py
--rw-r--r--   0        0        0    12592 2023-05-17 00:32:28.058499 humanloop-0.4.0/humanloop/paths/apps/get.pyi
--rw-r--r--   0        0        0      291 2023-05-17 00:32:28.058730 humanloop-0.4.0/humanloop/paths/apps_id/__init__.py
--rw-r--r--   0        0        0    11966 2023-05-17 00:32:28.058935 humanloop-0.4.0/humanloop/paths/apps_id/get.py
--rw-r--r--   0        0        0    11823 2023-05-17 00:32:28.059171 humanloop-0.4.0/humanloop/paths/apps_id/get.pyi
--rw-r--r--   0        0        0      309 2023-05-17 00:32:28.059366 humanloop-0.4.0/humanloop/paths/apps_id_sessions/__init__.py
--rw-r--r--   0        0        0    15570 2023-05-17 00:32:28.059569 humanloop-0.4.0/humanloop/paths/apps_id_sessions/get.py
--rw-r--r--   0        0        0    15427 2023-05-17 00:32:28.059961 humanloop-0.4.0/humanloop/paths/apps_id_sessions/get.pyi
--rw-r--r--   0        0        0      285 2023-05-17 00:32:28.060144 humanloop-0.4.0/humanloop/paths/chat/__init__.py
--rw-r--r--   0        0        0    17428 2023-05-17 00:32:28.060339 humanloop-0.4.0/humanloop/paths/chat/post.py
--rw-r--r--   0        0        0    17285 2023-05-17 00:32:28.060604 humanloop-0.4.0/humanloop/paths/chat/post.pyi
--rw-r--r--   0        0        0      302 2023-05-17 00:32:28.060801 humanloop-0.4.0/humanloop/paths/chat_deployed/__init__.py
--rw-r--r--   0        0        0    16991 2023-05-17 00:32:28.061052 humanloop-0.4.0/humanloop/paths/chat_deployed/post.py
--rw-r--r--   0        0        0    16848 2023-05-17 00:32:28.061378 humanloop-0.4.0/humanloop/paths/chat_deployed/post.pyi
--rw-r--r--   0        0        0      306 2023-05-17 00:32:28.061591 humanloop-0.4.0/humanloop/paths/chat_experiment/__init__.py
--rw-r--r--   0        0        0    17434 2023-05-17 00:32:28.061804 humanloop-0.4.0/humanloop/paths/chat_experiment/post.py
--rw-r--r--   0        0        0    17291 2023-05-17 00:32:28.062097 humanloop-0.4.0/humanloop/paths/chat_experiment/post.pyi
--rw-r--r--   0        0        0      309 2023-05-17 00:32:28.062382 humanloop-0.4.0/humanloop/paths/chat_model_config/__init__.py
--rw-r--r--   0        0        0    17609 2023-05-17 00:32:28.062652 humanloop-0.4.0/humanloop/paths/chat_model_config/post.py
--rw-r--r--   0        0        0    17466 2023-05-17 00:32:28.062920 humanloop-0.4.0/humanloop/paths/chat_model_config/post.pyi
--rw-r--r--   0        0        0      297 2023-05-17 00:32:28.063158 humanloop-0.4.0/humanloop/paths/completion/__init__.py
--rw-r--r--   0        0        0    17744 2023-05-17 00:32:28.063422 humanloop-0.4.0/humanloop/paths/completion/post.py
--rw-r--r--   0        0        0    17601 2023-05-17 00:32:28.063713 humanloop-0.4.0/humanloop/paths/completion/post.pyi
--rw-r--r--   0        0        0      314 2023-05-17 00:32:28.063936 humanloop-0.4.0/humanloop/paths/completion_deployed/__init__.py
--rw-r--r--   0        0        0    17247 2023-05-17 00:32:28.064140 humanloop-0.4.0/humanloop/paths/completion_deployed/post.py
--rw-r--r--   0        0        0    17104 2023-05-17 00:32:28.064362 humanloop-0.4.0/humanloop/paths/completion_deployed/post.pyi
--rw-r--r--   0        0        0      318 2023-05-17 00:32:28.064549 humanloop-0.4.0/humanloop/paths/completion_experiment/__init__.py
--rw-r--r--   0        0        0    17690 2023-05-17 00:32:28.064739 humanloop-0.4.0/humanloop/paths/completion_experiment/post.py
--rw-r--r--   0        0        0    17547 2023-05-17 00:32:28.064957 humanloop-0.4.0/humanloop/paths/completion_experiment/post.pyi
--rw-r--r--   0        0        0      321 2023-05-17 00:32:28.065154 humanloop-0.4.0/humanloop/paths/completion_model_config/__init__.py
--rw-r--r--   0        0        0    17865 2023-05-17 00:32:28.065344 humanloop-0.4.0/humanloop/paths/completion_model_config/post.py
--rw-r--r--   0        0        0    17722 2023-05-17 00:32:28.065566 humanloop-0.4.0/humanloop/paths/completion_model_config/post.pyi
--rw-r--r--   0        0        0      327 2023-05-17 00:32:28.065749 humanloop-0.4.0/humanloop/paths/experiments_experiment_id/__init__.py
--rw-r--r--   0        0        0    11995 2023-05-17 00:32:28.065926 humanloop-0.4.0/humanloop/paths/experiments_experiment_id/delete.py
--rw-r--r--   0        0        0    11852 2023-05-17 00:32:28.066133 humanloop-0.4.0/humanloop/paths/experiments_experiment_id/delete.pyi
--rw-r--r--   0        0        0    17043 2023-05-17 00:32:28.066365 humanloop-0.4.0/humanloop/paths/experiments_experiment_id/patch.py
--rw-r--r--   0        0        0    16900 2023-05-17 00:32:28.066590 humanloop-0.4.0/humanloop/paths/experiments_experiment_id/patch.pyi
--rw-r--r--   0        0        0      352 2023-05-17 00:32:28.066790 humanloop-0.4.0/humanloop/paths/experiments_experiment_id_model_config/__init__.py
--rw-r--r--   0        0        0    12496 2023-05-17 00:32:28.066952 humanloop-0.4.0/humanloop/paths/experiments_experiment_id_model_config/get.py
--rw-r--r--   0        0        0    12353 2023-05-17 00:32:28.067169 humanloop-0.4.0/humanloop/paths/experiments_experiment_id_model_config/get.pyi
--rw-r--r--   0        0        0      293 2023-05-17 00:32:28.067433 humanloop-0.4.0/humanloop/paths/feedback/__init__.py
--rw-r--r--   0        0        0    15089 2023-05-17 00:32:28.067627 humanloop-0.4.0/humanloop/paths/feedback/post.py
--rw-r--r--   0        0        0    14946 2023-05-17 00:32:28.067804 humanloop-0.4.0/humanloop/paths/feedback/post.pyi
--rw-r--r--   0        0        0      285 2023-05-17 00:32:28.068235 humanloop-0.4.0/humanloop/paths/logs/__init__.py
--rw-r--r--   0        0        0    19620 2023-05-17 00:32:28.068454 humanloop-0.4.0/humanloop/paths/logs/post.py
--rw-r--r--   0        0        0    19477 2023-05-17 00:32:28.068697 humanloop-0.4.0/humanloop/paths/logs/post.pyi
--rw-r--r--   0        0        0      302 2023-05-17 00:32:28.068880 humanloop-0.4.0/humanloop/paths/model_configs/__init__.py
--rw-r--r--   0        0        0    20552 2023-05-17 00:32:28.069059 humanloop-0.4.0/humanloop/paths/model_configs/post.py
--rw-r--r--   0        0        0    20409 2023-05-17 00:32:28.069292 humanloop-0.4.0/humanloop/paths/model_configs/post.pyi
--rw-r--r--   0        0        0      308 2023-05-17 00:32:28.069526 humanloop-0.4.0/humanloop/paths/model_configs_id/__init__.py
--rw-r--r--   0        0        0    12309 2023-05-17 00:32:28.069758 humanloop-0.4.0/humanloop/paths/model_configs_id/get.py
--rw-r--r--   0        0        0    12166 2023-05-17 00:32:28.069972 humanloop-0.4.0/humanloop/paths/model_configs_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-17 00:32:28.070180 humanloop-0.4.0/humanloop/paths/projects/__init__.py
--rw-r--r--   0        0        0    20518 2023-05-17 00:32:28.070425 humanloop-0.4.0/humanloop/paths/projects/get.py
--rw-r--r--   0        0        0    20375 2023-05-17 00:32:28.070721 humanloop-0.4.0/humanloop/paths/projects/get.pyi
--rw-r--r--   0        0        0    13007 2023-05-17 00:32:28.070949 humanloop-0.4.0/humanloop/paths/projects/post.py
--rw-r--r--   0        0        0    12864 2023-05-17 00:32:28.071168 humanloop-0.4.0/humanloop/paths/projects/post.pyi
--rw-r--r--   0        0        0      299 2023-05-17 00:32:28.071370 humanloop-0.4.0/humanloop/paths/projects_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-17 00:32:28.071518 humanloop-0.4.0/humanloop/paths/projects_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-17 00:32:28.071743 humanloop-0.4.0/humanloop/paths/projects_id/get.pyi
--rw-r--r--   0        0        0    16162 2023-05-17 00:32:28.072005 humanloop-0.4.0/humanloop/paths/projects_id/patch.py
--rw-r--r--   0        0        0    16019 2023-05-17 00:32:28.072388 humanloop-0.4.0/humanloop/paths/projects_id/patch.pyi
--rw-r--r--   0        0        0      334 2023-05-17 00:32:28.072880 humanloop-0.4.0/humanloop/paths/projects_id_active_experiment/__init__.py
--rw-r--r--   0        0        0    12306 2023-05-17 00:32:28.073084 humanloop-0.4.0/humanloop/paths/projects_id_active_experiment/delete.py
--rw-r--r--   0        0        0    12163 2023-05-17 00:32:28.073334 humanloop-0.4.0/humanloop/paths/projects_id_active_experiment/delete.pyi
--rw-r--r--   0        0        0      337 2023-05-17 00:32:28.073569 humanloop-0.4.0/humanloop/paths/projects_id_active_model_config/__init__.py
--rw-r--r--   0        0        0    12337 2023-05-17 00:32:28.073841 humanloop-0.4.0/humanloop/paths/projects_id_active_model_config/delete.py
--rw-r--r--   0        0        0    12194 2023-05-17 00:32:28.074432 humanloop-0.4.0/humanloop/paths/projects_id_active_model_config/delete.pyi
--rw-r--r--   0        0        0      313 2023-05-17 00:32:28.074644 humanloop-0.4.0/humanloop/paths/projects_id_export/__init__.py
--rw-r--r--   0        0        0    15728 2023-05-17 00:32:28.074826 humanloop-0.4.0/humanloop/paths/projects_id_export/post.py
--rw-r--r--   0        0        0    15585 2023-05-17 00:32:28.075070 humanloop-0.4.0/humanloop/paths/projects_id_export/post.pyi
--rw-r--r--   0        0        0      328 2023-05-17 00:32:28.075399 humanloop-0.4.0/humanloop/paths/projects_id_feedback_types/__init__.py
--rw-r--r--   0        0        0    14809 2023-05-17 00:32:28.075504 humanloop-0.4.0/humanloop/paths/projects_id_feedback_types/patch.py
--rw-r--r--   0        0        0    14666 2023-05-17 00:32:28.075891 humanloop-0.4.0/humanloop/paths/projects_id_feedback_types/patch.pyi
--rw-r--r--   0        0        0      324 2023-05-17 00:32:28.076160 humanloop-0.4.0/humanloop/paths/projects_id_model_config/__init__.py
--rw-r--r--   0        0        0    12229 2023-05-17 00:32:28.076355 humanloop-0.4.0/humanloop/paths/projects_id_model_config/get.py
--rw-r--r--   0        0        0    12086 2023-05-17 00:32:28.076532 humanloop-0.4.0/humanloop/paths/projects_id_model_config/get.pyi
--rw-r--r--   0        0        0      326 2023-05-17 00:32:28.076658 humanloop-0.4.0/humanloop/paths/projects_id_model_configs/__init__.py
--rw-r--r--   0        0        0    12319 2023-05-17 00:32:28.076765 humanloop-0.4.0/humanloop/paths/projects_id_model_configs/get.py
--rw-r--r--   0        0        0    12176 2023-05-17 00:32:28.076916 humanloop-0.4.0/humanloop/paths/projects_id_model_configs/get.pyi
--rw-r--r--   0        0        0      339 2023-05-17 00:32:28.077039 humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/__init__.py
--rw-r--r--   0        0        0    12256 2023-05-17 00:32:28.077164 humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/get.py
--rw-r--r--   0        0        0    12113 2023-05-17 00:32:28.077299 humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/get.pyi
--rw-r--r--   0        0        0    16346 2023-05-17 00:32:28.077429 humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/post.py
--rw-r--r--   0        0        0    16203 2023-05-17 00:32:28.077576 humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/post.pyi
--rw-r--r--   0        0        0      293 2023-05-17 00:32:28.077729 humanloop-0.4.0/humanloop/paths/sessions/__init__.py
--rw-r--r--   0        0        0    12149 2023-05-17 00:32:28.077880 humanloop-0.4.0/humanloop/paths/sessions/post.py
--rw-r--r--   0        0        0    12006 2023-05-17 00:32:28.078187 humanloop-0.4.0/humanloop/paths/sessions/post.pyi
--rw-r--r--   0        0        0      299 2023-05-17 00:32:28.078396 humanloop-0.4.0/humanloop/paths/sessions_id/__init__.py
--rw-r--r--   0        0        0    11974 2023-05-17 00:32:28.078537 humanloop-0.4.0/humanloop/paths/sessions_id/get.py
--rw-r--r--   0        0        0    11831 2023-05-17 00:32:28.078720 humanloop-0.4.0/humanloop/paths/sessions_id/get.pyi
--rw-r--r--   0        0        0      313 2023-05-17 00:32:28.078926 humanloop-0.4.0/humanloop/paths/sessions_id_events/__init__.py
--rw-r--r--   0        0        0    12085 2023-05-17 00:32:28.079090 humanloop-0.4.0/humanloop/paths/sessions_id_events/get.py
--rw-r--r--   0        0        0    11942 2023-05-17 00:32:28.079295 humanloop-0.4.0/humanloop/paths/sessions_id_events/get.pyi
--rw-r--r--   0        0        0     1011 2023-05-17 00:32:28.079439 humanloop-0.4.0/humanloop/request_after_hook.py
--rw-r--r--   0        0        0     1012 2023-05-17 00:32:28.079570 humanloop-0.4.0/humanloop/request_before_hook.py
--rw-r--r--   0        0        0    11329 2023-05-17 00:32:28.079726 humanloop-0.4.0/humanloop/rest.py
--rw-r--r--   0        0        0    95913 2023-05-17 00:32:28.080022 humanloop-0.4.0/humanloop/schemas.py
--rw-r--r--   0        0        0        0 2023-05-17 00:32:28.080179 humanloop-0.4.0/humanloop/type/__init__.py
--rw-r--r--   0        0        0     1489 2023-05-17 00:32:28.080289 humanloop-0.4.0/humanloop/type/base_metric_response.py
--rw-r--r--   0        0        0     1137 2023-05-17 00:32:28.080400 humanloop-0.4.0/humanloop/type/categorical_feedback_label.py
--rw-r--r--   0        0        0     2272 2023-05-17 00:32:28.080505 humanloop-0.4.0/humanloop/type/chat_data_response.py
--rw-r--r--   0        0        0     2085 2023-05-17 00:32:28.080606 humanloop-0.4.0/humanloop/type/chat_deployed_request.py
--rw-r--r--   0        0        0     2337 2023-05-17 00:32:28.080705 humanloop-0.4.0/humanloop/type/chat_experiment_request.py
--rw-r--r--   0        0        0      980 2023-05-17 00:32:28.080802 humanloop-0.4.0/humanloop/type/chat_message.py
--rw-r--r--   0        0        0     2208 2023-05-17 00:32:28.080894 humanloop-0.4.0/humanloop/type/chat_model_config_request.py
--rw-r--r--   0        0        0     2212 2023-05-17 00:32:28.080983 humanloop-0.4.0/humanloop/type/chat_request.py
--rw-r--r--   0        0        0     1899 2023-05-17 00:32:28.081070 humanloop-0.4.0/humanloop/type/chat_response.py
--rw-r--r--   0        0        0      711 2023-05-17 00:32:28.081171 humanloop-0.4.0/humanloop/type/chat_role.py
--rw-r--r--   0        0        0     2205 2023-05-17 00:32:28.081269 humanloop-0.4.0/humanloop/type/completion_deployed_request.py
--rw-r--r--   0        0        0     2460 2023-05-17 00:32:28.081373 humanloop-0.4.0/humanloop/type/completion_experiment_request.py
--rw-r--r--   0        0        0     2328 2023-05-17 00:32:28.081471 humanloop-0.4.0/humanloop/type/completion_model_config_request.py
--rw-r--r--   0        0        0     2336 2023-05-17 00:32:28.081568 humanloop-0.4.0/humanloop/type/completion_request.py
--rw-r--r--   0        0        0     1957 2023-05-17 00:32:28.081668 humanloop-0.4.0/humanloop/type/completion_response.py
--rw-r--r--   0        0        0     1468 2023-05-17 00:32:28.081771 humanloop-0.4.0/humanloop/type/create_experiment_request.py
--rw-r--r--   0        0        0     1085 2023-05-17 00:32:28.081869 humanloop-0.4.0/humanloop/type/create_log_response.py
--rw-r--r--   0        0        0     1142 2023-05-17 00:32:28.081963 humanloop-0.4.0/humanloop/type/create_project_request.py
--rw-r--r--   0        0        0     1000 2023-05-17 00:32:28.082078 humanloop-0.4.0/humanloop/type/create_session_request.py
--rw-r--r--   0        0        0     2091 2023-05-17 00:32:28.082207 humanloop-0.4.0/humanloop/type/data_response.py
--rw-r--r--   0        0        0     1954 2023-05-17 00:32:28.082324 humanloop-0.4.0/humanloop/type/experiment_model_config_response.py
--rw-r--r--   0        0        0     1909 2023-05-17 00:32:28.082437 humanloop-0.4.0/humanloop/type/experiment_response.py
--rw-r--r--   0        0        0      718 2023-05-17 00:32:28.082568 humanloop-0.4.0/humanloop/type/experiment_status.py
--rw-r--r--   0        0        0      785 2023-05-17 00:32:28.082703 humanloop-0.4.0/humanloop/type/experiments_list_response.py
--rw-r--r--   0        0        0     1510 2023-05-17 00:32:28.082834 humanloop-0.4.0/humanloop/type/feedback.py
--rw-r--r--   0        0        0      719 2023-05-17 00:32:28.082970 humanloop-0.4.0/humanloop/type/feedback_class.py
--rw-r--r--   0        0        0     1046 2023-05-17 00:32:28.083117 humanloop-0.4.0/humanloop/type/feedback_label_request.py
--rw-r--r--   0        0        0     1624 2023-05-17 00:32:28.083264 humanloop-0.4.0/humanloop/type/feedback_request.py
--rw-r--r--   0        0        0     1658 2023-05-17 00:32:28.083390 humanloop-0.4.0/humanloop/type/feedback_response.py
--rw-r--r--   0        0        0      804 2023-05-17 00:32:28.083515 humanloop-0.4.0/humanloop/type/feedback_submit_request.py
--rw-r--r--   0        0        0      809 2023-05-17 00:32:28.083627 humanloop-0.4.0/humanloop/type/feedback_submit_response.py
--rw-r--r--   0        0        0      738 2023-05-17 00:32:28.083739 humanloop-0.4.0/humanloop/type/feedback_type.py
--rw-r--r--   0        0        0     1377 2023-05-17 00:32:28.083843 humanloop-0.4.0/humanloop/type/feedback_type_model.py
--rw-r--r--   0        0        0     1541 2023-05-17 00:32:28.083942 humanloop-0.4.0/humanloop/type/feedback_type_request.py
--rw-r--r--   0        0        0      773 2023-05-17 00:32:28.084029 humanloop-0.4.0/humanloop/type/feedback_types.py
--rw-r--r--   0        0        0     4271 2023-05-17 00:32:28.084150 humanloop-0.4.0/humanloop/type/get_model_config_response.py
--rw-r--r--   0        0        0     1034 2023-05-17 00:32:28.084296 humanloop-0.4.0/humanloop/type/http_validation_error.py
--rw-r--r--   0        0        0      730 2023-05-17 00:32:28.084409 humanloop-0.4.0/humanloop/type/label_sentiment.py
--rw-r--r--   0        0        0      782 2023-05-17 00:32:28.084519 humanloop-0.4.0/humanloop/type/log_datapoint_request.py
--rw-r--r--   0        0        0     2430 2023-05-17 00:32:28.084641 humanloop-0.4.0/humanloop/type/log_request.py
--rw-r--r--   0        0        0     2968 2023-05-17 00:32:28.084763 humanloop-0.4.0/humanloop/type/log_response.py
--rw-r--r--   0        0        0      807 2023-05-17 00:32:28.084884 humanloop-0.4.0/humanloop/type/logs_log_response.py
--rw-r--r--   0        0        0     2927 2023-05-17 00:32:28.085008 humanloop-0.4.0/humanloop/type/model_config_chat_request.py
--rw-r--r--   0        0        0     2832 2023-05-17 00:32:28.085123 humanloop-0.4.0/humanloop/type/model_config_completion_request.py
--rw-r--r--   0        0        0      714 2023-05-17 00:32:28.085249 humanloop-0.4.0/humanloop/type/model_endpoints.py
--rw-r--r--   0        0        0      738 2023-05-17 00:32:28.085380 humanloop-0.4.0/humanloop/type/model_providers.py
--rw-r--r--   0        0        0     1113 2023-05-17 00:32:28.085504 humanloop-0.4.0/humanloop/type/paginated_data_log_response.py
--rw-r--r--   0        0        0     1153 2023-05-17 00:32:28.085634 humanloop-0.4.0/humanloop/type/paginated_data_project_response.py
--rw-r--r--   0        0        0      924 2023-05-17 00:32:28.085752 humanloop-0.4.0/humanloop/type/positive_label.py
--rw-r--r--   0        0        0     3535 2023-05-17 00:32:28.085859 humanloop-0.4.0/humanloop/type/project_model_config_request.py
--rw-r--r--   0        0        0     2190 2023-05-17 00:32:28.085960 humanloop-0.4.0/humanloop/type/project_response.py
--rw-r--r--   0        0        0      721 2023-05-17 00:32:28.086073 humanloop-0.4.0/humanloop/type/project_sort_by.py
--rw-r--r--   0        0        0     1099 2023-05-17 00:32:28.086185 humanloop-0.4.0/humanloop/type/project_user_response.py
--rw-r--r--   0        0        0      928 2023-05-17 00:32:28.086308 humanloop-0.4.0/humanloop/type/projects_get_model_configs_response.py
--rw-r--r--   0        0        0      800 2023-05-17 00:32:28.086422 humanloop-0.4.0/humanloop/type/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0      980 2023-05-17 00:32:28.086530 humanloop-0.4.0/humanloop/type/provider_api_keys.py
--rw-r--r--   0        0        0     1024 2023-05-17 00:32:28.086636 humanloop-0.4.0/humanloop/type/session_app_response.py
--rw-r--r--   0        0        0     1074 2023-05-17 00:32:28.086743 humanloop-0.4.0/humanloop/type/session_response.py
--rw-r--r--   0        0        0      696 2023-05-17 00:32:28.086855 humanloop-0.4.0/humanloop/type/sort_order.py
--rw-r--r--   0        0        0     3508 2023-05-17 00:32:28.086984 humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0     1420 2023-05-17 00:32:28.087112 humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4439 2023-05-17 00:32:28.087223 humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0     3528 2023-05-17 00:32:28.087350 humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_model_config_response.py
--rw-r--r--   0        0        0     1420 2023-05-17 00:32:28.087480 humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4459 2023-05-17 00:32:28.087601 humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0      999 2023-05-17 00:32:28.087713 humanloop-0.4.0/humanloop/type/tool_result_response.py
--rw-r--r--   0        0        0     1440 2023-05-17 00:32:28.087821 humanloop-0.4.0/humanloop/type/update_experiment_request.py
--rw-r--r--   0        0        0     1529 2023-05-17 00:32:28.087945 humanloop-0.4.0/humanloop/type/update_project_request.py
--rw-r--r--   0        0        0     1082 2023-05-17 00:32:28.088045 humanloop-0.4.0/humanloop/type/usage.py
--rw-r--r--   0        0        0     1011 2023-05-17 00:32:28.088140 humanloop-0.4.0/humanloop/type/validation_error.py
--rw-r--r--   0        0        0      868 2023-05-17 00:32:28.088237 humanloop-0.4.0/humanloop/type_util.py
--rw-r--r--   0        0        0     3165 2023-05-17 00:32:28.088385 humanloop-0.4.0/humanloop/validation_metadata.py
--rw-r--r--   0        0        0      714 2023-05-17 00:32:28.088820 humanloop-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9071 1970-01-01 00:00:00.000000 humanloop-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-16 00:03:04.788320 humanloop-0.4.0a4/LICENSE
+-rw-r--r--   0        0        0     7529 2023-05-16 00:03:04.832925 humanloop-0.4.0a4/README.md
+-rw-r--r--   0        0        0     1061 2023-05-16 00:03:04.713744 humanloop-0.4.0a4/humanloop/__init__.py
+-rw-r--r--   0        0        0    73011 2023-05-16 00:03:04.713958 humanloop-0.4.0a4/humanloop/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-16 00:03:04.714240 humanloop-0.4.0a4/humanloop/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-16 00:03:04.714367 humanloop-0.4.0a4/humanloop/apis/__init__.py
+-rw-r--r--   0        0        0     5316 2023-05-16 00:03:04.714479 humanloop-0.4.0a4/humanloop/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-05-16 00:03:04.714606 humanloop-0.4.0a4/humanloop/apis/paths/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-16 00:03:04.714740 humanloop-0.4.0a4/humanloop/apis/paths/apps.py
+-rw-r--r--   0        0        0       93 2023-05-16 00:03:04.714876 humanloop-0.4.0a4/humanloop/apis/paths/apps_id.py
+-rw-r--r--   0        0        0      110 2023-05-16 00:03:04.714994 humanloop-0.4.0a4/humanloop/apis/paths/apps_id_sessions.py
+-rw-r--r--   0        0        0       91 2023-05-16 00:03:04.715096 humanloop-0.4.0a4/humanloop/apis/paths/chat.py
+-rw-r--r--   0        0        0      108 2023-05-16 00:03:04.715202 humanloop-0.4.0a4/humanloop/apis/paths/chat_deployed.py
+-rw-r--r--   0        0        0      112 2023-05-16 00:03:04.715300 humanloop-0.4.0a4/humanloop/apis/paths/chat_experiment.py
+-rw-r--r--   0        0        0      115 2023-05-16 00:03:04.715416 humanloop-0.4.0a4/humanloop/apis/paths/chat_model_config.py
+-rw-r--r--   0        0        0      103 2023-05-16 00:03:04.715534 humanloop-0.4.0a4/humanloop/apis/paths/completion.py
+-rw-r--r--   0        0        0      120 2023-05-16 00:03:04.715656 humanloop-0.4.0a4/humanloop/apis/paths/completion_deployed.py
+-rw-r--r--   0        0        0      124 2023-05-16 00:03:04.715801 humanloop-0.4.0a4/humanloop/apis/paths/completion_experiment.py
+-rw-r--r--   0        0        0      127 2023-05-16 00:03:04.715947 humanloop-0.4.0a4/humanloop/apis/paths/completion_model_config.py
+-rw-r--r--   0        0        0      226 2023-05-16 00:03:04.716070 humanloop-0.4.0a4/humanloop/apis/paths/experiments_experiment_id.py
+-rw-r--r--   0        0        0      152 2023-05-16 00:03:04.716182 humanloop-0.4.0a4/humanloop/apis/paths/experiments_experiment_id_model_config.py
+-rw-r--r--   0        0        0       99 2023-05-16 00:03:04.716308 humanloop-0.4.0a4/humanloop/apis/paths/feedback.py
+-rw-r--r--   0        0        0       91 2023-05-16 00:03:04.716431 humanloop-0.4.0a4/humanloop/apis/paths/logs.py
+-rw-r--r--   0        0        0      108 2023-05-16 00:03:04.716556 humanloop-0.4.0a4/humanloop/apis/paths/model_configs.py
+-rw-r--r--   0        0        0      110 2023-05-16 00:03:04.716685 humanloop-0.4.0a4/humanloop/apis/paths/model_configs_id.py
+-rw-r--r--   0        0        0      165 2023-05-16 00:03:04.716812 humanloop-0.4.0a4/humanloop/apis/paths/projects.py
+-rw-r--r--   0        0        0      176 2023-05-16 00:03:04.716936 humanloop-0.4.0a4/humanloop/apis/paths/projects_id.py
+-rw-r--r--   0        0        0      144 2023-05-16 00:03:04.717064 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_active_experiment.py
+-rw-r--r--   0        0        0      147 2023-05-16 00:03:04.717178 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_active_model_config.py
+-rw-r--r--   0        0        0      117 2023-05-16 00:03:04.717308 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_export.py
+-rw-r--r--   0        0        0      135 2023-05-16 00:03:04.717406 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_feedback_types.py
+-rw-r--r--   0        0        0      125 2023-05-16 00:03:04.717500 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_model_config.py
+-rw-r--r--   0        0        0      127 2023-05-16 00:03:04.717601 humanloop-0.4.0a4/humanloop/apis/paths/projects_id_model_configs.py
+-rw-r--r--   0        0        0      231 2023-05-16 00:03:04.717701 humanloop-0.4.0a4/humanloop/apis/paths/projects_project_id_experiments.py
+-rw-r--r--   0        0        0       99 2023-05-16 00:03:04.717802 humanloop-0.4.0a4/humanloop/apis/paths/sessions.py
+-rw-r--r--   0        0        0      101 2023-05-16 00:03:04.717895 humanloop-0.4.0a4/humanloop/apis/paths/sessions_id.py
+-rw-r--r--   0        0        0      114 2023-05-16 00:03:04.718000 humanloop-0.4.0a4/humanloop/apis/paths/sessions_id_events.py
+-rw-r--r--   0        0        0     1642 2023-05-16 00:03:04.718091 humanloop-0.4.0a4/humanloop/apis/tag_to_api.py
+-rw-r--r--   0        0        0      568 2023-05-16 00:03:04.718179 humanloop-0.4.0a4/humanloop/apis/tags/__init__.py
+-rw-r--r--   0        0        0      839 2023-05-16 00:03:04.718256 humanloop-0.4.0a4/humanloop/apis/tags/apps_api.py
+-rw-r--r--   0        0        0     1006 2023-05-16 00:03:04.718359 humanloop-0.4.0a4/humanloop/apis/tags/chats_api.py
+-rw-r--r--   0        0        0     1020 2023-05-16 00:03:04.718452 humanloop-0.4.0a4/humanloop/apis/tags/completions_api.py
+-rw-r--r--   0        0        0     1091 2023-05-16 00:03:04.718538 humanloop-0.4.0a4/humanloop/apis/tags/experiments_api.py
+-rw-r--r--   0        0        0      721 2023-05-16 00:03:04.718641 humanloop-0.4.0a4/humanloop/apis/tags/feedback_api.py
+-rw-r--r--   0        0        0      707 2023-05-16 00:03:04.718741 humanloop-0.4.0a4/humanloop/apis/tags/logs_api.py
+-rw-r--r--   0        0        0      803 2023-05-16 00:03:04.718832 humanloop-0.4.0a4/humanloop/apis/tags/model_configurations_api.py
+-rw-r--r--   0        0        0     1519 2023-05-16 00:03:04.718916 humanloop-0.4.0a4/humanloop/apis/tags/projects_api.py
+-rw-r--r--   0        0        0      854 2023-05-16 00:03:04.719001 humanloop-0.4.0a4/humanloop/apis/tags/sessions_api.py
+-rw-r--r--   0        0        0    27541 2023-05-16 00:03:04.719140 humanloop-0.4.0a4/humanloop/client.py
+-rw-r--r--   0        0        0    27541 2023-05-16 00:03:04.719275 humanloop-0.4.0a4/humanloop/client.pyi
+-rw-r--r--   0        0        0     6819 2023-05-11 17:36:33.683951 humanloop-0.4.0a4/humanloop/client_custom.py
+-rw-r--r--   0        0        0    18311 2023-05-16 00:03:04.719398 humanloop-0.4.0a4/humanloop/configuration.py
+-rw-r--r--   0        0        0     7678 2023-05-16 00:03:04.719531 humanloop-0.4.0a4/humanloop/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-16 00:03:04.719627 humanloop-0.4.0a4/humanloop/exceptions_base.py
+-rw-r--r--   0        0        0      343 2023-05-16 00:03:04.719792 humanloop-0.4.0a4/humanloop/model/__init__.py
+-rw-r--r--   0        0        0     6379 2023-05-16 00:03:04.719904 humanloop-0.4.0a4/humanloop/model/base_metric_response.py
+-rw-r--r--   0        0        0     6379 2023-05-16 00:03:04.720008 humanloop-0.4.0a4/humanloop/model/base_metric_response.pyi
+-rw-r--r--   0        0        0     5150 2023-05-16 00:03:04.720103 humanloop-0.4.0a4/humanloop/model/categorical_feedback_label.py
+-rw-r--r--   0        0        0     5150 2023-05-16 00:03:04.720197 humanloop-0.4.0a4/humanloop/model/categorical_feedback_label.pyi
+-rw-r--r--   0        0        0     8957 2023-05-16 00:03:04.720308 humanloop-0.4.0a4/humanloop/model/chat_data_response.py
+-rw-r--r--   0        0        0     8957 2023-05-16 00:03:04.720441 humanloop-0.4.0a4/humanloop/model/chat_data_response.pyi
+-rw-r--r--   0        0        0     9998 2023-05-16 00:03:04.720591 humanloop-0.4.0a4/humanloop/model/chat_deployed_request.py
+-rw-r--r--   0        0        0     9998 2023-05-16 00:03:04.720727 humanloop-0.4.0a4/humanloop/model/chat_deployed_request.pyi
+-rw-r--r--   0        0        0    10659 2023-05-16 00:03:04.720851 humanloop-0.4.0a4/humanloop/model/chat_experiment_request.py
+-rw-r--r--   0        0        0    10659 2023-05-16 00:03:04.720978 humanloop-0.4.0a4/humanloop/model/chat_experiment_request.pyi
+-rw-r--r--   0        0        0     3702 2023-05-16 00:03:04.721087 humanloop-0.4.0a4/humanloop/model/chat_message.py
+-rw-r--r--   0        0        0     3702 2023-05-16 00:03:04.721186 humanloop-0.4.0a4/humanloop/model/chat_message.pyi
+-rw-r--r--   0        0        0    10693 2023-05-16 00:03:04.721296 humanloop-0.4.0a4/humanloop/model/chat_model_config_request.py
+-rw-r--r--   0        0        0    10693 2023-05-16 00:03:04.721409 humanloop-0.4.0a4/humanloop/model/chat_model_config_request.pyi
+-rw-r--r--   0        0        0    12556 2023-05-16 00:03:04.721535 humanloop-0.4.0a4/humanloop/model/chat_request.py
+-rw-r--r--   0        0        0    12556 2023-05-16 00:03:04.721672 humanloop-0.4.0a4/humanloop/model/chat_request.pyi
+-rw-r--r--   0        0        0    11076 2023-05-16 00:03:04.721789 humanloop-0.4.0a4/humanloop/model/chat_response.py
+-rw-r--r--   0        0        0    11076 2023-05-16 00:03:04.721911 humanloop-0.4.0a4/humanloop/model/chat_response.pyi
+-rw-r--r--   0        0        0     1446 2023-05-16 00:03:04.722025 humanloop-0.4.0a4/humanloop/model/chat_role.py
+-rw-r--r--   0        0        0     1285 2023-05-16 00:03:04.722124 humanloop-0.4.0a4/humanloop/model/chat_role.pyi
+-rw-r--r--   0        0        0     9674 2023-05-16 00:03:04.722221 humanloop-0.4.0a4/humanloop/model/completion_deployed_request.py
+-rw-r--r--   0        0        0     9674 2023-05-16 00:03:04.722341 humanloop-0.4.0a4/humanloop/model/completion_deployed_request.pyi
+-rw-r--r--   0        0        0    10340 2023-05-16 00:03:04.722453 humanloop-0.4.0a4/humanloop/model/completion_experiment_request.py
+-rw-r--r--   0        0        0    10340 2023-05-16 00:03:04.722601 humanloop-0.4.0a4/humanloop/model/completion_experiment_request.pyi
+-rw-r--r--   0        0        0    10376 2023-05-16 00:03:04.722777 humanloop-0.4.0a4/humanloop/model/completion_model_config_request.py
+-rw-r--r--   0        0        0    10376 2023-05-16 00:03:04.722950 humanloop-0.4.0a4/humanloop/model/completion_model_config_request.pyi
+-rw-r--r--   0        0        0    12258 2023-05-16 00:03:04.723114 humanloop-0.4.0a4/humanloop/model/completion_request.py
+-rw-r--r--   0        0        0    12258 2023-05-16 00:03:04.723324 humanloop-0.4.0a4/humanloop/model/completion_request.pyi
+-rw-r--r--   0        0        0    11017 2023-05-16 00:03:04.723480 humanloop-0.4.0a4/humanloop/model/completion_response.py
+-rw-r--r--   0        0        0    11017 2023-05-16 00:03:04.723648 humanloop-0.4.0a4/humanloop/model/completion_response.pyi
+-rw-r--r--   0        0        0     6280 2023-05-16 00:03:04.723802 humanloop-0.4.0a4/humanloop/model/create_experiment_request.py
+-rw-r--r--   0        0        0     6280 2023-05-16 00:03:04.723940 humanloop-0.4.0a4/humanloop/model/create_experiment_request.pyi
+-rw-r--r--   0        0        0     3199 2023-05-16 00:03:04.724074 humanloop-0.4.0a4/humanloop/model/create_log_response.py
+-rw-r--r--   0        0        0     3199 2023-05-16 00:03:04.724198 humanloop-0.4.0a4/humanloop/model/create_log_response.pyi
+-rw-r--r--   0        0        0     4266 2023-05-16 00:03:04.724328 humanloop-0.4.0a4/humanloop/model/create_project_request.py
+-rw-r--r--   0        0        0     4266 2023-05-16 00:03:04.724467 humanloop-0.4.0a4/humanloop/model/create_project_request.pyi
+-rw-r--r--   0        0        0     2649 2023-05-16 00:03:04.724583 humanloop-0.4.0a4/humanloop/model/create_session_request.py
+-rw-r--r--   0        0        0     2649 2023-05-16 00:03:04.724700 humanloop-0.4.0a4/humanloop/model/create_session_request.pyi
+-rw-r--r--   0        0        0     7455 2023-05-16 00:03:04.724817 humanloop-0.4.0a4/humanloop/model/data_response.py
+-rw-r--r--   0        0        0     7455 2023-05-16 00:03:04.724951 humanloop-0.4.0a4/humanloop/model/data_response.pyi
+-rw-r--r--   0        0        0     9235 2023-05-16 00:03:04.725084 humanloop-0.4.0a4/humanloop/model/experiment_model_config_response.py
+-rw-r--r--   0        0        0     9235 2023-05-16 00:03:04.725243 humanloop-0.4.0a4/humanloop/model/experiment_model_config_response.pyi
+-rw-r--r--   0        0        0    12947 2023-05-16 00:03:04.725405 humanloop-0.4.0a4/humanloop/model/experiment_response.py
+-rw-r--r--   0        0        0    12947 2023-05-16 00:03:04.725576 humanloop-0.4.0a4/humanloop/model/experiment_response.pyi
+-rw-r--r--   0        0        0     1376 2023-05-16 00:03:04.725732 humanloop-0.4.0a4/humanloop/model/experiment_status.py
+-rw-r--r--   0        0        0     1229 2023-05-16 00:03:04.725857 humanloop-0.4.0a4/humanloop/model/experiment_status.pyi
+-rw-r--r--   0        0        0     1685 2023-05-16 00:03:04.725997 humanloop-0.4.0a4/humanloop/model/experiments_list_response.py
+-rw-r--r--   0        0        0     1685 2023-05-16 00:03:04.726151 humanloop-0.4.0a4/humanloop/model/experiments_list_response.pyi
+-rw-r--r--   0        0        0     6681 2023-05-16 00:03:04.726299 humanloop-0.4.0a4/humanloop/model/feedback.py
+-rw-r--r--   0        0        0     6681 2023-05-16 00:03:04.726436 humanloop-0.4.0a4/humanloop/model/feedback.pyi
+-rw-r--r--   0        0        0     1463 2023-05-16 00:03:04.726559 humanloop-0.4.0a4/humanloop/model/feedback_class.py
+-rw-r--r--   0        0        0     1296 2023-05-16 00:03:04.726681 humanloop-0.4.0a4/humanloop/model/feedback_class.pyi
+-rw-r--r--   0        0        0     3334 2023-05-16 00:03:04.726815 humanloop-0.4.0a4/humanloop/model/feedback_label_request.py
+-rw-r--r--   0        0        0     3334 2023-05-16 00:03:04.726940 humanloop-0.4.0a4/humanloop/model/feedback_label_request.pyi
+-rw-r--r--   0        0        0     7189 2023-05-16 00:03:04.727085 humanloop-0.4.0a4/humanloop/model/feedback_request.py
+-rw-r--r--   0        0        0     7189 2023-05-16 00:03:04.727230 humanloop-0.4.0a4/humanloop/model/feedback_request.pyi
+-rw-r--r--   0        0        0     7141 2023-05-16 00:03:04.727346 humanloop-0.4.0a4/humanloop/model/feedback_response.py
+-rw-r--r--   0        0        0     7141 2023-05-16 00:03:04.727476 humanloop-0.4.0a4/humanloop/model/feedback_response.pyi
+-rw-r--r--   0        0        0     3200 2023-05-16 00:03:04.727601 humanloop-0.4.0a4/humanloop/model/feedback_submit_request.py
+-rw-r--r--   0        0        0     3200 2023-05-16 00:03:04.727718 humanloop-0.4.0a4/humanloop/model/feedback_submit_request.pyi
+-rw-r--r--   0        0        0     3210 2023-05-16 00:03:04.727830 humanloop-0.4.0a4/humanloop/model/feedback_submit_response.py
+-rw-r--r--   0        0        0     3210 2023-05-16 00:03:04.727941 humanloop-0.4.0a4/humanloop/model/feedback_submit_response.pyi
+-rw-r--r--   0        0        0     1690 2023-05-16 00:03:04.728045 humanloop-0.4.0a4/humanloop/model/feedback_type.py
+-rw-r--r--   0        0        0     1459 2023-05-16 00:03:04.728196 humanloop-0.4.0a4/humanloop/model/feedback_type.pyi
+-rw-r--r--   0        0        0     6161 2023-05-16 00:03:04.728383 humanloop-0.4.0a4/humanloop/model/feedback_type_model.py
+-rw-r--r--   0        0        0     6161 2023-05-16 00:03:04.728532 humanloop-0.4.0a4/humanloop/model/feedback_type_model.pyi
+-rw-r--r--   0        0        0     6289 2023-05-16 00:03:04.728654 humanloop-0.4.0a4/humanloop/model/feedback_type_request.py
+-rw-r--r--   0        0        0     6289 2023-05-16 00:03:04.728756 humanloop-0.4.0a4/humanloop/model/feedback_type_request.pyi
+-rw-r--r--   0        0        0     1659 2023-05-16 00:03:04.728861 humanloop-0.4.0a4/humanloop/model/feedback_types.py
+-rw-r--r--   0        0        0     1659 2023-05-16 00:03:04.728963 humanloop-0.4.0a4/humanloop/model/feedback_types.pyi
+-rw-r--r--   0        0        0    24518 2023-05-16 00:03:04.729106 humanloop-0.4.0a4/humanloop/model/get_model_config_response.py
+-rw-r--r--   0        0        0    24518 2023-05-16 00:03:04.729297 humanloop-0.4.0a4/humanloop/model/get_model_config_response.pyi
+-rw-r--r--   0        0        0     3611 2023-05-16 00:03:04.729434 humanloop-0.4.0a4/humanloop/model/http_validation_error.py
+-rw-r--r--   0        0        0     3611 2023-05-16 00:03:04.729557 humanloop-0.4.0a4/humanloop/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     1667 2023-05-16 00:03:04.729659 humanloop-0.4.0a4/humanloop/model/label_sentiment.py
+-rw-r--r--   0        0        0     1468 2023-05-16 00:03:04.729775 humanloop-0.4.0a4/humanloop/model/label_sentiment.pyi
+-rw-r--r--   0        0        0     3156 2023-05-16 00:03:04.729901 humanloop-0.4.0a4/humanloop/model/log_datapoint_request.py
+-rw-r--r--   0        0        0     3156 2023-05-16 00:03:04.730045 humanloop-0.4.0a4/humanloop/model/log_datapoint_request.pyi
+-rw-r--r--   0        0        0    14677 2023-05-16 00:03:04.730220 humanloop-0.4.0a4/humanloop/model/log_request.py
+-rw-r--r--   0        0        0    14677 2023-05-16 00:03:04.730378 humanloop-0.4.0a4/humanloop/model/log_request.pyi
+-rw-r--r--   0        0        0    18636 2023-05-16 00:03:04.730513 humanloop-0.4.0a4/humanloop/model/log_response.py
+-rw-r--r--   0        0        0    18636 2023-05-16 00:03:04.730663 humanloop-0.4.0a4/humanloop/model/log_response.pyi
+-rw-r--r--   0        0        0     3205 2023-05-16 00:03:04.730802 humanloop-0.4.0a4/humanloop/model/logs_log_response.py
+-rw-r--r--   0        0        0     3205 2023-05-16 00:03:04.730911 humanloop-0.4.0a4/humanloop/model/logs_log_response.pyi
+-rw-r--r--   0        0        0    16089 2023-05-16 00:03:04.731013 humanloop-0.4.0a4/humanloop/model/model_config_chat_request.py
+-rw-r--r--   0        0        0    16089 2023-05-16 00:03:04.731143 humanloop-0.4.0a4/humanloop/model/model_config_chat_request.pyi
+-rw-r--r--   0        0        0    15229 2023-05-16 00:03:04.731260 humanloop-0.4.0a4/humanloop/model/model_config_completion_request.py
+-rw-r--r--   0        0        0    15229 2023-05-16 00:03:04.731417 humanloop-0.4.0a4/humanloop/model/model_config_completion_request.pyi
+-rw-r--r--   0        0        0     1460 2023-05-16 00:03:04.731575 humanloop-0.4.0a4/humanloop/model/model_endpoints.py
+-rw-r--r--   0        0        0     1305 2023-05-16 00:03:04.731690 humanloop-0.4.0a4/humanloop/model/model_endpoints.pyi
+-rw-r--r--   0        0        0     1695 2023-05-16 00:03:04.731807 humanloop-0.4.0a4/humanloop/model/model_providers.py
+-rw-r--r--   0        0        0     1468 2023-05-16 00:03:04.731920 humanloop-0.4.0a4/humanloop/model/model_providers.pyi
+-rw-r--r--   0        0        0     5144 2023-05-16 00:03:04.732047 humanloop-0.4.0a4/humanloop/model/paginated_data_log_response.py
+-rw-r--r--   0        0        0     5144 2023-05-16 00:03:04.732174 humanloop-0.4.0a4/humanloop/model/paginated_data_log_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-16 00:03:04.732291 humanloop-0.4.0a4/humanloop/model/paginated_data_project_response.py
+-rw-r--r--   0        0        0     5180 2023-05-16 00:03:04.732488 humanloop-0.4.0a4/humanloop/model/paginated_data_project_response.pyi
+-rw-r--r--   0        0        0     3143 2023-05-16 00:03:04.732659 humanloop-0.4.0a4/humanloop/model/positive_label.py
+-rw-r--r--   0        0        0     3143 2023-05-16 00:03:04.733065 humanloop-0.4.0a4/humanloop/model/positive_label.pyi
+-rw-r--r--   0        0        0    18363 2023-05-16 00:03:04.733235 humanloop-0.4.0a4/humanloop/model/project_model_config_request.py
+-rw-r--r--   0        0        0    18363 2023-05-16 00:03:04.733468 humanloop-0.4.0a4/humanloop/model/project_model_config_request.pyi
+-rw-r--r--   0        0        0    13460 2023-05-16 00:03:04.733675 humanloop-0.4.0a4/humanloop/model/project_response.py
+-rw-r--r--   0        0        0    13460 2023-05-16 00:03:04.733834 humanloop-0.4.0a4/humanloop/model/project_response.pyi
+-rw-r--r--   0        0        0     1471 2023-05-16 00:03:04.733986 humanloop-0.4.0a4/humanloop/model/project_sort_by.py
+-rw-r--r--   0        0        0     1300 2023-05-16 00:03:04.734138 humanloop-0.4.0a4/humanloop/model/project_sort_by.pyi
+-rw-r--r--   0        0        0     3795 2023-05-16 00:03:04.734264 humanloop-0.4.0a4/humanloop/model/project_user_response.py
+-rw-r--r--   0        0        0     3795 2023-05-16 00:03:04.734358 humanloop-0.4.0a4/humanloop/model/project_user_response.pyi
+-rw-r--r--   0        0        0     2004 2023-05-16 00:03:04.734475 humanloop-0.4.0a4/humanloop/model/projects_get_model_configs_response.py
+-rw-r--r--   0        0        0     2004 2023-05-16 00:03:04.734568 humanloop-0.4.0a4/humanloop/model/projects_get_model_configs_response.pyi
+-rw-r--r--   0        0        0     1715 2023-05-16 00:03:04.734680 humanloop-0.4.0a4/humanloop/model/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1715 2023-05-16 00:03:04.734801 humanloop-0.4.0a4/humanloop/model/projects_update_feedback_types_request.pyi
+-rw-r--r--   0        0        0     4150 2023-05-16 00:03:04.734926 humanloop-0.4.0a4/humanloop/model/provider_api_keys.py
+-rw-r--r--   0        0        0     4150 2023-05-16 00:03:04.735051 humanloop-0.4.0a4/humanloop/model/provider_api_keys.pyi
+-rw-r--r--   0        0        0     3675 2023-05-16 00:03:04.735168 humanloop-0.4.0a4/humanloop/model/session_app_response.py
+-rw-r--r--   0        0        0     3675 2023-05-16 00:03:04.735292 humanloop-0.4.0a4/humanloop/model/session_app_response.pyi
+-rw-r--r--   0        0        0     4394 2023-05-16 00:03:04.735427 humanloop-0.4.0a4/humanloop/model/session_response.py
+-rw-r--r--   0        0        0     4394 2023-05-16 00:03:04.735578 humanloop-0.4.0a4/humanloop/model/session_response.pyi
+-rw-r--r--   0        0        0     1309 2023-05-16 00:03:04.735714 humanloop-0.4.0a4/humanloop/model/sort_order.py
+-rw-r--r--   0        0        0     1192 2023-05-16 00:03:04.735826 humanloop-0.4.0a4/humanloop/model/sort_order.pyi
+-rw-r--r--   0        0        0    17927 2023-05-16 00:03:04.736012 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py
+-rw-r--r--   0        0        0    17927 2023-05-16 00:03:04.736235 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi
+-rw-r--r--   0        0        0     4889 2023-05-16 00:03:04.736390 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4889 2023-05-16 00:03:04.736521 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0    24036 2023-05-16 00:03:04.736692 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py
+-rw-r--r--   0        0        0    24036 2023-05-16 00:03:04.736890 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi
+-rw-r--r--   0        0        0    17927 2023-05-16 00:03:04.737114 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py
+-rw-r--r--   0        0        0    17927 2023-05-16 00:03:04.737291 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi
+-rw-r--r--   0        0        0     4889 2023-05-16 00:03:04.737443 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4889 2023-05-16 00:03:04.737587 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0    24036 2023-05-16 00:03:04.737753 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py
+-rw-r--r--   0        0        0    24036 2023-05-16 00:03:04.737961 humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi
+-rw-r--r--   0        0        0     4232 2023-05-16 00:03:04.738110 humanloop-0.4.0a4/humanloop/model/tool_result_response.py
+-rw-r--r--   0        0        0     4232 2023-05-16 00:03:04.738231 humanloop-0.4.0a4/humanloop/model/tool_result_response.pyi
+-rw-r--r--   0        0        0     7302 2023-05-16 00:03:04.738336 humanloop-0.4.0a4/humanloop/model/update_experiment_request.py
+-rw-r--r--   0        0        0     7302 2023-05-16 00:03:04.738427 humanloop-0.4.0a4/humanloop/model/update_experiment_request.pyi
+-rw-r--r--   0        0        0     5125 2023-05-16 00:03:04.738526 humanloop-0.4.0a4/humanloop/model/update_project_request.py
+-rw-r--r--   0        0        0     5125 2023-05-16 00:03:04.738619 humanloop-0.4.0a4/humanloop/model/update_project_request.pyi
+-rw-r--r--   0        0        0     4118 2023-05-16 00:03:04.738724 humanloop-0.4.0a4/humanloop/model/usage.py
+-rw-r--r--   0        0        0     4118 2023-05-16 00:03:04.738826 humanloop-0.4.0a4/humanloop/model/usage.pyi
+-rw-r--r--   0        0        0     6805 2023-05-16 00:03:04.738923 humanloop-0.4.0a4/humanloop/model/validation_error.py
+-rw-r--r--   0        0        0     6805 2023-05-16 00:03:04.739021 humanloop-0.4.0a4/humanloop/model/validation_error.pyi
+-rw-r--r--   0        0        0     5725 2023-05-16 00:03:04.739123 humanloop-0.4.0a4/humanloop/models/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-16 00:03:04.739229 humanloop-0.4.0a4/humanloop/paths/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-16 00:03:04.739330 humanloop-0.4.0a4/humanloop/paths/apps/__init__.py
+-rw-r--r--   0        0        0    12735 2023-05-16 00:03:04.739426 humanloop-0.4.0a4/humanloop/paths/apps/get.py
+-rw-r--r--   0        0        0    12592 2023-05-16 00:03:04.739557 humanloop-0.4.0a4/humanloop/paths/apps/get.pyi
+-rw-r--r--   0        0        0      291 2023-05-16 00:03:04.739684 humanloop-0.4.0a4/humanloop/paths/apps_id/__init__.py
+-rw-r--r--   0        0        0    11966 2023-05-16 00:03:04.739788 humanloop-0.4.0a4/humanloop/paths/apps_id/get.py
+-rw-r--r--   0        0        0    11823 2023-05-16 00:03:04.739912 humanloop-0.4.0a4/humanloop/paths/apps_id/get.pyi
+-rw-r--r--   0        0        0      309 2023-05-16 00:03:04.740043 humanloop-0.4.0a4/humanloop/paths/apps_id_sessions/__init__.py
+-rw-r--r--   0        0        0    15570 2023-05-16 00:03:04.740149 humanloop-0.4.0a4/humanloop/paths/apps_id_sessions/get.py
+-rw-r--r--   0        0        0    15427 2023-05-16 00:03:04.740271 humanloop-0.4.0a4/humanloop/paths/apps_id_sessions/get.pyi
+-rw-r--r--   0        0        0      285 2023-05-16 00:03:04.740399 humanloop-0.4.0a4/humanloop/paths/chat/__init__.py
+-rw-r--r--   0        0        0    17428 2023-05-16 00:03:04.740507 humanloop-0.4.0a4/humanloop/paths/chat/post.py
+-rw-r--r--   0        0        0    17285 2023-05-16 00:03:04.740637 humanloop-0.4.0a4/humanloop/paths/chat/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-16 00:03:04.740747 humanloop-0.4.0a4/humanloop/paths/chat_deployed/__init__.py
+-rw-r--r--   0        0        0    16991 2023-05-16 00:03:04.740843 humanloop-0.4.0a4/humanloop/paths/chat_deployed/post.py
+-rw-r--r--   0        0        0    16848 2023-05-16 00:03:04.740961 humanloop-0.4.0a4/humanloop/paths/chat_deployed/post.pyi
+-rw-r--r--   0        0        0      306 2023-05-16 00:03:04.741110 humanloop-0.4.0a4/humanloop/paths/chat_experiment/__init__.py
+-rw-r--r--   0        0        0    17434 2023-05-16 00:03:04.741231 humanloop-0.4.0a4/humanloop/paths/chat_experiment/post.py
+-rw-r--r--   0        0        0    17291 2023-05-16 00:03:04.741353 humanloop-0.4.0a4/humanloop/paths/chat_experiment/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-16 00:03:04.741467 humanloop-0.4.0a4/humanloop/paths/chat_model_config/__init__.py
+-rw-r--r--   0        0        0    17609 2023-05-16 00:03:04.741582 humanloop-0.4.0a4/humanloop/paths/chat_model_config/post.py
+-rw-r--r--   0        0        0    17466 2023-05-16 00:03:04.741703 humanloop-0.4.0a4/humanloop/paths/chat_model_config/post.pyi
+-rw-r--r--   0        0        0      297 2023-05-16 00:03:04.741806 humanloop-0.4.0a4/humanloop/paths/completion/__init__.py
+-rw-r--r--   0        0        0    17744 2023-05-16 00:03:04.741909 humanloop-0.4.0a4/humanloop/paths/completion/post.py
+-rw-r--r--   0        0        0    17601 2023-05-16 00:03:04.742045 humanloop-0.4.0a4/humanloop/paths/completion/post.pyi
+-rw-r--r--   0        0        0      314 2023-05-16 00:03:04.742156 humanloop-0.4.0a4/humanloop/paths/completion_deployed/__init__.py
+-rw-r--r--   0        0        0    17247 2023-05-16 00:03:04.742268 humanloop-0.4.0a4/humanloop/paths/completion_deployed/post.py
+-rw-r--r--   0        0        0    17104 2023-05-16 00:03:04.742384 humanloop-0.4.0a4/humanloop/paths/completion_deployed/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-16 00:03:04.742492 humanloop-0.4.0a4/humanloop/paths/completion_experiment/__init__.py
+-rw-r--r--   0        0        0    17690 2023-05-16 00:03:04.742601 humanloop-0.4.0a4/humanloop/paths/completion_experiment/post.py
+-rw-r--r--   0        0        0    17547 2023-05-16 00:03:04.742728 humanloop-0.4.0a4/humanloop/paths/completion_experiment/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-16 00:03:04.742832 humanloop-0.4.0a4/humanloop/paths/completion_model_config/__init__.py
+-rw-r--r--   0        0        0    17865 2023-05-16 00:03:04.742975 humanloop-0.4.0a4/humanloop/paths/completion_model_config/post.py
+-rw-r--r--   0        0        0    17722 2023-05-16 00:03:04.743208 humanloop-0.4.0a4/humanloop/paths/completion_model_config/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-16 00:03:04.743349 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/__init__.py
+-rw-r--r--   0        0        0    11995 2023-05-16 00:03:04.743452 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/delete.py
+-rw-r--r--   0        0        0    11852 2023-05-16 00:03:04.743592 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/delete.pyi
+-rw-r--r--   0        0        0    17043 2023-05-16 00:03:04.743747 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/patch.py
+-rw-r--r--   0        0        0    16900 2023-05-16 00:03:04.743879 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/patch.pyi
+-rw-r--r--   0        0        0      352 2023-05-16 00:03:04.744011 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12496 2023-05-16 00:03:04.744108 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id_model_config/get.py
+-rw-r--r--   0        0        0    12353 2023-05-16 00:03:04.744228 humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id_model_config/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-16 00:03:04.744350 humanloop-0.4.0a4/humanloop/paths/feedback/__init__.py
+-rw-r--r--   0        0        0    15089 2023-05-16 00:03:04.744488 humanloop-0.4.0a4/humanloop/paths/feedback/post.py
+-rw-r--r--   0        0        0    14946 2023-05-16 00:03:04.744677 humanloop-0.4.0a4/humanloop/paths/feedback/post.pyi
+-rw-r--r--   0        0        0      285 2023-05-16 00:03:04.744815 humanloop-0.4.0a4/humanloop/paths/logs/__init__.py
+-rw-r--r--   0        0        0    19620 2023-05-16 00:03:04.744929 humanloop-0.4.0a4/humanloop/paths/logs/post.py
+-rw-r--r--   0        0        0    19477 2023-05-16 00:03:04.745057 humanloop-0.4.0a4/humanloop/paths/logs/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-16 00:03:04.745178 humanloop-0.4.0a4/humanloop/paths/model_configs/__init__.py
+-rw-r--r--   0        0        0    20552 2023-05-16 00:03:04.745285 humanloop-0.4.0a4/humanloop/paths/model_configs/post.py
+-rw-r--r--   0        0        0    20409 2023-05-16 00:03:04.745436 humanloop-0.4.0a4/humanloop/paths/model_configs/post.pyi
+-rw-r--r--   0        0        0      308 2023-05-16 00:03:04.745591 humanloop-0.4.0a4/humanloop/paths/model_configs_id/__init__.py
+-rw-r--r--   0        0        0    12309 2023-05-16 00:03:04.745723 humanloop-0.4.0a4/humanloop/paths/model_configs_id/get.py
+-rw-r--r--   0        0        0    12166 2023-05-16 00:03:04.745878 humanloop-0.4.0a4/humanloop/paths/model_configs_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-16 00:03:04.746008 humanloop-0.4.0a4/humanloop/paths/projects/__init__.py
+-rw-r--r--   0        0        0    20518 2023-05-16 00:03:04.746251 humanloop-0.4.0a4/humanloop/paths/projects/get.py
+-rw-r--r--   0        0        0    20375 2023-05-16 00:03:04.746431 humanloop-0.4.0a4/humanloop/paths/projects/get.pyi
+-rw-r--r--   0        0        0    13007 2023-05-16 00:03:04.746568 humanloop-0.4.0a4/humanloop/paths/projects/post.py
+-rw-r--r--   0        0        0    12864 2023-05-16 00:03:04.746697 humanloop-0.4.0a4/humanloop/paths/projects/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-16 00:03:04.746835 humanloop-0.4.0a4/humanloop/paths/projects_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-16 00:03:04.746962 humanloop-0.4.0a4/humanloop/paths/projects_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-16 00:03:04.747102 humanloop-0.4.0a4/humanloop/paths/projects_id/get.pyi
+-rw-r--r--   0        0        0    16162 2023-05-16 00:03:04.747305 humanloop-0.4.0a4/humanloop/paths/projects_id/patch.py
+-rw-r--r--   0        0        0    16019 2023-05-16 00:03:04.747471 humanloop-0.4.0a4/humanloop/paths/projects_id/patch.pyi
+-rw-r--r--   0        0        0      334 2023-05-16 00:03:04.747674 humanloop-0.4.0a4/humanloop/paths/projects_id_active_experiment/__init__.py
+-rw-r--r--   0        0        0    12306 2023-05-16 00:03:04.747801 humanloop-0.4.0a4/humanloop/paths/projects_id_active_experiment/delete.py
+-rw-r--r--   0        0        0    12163 2023-05-16 00:03:04.747950 humanloop-0.4.0a4/humanloop/paths/projects_id_active_experiment/delete.pyi
+-rw-r--r--   0        0        0      337 2023-05-16 00:03:04.748093 humanloop-0.4.0a4/humanloop/paths/projects_id_active_model_config/__init__.py
+-rw-r--r--   0        0        0    12337 2023-05-16 00:03:04.748220 humanloop-0.4.0a4/humanloop/paths/projects_id_active_model_config/delete.py
+-rw-r--r--   0        0        0    12194 2023-05-16 00:03:04.748385 humanloop-0.4.0a4/humanloop/paths/projects_id_active_model_config/delete.pyi
+-rw-r--r--   0        0        0      313 2023-05-16 00:03:04.748535 humanloop-0.4.0a4/humanloop/paths/projects_id_export/__init__.py
+-rw-r--r--   0        0        0    15728 2023-05-16 00:03:04.748647 humanloop-0.4.0a4/humanloop/paths/projects_id_export/post.py
+-rw-r--r--   0        0        0    15585 2023-05-16 00:03:04.748762 humanloop-0.4.0a4/humanloop/paths/projects_id_export/post.pyi
+-rw-r--r--   0        0        0      328 2023-05-16 00:03:04.748875 humanloop-0.4.0a4/humanloop/paths/projects_id_feedback_types/__init__.py
+-rw-r--r--   0        0        0    14809 2023-05-16 00:03:04.748967 humanloop-0.4.0a4/humanloop/paths/projects_id_feedback_types/patch.py
+-rw-r--r--   0        0        0    14666 2023-05-16 00:03:04.749078 humanloop-0.4.0a4/humanloop/paths/projects_id_feedback_types/patch.pyi
+-rw-r--r--   0        0        0      324 2023-05-16 00:03:04.749191 humanloop-0.4.0a4/humanloop/paths/projects_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12229 2023-05-16 00:03:04.749297 humanloop-0.4.0a4/humanloop/paths/projects_id_model_config/get.py
+-rw-r--r--   0        0        0    12086 2023-05-16 00:03:04.749422 humanloop-0.4.0a4/humanloop/paths/projects_id_model_config/get.pyi
+-rw-r--r--   0        0        0      326 2023-05-16 00:03:04.749535 humanloop-0.4.0a4/humanloop/paths/projects_id_model_configs/__init__.py
+-rw-r--r--   0        0        0    12319 2023-05-16 00:03:04.749637 humanloop-0.4.0a4/humanloop/paths/projects_id_model_configs/get.py
+-rw-r--r--   0        0        0    12176 2023-05-16 00:03:04.749748 humanloop-0.4.0a4/humanloop/paths/projects_id_model_configs/get.pyi
+-rw-r--r--   0        0        0      339 2023-05-16 00:03:04.749897 humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/__init__.py
+-rw-r--r--   0        0        0    12256 2023-05-16 00:03:04.750004 humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/get.py
+-rw-r--r--   0        0        0    12113 2023-05-16 00:03:04.750139 humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/get.pyi
+-rw-r--r--   0        0        0    16346 2023-05-16 00:03:04.750266 humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/post.py
+-rw-r--r--   0        0        0    16203 2023-05-16 00:03:04.750393 humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/post.pyi
+-rw-r--r--   0        0        0      293 2023-05-16 00:03:04.750563 humanloop-0.4.0a4/humanloop/paths/sessions/__init__.py
+-rw-r--r--   0        0        0    12149 2023-05-16 00:03:04.750690 humanloop-0.4.0a4/humanloop/paths/sessions/post.py
+-rw-r--r--   0        0        0    12006 2023-05-16 00:03:04.750841 humanloop-0.4.0a4/humanloop/paths/sessions/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-16 00:03:04.750989 humanloop-0.4.0a4/humanloop/paths/sessions_id/__init__.py
+-rw-r--r--   0        0        0    11974 2023-05-16 00:03:04.751101 humanloop-0.4.0a4/humanloop/paths/sessions_id/get.py
+-rw-r--r--   0        0        0    11831 2023-05-16 00:03:04.751232 humanloop-0.4.0a4/humanloop/paths/sessions_id/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-16 00:03:04.751354 humanloop-0.4.0a4/humanloop/paths/sessions_id_events/__init__.py
+-rw-r--r--   0        0        0    12085 2023-05-16 00:03:04.751542 humanloop-0.4.0a4/humanloop/paths/sessions_id_events/get.py
+-rw-r--r--   0        0        0    11942 2023-05-16 00:03:04.751850 humanloop-0.4.0a4/humanloop/paths/sessions_id_events/get.pyi
+-rw-r--r--   0        0        0     1011 2023-05-16 00:03:04.752020 humanloop-0.4.0a4/humanloop/request_after_hook.py
+-rw-r--r--   0        0        0     1012 2023-05-16 00:03:04.752202 humanloop-0.4.0a4/humanloop/request_before_hook.py
+-rw-r--r--   0        0        0    11329 2023-05-16 00:03:04.752391 humanloop-0.4.0a4/humanloop/rest.py
+-rw-r--r--   0        0        0    95913 2023-05-16 00:03:04.752893 humanloop-0.4.0a4/humanloop/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-16 00:03:04.753119 humanloop-0.4.0a4/humanloop/type/__init__.py
+-rw-r--r--   0        0        0     1489 2023-05-16 00:03:04.753292 humanloop-0.4.0a4/humanloop/type/base_metric_response.py
+-rw-r--r--   0        0        0     1137 2023-05-16 00:03:04.753445 humanloop-0.4.0a4/humanloop/type/categorical_feedback_label.py
+-rw-r--r--   0        0        0     2272 2023-05-16 00:03:04.753659 humanloop-0.4.0a4/humanloop/type/chat_data_response.py
+-rw-r--r--   0        0        0     2085 2023-05-16 00:03:04.753823 humanloop-0.4.0a4/humanloop/type/chat_deployed_request.py
+-rw-r--r--   0        0        0     2337 2023-05-16 00:03:04.753982 humanloop-0.4.0a4/humanloop/type/chat_experiment_request.py
+-rw-r--r--   0        0        0      980 2023-05-16 00:03:04.754362 humanloop-0.4.0a4/humanloop/type/chat_message.py
+-rw-r--r--   0        0        0     2208 2023-05-16 00:03:04.754545 humanloop-0.4.0a4/humanloop/type/chat_model_config_request.py
+-rw-r--r--   0        0        0     2212 2023-05-16 00:03:04.754701 humanloop-0.4.0a4/humanloop/type/chat_request.py
+-rw-r--r--   0        0        0     1899 2023-05-16 00:03:04.754855 humanloop-0.4.0a4/humanloop/type/chat_response.py
+-rw-r--r--   0        0        0      711 2023-05-16 00:03:04.755022 humanloop-0.4.0a4/humanloop/type/chat_role.py
+-rw-r--r--   0        0        0     2205 2023-05-16 00:03:04.755133 humanloop-0.4.0a4/humanloop/type/completion_deployed_request.py
+-rw-r--r--   0        0        0     2460 2023-05-16 00:03:04.755233 humanloop-0.4.0a4/humanloop/type/completion_experiment_request.py
+-rw-r--r--   0        0        0     2328 2023-05-16 00:03:04.755430 humanloop-0.4.0a4/humanloop/type/completion_model_config_request.py
+-rw-r--r--   0        0        0     2336 2023-05-16 00:03:04.755625 humanloop-0.4.0a4/humanloop/type/completion_request.py
+-rw-r--r--   0        0        0     1957 2023-05-16 00:03:04.755795 humanloop-0.4.0a4/humanloop/type/completion_response.py
+-rw-r--r--   0        0        0     1468 2023-05-16 00:03:04.756006 humanloop-0.4.0a4/humanloop/type/create_experiment_request.py
+-rw-r--r--   0        0        0     1085 2023-05-16 00:03:04.756306 humanloop-0.4.0a4/humanloop/type/create_log_response.py
+-rw-r--r--   0        0        0     1142 2023-05-16 00:03:04.756541 humanloop-0.4.0a4/humanloop/type/create_project_request.py
+-rw-r--r--   0        0        0     1000 2023-05-16 00:03:04.756791 humanloop-0.4.0a4/humanloop/type/create_session_request.py
+-rw-r--r--   0        0        0     2091 2023-05-16 00:03:04.757863 humanloop-0.4.0a4/humanloop/type/data_response.py
+-rw-r--r--   0        0        0     1954 2023-05-16 00:03:04.758085 humanloop-0.4.0a4/humanloop/type/experiment_model_config_response.py
+-rw-r--r--   0        0        0     1909 2023-05-16 00:03:04.758275 humanloop-0.4.0a4/humanloop/type/experiment_response.py
+-rw-r--r--   0        0        0      718 2023-05-16 00:03:04.758424 humanloop-0.4.0a4/humanloop/type/experiment_status.py
+-rw-r--r--   0        0        0      785 2023-05-16 00:03:04.758581 humanloop-0.4.0a4/humanloop/type/experiments_list_response.py
+-rw-r--r--   0        0        0     1510 2023-05-16 00:03:04.758767 humanloop-0.4.0a4/humanloop/type/feedback.py
+-rw-r--r--   0        0        0      719 2023-05-16 00:03:04.758991 humanloop-0.4.0a4/humanloop/type/feedback_class.py
+-rw-r--r--   0        0        0     1046 2023-05-16 00:03:04.759214 humanloop-0.4.0a4/humanloop/type/feedback_label_request.py
+-rw-r--r--   0        0        0     1624 2023-05-16 00:03:04.759425 humanloop-0.4.0a4/humanloop/type/feedback_request.py
+-rw-r--r--   0        0        0     1658 2023-05-16 00:03:04.759599 humanloop-0.4.0a4/humanloop/type/feedback_response.py
+-rw-r--r--   0        0        0      804 2023-05-16 00:03:04.759807 humanloop-0.4.0a4/humanloop/type/feedback_submit_request.py
+-rw-r--r--   0        0        0      809 2023-05-16 00:03:04.760000 humanloop-0.4.0a4/humanloop/type/feedback_submit_response.py
+-rw-r--r--   0        0        0      738 2023-05-16 00:03:04.760186 humanloop-0.4.0a4/humanloop/type/feedback_type.py
+-rw-r--r--   0        0        0     1377 2023-05-16 00:03:04.760353 humanloop-0.4.0a4/humanloop/type/feedback_type_model.py
+-rw-r--r--   0        0        0     1541 2023-05-16 00:03:04.760531 humanloop-0.4.0a4/humanloop/type/feedback_type_request.py
+-rw-r--r--   0        0        0      773 2023-05-16 00:03:04.760686 humanloop-0.4.0a4/humanloop/type/feedback_types.py
+-rw-r--r--   0        0        0     4271 2023-05-16 00:03:04.760843 humanloop-0.4.0a4/humanloop/type/get_model_config_response.py
+-rw-r--r--   0        0        0     1034 2023-05-16 00:03:04.761010 humanloop-0.4.0a4/humanloop/type/http_validation_error.py
+-rw-r--r--   0        0        0      730 2023-05-16 00:03:04.761164 humanloop-0.4.0a4/humanloop/type/label_sentiment.py
+-rw-r--r--   0        0        0      782 2023-05-16 00:03:04.761327 humanloop-0.4.0a4/humanloop/type/log_datapoint_request.py
+-rw-r--r--   0        0        0     2430 2023-05-16 00:03:04.761466 humanloop-0.4.0a4/humanloop/type/log_request.py
+-rw-r--r--   0        0        0     2968 2023-05-16 00:03:04.761614 humanloop-0.4.0a4/humanloop/type/log_response.py
+-rw-r--r--   0        0        0      807 2023-05-16 00:03:04.761751 humanloop-0.4.0a4/humanloop/type/logs_log_response.py
+-rw-r--r--   0        0        0     2927 2023-05-16 00:03:04.761904 humanloop-0.4.0a4/humanloop/type/model_config_chat_request.py
+-rw-r--r--   0        0        0     2832 2023-05-16 00:03:04.762058 humanloop-0.4.0a4/humanloop/type/model_config_completion_request.py
+-rw-r--r--   0        0        0      714 2023-05-16 00:03:04.762205 humanloop-0.4.0a4/humanloop/type/model_endpoints.py
+-rw-r--r--   0        0        0      738 2023-05-16 00:03:04.762350 humanloop-0.4.0a4/humanloop/type/model_providers.py
+-rw-r--r--   0        0        0     1113 2023-05-16 00:03:04.762502 humanloop-0.4.0a4/humanloop/type/paginated_data_log_response.py
+-rw-r--r--   0        0        0     1153 2023-05-16 00:03:04.762662 humanloop-0.4.0a4/humanloop/type/paginated_data_project_response.py
+-rw-r--r--   0        0        0      924 2023-05-16 00:03:04.762851 humanloop-0.4.0a4/humanloop/type/positive_label.py
+-rw-r--r--   0        0        0     3535 2023-05-16 00:03:04.762992 humanloop-0.4.0a4/humanloop/type/project_model_config_request.py
+-rw-r--r--   0        0        0     2190 2023-05-16 00:03:04.763147 humanloop-0.4.0a4/humanloop/type/project_response.py
+-rw-r--r--   0        0        0      721 2023-05-16 00:03:04.763295 humanloop-0.4.0a4/humanloop/type/project_sort_by.py
+-rw-r--r--   0        0        0     1099 2023-05-16 00:03:04.763447 humanloop-0.4.0a4/humanloop/type/project_user_response.py
+-rw-r--r--   0        0        0      928 2023-05-16 00:03:04.763600 humanloop-0.4.0a4/humanloop/type/projects_get_model_configs_response.py
+-rw-r--r--   0        0        0      800 2023-05-16 00:03:04.764224 humanloop-0.4.0a4/humanloop/type/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0      980 2023-05-16 00:03:04.764386 humanloop-0.4.0a4/humanloop/type/provider_api_keys.py
+-rw-r--r--   0        0        0     1024 2023-05-16 00:03:04.764546 humanloop-0.4.0a4/humanloop/type/session_app_response.py
+-rw-r--r--   0        0        0     1074 2023-05-16 00:03:04.764695 humanloop-0.4.0a4/humanloop/type/session_response.py
+-rw-r--r--   0        0        0      696 2023-05-16 00:03:04.764836 humanloop-0.4.0a4/humanloop/type/sort_order.py
+-rw-r--r--   0        0        0     3508 2023-05-16 00:03:04.764982 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py
+-rw-r--r--   0        0        0     1420 2023-05-16 00:03:04.765800 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4439 2023-05-16 00:03:04.766109 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_response.py
+-rw-r--r--   0        0        0     3528 2023-05-16 00:03:04.766309 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_model_config_response.py
+-rw-r--r--   0        0        0     1420 2023-05-16 00:03:04.766487 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4459 2023-05-16 00:03:04.766643 humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_response.py
+-rw-r--r--   0        0        0      999 2023-05-16 00:03:04.766797 humanloop-0.4.0a4/humanloop/type/tool_result_response.py
+-rw-r--r--   0        0        0     1440 2023-05-16 00:03:04.766998 humanloop-0.4.0a4/humanloop/type/update_experiment_request.py
+-rw-r--r--   0        0        0     1529 2023-05-16 00:03:04.767215 humanloop-0.4.0a4/humanloop/type/update_project_request.py
+-rw-r--r--   0        0        0     1082 2023-05-16 00:03:04.767362 humanloop-0.4.0a4/humanloop/type/usage.py
+-rw-r--r--   0        0        0     1011 2023-05-16 00:03:04.767563 humanloop-0.4.0a4/humanloop/type/validation_error.py
+-rw-r--r--   0        0        0      868 2023-05-16 00:03:04.767830 humanloop-0.4.0a4/humanloop/type_util.py
+-rw-r--r--   0        0        0     3165 2023-05-16 00:03:04.768042 humanloop-0.4.0a4/humanloop/validation_metadata.py
+-rw-r--r--   0        0        0     1121 2023-05-16 00:03:04.768757 humanloop-0.4.0a4/pyproject.toml
+-rw-r--r--   0        0        0     8827 1970-01-01 00:00:00.000000 humanloop-0.4.0a4/PKG-INFO
```

### Comparing `humanloop-0.4.0/LICENSE` & `humanloop-0.4.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/README.md` & `humanloop-0.4.0a4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# humanloop@0.4.0
+# humanloop@0.4.0a4
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.0
+pip install humanloop==0.4.0a4
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
@@ -54,15 +54,15 @@
     pprint(chat_response.body["project_id"])
     pprint(chat_response.body["data"][0])
     pprint(chat_response.body["provider_responses"])
     pprint(chat_response.headers)
     pprint(chat_response.status)
     pprint(chat_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .chat: %s\n" % e)
+    print("Exception when calling .response: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -86,15 +86,15 @@
     pprint(complete_response.body["project_id"])
     pprint(complete_response.body["data"][0])
     pprint(complete_response.body["provider_responses"])
     pprint(complete_response.headers)
     pprint(complete_response.status)
     pprint(complete_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .complete: %s\n" % e)
+    print("Exception when calling .create: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -108,15 +108,15 @@
         user="user@example.com",
     )
     pprint(feedback_response.body)
     pprint(feedback_response.headers)
     pprint(feedback_response.status)
     pprint(feedback_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .feedback: %s\n" % e)
+    print("Exception when calling .submit: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -153,47 +153,39 @@
 ```
 
 ## Async
 
 `async` support is available by prepending `a` to any method.
 
 ```python
-import asyncio
 from pprint import pprint
 from humanloop import Humanloop, ApiException
 
 humanloop = Humanloop(
+    # Defining the host is optional and defaults to https://api.humanloop.com/v4
+    # See configuration.py for a list of all supported configuration parameters.
+    host="https://api.humanloop.com/v4",
+    # Configure API key authorization: APIKeyHeader
     api_key="YOUR_API_KEY",
+    # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+    # api_key_prefix = {'APIKeyHeader': 'Bearer'},
 )
 
 
 async def main():
     try:
-        complete_response = await humanloop.acomplete(
-            project="sdk-example",
-            inputs={
-                "text": "Llamas that are well-socialized and trained to halter and lead after weaning and are very friendly and pleasant to be around. They are extremely curious and most will approach people easily. However, llamas that are bottle-fed or over-socialized and over-handled as youth will become extremely difficult to handle when mature, when they will begin to treat humans as they treat each other, which is characterized by bouts of spitting, kicking and neck wrestling.[33]",
-            },
-            model_config={
-                "model": "gpt-3.5-turbo",
-                "max_tokens": -1,
-                "temperature": 0.7,
-                "prompt_template": "Summarize this for a second-grade student:\n\nText:\n{{text}}\n\nSummary:\n",
-            },
-            stream=False,
+        # Get App
+        get_response = await humanloop.apps.aget(
+            id="id_example",  # required
         )
-        pprint(complete_response.body)
-        pprint(complete_response.body["project_id"])
-        pprint(complete_response.body["data"][0])
-        pprint(complete_response.body["provider_responses"])
-        pprint(complete_response.headers)
-        pprint(complete_response.status)
-        pprint(complete_response.round_trip_time)
+        pprint(get_response.headers)
+        pprint(get_response.status)
+        pprint(get_response.round_trip_time)
     except ApiException as e:
-        print("Exception when calling .complete: %s\n" % e)
+        print("Exception when calling AppsApi.get: %s\n" % e)
         pprint(e.body)
         if e.status == 422:
             pprint(e.body["detail"])
         pprint(e.headers)
         pprint(e.status)
         pprint(e.reason)
         pprint(e.round_trip_time)
```

### Comparing `humanloop-0.4.0/humanloop/__init__.py` & `humanloop-0.4.0a4/humanloop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.4.0"
+__version__ = "0.4.0a4"
 
 # import ApiClient
 from humanloop.api_client import ApiClient
 
 # import Configuration
 from humanloop.configuration import Configuration
```

### Comparing `humanloop-0.4.0/humanloop/api_client.py` & `humanloop-0.4.0a4/humanloop/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2760,1805 +2760,1805 @@
 0000ac70: 6465 725f 7661 6c75 650a 2020 2020 2020  der_value.      
 0000ac80: 2020 7365 6c66 2e63 6f6f 6b69 6520 3d20    self.cookie = 
 0000ac90: 636f 6f6b 6965 0a20 2020 2020 2020 2023  cookie.        #
 0000aca0: 2053 6574 2064 6566 6175 6c74 2055 7365   Set default Use
 0000acb0: 722d 4167 656e 742e 0a20 2020 2020 2020  r-Agent..       
 0000acc0: 2073 656c 662e 7573 6572 5f61 6765 6e74   self.user_agent
 0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e30   = 'Konfig/0.4.0
-0000ace0: 2f70 7974 686f 6e27 0a0a 2020 2020 6465  /python'..    de
-0000acf0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
-0000ad00: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0000ad10: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
-0000ad20: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
-0000ad30: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
-0000ad40: 7565 2c20 7472 6163 6562 6163 6b29 3a0a  ue, traceback):.
-0000ad50: 2020 2020 2020 2020 7365 6c66 2e63 6c6f          self.clo
-0000ad60: 7365 2829 0a0a 2020 2020 6465 6620 636c  se()..    def cl
-0000ad70: 6f73 6528 7365 6c66 293a 0a20 2020 2020  ose(self):.     
-0000ad80: 2020 2069 6620 7365 6c66 2e5f 706f 6f6c     if self._pool
-0000ad90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ada0: 6c66 2e5f 706f 6f6c 2e63 6c6f 7365 2829  lf._pool.close()
-0000adb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000adc0: 662e 5f70 6f6f 6c2e 6a6f 696e 2829 0a20  f._pool.join(). 
-0000add0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ade0: 5f70 6f6f 6c20 3d20 4e6f 6e65 0a20 2020  _pool = None.   
-0000adf0: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
-0000ae00: 7474 7228 6174 6578 6974 2c20 2775 6e72  ttr(atexit, 'unr
-0000ae10: 6567 6973 7465 7227 293a 0a20 2020 2020  egister'):.     
-0000ae20: 2020 2020 2020 2020 2020 2061 7465 7869             atexi
-0000ae30: 742e 756e 7265 6769 7374 6572 2873 656c  t.unregister(sel
-0000ae40: 662e 636c 6f73 6529 0a0a 2020 2020 4070  f.close)..    @p
-0000ae50: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-0000ae60: 706f 6f6c 2873 656c 6629 3a0a 2020 2020  pool(self):.    
-0000ae70: 2020 2020 2222 2243 7265 6174 6520 7468      """Create th
-0000ae80: 7265 6164 2070 6f6f 6c20 6f6e 2066 6972  read pool on fir
-0000ae90: 7374 2072 6571 7565 7374 0a20 2020 2020  st request.     
-0000aea0: 2020 2020 6176 6f69 6473 2069 6e73 7461      avoids insta
-0000aeb0: 6e74 6961 7469 6e67 2075 6e75 7365 6420  ntiating unused 
-0000aec0: 7468 7265 6164 706f 6f6c 2066 6f72 2062  threadpool for b
-0000aed0: 6c6f 636b 696e 6720 636c 6965 6e74 732e  locking clients.
-0000aee0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000aef0: 2020 2020 2069 6620 7365 6c66 2e5f 706f       if self._po
-0000af00: 6f6c 2069 7320 4e6f 6e65 3a0a 2020 2020  ol is None:.    
-0000af10: 2020 2020 2020 2020 6174 6578 6974 2e72          atexit.r
-0000af20: 6567 6973 7465 7228 7365 6c66 2e63 6c6f  egister(self.clo
-0000af30: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-0000af40: 7365 6c66 2e5f 706f 6f6c 203d 2054 6872  self._pool = Thr
-0000af50: 6561 6450 6f6f 6c28 7365 6c66 2e70 6f6f  eadPool(self.poo
-0000af60: 6c5f 7468 7265 6164 7329 0a20 2020 2020  l_threads).     
-0000af70: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000af80: 706f 6f6c 0a0a 2020 2020 4070 726f 7065  pool..    @prope
-0000af90: 7274 790a 2020 2020 6465 6620 7573 6572  rty.    def user
-0000afa0: 5f61 6765 6e74 2873 656c 6629 3a0a 2020  _agent(self):.  
-0000afb0: 2020 2020 2020 2222 2255 7365 7220 6167        """User ag
-0000afc0: 656e 7420 666f 7220 7468 6973 2041 5049  ent for this API
-0000afd0: 2063 6c69 656e 7422 2222 0a20 2020 2020   client""".     
-0000afe0: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-0000aff0: 6566 6175 6c74 5f68 6561 6465 7273 5b27  efault_headers['
-0000b000: 5573 6572 2d41 6765 6e74 275d 0a0a 2020  User-Agent']..  
-0000b010: 2020 4075 7365 725f 6167 656e 742e 7365    @user_agent.se
-0000b020: 7474 6572 0a20 2020 2064 6566 2075 7365  tter.    def use
-0000b030: 725f 6167 656e 7428 7365 6c66 2c20 7661  r_agent(self, va
-0000b040: 6c75 6529 3a0a 2020 2020 2020 2020 7365  lue):.        se
-0000b050: 6c66 2e64 6566 6175 6c74 5f68 6561 6465  lf.default_heade
-0000b060: 7273 5b27 5573 6572 2d41 6765 6e74 275d  rs['User-Agent']
-0000b070: 203d 2076 616c 7565 0a0a 2020 2020 6465   = value..    de
-0000b080: 6620 7365 745f 6465 6661 756c 745f 6865  f set_default_he
-0000b090: 6164 6572 2873 656c 662c 2068 6561 6465  ader(self, heade
-0000b0a0: 725f 6e61 6d65 2c20 6865 6164 6572 5f76  r_name, header_v
-0000b0b0: 616c 7565 293a 0a20 2020 2020 2020 2073  alue):.        s
-0000b0c0: 656c 662e 6465 6661 756c 745f 6865 6164  elf.default_head
-0000b0d0: 6572 735b 6865 6164 6572 5f6e 616d 655d  ers[header_name]
-0000b0e0: 203d 2068 6561 6465 725f 7661 6c75 650a   = header_value.
-0000b0f0: 0a20 2020 2061 7379 6e63 2064 6566 205f  .    async def _
-0000b100: 5f61 7379 6e63 5f63 616c 6c5f 6170 6928  _async_call_api(
-0000b110: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000b120: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
-0000b130: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
-0000b140: 2020 206d 6574 686f 643a 2073 7472 2c0a     method: str,.
-0000b150: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0000b160: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0000b170: 5b48 5454 5048 6561 6465 7244 6963 745d  [HTTPHeaderDict]
-0000b180: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000b190: 2073 6572 6961 6c69 7a65 645f 626f 6479   serialized_body
-0000b1a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000b1b0: 6c5b 7479 7069 6e67 2e55 6e69 6f6e 5b73  l[typing.Union[s
-0000b1c0: 7472 2c20 6279 7465 735d 5d20 3d20 4e6f  tr, bytes]] = No
-0000b1d0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-0000b1e0: 3a20 7479 7069 6e67 2e41 6e79 203d 204e  : typing.Any = N
-0000b1f0: 6f6e 652c 0a20 2020 2020 2020 2066 6965  one,.        fie
-0000b200: 6c64 733a 2074 7970 696e 672e 4f70 7469  lds: typing.Opti
-0000b210: 6f6e 616c 5b74 7970 696e 672e 5475 706c  onal[typing.Tupl
-0000b220: 655b 7479 7069 6e67 2e54 7570 6c65 5b73  e[typing.Tuple[s
-0000b230: 7472 2c20 7374 725d 2c20 2e2e 2e5d 5d20  tr, str], ...]] 
-0000b240: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b250: 6175 7468 5f73 6574 7469 6e67 733a 2074  auth_settings: t
-0000b260: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000b270: 7970 696e 672e 4c69 7374 5b73 7472 5d5d  yping.List[str]]
-0000b280: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000b290: 2073 7472 6561 6d3a 2062 6f6f 6c20 3d20   stream: bool = 
-0000b2a0: 4661 6c73 652c 0a20 2020 2020 2020 2074  False,.        t
-0000b2b0: 696d 656f 7574 3a20 7479 7069 6e67 2e4f  imeout: typing.O
-0000b2c0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0000b2d0: 6e69 6f6e 5b69 6e74 2c20 7479 7069 6e67  nion[int, typing
-0000b2e0: 2e54 7570 6c65 5d5d 203d 204e 6f6e 652c  .Tuple]] = None,
-0000b2f0: 0a20 2020 2020 2020 2068 6f73 743a 2074  .        host: t
-0000b300: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-0000b310: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000b320: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
-0000b330: 6174 6f72 5f69 7465 7261 746f 723a 2050  ator_iterator: P
-0000b340: 7265 6669 7853 6570 6172 6174 6f72 4974  refixSeparatorIt
-0000b350: 6572 6174 6f72 203d 204e 6f6e 652c 0a20  erator = None,. 
-0000b360: 2020 2029 202d 3e20 4173 796e 6352 6573     ) -> AsyncRes
-0000b370: 706f 6e73 6557 7261 7070 6572 3a0a 0a20  ponseWrapper:.. 
-0000b380: 2020 2020 2020 2072 6571 7565 7374 5f62         request_b
-0000b390: 6566 6f72 655f 686f 6f6b 280a 2020 2020  efore_hook(.    
-0000b3a0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-0000b3b0: 5f70 6174 683d 7265 736f 7572 6365 5f70  _path=resource_p
-0000b3c0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000b3d0: 206d 6574 686f 643d 6d65 7468 6f64 2c0a   method=method,.
-0000b3e0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-0000b3f0: 6967 7572 6174 696f 6e3d 7365 6c66 2e63  iguration=self.c
-0000b400: 6f6e 6669 6775 7261 7469 6f6e 2c0a 2020  onfiguration,.  
-0000b410: 2020 2020 2020 2020 2020 626f 6479 3d62            body=b
-0000b420: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
-0000b430: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
-0000b440: 2020 2020 2020 2020 2020 2020 6175 7468              auth
-0000b450: 5f73 6574 7469 6e67 733d 6175 7468 5f73  _settings=auth_s
-0000b460: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
-0000b470: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
-0000b480: 6465 7273 2c0a 2020 2020 2020 2020 290a  ders,.        ).
-0000b490: 0a20 2020 2020 2020 2023 2068 6561 6465  .        # heade
-0000b4a0: 7220 7061 7261 6d65 7465 7273 0a20 2020  r parameters.   
-0000b4b0: 2020 2020 2075 7365 645f 6865 6164 6572       used_header
-0000b4c0: 7320 3d20 4854 5450 4865 6164 6572 4469  s = HTTPHeaderDi
-0000b4d0: 6374 2873 656c 662e 6465 6661 756c 745f  ct(self.default_
-0000b4e0: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
-0000b4f0: 2069 6620 7365 6c66 2e63 6f6f 6b69 653a   if self.cookie:
-0000b500: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
-0000b510: 6465 7273 5b27 436f 6f6b 6965 275d 203d  ders['Cookie'] =
-0000b520: 2073 656c 662e 636f 6f6b 6965 0a0a 2020   self.cookie..  
-0000b530: 2020 2020 2020 2320 6175 7468 2073 6574        # auth set
-0000b540: 7469 6e67 0a20 2020 2020 2020 2072 6573  ting.        res
-0000b550: 6f75 7263 655f 7061 7468 203d 2073 656c  ource_path = sel
-0000b560: 662e 7570 6461 7465 5f70 6172 616d 735f  f.update_params_
-0000b570: 666f 725f 6175 7468 280a 2020 2020 2020  for_auth(.      
-0000b580: 2020 2020 2020 7573 6564 5f68 6561 6465        used_heade
-0000b590: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-0000b5a0: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
-0000b5b0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-0000b5c0: 7263 655f 7061 7468 2c0a 2020 2020 2020  rce_path,.      
-0000b5d0: 2020 2020 2020 6d65 7468 6f64 2c0a 2020        method,.  
-0000b5e0: 2020 2020 2020 2020 2020 626f 6479 2c0a            body,.
-0000b5f0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
-0000b600: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-0000b610: 7261 746f 720a 2020 2020 2020 2020 290a  rator.        ).
-0000b620: 0a20 2020 2020 2020 2023 206d 7573 7420  .        # must 
-0000b630: 6861 7070 656e 2061 6674 6572 2063 6f6f  happen after coo
-0000b640: 6b69 6520 7365 7474 696e 6720 616e 6420  kie setting and 
-0000b650: 6175 7468 2073 6574 7469 6e67 2069 6e20  auth setting in 
-0000b660: 6361 7365 2075 7365 7220 6973 206f 7665  case user is ove
-0000b670: 7272 6964 696e 6720 7468 6f73 650a 2020  rriding those.  
-0000b680: 2020 2020 2020 6966 2068 6561 6465 7273        if headers
-0000b690: 3a0a 2020 2020 2020 2020 2020 2020 7573  :.            us
-0000b6a0: 6564 5f68 6561 6465 7273 2e75 7064 6174  ed_headers.updat
-0000b6b0: 6528 6865 6164 6572 7329 0a0a 2020 2020  e(headers)..    
-0000b6c0: 2020 2020 2320 7265 7175 6573 7420 7572      # request ur
-0000b6d0: 6c0a 2020 2020 2020 2020 6966 2068 6f73  l.        if hos
-0000b6e0: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
-0000b6f0: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
-0000b700: 662e 636f 6e66 6967 7572 6174 696f 6e2e  f.configuration.
-0000b710: 686f 7374 202b 2072 6573 6f75 7263 655f  host + resource_
-0000b720: 7061 7468 0a20 2020 2020 2020 2065 6c73  path.        els
-0000b730: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000b740: 2075 7365 2073 6572 7665 722f 686f 7374   use server/host
-0000b750: 2064 6566 696e 6564 2069 6e20 7061 7468   defined in path
-0000b760: 206f 7220 6f70 6572 6174 696f 6e20 696e   or operation in
-0000b770: 7374 6561 640a 2020 2020 2020 2020 2020  stead.          
-0000b780: 2020 7572 6c20 3d20 686f 7374 202b 2072    url = host + r
-0000b790: 6573 6f75 7263 655f 7061 7468 0a0a 2020  esource_path..  
-0000b7a0: 2020 2020 2020 7265 7175 6573 745f 6166        request_af
-0000b7b0: 7465 725f 686f 6f6b 280a 2020 2020 2020  ter_hook(.      
-0000b7c0: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
-0000b7d0: 6174 683d 7265 736f 7572 6365 5f70 6174  ath=resource_pat
-0000b7e0: 682c 0a20 2020 2020 2020 2020 2020 206d  h,.            m
-0000b7f0: 6574 686f 643d 6d65 7468 6f64 2c0a 2020  ethod=method,.  
-0000b800: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000b810: 7572 6174 696f 6e3d 7365 6c66 2e63 6f6e  uration=self.con
-0000b820: 6669 6775 7261 7469 6f6e 2c0a 2020 2020  figuration,.    
-0000b830: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
-0000b840: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
-0000b850: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
-0000b860: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
-0000b870: 6574 7469 6e67 733d 6175 7468 5f73 6574  ettings=auth_set
-0000b880: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-0000b890: 2020 2068 6561 6465 7273 3d75 7365 645f     headers=used_
-0000b8a0: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
-0000b8b0: 2029 0a0a 2020 2020 2020 2020 2320 7065   )..        # pe
-0000b8c0: 7266 6f72 6d20 7265 7175 6573 7420 616e  rform request an
-0000b8d0: 6420 7265 7475 726e 2072 6573 706f 6e73  d return respons
-0000b8e0: 650a 2020 2020 2020 2020 7265 7370 6f6e  e.        respon
-0000b8f0: 7365 203d 2061 7761 6974 2073 656c 662e  se = await self.
-0000b900: 6173 796e 635f 7265 7175 6573 7428 0a20  async_request(. 
-0000b910: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-0000b920: 642c 0a20 2020 2020 2020 2020 2020 2075  d,.            u
-0000b930: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-0000b940: 6865 6164 6572 733d 7573 6564 5f68 6561  headers=used_hea
-0000b950: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
-0000b960: 2020 6669 656c 6473 3d66 6965 6c64 732c    fields=fields,
-0000b970: 0a20 2020 2020 2020 2020 2020 2062 6f64  .            bod
-0000b980: 793d 7365 7269 616c 697a 6564 5f62 6f64  y=serialized_bod
-0000b990: 792c 0a20 2020 2020 2020 2020 2020 2073  y,.            s
-0000b9a0: 7472 6561 6d3d 7374 7265 616d 2c0a 2020  tream=stream,.  
-0000b9b0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-0000b9c0: 743d 7469 6d65 6f75 742c 0a20 2020 2020  t=timeout,.     
-0000b9d0: 2020 2029 0a0a 0a20 2020 2020 2020 2072     )...        r
-0000b9e0: 6574 7572 6e20 7265 7370 6f6e 7365 0a0a  eturn response..
-0000b9f0: 2020 2020 6465 6620 5f5f 6361 6c6c 5f61      def __call_a
-0000ba00: 7069 280a 2020 2020 2020 2020 7365 6c66  pi(.        self
-0000ba10: 2c0a 2020 2020 2020 2020 7265 736f 7572  ,.        resour
-0000ba20: 6365 5f70 6174 683a 2073 7472 2c0a 2020  ce_path: str,.  
-0000ba30: 2020 2020 2020 6d65 7468 6f64 3a20 7374        method: st
-0000ba40: 722c 0a20 2020 2020 2020 2068 6561 6465  r,.        heade
-0000ba50: 7273 3a20 7479 7069 6e67 2e4f 7074 696f  rs: typing.Optio
-0000ba60: 6e61 6c5b 4854 5450 4865 6164 6572 4469  nal[HTTPHeaderDi
-0000ba70: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-0000ba80: 2020 2020 7365 7269 616c 697a 6564 5f62      serialized_b
-0000ba90: 6f64 793a 2074 7970 696e 672e 4f70 7469  ody: typing.Opti
-0000baa0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
-0000bab0: 6e5b 7374 722c 2062 7974 6573 5d5d 203d  n[str, bytes]] =
-0000bac0: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-0000bad0: 6f64 793a 2074 7970 696e 672e 416e 7920  ody: typing.Any 
-0000bae0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000baf0: 6669 656c 6473 3a20 7479 7069 6e67 2e4f  fields: typing.O
-0000bb00: 7074 696f 6e61 6c5b 7479 7069 6e67 2e54  ptional[typing.T
-0000bb10: 7570 6c65 5b74 7970 696e 672e 5475 706c  uple[typing.Tupl
-0000bb20: 655b 7374 722c 2073 7472 5d2c 202e 2e2e  e[str, str], ...
-0000bb30: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-0000bb40: 2020 2061 7574 685f 7365 7474 696e 6773     auth_settings
-0000bb50: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000bb60: 6c5b 7479 7069 6e67 2e4c 6973 745b 7374  l[typing.List[st
-0000bb70: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
-0000bb80: 2020 2020 7374 7265 616d 3a20 626f 6f6c      stream: bool
-0000bb90: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000bba0: 2020 7469 6d65 6f75 743a 2074 7970 696e    timeout: typin
-0000bbb0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0000bbc0: 672e 556e 696f 6e5b 696e 742c 2074 7970  g.Union[int, typ
-0000bbd0: 696e 672e 5475 706c 655d 5d20 3d20 4e6f  ing.Tuple]] = No
-0000bbe0: 6e65 2c0a 2020 2020 2020 2020 686f 7374  ne,.        host
-0000bbf0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000bc00: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000bc10: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-0000bc20: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-0000bc30: 3a20 5072 6566 6978 5365 7061 7261 746f  : PrefixSeparato
-0000bc40: 7249 7465 7261 746f 7220 3d20 4e6f 6e65  rIterator = None
-0000bc50: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-0000bc60: 6e73 6557 7261 7070 6572 3a0a 0a20 2020  nseWrapper:..   
-0000bc70: 2020 2020 2072 6571 7565 7374 5f62 6566       request_bef
-0000bc80: 6f72 655f 686f 6f6b 280a 2020 2020 2020  ore_hook(.      
-0000bc90: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
-0000bca0: 6174 683d 7265 736f 7572 6365 5f70 6174  ath=resource_pat
-0000bcb0: 682c 0a20 2020 2020 2020 2020 2020 206d  h,.            m
-0000bcc0: 6574 686f 643d 6d65 7468 6f64 2c0a 2020  ethod=method,.  
-0000bcd0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000bce0: 7572 6174 696f 6e3d 7365 6c66 2e63 6f6e  uration=self.con
-0000bcf0: 6669 6775 7261 7469 6f6e 2c0a 2020 2020  figuration,.    
-0000bd00: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
-0000bd10: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
-0000bd20: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
-0000bd30: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
-0000bd40: 6574 7469 6e67 733d 6175 7468 5f73 6574  ettings=auth_set
-0000bd50: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-0000bd60: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
-0000bd70: 7273 2c0a 2020 2020 2020 2020 290a 0a20  rs,.        ).. 
-0000bd80: 2020 2020 2020 2023 2068 6561 6465 7220         # header 
-0000bd90: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-0000bda0: 2020 2075 7365 645f 6865 6164 6572 7320     used_headers 
-0000bdb0: 3d20 4854 5450 4865 6164 6572 4469 6374  = HTTPHeaderDict
-0000bdc0: 2873 656c 662e 6465 6661 756c 745f 6865  (self.default_he
-0000bdd0: 6164 6572 7329 0a20 2020 2020 2020 2069  aders).        i
-0000bde0: 6620 7365 6c66 2e63 6f6f 6b69 653a 0a20  f self.cookie:. 
-0000bdf0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0000be00: 7273 5b27 436f 6f6b 6965 275d 203d 2073  rs['Cookie'] = s
-0000be10: 656c 662e 636f 6f6b 6965 0a0a 2020 2020  elf.cookie..    
-0000be20: 2020 2020 2320 6175 7468 2073 6574 7469      # auth setti
-0000be30: 6e67 0a20 2020 2020 2020 2072 6573 6f75  ng.        resou
-0000be40: 7263 655f 7061 7468 203d 2073 656c 662e  rce_path = self.
-0000be50: 7570 6461 7465 5f70 6172 616d 735f 666f  update_params_fo
-0000be60: 725f 6175 7468 280a 2020 2020 2020 2020  r_auth(.        
-0000be70: 2020 2020 7573 6564 5f68 6561 6465 7273      used_headers
-0000be80: 2c0a 2020 2020 2020 2020 2020 2020 6175  ,.            au
-0000be90: 7468 5f73 6574 7469 6e67 732c 0a20 2020  th_settings,.   
-0000bea0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-0000beb0: 655f 7061 7468 2c0a 2020 2020 2020 2020  e_path,.        
-0000bec0: 2020 2020 6d65 7468 6f64 2c0a 2020 2020      method,.    
-0000bed0: 2020 2020 2020 2020 626f 6479 2c0a 2020          body,.  
-0000bee0: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-0000bef0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-0000bf00: 746f 720a 2020 2020 2020 2020 290a 0a20  tor.        ).. 
-0000bf10: 2020 2020 2020 2023 206d 7573 7420 6861         # must ha
-0000bf20: 7070 656e 2061 6674 6572 2063 6f6f 6b69  ppen after cooki
-0000bf30: 6520 7365 7474 696e 6720 616e 6420 6175  e setting and au
-0000bf40: 7468 2073 6574 7469 6e67 2069 6e20 6361  th setting in ca
-0000bf50: 7365 2075 7365 7220 6973 206f 7665 7272  se user is overr
-0000bf60: 6964 696e 6720 7468 6f73 650a 2020 2020  iding those.    
-0000bf70: 2020 2020 6966 2068 6561 6465 7273 3a0a      if headers:.
-0000bf80: 2020 2020 2020 2020 2020 2020 7573 6564              used
-0000bf90: 5f68 6561 6465 7273 2e75 7064 6174 6528  _headers.update(
-0000bfa0: 6865 6164 6572 7329 0a0a 2020 2020 2020  headers)..      
-0000bfb0: 2020 2320 7265 7175 6573 7420 7572 6c0a    # request url.
-0000bfc0: 2020 2020 2020 2020 6966 2068 6f73 7420          if host 
-0000bfd0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000bfe0: 2020 2020 2075 726c 203d 2073 656c 662e       url = self.
-0000bff0: 636f 6e66 6967 7572 6174 696f 6e2e 686f  configuration.ho
-0000c000: 7374 202b 2072 6573 6f75 7263 655f 7061  st + resource_pa
-0000c010: 7468 0a20 2020 2020 2020 2065 6c73 653a  th.        else:
-0000c020: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-0000c030: 7365 2073 6572 7665 722f 686f 7374 2064  se server/host d
-0000c040: 6566 696e 6564 2069 6e20 7061 7468 206f  efined in path o
-0000c050: 7220 6f70 6572 6174 696f 6e20 696e 7374  r operation inst
-0000c060: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
-0000c070: 7572 6c20 3d20 686f 7374 202b 2072 6573  url = host + res
-0000c080: 6f75 7263 655f 7061 7468 0a0a 2020 2020  ource_path..    
-0000c090: 2020 2020 7265 7175 6573 745f 6166 7465      request_afte
-0000c0a0: 725f 686f 6f6b 280a 2020 2020 2020 2020  r_hook(.        
-0000c0b0: 2020 2020 7265 736f 7572 6365 5f70 6174      resource_pat
-0000c0c0: 683d 7265 736f 7572 6365 5f70 6174 682c  h=resource_path,
-0000c0d0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0000c0e0: 686f 643d 6d65 7468 6f64 2c0a 2020 2020  hod=method,.    
-0000c0f0: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-0000c100: 6174 696f 6e3d 7365 6c66 2e63 6f6e 6669  ation=self.confi
-0000c110: 6775 7261 7469 6f6e 2c0a 2020 2020 2020  guration,.      
-0000c120: 2020 2020 2020 626f 6479 3d62 6f64 792c        body=body,
-0000c130: 0a20 2020 2020 2020 2020 2020 2066 6965  .            fie
-0000c140: 6c64 733d 6669 656c 6473 2c0a 2020 2020  lds=fields,.    
-0000c150: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
-0000c160: 7469 6e67 733d 6175 7468 5f73 6574 7469  tings=auth_setti
-0000c170: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
-0000c180: 2068 6561 6465 7273 3d75 7365 645f 6865   headers=used_he
-0000c190: 6164 6572 732c 0a20 2020 2020 2020 2029  aders,.        )
-0000c1a0: 0a0a 2020 2020 2020 2020 2320 7065 7266  ..        # perf
-0000c1b0: 6f72 6d20 7265 7175 6573 7420 616e 6420  orm request and 
-0000c1c0: 7265 7475 726e 2072 6573 706f 6e73 650a  return response.
-0000c1d0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000c1e0: 203d 2073 656c 662e 7265 7175 6573 7428   = self.request(
-0000c1f0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-0000c200: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
-0000c210: 2075 726c 2c0a 2020 2020 2020 2020 2020   url,.          
-0000c220: 2020 6865 6164 6572 733d 7573 6564 5f68    headers=used_h
-0000c230: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
-0000c240: 2020 2020 6669 656c 6473 3d66 6965 6c64      fields=field
-0000c250: 732c 0a20 2020 2020 2020 2020 2020 2062  s,.            b
-0000c260: 6f64 793d 7365 7269 616c 697a 6564 5f62  ody=serialized_b
-0000c270: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
-0000c280: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
-0000c290: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000c2a0: 6f75 743d 7469 6d65 6f75 742c 0a20 2020  out=timeout,.   
-0000c2b0: 2020 2020 2029 0a0a 0a20 2020 2020 2020       )...       
-0000c2c0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-0000c2d0: 0a0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-0000c2e0: 6173 796e 635f 6361 6c6c 5f61 7069 280a  async_call_api(.
-0000c2f0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000c300: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
-0000c310: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
-0000c320: 2020 6d65 7468 6f64 3a20 7374 722c 0a20    method: str,. 
-0000c330: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-0000c340: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0000c350: 4854 5450 4865 6164 6572 4469 6374 5d20  HTTPHeaderDict] 
-0000c360: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000c370: 7365 7269 616c 697a 6564 5f62 6f64 793a  serialized_body:
-0000c380: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0000c390: 5b74 7970 696e 672e 556e 696f 6e5b 7374  [typing.Union[st
-0000c3a0: 722c 2062 7974 6573 5d5d 203d 204e 6f6e  r, bytes]] = Non
-0000c3b0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-0000c3c0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
-0000c3d0: 6e65 2c0a 2020 2020 2020 2020 6669 656c  ne,.        fiel
-0000c3e0: 6473 3a20 7479 7069 6e67 2e4f 7074 696f  ds: typing.Optio
-0000c3f0: 6e61 6c5b 7479 7069 6e67 2e54 7570 6c65  nal[typing.Tuple
-0000c400: 5b74 7970 696e 672e 5475 706c 655b 7374  [typing.Tuple[st
-0000c410: 722c 2073 7472 5d2c 202e 2e2e 5d5d 203d  r, str], ...]] =
-0000c420: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
-0000c430: 7574 685f 7365 7474 696e 6773 3a20 7479  uth_settings: ty
-0000c440: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0000c450: 7069 6e67 2e4c 6973 745b 7374 725d 5d20  ping.List[str]] 
-0000c460: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000c470: 7374 7265 616d 3a20 626f 6f6c 203d 2046  stream: bool = F
-0000c480: 616c 7365 2c0a 2020 2020 2020 2020 7469  alse,.        ti
-0000c490: 6d65 6f75 743a 2074 7970 696e 672e 4f70  meout: typing.Op
-0000c4a0: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
-0000c4b0: 696f 6e5b 696e 742c 2074 7970 696e 672e  ion[int, typing.
-0000c4c0: 5475 706c 655d 5d20 3d20 4e6f 6e65 2c0a  Tuple]] = None,.
-0000c4d0: 2020 2020 2020 2020 686f 7374 3a20 7479          host: ty
-0000c4e0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-0000c4f0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-0000c500: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-0000c510: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
-0000c520: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
-0000c530: 7261 746f 7220 3d20 4e6f 6e65 2c0a 2020  rator = None,.  
-0000c540: 2020 2920 2d3e 2041 7379 6e63 5265 7370    ) -> AsyncResp
-0000c550: 6f6e 7365 5772 6170 7065 723a 0a20 2020  onseWrapper:.   
-0000c560: 2020 2020 2022 2222 4d61 6b65 7320 7468       """Makes th
-0000c570: 6520 4854 5450 2072 6571 7565 7374 2028  e HTTP request (
-0000c580: 7379 6e63 6872 6f6e 6f75 7329 2061 6e64  synchronous) and
-0000c590: 2072 6574 7572 6e73 2064 6573 6572 6961   returns deseria
-0000c5a0: 6c69 7a65 6420 6461 7461 2e0a 0a20 2020  lized data...   
-0000c5b0: 2020 2020 203a 7061 7261 6d20 7265 736f       :param reso
-0000c5c0: 7572 6365 5f70 6174 683a 2050 6174 6820  urce_path: Path 
-0000c5d0: 746f 206d 6574 686f 6420 656e 6470 6f69  to method endpoi
-0000c5e0: 6e74 2e0a 2020 2020 2020 2020 3a70 6172  nt..        :par
-0000c5f0: 616d 206d 6574 686f 643a 204d 6574 686f  am method: Metho
-0000c600: 6420 746f 2063 616c 6c2e 0a20 2020 2020  d to call..     
-0000c610: 2020 203a 7061 7261 6d20 6865 6164 6572     :param header
-0000c620: 733a 2048 6561 6465 7220 7061 7261 6d65  s: Header parame
-0000c630: 7465 7273 2074 6f20 6265 0a20 2020 2020  ters to be.     
-0000c640: 2020 2020 2020 2070 6c61 6365 6420 696e         placed in
-0000c650: 2074 6865 2072 6571 7565 7374 2068 6561   the request hea
-0000c660: 6465 722e 0a20 2020 2020 2020 203a 7061  der..        :pa
-0000c670: 7261 6d20 626f 6479 3a20 5265 7175 6573  ram body: Reques
-0000c680: 7420 626f 6479 2e0a 2020 2020 2020 2020  t body..        
-0000c690: 3a70 6172 616d 2066 6965 6c64 733a 2052  :param fields: R
-0000c6a0: 6571 7565 7374 2070 6f73 7420 666f 726d  equest post form
-0000c6b0: 2070 6172 616d 6574 6572 732c 0a20 2020   parameters,.   
-0000c6c0: 2020 2020 2020 2020 2066 6f72 2060 6170           for `ap
-0000c6d0: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
-0000c6e0: 666f 726d 2d75 726c 656e 636f 6465 6460  form-urlencoded`
-0000c6f0: 2c20 606d 756c 7469 7061 7274 2f66 6f72  , `multipart/for
-0000c700: 6d2d 6461 7461 602e 0a20 2020 2020 2020  m-data`..       
-0000c710: 203a 7061 7261 6d20 6175 7468 5f73 6574   :param auth_set
-0000c720: 7469 6e67 733a 2041 7574 6820 5365 7474  tings: Auth Sett
-0000c730: 696e 6773 206e 616d 6573 2066 6f72 2074  ings names for t
-0000c740: 6865 2072 6571 7565 7374 2e0a 2020 2020  he request..    
-0000c750: 2020 2020 3a70 6172 616d 2073 7472 6561      :param strea
-0000c760: 6d3a 2069 6620 5472 7565 2c20 7468 6520  m: if True, the 
-0000c770: 7572 6c6c 6962 332e 4854 5450 5265 7370  urllib3.HTTPResp
-0000c780: 6f6e 7365 206f 626a 6563 7420 7769 6c6c  onse object will
-0000c790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ace0: 6134 2f70 7974 686f 6e27 0a0a 2020 2020  a4/python'..    
+0000acf0: 6465 6620 5f5f 656e 7465 725f 5f28 7365  def __enter__(se
+0000ad00: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0000ad10: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
+0000ad20: 6620 5f5f 6578 6974 5f5f 2873 656c 662c  f __exit__(self,
+0000ad30: 2065 7863 5f74 7970 652c 2065 7863 5f76   exc_type, exc_v
+0000ad40: 616c 7565 2c20 7472 6163 6562 6163 6b29  alue, traceback)
+0000ad50: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
+0000ad60: 6c6f 7365 2829 0a0a 2020 2020 6465 6620  lose()..    def 
+0000ad70: 636c 6f73 6528 7365 6c66 293a 0a20 2020  close(self):.   
+0000ad80: 2020 2020 2069 6620 7365 6c66 2e5f 706f       if self._po
+0000ad90: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+0000ada0: 7365 6c66 2e5f 706f 6f6c 2e63 6c6f 7365  self._pool.close
+0000adb0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+0000adc0: 656c 662e 5f70 6f6f 6c2e 6a6f 696e 2829  elf._pool.join()
+0000add0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ade0: 662e 5f70 6f6f 6c20 3d20 4e6f 6e65 0a20  f._pool = None. 
+0000adf0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+0000ae00: 7361 7474 7228 6174 6578 6974 2c20 2775  sattr(atexit, 'u
+0000ae10: 6e72 6567 6973 7465 7227 293a 0a20 2020  nregister'):.   
+0000ae20: 2020 2020 2020 2020 2020 2020 2061 7465               ate
+0000ae30: 7869 742e 756e 7265 6769 7374 6572 2873  xit.unregister(s
+0000ae40: 656c 662e 636c 6f73 6529 0a0a 2020 2020  elf.close)..    
+0000ae50: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000ae60: 6620 706f 6f6c 2873 656c 6629 3a0a 2020  f pool(self):.  
+0000ae70: 2020 2020 2020 2222 2243 7265 6174 6520        """Create 
+0000ae80: 7468 7265 6164 2070 6f6f 6c20 6f6e 2066  thread pool on f
+0000ae90: 6972 7374 2072 6571 7565 7374 0a20 2020  irst request.   
+0000aea0: 2020 2020 2020 6176 6f69 6473 2069 6e73        avoids ins
+0000aeb0: 7461 6e74 6961 7469 6e67 2075 6e75 7365  tantiating unuse
+0000aec0: 6420 7468 7265 6164 706f 6f6c 2066 6f72  d threadpool for
+0000aed0: 2062 6c6f 636b 696e 6720 636c 6965 6e74   blocking client
+0000aee0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0000aef0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000af00: 706f 6f6c 2069 7320 4e6f 6e65 3a0a 2020  pool is None:.  
+0000af10: 2020 2020 2020 2020 2020 6174 6578 6974            atexit
+0000af20: 2e72 6567 6973 7465 7228 7365 6c66 2e63  .register(self.c
+0000af30: 6c6f 7365 290a 2020 2020 2020 2020 2020  lose).          
+0000af40: 2020 7365 6c66 2e5f 706f 6f6c 203d 2054    self._pool = T
+0000af50: 6872 6561 6450 6f6f 6c28 7365 6c66 2e70  hreadPool(self.p
+0000af60: 6f6f 6c5f 7468 7265 6164 7329 0a20 2020  ool_threads).   
+0000af70: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000af80: 2e5f 706f 6f6c 0a0a 2020 2020 4070 726f  ._pool..    @pro
+0000af90: 7065 7274 790a 2020 2020 6465 6620 7573  perty.    def us
+0000afa0: 6572 5f61 6765 6e74 2873 656c 6629 3a0a  er_agent(self):.
+0000afb0: 2020 2020 2020 2020 2222 2255 7365 7220          """User 
+0000afc0: 6167 656e 7420 666f 7220 7468 6973 2041  agent for this A
+0000afd0: 5049 2063 6c69 656e 7422 2222 0a20 2020  PI client""".   
+0000afe0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000aff0: 2e64 6566 6175 6c74 5f68 6561 6465 7273  .default_headers
+0000b000: 5b27 5573 6572 2d41 6765 6e74 275d 0a0a  ['User-Agent']..
+0000b010: 2020 2020 4075 7365 725f 6167 656e 742e      @user_agent.
+0000b020: 7365 7474 6572 0a20 2020 2064 6566 2075  setter.    def u
+0000b030: 7365 725f 6167 656e 7428 7365 6c66 2c20  ser_agent(self, 
+0000b040: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0000b050: 7365 6c66 2e64 6566 6175 6c74 5f68 6561  self.default_hea
+0000b060: 6465 7273 5b27 5573 6572 2d41 6765 6e74  ders['User-Agent
+0000b070: 275d 203d 2076 616c 7565 0a0a 2020 2020  '] = value..    
+0000b080: 6465 6620 7365 745f 6465 6661 756c 745f  def set_default_
+0000b090: 6865 6164 6572 2873 656c 662c 2068 6561  header(self, hea
+0000b0a0: 6465 725f 6e61 6d65 2c20 6865 6164 6572  der_name, header
+0000b0b0: 5f76 616c 7565 293a 0a20 2020 2020 2020  _value):.       
+0000b0c0: 2073 656c 662e 6465 6661 756c 745f 6865   self.default_he
+0000b0d0: 6164 6572 735b 6865 6164 6572 5f6e 616d  aders[header_nam
+0000b0e0: 655d 203d 2068 6561 6465 725f 7661 6c75  e] = header_valu
+0000b0f0: 650a 0a20 2020 2061 7379 6e63 2064 6566  e..    async def
+0000b100: 205f 5f61 7379 6e63 5f63 616c 6c5f 6170   __async_call_ap
+0000b110: 6928 0a20 2020 2020 2020 2073 656c 662c  i(.        self,
+0000b120: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+0000b130: 655f 7061 7468 3a20 7374 722c 0a20 2020  e_path: str,.   
+0000b140: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+0000b150: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0000b160: 733a 2074 7970 696e 672e 4f70 7469 6f6e  s: typing.Option
+0000b170: 616c 5b48 5454 5048 6561 6465 7244 6963  al[HTTPHeaderDic
+0000b180: 745d 203d 204e 6f6e 652c 0a20 2020 2020  t] = None,.     
+0000b190: 2020 2073 6572 6961 6c69 7a65 645f 626f     serialized_bo
+0000b1a0: 6479 3a20 7479 7069 6e67 2e4f 7074 696f  dy: typing.Optio
+0000b1b0: 6e61 6c5b 7479 7069 6e67 2e55 6e69 6f6e  nal[typing.Union
+0000b1c0: 5b73 7472 2c20 6279 7465 735d 5d20 3d20  [str, bytes]] = 
+0000b1d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+0000b1e0: 6479 3a20 7479 7069 6e67 2e41 6e79 203d  dy: typing.Any =
+0000b1f0: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
+0000b200: 6965 6c64 733a 2074 7970 696e 672e 4f70  ields: typing.Op
+0000b210: 7469 6f6e 616c 5b74 7970 696e 672e 5475  tional[typing.Tu
+0000b220: 706c 655b 7479 7069 6e67 2e54 7570 6c65  ple[typing.Tuple
+0000b230: 5b73 7472 2c20 7374 725d 2c20 2e2e 2e5d  [str, str], ...]
+0000b240: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000b250: 2020 6175 7468 5f73 6574 7469 6e67 733a    auth_settings:
+0000b260: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000b270: 5b74 7970 696e 672e 4c69 7374 5b73 7472  [typing.List[str
+0000b280: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000b290: 2020 2073 7472 6561 6d3a 2062 6f6f 6c20     stream: bool 
+0000b2a0: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+0000b2b0: 2074 696d 656f 7574 3a20 7479 7069 6e67   timeout: typing
+0000b2c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000b2d0: 2e55 6e69 6f6e 5b69 6e74 2c20 7479 7069  .Union[int, typi
+0000b2e0: 6e67 2e54 7570 6c65 5d5d 203d 204e 6f6e  ng.Tuple]] = Non
+0000b2f0: 652c 0a20 2020 2020 2020 2068 6f73 743a  e,.        host:
+0000b300: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000b310: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+0000b320: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+0000b330: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
+0000b340: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+0000b350: 4974 6572 6174 6f72 203d 204e 6f6e 652c  Iterator = None,
+0000b360: 0a20 2020 2029 202d 3e20 4173 796e 6352  .    ) -> AsyncR
+0000b370: 6573 706f 6e73 6557 7261 7070 6572 3a0a  esponseWrapper:.
+0000b380: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0000b390: 5f62 6566 6f72 655f 686f 6f6b 280a 2020  _before_hook(.  
+0000b3a0: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0000b3b0: 6365 5f70 6174 683d 7265 736f 7572 6365  ce_path=resource
+0000b3c0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0000b3d0: 2020 206d 6574 686f 643d 6d65 7468 6f64     method=method
+0000b3e0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+0000b3f0: 6e66 6967 7572 6174 696f 6e3d 7365 6c66  nfiguration=self
+0000b400: 2e63 6f6e 6669 6775 7261 7469 6f6e 2c0a  .configuration,.
+0000b410: 2020 2020 2020 2020 2020 2020 626f 6479              body
+0000b420: 3d62 6f64 792c 0a20 2020 2020 2020 2020  =body,.         
+0000b430: 2020 2066 6965 6c64 733d 6669 656c 6473     fields=fields
+0000b440: 2c0a 2020 2020 2020 2020 2020 2020 6175  ,.            au
+0000b450: 7468 5f73 6574 7469 6e67 733d 6175 7468  th_settings=auth
+0000b460: 5f73 6574 7469 6e67 732c 0a20 2020 2020  _settings,.     
+0000b470: 2020 2020 2020 2068 6561 6465 7273 3d68         headers=h
+0000b480: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
+0000b490: 290a 0a20 2020 2020 2020 2023 2068 6561  )..        # hea
+0000b4a0: 6465 7220 7061 7261 6d65 7465 7273 0a20  der parameters. 
+0000b4b0: 2020 2020 2020 2075 7365 645f 6865 6164         used_head
+0000b4c0: 6572 7320 3d20 4854 5450 4865 6164 6572  ers = HTTPHeader
+0000b4d0: 4469 6374 2873 656c 662e 6465 6661 756c  Dict(self.defaul
+0000b4e0: 745f 6865 6164 6572 7329 0a20 2020 2020  t_headers).     
+0000b4f0: 2020 2069 6620 7365 6c66 2e63 6f6f 6b69     if self.cooki
+0000b500: 653a 0a20 2020 2020 2020 2020 2020 2068  e:.            h
+0000b510: 6561 6465 7273 5b27 436f 6f6b 6965 275d  eaders['Cookie']
+0000b520: 203d 2073 656c 662e 636f 6f6b 6965 0a0a   = self.cookie..
+0000b530: 2020 2020 2020 2020 2320 6175 7468 2073          # auth s
+0000b540: 6574 7469 6e67 0a20 2020 2020 2020 2072  etting.        r
+0000b550: 6573 6f75 7263 655f 7061 7468 203d 2073  esource_path = s
+0000b560: 656c 662e 7570 6461 7465 5f70 6172 616d  elf.update_param
+0000b570: 735f 666f 725f 6175 7468 280a 2020 2020  s_for_auth(.    
+0000b580: 2020 2020 2020 2020 7573 6564 5f68 6561          used_hea
+0000b590: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
+0000b5a0: 2020 6175 7468 5f73 6574 7469 6e67 732c    auth_settings,
+0000b5b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000b5c0: 6f75 7263 655f 7061 7468 2c0a 2020 2020  ource_path,.    
+0000b5d0: 2020 2020 2020 2020 6d65 7468 6f64 2c0a          method,.
+0000b5e0: 2020 2020 2020 2020 2020 2020 626f 6479              body
+0000b5f0: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
+0000b600: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+0000b610: 7465 7261 746f 720a 2020 2020 2020 2020  terator.        
+0000b620: 290a 0a20 2020 2020 2020 2023 206d 7573  )..        # mus
+0000b630: 7420 6861 7070 656e 2061 6674 6572 2063  t happen after c
+0000b640: 6f6f 6b69 6520 7365 7474 696e 6720 616e  ookie setting an
+0000b650: 6420 6175 7468 2073 6574 7469 6e67 2069  d auth setting i
+0000b660: 6e20 6361 7365 2075 7365 7220 6973 206f  n case user is o
+0000b670: 7665 7272 6964 696e 6720 7468 6f73 650a  verriding those.
+0000b680: 2020 2020 2020 2020 6966 2068 6561 6465          if heade
+0000b690: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+0000b6a0: 7573 6564 5f68 6561 6465 7273 2e75 7064  used_headers.upd
+0000b6b0: 6174 6528 6865 6164 6572 7329 0a0a 2020  ate(headers)..  
+0000b6c0: 2020 2020 2020 2320 7265 7175 6573 7420        # request 
+0000b6d0: 7572 6c0a 2020 2020 2020 2020 6966 2068  url.        if h
+0000b6e0: 6f73 7420 6973 204e 6f6e 653a 0a20 2020  ost is None:.   
+0000b6f0: 2020 2020 2020 2020 2075 726c 203d 2073           url = s
+0000b700: 656c 662e 636f 6e66 6967 7572 6174 696f  elf.configuratio
+0000b710: 6e2e 686f 7374 202b 2072 6573 6f75 7263  n.host + resourc
+0000b720: 655f 7061 7468 0a20 2020 2020 2020 2065  e_path.        e
+0000b730: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000b740: 2023 2075 7365 2073 6572 7665 722f 686f   # use server/ho
+0000b750: 7374 2064 6566 696e 6564 2069 6e20 7061  st defined in pa
+0000b760: 7468 206f 7220 6f70 6572 6174 696f 6e20  th or operation 
+0000b770: 696e 7374 6561 640a 2020 2020 2020 2020  instead.        
+0000b780: 2020 2020 7572 6c20 3d20 686f 7374 202b      url = host +
+0000b790: 2072 6573 6f75 7263 655f 7061 7468 0a0a   resource_path..
+0000b7a0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+0000b7b0: 6166 7465 725f 686f 6f6b 280a 2020 2020  after_hook(.    
+0000b7c0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000b7d0: 5f70 6174 683d 7265 736f 7572 6365 5f70  _path=resource_p
+0000b7e0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000b7f0: 206d 6574 686f 643d 6d65 7468 6f64 2c0a   method=method,.
+0000b800: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000b810: 6967 7572 6174 696f 6e3d 7365 6c66 2e63  iguration=self.c
+0000b820: 6f6e 6669 6775 7261 7469 6f6e 2c0a 2020  onfiguration,.  
+0000b830: 2020 2020 2020 2020 2020 626f 6479 3d62            body=b
+0000b840: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
+0000b850: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
+0000b860: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+0000b870: 5f73 6574 7469 6e67 733d 6175 7468 5f73  _settings=auth_s
+0000b880: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
+0000b890: 2020 2020 2068 6561 6465 7273 3d75 7365       headers=use
+0000b8a0: 645f 6865 6164 6572 732c 0a20 2020 2020  d_headers,.     
+0000b8b0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+0000b8c0: 7065 7266 6f72 6d20 7265 7175 6573 7420  perform request 
+0000b8d0: 616e 6420 7265 7475 726e 2072 6573 706f  and return respo
+0000b8e0: 6e73 650a 2020 2020 2020 2020 7265 7370  nse.        resp
+0000b8f0: 6f6e 7365 203d 2061 7761 6974 2073 656c  onse = await sel
+0000b900: 662e 6173 796e 635f 7265 7175 6573 7428  f.async_request(
+0000b910: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+0000b920: 686f 642c 0a20 2020 2020 2020 2020 2020  hod,.           
+0000b930: 2075 726c 2c0a 2020 2020 2020 2020 2020   url,.          
+0000b940: 2020 6865 6164 6572 733d 7573 6564 5f68    headers=used_h
+0000b950: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
+0000b960: 2020 2020 6669 656c 6473 3d66 6965 6c64      fields=field
+0000b970: 732c 0a20 2020 2020 2020 2020 2020 2062  s,.            b
+0000b980: 6f64 793d 7365 7269 616c 697a 6564 5f62  ody=serialized_b
+0000b990: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
+0000b9a0: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
+0000b9b0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000b9c0: 6f75 743d 7469 6d65 6f75 742c 0a20 2020  out=timeout,.   
+0000b9d0: 2020 2020 2029 0a0a 0a20 2020 2020 2020       )...       
+0000b9e0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+0000b9f0: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+0000ba00: 5f61 7069 280a 2020 2020 2020 2020 7365  _api(.        se
+0000ba10: 6c66 2c0a 2020 2020 2020 2020 7265 736f  lf,.        reso
+0000ba20: 7572 6365 5f70 6174 683a 2073 7472 2c0a  urce_path: str,.
+0000ba30: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+0000ba40: 7374 722c 0a20 2020 2020 2020 2068 6561  str,.        hea
+0000ba50: 6465 7273 3a20 7479 7069 6e67 2e4f 7074  ders: typing.Opt
+0000ba60: 696f 6e61 6c5b 4854 5450 4865 6164 6572  ional[HTTPHeader
+0000ba70: 4469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  Dict] = None,.  
+0000ba80: 2020 2020 2020 7365 7269 616c 697a 6564        serialized
+0000ba90: 5f62 6f64 793a 2074 7970 696e 672e 4f70  _body: typing.Op
+0000baa0: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0000bab0: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+0000bac0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000bad0: 2062 6f64 793a 2074 7970 696e 672e 416e   body: typing.An
+0000bae0: 7920 3d20 4e6f 6e65 2c0a 2020 2020 2020  y = None,.      
+0000baf0: 2020 6669 656c 6473 3a20 7479 7069 6e67    fields: typing
+0000bb00: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000bb10: 2e54 7570 6c65 5b74 7970 696e 672e 5475  .Tuple[typing.Tu
+0000bb20: 706c 655b 7374 722c 2073 7472 5d2c 202e  ple[str, str], .
+0000bb30: 2e2e 5d5d 203d 204e 6f6e 652c 0a20 2020  ..]] = None,.   
+0000bb40: 2020 2020 2061 7574 685f 7365 7474 696e       auth_settin
+0000bb50: 6773 3a20 7479 7069 6e67 2e4f 7074 696f  gs: typing.Optio
+0000bb60: 6e61 6c5b 7479 7069 6e67 2e4c 6973 745b  nal[typing.List[
+0000bb70: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0000bb80: 2020 2020 2020 7374 7265 616d 3a20 626f        stream: bo
+0000bb90: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0000bba0: 2020 2020 7469 6d65 6f75 743a 2074 7970      timeout: typ
+0000bbb0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0000bbc0: 696e 672e 556e 696f 6e5b 696e 742c 2074  ing.Union[int, t
+0000bbd0: 7970 696e 672e 5475 706c 655d 5d20 3d20  yping.Tuple]] = 
+0000bbe0: 4e6f 6e65 2c0a 2020 2020 2020 2020 686f  None,.        ho
+0000bbf0: 7374 3a20 7479 7069 6e67 2e4f 7074 696f  st: typing.Optio
+0000bc00: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000bc10: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
+0000bc20: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+0000bc30: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
+0000bc40: 746f 7249 7465 7261 746f 7220 3d20 4e6f  torIterator = No
+0000bc50: 6e65 2c0a 2020 2020 2920 2d3e 2052 6573  ne,.    ) -> Res
+0000bc60: 706f 6e73 6557 7261 7070 6572 3a0a 0a20  ponseWrapper:.. 
+0000bc70: 2020 2020 2020 2072 6571 7565 7374 5f62         request_b
+0000bc80: 6566 6f72 655f 686f 6f6b 280a 2020 2020  efore_hook(.    
+0000bc90: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000bca0: 5f70 6174 683d 7265 736f 7572 6365 5f70  _path=resource_p
+0000bcb0: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000bcc0: 206d 6574 686f 643d 6d65 7468 6f64 2c0a   method=method,.
+0000bcd0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000bce0: 6967 7572 6174 696f 6e3d 7365 6c66 2e63  iguration=self.c
+0000bcf0: 6f6e 6669 6775 7261 7469 6f6e 2c0a 2020  onfiguration,.  
+0000bd00: 2020 2020 2020 2020 2020 626f 6479 3d62            body=b
+0000bd10: 6f64 792c 0a20 2020 2020 2020 2020 2020  ody,.           
+0000bd20: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
+0000bd30: 2020 2020 2020 2020 2020 2020 6175 7468              auth
+0000bd40: 5f73 6574 7469 6e67 733d 6175 7468 5f73  _settings=auth_s
+0000bd50: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
+0000bd60: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
+0000bd70: 6465 7273 2c0a 2020 2020 2020 2020 290a  ders,.        ).
+0000bd80: 0a20 2020 2020 2020 2023 2068 6561 6465  .        # heade
+0000bd90: 7220 7061 7261 6d65 7465 7273 0a20 2020  r parameters.   
+0000bda0: 2020 2020 2075 7365 645f 6865 6164 6572       used_header
+0000bdb0: 7320 3d20 4854 5450 4865 6164 6572 4469  s = HTTPHeaderDi
+0000bdc0: 6374 2873 656c 662e 6465 6661 756c 745f  ct(self.default_
+0000bdd0: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
+0000bde0: 2069 6620 7365 6c66 2e63 6f6f 6b69 653a   if self.cookie:
+0000bdf0: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+0000be00: 6465 7273 5b27 436f 6f6b 6965 275d 203d  ders['Cookie'] =
+0000be10: 2073 656c 662e 636f 6f6b 6965 0a0a 2020   self.cookie..  
+0000be20: 2020 2020 2020 2320 6175 7468 2073 6574        # auth set
+0000be30: 7469 6e67 0a20 2020 2020 2020 2072 6573  ting.        res
+0000be40: 6f75 7263 655f 7061 7468 203d 2073 656c  ource_path = sel
+0000be50: 662e 7570 6461 7465 5f70 6172 616d 735f  f.update_params_
+0000be60: 666f 725f 6175 7468 280a 2020 2020 2020  for_auth(.      
+0000be70: 2020 2020 2020 7573 6564 5f68 6561 6465        used_heade
+0000be80: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000be90: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
+0000bea0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0000beb0: 7263 655f 7061 7468 2c0a 2020 2020 2020  rce_path,.      
+0000bec0: 2020 2020 2020 6d65 7468 6f64 2c0a 2020        method,.  
+0000bed0: 2020 2020 2020 2020 2020 626f 6479 2c0a            body,.
+0000bee0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+0000bef0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000bf00: 7261 746f 720a 2020 2020 2020 2020 290a  rator.        ).
+0000bf10: 0a20 2020 2020 2020 2023 206d 7573 7420  .        # must 
+0000bf20: 6861 7070 656e 2061 6674 6572 2063 6f6f  happen after coo
+0000bf30: 6b69 6520 7365 7474 696e 6720 616e 6420  kie setting and 
+0000bf40: 6175 7468 2073 6574 7469 6e67 2069 6e20  auth setting in 
+0000bf50: 6361 7365 2075 7365 7220 6973 206f 7665  case user is ove
+0000bf60: 7272 6964 696e 6720 7468 6f73 650a 2020  rriding those.  
+0000bf70: 2020 2020 2020 6966 2068 6561 6465 7273        if headers
+0000bf80: 3a0a 2020 2020 2020 2020 2020 2020 7573  :.            us
+0000bf90: 6564 5f68 6561 6465 7273 2e75 7064 6174  ed_headers.updat
+0000bfa0: 6528 6865 6164 6572 7329 0a0a 2020 2020  e(headers)..    
+0000bfb0: 2020 2020 2320 7265 7175 6573 7420 7572      # request ur
+0000bfc0: 6c0a 2020 2020 2020 2020 6966 2068 6f73  l.        if hos
+0000bfd0: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+0000bfe0: 2020 2020 2020 2075 726c 203d 2073 656c         url = sel
+0000bff0: 662e 636f 6e66 6967 7572 6174 696f 6e2e  f.configuration.
+0000c000: 686f 7374 202b 2072 6573 6f75 7263 655f  host + resource_
+0000c010: 7061 7468 0a20 2020 2020 2020 2065 6c73  path.        els
+0000c020: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+0000c030: 2075 7365 2073 6572 7665 722f 686f 7374   use server/host
+0000c040: 2064 6566 696e 6564 2069 6e20 7061 7468   defined in path
+0000c050: 206f 7220 6f70 6572 6174 696f 6e20 696e   or operation in
+0000c060: 7374 6561 640a 2020 2020 2020 2020 2020  stead.          
+0000c070: 2020 7572 6c20 3d20 686f 7374 202b 2072    url = host + r
+0000c080: 6573 6f75 7263 655f 7061 7468 0a0a 2020  esource_path..  
+0000c090: 2020 2020 2020 7265 7175 6573 745f 6166        request_af
+0000c0a0: 7465 725f 686f 6f6b 280a 2020 2020 2020  ter_hook(.      
+0000c0b0: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
+0000c0c0: 6174 683d 7265 736f 7572 6365 5f70 6174  ath=resource_pat
+0000c0d0: 682c 0a20 2020 2020 2020 2020 2020 206d  h,.            m
+0000c0e0: 6574 686f 643d 6d65 7468 6f64 2c0a 2020  ethod=method,.  
+0000c0f0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000c100: 7572 6174 696f 6e3d 7365 6c66 2e63 6f6e  uration=self.con
+0000c110: 6669 6775 7261 7469 6f6e 2c0a 2020 2020  figuration,.    
+0000c120: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
+0000c130: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
+0000c140: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
+0000c150: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
+0000c160: 6574 7469 6e67 733d 6175 7468 5f73 6574  ettings=auth_set
+0000c170: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
+0000c180: 2020 2068 6561 6465 7273 3d75 7365 645f     headers=used_
+0000c190: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
+0000c1a0: 2029 0a0a 2020 2020 2020 2020 2320 7065   )..        # pe
+0000c1b0: 7266 6f72 6d20 7265 7175 6573 7420 616e  rform request an
+0000c1c0: 6420 7265 7475 726e 2072 6573 706f 6e73  d return respons
+0000c1d0: 650a 2020 2020 2020 2020 7265 7370 6f6e  e.        respon
+0000c1e0: 7365 203d 2073 656c 662e 7265 7175 6573  se = self.reques
+0000c1f0: 7428 0a20 2020 2020 2020 2020 2020 206d  t(.            m
+0000c200: 6574 686f 642c 0a20 2020 2020 2020 2020  ethod,.         
+0000c210: 2020 2075 726c 2c0a 2020 2020 2020 2020     url,.        
+0000c220: 2020 2020 6865 6164 6572 733d 7573 6564      headers=used
+0000c230: 5f68 6561 6465 7273 2c0a 2020 2020 2020  _headers,.      
+0000c240: 2020 2020 2020 6669 656c 6473 3d66 6965        fields=fie
+0000c250: 6c64 732c 0a20 2020 2020 2020 2020 2020  lds,.           
+0000c260: 2062 6f64 793d 7365 7269 616c 697a 6564   body=serialized
+0000c270: 5f62 6f64 792c 0a20 2020 2020 2020 2020  _body,.         
+0000c280: 2020 2073 7472 6561 6d3d 7374 7265 616d     stream=stream
+0000c290: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
+0000c2a0: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
+0000c2b0: 2020 2020 2020 2029 0a0a 0a20 2020 2020         )...     
+0000c2c0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+0000c2d0: 7365 0a0a 2020 2020 6173 796e 6320 6465  se..    async de
+0000c2e0: 6620 6173 796e 635f 6361 6c6c 5f61 7069  f async_call_api
+0000c2f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000c300: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000c310: 5f70 6174 683a 2073 7472 2c0a 2020 2020  _path: str,.    
+0000c320: 2020 2020 6d65 7468 6f64 3a20 7374 722c      method: str,
+0000c330: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+0000c340: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000c350: 6c5b 4854 5450 4865 6164 6572 4469 6374  l[HTTPHeaderDict
+0000c360: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000c370: 2020 7365 7269 616c 697a 6564 5f62 6f64    serialized_bod
+0000c380: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+0000c390: 616c 5b74 7970 696e 672e 556e 696f 6e5b  al[typing.Union[
+0000c3a0: 7374 722c 2062 7974 6573 5d5d 203d 204e  str, bytes]] = N
+0000c3b0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0000c3c0: 793a 2074 7970 696e 672e 416e 7920 3d20  y: typing.Any = 
+0000c3d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6669  None,.        fi
+0000c3e0: 656c 6473 3a20 7479 7069 6e67 2e4f 7074  elds: typing.Opt
+0000c3f0: 696f 6e61 6c5b 7479 7069 6e67 2e54 7570  ional[typing.Tup
+0000c400: 6c65 5b74 7970 696e 672e 5475 706c 655b  le[typing.Tuple[
+0000c410: 7374 722c 2073 7472 5d2c 202e 2e2e 5d5d  str, str], ...]]
+0000c420: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000c430: 2061 7574 685f 7365 7474 696e 6773 3a20   auth_settings: 
+0000c440: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000c450: 7479 7069 6e67 2e4c 6973 745b 7374 725d  typing.List[str]
+0000c460: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000c470: 2020 7374 7265 616d 3a20 626f 6f6c 203d    stream: bool =
+0000c480: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000c490: 7469 6d65 6f75 743a 2074 7970 696e 672e  timeout: typing.
+0000c4a0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0000c4b0: 556e 696f 6e5b 696e 742c 2074 7970 696e  Union[int, typin
+0000c4c0: 672e 5475 706c 655d 5d20 3d20 4e6f 6e65  g.Tuple]] = None
+0000c4d0: 2c0a 2020 2020 2020 2020 686f 7374 3a20  ,.        host: 
+0000c4e0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000c4f0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0000c500: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
+0000c510: 7261 746f 725f 6974 6572 6174 6f72 3a20  rator_iterator: 
+0000c520: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+0000c530: 7465 7261 746f 7220 3d20 4e6f 6e65 2c0a  terator = None,.
+0000c540: 2020 2020 2920 2d3e 2041 7379 6e63 5265      ) -> AsyncRe
+0000c550: 7370 6f6e 7365 5772 6170 7065 723a 0a20  sponseWrapper:. 
+0000c560: 2020 2020 2020 2022 2222 4d61 6b65 7320         """Makes 
+0000c570: 7468 6520 4854 5450 2072 6571 7565 7374  the HTTP request
+0000c580: 2028 7379 6e63 6872 6f6e 6f75 7329 2061   (synchronous) a
+0000c590: 6e64 2072 6574 7572 6e73 2064 6573 6572  nd returns deser
+0000c5a0: 6961 6c69 7a65 6420 6461 7461 2e0a 0a20  ialized data... 
+0000c5b0: 2020 2020 2020 203a 7061 7261 6d20 7265         :param re
+0000c5c0: 736f 7572 6365 5f70 6174 683a 2050 6174  source_path: Pat
+0000c5d0: 6820 746f 206d 6574 686f 6420 656e 6470  h to method endp
+0000c5e0: 6f69 6e74 2e0a 2020 2020 2020 2020 3a70  oint..        :p
+0000c5f0: 6172 616d 206d 6574 686f 643a 204d 6574  aram method: Met
+0000c600: 686f 6420 746f 2063 616c 6c2e 0a20 2020  hod to call..   
+0000c610: 2020 2020 203a 7061 7261 6d20 6865 6164       :param head
+0000c620: 6572 733a 2048 6561 6465 7220 7061 7261  ers: Header para
+0000c630: 6d65 7465 7273 2074 6f20 6265 0a20 2020  meters to be.   
+0000c640: 2020 2020 2020 2020 2070 6c61 6365 6420           placed 
+0000c650: 696e 2074 6865 2072 6571 7565 7374 2068  in the request h
+0000c660: 6561 6465 722e 0a20 2020 2020 2020 203a  eader..        :
+0000c670: 7061 7261 6d20 626f 6479 3a20 5265 7175  param body: Requ
+0000c680: 6573 7420 626f 6479 2e0a 2020 2020 2020  est body..      
+0000c690: 2020 3a70 6172 616d 2066 6965 6c64 733a    :param fields:
+0000c6a0: 2052 6571 7565 7374 2070 6f73 7420 666f   Request post fo
+0000c6b0: 726d 2070 6172 616d 6574 6572 732c 0a20  rm parameters,. 
+0000c6c0: 2020 2020 2020 2020 2020 2066 6f72 2060             for `
+0000c6d0: 6170 706c 6963 6174 696f 6e2f 782d 7777  application/x-ww
+0000c6e0: 772d 666f 726d 2d75 726c 656e 636f 6465  w-form-urlencode
+0000c6f0: 6460 2c20 606d 756c 7469 7061 7274 2f66  d`, `multipart/f
+0000c700: 6f72 6d2d 6461 7461 602e 0a20 2020 2020  orm-data`..     
+0000c710: 2020 203a 7061 7261 6d20 6175 7468 5f73     :param auth_s
+0000c720: 6574 7469 6e67 733a 2041 7574 6820 5365  ettings: Auth Se
+0000c730: 7474 696e 6773 206e 616d 6573 2066 6f72  ttings names for
+0000c740: 2074 6865 2072 6571 7565 7374 2e0a 2020   the request..  
+0000c750: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+0000c760: 6561 6d3a 2069 6620 5472 7565 2c20 7468  eam: if True, th
+0000c770: 6520 7572 6c6c 6962 332e 4854 5450 5265  e urllib3.HTTPRe
+0000c780: 7370 6f6e 7365 206f 626a 6563 7420 7769  sponse object wi
+0000c790: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
 0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 6265 2072 6574 7572 6e65 6420 7769    be returned wi
-0000c7c0: 7468 6f75 7420 7265 6164 696e 672f 6465  thout reading/de
-0000c7d0: 636f 6469 6e67 2072 6573 706f 6e73 650a  coding response.
-0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 6265 2072 6574 7572 6e65 6420      be returned 
+0000c7c0: 7769 7468 6f75 7420 7265 6164 696e 672f  without reading/
+0000c7d0: 6465 636f 6469 6e67 2072 6573 706f 6e73  decoding respons
+0000c7e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
 0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2064 6174 612e 2041 6c73 6f20 7768 656e   data. Also when
-0000c810: 2054 7275 652c 2069 6620 7468 6520 6f70   True, if the op
-0000c820: 656e 6170 6920 7370 6563 2064 6573 6372  enapi spec descr
-0000c830: 6962 6573 2061 2066 696c 6520 646f 776e  ibes a file down
-0000c840: 6c6f 6164 2c0a 2020 2020 2020 2020 2020  load,.          
+0000c800: 2020 2064 6174 612e 2041 6c73 6f20 7768     data. Also wh
+0000c810: 656e 2054 7275 652c 2069 6620 7468 6520  en True, if the 
+0000c820: 6f70 656e 6170 6920 7370 6563 2064 6573  openapi spec des
+0000c830: 6372 6962 6573 2061 2066 696c 6520 646f  cribes a file do
+0000c840: 776e 6c6f 6164 2c0a 2020 2020 2020 2020  wnload,.        
 0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c860: 2020 2020 2020 2074 6865 2064 6174 6120         the data 
-0000c870: 7769 6c6c 2062 6520 7772 6974 7465 6e20  will be written 
-0000c880: 746f 2061 206c 6f63 616c 2066 696c 6573  to a local files
-0000c890: 7973 746d 6520 6669 6c65 2061 6e64 2074  ystme file and t
-0000c8a0: 6865 2042 696e 6172 7953 6368 656d 610a  he BinarySchema.
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2020 2020 2074 6865 2064 6174           the dat
+0000c870: 6120 7769 6c6c 2062 6520 7772 6974 7465  a will be writte
+0000c880: 6e20 746f 2061 206c 6f63 616c 2066 696c  n to a local fil
+0000c890: 6573 7973 746d 6520 6669 6c65 2061 6e64  esystme file and
+0000c8a0: 2074 6865 2042 696e 6172 7953 6368 656d   the BinarySchem
+0000c8b0: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
 0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8d0: 2069 6e73 7461 6e63 6520 7769 6c6c 2061   instance will a
-0000c8e0: 6c73 6f20 696e 6865 7269 7420 6672 6f6d  lso inherit from
-0000c8f0: 2046 696c 6553 6368 656d 6120 616e 6420   FileSchema and 
-0000c900: 4669 6c65 494f 0a20 2020 2020 2020 2020  FileIO.         
+0000c8d0: 2020 2069 6e73 7461 6e63 6520 7769 6c6c     instance will
+0000c8e0: 2061 6c73 6f20 696e 6865 7269 7420 6672   also inherit fr
+0000c8f0: 6f6d 2046 696c 6553 6368 656d 6120 616e  om FileSchema an
+0000c900: 6420 4669 6c65 494f 0a20 2020 2020 2020  d FileIO.       
 0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c920: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-0000c930: 6973 2046 616c 7365 2e0a 2020 2020 2020  is False..      
-0000c940: 2020 3a74 7970 6520 7374 7265 616d 3a20    :type stream: 
-0000c950: 626f 6f6c 2c20 6f70 7469 6f6e 616c 0a20  bool, optional. 
-0000c960: 2020 2020 2020 203a 7061 7261 6d20 7469         :param ti
-0000c970: 6d65 6f75 743a 2074 696d 656f 7574 2073  meout: timeout s
-0000c980: 6574 7469 6e67 2066 6f72 2074 6869 7320  etting for this 
-0000c990: 7265 7175 6573 742e 2049 6620 6f6e 650a  request. If one.
-0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c920: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+0000c930: 7420 6973 2046 616c 7365 2e0a 2020 2020  t is False..    
+0000c940: 2020 2020 3a74 7970 6520 7374 7265 616d      :type stream
+0000c950: 3a20 626f 6f6c 2c20 6f70 7469 6f6e 616c  : bool, optional
+0000c960: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c970: 7469 6d65 6f75 743a 2074 696d 656f 7574  timeout: timeout
+0000c980: 2073 6574 7469 6e67 2066 6f72 2074 6869   setting for thi
+0000c990: 7320 7265 7175 6573 742e 2049 6620 6f6e  s request. If on
+0000c9a0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
 0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9c0: 206e 756d 6265 7220 7072 6f76 6964 6564   number provided
-0000c9d0: 2c20 6974 2077 696c 6c20 6265 2074 6f74  , it will be tot
-0000c9e0: 616c 2072 6571 7565 7374 0a20 2020 2020  al request.     
+0000c9c0: 2020 206e 756d 6265 7220 7072 6f76 6964     number provid
+0000c9d0: 6564 2c20 6974 2077 696c 6c20 6265 2074  ed, it will be t
+0000c9e0: 6f74 616c 2072 6571 7565 7374 0a20 2020  otal request.   
 0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca00: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000ca10: 6f75 742e 2049 7420 6361 6e20 616c 736f  out. It can also
-0000ca20: 2062 6520 6120 7061 6972 2028 7475 706c   be a pair (tupl
-0000ca30: 6529 206f 660a 2020 2020 2020 2020 2020  e) of.          
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0000ca10: 6d65 6f75 742e 2049 7420 6361 6e20 616c  meout. It can al
+0000ca20: 736f 2062 6520 6120 7061 6972 2028 7475  so be a pair (tu
+0000ca30: 706c 6529 206f 660a 2020 2020 2020 2020  ple) of.        
 0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 2020 2020 2028 636f 6e6e 6563 7469         (connecti
-0000ca60: 6f6e 2c20 7265 6164 2920 7469 6d65 6f75  on, read) timeou
-0000ca70: 7473 2e0a 2020 2020 2020 2020 3a70 6172  ts..        :par
-0000ca80: 616d 2068 6f73 743a 2061 7069 2065 6e64  am host: api end
-0000ca90: 706f 696e 7420 686f 7374 0a20 2020 2020  point host.     
-0000caa0: 2020 203a 7265 7475 726e 3a20 7265 7370     :return: resp
-0000cab0: 6f6e 7365 0a20 2020 2020 2020 2022 2222  onse.        """
-0000cac0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000cad0: 6177 6169 7420 7365 6c66 2e5f 5f61 7379  await self.__asy
-0000cae0: 6e63 5f63 616c 6c5f 6170 6928 0a20 2020  nc_call_api(.   
-0000caf0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-0000cb00: 655f 7061 7468 2c0a 2020 2020 2020 2020  e_path,.        
-0000cb10: 2020 2020 6d65 7468 6f64 2c0a 2020 2020      method,.    
-0000cb20: 2020 2020 2020 2020 6865 6164 6572 732c          headers,
-0000cb30: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-0000cb40: 6961 6c69 7a65 645f 626f 6479 2c0a 2020  ialized_body,.  
-0000cb50: 2020 2020 2020 2020 2020 626f 6479 2c0a            body,.
-0000cb60: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
-0000cb70: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-0000cb80: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
-0000cb90: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-0000cba0: 6d2c 0a20 2020 2020 2020 2020 2020 2074  m,.            t
-0000cbb0: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
-0000cbc0: 2020 2020 686f 7374 2c0a 2020 2020 2020      host,.      
-0000cbd0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-0000cbe0: 6172 6174 6f72 5f69 7465 7261 746f 722c  arator_iterator,
-0000cbf0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000cc00: 6465 6620 6361 6c6c 5f61 7069 280a 2020  def call_api(.  
-0000cc10: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000cc20: 2020 2020 7265 736f 7572 6365 5f70 6174      resource_pat
-0000cc30: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-0000cc40: 6d65 7468 6f64 3a20 7374 722c 0a20 2020  method: str,.   
-0000cc50: 2020 2020 2068 6561 6465 7273 3a20 7479       headers: ty
-0000cc60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 4854  ping.Optional[HT
-0000cc70: 5450 4865 6164 6572 4469 6374 5d20 3d20  TPHeaderDict] = 
-0000cc80: 4e6f 6e65 2c0a 2020 2020 2020 2020 7365  None,.        se
-0000cc90: 7269 616c 697a 6564 5f62 6f64 793a 2074  rialized_body: t
-0000cca0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000ccb0: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
-0000ccc0: 2062 7974 6573 5d5d 203d 204e 6f6e 652c   bytes]] = None,
-0000ccd0: 0a20 2020 2020 2020 2062 6f64 793a 2074  .        body: t
-0000cce0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
-0000ccf0: 2c0a 2020 2020 2020 2020 6669 656c 6473  ,.        fields
-0000cd00: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000cd10: 6c5b 7479 7069 6e67 2e54 7570 6c65 5b74  l[typing.Tuple[t
-0000cd20: 7970 696e 672e 5475 706c 655b 7374 722c  yping.Tuple[str,
-0000cd30: 2073 7472 5d2c 202e 2e2e 5d5d 203d 204e   str], ...]] = N
-0000cd40: 6f6e 652c 0a20 2020 2020 2020 2061 7574  one,.        aut
-0000cd50: 685f 7365 7474 696e 6773 3a20 7479 7069  h_settings: typi
-0000cd60: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0000cd70: 6e67 2e4c 6973 745b 7374 725d 5d20 3d20  ng.List[str]] = 
-0000cd80: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-0000cd90: 7265 616d 3a20 626f 6f6c 203d 2046 616c  ream: bool = Fal
-0000cda0: 7365 2c0a 2020 2020 2020 2020 7469 6d65  se,.        time
-0000cdb0: 6f75 743a 2074 7970 696e 672e 4f70 7469  out: typing.Opti
-0000cdc0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
-0000cdd0: 6e5b 696e 742c 2074 7970 696e 672e 5475  n[int, typing.Tu
-0000cde0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
-0000cdf0: 2020 2020 2020 686f 7374 3a20 7479 7069        host: typi
-0000ce00: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-0000ce10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000ce20: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-0000ce30: 725f 6974 6572 6174 6f72 3a20 5072 6566  r_iterator: Pref
-0000ce40: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-0000ce50: 746f 7220 3d20 4e6f 6e65 2c0a 2020 2020  tor = None,.    
-0000ce60: 2920 2d3e 2052 6573 706f 6e73 6557 7261  ) -> ResponseWra
-0000ce70: 7070 6572 3a0a 2020 2020 2020 2020 2222  pper:.        ""
-0000ce80: 224d 616b 6573 2074 6865 2048 5454 5020  "Makes the HTTP 
-0000ce90: 7265 7175 6573 7420 2873 796e 6368 726f  request (synchro
-0000cea0: 6e6f 7573 2920 616e 6420 7265 7475 726e  nous) and return
-0000ceb0: 7320 6465 7365 7269 616c 697a 6564 2064  s deserialized d
-0000cec0: 6174 612e 0a0a 2020 2020 2020 2020 3a70  ata...        :p
-0000ced0: 6172 616d 2072 6573 6f75 7263 655f 7061  aram resource_pa
-0000cee0: 7468 3a20 5061 7468 2074 6f20 6d65 7468  th: Path to meth
-0000cef0: 6f64 2065 6e64 706f 696e 742e 0a20 2020  od endpoint..   
-0000cf00: 2020 2020 203a 7061 7261 6d20 6d65 7468       :param meth
-0000cf10: 6f64 3a20 4d65 7468 6f64 2074 6f20 6361  od: Method to ca
-0000cf20: 6c6c 2e0a 2020 2020 2020 2020 3a70 6172  ll..        :par
-0000cf30: 616d 2068 6561 6465 7273 3a20 4865 6164  am headers: Head
-0000cf40: 6572 2070 6172 616d 6574 6572 7320 746f  er parameters to
-0000cf50: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
-0000cf60: 706c 6163 6564 2069 6e20 7468 6520 7265  placed in the re
-0000cf70: 7175 6573 7420 6865 6164 6572 2e0a 2020  quest header..  
-0000cf80: 2020 2020 2020 3a70 6172 616d 2062 6f64        :param bod
-0000cf90: 793a 2052 6571 7565 7374 2062 6f64 792e  y: Request body.
-0000cfa0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000cfb0: 6669 656c 6473 3a20 5265 7175 6573 7420  fields: Request 
-0000cfc0: 706f 7374 2066 6f72 6d20 7061 7261 6d65  post form parame
-0000cfd0: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
-0000cfe0: 2020 666f 7220 6061 7070 6c69 6361 7469    for `applicati
-0000cff0: 6f6e 2f78 2d77 7777 2d66 6f72 6d2d 7572  on/x-www-form-ur
-0000d000: 6c65 6e63 6f64 6564 602c 2060 6d75 6c74  lencoded`, `mult
-0000d010: 6970 6172 742f 666f 726d 2d64 6174 6160  ipart/form-data`
-0000d020: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000d030: 2061 7574 685f 7365 7474 696e 6773 3a20   auth_settings: 
-0000d040: 4175 7468 2053 6574 7469 6e67 7320 6e61  Auth Settings na
-0000d050: 6d65 7320 666f 7220 7468 6520 7265 7175  mes for the requ
-0000d060: 6573 742e 0a20 2020 2020 2020 203a 7061  est..        :pa
-0000d070: 7261 6d20 7374 7265 616d 3a20 6966 2054  ram stream: if T
-0000d080: 7275 652c 2074 6865 2075 726c 6c69 6233  rue, the urllib3
-0000d090: 2e48 5454 5052 6573 706f 6e73 6520 6f62  .HTTPResponse ob
-0000d0a0: 6a65 6374 2077 696c 6c0a 2020 2020 2020  ject will.      
+0000ca50: 2020 2020 2020 2020 2028 636f 6e6e 6563           (connec
+0000ca60: 7469 6f6e 2c20 7265 6164 2920 7469 6d65  tion, read) time
+0000ca70: 6f75 7473 2e0a 2020 2020 2020 2020 3a70  outs..        :p
+0000ca80: 6172 616d 2068 6f73 743a 2061 7069 2065  aram host: api e
+0000ca90: 6e64 706f 696e 7420 686f 7374 0a20 2020  ndpoint host.   
+0000caa0: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
+0000cab0: 7370 6f6e 7365 0a20 2020 2020 2020 2022  sponse.        "
+0000cac0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000cad0: 6e20 6177 6169 7420 7365 6c66 2e5f 5f61  n await self.__a
+0000cae0: 7379 6e63 5f63 616c 6c5f 6170 6928 0a20  sync_call_api(. 
+0000caf0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
+0000cb00: 7263 655f 7061 7468 2c0a 2020 2020 2020  rce_path,.      
+0000cb10: 2020 2020 2020 6d65 7468 6f64 2c0a 2020        method,.  
+0000cb20: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0000cb30: 732c 0a20 2020 2020 2020 2020 2020 2073  s,.            s
+0000cb40: 6572 6961 6c69 7a65 645f 626f 6479 2c0a  erialized_body,.
+0000cb50: 2020 2020 2020 2020 2020 2020 626f 6479              body
+0000cb60: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
+0000cb70: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
+0000cb80: 2020 6175 7468 5f73 6574 7469 6e67 732c    auth_settings,
+0000cb90: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000cba0: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
+0000cbb0: 2074 696d 656f 7574 2c0a 2020 2020 2020   timeout,.      
+0000cbc0: 2020 2020 2020 686f 7374 2c0a 2020 2020        host,.    
+0000cbd0: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+0000cbe0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+0000cbf0: 722c 0a20 2020 2020 2020 2029 0a0a 2020  r,.        )..  
+0000cc00: 2020 6465 6620 6361 6c6c 5f61 7069 280a    def call_api(.
+0000cc10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000cc20: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
+0000cc30: 6174 683a 2073 7472 2c0a 2020 2020 2020  ath: str,.      
+0000cc40: 2020 6d65 7468 6f64 3a20 7374 722c 0a20    method: str,. 
+0000cc50: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+0000cc60: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000cc70: 4854 5450 4865 6164 6572 4469 6374 5d20  HTTPHeaderDict] 
+0000cc80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000cc90: 7365 7269 616c 697a 6564 5f62 6f64 793a  serialized_body:
+0000cca0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000ccb0: 5b74 7970 696e 672e 556e 696f 6e5b 7374  [typing.Union[st
+0000ccc0: 722c 2062 7974 6573 5d5d 203d 204e 6f6e  r, bytes]] = Non
+0000ccd0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0000cce0: 2074 7970 696e 672e 416e 7920 3d20 4e6f   typing.Any = No
+0000ccf0: 6e65 2c0a 2020 2020 2020 2020 6669 656c  ne,.        fiel
+0000cd00: 6473 3a20 7479 7069 6e67 2e4f 7074 696f  ds: typing.Optio
+0000cd10: 6e61 6c5b 7479 7069 6e67 2e54 7570 6c65  nal[typing.Tuple
+0000cd20: 5b74 7970 696e 672e 5475 706c 655b 7374  [typing.Tuple[st
+0000cd30: 722c 2073 7472 5d2c 202e 2e2e 5d5d 203d  r, str], ...]] =
+0000cd40: 204e 6f6e 652c 0a20 2020 2020 2020 2061   None,.        a
+0000cd50: 7574 685f 7365 7474 696e 6773 3a20 7479  uth_settings: ty
+0000cd60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000cd70: 7069 6e67 2e4c 6973 745b 7374 725d 5d20  ping.List[str]] 
+0000cd80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000cd90: 7374 7265 616d 3a20 626f 6f6c 203d 2046  stream: bool = F
+0000cda0: 616c 7365 2c0a 2020 2020 2020 2020 7469  alse,.        ti
+0000cdb0: 6d65 6f75 743a 2074 7970 696e 672e 4f70  meout: typing.Op
+0000cdc0: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0000cdd0: 696f 6e5b 696e 742c 2074 7970 696e 672e  ion[int, typing.
+0000cde0: 5475 706c 655d 5d20 3d20 4e6f 6e65 2c0a  Tuple]] = None,.
+0000cdf0: 2020 2020 2020 2020 686f 7374 3a20 7479          host: ty
+0000ce00: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+0000ce10: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000ce20: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+0000ce30: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
+0000ce40: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
+0000ce50: 7261 746f 7220 3d20 4e6f 6e65 2c0a 2020  rator = None,.  
+0000ce60: 2020 2920 2d3e 2052 6573 706f 6e73 6557    ) -> ResponseW
+0000ce70: 7261 7070 6572 3a0a 2020 2020 2020 2020  rapper:.        
+0000ce80: 2222 224d 616b 6573 2074 6865 2048 5454  """Makes the HTT
+0000ce90: 5020 7265 7175 6573 7420 2873 796e 6368  P request (synch
+0000cea0: 726f 6e6f 7573 2920 616e 6420 7265 7475  ronous) and retu
+0000ceb0: 726e 7320 6465 7365 7269 616c 697a 6564  rns deserialized
+0000cec0: 2064 6174 612e 0a0a 2020 2020 2020 2020   data...        
+0000ced0: 3a70 6172 616d 2072 6573 6f75 7263 655f  :param resource_
+0000cee0: 7061 7468 3a20 5061 7468 2074 6f20 6d65  path: Path to me
+0000cef0: 7468 6f64 2065 6e64 706f 696e 742e 0a20  thod endpoint.. 
+0000cf00: 2020 2020 2020 203a 7061 7261 6d20 6d65         :param me
+0000cf10: 7468 6f64 3a20 4d65 7468 6f64 2074 6f20  thod: Method to 
+0000cf20: 6361 6c6c 2e0a 2020 2020 2020 2020 3a70  call..        :p
+0000cf30: 6172 616d 2068 6561 6465 7273 3a20 4865  aram headers: He
+0000cf40: 6164 6572 2070 6172 616d 6574 6572 7320  ader parameters 
+0000cf50: 746f 2062 650a 2020 2020 2020 2020 2020  to be.          
+0000cf60: 2020 706c 6163 6564 2069 6e20 7468 6520    placed in the 
+0000cf70: 7265 7175 6573 7420 6865 6164 6572 2e0a  request header..
+0000cf80: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0000cf90: 6f64 793a 2052 6571 7565 7374 2062 6f64  ody: Request bod
+0000cfa0: 792e 0a20 2020 2020 2020 203a 7061 7261  y..        :para
+0000cfb0: 6d20 6669 656c 6473 3a20 5265 7175 6573  m fields: Reques
+0000cfc0: 7420 706f 7374 2066 6f72 6d20 7061 7261  t post form para
+0000cfd0: 6d65 7465 7273 2c0a 2020 2020 2020 2020  meters,.        
+0000cfe0: 2020 2020 666f 7220 6061 7070 6c69 6361      for `applica
+0000cff0: 7469 6f6e 2f78 2d77 7777 2d66 6f72 6d2d  tion/x-www-form-
+0000d000: 7572 6c65 6e63 6f64 6564 602c 2060 6d75  urlencoded`, `mu
+0000d010: 6c74 6970 6172 742f 666f 726d 2d64 6174  ltipart/form-dat
+0000d020: 6160 2e0a 2020 2020 2020 2020 3a70 6172  a`..        :par
+0000d030: 616d 2061 7574 685f 7365 7474 696e 6773  am auth_settings
+0000d040: 3a20 4175 7468 2053 6574 7469 6e67 7320  : Auth Settings 
+0000d050: 6e61 6d65 7320 666f 7220 7468 6520 7265  names for the re
+0000d060: 7175 6573 742e 0a20 2020 2020 2020 203a  quest..        :
+0000d070: 7061 7261 6d20 7374 7265 616d 3a20 6966  param stream: if
+0000d080: 2054 7275 652c 2074 6865 2075 726c 6c69   True, the urlli
+0000d090: 6233 2e48 5454 5052 6573 706f 6e73 6520  b3.HTTPResponse 
+0000d0a0: 6f62 6a65 6374 2077 696c 6c0a 2020 2020  object will.    
 0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 2020 2020 2062 6520 7265             be re
-0000d0d0: 7475 726e 6564 2077 6974 686f 7574 2072  turned without r
-0000d0e0: 6561 6469 6e67 2f64 6563 6f64 696e 6720  eading/decoding 
-0000d0f0: 7265 7370 6f6e 7365 0a20 2020 2020 2020  response.       
+0000d0c0: 2020 2020 2020 2020 2020 2020 2062 6520               be 
+0000d0d0: 7265 7475 726e 6564 2077 6974 686f 7574  returned without
+0000d0e0: 2072 6561 6469 6e67 2f64 6563 6f64 696e   reading/decodin
+0000d0f0: 6720 7265 7370 6f6e 7365 0a20 2020 2020  g response.     
 0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 2020 2020 2020 2020 2020 6461 7461 2e20            data. 
-0000d120: 416c 736f 2077 6865 6e20 5472 7565 2c20  Also when True, 
-0000d130: 6966 2074 6865 206f 7065 6e61 7069 2073  if the openapi s
-0000d140: 7065 6320 6465 7363 7269 6265 7320 6120  pec describes a 
-0000d150: 6669 6c65 2064 6f77 6e6c 6f61 642c 0a20  file download,. 
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d110: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000d120: 2e20 416c 736f 2077 6865 6e20 5472 7565  . Also when True
+0000d130: 2c20 6966 2074 6865 206f 7065 6e61 7069  , if the openapi
+0000d140: 2073 7065 6320 6465 7363 7269 6265 7320   spec describes 
+0000d150: 6120 6669 6c65 2064 6f77 6e6c 6f61 642c  a file download,
+0000d160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 7468 6520 6461 7461 2077 696c 6c20 6265  the data will be
-0000d190: 2077 7269 7474 656e 2074 6f20 6120 6c6f   written to a lo
-0000d1a0: 6361 6c20 6669 6c65 7379 7374 6d65 2066  cal filesystme f
-0000d1b0: 696c 6520 616e 6420 7468 6520 4269 6e61  ile and the Bina
-0000d1c0: 7279 5363 6865 6d61 0a20 2020 2020 2020  rySchema.       
+0000d180: 2020 7468 6520 6461 7461 2077 696c 6c20    the data will 
+0000d190: 6265 2077 7269 7474 656e 2074 6f20 6120  be written to a 
+0000d1a0: 6c6f 6361 6c20 6669 6c65 7379 7374 6d65  local filesystme
+0000d1b0: 2066 696c 6520 616e 6420 7468 6520 4269   file and the Bi
+0000d1c0: 6e61 7279 5363 6865 6d61 0a20 2020 2020  narySchema.     
 0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1e0: 2020 2020 2020 2020 2020 696e 7374 616e            instan
-0000d1f0: 6365 2077 696c 6c20 616c 736f 2069 6e68  ce will also inh
-0000d200: 6572 6974 2066 726f 6d20 4669 6c65 5363  erit from FileSc
-0000d210: 6865 6d61 2061 6e64 2046 696c 6549 4f0a  hema and FileIO.
-0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1e0: 2020 2020 2020 2020 2020 2020 696e 7374              inst
+0000d1f0: 616e 6365 2077 696c 6c20 616c 736f 2069  ance will also i
+0000d200: 6e68 6572 6974 2066 726f 6d20 4669 6c65  nherit from File
+0000d210: 5363 6865 6d61 2061 6e64 2046 696c 6549  Schema and FileI
+0000d220: 4f0a 2020 2020 2020 2020 2020 2020 2020  O.              
 0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
-0000d250: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-0000d260: 2073 7472 6561 6d3a 2062 6f6f 6c2c 206f   stream: bool, o
-0000d270: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0000d280: 3a70 6172 616d 2074 696d 656f 7574 3a20  :param timeout: 
-0000d290: 7469 6d65 6f75 7420 7365 7474 696e 6720  timeout setting 
-0000d2a0: 666f 7220 7468 6973 2072 6571 7565 7374  for this request
-0000d2b0: 2e20 4966 206f 6e65 0a20 2020 2020 2020  . If one.       
+0000d240: 2020 2044 6566 6175 6c74 2069 7320 4661     Default is Fa
+0000d250: 6c73 652e 0a20 2020 2020 2020 203a 7479  lse..        :ty
+0000d260: 7065 2073 7472 6561 6d3a 2062 6f6f 6c2c  pe stream: bool,
+0000d270: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0000d280: 2020 3a70 6172 616d 2074 696d 656f 7574    :param timeout
+0000d290: 3a20 7469 6d65 6f75 7420 7365 7474 696e  : timeout settin
+0000d2a0: 6720 666f 7220 7468 6973 2072 6571 7565  g for this reque
+0000d2b0: 7374 2e20 4966 206f 6e65 0a20 2020 2020  st. If one.     
 0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2d0: 2020 2020 2020 2020 2020 6e75 6d62 6572            number
-0000d2e0: 2070 726f 7669 6465 642c 2069 7420 7769   provided, it wi
-0000d2f0: 6c6c 2062 6520 746f 7461 6c20 7265 7175  ll be total requ
-0000d300: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
+0000d2d0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+0000d2e0: 6572 2070 726f 7669 6465 642c 2069 7420  er provided, it 
+0000d2f0: 7769 6c6c 2062 6520 746f 7461 6c20 7265  will be total re
+0000d300: 7175 6573 740a 2020 2020 2020 2020 2020  quest.          
 0000d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d320: 2020 2020 2074 696d 656f 7574 2e20 4974       timeout. It
-0000d330: 2063 616e 2061 6c73 6f20 6265 2061 2070   can also be a p
-0000d340: 6169 7220 2874 7570 6c65 2920 6f66 0a20  air (tuple) of. 
-0000d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d320: 2020 2020 2020 2074 696d 656f 7574 2e20         timeout. 
+0000d330: 4974 2063 616e 2061 6c73 6f20 6265 2061  It can also be a
+0000d340: 2070 6169 7220 2874 7570 6c65 2920 6f66   pair (tuple) of
+0000d350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d370: 2863 6f6e 6e65 6374 696f 6e2c 2072 6561  (connection, rea
-0000d380: 6429 2074 696d 656f 7574 732e 0a20 2020  d) timeouts..   
-0000d390: 2020 2020 203a 7061 7261 6d20 686f 7374       :param host
-0000d3a0: 3a20 6170 6920 656e 6470 6f69 6e74 2068  : api endpoint h
-0000d3b0: 6f73 740a 2020 2020 2020 2020 3a72 6574  ost.        :ret
-0000d3c0: 7572 6e3a 2072 6573 706f 6e73 650a 2020  urn: response.  
-0000d3d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d3e0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-0000d3f0: 6361 6c6c 5f61 7069 280a 2020 2020 2020  call_api(.      
-0000d400: 2020 2020 2020 7265 736f 7572 6365 5f70        resource_p
-0000d410: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000d420: 206d 6574 686f 642c 0a20 2020 2020 2020   method,.       
-0000d430: 2020 2020 2068 6561 6465 7273 2c0a 2020       headers,.  
-0000d440: 2020 2020 2020 2020 2020 7365 7269 616c            serial
-0000d450: 697a 6564 5f62 6f64 792c 0a20 2020 2020  ized_body,.     
-0000d460: 2020 2020 2020 2062 6f64 792c 0a20 2020         body,.   
-0000d470: 2020 2020 2020 2020 2066 6965 6c64 732c           fields,
-0000d480: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
-0000d490: 685f 7365 7474 696e 6773 2c0a 2020 2020  h_settings,.    
-0000d4a0: 2020 2020 2020 2020 7374 7265 616d 2c0a          stream,.
-0000d4b0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-0000d4c0: 6f75 742c 0a20 2020 2020 2020 2020 2020  out,.           
-0000d4d0: 2068 6f73 742c 0a20 2020 2020 2020 2020   host,.         
-0000d4e0: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-0000d4f0: 746f 725f 6974 6572 6174 6f72 2c0a 2020  tor_iterator,.  
-0000d500: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-0000d510: 2066 6965 6c64 735f 746f 5f64 6963 7428   fields_to_dict(
-0000d520: 7365 6c66 2c20 6669 656c 6473 3a20 7479  self, fields: ty
-0000d530: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-0000d540: 7069 6e67 2e54 7570 6c65 5b74 7970 696e  ping.Tuple[typin
-0000d550: 672e 5475 706c 655b 7374 722c 2073 7472  g.Tuple[str, str
-0000d560: 5d2c 202e 2e2e 5d5d 293a 0a20 2020 2020  ], ...]]):.     
-0000d570: 2020 2022 2222 436f 6e76 6572 7473 2066     """Converts f
-0000d580: 6965 6c64 7320 746f 2064 6963 742e 0a0a  ields to dict...
-0000d590: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-0000d5a0: 6965 6c64 733a 2066 6965 6c64 730a 2020  ields: fields.  
-0000d5b0: 2020 2020 2020 3a72 6574 7572 6e3a 2064        :return: d
-0000d5c0: 6963 740a 2020 2020 2020 2020 2222 220a  ict.        """.
-0000d5d0: 2020 2020 2020 2020 6966 2066 6965 6c64          if field
-0000d5e0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0000d5f0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-0000d600: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
-0000d610: 6e20 7b6b 3a20 7620 666f 7220 6b2c 2076  n {k: v for k, v
-0000d620: 2069 6e20 6669 656c 6473 7d0a 0a20 2020   in fields}..   
-0000d630: 2061 7379 6e63 2064 6566 2061 7379 6e63   async def async
-0000d640: 5f72 6571 7565 7374 280a 2020 2020 2020  _request(.      
-0000d650: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000d660: 6d65 7468 6f64 3a20 7374 722c 0a20 2020  method: str,.   
-0000d670: 2020 2020 2075 726c 3a20 7374 722c 0a20       url: str,. 
-0000d680: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-0000d690: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-0000d6a0: 4854 5450 4865 6164 6572 4469 6374 5d20  HTTPHeaderDict] 
-0000d6b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000d6c0: 6669 656c 6473 3a20 7479 7069 6e67 2e4f  fields: typing.O
-0000d6d0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e54  ptional[typing.T
-0000d6e0: 7570 6c65 5b74 7970 696e 672e 5475 706c  uple[typing.Tupl
-0000d6f0: 655b 7374 722c 2073 7472 5d2c 202e 2e2e  e[str, str], ...
-0000d700: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-0000d710: 2020 2062 6f64 793a 2074 7970 696e 672e     body: typing.
-0000d720: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0000d730: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
-0000d740: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-0000d750: 2020 2073 7472 6561 6d3a 2062 6f6f 6c20     stream: bool 
-0000d760: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
-0000d770: 2074 696d 656f 7574 3a20 7479 7069 6e67   timeout: typing
-0000d780: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0000d790: 2e55 6e69 6f6e 5b69 6e74 2c20 7479 7069  .Union[int, typi
-0000d7a0: 6e67 2e54 7570 6c65 5d5d 203d 204e 6f6e  ng.Tuple]] = Non
-0000d7b0: 652c 0a20 2020 2029 202d 3e20 4173 796e  e,.    ) -> Asyn
-0000d7c0: 6352 6573 706f 6e73 6557 7261 7070 6572  cResponseWrapper
-0000d7d0: 3a0a 2020 2020 2020 2020 6966 2062 6f64  :.        if bod
-0000d7e0: 7920 616e 6420 6669 656c 6473 3a0a 2020  y and fields:.  
-0000d7f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000d800: 4170 6956 616c 7565 4572 726f 7228 2262  ApiValueError("b
-0000d810: 6f64 7920 7061 7261 6d65 7465 7220 6361  ody parameter ca
-0000d820: 6e6e 6f74 2062 6520 7573 6564 2077 6974  nnot be used wit
-0000d830: 6820 6669 656c 6473 2070 6172 616d 6574  h fields paramet
-0000d840: 6572 2229 0a20 2020 2020 2020 2064 6174  er").        dat
-0000d850: 6120 3d20 4e6f 6e65 0a20 2020 2020 2020  a = None.       
-0000d860: 2069 6620 626f 6479 3a0a 2020 2020 2020   if body:.      
-0000d870: 2020 2020 2020 6461 7461 3d62 6f64 790a        data=body.
-0000d880: 2020 2020 2020 2020 6966 2066 6965 6c64          if field
-0000d890: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-0000d8a0: 6174 613d 7365 6c66 2e66 6965 6c64 735f  ata=self.fields_
-0000d8b0: 746f 5f64 6963 7428 6669 656c 6473 290a  to_dict(fields).
-0000d8c0: 2020 2020 2020 2020 7365 7373 696f 6e20          session 
-0000d8d0: 3d20 6169 6f68 7474 702e 436c 6965 6e74  = aiohttp.Client
-0000d8e0: 5365 7373 696f 6e28 290a 2020 2020 2020  Session().      
-0000d8f0: 2020 7431 203d 2074 696d 652e 7469 6d65    t1 = time.time
-0000d900: 2829 0a20 2020 2020 2020 2069 6620 6d65  ().        if me
-0000d910: 7468 6f64 203d 3d20 2247 4554 223a 0a20  thod == "GET":. 
-0000d920: 2020 2020 2020 2020 2020 2073 6573 7369             sessi
-0000d930: 6f6e 2e67 6574 2875 726c 290a 2020 2020  on.get(url).    
-0000d940: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000d950: 203d 2061 7761 6974 2073 6573 7369 6f6e   = await session
-0000d960: 2e67 6574 2875 726c 2c20 6865 6164 6572  .get(url, header
-0000d970: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
-0000d980: 2020 2020 2020 2072 6574 7572 6e20 4173         return As
-0000d990: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
-0000d9a0: 6572 2872 6573 706f 6e73 652c 2074 696d  er(response, tim
-0000d9b0: 652e 7469 6d65 2829 202d 2074 312c 2073  e.time() - t1, s
-0000d9c0: 6573 7369 6f6e 290a 2020 2020 2020 2020  ession).        
-0000d9d0: 656c 6966 206d 6574 686f 6420 3d3d 2022  elif method == "
-0000d9e0: 4845 4144 223a 0a20 2020 2020 2020 2020  HEAD":.         
-0000d9f0: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
-0000da00: 6169 7420 7365 7373 696f 6e2e 6865 6164  ait session.head
-0000da10: 2875 726c 2c20 6865 6164 6572 733d 6865  (url, headers=he
-0000da20: 6164 6572 7329 0a20 2020 2020 2020 2020  aders).         
-0000da30: 2020 2072 6574 7572 6e20 4173 796e 6352     return AsyncR
-0000da40: 6573 706f 6e73 6557 7261 7070 6572 2872  esponseWrapper(r
-0000da50: 6573 706f 6e73 652c 2074 696d 652e 7469  esponse, time.ti
-0000da60: 6d65 2829 202d 2074 312c 2073 6573 7369  me() - t1, sessi
-0000da70: 6f6e 290a 2020 2020 2020 2020 656c 6966  on).        elif
-0000da80: 206d 6574 686f 6420 3d3d 2022 4f50 5449   method == "OPTI
-0000da90: 4f4e 5322 3a0a 2020 2020 2020 2020 2020  ONS":.          
-0000daa0: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
-0000dab0: 6974 2073 6573 7369 6f6e 2e6f 7074 696f  it session.optio
-0000dac0: 6e73 2875 726c 2c20 6461 7461 3d64 6174  ns(url, data=dat
-0000dad0: 612c 2068 6561 6465 7273 3d68 6561 6465  a, headers=heade
-0000dae0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-0000daf0: 7265 7475 726e 2041 7379 6e63 5265 7370  return AsyncResp
-0000db00: 6f6e 7365 5772 6170 7065 7228 7265 7370  onseWrapper(resp
-0000db10: 6f6e 7365 2c20 7469 6d65 2e74 696d 6528  onse, time.time(
-0000db20: 2920 2d20 7431 2c20 7365 7373 696f 6e29  ) - t1, session)
-0000db30: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
-0000db40: 7468 6f64 203d 3d20 2250 4f53 5422 3a0a  thod == "POST":.
-0000db50: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-0000db60: 6f6e 7365 203d 2061 7761 6974 2073 6573  onse = await ses
-0000db70: 7369 6f6e 2e70 6f73 7428 7572 6c2c 2064  sion.post(url, d
-0000db80: 6174 613d 6461 7461 2c20 6865 6164 6572  ata=data, header
-0000db90: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
-0000dba0: 2020 2020 2020 2072 6574 7572 6e20 4173         return As
-0000dbb0: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
-0000dbc0: 6572 2872 6573 706f 6e73 652c 2074 696d  er(response, tim
-0000dbd0: 652e 7469 6d65 2829 202d 2074 312c 2073  e.time() - t1, s
-0000dbe0: 6573 7369 6f6e 290a 2020 2020 2020 2020  ession).        
-0000dbf0: 656c 6966 206d 6574 686f 6420 3d3d 2022  elif method == "
-0000dc00: 5055 5422 3a0a 2020 2020 2020 2020 2020  PUT":.          
-0000dc10: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
-0000dc20: 6974 2073 6573 7369 6f6e 2e70 7574 2875  it session.put(u
-0000dc30: 726c 2c20 6461 7461 3d64 6174 612c 2068  rl, data=data, h
-0000dc40: 6561 6465 7273 3d68 6561 6465 7273 290a  eaders=headers).
-0000dc50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000dc60: 726e 2041 7379 6e63 5265 7370 6f6e 7365  rn AsyncResponse
-0000dc70: 5772 6170 7065 7228 7265 7370 6f6e 7365  Wrapper(response
-0000dc80: 2c20 7469 6d65 2e74 696d 6528 2920 2d20  , time.time() - 
-0000dc90: 7431 2c20 7365 7373 696f 6e29 0a20 2020  t1, session).   
-0000dca0: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
-0000dcb0: 203d 3d20 2250 4154 4348 223a 0a20 2020   == "PATCH":.   
-0000dcc0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-0000dcd0: 6520 3d20 6177 6169 7420 7365 7373 696f  e = await sessio
-0000dce0: 6e2e 7061 7463 6828 7572 6c2c 2064 6174  n.patch(url, dat
-0000dcf0: 613d 6461 7461 2c20 6865 6164 6572 733d  a=data, headers=
-0000dd00: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
-0000dd10: 2020 2020 2072 6574 7572 6e20 4173 796e       return Asyn
-0000dd20: 6352 6573 706f 6e73 6557 7261 7070 6572  cResponseWrapper
-0000dd30: 2872 6573 706f 6e73 652c 2074 696d 652e  (response, time.
-0000dd40: 7469 6d65 2829 202d 2074 312c 2073 6573  time() - t1, ses
-0000dd50: 7369 6f6e 290a 2020 2020 2020 2020 656c  sion).        el
-0000dd60: 6966 206d 6574 686f 6420 3d3d 2022 4445  if method == "DE
-0000dd70: 4c45 5445 223a 0a20 2020 2020 2020 2020  LETE":.         
-0000dd80: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
-0000dd90: 6169 7420 7365 7373 696f 6e2e 6465 6c65  ait session.dele
-0000dda0: 7465 2875 726c 2c20 6461 7461 3d64 6174  te(url, data=dat
-0000ddb0: 612c 2068 6561 6465 7273 3d68 6561 6465  a, headers=heade
-0000ddc0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-0000ddd0: 7265 7475 726e 2041 7379 6e63 5265 7370  return AsyncResp
-0000dde0: 6f6e 7365 5772 6170 7065 7228 7265 7370  onseWrapper(resp
-0000ddf0: 6f6e 7365 2c20 7469 6d65 2e74 696d 6528  onse, time.time(
-0000de00: 2920 2d20 7431 2c20 7365 7373 696f 6e29  ) - t1, session)
-0000de10: 0a20 2020 2020 2020 2072 6169 7365 2041  .        raise A
-0000de20: 7069 5661 6c75 6545 7272 6f72 280a 2020  piValueError(.  
-0000de30: 2020 2020 2020 2020 2020 2268 7474 7020            "http 
-0000de40: 6d65 7468 6f64 206d 7573 7420 6265 2060  method must be `
-0000de50: 4745 5460 2c20 6048 4541 4460 2c20 604f  GET`, `HEAD`, `O
-0000de60: 5054 494f 4e53 602c 220a 2020 2020 2020  PTIONS`,".      
-0000de70: 2020 2020 2020 2220 6050 4f53 5460 2c20        " `POST`, 
-0000de80: 6050 4154 4348 602c 2060 5055 5460 206f  `PATCH`, `PUT` o
-0000de90: 7220 6044 454c 4554 4560 2e22 0a20 2020  r `DELETE`.".   
-0000dea0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000deb0: 7265 7175 6573 7428 0a20 2020 2020 2020  request(.       
-0000dec0: 2073 656c 662c 0a20 2020 2020 2020 206d   self,.        m
-0000ded0: 6574 686f 643a 2073 7472 2c0a 2020 2020  ethod: str,.    
-0000dee0: 2020 2020 7572 6c3a 2073 7472 2c0a 2020      url: str,.  
-0000def0: 2020 2020 2020 6865 6164 6572 733a 2074        headers: t
-0000df00: 7970 696e 672e 4f70 7469 6f6e 616c 5b48  yping.Optional[H
-0000df10: 5454 5048 6561 6465 7244 6963 745d 203d  TTPHeaderDict] =
-0000df20: 204e 6f6e 652c 0a20 2020 2020 2020 2066   None,.        f
-0000df30: 6965 6c64 733a 2074 7970 696e 672e 4f70  ields: typing.Op
-0000df40: 7469 6f6e 616c 5b74 7970 696e 672e 5475  tional[typing.Tu
-0000df50: 706c 655b 7479 7069 6e67 2e54 7570 6c65  ple[typing.Tuple
-0000df60: 5b73 7472 2c20 7374 725d 2c20 2e2e 2e5d  [str, str], ...]
-0000df70: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000df80: 2020 626f 6479 3a20 7479 7069 6e67 2e4f    body: typing.O
-0000df90: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
-0000dfa0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
-0000dfb0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000dfc0: 2020 7374 7265 616d 3a20 626f 6f6c 203d    stream: bool =
-0000dfd0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000dfe0: 7469 6d65 6f75 743a 2074 7970 696e 672e  timeout: typing.
-0000dff0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0000e000: 556e 696f 6e5b 696e 742c 2074 7970 696e  Union[int, typin
-0000e010: 672e 5475 706c 655d 5d20 3d20 4e6f 6e65  g.Tuple]] = None
-0000e020: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
-0000e030: 6e73 6557 7261 7070 6572 3a0a 2020 2020  nseWrapper:.    
-0000e040: 2020 2020 2222 224d 616b 6573 2074 6865      """Makes the
-0000e050: 2048 5454 5020 7265 7175 6573 7420 7573   HTTP request us
-0000e060: 696e 6720 5245 5354 436c 6965 6e74 2e22  ing RESTClient."
-0000e070: 2222 0a20 2020 2020 2020 2069 6620 6d65  "".        if me
-0000e080: 7468 6f64 203d 3d20 2247 4554 223a 0a20  thod == "GET":. 
-0000e090: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e0a0: 6e20 7365 6c66 2e72 6573 745f 636c 6965  n self.rest_clie
-0000e0b0: 6e74 2e47 4554 2875 726c 2c0a 2020 2020  nt.GET(url,.    
+0000d370: 2020 2863 6f6e 6e65 6374 696f 6e2c 2072    (connection, r
+0000d380: 6561 6429 2074 696d 656f 7574 732e 0a20  ead) timeouts.. 
+0000d390: 2020 2020 2020 203a 7061 7261 6d20 686f         :param ho
+0000d3a0: 7374 3a20 6170 6920 656e 6470 6f69 6e74  st: api endpoint
+0000d3b0: 2068 6f73 740a 2020 2020 2020 2020 3a72   host.        :r
+0000d3c0: 6574 7572 6e3a 2072 6573 706f 6e73 650a  eturn: response.
+0000d3d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d3e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000d3f0: 5f5f 6361 6c6c 5f61 7069 280a 2020 2020  __call_api(.    
+0000d400: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000d410: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0000d420: 2020 206d 6574 686f 642c 0a20 2020 2020     method,.     
+0000d430: 2020 2020 2020 2068 6561 6465 7273 2c0a         headers,.
+0000d440: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+0000d450: 616c 697a 6564 5f62 6f64 792c 0a20 2020  alized_body,.   
+0000d460: 2020 2020 2020 2020 2062 6f64 792c 0a20           body,. 
+0000d470: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+0000d480: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
+0000d490: 7574 685f 7365 7474 696e 6773 2c0a 2020  uth_settings,.  
+0000d4a0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+0000d4b0: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
+0000d4c0: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
+0000d4d0: 2020 2068 6f73 742c 0a20 2020 2020 2020     host,.       
+0000d4e0: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
+0000d4f0: 7261 746f 725f 6974 6572 6174 6f72 2c0a  rator_iterator,.
+0000d500: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000d510: 6566 2066 6965 6c64 735f 746f 5f64 6963  ef fields_to_dic
+0000d520: 7428 7365 6c66 2c20 6669 656c 6473 3a20  t(self, fields: 
+0000d530: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000d540: 7479 7069 6e67 2e54 7570 6c65 5b74 7970  typing.Tuple[typ
+0000d550: 696e 672e 5475 706c 655b 7374 722c 2073  ing.Tuple[str, s
+0000d560: 7472 5d2c 202e 2e2e 5d5d 293a 0a20 2020  tr], ...]]):.   
+0000d570: 2020 2020 2022 2222 436f 6e76 6572 7473       """Converts
+0000d580: 2066 6965 6c64 7320 746f 2064 6963 742e   fields to dict.
+0000d590: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000d5a0: 2066 6965 6c64 733a 2066 6965 6c64 730a   fields: fields.
+0000d5b0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+0000d5c0: 2064 6963 740a 2020 2020 2020 2020 2222   dict.        ""
+0000d5d0: 220a 2020 2020 2020 2020 6966 2066 6965  ".        if fie
+0000d5e0: 6c64 7320 6973 204e 6f6e 653a 0a20 2020  lds is None:.   
+0000d5f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d600: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+0000d610: 7572 6e20 7b6b 3a20 7620 666f 7220 6b2c  urn {k: v for k,
+0000d620: 2076 2069 6e20 6669 656c 6473 7d0a 0a20   v in fields}.. 
+0000d630: 2020 2061 7379 6e63 2064 6566 2061 7379     async def asy
+0000d640: 6e63 5f72 6571 7565 7374 280a 2020 2020  nc_request(.    
+0000d650: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000d660: 2020 6d65 7468 6f64 3a20 7374 722c 0a20    method: str,. 
+0000d670: 2020 2020 2020 2075 726c 3a20 7374 722c         url: str,
+0000d680: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
+0000d690: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000d6a0: 6c5b 4854 5450 4865 6164 6572 4469 6374  l[HTTPHeaderDict
+0000d6b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000d6c0: 2020 6669 656c 6473 3a20 7479 7069 6e67    fields: typing
+0000d6d0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000d6e0: 2e54 7570 6c65 5b74 7970 696e 672e 5475  .Tuple[typing.Tu
+0000d6f0: 706c 655b 7374 722c 2073 7472 5d2c 202e  ple[str, str], .
+0000d700: 2e2e 5d5d 203d 204e 6f6e 652c 0a20 2020  ..]] = None,.   
+0000d710: 2020 2020 2062 6f64 793a 2074 7970 696e       body: typin
+0000d720: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000d730: 672e 556e 696f 6e5b 7374 722c 2062 7974  g.Union[str, byt
+0000d740: 6573 5d5d 203d 204e 6f6e 652c 0a20 2020  es]] = None,.   
+0000d750: 2020 2020 2073 7472 6561 6d3a 2062 6f6f       stream: boo
+0000d760: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+0000d770: 2020 2074 696d 656f 7574 3a20 7479 7069     timeout: typi
+0000d780: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+0000d790: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7479  ng.Union[int, ty
+0000d7a0: 7069 6e67 2e54 7570 6c65 5d5d 203d 204e  ping.Tuple]] = N
+0000d7b0: 6f6e 652c 0a20 2020 2029 202d 3e20 4173  one,.    ) -> As
+0000d7c0: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
+0000d7d0: 6572 3a0a 2020 2020 2020 2020 6966 2062  er:.        if b
+0000d7e0: 6f64 7920 616e 6420 6669 656c 6473 3a0a  ody and fields:.
+0000d7f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000d800: 6520 4170 6956 616c 7565 4572 726f 7228  e ApiValueError(
+0000d810: 2262 6f64 7920 7061 7261 6d65 7465 7220  "body parameter 
+0000d820: 6361 6e6e 6f74 2062 6520 7573 6564 2077  cannot be used w
+0000d830: 6974 6820 6669 656c 6473 2070 6172 616d  ith fields param
+0000d840: 6574 6572 2229 0a20 2020 2020 2020 2064  eter").        d
+0000d850: 6174 6120 3d20 4e6f 6e65 0a20 2020 2020  ata = None.     
+0000d860: 2020 2069 6620 626f 6479 3a0a 2020 2020     if body:.    
+0000d870: 2020 2020 2020 2020 6461 7461 3d62 6f64          data=bod
+0000d880: 790a 2020 2020 2020 2020 6966 2066 6965  y.        if fie
+0000d890: 6c64 733a 0a20 2020 2020 2020 2020 2020  lds:.           
+0000d8a0: 2064 6174 613d 7365 6c66 2e66 6965 6c64   data=self.field
+0000d8b0: 735f 746f 5f64 6963 7428 6669 656c 6473  s_to_dict(fields
+0000d8c0: 290a 2020 2020 2020 2020 7365 7373 696f  ).        sessio
+0000d8d0: 6e20 3d20 6169 6f68 7474 702e 436c 6965  n = aiohttp.Clie
+0000d8e0: 6e74 5365 7373 696f 6e28 290a 2020 2020  ntSession().    
+0000d8f0: 2020 2020 7431 203d 2074 696d 652e 7469      t1 = time.ti
+0000d900: 6d65 2829 0a20 2020 2020 2020 2069 6620  me().        if 
+0000d910: 6d65 7468 6f64 203d 3d20 2247 4554 223a  method == "GET":
+0000d920: 0a20 2020 2020 2020 2020 2020 2073 6573  .            ses
+0000d930: 7369 6f6e 2e67 6574 2875 726c 290a 2020  sion.get(url).  
+0000d940: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+0000d950: 7365 203d 2061 7761 6974 2073 6573 7369  se = await sessi
+0000d960: 6f6e 2e67 6574 2875 726c 2c20 6865 6164  on.get(url, head
+0000d970: 6572 733d 6865 6164 6572 7329 0a20 2020  ers=headers).   
+0000d980: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d990: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000d9a0: 7070 6572 2872 6573 706f 6e73 652c 2074  pper(response, t
+0000d9b0: 696d 652e 7469 6d65 2829 202d 2074 312c  ime.time() - t1,
+0000d9c0: 2073 6573 7369 6f6e 290a 2020 2020 2020   session).      
+0000d9d0: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
+0000d9e0: 2022 4845 4144 223a 0a20 2020 2020 2020   "HEAD":.       
+0000d9f0: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000da00: 6177 6169 7420 7365 7373 696f 6e2e 6865  await session.he
+0000da10: 6164 2875 726c 2c20 6865 6164 6572 733d  ad(url, headers=
+0000da20: 6865 6164 6572 7329 0a20 2020 2020 2020  headers).       
+0000da30: 2020 2020 2072 6574 7572 6e20 4173 796e       return Asyn
+0000da40: 6352 6573 706f 6e73 6557 7261 7070 6572  cResponseWrapper
+0000da50: 2872 6573 706f 6e73 652c 2074 696d 652e  (response, time.
+0000da60: 7469 6d65 2829 202d 2074 312c 2073 6573  time() - t1, ses
+0000da70: 7369 6f6e 290a 2020 2020 2020 2020 656c  sion).        el
+0000da80: 6966 206d 6574 686f 6420 3d3d 2022 4f50  if method == "OP
+0000da90: 5449 4f4e 5322 3a0a 2020 2020 2020 2020  TIONS":.        
+0000daa0: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+0000dab0: 7761 6974 2073 6573 7369 6f6e 2e6f 7074  wait session.opt
+0000dac0: 696f 6e73 2875 726c 2c20 6461 7461 3d64  ions(url, data=d
+0000dad0: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
+0000dae0: 6465 7273 290a 2020 2020 2020 2020 2020  ders).          
+0000daf0: 2020 7265 7475 726e 2041 7379 6e63 5265    return AsyncRe
+0000db00: 7370 6f6e 7365 5772 6170 7065 7228 7265  sponseWrapper(re
+0000db10: 7370 6f6e 7365 2c20 7469 6d65 2e74 696d  sponse, time.tim
+0000db20: 6528 2920 2d20 7431 2c20 7365 7373 696f  e() - t1, sessio
+0000db30: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
+0000db40: 6d65 7468 6f64 203d 3d20 2250 4f53 5422  method == "POST"
+0000db50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000db60: 7370 6f6e 7365 203d 2061 7761 6974 2073  sponse = await s
+0000db70: 6573 7369 6f6e 2e70 6f73 7428 7572 6c2c  ession.post(url,
+0000db80: 2064 6174 613d 6461 7461 2c20 6865 6164   data=data, head
+0000db90: 6572 733d 6865 6164 6572 7329 0a20 2020  ers=headers).   
+0000dba0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000dbb0: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000dbc0: 7070 6572 2872 6573 706f 6e73 652c 2074  pper(response, t
+0000dbd0: 696d 652e 7469 6d65 2829 202d 2074 312c  ime.time() - t1,
+0000dbe0: 2073 6573 7369 6f6e 290a 2020 2020 2020   session).      
+0000dbf0: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
+0000dc00: 2022 5055 5422 3a0a 2020 2020 2020 2020   "PUT":.        
+0000dc10: 2020 2020 7265 7370 6f6e 7365 203d 2061      response = a
+0000dc20: 7761 6974 2073 6573 7369 6f6e 2e70 7574  wait session.put
+0000dc30: 2875 726c 2c20 6461 7461 3d64 6174 612c  (url, data=data,
+0000dc40: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
+0000dc50: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000dc60: 7475 726e 2041 7379 6e63 5265 7370 6f6e  turn AsyncRespon
+0000dc70: 7365 5772 6170 7065 7228 7265 7370 6f6e  seWrapper(respon
+0000dc80: 7365 2c20 7469 6d65 2e74 696d 6528 2920  se, time.time() 
+0000dc90: 2d20 7431 2c20 7365 7373 696f 6e29 0a20  - t1, session). 
+0000dca0: 2020 2020 2020 2065 6c69 6620 6d65 7468         elif meth
+0000dcb0: 6f64 203d 3d20 2250 4154 4348 223a 0a20  od == "PATCH":. 
+0000dcc0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+0000dcd0: 6e73 6520 3d20 6177 6169 7420 7365 7373  nse = await sess
+0000dce0: 696f 6e2e 7061 7463 6828 7572 6c2c 2064  ion.patch(url, d
+0000dcf0: 6174 613d 6461 7461 2c20 6865 6164 6572  ata=data, header
+0000dd00: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
+0000dd10: 2020 2020 2020 2072 6574 7572 6e20 4173         return As
+0000dd20: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
+0000dd30: 6572 2872 6573 706f 6e73 652c 2074 696d  er(response, tim
+0000dd40: 652e 7469 6d65 2829 202d 2074 312c 2073  e.time() - t1, s
+0000dd50: 6573 7369 6f6e 290a 2020 2020 2020 2020  ession).        
+0000dd60: 656c 6966 206d 6574 686f 6420 3d3d 2022  elif method == "
+0000dd70: 4445 4c45 5445 223a 0a20 2020 2020 2020  DELETE":.       
+0000dd80: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+0000dd90: 6177 6169 7420 7365 7373 696f 6e2e 6465  await session.de
+0000dda0: 6c65 7465 2875 726c 2c20 6461 7461 3d64  lete(url, data=d
+0000ddb0: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
+0000ddc0: 6465 7273 290a 2020 2020 2020 2020 2020  ders).          
+0000ddd0: 2020 7265 7475 726e 2041 7379 6e63 5265    return AsyncRe
+0000dde0: 7370 6f6e 7365 5772 6170 7065 7228 7265  sponseWrapper(re
+0000ddf0: 7370 6f6e 7365 2c20 7469 6d65 2e74 696d  sponse, time.tim
+0000de00: 6528 2920 2d20 7431 2c20 7365 7373 696f  e() - t1, sessio
+0000de10: 6e29 0a20 2020 2020 2020 2072 6169 7365  n).        raise
+0000de20: 2041 7069 5661 6c75 6545 7272 6f72 280a   ApiValueError(.
+0000de30: 2020 2020 2020 2020 2020 2020 2268 7474              "htt
+0000de40: 7020 6d65 7468 6f64 206d 7573 7420 6265  p method must be
+0000de50: 2060 4745 5460 2c20 6048 4541 4460 2c20   `GET`, `HEAD`, 
+0000de60: 604f 5054 494f 4e53 602c 220a 2020 2020  `OPTIONS`,".    
+0000de70: 2020 2020 2020 2020 2220 6050 4f53 5460          " `POST`
+0000de80: 2c20 6050 4154 4348 602c 2060 5055 5460  , `PATCH`, `PUT`
+0000de90: 206f 7220 6044 454c 4554 4560 2e22 0a20   or `DELETE`.". 
+0000dea0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+0000deb0: 6620 7265 7175 6573 7428 0a20 2020 2020  f request(.     
+0000dec0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000ded0: 206d 6574 686f 643a 2073 7472 2c0a 2020   method: str,.  
+0000dee0: 2020 2020 2020 7572 6c3a 2073 7472 2c0a        url: str,.
+0000def0: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+0000df00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000df10: 5b48 5454 5048 6561 6465 7244 6963 745d  [HTTPHeaderDict]
+0000df20: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000df30: 2066 6965 6c64 733a 2074 7970 696e 672e   fields: typing.
+0000df40: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+0000df50: 5475 706c 655b 7479 7069 6e67 2e54 7570  Tuple[typing.Tup
+0000df60: 6c65 5b73 7472 2c20 7374 725d 2c20 2e2e  le[str, str], ..
+0000df70: 2e5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  .]] = None,.    
+0000df80: 2020 2020 626f 6479 3a20 7479 7069 6e67      body: typing
+0000df90: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000dfa0: 2e55 6e69 6f6e 5b73 7472 2c20 6279 7465  .Union[str, byte
+0000dfb0: 735d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  s]] = None,.    
+0000dfc0: 2020 2020 7374 7265 616d 3a20 626f 6f6c      stream: bool
+0000dfd0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+0000dfe0: 2020 7469 6d65 6f75 743a 2074 7970 696e    timeout: typin
+0000dff0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000e000: 672e 556e 696f 6e5b 696e 742c 2074 7970  g.Union[int, typ
+0000e010: 696e 672e 5475 706c 655d 5d20 3d20 4e6f  ing.Tuple]] = No
+0000e020: 6e65 2c0a 2020 2020 2920 2d3e 2052 6573  ne,.    ) -> Res
+0000e030: 706f 6e73 6557 7261 7070 6572 3a0a 2020  ponseWrapper:.  
+0000e040: 2020 2020 2020 2222 224d 616b 6573 2074        """Makes t
+0000e050: 6865 2048 5454 5020 7265 7175 6573 7420  he HTTP request 
+0000e060: 7573 696e 6720 5245 5354 436c 6965 6e74  using RESTClient
+0000e070: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+0000e080: 6d65 7468 6f64 203d 3d20 2247 4554 223a  method == "GET":
+0000e090: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e0a0: 7572 6e20 7365 6c66 2e72 6573 745f 636c  urn self.rest_cl
+0000e0b0: 6965 6e74 2e47 4554 2875 726c 2c0a 2020  ient.GET(url,.  
 0000e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 7374 7265 616d 3d73 7472 6561      stream=strea
-0000e0f0: 6d2c 0a20 2020 2020 2020 2020 2020 2020  m,.             
+0000e0e0: 2020 2020 2020 7374 7265 616d 3d73 7472        stream=str
+0000e0f0: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
 0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e110: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-0000e120: 7574 3d74 696d 656f 7574 2c0a 2020 2020  ut=timeout,.    
+0000e110: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+0000e120: 656f 7574 3d74 696d 656f 7574 2c0a 2020  eout=timeout,.  
 0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e150: 2020 2020 6865 6164 6572 733d 6865 6164      headers=head
-0000e160: 6572 7329 0a20 2020 2020 2020 2065 6c69  ers).        eli
-0000e170: 6620 6d65 7468 6f64 203d 3d20 2248 4541  f method == "HEA
-0000e180: 4422 3a0a 2020 2020 2020 2020 2020 2020  D":.            
-0000e190: 7265 7475 726e 2073 656c 662e 7265 7374  return self.rest
-0000e1a0: 5f63 6c69 656e 742e 4845 4144 2875 726c  _client.HEAD(url
-0000e1b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e150: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
+0000e160: 6164 6572 7329 0a20 2020 2020 2020 2065  aders).        e
+0000e170: 6c69 6620 6d65 7468 6f64 203d 3d20 2248  lif method == "H
+0000e180: 4541 4422 3a0a 2020 2020 2020 2020 2020  EAD":.          
+0000e190: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
+0000e1a0: 7374 5f63 6c69 656e 742e 4845 4144 2875  st_client.HEAD(u
+0000e1b0: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
 0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1d0: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-0000e1e0: 6d3d 7374 7265 616d 2c0a 2020 2020 2020  m=stream,.      
+0000e1d0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000e1e0: 6561 6d3d 7374 7265 616d 2c0a 2020 2020  eam=stream,.    
 0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e210: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
-0000e220: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
+0000e210: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
+0000e220: 656f 7574 2c0a 2020 2020 2020 2020 2020  eout,.          
 0000e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e240: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-0000e250: 6465 7273 3d68 6561 6465 7273 290a 2020  ders=headers).  
-0000e260: 2020 2020 2020 656c 6966 206d 6574 686f        elif metho
-0000e270: 6420 3d3d 2022 4f50 5449 4f4e 5322 3a0a  d == "OPTIONS":.
-0000e280: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000e290: 726e 2073 656c 662e 7265 7374 5f63 6c69  rn self.rest_cli
-0000e2a0: 656e 742e 4f50 5449 4f4e 5328 7572 6c2c  ent.OPTIONS(url,
-0000e2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e240: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000e250: 6561 6465 7273 3d68 6561 6465 7273 290a  eaders=headers).
+0000e260: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
+0000e270: 686f 6420 3d3d 2022 4f50 5449 4f4e 5322  hod == "OPTIONS"
+0000e280: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e290: 7475 726e 2073 656c 662e 7265 7374 5f63  turn self.rest_c
+0000e2a0: 6c69 656e 742e 4f50 5449 4f4e 5328 7572  lient.OPTIONS(ur
+0000e2b0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
 0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2d0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-0000e2e0: 6465 7273 3d68 6561 6465 7273 2c0a 2020  ders=headers,.  
+0000e2d0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000e2e0: 6561 6465 7273 3d68 6561 6465 7273 2c0a  eaders=headers,.
 0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e310: 2020 2020 2020 2020 2020 6669 656c 6473            fields
-0000e320: 3d66 6965 6c64 732c 0a20 2020 2020 2020  =fields,.       
+0000e310: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+0000e320: 6473 3d66 6965 6c64 732c 0a20 2020 2020  ds=fields,.     
 0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e350: 2020 2020 2073 7472 6561 6d3d 7374 7265       stream=stre
-0000e360: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
+0000e350: 2020 2020 2020 2073 7472 6561 6d3d 7374         stream=st
+0000e360: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
 0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
-0000e3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e390: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+0000e3a0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
 0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
-0000e3d0: 793d 626f 6479 290a 2020 2020 2020 2020  y=body).        
-0000e3e0: 656c 6966 206d 6574 686f 6420 3d3d 2022  elif method == "
-0000e3f0: 504f 5354 223a 0a20 2020 2020 2020 2020  POST":.         
-0000e400: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
-0000e410: 6573 745f 636c 6965 6e74 2e50 4f53 5428  est_client.POST(
-0000e420: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000e3d0: 6f64 793d 626f 6479 290a 2020 2020 2020  ody=body).      
+0000e3e0: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
+0000e3f0: 2022 504f 5354 223a 0a20 2020 2020 2020   "POST":.       
+0000e400: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000e410: 2e72 6573 745f 636c 6965 6e74 2e50 4f53  .rest_client.POS
+0000e420: 5428 7572 6c2c 0a20 2020 2020 2020 2020  T(url,.         
 0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e440: 2020 2020 2020 2020 2020 2020 2020 6865                he
-0000e450: 6164 6572 733d 6865 6164 6572 732c 0a20  aders=headers,. 
-0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e450: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
+0000e460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e480: 2020 2020 2020 2020 6669 656c 6473 3d66          fields=f
-0000e490: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+0000e480: 2020 2020 2020 2020 2020 6669 656c 6473            fields
+0000e490: 3d66 6965 6c64 732c 0a20 2020 2020 2020  =fields,.       
 0000e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4c0: 7374 7265 616d 3d73 7472 6561 6d2c 0a20  stream=stream,. 
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 7374 7265 616d 3d73 7472 6561 6d2c    stream=stream,
+0000e4d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 2020 2020 2020 2020 7469 6d65 6f75 743d          timeout=
-0000e500: 7469 6d65 6f75 742c 0a20 2020 2020 2020  timeout,.       
+0000e4f0: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
+0000e500: 743d 7469 6d65 6f75 742c 0a20 2020 2020  t=timeout,.     
 0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e530: 2020 626f 6479 3d62 6f64 7929 0a20 2020    body=body).   
-0000e540: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
-0000e550: 203d 3d20 2250 5554 223a 0a20 2020 2020   == "PUT":.     
-0000e560: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e570: 6c66 2e72 6573 745f 636c 6965 6e74 2e50  lf.rest_client.P
-0000e580: 5554 2875 726c 2c0a 2020 2020 2020 2020  UT(url,.        
+0000e530: 2020 2020 626f 6479 3d62 6f64 7929 0a20      body=body). 
+0000e540: 2020 2020 2020 2065 6c69 6620 6d65 7468         elif meth
+0000e550: 6f64 203d 3d20 2250 5554 223a 0a20 2020  od == "PUT":.   
+0000e560: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e570: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
+0000e580: 2e50 5554 2875 726c 2c0a 2020 2020 2020  .PUT(url,.      
 0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5b0: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
-0000e5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e5b0: 2020 6865 6164 6572 733d 6865 6164 6572    headers=header
+0000e5c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
 0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2020 2020 2020 2020 2066 6965 6c64 733d           fields=
-0000e5f0: 6669 656c 6473 2c0a 2020 2020 2020 2020  fields,.        
+0000e5e0: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+0000e5f0: 733d 6669 656c 6473 2c0a 2020 2020 2020  s=fields,.      
 0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e620: 7374 7265 616d 3d73 7472 6561 6d2c 0a20  stream=stream,. 
-0000e630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 7374 7265 616d 3d73 7472 6561 6d2c    stream=stream,
+0000e630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
-0000e660: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
+0000e650: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0000e660: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
 0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e690: 626f 6479 3d62 6f64 7929 0a20 2020 2020  body=body).     
-0000e6a0: 2020 2065 6c69 6620 6d65 7468 6f64 203d     elif method =
-0000e6b0: 3d20 2250 4154 4348 223a 0a20 2020 2020  = "PATCH":.     
-0000e6c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000e6d0: 6c66 2e72 6573 745f 636c 6965 6e74 2e50  lf.rest_client.P
-0000e6e0: 4154 4348 2875 726c 2c0a 2020 2020 2020  ATCH(url,.      
+0000e690: 2020 626f 6479 3d62 6f64 7929 0a20 2020    body=body).   
+0000e6a0: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
+0000e6b0: 203d 3d20 2250 4154 4348 223a 0a20 2020   == "PATCH":.   
+0000e6c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e6d0: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
+0000e6e0: 2e50 4154 4348 2875 726c 2c0a 2020 2020  .PATCH(url,.    
 0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 2020 2020 6865 6164 6572 733d 6865 6164      headers=head
-0000e720: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
+0000e710: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
+0000e720: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
 0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e740: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e750: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
 0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e780: 2020 2020 2020 2020 7374 7265 616d 3d73          stream=s
-0000e790: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
+0000e780: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+0000e790: 3d73 7472 6561 6d2c 0a20 2020 2020 2020  =stream,.       
 0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7c0: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
-0000e7d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e7c0: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
+0000e7d0: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
 0000e7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7f0: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0000e800: 3d62 6f64 7929 0a20 2020 2020 2020 2065  =body).        e
-0000e810: 6c69 6620 6d65 7468 6f64 203d 3d20 2244  lif method == "D
-0000e820: 454c 4554 4522 3a0a 2020 2020 2020 2020  ELETE":.        
-0000e830: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000e840: 7265 7374 5f63 6c69 656e 742e 4445 4c45  rest_client.DELE
-0000e850: 5445 2875 726c 2c0a 2020 2020 2020 2020  TE(url,.        
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+0000e800: 6479 3d62 6f64 7929 0a20 2020 2020 2020  dy=body).       
+0000e810: 2065 6c69 6620 6d65 7468 6f64 203d 3d20   elif method == 
+0000e820: 2244 454c 4554 4522 3a0a 2020 2020 2020  "DELETE":.      
+0000e830: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000e840: 662e 7265 7374 5f63 6c69 656e 742e 4445  f.rest_client.DE
+0000e850: 4c45 5445 2875 726c 2c0a 2020 2020 2020  LETE(url,.      
 0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e880: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
-0000e890: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000e880: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
+0000e890: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
 0000e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e8c0: 7472 6561 6d3d 7374 7265 616d 2c0a 2020  tream=stream,.  
+0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8c0: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
 0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8f0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-0000e900: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
+0000e8f0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+0000e900: 7574 3d74 696d 656f 7574 2c0a 2020 2020  ut=timeout,.    
 0000e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e930: 2020 2020 2062 6f64 793d 626f 6479 290a       body=body).
-0000e940: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e950: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000e960: 4170 6956 616c 7565 4572 726f 7228 0a20  ApiValueError(. 
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e980: 6874 7470 206d 6574 686f 6420 6d75 7374  http method must
-0000e990: 2062 6520 6047 4554 602c 2060 4845 4144   be `GET`, `HEAD
-0000e9a0: 602c 2060 4f50 5449 4f4e 5360 2c22 0a20  `, `OPTIONS`,". 
-0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e9c0: 2060 504f 5354 602c 2060 5041 5443 4860   `POST`, `PATCH`
-0000e9d0: 2c20 6050 5554 6020 6f72 2060 4445 4c45  , `PUT` or `DELE
-0000e9e0: 5445 602e 220a 2020 2020 2020 2020 2020  TE`.".          
-0000e9f0: 2020 290a 0a20 2020 2064 6566 2075 7064    )..    def upd
-0000ea00: 6174 655f 7061 7261 6d73 5f66 6f72 5f61  ate_params_for_a
-0000ea10: 7574 6828 0a20 2020 2020 2020 2020 2020  uth(.           
-0000ea20: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0000ea30: 2020 2068 6561 6465 7273 2c0a 2020 2020     headers,.    
-0000ea40: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
-0000ea50: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-0000ea60: 2020 2072 6573 6f75 7263 655f 7061 7468     resource_path
-0000ea70: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-0000ea80: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
-0000ea90: 2020 626f 6479 2c0a 2020 2020 2020 2020    body,.        
-0000eaa0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
-0000eab0: 6174 6f72 5f69 7465 7261 746f 723a 2050  ator_iterator: P
-0000eac0: 7265 6669 7853 6570 6172 6174 6f72 4974  refixSeparatorIt
-0000ead0: 6572 6174 6f72 203d 204e 6f6e 650a 2020  erator = None.  
-0000eae0: 2020 2020 2020 2920 2d3e 2073 7472 3a0a        ) -> str:.
-0000eaf0: 2020 2020 2020 2020 2222 2255 7064 6174          """Updat
-0000eb00: 6573 2068 6561 6465 7220 616e 6420 7175  es header and qu
-0000eb10: 6572 7920 7061 7261 6d73 2062 6173 6564  ery params based
-0000eb20: 206f 6e20 6175 7468 656e 7469 6361 7469   on authenticati
-0000eb30: 6f6e 2073 6574 7469 6e67 2e0a 0a20 2020  on setting...   
-0000eb40: 2020 2020 203a 7061 7261 6d20 6865 6164       :param head
-0000eb50: 6572 733a 2048 6561 6465 7220 7061 7261  ers: Header para
-0000eb60: 6d65 7465 7273 2064 6963 7420 746f 2062  meters dict to b
-0000eb70: 6520 7570 6461 7465 642e 0a20 2020 2020  e updated..     
-0000eb80: 2020 203a 7061 7261 6d20 6175 7468 5f73     :param auth_s
-0000eb90: 6574 7469 6e67 733a 2041 7574 6865 6e74  ettings: Authent
-0000eba0: 6963 6174 696f 6e20 7365 7474 696e 6720  ication setting 
-0000ebb0: 6964 656e 7469 6669 6572 7320 6c69 7374  identifiers list
-0000ebc0: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000ebd0: 2072 6573 6f75 7263 655f 7061 7468 3a20   resource_path: 
-0000ebe0: 4120 7374 7269 6e67 2072 6570 7265 7365  A string represe
-0000ebf0: 6e74 6174 696f 6e20 6f66 2074 6865 2048  ntation of the H
-0000ec00: 5454 5020 7265 7175 6573 7420 7265 736f  TTP request reso
-0000ec10: 7572 6365 2070 6174 682e 0a20 2020 2020  urce path..     
-0000ec20: 2020 203a 7061 7261 6d20 6d65 7468 6f64     :param method
-0000ec30: 3a20 4120 7374 7269 6e67 2072 6570 7265  : A string repre
-0000ec40: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
-0000ec50: 2048 5454 5020 7265 7175 6573 7420 6d65   HTTP request me
-0000ec60: 7468 6f64 2e0a 2020 2020 2020 2020 3a70  thod..        :p
-0000ec70: 6172 616d 2062 6f64 793a 2041 206f 626a  aram body: A obj
-0000ec80: 6563 7420 7265 7072 6573 656e 7469 6e67  ect representing
-0000ec90: 2074 6865 2062 6f64 7920 6f66 2074 6865   the body of the
-0000eca0: 2048 5454 5020 7265 7175 6573 742e 0a20   HTTP request.. 
-0000ecb0: 2020 2020 2020 2020 2020 2054 6865 206f             The o
-0000ecc0: 626a 6563 7420 7479 7065 2069 7320 7468  bject type is th
-0000ecd0: 6520 7265 7475 726e 2076 616c 7565 206f  e return value o
-0000ece0: 6620 5f65 6e63 6f64 6572 2e64 6566 6175  f _encoder.defau
-0000ecf0: 6c74 2829 2e0a 2020 2020 2020 2020 2222  lt()..        ""
-0000ed00: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
-0000ed10: 2061 7574 685f 7365 7474 696e 6773 3a0a   auth_settings:.
-0000ed20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ed30: 726e 2072 6573 6f75 7263 655f 7061 7468  rn resource_path
-0000ed40: 0a20 2020 2020 2020 2069 6620 7072 6566  .        if pref
-0000ed50: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-0000ed60: 7261 746f 7220 6973 204e 6f6e 653a 0a20  rator is None:. 
-0000ed70: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-0000ed80: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-0000ed90: 6174 6f72 203d 2050 7265 6669 7853 6570  ator = PrefixSep
-0000eda0: 6172 6174 6f72 4974 6572 6174 6f72 2822  aratorIterator("
-0000edb0: 3f22 2c20 2226 2229 0a0a 2020 2020 2020  ?", "&")..      
-0000edc0: 2020 666f 7220 6175 7468 2069 6e20 6175    for auth in au
-0000edd0: 7468 5f73 6574 7469 6e67 733a 0a20 2020  th_settings:.   
-0000ede0: 2020 2020 2020 2020 2061 7574 685f 7365           auth_se
-0000edf0: 7474 696e 6720 3d20 7365 6c66 2e63 6f6e  tting = self.con
-0000ee00: 6669 6775 7261 7469 6f6e 2e61 7574 685f  figuration.auth_
-0000ee10: 7365 7474 696e 6773 2829 2e67 6574 2861  settings().get(a
-0000ee20: 7574 6829 0a20 2020 2020 2020 2020 2020  uth).           
-0000ee30: 2069 6620 6e6f 7420 6175 7468 5f73 6574   if not auth_set
-0000ee40: 7469 6e67 3a0a 2020 2020 2020 2020 2020  ting:.          
-0000ee50: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0000ee60: 2020 2020 2020 2020 2020 2069 6620 6175             if au
-0000ee70: 7468 5f73 6574 7469 6e67 5b27 696e 275d  th_setting['in']
-0000ee80: 203d 3d20 2763 6f6f 6b69 6527 3a0a 2020   == 'cookie':.  
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 6865                he
-0000eea0: 6164 6572 732e 6164 6428 2743 6f6f 6b69  aders.add('Cooki
-0000eeb0: 6527 2c20 6175 7468 5f73 6574 7469 6e67  e', auth_setting
-0000eec0: 5b27 7661 6c75 6527 5d29 0a20 2020 2020  ['value']).     
-0000eed0: 2020 2020 2020 2065 6c69 6620 6175 7468         elif auth
-0000eee0: 5f73 6574 7469 6e67 5b27 696e 275d 203d  _setting['in'] =
-0000eef0: 3d20 2768 6561 6465 7227 3a0a 2020 2020  = 'header':.    
-0000ef00: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0000ef10: 7574 685f 7365 7474 696e 675b 2774 7970  uth_setting['typ
-0000ef20: 6527 5d20 213d 2027 6874 7470 2d73 6967  e'] != 'http-sig
-0000ef30: 6e61 7475 7265 273a 0a20 2020 2020 2020  nature':.       
-0000ef40: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-0000ef50: 6465 7273 2e61 6464 2861 7574 685f 7365  ders.add(auth_se
-0000ef60: 7474 696e 675b 276b 6579 275d 2c20 6175  tting['key'], au
-0000ef70: 7468 5f73 6574 7469 6e67 5b27 7661 6c75  th_setting['valu
-0000ef80: 6527 5d29 0a20 2020 2020 2020 2020 2020  e']).           
-0000ef90: 2065 6c69 6620 6175 7468 5f73 6574 7469   elif auth_setti
-0000efa0: 6e67 5b27 696e 275d 203d 3d20 2771 7565  ng['in'] == 'que
-0000efb0: 7279 273a 0a20 2020 2020 2020 2020 2020  ry':.           
-0000efc0: 2020 2020 2022 2222 2054 4f44 4f20 696d       """ TODO im
-0000efd0: 706c 656d 656e 7420 6175 7468 2069 6e20  plement auth in 
-0000efe0: 7175 6572 790a 2020 2020 2020 2020 2020  query.          
-0000eff0: 2020 2020 2020 6e65 6564 2074 6f20 7061        need to pa
-0000f000: 7373 2069 6e20 7072 6566 6978 5f73 6570  ss in prefix_sep
-0000f010: 6172 6174 6f72 5f69 7465 7261 746f 720a  arator_iterator.
-0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f030: 616e 6420 6e65 6564 2074 6f20 6f75 7470  and need to outp
-0000f040: 7574 2072 6573 6f75 7263 655f 7061 7468  ut resource_path
-0000f050: 2077 6974 6820 7175 6572 7920 7061 7261   with query para
-0000f060: 6d73 2061 6464 6564 0a20 2020 2020 2020  ms added.       
-0000f070: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
-0000f080: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000f090: 6f75 7263 655f 7061 7468 202b 3d20 5061  ource_path += Pa
-0000f0a0: 7261 6d65 7465 7253 6572 6961 6c69 7a65  rameterSerialize
-0000f0b0: 7242 6173 652e 5f72 6566 3635 3730 5f65  rBase._ref6570_e
-0000f0c0: 7870 616e 7369 6f6e 280a 2020 2020 2020  xpansion(.      
-0000f0d0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000f0e0: 7269 6162 6c65 5f6e 616d 653d 6175 7468  riable_name=auth
-0000f0f0: 5f73 6574 7469 6e67 5b27 6b65 7927 5d2c  _setting['key'],
-0000f100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f110: 2020 2020 2069 6e5f 6461 7461 3d61 7574       in_data=aut
-0000f120: 685f 7365 7474 696e 675b 2776 616c 7565  h_setting['value
-0000f130: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-0000f140: 2020 2020 2020 2020 6578 706c 6f64 653d          explode=
-0000f150: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0000f160: 2020 2020 2020 2020 2020 2070 6572 6365             perce
-0000f170: 6e74 5f65 6e63 6f64 653d 4661 6c73 652c  nt_encode=False,
-0000f180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f190: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-0000f1a0: 7261 746f 725f 6974 6572 6174 6f72 3d70  rator_iterator=p
-0000f1b0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-0000f1c0: 6974 6572 6174 6f72 0a20 2020 2020 2020  iterator.       
-0000f1d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000f1e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000f1f0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000f200: 7365 2041 7069 5661 6c75 6545 7272 6f72  se ApiValueError
-0000f210: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f220: 2020 2020 2020 2741 7574 6865 6e74 6963        'Authentic
-0000f230: 6174 696f 6e20 746f 6b65 6e20 6d75 7374  ation token must
-0000f240: 2062 6520 696e 2060 7175 6572 7960 206f   be in `query` o
-0000f250: 7220 6068 6561 6465 7260 270a 2020 2020  r `header`'.    
-0000f260: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000f270: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000f280: 6f75 7263 655f 7061 7468 0a0a 0a63 6c61  ource_path...cla
-0000f290: 7373 2041 7069 3a0a 2020 2020 2222 224e  ss Api:.    """N
-0000f2a0: 4f54 453a 0a20 2020 2054 6869 7320 636c  OTE:.    This cl
-0000f2b0: 6173 7320 6973 2061 7574 6f20 6765 6e65  ass is auto gene
-0000f2c0: 7261 7465 6420 6279 204b 6f6e 6669 6720  rated by Konfig 
-0000f2d0: 2868 7474 7073 3a2f 2f6b 6f6e 6669 6774  (https://konfigt
-0000f2e0: 6869 732e 636f 6d29 0a20 2020 2022 2222  his.com).    """
-0000f2f0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0000f300: 5f5f 2873 656c 662c 2061 7069 5f63 6c69  __(self, api_cli
-0000f310: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
-0000f320: 6f6e 616c 5b41 7069 436c 6965 6e74 5d20  onal[ApiClient] 
-0000f330: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0000f340: 2069 6620 6170 695f 636c 6965 6e74 2069   if api_client i
-0000f350: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000f360: 2020 2020 6170 695f 636c 6965 6e74 203d      api_client =
-0000f370: 2041 7069 436c 6965 6e74 2829 0a20 2020   ApiClient().   
-0000f380: 2020 2020 2073 656c 662e 6170 695f 636c       self.api_cl
-0000f390: 6965 6e74 203d 2061 7069 5f63 6c69 656e  ient = api_clien
-0000f3a0: 740a 0a20 2020 2040 7374 6174 6963 6d65  t..    @staticme
-0000f3b0: 7468 6f64 0a20 2020 2064 6566 205f 7665  thod.    def _ve
-0000f3c0: 7269 6679 5f74 7970 6564 5f64 6963 745f  rify_typed_dict_
-0000f3d0: 696e 7075 7473 5f6f 6170 6728 636c 733a  inputs_oapg(cls:
-0000f3e0: 2074 7970 696e 672e 5479 7065 5b74 7970   typing.Type[typ
-0000f3f0: 696e 675f 6578 7465 6e73 696f 6e73 2e54  ing_extensions.T
-0000f400: 7970 6564 4469 6374 5d2c 2064 6174 613a  ypedDict], data:
-0000f410: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-0000f420: 2c20 7479 7069 6e67 2e41 6e79 5d29 3a0a  , typing.Any]):.
-0000f430: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f440: 2020 2020 456e 7375 7265 7320 7468 6174      Ensures that
-0000f450: 3a0a 2020 2020 2020 2020 2d20 7265 7175  :.        - requ
-0000f460: 6972 6564 206b 6579 7320 6172 6520 7072  ired keys are pr
-0000f470: 6573 656e 740a 2020 2020 2020 2020 2d20  esent.        - 
-0000f480: 6164 6469 7469 6f6e 616c 2070 726f 7065  additional prope
-0000f490: 7274 6965 7320 6172 6520 6e6f 7420 696e  rties are not in
-0000f4a0: 7075 740a 2020 2020 2020 2020 2d20 7661  put.        - va
-0000f4b0: 6c75 6520 7374 6f72 6564 2075 6e64 6572  lue stored under
-0000f4c0: 2072 6571 7569 7265 6420 6b65 7973 2064   required keys d
-0000f4d0: 6f20 6e6f 7420 6861 7665 2074 6865 2076  o not have the v
-0000f4e0: 616c 7565 2075 6e73 6574 0a20 2020 2020  alue unset.     
-0000f4f0: 2020 204e 6f74 653a 2064 6574 6169 6c65     Note: detaile
-0000f500: 6420 7661 6c75 6520 6368 6563 6b69 6e67  d value checking
-0000f510: 2069 7320 646f 6e65 2069 6e20 7363 6865   is done in sche
-0000f520: 6d61 2063 6c61 7373 6573 0a20 2020 2020  ma classes.     
-0000f530: 2020 2022 2222 0a20 2020 2020 2020 206d     """.        m
-0000f540: 6973 7369 6e67 5f72 6571 7569 7265 645f  issing_required_
-0000f550: 6b65 7973 203d 205b 5d0a 2020 2020 2020  keys = [].      
-0000f560: 2020 7265 7175 6972 6564 5f6b 6579 735f    required_keys_
-0000f570: 7769 7468 5f75 6e73 6574 5f76 616c 7565  with_unset_value
-0000f580: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0000f590: 6f72 2072 6571 7569 7265 645f 6b65 7920  or required_key 
-0000f5a0: 696e 2063 6c73 2e5f 5f72 6571 7569 7265  in cls.__require
-0000f5b0: 645f 6b65 7973 5f5f 3a0a 2020 2020 2020  d_keys__:.      
-0000f5c0: 2020 2020 2020 6966 2072 6571 7569 7265        if require
-0000f5d0: 645f 6b65 7920 6e6f 7420 696e 2064 6174  d_key not in dat
-0000f5e0: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-0000f5f0: 2020 206d 6973 7369 6e67 5f72 6571 7569     missing_requi
-0000f600: 7265 645f 6b65 7973 2e61 7070 656e 6428  red_keys.append(
-0000f610: 7265 7175 6972 6564 5f6b 6579 290a 2020  required_key).  
-0000f620: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f630: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0000f640: 2020 2076 616c 7565 203d 2064 6174 615b     value = data[
-0000f650: 7265 7175 6972 6564 5f6b 6579 5d0a 2020  required_key].  
-0000f660: 2020 2020 2020 2020 2020 6966 2076 616c            if val
-0000f670: 7565 2069 7320 756e 7365 743a 0a20 2020  ue is unset:.   
-0000f680: 2020 2020 2020 2020 2020 2020 2072 6571               req
-0000f690: 7569 7265 645f 6b65 7973 5f77 6974 685f  uired_keys_with_
-0000f6a0: 756e 7365 745f 7661 6c75 6573 2e61 7070  unset_values.app
-0000f6b0: 656e 6428 7265 7175 6972 6564 5f6b 6579  end(required_key
-0000f6c0: 290a 2020 2020 2020 2020 6966 206d 6973  ).        if mis
-0000f6d0: 7369 6e67 5f72 6571 7569 7265 645f 6b65  sing_required_ke
-0000f6e0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-0000f6f0: 7261 6973 6520 4170 6954 7970 6545 7272  raise ApiTypeErr
-0000f700: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000f710: 2020 2020 277b 7d20 6d69 7373 696e 6720      '{} missing 
-0000f720: 7b7d 2072 6571 7569 7265 6420 6172 6775  {} required argu
-0000f730: 6d65 6e74 733a 207b 7d27 2e66 6f72 6d61  ments: {}'.forma
-0000f740: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000f750: 2020 2020 2020 2063 6c73 2e5f 5f6e 616d         cls.__nam
-0000f760: 655f 5f2c 206c 656e 286d 6973 7369 6e67  e__, len(missing
-0000f770: 5f72 6571 7569 7265 645f 6b65 7973 292c  _required_keys),
-0000f780: 206d 6973 7369 6e67 5f72 6571 7569 7265   missing_require
-0000f790: 645f 6b65 7973 0a20 2020 2020 2020 2020  d_keys.         
-0000f7a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000f7b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000f7c0: 2069 6620 7265 7175 6972 6564 5f6b 6579   if required_key
-0000f7d0: 735f 7769 7468 5f75 6e73 6574 5f76 616c  s_with_unset_val
-0000f7e0: 7565 733a 0a20 2020 2020 2020 2020 2020  ues:.           
-0000f7f0: 2072 6169 7365 2041 7069 5661 6c75 6545   raise ApiValueE
-0000f800: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-0000f810: 2020 2020 2020 277b 7d20 636f 6e74 6169        '{} contai
-0000f820: 6e73 2069 6e76 616c 6964 2075 6e73 6574  ns invalid unset
-0000f830: 2076 616c 7565 7320 666f 7220 7b7d 2072   values for {} r
-0000f840: 6571 7569 7265 6420 6b65 7973 3a20 7b7d  equired keys: {}
-0000f850: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
-0000f860: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-0000f870: 732e 5f5f 6e61 6d65 5f5f 2c20 6c65 6e28  s.__name__, len(
-0000f880: 7265 7175 6972 6564 5f6b 6579 735f 7769  required_keys_wi
-0000f890: 7468 5f75 6e73 6574 5f76 616c 7565 7329  th_unset_values)
-0000f8a0: 2c20 7265 7175 6972 6564 5f6b 6579 735f  , required_keys_
-0000f8b0: 7769 7468 5f75 6e73 6574 5f76 616c 7565  with_unset_value
-0000f8c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000f8d0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000f8e0: 290a 0a20 2020 2020 2020 2064 6973 616c  )..        disal
-0000f8f0: 6c6f 7765 645f 6164 6469 7469 6f6e 616c  lowed_additional
-0000f900: 5f6b 6579 7320 3d20 5b5d 0a20 2020 2020  _keys = [].     
-0000f910: 2020 2066 6f72 206b 6579 2069 6e20 6461     for key in da
-0000f920: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-0000f930: 6966 206b 6579 2069 6e20 636c 732e 5f5f  if key in cls.__
-0000f940: 7265 7175 6972 6564 5f6b 6579 735f 5f20  required_keys__ 
-0000f950: 6f72 206b 6579 2069 6e20 636c 732e 5f5f  or key in cls.__
-0000f960: 6f70 7469 6f6e 616c 5f6b 6579 735f 5f3a  optional_keys__:
-0000f970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f980: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000f990: 2020 2020 2020 6469 7361 6c6c 6f77 6564        disallowed
-0000f9a0: 5f61 6464 6974 696f 6e61 6c5f 6b65 7973  _additional_keys
-0000f9b0: 2e61 7070 656e 6428 6b65 7929 0a20 2020  .append(key).   
-0000f9c0: 2020 2020 2069 6620 6469 7361 6c6c 6f77       if disallow
-0000f9d0: 6564 5f61 6464 6974 696f 6e61 6c5f 6b65  ed_additional_ke
-0000f9e0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-0000f9f0: 7261 6973 6520 4170 6954 7970 6545 7272  raise ApiTypeErr
-0000fa00: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000fa10: 2020 2020 277b 7d20 676f 7420 7b7d 2075      '{} got {} u
-0000fa20: 6e65 7870 6563 7465 6420 6b65 7977 6f72  nexpected keywor
-0000fa30: 6420 6172 6775 6d65 6e74 733a 207b 7d27  d arguments: {}'
-0000fa40: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0000fa50: 2020 2020 2020 2020 2020 2020 2063 6c73               cls
-0000fa60: 2e5f 5f6e 616d 655f 5f2c 206c 656e 2864  .__name__, len(d
-0000fa70: 6973 616c 6c6f 7765 645f 6164 6469 7469  isallowed_additi
-0000fa80: 6f6e 616c 5f6b 6579 7329 2c20 6469 7361  onal_keys), disa
-0000fa90: 6c6c 6f77 6564 5f61 6464 6974 696f 6e61  llowed_additiona
-0000faa0: 6c5f 6b65 7973 0a20 2020 2020 2020 2020  l_keys.         
-0000fab0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000fac0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000fad0: 5f67 6574 5f68 6f73 745f 6f61 7067 280a  _get_host_oapg(.
-0000fae0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000faf0: 2020 2020 2020 6f70 6572 6174 696f 6e5f        operation_
-0000fb00: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
-0000fb10: 2073 6572 7665 7273 3a20 7479 7069 6e67   servers: typing
-0000fb20: 2e54 7570 6c65 5b74 7970 696e 672e 4469  .Tuple[typing.Di
-0000fb30: 6374 5b73 7472 2c20 7374 725d 2c20 2e2e  ct[str, str], ..
-0000fb40: 2e5d 203d 2074 7570 6c65 2829 2c0a 2020  .] = tuple(),.  
-0000fb50: 2020 2020 2020 686f 7374 5f69 6e64 6578        host_index
-0000fb60: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000fb70: 6c5b 696e 745d 203d 204e 6f6e 650a 2020  l[int] = None.  
-0000fb80: 2020 2920 2d3e 2074 7970 696e 672e 4f70    ) -> typing.Op
-0000fb90: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
-0000fba0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-0000fbb0: 6f6e 203d 2073 656c 662e 6170 695f 636c  on = self.api_cl
-0000fbc0: 6965 6e74 2e63 6f6e 6669 6775 7261 7469  ient.configurati
-0000fbd0: 6f6e 0a20 2020 2020 2020 2074 7279 3a0a  on.        try:.
-0000fbe0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-0000fbf0: 6f73 745f 696e 6465 7820 6973 204e 6f6e  ost_index is Non
-0000fc00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000fc10: 2020 2069 6e64 6578 203d 2063 6f6e 6669     index = confi
-0000fc20: 6775 7261 7469 6f6e 2e73 6572 7665 725f  guration.server_
-0000fc30: 6f70 6572 6174 696f 6e5f 696e 6465 782e  operation_index.
-0000fc40: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-0000fc50: 2020 2020 2020 2020 206f 7065 7261 7469           operati
-0000fc60: 6f6e 5f69 642c 2063 6f6e 6669 6775 7261  on_id, configura
-0000fc70: 7469 6f6e 2e73 6572 7665 725f 696e 6465  tion.server_inde
-0000fc80: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
-0000fc90: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000fca0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000fcb0: 2020 2020 2020 696e 6465 7820 3d20 686f        index = ho
-0000fcc0: 7374 5f69 6e64 6578 0a20 2020 2020 2020  st_index.       
-0000fcd0: 2020 2020 2073 6572 7665 725f 7661 7269       server_vari
-0000fce0: 6162 6c65 7320 3d20 636f 6e66 6967 7572  ables = configur
-0000fcf0: 6174 696f 6e2e 7365 7276 6572 5f6f 7065  ation.server_ope
-0000fd00: 7261 7469 6f6e 5f76 6172 6961 626c 6573  ration_variables
-0000fd10: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-0000fd20: 2020 2020 2020 6f70 6572 6174 696f 6e5f        operation_
-0000fd30: 6964 2c20 636f 6e66 6967 7572 6174 696f  id, configuratio
-0000fd40: 6e2e 7365 7276 6572 5f76 6172 6961 626c  n.server_variabl
-0000fd50: 6573 0a20 2020 2020 2020 2020 2020 2029  es.            )
-0000fd60: 0a20 2020 2020 2020 2020 2020 2068 6f73  .            hos
-0000fd70: 7420 3d20 636f 6e66 6967 7572 6174 696f  t = configuratio
-0000fd80: 6e2e 6765 745f 686f 7374 5f66 726f 6d5f  n.get_host_from_
-0000fd90: 7365 7474 696e 6773 280a 2020 2020 2020  settings(.      
-0000fda0: 2020 2020 2020 2020 2020 696e 6465 782c            index,
-0000fdb0: 2076 6172 6961 626c 6573 3d73 6572 7665   variables=serve
-0000fdc0: 725f 7661 7269 6162 6c65 732c 2073 6572  r_variables, ser
-0000fdd0: 7665 7273 3d73 6572 7665 7273 0a20 2020  vers=servers.   
-0000fde0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000fdf0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
-0000fe00: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-0000fe10: 2020 6966 2073 6572 7665 7273 3a0a 2020    if servers:.  
-0000fe20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000fe30: 6973 6520 4170 6956 616c 7565 4572 726f  ise ApiValueErro
-0000fe40: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000fe50: 2020 2020 2020 2022 496e 7661 6c69 6420         "Invalid 
-0000fe60: 686f 7374 2069 6e64 6578 2e20 4d75 7374  host index. Must
-0000fe70: 2062 6520 3020 3c3d 2069 6e64 6578 203c   be 0 <= index <
-0000fe80: 2025 7322 2025 0a20 2020 2020 2020 2020   %s" %.         
-0000fe90: 2020 2020 2020 2020 2020 206c 656e 2873             len(s
-0000fea0: 6572 7665 7273 290a 2020 2020 2020 2020  ervers).        
-0000feb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000fec0: 2020 2020 2020 686f 7374 203d 204e 6f6e        host = Non
-0000fed0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000fee0: 2068 6f73 740a 0a0a 636c 6173 7320 5365   host...class Se
-0000fef0: 7269 616c 697a 6564 5265 7175 6573 7442  rializedRequestB
-0000ff00: 6f64 7928 7479 7069 6e67 5f65 7874 656e  ody(typing_exten
-0000ff10: 7369 6f6e 732e 5479 7065 6444 6963 742c  sions.TypedDict,
-0000ff20: 2074 6f74 616c 3d46 616c 7365 293a 0a20   total=False):. 
-0000ff30: 2020 2062 6f64 793a 2074 7970 696e 672e     body: typing.
-0000ff40: 556e 696f 6e5b 7374 722c 2062 7974 6573  Union[str, bytes
-0000ff50: 5d0a 2020 2020 6669 656c 6473 3a20 7479  ].    fields: ty
-0000ff60: 7069 6e67 2e54 7570 6c65 5b74 7970 696e  ping.Tuple[typin
-0000ff70: 672e 556e 696f 6e5b 5265 7175 6573 7446  g.Union[RequestF
-0000ff80: 6965 6c64 2c20 7479 7069 6e67 2e54 7570  ield, typing.Tup
-0000ff90: 6c65 5b73 7472 2c20 7374 725d 5d2c 202e  le[str, str]], .
-0000ffa0: 2e2e 5d0a 0a0a 636c 6173 7320 5265 7175  ..]...class Requ
-0000ffb0: 6573 7442 6f64 7928 5374 796c 6546 6f72  estBody(StyleFor
-0000ffc0: 6d53 6572 6961 6c69 7a65 722c 204a 534f  mSerializer, JSO
-0000ffd0: 4e44 6574 6563 746f 7229 3a0a 2020 2020  NDetector):.    
-0000ffe0: 2222 220a 2020 2020 4120 7265 7175 6573  """.    A reques
-0000fff0: 7420 626f 6479 2070 6172 616d 6574 6572  t body parameter
-00010000: 0a20 2020 2063 6f6e 7465 6e74 3a20 636f  .    content: co
-00010010: 6e74 656e 745f 7479 7065 2074 6f20 4d65  ntent_type to Me
-00010020: 6469 6154 7970 6520 5363 6865 6d61 2069  diaType Schema i
-00010030: 6e66 6f0a 2020 2020 2222 220a 2020 2020  nfo.    """.    
-00010040: 5f5f 6a73 6f6e 5f65 6e63 6f64 6572 203d  __json_encoder =
-00010050: 204a 534f 4e45 6e63 6f64 6572 2829 0a0a   JSONEncoder()..
-00010060: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00010070: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00010080: 2020 2020 2020 2020 636f 6e74 656e 743a          content:
-00010090: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-000100a0: 2c20 4d65 6469 6154 7970 655d 2c0a 2020  , MediaType],.  
-000100b0: 2020 2020 2020 7265 7175 6972 6564 3a20        required: 
-000100c0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-000100d0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000100e0: 662e 7265 7175 6972 6564 203d 2072 6571  f.required = req
-000100f0: 7569 7265 640a 2020 2020 2020 2020 6966  uired.        if
-00010100: 206c 656e 2863 6f6e 7465 6e74 2920 3d3d   len(content) ==
-00010110: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-00010120: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00010130: 2827 496e 7661 6c69 6420 7661 6c75 6520  ('Invalid value 
-00010140: 666f 7220 636f 6e74 656e 742c 2074 6865  for content, the
-00010150: 2063 6f6e 7465 6e74 2064 6963 7420 6d75   content dict mu
-00010160: 7374 2068 6176 6520 3e3d 2031 2065 6e74  st have >= 1 ent
-00010170: 7279 2729 0a20 2020 2020 2020 2073 656c  ry').        sel
-00010180: 662e 636f 6e74 656e 7420 3d20 636f 6e74  f.content = cont
-00010190: 656e 740a 0a20 2020 2064 6566 205f 5f73  ent..    def __s
-000101a0: 6572 6961 6c69 7a65 5f6a 736f 6e28 0a20  erialize_json(. 
-000101b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000101c0: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
-000101d0: 7069 6e67 2e41 6e79 0a20 2020 2029 202d  ping.Any.    ) -
-000101e0: 3e20 7479 7069 6e67 2e44 6963 745b 7374  > typing.Dict[st
-000101f0: 722c 2062 7974 6573 5d3a 0a20 2020 2020  r, bytes]:.     
-00010200: 2020 2069 6e5f 6461 7461 203d 2073 656c     in_data = sel
-00010210: 662e 5f5f 6a73 6f6e 5f65 6e63 6f64 6572  f.__json_encoder
-00010220: 2e64 6566 6175 6c74 2869 6e5f 6461 7461  .default(in_data
-00010230: 290a 2020 2020 2020 2020 6a73 6f6e 5f73  ).        json_s
-00010240: 7472 203d 206a 736f 6e2e 6475 6d70 7328  tr = json.dumps(
-00010250: 696e 5f64 6174 612c 2073 6570 6172 6174  in_data, separat
-00010260: 6f72 733d 2822 2c22 2c20 223a 2229 2c20  ors=(",", ":"), 
-00010270: 656e 7375 7265 5f61 7363 6969 3d46 616c  ensure_ascii=Fal
-00010280: 7365 292e 656e 636f 6465 280a 2020 2020  se).encode(.    
-00010290: 2020 2020 2020 2020 2275 7466 2d38 220a          "utf-8".
-000102a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000102b0: 2020 7265 7475 726e 2064 6963 7428 626f    return dict(bo
-000102c0: 6479 3d6a 736f 6e5f 7374 7229 0a0a 2020  dy=json_str)..  
-000102d0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-000102e0: 2020 2020 6465 6620 5f5f 7365 7269 616c      def __serial
-000102f0: 697a 655f 7465 7874 5f70 6c61 696e 2869  ize_text_plain(i
-00010300: 6e5f 6461 7461 3a20 7479 7069 6e67 2e41  n_data: typing.A
-00010310: 6e79 2920 2d3e 2074 7970 696e 672e 4469  ny) -> typing.Di
-00010320: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
-00010330: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00010340: 6e63 6528 696e 5f64 6174 612c 2066 726f  nce(in_data, fro
-00010350: 7a65 6e64 6963 742e 6672 6f7a 656e 6469  zendict.frozendi
-00010360: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-00010370: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00010380: 7228 2755 6e61 626c 6520 746f 2073 6572  r('Unable to ser
-00010390: 6961 6c69 7a65 2074 7970 6520 6672 6f7a  ialize type froz
-000103a0: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
-000103b0: 7420 746f 2074 6578 742f 706c 6169 6e27  t to text/plain'
-000103c0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
-000103d0: 7369 6e73 7461 6e63 6528 696e 5f64 6174  sinstance(in_dat
-000103e0: 612c 2074 7570 6c65 293a 0a20 2020 2020  a, tuple):.     
-000103f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00010400: 7565 4572 726f 7228 2755 6e61 626c 6520  ueError('Unable 
-00010410: 746f 2073 6572 6961 6c69 7a65 2074 7970  to serialize typ
-00010420: 6520 7475 706c 6520 746f 2074 6578 742f  e tuple to text/
-00010430: 706c 6169 6e27 290a 2020 2020 2020 2020  plain').        
-00010440: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00010450: 696e 5f64 6174 612c 204e 6f6e 6543 6c61  in_data, NoneCla
-00010460: 7373 293a 0a20 2020 2020 2020 2020 2020  ss):.           
-00010470: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00010480: 7228 2755 6e61 626c 6520 746f 2073 6572  r('Unable to ser
-00010490: 6961 6c69 7a65 2074 7970 6520 4e6f 6e65  ialize type None
-000104a0: 436c 6173 7320 746f 2074 6578 742f 706c  Class to text/pl
-000104b0: 6169 6e27 290a 2020 2020 2020 2020 656c  ain').        el
-000104c0: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
-000104d0: 5f64 6174 612c 2042 6f6f 6c43 6c61 7373  _data, BoolClass
-000104e0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-000104f0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00010500: 2755 6e61 626c 6520 746f 2073 6572 6961  'Unable to seria
-00010510: 6c69 7a65 2074 7970 6520 426f 6f6c 436c  lize type BoolCl
-00010520: 6173 7320 746f 2074 6578 742f 706c 6169  ass to text/plai
-00010530: 6e27 290a 2020 2020 2020 2020 7265 7475  n').        retu
-00010540: 726e 2064 6963 7428 626f 6479 3d73 7472  rn dict(body=str
-00010550: 2869 6e5f 6461 7461 2929 0a0a 2020 2020  (in_data))..    
-00010560: 6465 6620 5f5f 6d75 6c74 6970 6172 745f  def __multipart_
-00010570: 6a73 6f6e 5f69 7465 6d28 7365 6c66 2c20  json_item(self, 
-00010580: 6b65 793a 2073 7472 2c20 7661 6c75 653a  key: str, value:
-00010590: 2053 6368 656d 6129 202d 3e20 5265 7175   Schema) -> Requ
-000105a0: 6573 7446 6965 6c64 3a0a 2020 2020 2020  estField:.      
-000105b0: 2020 6a73 6f6e 5f76 616c 7565 203d 2073    json_value = s
-000105c0: 656c 662e 5f5f 6a73 6f6e 5f65 6e63 6f64  elf.__json_encod
-000105d0: 6572 2e64 6566 6175 6c74 2876 616c 7565  er.default(value
-000105e0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000105f0: 2052 6571 7565 7374 4669 656c 6428 6e61   RequestField(na
-00010600: 6d65 3d6b 6579 2c20 6461 7461 3d6a 736f  me=key, data=jso
-00010610: 6e2e 6475 6d70 7328 6a73 6f6e 5f76 616c  n.dumps(json_val
-00010620: 7565 292c 2068 6561 6465 7273 3d7b 2743  ue), headers={'C
-00010630: 6f6e 7465 6e74 2d54 7970 6527 3a20 2761  ontent-Type': 'a
-00010640: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e27  pplication/json'
-00010650: 7d29 0a0a 2020 2020 6465 6620 5f5f 6d75  })..    def __mu
-00010660: 6c74 6970 6172 745f 666f 726d 5f69 7465  ltipart_form_ite
-00010670: 6d28 7365 6c66 2c20 6b65 793a 2073 7472  m(self, key: str
-00010680: 2c20 7661 6c75 653a 2053 6368 656d 6129  , value: Schema)
-00010690: 202d 3e20 5265 7175 6573 7446 6965 6c64   -> RequestField
-000106a0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-000106b0: 6e73 7461 6e63 6528 7661 6c75 652c 2073  nstance(value, s
-000106c0: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-000106d0: 2072 6574 7572 6e20 5265 7175 6573 7446   return RequestF
-000106e0: 6965 6c64 286e 616d 653d 6b65 792c 2064  ield(name=key, d
-000106f0: 6174 613d 7374 7228 7661 6c75 6529 2c20  ata=str(value), 
-00010700: 6865 6164 6572 733d 7b27 436f 6e74 656e  headers={'Conten
-00010710: 742d 5479 7065 273a 2027 7465 7874 2f70  t-Type': 'text/p
-00010720: 6c61 696e 277d 290a 2020 2020 2020 2020  lain'}).        
-00010730: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
-00010740: 7661 6c75 652c 2062 7974 6573 293a 0a20  value, bytes):. 
-00010750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010760: 6e20 5265 7175 6573 7446 6965 6c64 286e  n RequestField(n
-00010770: 616d 653d 6b65 792c 2064 6174 613d 7661  ame=key, data=va
-00010780: 6c75 652c 2068 6561 6465 7273 3d7b 2743  lue, headers={'C
-00010790: 6f6e 7465 6e74 2d54 7970 6527 3a20 2761  ontent-Type': 'a
-000107a0: 7070 6c69 6361 7469 6f6e 2f6f 6374 6574  pplication/octet
-000107b0: 2d73 7472 6561 6d27 7d29 0a20 2020 2020  -stream'}).     
-000107c0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-000107d0: 6365 2876 616c 7565 2c20 4669 6c65 494f  ce(value, FileIO
-000107e0: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
-000107f0: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
-00010800: 682e 6261 7365 6e61 6d65 2876 616c 7565  h.basename(value
-00010810: 2e6e 616d 6529 0a20 2020 2020 2020 2020  .name).         
-00010820: 2020 2072 6571 7565 7374 5f66 6965 6c64     request_field
-00010830: 203d 2052 6571 7565 7374 4669 656c 6428   = RequestField(
-00010840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010850: 206e 616d 653d 6b65 792c 0a20 2020 2020   name=key,.     
-00010860: 2020 2020 2020 2020 2020 2064 6174 613d             data=
-00010870: 7661 6c75 652e 7265 6164 2829 2c0a 2020  value.read(),.  
-00010880: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00010890: 6c65 6e61 6d65 3d66 696c 656e 616d 652c  lename=filename,
-000108a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000108b0: 2068 6561 6465 7273 3d7b 2743 6f6e 7465   headers={'Conte
-000108c0: 6e74 2d54 7970 6527 3a20 6775 6573 735f  nt-Type': guess_
-000108d0: 636f 6e74 656e 745f 7479 7065 2866 696c  content_type(fil
-000108e0: 656e 616d 6529 7d0a 2020 2020 2020 2020  ename)}.        
-000108f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010900: 2020 7661 6c75 652e 636c 6f73 6528 290a    value.close().
-00010910: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010920: 726e 2072 6571 7565 7374 5f66 6965 6c64  rn request_field
-00010930: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00010940: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010950: 6e20 7365 6c66 2e5f 5f6d 756c 7469 7061  n self.__multipa
-00010960: 7274 5f6a 736f 6e5f 6974 656d 286b 6579  rt_json_item(key
-00010970: 3d6b 6579 2c20 7661 6c75 653d 7661 6c75  =key, value=valu
-00010980: 6529 0a0a 2020 2020 6465 6620 5f5f 7365  e)..    def __se
-00010990: 7269 616c 697a 655f 6d75 6c74 6970 6172  rialize_multipar
-000109a0: 745f 666f 726d 5f64 6174 6128 0a20 2020  t_form_data(.   
-000109b0: 2020 2020 2073 656c 662c 2069 6e5f 6461       self, in_da
-000109c0: 7461 3a20 5363 6865 6d61 0a20 2020 2029  ta: Schema.    )
-000109d0: 202d 3e20 7479 7069 6e67 2e44 6963 745b   -> typing.Dict[
-000109e0: 7374 722c 2074 7970 696e 672e 5475 706c  str, typing.Tupl
-000109f0: 655b 5265 7175 6573 7446 6965 6c64 2c20  e[RequestField, 
-00010a00: 2e2e 2e5d 5d3a 0a20 2020 2020 2020 2069  ...]]:.        i
-00010a10: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00010a20: 2869 6e5f 6461 7461 2c20 6672 6f7a 656e  (in_data, frozen
-00010a30: 6469 6374 2e66 726f 7a65 6e64 6963 7429  dict.frozendict)
-00010a40: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00010a50: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-00010a60: 2755 6e61 626c 6520 746f 2073 6572 6961  'Unable to seria
-00010a70: 6c69 7a65 207b 696e 5f64 6174 617d 2074  lize {in_data} t
-00010a80: 6f20 6d75 6c74 6970 6172 742f 666f 726d  o multipart/form
-00010a90: 2d64 6174 6120 6265 6361 7573 6520 6974  -data because it
-00010aa0: 2069 7320 6e6f 7420 6120 6469 6374 206f   is not a dict o
-00010ab0: 6620 6461 7461 2729 0a20 2020 2020 2020  f data').       
-00010ac0: 2022 2222 0a20 2020 2020 2020 2049 6e20   """.        In 
-00010ad0: 6120 6d75 6c74 6970 6172 742f 666f 726d  a multipart/form
-00010ae0: 2d64 6174 6120 7265 7175 6573 7420 626f  -data request bo
-00010af0: 6479 2c20 6561 6368 2073 6368 656d 6120  dy, each schema 
-00010b00: 7072 6f70 6572 7479 2c20 6f72 2065 6163  property, or eac
-00010b10: 6820 656c 656d 656e 7420 6f66 2061 2073  h element of a s
-00010b20: 6368 656d 6120 6172 7261 7920 7072 6f70  chema array prop
-00010b30: 6572 7479 2c0a 2020 2020 2020 2020 7461  erty,.        ta
-00010b40: 6b65 7320 6120 7365 6374 696f 6e20 696e  kes a section in
-00010b50: 2074 6865 2070 6179 6c6f 6164 2077 6974   the payload wit
-00010b60: 6820 616e 2069 6e74 6572 6e61 6c20 6865  h an internal he
-00010b70: 6164 6572 2061 7320 6465 6669 6e65 6420  ader as defined 
-00010b80: 6279 2052 4643 3735 3738 2e20 5468 6520  by RFC7578. The 
-00010b90: 7365 7269 616c 697a 6174 696f 6e20 7374  serialization st
-00010ba0: 7261 7465 6779 0a20 2020 2020 2020 2066  rategy.        f
-00010bb0: 6f72 2065 6163 6820 7072 6f70 6572 7479  or each property
-00010bc0: 206f 6620 6120 6d75 6c74 6970 6172 742f   of a multipart/
-00010bd0: 666f 726d 2d64 6174 6120 7265 7175 6573  form-data reques
-00010be0: 7420 626f 6479 2063 616e 2062 6520 7370  t body can be sp
-00010bf0: 6563 6966 6965 6420 696e 2061 6e20 6173  ecified in an as
-00010c00: 736f 6369 6174 6564 2045 6e63 6f64 696e  sociated Encodin
-00010c10: 6720 4f62 6a65 6374 2e0a 0a20 2020 2020  g Object...     
-00010c20: 2020 2057 6865 6e20 7061 7373 696e 6720     When passing 
-00010c30: 696e 206d 756c 7469 7061 7274 2074 7970  in multipart typ
-00010c40: 6573 2c20 626f 756e 6461 7269 6573 204d  es, boundaries M
-00010c50: 4159 2062 6520 7573 6564 2074 6f20 7365  AY be used to se
-00010c60: 7061 7261 7465 2073 6563 7469 6f6e 7320  parate sections 
-00010c70: 6f66 2074 6865 2063 6f6e 7465 6e74 2062  of the content b
-00010c80: 6569 6e67 0a20 2020 2020 2020 2074 7261  eing.        tra
-00010c90: 6e73 6665 7272 6564 20e2 8093 2074 6875  nsferred ... thu
-00010ca0: 732c 2074 6865 2066 6f6c 6c6f 7769 6e67  s, the following
-00010cb0: 2064 6566 6175 6c74 2043 6f6e 7465 6e74   default Content
-00010cc0: 2d54 7970 6573 2061 7265 2064 6566 696e  -Types are defin
-00010cd0: 6564 2066 6f72 206d 756c 7469 7061 7274  ed for multipart
-00010ce0: 3a0a 0a20 2020 2020 2020 2049 6620 7468  :..        If th
-00010cf0: 6520 286f 626a 6563 7429 2070 726f 7065  e (object) prope
-00010d00: 7274 7920 6973 2061 2070 7269 6d69 7469  rty is a primiti
-00010d10: 7665 2c20 6f72 2061 6e20 6172 7261 7920  ve, or an array 
-00010d20: 6f66 2070 7269 6d69 7469 7665 2076 616c  of primitive val
-00010d30: 7565 732c 2074 6865 2064 6566 6175 6c74  ues, the default
-00010d40: 2043 6f6e 7465 6e74 2d54 7970 6520 6973   Content-Type is
-00010d50: 2074 6578 742f 706c 6169 6e0a 2020 2020   text/plain.    
-00010d60: 2020 2020 4966 2074 6865 2070 726f 7065      If the prope
-00010d70: 7274 7920 6973 2063 6f6d 706c 6578 2c20  rty is complex, 
-00010d80: 6f72 2061 6e20 6172 7261 7920 6f66 2063  or an array of c
-00010d90: 6f6d 706c 6578 2076 616c 7565 732c 2074  omplex values, t
-00010da0: 6865 2064 6566 6175 6c74 2043 6f6e 7465  he default Conte
-00010db0: 6e74 2d54 7970 6520 6973 2061 7070 6c69  nt-Type is appli
-00010dc0: 6361 7469 6f6e 2f6a 736f 6e0a 2020 2020  cation/json.    
-00010dd0: 2020 2020 2020 2020 5175 6573 7469 6f6e          Question
-00010de0: 3a20 686f 7720 6973 2074 6865 2061 7272  : how is the arr
-00010df0: 6179 206f 6620 7072 696d 6974 6976 6573  ay of primitives
-00010e00: 2065 6e63 6f64 6564 3f0a 2020 2020 2020   encoded?.      
-00010e10: 2020 4966 2074 6865 2070 726f 7065 7274    If the propert
-00010e20: 7920 6973 2061 2074 7970 653a 2073 7472  y is a type: str
-00010e30: 696e 6720 7769 7468 2061 2063 6f6e 7465  ing with a conte
-00010e40: 6e74 456e 636f 6469 6e67 2c20 7468 6520  ntEncoding, the 
-00010e50: 6465 6661 756c 7420 436f 6e74 656e 742d  default Content-
-00010e60: 5479 7065 2069 7320 6170 706c 6963 6174  Type is applicat
-00010e70: 696f 6e2f 6f63 7465 742d 7374 7265 616d  ion/octet-stream
-00010e80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010e90: 2020 2020 2066 6965 6c64 733a 2074 7970       fields: typ
-00010ea0: 696e 672e 4c69 7374 5b52 6571 7565 7374  ing.List[Request
-00010eb0: 4669 656c 645d 203d 205b 5d0a 2020 2020  Field] = [].    
-00010ec0: 2020 2020 666f 7220 6b65 792c 2076 616c      for key, val
-00010ed0: 7565 2069 6e20 696e 5f64 6174 612e 6974  ue in in_data.it
-00010ee0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00010ef0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00010f00: 2876 616c 7565 2c20 7475 706c 6529 3a0a  (value, tuple):.
-00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 6966 2076 616c 7565 3a0a 2020 2020 2020  if value:.      
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00010f40: 7661 6c75 6573 2075 7365 2065 7870 6c6f  values use explo
-00010f50: 6465 203d 2054 7275 652c 2073 6f20 7468  de = True, so th
-00010f60: 6520 636f 6465 206d 616b 6573 2061 2052  e code makes a R
-00010f70: 6571 7565 7374 4669 656c 6420 666f 7220  equestField for 
-00010f80: 6561 6368 2069 7465 6d20 7769 7468 206e  each item with n
-00010f90: 616d 653d 6b65 790a 2020 2020 2020 2020  ame=key.        
-00010fa0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00010fb0: 6974 656d 2069 6e20 7661 6c75 653a 0a20  item in value:. 
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fd0: 2020 2020 2020 2072 6571 7565 7374 5f66         request_f
-00010fe0: 6965 6c64 203d 2073 656c 662e 5f5f 6d75  ield = self.__mu
-00010ff0: 6c74 6970 6172 745f 666f 726d 5f69 7465  ltipart_form_ite
-00011000: 6d28 6b65 793d 6b65 792c 2076 616c 7565  m(key=key, value
-00011010: 3d69 7465 6d29 0a20 2020 2020 2020 2020  =item).         
-00011020: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011030: 6965 6c64 732e 6170 7065 6e64 2872 6571  ields.append(req
-00011040: 7565 7374 5f66 6965 6c64 290a 2020 2020  uest_field).    
-00011050: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00011060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00011070: 2020 2020 2020 2320 7365 6e64 2061 6e20        # send an 
-00011080: 656d 7074 7920 6172 7261 7920 6173 206a  empty array as j
-00011090: 736f 6e20 6265 6361 7573 6520 6578 706c  son because expl
-000110a0: 6f64 696e 6720 7769 6c6c 206e 6f74 2073  oding will not s
-000110b0: 656e 6420 6974 0a20 2020 2020 2020 2020  end it.         
-000110c0: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-000110d0: 7374 5f66 6965 6c64 203d 2073 656c 662e  st_field = self.
-000110e0: 5f5f 6d75 6c74 6970 6172 745f 6a73 6f6e  __multipart_json
-000110f0: 5f69 7465 6d28 6b65 793d 6b65 792c 2076  _item(key=key, v
-00011100: 616c 7565 3d76 616c 7565 290a 2020 2020  alue=value).    
+0000e930: 2020 2020 2020 2062 6f64 793d 626f 6479         body=body
+0000e940: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000e950: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000e960: 6520 4170 6956 616c 7565 4572 726f 7228  e ApiValueError(
+0000e970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e980: 2022 6874 7470 206d 6574 686f 6420 6d75   "http method mu
+0000e990: 7374 2062 6520 6047 4554 602c 2060 4845  st be `GET`, `HE
+0000e9a0: 4144 602c 2060 4f50 5449 4f4e 5360 2c22  AD`, `OPTIONS`,"
+0000e9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e9c0: 2022 2060 504f 5354 602c 2060 5041 5443   " `POST`, `PATC
+0000e9d0: 4860 2c20 6050 5554 6020 6f72 2060 4445  H`, `PUT` or `DE
+0000e9e0: 4c45 5445 602e 220a 2020 2020 2020 2020  LETE`.".        
+0000e9f0: 2020 2020 290a 0a20 2020 2064 6566 2075      )..    def u
+0000ea00: 7064 6174 655f 7061 7261 6d73 5f66 6f72  pdate_params_for
+0000ea10: 5f61 7574 6828 0a20 2020 2020 2020 2020  _auth(.         
+0000ea20: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000ea30: 2020 2020 2068 6561 6465 7273 2c0a 2020       headers,.  
+0000ea40: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
+0000ea50: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
+0000ea60: 2020 2020 2072 6573 6f75 7263 655f 7061       resource_pa
+0000ea70: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000ea80: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
+0000ea90: 2020 2020 626f 6479 2c0a 2020 2020 2020      body,.      
+0000eaa0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+0000eab0: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
+0000eac0: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+0000ead0: 4974 6572 6174 6f72 203d 204e 6f6e 650a  Iterator = None.
+0000eae0: 2020 2020 2020 2020 2920 2d3e 2073 7472          ) -> str
+0000eaf0: 3a0a 2020 2020 2020 2020 2222 2255 7064  :.        """Upd
+0000eb00: 6174 6573 2068 6561 6465 7220 616e 6420  ates header and 
+0000eb10: 7175 6572 7920 7061 7261 6d73 2062 6173  query params bas
+0000eb20: 6564 206f 6e20 6175 7468 656e 7469 6361  ed on authentica
+0000eb30: 7469 6f6e 2073 6574 7469 6e67 2e0a 0a20  tion setting... 
+0000eb40: 2020 2020 2020 203a 7061 7261 6d20 6865         :param he
+0000eb50: 6164 6572 733a 2048 6561 6465 7220 7061  aders: Header pa
+0000eb60: 7261 6d65 7465 7273 2064 6963 7420 746f  rameters dict to
+0000eb70: 2062 6520 7570 6461 7465 642e 0a20 2020   be updated..   
+0000eb80: 2020 2020 203a 7061 7261 6d20 6175 7468       :param auth
+0000eb90: 5f73 6574 7469 6e67 733a 2041 7574 6865  _settings: Authe
+0000eba0: 6e74 6963 6174 696f 6e20 7365 7474 696e  ntication settin
+0000ebb0: 6720 6964 656e 7469 6669 6572 7320 6c69  g identifiers li
+0000ebc0: 7374 2e0a 2020 2020 2020 2020 3a70 6172  st..        :par
+0000ebd0: 616d 2072 6573 6f75 7263 655f 7061 7468  am resource_path
+0000ebe0: 3a20 4120 7374 7269 6e67 2072 6570 7265  : A string repre
+0000ebf0: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
+0000ec00: 2048 5454 5020 7265 7175 6573 7420 7265   HTTP request re
+0000ec10: 736f 7572 6365 2070 6174 682e 0a20 2020  source path..   
+0000ec20: 2020 2020 203a 7061 7261 6d20 6d65 7468       :param meth
+0000ec30: 6f64 3a20 4120 7374 7269 6e67 2072 6570  od: A string rep
+0000ec40: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+0000ec50: 6865 2048 5454 5020 7265 7175 6573 7420  he HTTP request 
+0000ec60: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
+0000ec70: 3a70 6172 616d 2062 6f64 793a 2041 206f  :param body: A o
+0000ec80: 626a 6563 7420 7265 7072 6573 656e 7469  bject representi
+0000ec90: 6e67 2074 6865 2062 6f64 7920 6f66 2074  ng the body of t
+0000eca0: 6865 2048 5454 5020 7265 7175 6573 742e  he HTTP request.
+0000ecb0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000ecc0: 206f 626a 6563 7420 7479 7065 2069 7320   object type is 
+0000ecd0: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
+0000ece0: 206f 6620 5f65 6e63 6f64 6572 2e64 6566   of _encoder.def
+0000ecf0: 6175 6c74 2829 2e0a 2020 2020 2020 2020  ault()..        
+0000ed00: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+0000ed10: 6f74 2061 7574 685f 7365 7474 696e 6773  ot auth_settings
+0000ed20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000ed30: 7475 726e 2072 6573 6f75 7263 655f 7061  turn resource_pa
+0000ed40: 7468 0a20 2020 2020 2020 2069 6620 7072  th.        if pr
+0000ed50: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+0000ed60: 7465 7261 746f 7220 6973 204e 6f6e 653a  terator is None:
+0000ed70: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+0000ed80: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+0000ed90: 6572 6174 6f72 203d 2050 7265 6669 7853  erator = PrefixS
+0000eda0: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
+0000edb0: 2822 3f22 2c20 2226 2229 0a0a 2020 2020  ("?", "&")..    
+0000edc0: 2020 2020 666f 7220 6175 7468 2069 6e20      for auth in 
+0000edd0: 6175 7468 5f73 6574 7469 6e67 733a 0a20  auth_settings:. 
+0000ede0: 2020 2020 2020 2020 2020 2061 7574 685f             auth_
+0000edf0: 7365 7474 696e 6720 3d20 7365 6c66 2e63  setting = self.c
+0000ee00: 6f6e 6669 6775 7261 7469 6f6e 2e61 7574  onfiguration.aut
+0000ee10: 685f 7365 7474 696e 6773 2829 2e67 6574  h_settings().get
+0000ee20: 2861 7574 6829 0a20 2020 2020 2020 2020  (auth).         
+0000ee30: 2020 2069 6620 6e6f 7420 6175 7468 5f73     if not auth_s
+0000ee40: 6574 7469 6e67 3a0a 2020 2020 2020 2020  etting:.        
+0000ee50: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000ee60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ee70: 6175 7468 5f73 6574 7469 6e67 5b27 696e  auth_setting['in
+0000ee80: 275d 203d 3d20 2763 6f6f 6b69 6527 3a0a  '] == 'cookie':.
+0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eea0: 6865 6164 6572 732e 6164 6428 2743 6f6f  headers.add('Coo
+0000eeb0: 6b69 6527 2c20 6175 7468 5f73 6574 7469  kie', auth_setti
+0000eec0: 6e67 5b27 7661 6c75 6527 5d29 0a20 2020  ng['value']).   
+0000eed0: 2020 2020 2020 2020 2065 6c69 6620 6175           elif au
+0000eee0: 7468 5f73 6574 7469 6e67 5b27 696e 275d  th_setting['in']
+0000eef0: 203d 3d20 2768 6561 6465 7227 3a0a 2020   == 'header':.  
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000ef10: 2061 7574 685f 7365 7474 696e 675b 2774   auth_setting['t
+0000ef20: 7970 6527 5d20 213d 2027 6874 7470 2d73  ype'] != 'http-s
+0000ef30: 6967 6e61 7475 7265 273a 0a20 2020 2020  ignature':.     
+0000ef40: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000ef50: 6561 6465 7273 2e61 6464 2861 7574 685f  eaders.add(auth_
+0000ef60: 7365 7474 696e 675b 276b 6579 275d 2c20  setting['key'], 
+0000ef70: 6175 7468 5f73 6574 7469 6e67 5b27 7661  auth_setting['va
+0000ef80: 6c75 6527 5d29 0a20 2020 2020 2020 2020  lue']).         
+0000ef90: 2020 2065 6c69 6620 6175 7468 5f73 6574     elif auth_set
+0000efa0: 7469 6e67 5b27 696e 275d 203d 3d20 2771  ting['in'] == 'q
+0000efb0: 7565 7279 273a 0a20 2020 2020 2020 2020  uery':.         
+0000efc0: 2020 2020 2020 2022 2222 2054 4f44 4f20         """ TODO 
+0000efd0: 696d 706c 656d 656e 7420 6175 7468 2069  implement auth i
+0000efe0: 6e20 7175 6572 790a 2020 2020 2020 2020  n query.        
+0000eff0: 2020 2020 2020 2020 6e65 6564 2074 6f20          need to 
+0000f000: 7061 7373 2069 6e20 7072 6566 6978 5f73  pass in prefix_s
+0000f010: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+0000f020: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000f030: 2020 616e 6420 6e65 6564 2074 6f20 6f75    and need to ou
+0000f040: 7470 7574 2072 6573 6f75 7263 655f 7061  tput resource_pa
+0000f050: 7468 2077 6974 6820 7175 6572 7920 7061  th with query pa
+0000f060: 7261 6d73 2061 6464 6564 0a20 2020 2020  rams added.     
+0000f070: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f090: 6573 6f75 7263 655f 7061 7468 202b 3d20  esource_path += 
+0000f0a0: 5061 7261 6d65 7465 7253 6572 6961 6c69  ParameterSeriali
+0000f0b0: 7a65 7242 6173 652e 5f72 6566 3635 3730  zerBase._ref6570
+0000f0c0: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
+0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0e0: 7661 7269 6162 6c65 5f6e 616d 653d 6175  variable_name=au
+0000f0f0: 7468 5f73 6574 7469 6e67 5b27 6b65 7927  th_setting['key'
+0000f100: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000f110: 2020 2020 2020 2069 6e5f 6461 7461 3d61         in_data=a
+0000f120: 7574 685f 7365 7474 696e 675b 2776 616c  uth_setting['val
+0000f130: 7565 275d 2c0a 2020 2020 2020 2020 2020  ue'],.          
+0000f140: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
+0000f150: 653d 4661 6c73 652c 0a20 2020 2020 2020  e=False,.       
+0000f160: 2020 2020 2020 2020 2020 2020 2070 6572               per
+0000f170: 6365 6e74 5f65 6e63 6f64 653d 4661 6c73  cent_encode=Fals
+0000f180: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000f190: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+0000f1a0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+0000f1b0: 3d70 7265 6669 785f 7365 7061 7261 746f  =prefix_separato
+0000f1c0: 725f 6974 6572 6174 6f72 0a20 2020 2020  r_iterator.     
+0000f1d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f1e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000f1f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f200: 6169 7365 2041 7069 5661 6c75 6545 7272  aise ApiValueErr
+0000f210: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000f220: 2020 2020 2020 2020 2741 7574 6865 6e74          'Authent
+0000f230: 6963 6174 696f 6e20 746f 6b65 6e20 6d75  ication token mu
+0000f240: 7374 2062 6520 696e 2060 7175 6572 7960  st be in `query`
+0000f250: 206f 7220 6068 6561 6465 7260 270a 2020   or `header`'.  
+0000f260: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000f270: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000f280: 6573 6f75 7263 655f 7061 7468 0a0a 0a63  esource_path...c
+0000f290: 6c61 7373 2041 7069 3a0a 2020 2020 2222  lass Api:.    ""
+0000f2a0: 224e 4f54 453a 0a20 2020 2054 6869 7320  "NOTE:.    This 
+0000f2b0: 636c 6173 7320 6973 2061 7574 6f20 6765  class is auto ge
+0000f2c0: 6e65 7261 7465 6420 6279 204b 6f6e 6669  nerated by Konfi
+0000f2d0: 6720 2868 7474 7073 3a2f 2f6b 6f6e 6669  g (https://konfi
+0000f2e0: 6774 6869 732e 636f 6d29 0a20 2020 2022  gthis.com).    "
+0000f2f0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+0000f300: 6974 5f5f 2873 656c 662c 2061 7069 5f63  it__(self, api_c
+0000f310: 6c69 656e 743a 2074 7970 696e 672e 4f70  lient: typing.Op
+0000f320: 7469 6f6e 616c 5b41 7069 436c 6965 6e74  tional[ApiClient
+0000f330: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+0000f340: 2020 2069 6620 6170 695f 636c 6965 6e74     if api_client
+0000f350: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000f360: 2020 2020 2020 6170 695f 636c 6965 6e74        api_client
+0000f370: 203d 2041 7069 436c 6965 6e74 2829 0a20   = ApiClient(). 
+0000f380: 2020 2020 2020 2073 656c 662e 6170 695f         self.api_
+0000f390: 636c 6965 6e74 203d 2061 7069 5f63 6c69  client = api_cli
+0000f3a0: 656e 740a 0a20 2020 2040 7374 6174 6963  ent..    @static
+0000f3b0: 6d65 7468 6f64 0a20 2020 2064 6566 205f  method.    def _
+0000f3c0: 7665 7269 6679 5f74 7970 6564 5f64 6963  verify_typed_dic
+0000f3d0: 745f 696e 7075 7473 5f6f 6170 6728 636c  t_inputs_oapg(cl
+0000f3e0: 733a 2074 7970 696e 672e 5479 7065 5b74  s: typing.Type[t
+0000f3f0: 7970 696e 675f 6578 7465 6e73 696f 6e73  yping_extensions
+0000f400: 2e54 7970 6564 4469 6374 5d2c 2064 6174  .TypedDict], dat
+0000f410: 613a 2074 7970 696e 672e 4469 6374 5b73  a: typing.Dict[s
+0000f420: 7472 2c20 7479 7069 6e67 2e41 6e79 5d29  tr, typing.Any])
+0000f430: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f440: 2020 2020 2020 456e 7375 7265 7320 7468        Ensures th
+0000f450: 6174 3a0a 2020 2020 2020 2020 2d20 7265  at:.        - re
+0000f460: 7175 6972 6564 206b 6579 7320 6172 6520  quired keys are 
+0000f470: 7072 6573 656e 740a 2020 2020 2020 2020  present.        
+0000f480: 2d20 6164 6469 7469 6f6e 616c 2070 726f  - additional pro
+0000f490: 7065 7274 6965 7320 6172 6520 6e6f 7420  perties are not 
+0000f4a0: 696e 7075 740a 2020 2020 2020 2020 2d20  input.        - 
+0000f4b0: 7661 6c75 6520 7374 6f72 6564 2075 6e64  value stored und
+0000f4c0: 6572 2072 6571 7569 7265 6420 6b65 7973  er required keys
+0000f4d0: 2064 6f20 6e6f 7420 6861 7665 2074 6865   do not have the
+0000f4e0: 2076 616c 7565 2075 6e73 6574 0a20 2020   value unset.   
+0000f4f0: 2020 2020 204e 6f74 653a 2064 6574 6169       Note: detai
+0000f500: 6c65 6420 7661 6c75 6520 6368 6563 6b69  led value checki
+0000f510: 6e67 2069 7320 646f 6e65 2069 6e20 7363  ng is done in sc
+0000f520: 6865 6d61 2063 6c61 7373 6573 0a20 2020  hema classes.   
+0000f530: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f540: 206d 6973 7369 6e67 5f72 6571 7569 7265   missing_require
+0000f550: 645f 6b65 7973 203d 205b 5d0a 2020 2020  d_keys = [].    
+0000f560: 2020 2020 7265 7175 6972 6564 5f6b 6579      required_key
+0000f570: 735f 7769 7468 5f75 6e73 6574 5f76 616c  s_with_unset_val
+0000f580: 7565 7320 3d20 5b5d 0a20 2020 2020 2020  ues = [].       
+0000f590: 2066 6f72 2072 6571 7569 7265 645f 6b65   for required_ke
+0000f5a0: 7920 696e 2063 6c73 2e5f 5f72 6571 7569  y in cls.__requi
+0000f5b0: 7265 645f 6b65 7973 5f5f 3a0a 2020 2020  red_keys__:.    
+0000f5c0: 2020 2020 2020 2020 6966 2072 6571 7569          if requi
+0000f5d0: 7265 645f 6b65 7920 6e6f 7420 696e 2064  red_key not in d
+0000f5e0: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+0000f5f0: 2020 2020 206d 6973 7369 6e67 5f72 6571       missing_req
+0000f600: 7569 7265 645f 6b65 7973 2e61 7070 656e  uired_keys.appen
+0000f610: 6428 7265 7175 6972 6564 5f6b 6579 290a  d(required_key).
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+0000f640: 2020 2020 2076 616c 7565 203d 2064 6174       value = dat
+0000f650: 615b 7265 7175 6972 6564 5f6b 6579 5d0a  a[required_key].
+0000f660: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+0000f670: 616c 7565 2069 7320 756e 7365 743a 0a20  alue is unset:. 
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f690: 6571 7569 7265 645f 6b65 7973 5f77 6974  equired_keys_wit
+0000f6a0: 685f 756e 7365 745f 7661 6c75 6573 2e61  h_unset_values.a
+0000f6b0: 7070 656e 6428 7265 7175 6972 6564 5f6b  ppend(required_k
+0000f6c0: 6579 290a 2020 2020 2020 2020 6966 206d  ey).        if m
+0000f6d0: 6973 7369 6e67 5f72 6571 7569 7265 645f  issing_required_
+0000f6e0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+0000f6f0: 2020 7261 6973 6520 4170 6954 7970 6545    raise ApiTypeE
+0000f700: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000f710: 2020 2020 2020 277b 7d20 6d69 7373 696e        '{} missin
+0000f720: 6720 7b7d 2072 6571 7569 7265 6420 6172  g {} required ar
+0000f730: 6775 6d65 6e74 733a 207b 7d27 2e66 6f72  guments: {}'.for
+0000f740: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0000f750: 2020 2020 2020 2020 2063 6c73 2e5f 5f6e           cls.__n
+0000f760: 616d 655f 5f2c 206c 656e 286d 6973 7369  ame__, len(missi
+0000f770: 6e67 5f72 6571 7569 7265 645f 6b65 7973  ng_required_keys
+0000f780: 292c 206d 6973 7369 6e67 5f72 6571 7569  ), missing_requi
+0000f790: 7265 645f 6b65 7973 0a20 2020 2020 2020  red_keys.       
+0000f7a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f7b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000f7c0: 2020 2069 6620 7265 7175 6972 6564 5f6b     if required_k
+0000f7d0: 6579 735f 7769 7468 5f75 6e73 6574 5f76  eys_with_unset_v
+0000f7e0: 616c 7565 733a 0a20 2020 2020 2020 2020  alues:.         
+0000f7f0: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
+0000f800: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000f810: 2020 2020 2020 2020 277b 7d20 636f 6e74          '{} cont
+0000f820: 6169 6e73 2069 6e76 616c 6964 2075 6e73  ains invalid uns
+0000f830: 6574 2076 616c 7565 7320 666f 7220 7b7d  et values for {}
+0000f840: 2072 6571 7569 7265 6420 6b65 7973 3a20   required keys: 
+0000f850: 7b7d 272e 666f 726d 6174 280a 2020 2020  {}'.format(.    
+0000f860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f870: 636c 732e 5f5f 6e61 6d65 5f5f 2c20 6c65  cls.__name__, le
+0000f880: 6e28 7265 7175 6972 6564 5f6b 6579 735f  n(required_keys_
+0000f890: 7769 7468 5f75 6e73 6574 5f76 616c 7565  with_unset_value
+0000f8a0: 7329 2c20 7265 7175 6972 6564 5f6b 6579  s), required_key
+0000f8b0: 735f 7769 7468 5f75 6e73 6574 5f76 616c  s_with_unset_val
+0000f8c0: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
+0000f8d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000f8e0: 2020 290a 0a20 2020 2020 2020 2064 6973    )..        dis
+0000f8f0: 616c 6c6f 7765 645f 6164 6469 7469 6f6e  allowed_addition
+0000f900: 616c 5f6b 6579 7320 3d20 5b5d 0a20 2020  al_keys = [].   
+0000f910: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
+0000f920: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+0000f930: 2020 6966 206b 6579 2069 6e20 636c 732e    if key in cls.
+0000f940: 5f5f 7265 7175 6972 6564 5f6b 6579 735f  __required_keys_
+0000f950: 5f20 6f72 206b 6579 2069 6e20 636c 732e  _ or key in cls.
+0000f960: 5f5f 6f70 7469 6f6e 616c 5f6b 6579 735f  __optional_keys_
+0000f970: 5f3a 0a20 2020 2020 2020 2020 2020 2020  _:.             
+0000f980: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+0000f990: 2020 2020 2020 2020 6469 7361 6c6c 6f77          disallow
+0000f9a0: 6564 5f61 6464 6974 696f 6e61 6c5f 6b65  ed_additional_ke
+0000f9b0: 7973 2e61 7070 656e 6428 6b65 7929 0a20  ys.append(key). 
+0000f9c0: 2020 2020 2020 2069 6620 6469 7361 6c6c         if disall
+0000f9d0: 6f77 6564 5f61 6464 6974 696f 6e61 6c5f  owed_additional_
+0000f9e0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+0000f9f0: 2020 7261 6973 6520 4170 6954 7970 6545    raise ApiTypeE
+0000fa00: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000fa10: 2020 2020 2020 277b 7d20 676f 7420 7b7d        '{} got {}
+0000fa20: 2075 6e65 7870 6563 7465 6420 6b65 7977   unexpected keyw
+0000fa30: 6f72 6420 6172 6775 6d65 6e74 733a 207b  ord arguments: {
+0000fa40: 7d27 2e66 6f72 6d61 7428 0a20 2020 2020  }'.format(.     
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000fa60: 6c73 2e5f 5f6e 616d 655f 5f2c 206c 656e  ls.__name__, len
+0000fa70: 2864 6973 616c 6c6f 7765 645f 6164 6469  (disallowed_addi
+0000fa80: 7469 6f6e 616c 5f6b 6579 7329 2c20 6469  tional_keys), di
+0000fa90: 7361 6c6c 6f77 6564 5f61 6464 6974 696f  sallowed_additio
+0000faa0: 6e61 6c5f 6b65 7973 0a20 2020 2020 2020  nal_keys.       
+0000fab0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000fac0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+0000fad0: 6620 5f67 6574 5f68 6f73 745f 6f61 7067  f _get_host_oapg
+0000fae0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000faf0: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+0000fb00: 6e5f 6964 3a20 7374 722c 0a20 2020 2020  n_id: str,.     
+0000fb10: 2020 2073 6572 7665 7273 3a20 7479 7069     servers: typi
+0000fb20: 6e67 2e54 7570 6c65 5b74 7970 696e 672e  ng.Tuple[typing.
+0000fb30: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
+0000fb40: 2e2e 2e5d 203d 2074 7570 6c65 2829 2c0a  ...] = tuple(),.
+0000fb50: 2020 2020 2020 2020 686f 7374 5f69 6e64          host_ind
+0000fb60: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+0000fb70: 6e61 6c5b 696e 745d 203d 204e 6f6e 650a  nal[int] = None.
+0000fb80: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
+0000fb90: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
+0000fba0: 2020 2020 2020 2063 6f6e 6669 6775 7261         configura
+0000fbb0: 7469 6f6e 203d 2073 656c 662e 6170 695f  tion = self.api_
+0000fbc0: 636c 6965 6e74 2e63 6f6e 6669 6775 7261  client.configura
+0000fbd0: 7469 6f6e 0a20 2020 2020 2020 2074 7279  tion.        try
+0000fbe0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000fbf0: 2068 6f73 745f 696e 6465 7820 6973 204e   host_index is N
+0000fc00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000fc10: 2020 2020 2069 6e64 6578 203d 2063 6f6e       index = con
+0000fc20: 6669 6775 7261 7469 6f6e 2e73 6572 7665  figuration.serve
+0000fc30: 725f 6f70 6572 6174 696f 6e5f 696e 6465  r_operation_inde
+0000fc40: 782e 6765 7428 0a20 2020 2020 2020 2020  x.get(.         
+0000fc50: 2020 2020 2020 2020 2020 206f 7065 7261             opera
+0000fc60: 7469 6f6e 5f69 642c 2063 6f6e 6669 6775  tion_id, configu
+0000fc70: 7261 7469 6f6e 2e73 6572 7665 725f 696e  ration.server_in
+0000fc80: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
+0000fc90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000fca0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fcb0: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
+0000fcc0: 686f 7374 5f69 6e64 6578 0a20 2020 2020  host_index.     
+0000fcd0: 2020 2020 2020 2073 6572 7665 725f 7661         server_va
+0000fce0: 7269 6162 6c65 7320 3d20 636f 6e66 6967  riables = config
+0000fcf0: 7572 6174 696f 6e2e 7365 7276 6572 5f6f  uration.server_o
+0000fd00: 7065 7261 7469 6f6e 5f76 6172 6961 626c  peration_variabl
+0000fd10: 6573 2e67 6574 280a 2020 2020 2020 2020  es.get(.        
+0000fd20: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
+0000fd30: 6e5f 6964 2c20 636f 6e66 6967 7572 6174  n_id, configurat
+0000fd40: 696f 6e2e 7365 7276 6572 5f76 6172 6961  ion.server_varia
+0000fd50: 626c 6573 0a20 2020 2020 2020 2020 2020  bles.           
+0000fd60: 2029 0a20 2020 2020 2020 2020 2020 2068   ).            h
+0000fd70: 6f73 7420 3d20 636f 6e66 6967 7572 6174  ost = configurat
+0000fd80: 696f 6e2e 6765 745f 686f 7374 5f66 726f  ion.get_host_fro
+0000fd90: 6d5f 7365 7474 696e 6773 280a 2020 2020  m_settings(.    
+0000fda0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000fdb0: 782c 2076 6172 6961 626c 6573 3d73 6572  x, variables=ser
+0000fdc0: 7665 725f 7661 7269 6162 6c65 732c 2073  ver_variables, s
+0000fdd0: 6572 7665 7273 3d73 6572 7665 7273 0a20  ervers=servers. 
+0000fde0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fdf0: 2020 2020 2065 7863 6570 7420 496e 6465       except Inde
+0000fe00: 7845 7272 6f72 3a0a 2020 2020 2020 2020  xError:.        
+0000fe10: 2020 2020 6966 2073 6572 7665 7273 3a0a      if servers:.
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe30: 7261 6973 6520 4170 6956 616c 7565 4572  raise ApiValueEr
+0000fe40: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000fe50: 2020 2020 2020 2020 2022 496e 7661 6c69           "Invali
+0000fe60: 6420 686f 7374 2069 6e64 6578 2e20 4d75  d host index. Mu
+0000fe70: 7374 2062 6520 3020 3c3d 2069 6e64 6578  st be 0 <= index
+0000fe80: 203c 2025 7322 2025 0a20 2020 2020 2020   < %s" %.       
+0000fe90: 2020 2020 2020 2020 2020 2020 206c 656e               len
+0000fea0: 2873 6572 7665 7273 290a 2020 2020 2020  (servers).      
+0000feb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000fec0: 2020 2020 2020 2020 686f 7374 203d 204e          host = N
+0000fed0: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
+0000fee0: 726e 2068 6f73 740a 0a0a 636c 6173 7320  rn host...class 
+0000fef0: 5365 7269 616c 697a 6564 5265 7175 6573  SerializedReques
+0000ff00: 7442 6f64 7928 7479 7069 6e67 5f65 7874  tBody(typing_ext
+0000ff10: 656e 7369 6f6e 732e 5479 7065 6444 6963  ensions.TypedDic
+0000ff20: 742c 2074 6f74 616c 3d46 616c 7365 293a  t, total=False):
+0000ff30: 0a20 2020 2062 6f64 793a 2074 7970 696e  .    body: typin
+0000ff40: 672e 556e 696f 6e5b 7374 722c 2062 7974  g.Union[str, byt
+0000ff50: 6573 5d0a 2020 2020 6669 656c 6473 3a20  es].    fields: 
+0000ff60: 7479 7069 6e67 2e54 7570 6c65 5b74 7970  typing.Tuple[typ
+0000ff70: 696e 672e 556e 696f 6e5b 5265 7175 6573  ing.Union[Reques
+0000ff80: 7446 6965 6c64 2c20 7479 7069 6e67 2e54  tField, typing.T
+0000ff90: 7570 6c65 5b73 7472 2c20 7374 725d 5d2c  uple[str, str]],
+0000ffa0: 202e 2e2e 5d0a 0a0a 636c 6173 7320 5265   ...]...class Re
+0000ffb0: 7175 6573 7442 6f64 7928 5374 796c 6546  questBody(StyleF
+0000ffc0: 6f72 6d53 6572 6961 6c69 7a65 722c 204a  ormSerializer, J
+0000ffd0: 534f 4e44 6574 6563 746f 7229 3a0a 2020  SONDetector):.  
+0000ffe0: 2020 2222 220a 2020 2020 4120 7265 7175    """.    A requ
+0000fff0: 6573 7420 626f 6479 2070 6172 616d 6574  est body paramet
+00010000: 6572 0a20 2020 2063 6f6e 7465 6e74 3a20  er.    content: 
+00010010: 636f 6e74 656e 745f 7479 7065 2074 6f20  content_type to 
+00010020: 4d65 6469 6154 7970 6520 5363 6865 6d61  MediaType Schema
+00010030: 2069 6e66 6f0a 2020 2020 2222 220a 2020   info.    """.  
+00010040: 2020 5f5f 6a73 6f6e 5f65 6e63 6f64 6572    __json_encoder
+00010050: 203d 204a 534f 4e45 6e63 6f64 6572 2829   = JSONEncoder()
+00010060: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00010070: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00010080: 2c0a 2020 2020 2020 2020 636f 6e74 656e  ,.        conten
+00010090: 743a 2074 7970 696e 672e 4469 6374 5b73  t: typing.Dict[s
+000100a0: 7472 2c20 4d65 6469 6154 7970 655d 2c0a  tr, MediaType],.
+000100b0: 2020 2020 2020 2020 7265 7175 6972 6564          required
+000100c0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+000100d0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+000100e0: 656c 662e 7265 7175 6972 6564 203d 2072  elf.required = r
+000100f0: 6571 7569 7265 640a 2020 2020 2020 2020  equired.        
+00010100: 6966 206c 656e 2863 6f6e 7465 6e74 2920  if len(content) 
+00010110: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00010120: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00010130: 6f72 2827 496e 7661 6c69 6420 7661 6c75  or('Invalid valu
+00010140: 6520 666f 7220 636f 6e74 656e 742c 2074  e for content, t
+00010150: 6865 2063 6f6e 7465 6e74 2064 6963 7420  he content dict 
+00010160: 6d75 7374 2068 6176 6520 3e3d 2031 2065  must have >= 1 e
+00010170: 6e74 7279 2729 0a20 2020 2020 2020 2073  ntry').        s
+00010180: 656c 662e 636f 6e74 656e 7420 3d20 636f  elf.content = co
+00010190: 6e74 656e 740a 0a20 2020 2064 6566 205f  ntent..    def _
+000101a0: 5f73 6572 6961 6c69 7a65 5f6a 736f 6e28  _serialize_json(
+000101b0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000101c0: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
+000101d0: 7479 7069 6e67 2e41 6e79 0a20 2020 2029  typing.Any.    )
+000101e0: 202d 3e20 7479 7069 6e67 2e44 6963 745b   -> typing.Dict[
+000101f0: 7374 722c 2062 7974 6573 5d3a 0a20 2020  str, bytes]:.   
+00010200: 2020 2020 2069 6e5f 6461 7461 203d 2073       in_data = s
+00010210: 656c 662e 5f5f 6a73 6f6e 5f65 6e63 6f64  elf.__json_encod
+00010220: 6572 2e64 6566 6175 6c74 2869 6e5f 6461  er.default(in_da
+00010230: 7461 290a 2020 2020 2020 2020 6a73 6f6e  ta).        json
+00010240: 5f73 7472 203d 206a 736f 6e2e 6475 6d70  _str = json.dump
+00010250: 7328 696e 5f64 6174 612c 2073 6570 6172  s(in_data, separ
+00010260: 6174 6f72 733d 2822 2c22 2c20 223a 2229  ators=(",", ":")
+00010270: 2c20 656e 7375 7265 5f61 7363 6969 3d46  , ensure_ascii=F
+00010280: 616c 7365 292e 656e 636f 6465 280a 2020  alse).encode(.  
+00010290: 2020 2020 2020 2020 2020 2275 7466 2d38            "utf-8
+000102a0: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
+000102b0: 2020 2020 7265 7475 726e 2064 6963 7428      return dict(
+000102c0: 626f 6479 3d6a 736f 6e5f 7374 7229 0a0a  body=json_str)..
+000102d0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+000102e0: 640a 2020 2020 6465 6620 5f5f 7365 7269  d.    def __seri
+000102f0: 616c 697a 655f 7465 7874 5f70 6c61 696e  alize_text_plain
+00010300: 2869 6e5f 6461 7461 3a20 7479 7069 6e67  (in_data: typing
+00010310: 2e41 6e79 2920 2d3e 2074 7970 696e 672e  .Any) -> typing.
+00010320: 4469 6374 5b73 7472 2c20 7374 725d 3a0a  Dict[str, str]:.
+00010330: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00010340: 7461 6e63 6528 696e 5f64 6174 612c 2066  tance(in_data, f
+00010350: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
+00010360: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
+00010370: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010380: 726f 7228 2755 6e61 626c 6520 746f 2073  ror('Unable to s
+00010390: 6572 6961 6c69 7a65 2074 7970 6520 6672  erialize type fr
+000103a0: 6f7a 656e 6469 6374 2e66 726f 7a65 6e64  ozendict.frozend
+000103b0: 6963 7420 746f 2074 6578 742f 706c 6169  ict to text/plai
+000103c0: 6e27 290a 2020 2020 2020 2020 656c 6966  n').        elif
+000103d0: 2069 7369 6e73 7461 6e63 6528 696e 5f64   isinstance(in_d
+000103e0: 6174 612c 2074 7570 6c65 293a 0a20 2020  ata, tuple):.   
+000103f0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00010400: 616c 7565 4572 726f 7228 2755 6e61 626c  alueError('Unabl
+00010410: 6520 746f 2073 6572 6961 6c69 7a65 2074  e to serialize t
+00010420: 7970 6520 7475 706c 6520 746f 2074 6578  ype tuple to tex
+00010430: 742f 706c 6169 6e27 290a 2020 2020 2020  t/plain').      
+00010440: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00010450: 6528 696e 5f64 6174 612c 204e 6f6e 6543  e(in_data, NoneC
+00010460: 6c61 7373 293a 0a20 2020 2020 2020 2020  lass):.         
+00010470: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00010480: 726f 7228 2755 6e61 626c 6520 746f 2073  ror('Unable to s
+00010490: 6572 6961 6c69 7a65 2074 7970 6520 4e6f  erialize type No
+000104a0: 6e65 436c 6173 7320 746f 2074 6578 742f  neClass to text/
+000104b0: 706c 6169 6e27 290a 2020 2020 2020 2020  plain').        
+000104c0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+000104d0: 696e 5f64 6174 612c 2042 6f6f 6c43 6c61  in_data, BoolCla
+000104e0: 7373 293a 0a20 2020 2020 2020 2020 2020  ss):.           
+000104f0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00010500: 7228 2755 6e61 626c 6520 746f 2073 6572  r('Unable to ser
+00010510: 6961 6c69 7a65 2074 7970 6520 426f 6f6c  ialize type Bool
+00010520: 436c 6173 7320 746f 2074 6578 742f 706c  Class to text/pl
+00010530: 6169 6e27 290a 2020 2020 2020 2020 7265  ain').        re
+00010540: 7475 726e 2064 6963 7428 626f 6479 3d73  turn dict(body=s
+00010550: 7472 2869 6e5f 6461 7461 2929 0a0a 2020  tr(in_data))..  
+00010560: 2020 6465 6620 5f5f 6d75 6c74 6970 6172    def __multipar
+00010570: 745f 6a73 6f6e 5f69 7465 6d28 7365 6c66  t_json_item(self
+00010580: 2c20 6b65 793a 2073 7472 2c20 7661 6c75  , key: str, valu
+00010590: 653a 2053 6368 656d 6129 202d 3e20 5265  e: Schema) -> Re
+000105a0: 7175 6573 7446 6965 6c64 3a0a 2020 2020  questField:.    
+000105b0: 2020 2020 6a73 6f6e 5f76 616c 7565 203d      json_value =
+000105c0: 2073 656c 662e 5f5f 6a73 6f6e 5f65 6e63   self.__json_enc
+000105d0: 6f64 6572 2e64 6566 6175 6c74 2876 616c  oder.default(val
+000105e0: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+000105f0: 726e 2052 6571 7565 7374 4669 656c 6428  rn RequestField(
+00010600: 6e61 6d65 3d6b 6579 2c20 6461 7461 3d6a  name=key, data=j
+00010610: 736f 6e2e 6475 6d70 7328 6a73 6f6e 5f76  son.dumps(json_v
+00010620: 616c 7565 292c 2068 6561 6465 7273 3d7b  alue), headers={
+00010630: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+00010640: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
+00010650: 6e27 7d29 0a0a 2020 2020 6465 6620 5f5f  n'})..    def __
+00010660: 6d75 6c74 6970 6172 745f 666f 726d 5f69  multipart_form_i
+00010670: 7465 6d28 7365 6c66 2c20 6b65 793a 2073  tem(self, key: s
+00010680: 7472 2c20 7661 6c75 653a 2053 6368 656d  tr, value: Schem
+00010690: 6129 202d 3e20 5265 7175 6573 7446 6965  a) -> RequestFie
+000106a0: 6c64 3a0a 2020 2020 2020 2020 6966 2069  ld:.        if i
+000106b0: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
+000106c0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
+000106d0: 2020 2072 6574 7572 6e20 5265 7175 6573     return Reques
+000106e0: 7446 6965 6c64 286e 616d 653d 6b65 792c  tField(name=key,
+000106f0: 2064 6174 613d 7374 7228 7661 6c75 6529   data=str(value)
+00010700: 2c20 6865 6164 6572 733d 7b27 436f 6e74  , headers={'Cont
+00010710: 656e 742d 5479 7065 273a 2027 7465 7874  ent-Type': 'text
+00010720: 2f70 6c61 696e 277d 290a 2020 2020 2020  /plain'}).      
+00010730: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00010740: 6528 7661 6c75 652c 2062 7974 6573 293a  e(value, bytes):
+00010750: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010760: 7572 6e20 5265 7175 6573 7446 6965 6c64  urn RequestField
+00010770: 286e 616d 653d 6b65 792c 2064 6174 613d  (name=key, data=
+00010780: 7661 6c75 652c 2068 6561 6465 7273 3d7b  value, headers={
+00010790: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
+000107a0: 2761 7070 6c69 6361 7469 6f6e 2f6f 6374  'application/oct
+000107b0: 6574 2d73 7472 6561 6d27 7d29 0a20 2020  et-stream'}).   
+000107c0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+000107d0: 616e 6365 2876 616c 7565 2c20 4669 6c65  ance(value, File
+000107e0: 494f 293a 0a20 2020 2020 2020 2020 2020  IO):.           
+000107f0: 2066 696c 656e 616d 6520 3d20 6f73 2e70   filename = os.p
+00010800: 6174 682e 6261 7365 6e61 6d65 2876 616c  ath.basename(val
+00010810: 7565 2e6e 616d 6529 0a20 2020 2020 2020  ue.name).       
+00010820: 2020 2020 2072 6571 7565 7374 5f66 6965       request_fie
+00010830: 6c64 203d 2052 6571 7565 7374 4669 656c  ld = RequestFiel
+00010840: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00010850: 2020 206e 616d 653d 6b65 792c 0a20 2020     name=key,.   
+00010860: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00010870: 613d 7661 6c75 652e 7265 6164 2829 2c0a  a=value.read(),.
+00010880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010890: 6669 6c65 6e61 6d65 3d66 696c 656e 616d  filename=filenam
+000108a0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000108b0: 2020 2068 6561 6465 7273 3d7b 2743 6f6e     headers={'Con
+000108c0: 7465 6e74 2d54 7970 6527 3a20 6775 6573  tent-Type': gues
+000108d0: 735f 636f 6e74 656e 745f 7479 7065 2866  s_content_type(f
+000108e0: 696c 656e 616d 6529 7d0a 2020 2020 2020  ilename)}.      
+000108f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010900: 2020 2020 7661 6c75 652e 636c 6f73 6528      value.close(
+00010910: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00010920: 7475 726e 2072 6571 7565 7374 5f66 6965  turn request_fie
+00010930: 6c64 0a20 2020 2020 2020 2065 6c73 653a  ld.        else:
+00010940: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010950: 7572 6e20 7365 6c66 2e5f 5f6d 756c 7469  urn self.__multi
+00010960: 7061 7274 5f6a 736f 6e5f 6974 656d 286b  part_json_item(k
+00010970: 6579 3d6b 6579 2c20 7661 6c75 653d 7661  ey=key, value=va
+00010980: 6c75 6529 0a0a 2020 2020 6465 6620 5f5f  lue)..    def __
+00010990: 7365 7269 616c 697a 655f 6d75 6c74 6970  serialize_multip
+000109a0: 6172 745f 666f 726d 5f64 6174 6128 0a20  art_form_data(. 
+000109b0: 2020 2020 2020 2073 656c 662c 2069 6e5f         self, in_
+000109c0: 6461 7461 3a20 5363 6865 6d61 0a20 2020  data: Schema.   
+000109d0: 2029 202d 3e20 7479 7069 6e67 2e44 6963   ) -> typing.Dic
+000109e0: 745b 7374 722c 2074 7970 696e 672e 5475  t[str, typing.Tu
+000109f0: 706c 655b 5265 7175 6573 7446 6965 6c64  ple[RequestField
+00010a00: 2c20 2e2e 2e5d 5d3a 0a20 2020 2020 2020  , ...]]:.       
+00010a10: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00010a20: 6365 2869 6e5f 6461 7461 2c20 6672 6f7a  ce(in_data, froz
+00010a30: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
+00010a40: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00010a50: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00010a60: 2866 2755 6e61 626c 6520 746f 2073 6572  (f'Unable to ser
+00010a70: 6961 6c69 7a65 207b 696e 5f64 6174 617d  ialize {in_data}
+00010a80: 2074 6f20 6d75 6c74 6970 6172 742f 666f   to multipart/fo
+00010a90: 726d 2d64 6174 6120 6265 6361 7573 6520  rm-data because 
+00010aa0: 6974 2069 7320 6e6f 7420 6120 6469 6374  it is not a dict
+00010ab0: 206f 6620 6461 7461 2729 0a20 2020 2020   of data').     
+00010ac0: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
+00010ad0: 6e20 6120 6d75 6c74 6970 6172 742f 666f  n a multipart/fo
+00010ae0: 726d 2d64 6174 6120 7265 7175 6573 7420  rm-data request 
+00010af0: 626f 6479 2c20 6561 6368 2073 6368 656d  body, each schem
+00010b00: 6120 7072 6f70 6572 7479 2c20 6f72 2065  a property, or e
+00010b10: 6163 6820 656c 656d 656e 7420 6f66 2061  ach element of a
+00010b20: 2073 6368 656d 6120 6172 7261 7920 7072   schema array pr
+00010b30: 6f70 6572 7479 2c0a 2020 2020 2020 2020  operty,.        
+00010b40: 7461 6b65 7320 6120 7365 6374 696f 6e20  takes a section 
+00010b50: 696e 2074 6865 2070 6179 6c6f 6164 2077  in the payload w
+00010b60: 6974 6820 616e 2069 6e74 6572 6e61 6c20  ith an internal 
+00010b70: 6865 6164 6572 2061 7320 6465 6669 6e65  header as define
+00010b80: 6420 6279 2052 4643 3735 3738 2e20 5468  d by RFC7578. Th
+00010b90: 6520 7365 7269 616c 697a 6174 696f 6e20  e serialization 
+00010ba0: 7374 7261 7465 6779 0a20 2020 2020 2020  strategy.       
+00010bb0: 2066 6f72 2065 6163 6820 7072 6f70 6572   for each proper
+00010bc0: 7479 206f 6620 6120 6d75 6c74 6970 6172  ty of a multipar
+00010bd0: 742f 666f 726d 2d64 6174 6120 7265 7175  t/form-data requ
+00010be0: 6573 7420 626f 6479 2063 616e 2062 6520  est body can be 
+00010bf0: 7370 6563 6966 6965 6420 696e 2061 6e20  specified in an 
+00010c00: 6173 736f 6369 6174 6564 2045 6e63 6f64  associated Encod
+00010c10: 696e 6720 4f62 6a65 6374 2e0a 0a20 2020  ing Object...   
+00010c20: 2020 2020 2057 6865 6e20 7061 7373 696e       When passin
+00010c30: 6720 696e 206d 756c 7469 7061 7274 2074  g in multipart t
+00010c40: 7970 6573 2c20 626f 756e 6461 7269 6573  ypes, boundaries
+00010c50: 204d 4159 2062 6520 7573 6564 2074 6f20   MAY be used to 
+00010c60: 7365 7061 7261 7465 2073 6563 7469 6f6e  separate section
+00010c70: 7320 6f66 2074 6865 2063 6f6e 7465 6e74  s of the content
+00010c80: 2062 6569 6e67 0a20 2020 2020 2020 2074   being.        t
+00010c90: 7261 6e73 6665 7272 6564 20e2 8093 2074  ransferred ... t
+00010ca0: 6875 732c 2074 6865 2066 6f6c 6c6f 7769  hus, the followi
+00010cb0: 6e67 2064 6566 6175 6c74 2043 6f6e 7465  ng default Conte
+00010cc0: 6e74 2d54 7970 6573 2061 7265 2064 6566  nt-Types are def
+00010cd0: 696e 6564 2066 6f72 206d 756c 7469 7061  ined for multipa
+00010ce0: 7274 3a0a 0a20 2020 2020 2020 2049 6620  rt:..        If 
+00010cf0: 7468 6520 286f 626a 6563 7429 2070 726f  the (object) pro
+00010d00: 7065 7274 7920 6973 2061 2070 7269 6d69  perty is a primi
+00010d10: 7469 7665 2c20 6f72 2061 6e20 6172 7261  tive, or an arra
+00010d20: 7920 6f66 2070 7269 6d69 7469 7665 2076  y of primitive v
+00010d30: 616c 7565 732c 2074 6865 2064 6566 6175  alues, the defau
+00010d40: 6c74 2043 6f6e 7465 6e74 2d54 7970 6520  lt Content-Type 
+00010d50: 6973 2074 6578 742f 706c 6169 6e0a 2020  is text/plain.  
+00010d60: 2020 2020 2020 4966 2074 6865 2070 726f        If the pro
+00010d70: 7065 7274 7920 6973 2063 6f6d 706c 6578  perty is complex
+00010d80: 2c20 6f72 2061 6e20 6172 7261 7920 6f66  , or an array of
+00010d90: 2063 6f6d 706c 6578 2076 616c 7565 732c   complex values,
+00010da0: 2074 6865 2064 6566 6175 6c74 2043 6f6e   the default Con
+00010db0: 7465 6e74 2d54 7970 6520 6973 2061 7070  tent-Type is app
+00010dc0: 6c69 6361 7469 6f6e 2f6a 736f 6e0a 2020  lication/json.  
+00010dd0: 2020 2020 2020 2020 2020 5175 6573 7469            Questi
+00010de0: 6f6e 3a20 686f 7720 6973 2074 6865 2061  on: how is the a
+00010df0: 7272 6179 206f 6620 7072 696d 6974 6976  rray of primitiv
+00010e00: 6573 2065 6e63 6f64 6564 3f0a 2020 2020  es encoded?.    
+00010e10: 2020 2020 4966 2074 6865 2070 726f 7065      If the prope
+00010e20: 7274 7920 6973 2061 2074 7970 653a 2073  rty is a type: s
+00010e30: 7472 696e 6720 7769 7468 2061 2063 6f6e  tring with a con
+00010e40: 7465 6e74 456e 636f 6469 6e67 2c20 7468  tentEncoding, th
+00010e50: 6520 6465 6661 756c 7420 436f 6e74 656e  e default Conten
+00010e60: 742d 5479 7065 2069 7320 6170 706c 6963  t-Type is applic
+00010e70: 6174 696f 6e2f 6f63 7465 742d 7374 7265  ation/octet-stre
+00010e80: 616d 0a20 2020 2020 2020 2022 2222 0a20  am.        """. 
+00010e90: 2020 2020 2020 2066 6965 6c64 733a 2074         fields: t
+00010ea0: 7970 696e 672e 4c69 7374 5b52 6571 7565  yping.List[Reque
+00010eb0: 7374 4669 656c 645d 203d 205b 5d0a 2020  stField] = [].  
+00010ec0: 2020 2020 2020 666f 7220 6b65 792c 2076        for key, v
+00010ed0: 616c 7565 2069 6e20 696e 5f64 6174 612e  alue in in_data.
+00010ee0: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00010ef0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00010f00: 6365 2876 616c 7565 2c20 7475 706c 6529  ce(value, tuple)
+00010f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010f20: 2020 6966 2076 616c 7565 3a0a 2020 2020    if value:.    
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 2320 7661 6c75 6573 2075 7365 2065 7870  # values use exp
+00010f50: 6c6f 6465 203d 2054 7275 652c 2073 6f20  lode = True, so 
+00010f60: 7468 6520 636f 6465 206d 616b 6573 2061  the code makes a
+00010f70: 2052 6571 7565 7374 4669 656c 6420 666f   RequestField fo
+00010f80: 7220 6561 6368 2069 7465 6d20 7769 7468  r each item with
+00010f90: 206e 616d 653d 6b65 790a 2020 2020 2020   name=key.      
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010fb0: 7220 6974 656d 2069 6e20 7661 6c75 653a  r item in value:
+00010fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010fd0: 2020 2020 2020 2020 2072 6571 7565 7374           request
+00010fe0: 5f66 6965 6c64 203d 2073 656c 662e 5f5f  _field = self.__
+00010ff0: 6d75 6c74 6970 6172 745f 666f 726d 5f69  multipart_form_i
+00011000: 7465 6d28 6b65 793d 6b65 792c 2076 616c  tem(key=key, val
+00011010: 7565 3d69 7465 6d29 0a20 2020 2020 2020  ue=item).       
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2066 6965 6c64 732e 6170 7065 6e64 2872   fields.append(r
+00011040: 6571 7565 7374 5f66 6965 6c64 290a 2020  equest_field).  
+00011050: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00011060: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011070: 2020 2020 2020 2020 2320 7365 6e64 2061          # send a
+00011080: 6e20 656d 7074 7920 6172 7261 7920 6173  n empty array as
+00011090: 206a 736f 6e20 6265 6361 7573 6520 6578   json because ex
+000110a0: 706c 6f64 696e 6720 7769 6c6c 206e 6f74  ploding will not
+000110b0: 2073 656e 6420 6974 0a20 2020 2020 2020   send it.       
+000110c0: 2020 2020 2020 2020 2020 2020 2072 6571               req
+000110d0: 7565 7374 5f66 6965 6c64 203d 2073 656c  uest_field = sel
+000110e0: 662e 5f5f 6d75 6c74 6970 6172 745f 6a73  f.__multipart_js
+000110f0: 6f6e 5f69 7465 6d28 6b65 793d 6b65 792c  on_item(key=key,
+00011100: 2076 616c 7565 3d76 616c 7565 290a 2020   value=value).  
 00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 6669 656c 6473 2e61 7070 656e 6428 7265  fields.append(re
-00011130: 7175 6573 745f 6669 656c 6429 0a20 2020  quest_field).   
-00011140: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00011150: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00011160: 6571 7565 7374 5f66 6965 6c64 203d 2073  equest_field = s
-00011170: 656c 662e 5f5f 6d75 6c74 6970 6172 745f  elf.__multipart_
-00011180: 666f 726d 5f69 7465 6d28 6b65 793d 6b65  form_item(key=ke
-00011190: 792c 2076 616c 7565 3d76 616c 7565 290a  y, value=value).
-000111a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111b0: 6669 656c 6473 2e61 7070 656e 6428 7265  fields.append(re
-000111c0: 7175 6573 745f 6669 656c 6429 0a0a 2020  quest_field)..  
-000111d0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
-000111e0: 6e65 6365 7373 6172 7920 746f 2066 696c  necessary to fil
-000111f0: 6c20 7468 6520 2243 6f6e 7465 6e74 2d44  l the "Content-D
-00011200: 6973 706f 7369 7469 6f6e 2220 6865 6164  isposition" head
-00011210: 6572 206e 6565 6465 6420 666f 7220 6e61  er needed for na
-00011220: 6d69 6e67 2066 6965 6c64 7320 696e 206d  ming fields in m
-00011230: 756c 7469 7061 7274 0a20 2020 2020 2020  ultipart.       
-00011240: 2066 6f72 2066 6965 6c64 2069 6e20 6669   for field in fi
-00011250: 656c 6473 3a0a 2020 2020 2020 2020 2020  elds:.          
-00011260: 2020 6669 656c 642e 6d61 6b65 5f6d 756c    field.make_mul
-00011270: 7469 7061 7274 2863 6f6e 7465 6e74 5f74  tipart(content_t
-00011280: 7970 653d 6669 656c 642e 6865 6164 6572  ype=field.header
-00011290: 735b 2243 6f6e 7465 6e74 2d54 7970 6522  s["Content-Type"
-000112a0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-000112b0: 6e20 6469 6374 2866 6965 6c64 733d 7475  n dict(fields=tu
-000112c0: 706c 6528 6669 656c 6473 2929 0a0a 2020  ple(fields))..  
-000112d0: 2020 6465 6620 5f5f 7365 7269 616c 697a    def __serializ
-000112e0: 655f 6170 706c 6963 6174 696f 6e5f 6f63  e_application_oc
-000112f0: 7465 745f 7374 7265 616d 2873 656c 662c  tet_stream(self,
-00011300: 2069 6e5f 6461 7461 3a20 4269 6e61 7279   in_data: Binary
-00011310: 5363 6865 6d61 2920 2d3e 2074 7970 696e  Schema) -> typin
-00011320: 672e 4469 6374 5b73 7472 2c20 6279 7465  g.Dict[str, byte
-00011330: 735d 3a0a 2020 2020 2020 2020 6966 2069  s]:.        if i
-00011340: 7369 6e73 7461 6e63 6528 696e 5f64 6174  sinstance(in_dat
-00011350: 612c 2062 7974 6573 293a 0a20 2020 2020  a, bytes):.     
-00011360: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-00011370: 6374 2862 6f64 793d 696e 5f64 6174 6129  ct(body=in_data)
-00011380: 0a20 2020 2020 2020 2023 2046 696c 6549  .        # FileI
-00011390: 4f20 7479 7065 0a20 2020 2020 2020 2072  O type.        r
-000113a0: 6573 756c 7420 3d20 6469 6374 2862 6f64  esult = dict(bod
-000113b0: 793d 696e 5f64 6174 612e 7265 6164 2829  y=in_data.read()
-000113c0: 290a 2020 2020 2020 2020 696e 5f64 6174  ).        in_dat
-000113d0: 612e 636c 6f73 6528 290a 2020 2020 2020  a.close().      
-000113e0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000113f0: 0a20 2020 2064 6566 205f 5f73 6572 6961  .    def __seria
-00011400: 6c69 7a65 5f61 7070 6c69 6361 7469 6f6e  lize_application
-00011410: 5f78 5f77 7777 5f66 6f72 6d5f 6461 7461  _x_www_form_data
-00011420: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00011430: 696e 5f64 6174 613a 2074 7970 696e 672e  in_data: typing.
-00011440: 416e 790a 2020 2020 2920 2d3e 2053 6572  Any.    ) -> Ser
-00011450: 6961 6c69 7a65 6452 6571 7565 7374 426f  ializedRequestBo
-00011460: 6479 3a0a 2020 2020 2020 2020 2222 220a  dy:.        """.
-00011470: 2020 2020 2020 2020 504f 5354 2073 7562          POST sub
-00011480: 6d69 7373 696f 6e20 6f66 2066 6f72 6d20  mission of form 
-00011490: 6461 7461 2069 6e20 626f 6479 0a20 2020  data in body.   
-000114a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000114b0: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-000114c0: 6365 2869 6e5f 6461 7461 2c20 6672 6f7a  ce(in_data, froz
-000114d0: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
-000114e0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000114f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00011500: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011510: 2020 6627 556e 6162 6c65 2074 6f20 7365    f'Unable to se
-00011520: 7269 616c 697a 6520 7b69 6e5f 6461 7461  rialize {in_data
-00011530: 7d20 746f 2061 7070 6c69 6361 7469 6f6e  } to application
-00011540: 2f78 2d77 7777 2d66 6f72 6d2d 7572 6c65  /x-www-form-urle
-00011550: 6e63 6f64 6564 2062 6563 6175 7365 2069  ncoded because i
-00011560: 7420 6973 206e 6f74 2061 2064 6963 7420  t is not a dict 
-00011570: 6f66 2064 6174 6127 290a 2020 2020 2020  of data').      
-00011580: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
-00011590: 2073 656c 662e 5f5f 6a73 6f6e 5f65 6e63   self.__json_enc
-000115a0: 6f64 6572 2e64 6566 6175 6c74 2869 6e5f  oder.default(in_
-000115b0: 6461 7461 290a 2020 2020 2020 2020 7661  data).        va
-000115c0: 6c75 6520 3d20 7365 6c66 2e5f 7365 7269  lue = self._seri
-000115d0: 616c 697a 655f 666f 726d 2863 6173 745f  alize_form(cast_
-000115e0: 696e 5f64 6174 612c 206e 616d 653d 2727  in_data, name=''
-000115f0: 2c20 6578 706c 6f64 653d 5472 7565 2c20  , explode=True, 
-00011600: 7065 7263 656e 745f 656e 636f 6465 3d54  percent_encode=T
-00011610: 7275 6529 0a20 2020 2020 2020 2072 6574  rue).        ret
-00011620: 7572 6e20 6469 6374 2862 6f64 793d 7661  urn dict(body=va
-00011630: 6c75 6529 0a0a 2020 2020 6465 6620 7365  lue)..    def se
-00011640: 7269 616c 697a 6528 0a20 2020 2020 2020  rialize(.       
-00011650: 2073 656c 662c 2069 6e5f 6461 7461 3a20   self, in_data: 
-00011660: 7479 7069 6e67 2e41 6e79 2c20 636f 6e74  typing.Any, cont
-00011670: 656e 745f 7479 7065 3a20 7374 720a 2020  ent_type: str.  
-00011680: 2020 2920 2d3e 2053 6572 6961 6c69 7a65    ) -> Serialize
-00011690: 6452 6571 7565 7374 426f 6479 3a0a 2020  dRequestBody:.  
-000116a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000116b0: 2020 4966 2061 2073 7472 2069 7320 7265    If a str is re
-000116c0: 7475 726e 6564 2074 6865 6e20 7468 6520  turned then the 
-000116d0: 7265 7375 6c74 2077 696c 6c20 6265 2061  result will be a
-000116e0: 7373 6967 6e65 6420 746f 2064 6174 6120  ssigned to data 
-000116f0: 7768 656e 206d 616b 696e 6720 7468 6520  when making the 
-00011700: 7265 7175 6573 740a 2020 2020 2020 2020  request.        
-00011710: 4966 2061 2074 7570 6c65 2069 7320 7265  If a tuple is re
-00011720: 7475 726e 6564 2074 6865 6e20 7468 6520  turned then the 
-00011730: 7265 7375 6c74 2077 696c 6c20 6265 2075  result will be u
-00011740: 7365 6420 6173 2066 6965 6c64 7320 696e  sed as fields in
-00011750: 7075 7420 696e 2065 6e63 6f64 655f 6d75  put in encode_mu
-00011760: 6c74 6970 6172 745f 666f 726d 6461 7461  ltipart_formdata
-00011770: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-00011780: 6120 7475 706c 6520 6f66 0a0a 2020 2020  a tuple of..    
-00011790: 2020 2020 5468 6520 6b65 7920 6f66 2074      The key of t
-000117a0: 6865 2072 6574 7572 6e20 6469 6374 2069  he return dict i
-000117b0: 730a 2020 2020 2020 2020 2d20 626f 6479  s.        - body
-000117c0: 2066 6f72 2061 7070 6c69 6361 7469 6f6e   for application
-000117d0: 2f6a 736f 6e0a 2020 2020 2020 2020 2d20  /json.        - 
-000117e0: 656e 636f 6465 5f6d 756c 7469 7061 7274  encode_multipart
-000117f0: 2061 6e64 2066 6965 6c64 7320 666f 7220   and fields for 
-00011800: 6d75 6c74 6970 6172 742f 666f 726d 2d64  multipart/form-d
-00011810: 6174 610a 2020 2020 2020 2020 2222 220a  ata.        """.
-00011820: 2020 2020 2020 2020 6d65 6469 615f 7479          media_ty
-00011830: 7065 203d 2073 656c 662e 636f 6e74 656e  pe = self.conten
-00011840: 745b 636f 6e74 656e 745f 7479 7065 5d0a  t[content_type].
-00011850: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00011860: 7461 6e63 6528 696e 5f64 6174 612c 206d  tance(in_data, m
-00011870: 6564 6961 5f74 7970 652e 7363 6865 6d61  edia_type.schema
-00011880: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00011890: 6173 745f 696e 5f64 6174 6120 3d20 696e  ast_in_data = in
-000118a0: 5f64 6174 610a 2020 2020 2020 2020 656c  _data.        el
-000118b0: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
-000118c0: 5f64 6174 612c 2028 6469 6374 2c20 6672  _data, (dict, fr
-000118d0: 6f7a 656e 6469 6374 2e66 726f 7a65 6e64  ozendict.frozend
-000118e0: 6963 7429 2920 616e 6420 696e 5f64 6174  ict)) and in_dat
-000118f0: 613a 0a20 2020 2020 2020 2020 2020 2074  a:.            t
-00011900: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00011910: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
-00011920: 203d 206d 6564 6961 5f74 7970 652e 7363   = media_type.sc
-00011930: 6865 6d61 282a 2a69 6e5f 6461 7461 290a  hema(**in_data).
-00011940: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00011950: 7074 2054 7970 6545 7272 6f72 2061 7320  pt TypeError as 
-00011960: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011970: 2020 2072 6169 7365 204d 6973 7369 6e67     raise Missing
-00011980: 5265 7175 6972 6564 5061 7261 6d65 7465  RequiredParamete
-00011990: 7273 4572 726f 7228 6529 0a20 2020 2020  rsError(e).     
-000119a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000119b0: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
-000119c0: 6120 3d20 6d65 6469 615f 7479 7065 2e73  a = media_type.s
-000119d0: 6368 656d 6128 696e 5f64 6174 6129 0a20  chema(in_data). 
-000119e0: 2020 2020 2020 2023 2054 4f44 4f20 6368         # TODO ch
-000119f0: 6563 6b20 666f 7220 616e 6420 7573 6520  eck for and use 
-00011a00: 656e 636f 6469 6e67 2069 6620 6974 2065  encoding if it e
-00011a10: 7869 7374 730a 2020 2020 2020 2020 2320  xists.        # 
-00011a20: 616e 6420 636f 6e74 656e 745f 7479 7065  and content_type
-00011a30: 2069 7320 6d75 6c74 6970 6172 7420 6f72   is multipart or
-00011a40: 2061 7070 6c69 6361 7469 6f6e 2f78 2d77   application/x-w
-00011a50: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
-00011a60: 6564 0a20 2020 2020 2020 2069 6620 7365  ed.        if se
-00011a70: 6c66 2e5f 636f 6e74 656e 745f 7479 7065  lf._content_type
-00011a80: 5f69 735f 6a73 6f6e 2863 6f6e 7465 6e74  _is_json(content
-00011a90: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
-00011aa0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011ab0: 5f5f 7365 7269 616c 697a 655f 6a73 6f6e  __serialize_json
-00011ac0: 2863 6173 745f 696e 5f64 6174 6129 0a20  (cast_in_data). 
-00011ad0: 2020 2020 2020 2065 6c69 6620 636f 6e74         elif cont
-00011ae0: 656e 745f 7479 7065 203d 3d20 2774 6578  ent_type == 'tex
-00011af0: 742f 706c 6169 6e27 3a0a 2020 2020 2020  t/plain':.      
-00011b00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00011b10: 662e 5f5f 7365 7269 616c 697a 655f 7465  f.__serialize_te
-00011b20: 7874 5f70 6c61 696e 2863 6173 745f 696e  xt_plain(cast_in
-00011b30: 5f64 6174 6129 0a20 2020 2020 2020 2065  _data).        e
-00011b40: 6c69 6620 636f 6e74 656e 745f 7479 7065  lif content_type
-00011b50: 203d 3d20 276d 756c 7469 7061 7274 2f66   == 'multipart/f
-00011b60: 6f72 6d2d 6461 7461 273a 0a20 2020 2020  orm-data':.     
-00011b70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011b80: 6c66 2e5f 5f73 6572 6961 6c69 7a65 5f6d  lf.__serialize_m
-00011b90: 756c 7469 7061 7274 5f66 6f72 6d5f 6461  ultipart_form_da
-00011ba0: 7461 2863 6173 745f 696e 5f64 6174 6129  ta(cast_in_data)
-00011bb0: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
-00011bc0: 6e74 656e 745f 7479 7065 203d 3d20 2761  ntent_type == 'a
-00011bd0: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
-00011be0: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
-00011bf0: 273a 0a20 2020 2020 2020 2020 2020 2072  ':.            r
-00011c00: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
-00011c10: 6961 6c69 7a65 5f61 7070 6c69 6361 7469  ialize_applicati
-00011c20: 6f6e 5f78 5f77 7777 5f66 6f72 6d5f 6461  on_x_www_form_da
-00011c30: 7461 2863 6173 745f 696e 5f64 6174 6129  ta(cast_in_data)
-00011c40: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
-00011c50: 6e74 656e 745f 7479 7065 203d 3d20 2761  ntent_type == 'a
-00011c60: 7070 6c69 6361 7469 6f6e 2f6f 6374 6574  pplication/octet
-00011c70: 2d73 7472 6561 6d27 3a0a 2020 2020 2020  -stream':.      
-00011c80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00011c90: 662e 5f5f 7365 7269 616c 697a 655f 6170  f.__serialize_ap
-00011ca0: 706c 6963 6174 696f 6e5f 6f63 7465 745f  plication_octet_
-00011cb0: 7374 7265 616d 2863 6173 745f 696e 5f64  stream(cast_in_d
-00011cc0: 6174 6129 0a20 2020 2020 2020 2072 6169  ata).        rai
-00011cd0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00011ce0: 6445 7272 6f72 2827 5365 7269 616c 697a  dError('Serializ
-00011cf0: 6174 696f 6e20 6861 7320 6e6f 7420 7965  ation has not ye
-00011d00: 7420 6265 656e 2069 6d70 6c65 6d65 6e74  t been implement
-00011d10: 6564 2066 6f72 207b 7d27 2e66 6f72 6d61  ed for {}'.forma
-00011d20: 7428 636f 6e74 656e 745f 7479 7065 2929  t(content_type))
-00011d30: 0a                                       .
+00011120: 2020 6669 656c 6473 2e61 7070 656e 6428    fields.append(
+00011130: 7265 7175 6573 745f 6669 656c 6429 0a20  request_field). 
+00011140: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011160: 2072 6571 7565 7374 5f66 6965 6c64 203d   request_field =
+00011170: 2073 656c 662e 5f5f 6d75 6c74 6970 6172   self.__multipar
+00011180: 745f 666f 726d 5f69 7465 6d28 6b65 793d  t_form_item(key=
+00011190: 6b65 792c 2076 616c 7565 3d76 616c 7565  key, value=value
+000111a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000111b0: 2020 6669 656c 6473 2e61 7070 656e 6428    fields.append(
+000111c0: 7265 7175 6573 745f 6669 656c 6429 0a0a  request_field)..
+000111d0: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
+000111e0: 7320 6e65 6365 7373 6172 7920 746f 2066  s necessary to f
+000111f0: 696c 6c20 7468 6520 2243 6f6e 7465 6e74  ill the "Content
+00011200: 2d44 6973 706f 7369 7469 6f6e 2220 6865  -Disposition" he
+00011210: 6164 6572 206e 6565 6465 6420 666f 7220  ader needed for 
+00011220: 6e61 6d69 6e67 2066 6965 6c64 7320 696e  naming fields in
+00011230: 206d 756c 7469 7061 7274 0a20 2020 2020   multipart.     
+00011240: 2020 2066 6f72 2066 6965 6c64 2069 6e20     for field in 
+00011250: 6669 656c 6473 3a0a 2020 2020 2020 2020  fields:.        
+00011260: 2020 2020 6669 656c 642e 6d61 6b65 5f6d      field.make_m
+00011270: 756c 7469 7061 7274 2863 6f6e 7465 6e74  ultipart(content
+00011280: 5f74 7970 653d 6669 656c 642e 6865 6164  _type=field.head
+00011290: 6572 735b 2243 6f6e 7465 6e74 2d54 7970  ers["Content-Typ
+000112a0: 6522 5d29 0a20 2020 2020 2020 2072 6574  e"]).        ret
+000112b0: 7572 6e20 6469 6374 2866 6965 6c64 733d  urn dict(fields=
+000112c0: 7475 706c 6528 6669 656c 6473 2929 0a0a  tuple(fields))..
+000112d0: 2020 2020 6465 6620 5f5f 7365 7269 616c      def __serial
+000112e0: 697a 655f 6170 706c 6963 6174 696f 6e5f  ize_application_
+000112f0: 6f63 7465 745f 7374 7265 616d 2873 656c  octet_stream(sel
+00011300: 662c 2069 6e5f 6461 7461 3a20 4269 6e61  f, in_data: Bina
+00011310: 7279 5363 6865 6d61 2920 2d3e 2074 7970  rySchema) -> typ
+00011320: 696e 672e 4469 6374 5b73 7472 2c20 6279  ing.Dict[str, by
+00011330: 7465 735d 3a0a 2020 2020 2020 2020 6966  tes]:.        if
+00011340: 2069 7369 6e73 7461 6e63 6528 696e 5f64   isinstance(in_d
+00011350: 6174 612c 2062 7974 6573 293a 0a20 2020  ata, bytes):.   
+00011360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011370: 6469 6374 2862 6f64 793d 696e 5f64 6174  dict(body=in_dat
+00011380: 6129 0a20 2020 2020 2020 2023 2046 696c  a).        # Fil
+00011390: 6549 4f20 7479 7065 0a20 2020 2020 2020  eIO type.       
+000113a0: 2072 6573 756c 7420 3d20 6469 6374 2862   result = dict(b
+000113b0: 6f64 793d 696e 5f64 6174 612e 7265 6164  ody=in_data.read
+000113c0: 2829 290a 2020 2020 2020 2020 696e 5f64  ()).        in_d
+000113d0: 6174 612e 636c 6f73 6528 290a 2020 2020  ata.close().    
+000113e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000113f0: 740a 0a20 2020 2064 6566 205f 5f73 6572  t..    def __ser
+00011400: 6961 6c69 7a65 5f61 7070 6c69 6361 7469  ialize_applicati
+00011410: 6f6e 5f78 5f77 7777 5f66 6f72 6d5f 6461  on_x_www_form_da
+00011420: 7461 280a 2020 2020 2020 2020 7365 6c66  ta(.        self
+00011430: 2c20 696e 5f64 6174 613a 2074 7970 696e  , in_data: typin
+00011440: 672e 416e 790a 2020 2020 2920 2d3e 2053  g.Any.    ) -> S
+00011450: 6572 6961 6c69 7a65 6452 6571 7565 7374  erializedRequest
+00011460: 426f 6479 3a0a 2020 2020 2020 2020 2222  Body:.        ""
+00011470: 220a 2020 2020 2020 2020 504f 5354 2073  ".        POST s
+00011480: 7562 6d69 7373 696f 6e20 6f66 2066 6f72  ubmission of for
+00011490: 6d20 6461 7461 2069 6e20 626f 6479 0a20  m data in body. 
+000114a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000114b0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+000114c0: 616e 6365 2869 6e5f 6461 7461 2c20 6672  ance(in_data, fr
+000114d0: 6f7a 656e 6469 6374 2e66 726f 7a65 6e64  ozendict.frozend
+000114e0: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
+000114f0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00011500: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00011510: 2020 2020 6627 556e 6162 6c65 2074 6f20      f'Unable to 
+00011520: 7365 7269 616c 697a 6520 7b69 6e5f 6461  serialize {in_da
+00011530: 7461 7d20 746f 2061 7070 6c69 6361 7469  ta} to applicati
+00011540: 6f6e 2f78 2d77 7777 2d66 6f72 6d2d 7572  on/x-www-form-ur
+00011550: 6c65 6e63 6f64 6564 2062 6563 6175 7365  lencoded because
+00011560: 2069 7420 6973 206e 6f74 2061 2064 6963   it is not a dic
+00011570: 7420 6f66 2064 6174 6127 290a 2020 2020  t of data').    
+00011580: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
+00011590: 203d 2073 656c 662e 5f5f 6a73 6f6e 5f65   = self.__json_e
+000115a0: 6e63 6f64 6572 2e64 6566 6175 6c74 2869  ncoder.default(i
+000115b0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+000115c0: 7661 6c75 6520 3d20 7365 6c66 2e5f 7365  value = self._se
+000115d0: 7269 616c 697a 655f 666f 726d 2863 6173  rialize_form(cas
+000115e0: 745f 696e 5f64 6174 612c 206e 616d 653d  t_in_data, name=
+000115f0: 2727 2c20 6578 706c 6f64 653d 5472 7565  '', explode=True
+00011600: 2c20 7065 7263 656e 745f 656e 636f 6465  , percent_encode
+00011610: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00011620: 6574 7572 6e20 6469 6374 2862 6f64 793d  eturn dict(body=
+00011630: 7661 6c75 6529 0a0a 2020 2020 6465 6620  value)..    def 
+00011640: 7365 7269 616c 697a 6528 0a20 2020 2020  serialize(.     
+00011650: 2020 2073 656c 662c 2069 6e5f 6461 7461     self, in_data
+00011660: 3a20 7479 7069 6e67 2e41 6e79 2c20 636f  : typing.Any, co
+00011670: 6e74 656e 745f 7479 7065 3a20 7374 720a  ntent_type: str.
+00011680: 2020 2020 2920 2d3e 2053 6572 6961 6c69      ) -> Seriali
+00011690: 7a65 6452 6571 7565 7374 426f 6479 3a0a  zedRequestBody:.
+000116a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000116b0: 2020 2020 4966 2061 2073 7472 2069 7320      If a str is 
+000116c0: 7265 7475 726e 6564 2074 6865 6e20 7468  returned then th
+000116d0: 6520 7265 7375 6c74 2077 696c 6c20 6265  e result will be
+000116e0: 2061 7373 6967 6e65 6420 746f 2064 6174   assigned to dat
+000116f0: 6120 7768 656e 206d 616b 696e 6720 7468  a when making th
+00011700: 6520 7265 7175 6573 740a 2020 2020 2020  e request.      
+00011710: 2020 4966 2061 2074 7570 6c65 2069 7320    If a tuple is 
+00011720: 7265 7475 726e 6564 2074 6865 6e20 7468  returned then th
+00011730: 6520 7265 7375 6c74 2077 696c 6c20 6265  e result will be
+00011740: 2075 7365 6420 6173 2066 6965 6c64 7320   used as fields 
+00011750: 696e 7075 7420 696e 2065 6e63 6f64 655f  input in encode_
+00011760: 6d75 6c74 6970 6172 745f 666f 726d 6461  multipart_formda
+00011770: 7461 0a20 2020 2020 2020 2052 6574 7572  ta.        Retur
+00011780: 6e20 6120 7475 706c 6520 6f66 0a0a 2020  n a tuple of..  
+00011790: 2020 2020 2020 5468 6520 6b65 7920 6f66        The key of
+000117a0: 2074 6865 2072 6574 7572 6e20 6469 6374   the return dict
+000117b0: 2069 730a 2020 2020 2020 2020 2d20 626f   is.        - bo
+000117c0: 6479 2066 6f72 2061 7070 6c69 6361 7469  dy for applicati
+000117d0: 6f6e 2f6a 736f 6e0a 2020 2020 2020 2020  on/json.        
+000117e0: 2d20 656e 636f 6465 5f6d 756c 7469 7061  - encode_multipa
+000117f0: 7274 2061 6e64 2066 6965 6c64 7320 666f  rt and fields fo
+00011800: 7220 6d75 6c74 6970 6172 742f 666f 726d  r multipart/form
+00011810: 2d64 6174 610a 2020 2020 2020 2020 2222  -data.        ""
+00011820: 220a 2020 2020 2020 2020 6d65 6469 615f  ".        media_
+00011830: 7479 7065 203d 2073 656c 662e 636f 6e74  type = self.cont
+00011840: 656e 745b 636f 6e74 656e 745f 7479 7065  ent[content_type
+00011850: 5d0a 2020 2020 2020 2020 6966 2069 7369  ].        if isi
+00011860: 6e73 7461 6e63 6528 696e 5f64 6174 612c  nstance(in_data,
+00011870: 206d 6564 6961 5f74 7970 652e 7363 6865   media_type.sche
+00011880: 6d61 293a 0a20 2020 2020 2020 2020 2020  ma):.           
+00011890: 2063 6173 745f 696e 5f64 6174 6120 3d20   cast_in_data = 
+000118a0: 696e 5f64 6174 610a 2020 2020 2020 2020  in_data.        
+000118b0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+000118c0: 696e 5f64 6174 612c 2028 6469 6374 2c20  in_data, (dict, 
+000118d0: 6672 6f7a 656e 6469 6374 2e66 726f 7a65  frozendict.froze
+000118e0: 6e64 6963 7429 2920 616e 6420 696e 5f64  ndict)) and in_d
+000118f0: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00011900: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00011910: 2020 2020 2020 6361 7374 5f69 6e5f 6461        cast_in_da
+00011920: 7461 203d 206d 6564 6961 5f74 7970 652e  ta = media_type.
+00011930: 7363 6865 6d61 282a 2a69 6e5f 6461 7461  schema(**in_data
+00011940: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+00011950: 6365 7074 2054 7970 6545 7272 6f72 2061  cept TypeError a
+00011960: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00011970: 2020 2020 2072 6169 7365 204d 6973 7369       raise Missi
+00011980: 6e67 5265 7175 6972 6564 5061 7261 6d65  ngRequiredParame
+00011990: 7465 7273 4572 726f 7228 6529 0a20 2020  tersError(e).   
+000119a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000119b0: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
+000119c0: 6174 6120 3d20 6d65 6469 615f 7479 7065  ata = media_type
+000119d0: 2e73 6368 656d 6128 696e 5f64 6174 6129  .schema(in_data)
+000119e0: 0a20 2020 2020 2020 2023 2054 4f44 4f20  .        # TODO 
+000119f0: 6368 6563 6b20 666f 7220 616e 6420 7573  check for and us
+00011a00: 6520 656e 636f 6469 6e67 2069 6620 6974  e encoding if it
+00011a10: 2065 7869 7374 730a 2020 2020 2020 2020   exists.        
+00011a20: 2320 616e 6420 636f 6e74 656e 745f 7479  # and content_ty
+00011a30: 7065 2069 7320 6d75 6c74 6970 6172 7420  pe is multipart 
+00011a40: 6f72 2061 7070 6c69 6361 7469 6f6e 2f78  or application/x
+00011a50: 2d77 7777 2d66 6f72 6d2d 7572 6c65 6e63  -www-form-urlenc
+00011a60: 6f64 6564 0a20 2020 2020 2020 2069 6620  oded.        if 
+00011a70: 7365 6c66 2e5f 636f 6e74 656e 745f 7479  self._content_ty
+00011a80: 7065 5f69 735f 6a73 6f6e 2863 6f6e 7465  pe_is_json(conte
+00011a90: 6e74 5f74 7970 6529 3a0a 2020 2020 2020  nt_type):.      
+00011aa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00011ab0: 662e 5f5f 7365 7269 616c 697a 655f 6a73  f.__serialize_js
+00011ac0: 6f6e 2863 6173 745f 696e 5f64 6174 6129  on(cast_in_data)
+00011ad0: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
+00011ae0: 6e74 656e 745f 7479 7065 203d 3d20 2774  ntent_type == 't
+00011af0: 6578 742f 706c 6169 6e27 3a0a 2020 2020  ext/plain':.    
+00011b00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011b10: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
+00011b20: 7465 7874 5f70 6c61 696e 2863 6173 745f  text_plain(cast_
+00011b30: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00011b40: 2065 6c69 6620 636f 6e74 656e 745f 7479   elif content_ty
+00011b50: 7065 203d 3d20 276d 756c 7469 7061 7274  pe == 'multipart
+00011b60: 2f66 6f72 6d2d 6461 7461 273a 0a20 2020  /form-data':.   
+00011b70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011b80: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
+00011b90: 5f6d 756c 7469 7061 7274 5f66 6f72 6d5f  _multipart_form_
+00011ba0: 6461 7461 2863 6173 745f 696e 5f64 6174  data(cast_in_dat
+00011bb0: 6129 0a20 2020 2020 2020 2065 6c69 6620  a).        elif 
+00011bc0: 636f 6e74 656e 745f 7479 7065 203d 3d20  content_type == 
+00011bd0: 2761 7070 6c69 6361 7469 6f6e 2f78 2d77  'application/x-w
+00011be0: 7777 2d66 6f72 6d2d 7572 6c65 6e63 6f64  ww-form-urlencod
+00011bf0: 6564 273a 0a20 2020 2020 2020 2020 2020  ed':.           
+00011c00: 2072 6574 7572 6e20 7365 6c66 2e5f 5f73   return self.__s
+00011c10: 6572 6961 6c69 7a65 5f61 7070 6c69 6361  erialize_applica
+00011c20: 7469 6f6e 5f78 5f77 7777 5f66 6f72 6d5f  tion_x_www_form_
+00011c30: 6461 7461 2863 6173 745f 696e 5f64 6174  data(cast_in_dat
+00011c40: 6129 0a20 2020 2020 2020 2065 6c69 6620  a).        elif 
+00011c50: 636f 6e74 656e 745f 7479 7065 203d 3d20  content_type == 
+00011c60: 2761 7070 6c69 6361 7469 6f6e 2f6f 6374  'application/oct
+00011c70: 6574 2d73 7472 6561 6d27 3a0a 2020 2020  et-stream':.    
+00011c80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011c90: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
+00011ca0: 6170 706c 6963 6174 696f 6e5f 6f63 7465  application_octe
+00011cb0: 745f 7374 7265 616d 2863 6173 745f 696e  t_stream(cast_in
+00011cc0: 5f64 6174 6129 0a20 2020 2020 2020 2072  _data).        r
+00011cd0: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
+00011ce0: 7465 6445 7272 6f72 2827 5365 7269 616c  tedError('Serial
+00011cf0: 697a 6174 696f 6e20 6861 7320 6e6f 7420  ization has not 
+00011d00: 7965 7420 6265 656e 2069 6d70 6c65 6d65  yet been impleme
+00011d10: 6e74 6564 2066 6f72 207b 7d27 2e66 6f72  nted for {}'.for
+00011d20: 6d61 7428 636f 6e74 656e 745f 7479 7065  mat(content_type
+00011d30: 2929 0a                                  )).
```

### Comparing `humanloop-0.4.0/humanloop/api_response.py` & `humanloop-0.4.0a4/humanloop/api_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/path_to_api.py` & `humanloop-0.4.0a4/humanloop/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tag_to_api.py` & `humanloop-0.4.0a4/humanloop/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/__init__.py` & `humanloop-0.4.0a4/humanloop/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/apps_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/apps_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/chats_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/chats_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/completions_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/completions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/experiments_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/experiments_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/feedback_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/feedback_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/logs_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/logs_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/model_configurations_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/model_configurations_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/projects_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/projects_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/apis/tags/sessions_api.py` & `humanloop-0.4.0a4/humanloop/apis/tags/sessions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/client.py` & `humanloop-0.4.0a4/humanloop/client.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/client.pyi` & `humanloop-0.4.0a4/humanloop/client.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/client_custom.py` & `humanloop-0.4.0a4/humanloop/client_custom.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,33 +30,26 @@
         api_client = ApiClient(configuration)
         self.chats = ChatsApi(api_client)
         self.completions = CompletionsApi(api_client)
 
     async def _parsed_generator(self, generator: typing.AsyncGenerator):
         async for line in generator:
             parsed = _parse_sse_chunk(line)
-            if parsed is None:
-                continue
-            try:
-                as_json = json.loads(parsed)
-
-                choice = as_json["provider_responses"][0]["choices"][0]
-                if "delta" in choice:
-                    # for /chat
-                    delta = as_json["provider_responses"][0]["choices"][0]["delta"]
-                    if "content" in delta:
-                        yield delta["content"]
-                elif "text" in choice:
-                    # for /completion
-                    yield as_json["provider_responses"][0]["choices"][0]["text"]
-                else:
-                    raise Exception("Unknown response type")
-            except Exception as e:
-                # move on silently
-                pass
+            as_json = json.loads(parsed)
+            choice = as_json["provider_responses"][0]["choices"][0]
+            if "delta" in choice:
+                # for /chat
+                delta = as_json["provider_responses"][0]["choices"][0]["delta"]
+                if "content" in delta:
+                    yield delta["content"]
+            elif "text" in choice:
+                # for /completion
+                yield as_json["provider_responses"][0]["choices"][0]["text"]
+            else:
+                raise Exception("Unknown response type")
 
     @copy_signature(ChatsApi.aresponse)
     async def chat_stream(self, *args, **kwargs):
         kwargs["stream"] = True
         args = self.chats._response_mapped_args(*args, **kwargs)
         response: AsyncGeneratorResponse = await self.chats._aresponse_oapg(stream=True, body=args.body)  # type: ignore
         return AsyncGeneratorResponse(
@@ -149,11 +142,8 @@
             content=self._parsed_generator(response.content),
             response=response.response,
         )
 
 
 def _parse_sse_chunk(chunk: bytes):
     """Parse a single Server-Sent Event byte chunk (e.g. "data: ....") and return the data (e.g. "....") as a string"""
-    decoded = chunk.decode("utf-8")
-    if "data: " not in decoded:
-        return None
-    return decoded.split("data: ")[1].strip()
+    return chunk.decode("utf-8").split("data: ")[1].strip()
```

### Comparing `humanloop-0.4.0/humanloop/configuration.py` & `humanloop-0.4.0a4/humanloop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 0.4.0".\
+               "SDK Package Version: 0.4.0a4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `humanloop-0.4.0/humanloop/exceptions.py` & `humanloop-0.4.0a4/humanloop/exceptions.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/exceptions_base.py` & `humanloop-0.4.0a4/humanloop/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/base_metric_response.py` & `humanloop-0.4.0a4/humanloop/model/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/base_metric_response.pyi` & `humanloop-0.4.0a4/humanloop/model/base_metric_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/categorical_feedback_label.py` & `humanloop-0.4.0a4/humanloop/model/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/categorical_feedback_label.pyi` & `humanloop-0.4.0a4/humanloop/model/categorical_feedback_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_data_response.py` & `humanloop-0.4.0a4/humanloop/model/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_data_response.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_deployed_request.py` & `humanloop-0.4.0a4/humanloop/model/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_deployed_request.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_experiment_request.py` & `humanloop-0.4.0a4/humanloop/model/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_experiment_request.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_message.py` & `humanloop-0.4.0a4/humanloop/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_message.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_message.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_model_config_request.py` & `humanloop-0.4.0a4/humanloop/model/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_model_config_request.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_request.py` & `humanloop-0.4.0a4/humanloop/model/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_request.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_response.py` & `humanloop-0.4.0a4/humanloop/model/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_response.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_role.py` & `humanloop-0.4.0a4/humanloop/model/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/chat_role.pyi` & `humanloop-0.4.0a4/humanloop/model/chat_role.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_deployed_request.py` & `humanloop-0.4.0a4/humanloop/model/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_deployed_request.pyi` & `humanloop-0.4.0a4/humanloop/model/completion_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_experiment_request.py` & `humanloop-0.4.0a4/humanloop/model/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_experiment_request.pyi` & `humanloop-0.4.0a4/humanloop/model/completion_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_model_config_request.py` & `humanloop-0.4.0a4/humanloop/model/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_model_config_request.pyi` & `humanloop-0.4.0a4/humanloop/model/completion_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_request.py` & `humanloop-0.4.0a4/humanloop/model/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_request.pyi` & `humanloop-0.4.0a4/humanloop/model/completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_response.py` & `humanloop-0.4.0a4/humanloop/model/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/completion_response.pyi` & `humanloop-0.4.0a4/humanloop/model/completion_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_experiment_request.py` & `humanloop-0.4.0a4/humanloop/model/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_experiment_request.pyi` & `humanloop-0.4.0a4/humanloop/model/create_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_log_response.py` & `humanloop-0.4.0a4/humanloop/model/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_log_response.pyi` & `humanloop-0.4.0a4/humanloop/model/create_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_project_request.py` & `humanloop-0.4.0a4/humanloop/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_project_request.pyi` & `humanloop-0.4.0a4/humanloop/model/create_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_session_request.py` & `humanloop-0.4.0a4/humanloop/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/create_session_request.pyi` & `humanloop-0.4.0a4/humanloop/model/create_session_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/data_response.py` & `humanloop-0.4.0a4/humanloop/model/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/data_response.pyi` & `humanloop-0.4.0a4/humanloop/model/data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/experiment_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/experiment_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_response.py` & `humanloop-0.4.0a4/humanloop/model/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_response.pyi` & `humanloop-0.4.0a4/humanloop/model/experiment_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_status.py` & `humanloop-0.4.0a4/humanloop/model/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiment_status.pyi` & `humanloop-0.4.0a4/humanloop/model/experiment_status.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiments_list_response.py` & `humanloop-0.4.0a4/humanloop/model/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/experiments_list_response.pyi` & `humanloop-0.4.0a4/humanloop/model/experiments_list_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback.py` & `humanloop-0.4.0a4/humanloop/model/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_class.py` & `humanloop-0.4.0a4/humanloop/model/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_class.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_class.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_label_request.py` & `humanloop-0.4.0a4/humanloop/model/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_label_request.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_label_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_request.py` & `humanloop-0.4.0a4/humanloop/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_request.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_response.py` & `humanloop-0.4.0a4/humanloop/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_response.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_submit_request.py` & `humanloop-0.4.0a4/humanloop/model/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_submit_request.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_submit_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_submit_response.py` & `humanloop-0.4.0a4/humanloop/model/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_submit_response.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_submit_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type.py` & `humanloop-0.4.0a4/humanloop/model/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type_model.py` & `humanloop-0.4.0a4/humanloop/model/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type_model.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_type_model.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type_request.py` & `humanloop-0.4.0a4/humanloop/model/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_type_request.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_type_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_types.py` & `humanloop-0.4.0a4/humanloop/model/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/feedback_types.pyi` & `humanloop-0.4.0a4/humanloop/model/feedback_types.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/get_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/get_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/get_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/http_validation_error.py` & `humanloop-0.4.0a4/humanloop/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/http_validation_error.pyi` & `humanloop-0.4.0a4/humanloop/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/label_sentiment.py` & `humanloop-0.4.0a4/humanloop/model/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/label_sentiment.pyi` & `humanloop-0.4.0a4/humanloop/model/label_sentiment.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_datapoint_request.py` & `humanloop-0.4.0a4/humanloop/model/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_datapoint_request.pyi` & `humanloop-0.4.0a4/humanloop/model/log_datapoint_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_request.py` & `humanloop-0.4.0a4/humanloop/model/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_request.pyi` & `humanloop-0.4.0a4/humanloop/model/log_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_response.py` & `humanloop-0.4.0a4/humanloop/model/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/log_response.pyi` & `humanloop-0.4.0a4/humanloop/model/log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/logs_log_response.py` & `humanloop-0.4.0a4/humanloop/model/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/logs_log_response.pyi` & `humanloop-0.4.0a4/humanloop/model/logs_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/model_config_chat_request.py` & `humanloop-0.4.0a4/humanloop/model/model_config_chat_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -214,15 +214,14 @@
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "endpoint": endpoint,
                 "chat_template": chat_template,
             }
-        additional_properties = schemas.NotAnyTypeSchema
     
     model: MetaOapg.properties.model
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
@@ -251,18 +250,22 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["chat_template"], ]):
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "chat_template", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
@@ -288,16 +291,20 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["chat_template"], ]):
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "chat_template", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
@@ -306,14 +313,15 @@
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ModelConfigChatRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
             provider=provider,
             max_tokens=max_tokens,
@@ -322,12 +330,13 @@
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             endpoint=endpoint,
             chat_template=chat_template,
             _configuration=_configuration,
+            **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.0/humanloop/model/model_config_chat_request.pyi` & `humanloop-0.4.0a4/humanloop/model/model_config_chat_request.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -214,15 +214,14 @@
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "endpoint": endpoint,
                 "chat_template": chat_template,
             }
-        additional_properties = schemas.NotAnyTypeSchema
     
     model: MetaOapg.properties.model
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
@@ -251,18 +250,22 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["chat_template"], ]):
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "chat_template", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
@@ -288,16 +291,20 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["chat_template"], ]):
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "chat_template", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
@@ -306,14 +313,15 @@
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ModelConfigChatRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
             provider=provider,
             max_tokens=max_tokens,
@@ -322,12 +330,13 @@
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             endpoint=endpoint,
             chat_template=chat_template,
             _configuration=_configuration,
+            **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.0/humanloop/model/model_config_completion_request.py` & `humanloop-0.4.0a4/humanloop/model/model_config_completion_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,15 +190,14 @@
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "endpoint": endpoint,
             }
-        additional_properties = schemas.NotAnyTypeSchema
     
     model: MetaOapg.properties.model
     prompt_template: MetaOapg.properties.prompt_template
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
@@ -228,18 +227,22 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], ]):
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "prompt_template", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
@@ -265,16 +268,20 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], ]):
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "prompt_template", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -283,14 +290,15 @@
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ModelConfigCompletionRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
             prompt_template=prompt_template,
             provider=provider,
@@ -299,11 +307,12 @@
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             endpoint=endpoint,
             _configuration=_configuration,
+            **kwargs,
         )
 
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.0/humanloop/model/model_config_completion_request.pyi` & `humanloop-0.4.0a4/humanloop/model/model_config_completion_request.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -190,15 +190,14 @@
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "endpoint": endpoint,
             }
-        additional_properties = schemas.NotAnyTypeSchema
     
     model: MetaOapg.properties.model
     prompt_template: MetaOapg.properties.prompt_template
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
@@ -228,18 +227,22 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], ]):
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "prompt_template", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
+    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
@@ -265,16 +268,20 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], ]):
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "prompt_template", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -283,14 +290,15 @@
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ModelConfigCompletionRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
             prompt_template=prompt_template,
             provider=provider,
@@ -299,11 +307,12 @@
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             endpoint=endpoint,
             _configuration=_configuration,
+            **kwargs,
         )
 
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.0/humanloop/model/model_endpoints.py` & `humanloop-0.4.0a4/humanloop/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/model_endpoints.pyi` & `humanloop-0.4.0a4/humanloop/model/model_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/model_providers.py` & `humanloop-0.4.0a4/humanloop/model/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/model_providers.pyi` & `humanloop-0.4.0a4/humanloop/model/model_providers.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/paginated_data_log_response.py` & `humanloop-0.4.0a4/humanloop/model/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/paginated_data_log_response.pyi` & `humanloop-0.4.0a4/humanloop/model/paginated_data_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/paginated_data_project_response.py` & `humanloop-0.4.0a4/humanloop/model/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/paginated_data_project_response.pyi` & `humanloop-0.4.0a4/humanloop/model/paginated_data_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/positive_label.py` & `humanloop-0.4.0a4/humanloop/model/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/positive_label.pyi` & `humanloop-0.4.0a4/humanloop/model/positive_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_model_config_request.py` & `humanloop-0.4.0a4/humanloop/model/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_model_config_request.pyi` & `humanloop-0.4.0a4/humanloop/model/project_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_response.py` & `humanloop-0.4.0a4/humanloop/model/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_response.pyi` & `humanloop-0.4.0a4/humanloop/model/project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_sort_by.py` & `humanloop-0.4.0a4/humanloop/model/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_sort_by.pyi` & `humanloop-0.4.0a4/humanloop/model/project_sort_by.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_user_response.py` & `humanloop-0.4.0a4/humanloop/model/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/project_user_response.pyi` & `humanloop-0.4.0a4/humanloop/model/project_user_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/projects_get_model_configs_response.py` & `humanloop-0.4.0a4/humanloop/model/projects_get_model_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/projects_get_model_configs_response.pyi` & `humanloop-0.4.0a4/humanloop/model/projects_get_model_configs_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/projects_update_feedback_types_request.py` & `humanloop-0.4.0a4/humanloop/model/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/projects_update_feedback_types_request.pyi` & `humanloop-0.4.0a4/humanloop/model/projects_update_feedback_types_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/provider_api_keys.py` & `humanloop-0.4.0a4/humanloop/model/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/provider_api_keys.pyi` & `humanloop-0.4.0a4/humanloop/model/provider_api_keys.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/session_app_response.py` & `humanloop-0.4.0a4/humanloop/model/session_app_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/session_app_response.pyi` & `humanloop-0.4.0a4/humanloop/model/session_app_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/session_response.py` & `humanloop-0.4.0a4/humanloop/model/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/session_response.pyi` & `humanloop-0.4.0a4/humanloop/model/session_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/sort_order.py` & `humanloop-0.4.0a4/humanloop/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/sort_order.pyi` & `humanloop-0.4.0a4/humanloop/model/sort_order.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi` & `humanloop-0.4.0a4/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/tool_result_response.py` & `humanloop-0.4.0a4/humanloop/model/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/tool_result_response.pyi` & `humanloop-0.4.0a4/humanloop/model/tool_result_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/update_experiment_request.py` & `humanloop-0.4.0a4/humanloop/model/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/update_experiment_request.pyi` & `humanloop-0.4.0a4/humanloop/model/update_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/update_project_request.py` & `humanloop-0.4.0a4/humanloop/model/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/update_project_request.pyi` & `humanloop-0.4.0a4/humanloop/model/update_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/usage.py` & `humanloop-0.4.0a4/humanloop/model/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/usage.pyi` & `humanloop-0.4.0a4/humanloop/model/usage.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/validation_error.py` & `humanloop-0.4.0a4/humanloop/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/model/validation_error.pyi` & `humanloop-0.4.0a4/humanloop/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/models/__init__.py` & `humanloop-0.4.0a4/humanloop/models/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/__init__.py` & `humanloop-0.4.0a4/humanloop/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps/get.py` & `humanloop-0.4.0a4/humanloop/paths/apps/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/apps/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps_id/get.py` & `humanloop-0.4.0a4/humanloop/paths/apps_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps_id/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/apps_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps_id_sessions/get.py` & `humanloop-0.4.0a4/humanloop/paths/apps_id_sessions/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/apps_id_sessions/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/apps_id_sessions/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat/post.py` & `humanloop-0.4.0a4/humanloop/paths/chat/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/chat/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_deployed/post.py` & `humanloop-0.4.0a4/humanloop/paths/chat_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_deployed/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/chat_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_experiment/post.py` & `humanloop-0.4.0a4/humanloop/paths/chat_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_experiment/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/chat_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_model_config/post.py` & `humanloop-0.4.0a4/humanloop/paths/chat_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/chat_model_config/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/chat_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion/post.py` & `humanloop-0.4.0a4/humanloop/paths/completion/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/completion/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_deployed/post.py` & `humanloop-0.4.0a4/humanloop/paths/completion_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_deployed/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/completion_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_experiment/post.py` & `humanloop-0.4.0a4/humanloop/paths/completion_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_experiment/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/completion_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_model_config/post.py` & `humanloop-0.4.0a4/humanloop/paths/completion_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/completion_model_config/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/completion_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id/delete.py` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id/delete.pyi` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id/patch.py` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id/patch.pyi` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id_model_config/get.py` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/experiments_experiment_id_model_config/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/experiments_experiment_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/feedback/post.py` & `humanloop-0.4.0a4/humanloop/paths/feedback/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/feedback/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/feedback/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/logs/post.py` & `humanloop-0.4.0a4/humanloop/paths/logs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/logs/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/logs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/model_configs/post.py` & `humanloop-0.4.0a4/humanloop/paths/model_configs/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/model_configs/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/model_configs/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/model_configs_id/get.py` & `humanloop-0.4.0a4/humanloop/paths/model_configs_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/model_configs_id/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/model_configs_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects/get.py` & `humanloop-0.4.0a4/humanloop/paths/projects/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects/post.py` & `humanloop-0.4.0a4/humanloop/paths/projects/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id/get.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id/patch.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id/patch.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_active_experiment/delete.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_active_experiment/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_active_experiment/delete.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_active_experiment/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_active_model_config/delete.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_active_model_config/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_active_model_config/delete.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_active_model_config/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_export/post.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_export/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_export/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_export/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_feedback_types/patch.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_feedback_types/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_feedback_types/patch.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_feedback_types/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_model_config/get.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_model_config/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_model_configs/get.py` & `humanloop-0.4.0a4/humanloop/paths/projects_id_model_configs/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_id_model_configs/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_id_model_configs/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/get.py` & `humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/post.py` & `humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/projects_project_id_experiments/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/projects_project_id_experiments/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions/post.py` & `humanloop-0.4.0a4/humanloop/paths/sessions/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions/post.pyi` & `humanloop-0.4.0a4/humanloop/paths/sessions/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions_id/get.py` & `humanloop-0.4.0a4/humanloop/paths/sessions_id/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions_id/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/sessions_id/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions_id_events/get.py` & `humanloop-0.4.0a4/humanloop/paths/sessions_id_events/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/paths/sessions_id_events/get.pyi` & `humanloop-0.4.0a4/humanloop/paths/sessions_id_events/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/request_after_hook.py` & `humanloop-0.4.0a4/humanloop/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/request_before_hook.py` & `humanloop-0.4.0a4/humanloop/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/rest.py` & `humanloop-0.4.0a4/humanloop/rest.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/schemas.py` & `humanloop-0.4.0a4/humanloop/schemas.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/base_metric_response.py` & `humanloop-0.4.0a4/humanloop/type/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/categorical_feedback_label.py` & `humanloop-0.4.0a4/humanloop/type/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_data_response.py` & `humanloop-0.4.0a4/humanloop/type/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_deployed_request.py` & `humanloop-0.4.0a4/humanloop/type/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_experiment_request.py` & `humanloop-0.4.0a4/humanloop/type/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_message.py` & `humanloop-0.4.0a4/humanloop/type/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_model_config_request.py` & `humanloop-0.4.0a4/humanloop/type/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_request.py` & `humanloop-0.4.0a4/humanloop/type/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_response.py` & `humanloop-0.4.0a4/humanloop/type/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/chat_role.py` & `humanloop-0.4.0a4/humanloop/type/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/completion_deployed_request.py` & `humanloop-0.4.0a4/humanloop/type/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/completion_experiment_request.py` & `humanloop-0.4.0a4/humanloop/type/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/completion_model_config_request.py` & `humanloop-0.4.0a4/humanloop/type/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/completion_request.py` & `humanloop-0.4.0a4/humanloop/type/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/completion_response.py` & `humanloop-0.4.0a4/humanloop/type/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/create_experiment_request.py` & `humanloop-0.4.0a4/humanloop/type/create_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/create_log_response.py` & `humanloop-0.4.0a4/humanloop/type/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/create_project_request.py` & `humanloop-0.4.0a4/humanloop/type/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/create_session_request.py` & `humanloop-0.4.0a4/humanloop/type/create_session_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/data_response.py` & `humanloop-0.4.0a4/humanloop/type/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/experiment_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/experiment_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/experiment_response.py` & `humanloop-0.4.0a4/humanloop/type/experiment_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/experiment_status.py` & `humanloop-0.4.0a4/humanloop/type/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/experiments_list_response.py` & `humanloop-0.4.0a4/humanloop/type/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback.py` & `humanloop-0.4.0a4/humanloop/type/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_class.py` & `humanloop-0.4.0a4/humanloop/type/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_label_request.py` & `humanloop-0.4.0a4/humanloop/type/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_request.py` & `humanloop-0.4.0a4/humanloop/type/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_response.py` & `humanloop-0.4.0a4/humanloop/type/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_submit_request.py` & `humanloop-0.4.0a4/humanloop/type/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_submit_response.py` & `humanloop-0.4.0a4/humanloop/type/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_type.py` & `humanloop-0.4.0a4/humanloop/type/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_type_model.py` & `humanloop-0.4.0a4/humanloop/type/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_type_request.py` & `humanloop-0.4.0a4/humanloop/type/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/feedback_types.py` & `humanloop-0.4.0a4/humanloop/type/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/get_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/get_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/http_validation_error.py` & `humanloop-0.4.0a4/humanloop/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/label_sentiment.py` & `humanloop-0.4.0a4/humanloop/type/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/log_datapoint_request.py` & `humanloop-0.4.0a4/humanloop/type/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/log_request.py` & `humanloop-0.4.0a4/humanloop/type/log_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/log_response.py` & `humanloop-0.4.0a4/humanloop/type/log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/logs_log_response.py` & `humanloop-0.4.0a4/humanloop/type/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/model_config_chat_request.py` & `humanloop-0.4.0a4/humanloop/type/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/model_config_completion_request.py` & `humanloop-0.4.0a4/humanloop/type/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/model_endpoints.py` & `humanloop-0.4.0a4/humanloop/type/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/model_providers.py` & `humanloop-0.4.0a4/humanloop/type/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/paginated_data_log_response.py` & `humanloop-0.4.0a4/humanloop/type/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/paginated_data_project_response.py` & `humanloop-0.4.0a4/humanloop/type/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/positive_label.py` & `humanloop-0.4.0a4/humanloop/type/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/project_model_config_request.py` & `humanloop-0.4.0a4/humanloop/type/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/project_response.py` & `humanloop-0.4.0a4/humanloop/type/project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/project_sort_by.py` & `humanloop-0.4.0a4/humanloop/type/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/project_user_response.py` & `humanloop-0.4.0a4/humanloop/type/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/projects_get_model_configs_response.py` & `humanloop-0.4.0a4/humanloop/type/projects_get_model_configs_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/projects_update_feedback_types_request.py` & `humanloop-0.4.0a4/humanloop/type/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/provider_api_keys.py` & `humanloop-0.4.0a4/humanloop/type/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/session_app_response.py` & `humanloop-0.4.0a4/humanloop/type/session_app_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/session_response.py` & `humanloop-0.4.0a4/humanloop/type/session_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/sort_order.py` & `humanloop-0.4.0a4/humanloop/type/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_response.py` & `humanloop-0.4.0a4/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/tool_result_response.py` & `humanloop-0.4.0a4/humanloop/type/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/update_experiment_request.py` & `humanloop-0.4.0a4/humanloop/type/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/update_project_request.py` & `humanloop-0.4.0a4/humanloop/type/update_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/usage.py` & `humanloop-0.4.0a4/humanloop/type/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type/validation_error.py` & `humanloop-0.4.0a4/humanloop/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/type_util.py` & `humanloop-0.4.0a4/humanloop/type_util.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/humanloop/validation_metadata.py` & `humanloop-0.4.0a4/humanloop/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.0/PKG-INFO` & `humanloop-0.4.0a4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: humanloop
-Version: 0.4.0
-Summary: Client for Humanloop API
+Version: 0.4.0a4
+Summary: The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  &#x60;&#x60;&#x60;bash pip install humanloop &#x60;&#x60;&#x60;  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -18,25 +18,25 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# humanloop@0.4.0
+# humanloop@0.4.0a4
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.0
+pip install humanloop==0.4.0a4
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
@@ -78,15 +78,15 @@
     pprint(chat_response.body["project_id"])
     pprint(chat_response.body["data"][0])
     pprint(chat_response.body["provider_responses"])
     pprint(chat_response.headers)
     pprint(chat_response.status)
     pprint(chat_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .chat: %s\n" % e)
+    print("Exception when calling .response: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -110,15 +110,15 @@
     pprint(complete_response.body["project_id"])
     pprint(complete_response.body["data"][0])
     pprint(complete_response.body["provider_responses"])
     pprint(complete_response.headers)
     pprint(complete_response.status)
     pprint(complete_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .complete: %s\n" % e)
+    print("Exception when calling .create: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -132,15 +132,15 @@
         user="user@example.com",
     )
     pprint(feedback_response.body)
     pprint(feedback_response.headers)
     pprint(feedback_response.status)
     pprint(feedback_response.round_trip_time)
 except ApiException as e:
-    print("Exception when calling .feedback: %s\n" % e)
+    print("Exception when calling .submit: %s\n" % e)
     pprint(e.body)
     if e.status == 422:
         pprint(e.body["detail"])
     pprint(e.headers)
     pprint(e.status)
     pprint(e.reason)
     pprint(e.round_trip_time)
@@ -177,47 +177,39 @@
 ```
 
 ## Async
 
 `async` support is available by prepending `a` to any method.
 
 ```python
-import asyncio
 from pprint import pprint
 from humanloop import Humanloop, ApiException
 
 humanloop = Humanloop(
+    # Defining the host is optional and defaults to https://api.humanloop.com/v4
+    # See configuration.py for a list of all supported configuration parameters.
+    host="https://api.humanloop.com/v4",
+    # Configure API key authorization: APIKeyHeader
     api_key="YOUR_API_KEY",
+    # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+    # api_key_prefix = {'APIKeyHeader': 'Bearer'},
 )
 
 
 async def main():
     try:
-        complete_response = await humanloop.acomplete(
-            project="sdk-example",
-            inputs={
-                "text": "Llamas that are well-socialized and trained to halter and lead after weaning and are very friendly and pleasant to be around. They are extremely curious and most will approach people easily. However, llamas that are bottle-fed or over-socialized and over-handled as youth will become extremely difficult to handle when mature, when they will begin to treat humans as they treat each other, which is characterized by bouts of spitting, kicking and neck wrestling.[33]",
-            },
-            model_config={
-                "model": "gpt-3.5-turbo",
-                "max_tokens": -1,
-                "temperature": 0.7,
-                "prompt_template": "Summarize this for a second-grade student:\n\nText:\n{{text}}\n\nSummary:\n",
-            },
-            stream=False,
+        # Get App
+        get_response = await humanloop.apps.aget(
+            id="id_example",  # required
         )
-        pprint(complete_response.body)
-        pprint(complete_response.body["project_id"])
-        pprint(complete_response.body["data"][0])
-        pprint(complete_response.body["provider_responses"])
-        pprint(complete_response.headers)
-        pprint(complete_response.status)
-        pprint(complete_response.round_trip_time)
+        pprint(get_response.headers)
+        pprint(get_response.status)
+        pprint(get_response.round_trip_time)
     except ApiException as e:
-        print("Exception when calling .complete: %s\n" % e)
+        print("Exception when calling AppsApi.get: %s\n" % e)
         pprint(e.body)
         if e.status == 422:
             pprint(e.body["detail"])
         pprint(e.headers)
         pprint(e.status)
         pprint(e.reason)
         pprint(e.round_trip_time)
```

