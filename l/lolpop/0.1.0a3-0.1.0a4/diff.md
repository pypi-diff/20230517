# Comparing `tmp/lolpop-0.1.0a3.tar.gz` & `tmp/lolpop-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a3.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a4.tar", max compression
```

## Comparing `lolpop-0.1.0a3.tar` & `lolpop-0.1.0a4.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11357 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/LICENSE
--rw-r--r--   0        0        0      220 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/__init__.py
--rw-r--r--   0        0        0     2456 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/cli.py
--rw-r--r--   0        0        0    12669 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/create.py
--rw-r--r--   0        0        0     3292 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/datagen.py
--rw-r--r--   0        0        0      260 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/package.py
--rw-r--r--   0        0        0     1756 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/run.py
--rw-r--r--   0        0        0     1864 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/seed.py
--rw-r--r--   0        0        0       89 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/test.py
--rw-r--r--   0        0        0     1311 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3652 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2160 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     6265 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/bigquery_data_connector.py
--rw-r--r--   0        0        0     5431 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/databricks_sql_data_connector.py
--rw-r--r--   0        0        0     4122 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/duckdb_data_connector.py
--rw-r--r--   0        0        0     4275 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/gcs_data_connector.py
--rw-r--r--   0        0        0     1299 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     5453 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/postgres_data_connector.py
--rw-r--r--   0        0        0      637 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/redshift_data_connector.py
--rw-r--r--   0        0        0     3352 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/s3_data_connector.py
--rw-r--r--   0        0        0     6484 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1912 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     8542 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0      712 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/bigquery_data_transformer.py
--rw-r--r--   0        0        0      870 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/databricks_sql_data_transformer.py
--rw-r--r--   0        0        0     4525 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0      613 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/duckdb_data_transformer.py
--rw-r--r--   0        0        0     2086 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0      838 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/postrgres_data_transformer.py
--rw-r--r--   0        0        0      962 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/redshift_data_transformer.py
--rw-r--r--   0        0        0      855 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/__init__.py
--rw-r--r--   0        0        0      228 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/base_genai_chatbot.py
--rw-r--r--   0        0        0      940 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/openai_chatbot.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9180 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0     1699 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0     2017 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12376 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      229 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0     5574 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2848 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3408 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0     7234 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2407 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     3881 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0     2346 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/extension/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4626 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7182 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4068 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5459 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7474 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4495 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      789 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1285 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     6578 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7686 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6130 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0      175 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       66 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0       32 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0     1408 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0     1363 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0      310 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      151 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    15386 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     2198 2023-05-16 22:51:47.223311 lolpop-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 lolpop-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0      220 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2552 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    12841 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3464 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      432 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1928 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/run.py
+-rw-r--r--   0        0        0     2037 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/seed.py
+-rw-r--r--   0        0        0      451 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1311 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     3652 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2160 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4122 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1912 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     8542 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2086 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9180 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     1699 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2017 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12376 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      229 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0     5574 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2848 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3408 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0     7234 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2407 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     3881 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0     2346 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     4626 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7182 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4068 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5459 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7474 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4495 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      789 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1285 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     6578 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7686 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6130 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0      175 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0     1408 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0     1363 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    15386 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2261 2023-05-17 13:45:38.588891 lolpop-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 lolpop-0.1.0a4/PKG-INFO
```

### Comparing `lolpop-0.1.0a3/LICENSE` & `lolpop-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/cli/cli.py` & `lolpop-0.1.0a4/lolpop/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import typer 
 import click 
 import os 
 
-import create, run, package, test, datagen, seed 
+from lolpop.cli import create, run, package, test, datagen, seed 
 from importlib.metadata import version
 from typing import Optional
 from pathlib import Path 
 from cookiecutter.main import cookiecutter
 from lolpop import __template_path__ as lolpop_template_path
+from typer.core import TyperGroup 
 
 try:
     __version__ = version("lolpop")
 except:
     __version__ = "local-dev"
 
-#class NaturalOrderGroup(click.Group):
-#    def list_commands(self, ctx):
-#        return self.commands.keys()
+class NaturalOrderGroup(TyperGroup):
+    def list_commands(self, ctx):
+        return self.commands.keys()
 
-app = typer.Typer(#cls=NaturalOrderGroup,
+app = typer.Typer(cls=NaturalOrderGroup,
                   help="lolpop: A software engineering framework for machine learning workflows.",
                   no_args_is_help=True)
 
 app.add_typer(run.app, name="run")
 app.add_typer(create.app, name="create")
-app.add_typer(test.app, name="test")
-app.add_typer(package.app, name="package")
 app.add_typer(datagen.app, name="datagen")
 app.add_typer(seed.app, name="seed")
+app.add_typer(test.app, name="test")
+app.add_typer(package.app, name="package")
+
 
 
 def version_callback(value: bool):
     if value:
         try:
-            typer.secho(f"lolpop version: %s" %__version__, fg="blue")
+            typer.secho("lolpop version: %s" % __version__, fg="blue")
+            raise typer.Exit()
         except Exception as e:
            raise typer.Exit()
 
 
 @app.callback(context_settings=dict(help_option_names=["-h", "--help"]))
 def main(
     version: Optional[bool] = typer.Option(
         None,
         "--version",
         callback=version_callback,
         is_eager=True,
         help="Print lolpop version",
     ),
 ):
-    return
+    return True
 
 @app.command("init", help="Initialize a lolpop project.")
 def initialize(
     project_name: str = typer.Argument(..., help="Name of the project to create."), 
     project_path: Path = typer.Option(Path(os.getcwd()), help="Path to create project."), 
     template_path: str = typer.Option(
         lolpop_template_path + "/project_template", help="Path to the project template."),
@@ -62,15 +65,15 @@
                     extra_context={"project_name": project_name},
                     output_dir=project_path, no_input=True)
         typer.secho("Successfully created lolpop project %s at location %s/%s" %
                     (project_name, project_path, project_name), fg="green")
     except Exception as e: 
         typer.secho("Failed to create project %s: %s" %(project_name, str(e)), fg="red") 
 
-@app.command("help", add_help_option=False, options_metavar="")
+@app.command("help", add_help_option=False, options_metavar="", hidden=True)
 def help(ctx: typer.Context):
     """Show CLI usage help."""
     ctx.info_name = None
     typer.echo(ctx.parent.command.get_help(ctx))
 
 if __name__ == "__main__":
     app()
```

### Comparing `lolpop-0.1.0a3/lolpop/cli/create.py` & `lolpop-0.1.0a4/lolpop/cli/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 import inspect 
 import os
 import json 
 
 from typing import List
 from cookiecutter.main import cookiecutter
 from pathlib import Path
+from typer.core import TyperGroup
 
 from lolpop import __template_path__ as lolpop_template_path
 from lolpop.utils import common_utils as utils
 
-app = typer.Typer(help="Create new runners, piplines, and components.")
+
+class NaturalOrderGroup(TyperGroup):
+    def list_commands(self, ctx):
+        return self.commands.keys()
+    
+app = typer.Typer(cls = NaturalOrderGroup, help="Create new runners, piplines, and components.")
 
 LOLPOP_DIR = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
 #PARENT_DIR = os.path.dirname(LOLPOP_DIR)
 
 
 @app.callback(invoke_without_command=True)
 def default(ctx: typer.Context):
```

### Comparing `lolpop-0.1.0a3/lolpop/cli/datagen.py` & `lolpop-0.1.0a4/lolpop/cli/datagen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import typer 
 from lolpop.utils import common_utils as utils
 from pathlib import Path
 import os 
+from typer.core import TyperGroup
 
-app = typer.Typer(help="Generate synthetic data from existing data.")
+
+class NaturalOrderGroup(TyperGroup):
+    def list_commands(self, ctx):
+        return self.commands.keys()
+    
+app = typer.Typer(cls = NaturalOrderGroup, help="Generate synthetic data from existing data.")
 
 
 @app.callback(invoke_without_command=True)
 def default(ctx: typer.Context):
     if ctx.invoked_subcommand is not None:
         return
     else:
```

### Comparing `lolpop-0.1.0a3/lolpop/cli/run.py` & `lolpop-0.1.0a4/lolpop/cli/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import typer 
 from pathlib import Path 
 from lolpop.utils import common_utils as utils
 from typing import List
 import json
+from typer.core import TyperGroup
 
-app = typer.Typer(help="Run workflows with lolpop.")
+
+class NaturalOrderGroup(TyperGroup):
+    def list_commands(self, ctx):
+        return self.commands.keys()
+    
+app = typer.Typer(cls = NaturalOrderGroup, help="Run workflows with lolpop.")
 
 
 @app.callback(invoke_without_command=True)
 def default(ctx: typer.Context):
     if ctx.invoked_subcommand is not None:
         return
     else:
```

### Comparing `lolpop-0.1.0a3/lolpop/component/__init__.py` & `lolpop-0.1.0a4/lolpop/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/base_component.py` & `lolpop-0.1.0a4/lolpop/component/base_component.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a4/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a4/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/bigquery_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/bigquery_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/databricks_sql_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/databricks_sql_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/duckdb_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/duckdb_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/gcs_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/gcs_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/postgres_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/postgres_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/redshift_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/redshift_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/s3_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/s3_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a4/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a4/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a4/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a4/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_profiler/ydata_profiling_data_profiler.py` & `lolpop-0.1.0a4/lolpop/component/data_profiler/ydata_profiling_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a4/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a4/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/bigquery_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/bigquery_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/databricks_sql_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/databricks_sql_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/dbt_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/duckdb_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/duckdb_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/postrgres_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/postrgres_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/redshift_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/redshift_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a4/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/genai_chatbot/openai_chatbot.py` & `lolpop-0.1.0a4/lolpop/component/genai_chatbot/openai_chatbot.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/logger/file_logger.py` & `lolpop-0.1.0a4/lolpop/component/logger/file_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/logger/stdout_logger.py` & `lolpop-0.1.0a4/lolpop/component/logger/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a4/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a4/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a4/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a4/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a4/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a4/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_checker/base_model_checker.py` & `lolpop-0.1.0a4/lolpop/component/model_checker/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a4/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a4/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a4/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a4/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a4/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a4/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_trainer/base_model_trainer.py` & `lolpop-0.1.0a4/lolpop/component/model_trainer/base_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a4/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a4/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a4/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a4/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a4/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a4/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a4/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/extension/__init__.py` & `lolpop-0.1.0a4/lolpop/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a4/lolpop/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a4/lolpop/pipeline/base_pipeline.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a4/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a4/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a4/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a4/lolpop/pipeline/predict/offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/process/metaflow_offline_process.py` & `lolpop-0.1.0a4/lolpop/pipeline/process/metaflow_offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a4/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a4/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a4/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a4/lolpop/pipeline/train/offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py` & `lolpop-0.1.0a4/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/runner/__init__.py` & `lolpop-0.1.0a4/lolpop/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/runner/base_runner.py` & `lolpop-0.1.0a4/lolpop/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a4/lolpop/runner/classification_runner/classification_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a4/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py` & `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py` & `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py` & `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/utils/common_utils.py` & `lolpop-0.1.0a4/lolpop/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a4/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a4/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a4/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a3/pyproject.toml` & `lolpop-0.1.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.3"
+version = "v0.1.0-alpha.4"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
@@ -57,19 +57,20 @@
 metaflow="^2.8.3"
 duckdb={version="^0.7.1", optional=true}
 databricks-sql-connector={version="^2.5.2", optional=true}
 boto3={version="^1.26.89", optional=true}
 db-dtypes={version="^1.1.1", optional=true}
 psychopg2={version="^2.9.6", optional=true}
 openai="^0.27.6"
+cookiecutter={version="^2.1.1", optional=true}
 
 [tool.poetry.extras]
 duckdb = ["duckdb"]
 databricks = ["databricks-sql-connector"]
-cli = ["sdv", "openai"]
+cli = ["sdv", "openai", "cookiecutter"]
 aws = ["boto3"]
 google = ["google-cloud-bigquery", "google-cloud-storage", "db-dtypes"]
 redshift = ["psychopg2"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 faker = "^14.0"
```

### Comparing `lolpop-0.1.0a3/PKG-INFO` & `lolpop-0.1.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolpop
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A software engineering framework for machine learning workflows
 Home-page: https://github.com/jordanvolz/lolpop
 License: Apache-2.0
 Keywords: machine learning,data science,mlops
 Author: jordanvolz
 Author-email: jordan.volz@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -19,14 +19,15 @@
 Provides-Extra: google
 Provides-Extra: redshift
 Requires-Dist: SQLAlchemy (>=1.4.37,<2.0.0)
 Requires-Dist: aif360 (>=0.5.0,<0.6.0)
 Requires-Dist: alibi[shap] (>=0.8.0,<0.9.0)
 Requires-Dist: boto3 (>=1.26.89,<2.0.0) ; extra == "aws"
 Requires-Dist: continual (>=2.0.0a51,<3.0.0)
+Requires-Dist: cookiecutter (>=2.1.1,<3.0.0) ; extra == "cli"
 Requires-Dist: databricks-sql-connector (>=2.5.2,<3.0.0) ; extra == "databricks"
 Requires-Dist: db-dtypes (>=1.1.1,<2.0.0) ; extra == "google"
 Requires-Dist: dbt-core (>=1.3,<2.0)
 Requires-Dist: dbt-snowflake (>=1.3,<2.0)
 Requires-Dist: deepchecks (>=0.13.0,<0.14.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0) ; extra == "duckdb"
 Requires-Dist: dvc (>=2.37.0,<3.0.0)
```

