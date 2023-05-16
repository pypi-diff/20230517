# Comparing `tmp/lolpop-0.1.0a2.tar.gz` & `tmp/lolpop-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a2.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a3.tar", max compression
```

## Comparing `lolpop-0.1.0a2.tar` & `lolpop-0.1.0a3.tar`

### file list

```diff
@@ -1,142 +1,157 @@
--rw-r--r--   0        0        0    11357 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/__init__.py
--rw-r--r--   0        0        0     2479 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/cli.py
--rw-r--r--   0        0        0     3917 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/create.py
--rw-r--r--   0        0        0     3409 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/datagen.py
--rw-r--r--   0        0        0      260 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/package.py
--rw-r--r--   0        0        0     1756 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/run.py
--rw-r--r--   0        0        0     1916 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/seed.py
--rw-r--r--   0        0        0       89 2023-05-06 03:26:20.545473 lolpop-0.1.0a2/cli/test.py
--rw-r--r--   0        0        0      265 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3535 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2160 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     1299 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     6491 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1912 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     8542 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0     3486 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0     2086 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0     1067 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9180 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0      427 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0      854 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12376 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      229 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0     5574 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2848 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3408 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-05-06 03:26:20.549473 lolpop-0.1.0a2/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0     7234 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2407 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     3881 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/extension/.gitkeep
--rw-r--r--   0        0        0     1235 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4481 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7182 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4068 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5459 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7474 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4495 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      789 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1220 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     6433 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7686 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6130 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    15157 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     1644 2023-05-06 03:26:38.833603 lolpop-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      175 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       38 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     1363 2023-05-06 03:26:20.553473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0     1355 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0     1310 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0      151 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-05-06 03:26:20.557473 lolpop-0.1.0a2/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 lolpop-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0      220 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2456 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    12669 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3292 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      260 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1756 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/run.py
+-rw-r--r--   0        0        0     1864 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/seed.py
+-rw-r--r--   0        0        0       89 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1311 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     3652 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2160 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-05-16 22:51:29.827463 lolpop-0.1.0a3/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4122 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1912 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     8542 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2086 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9180 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     1699 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2017 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12376 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      229 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0     5574 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2848 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3408 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0     7234 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2407 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     3881 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0     2346 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     4626 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7182 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4068 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5459 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7474 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4495 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      789 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1285 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     6578 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.831462 lolpop-0.1.0a3/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7686 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6130 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0      175 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0     1408 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0     1363 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    15386 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-05-16 22:51:29.835462 lolpop-0.1.0a3/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2198 2023-05-16 22:51:47.223311 lolpop-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 lolpop-0.1.0a3/PKG-INFO
```

### Comparing `lolpop-0.1.0a2/LICENSE` & `lolpop-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/cli/cli.py` & `lolpop-0.1.0a3/lolpop/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     try:
         cookiecutter(template=template_path,
                     extra_context={"project_name": project_name},
                     output_dir=project_path, no_input=True)
         typer.secho("Successfully created lolpop project %s at location %s/%s" %
                     (project_name, project_path, project_name), fg="green")
     except Exception as e: 
-        typer.secho("Failed to create template for %s %s: %s" %(template_type, object_class, str(e)), fg="red") 
+        typer.secho("Failed to create project %s: %s" %(project_name, str(e)), fg="red") 
 
 @app.command("help", add_help_option=False, options_metavar="")
 def help(ctx: typer.Context):
     """Show CLI usage help."""
     ctx.info_name = None
     typer.echo(ctx.parent.command.get_help(ctx))
```

### Comparing `lolpop-0.1.0a2/cli/datagen.py` & `lolpop-0.1.0a3/lolpop/cli/datagen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import typer 
 from lolpop.utils import common_utils as utils
 from pathlib import Path
 import os 
 
 app = typer.Typer(help="Generate synthetic data from existing data.")
 
-LOLPOP_DIR = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-#PARENT_DIR = os.path.dirname(LOLPOP_DIR)
-
 
 @app.callback(invoke_without_command=True)
 def default(ctx: typer.Context):
     if ctx.invoked_subcommand is not None:
         return
     else:
         typer.echo(ctx.command.get_help(ctx))
```

### Comparing `lolpop-0.1.0a2/cli/run.py` & `lolpop-0.1.0a3/lolpop/cli/run.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/cli/seed.py` & `lolpop-0.1.0a3/lolpop/cli/seed.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,43 +3,40 @@
 from pathlib import Path
 import os 
 import json
 import pandas as pd 
 
 app = typer.Typer(help="Upload local data into your data platform. ")
 
-LOLPOP_DIR = os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
-#PARENT_DIR = os.path.dirname(LOLPOP_DIR)
-
 
 @app.callback(invoke_without_command=True)
 def default(ctx: typer.Context):
     if ctx.invoked_subcommand is not None:
         return
     else:
         typer.echo(ctx.command.get_help(ctx))
 
 @app.command("file", help="Seed a file.")
 def seed_file(
     source_file: Path = typer.Argument(
         ..., help="Path to the source file"),
     target: str = typer.Argument(
         ..., help="Where the data is going. Should be a table in DW or path in the object store, etc."),
-    data_loader_class: str = typer.Option(
-        "SnowflakeDataTransformer", "--data-loader-class", "-c", help="Data Loader class name."),
-    dataloader_kwargs: str = typer.Option("{}", "--kwargs", "-k", 
-                                          help="Keyword arguments (as a string) to pass into the data loader."),
+    data_connector_class: str = typer.Option(None, "--data-connector-class", "-c", help="Data Connector class name."),
+    data_connector_kwargs: str = typer.Option("{}", "--kwargs", "-k", 
+                                          help="Keyword arguments (as a string) to pass into the data connector."),
 ):
-    typer.secho("Loading data loader class %s" % data_loader_class, fg="blue")
-    data_loader_cl = utils.load_class(data_loader_class, "component")
+    typer.secho("Loading data connector class %s" % data_connector_class, fg="blue")
+    data_connector_cl = utils.load_class(data_connector_class, "component")
     logger_cl = utils.load_class("StdOutLogger", "component")
-    data_loader = data_loader_cl(conf={}, pipeline_conf={}, runner_conf={}, components={"logger": logger_cl()}, **json.loads(dataloader_kwargs))
-    data_loader.suppress_logger = True
-    data_loader.suppress_notifier = True
-    typer.secho("Successfully loaded data loader class %s" %
-                data_loader_cl, fg="green")
+    data_connector = data_connector_cl(conf={}, pipeline_conf={}, runner_conf={}, components={
+                                       "logger": logger_cl()}, **json.loads(data_connector_kwargs))
+    data_connector.suppress_logger = True
+    data_connector.suppress_notifier = True
+    typer.secho("Successfully loaded data connector class %s" %
+                data_connector_cl, fg="green")
 
-    typer.secho("Begin saving file %s with data loader" %
+    typer.secho("Begin saving file %s with data connector" %
                 source_file, fg="blue")
     data = utils.create_df_from_file(source_file)
-    data_loader.save_data(data, target)
+    data_connector.save_data(data, target)
     typer.secho("Successfully saved data to %s!" %target, fg="green")
```

### Comparing `lolpop-0.1.0a2/lolpop/component/__init__.py` & `lolpop-0.1.0a3/lolpop/component/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,20 @@
     from inspect import isclass
     from .base_component import BaseComponent
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
-    subdirs = ["%s/%s" %(path,x) for x in os.listdir(path) if ((x[0] != "_") and (".py" not in x) )]
+    subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
+               if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs: 
-        files = [ x for x in os.listdir(subdir) if ((".py" in x) and ("__" not in x))]
+        files = [x for x in os.listdir(subdir) if (
+            (".py" in x) and (x[0] != ".") and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace. 
         for file in files:
             module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
             classes = [x for x in dir(module) if isclass(getattr(module, x))]
             components = [x for x in classes if issubclass(getattr(module, x), BaseComponent)]
             globals().update({name: getattr(module,name) for name in components})
```

### Comparing `lolpop-0.1.0a2/lolpop/component/base_component.py` & `lolpop-0.1.0a3/lolpop/component/base_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from lolpop.utils import common_utils as utils
 from omegaconf import OmegaConf
-
+from inspect import currentframe
 class BaseComponent: 
     __REQUIRED_CONF__ = {
         "config" : []
     }
     __DEFAULT_CONF__ = {
         "config" : {}
     }
@@ -54,17 +54,17 @@
             if len(missing.get("components",{})) > 0: 
                 for component in missing.get("components"): 
                     if components.get(component, None) is not None: 
                         total_missing = total_missing - 1
             if total_missing > 0:   
                 raise Exception ("Missing the following from %s component configuration: %s" %(type(self).__name__, missing))
 
-    def log(self, msg, level="INFO"): 
+    def log(self, msg, level="INFO", **kwargs): 
         if not self.suppress_logger:
-            utils.log(self, msg, level)
+            self.logger.log(msg, level, process_name=self.name, line_num=currentframe().f_back.f_lineno, **kwargs)
 
 
     def notify(self, msg, level="ERROR"): 
         if not self.suppress_notifier: 
             self.notifier.notify(msg, level)
             self.log("Notification Sent: %s" %msg, level)
```

### Comparing `lolpop-0.1.0a2/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a3/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a3/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a3/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a3/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,18 @@
             column_type = 'DATETIME'
         elif col_type.kind == 'm':
             # timedelta columns in pandas are converted to timedelta64[ns] dtype, which corresponds to 'variant' in Snowflake
             column_type = 'VARIANT'
         elif col_type.kind == 'b':
             # boolean columns in pandas are converted to 'bool' dtype, which corresponds to 'boolean' in Snowflake
             column_type = 'BOOLEAN'
-        elif col_type.kind == 'i':
+        elif col_type.kind == 'i' or col_type.kind == 'u':
             # integer columns in pandas are converted to 'int64' dtype, which corresponds to 'integer' in Snowflake
             column_type = 'INTEGER'
-        elif col_type.kind == 'f':
+        elif col_type.kind == 'f' or col_type.kind == 'c':
             # float columns in pandas are converted to 'float64' dtype, which corresponds to 'float' in Snowflake
             column_type = 'FLOAT'
         else:
             # All other column types in pandas are assumed to be string columns, which correspond to 'varchar' in Snowflake
             column_type = 'VARCHAR'
         return column_type
 
@@ -139,14 +139,17 @@
     )
     cur = connection.cursor()
     cur.execute(sql)
     #coerce_float helps in converting numeric types into floats
     #otherwise they end up as strings and mess stuff up
     df = pd.DataFrame.from_records(
         iter(cur), columns=[x[0] for x in cur.description], coerce_float=True)
+    
+    connection.close()
+    
     return df
 
 #save to snowflake
 
 
 def save_to_snowflake(df, table_name, account, user, password, database, schema, warehouse):
     chunksize = 16384  # maximum allowed by snowflake
@@ -157,18 +160,15 @@
         database=database,
         schema=schema,
         warehouse=warehouse,
     ))
     connection = engine.connect()
     df = df.rename(columns=str.upper)
     with tqdm(total=len(df), desc="Upload to %s.%s.%s" % (database, schema, table_name)) as pbar:
-        for i, cdf in enumerate(chunker(df, chunksize)):
+        for i, cdf in enumerate(utils.chunker(df, chunksize)):
             cdf.to_sql(table_name.replace(" ", "_").upper(), con=engine,
                         index=False, if_exists="append", chunksize=chunksize,
                         method=snow_conn.pandas_tools.pd_writer)
             pbar.update(chunksize)
     connection.close()
     engine.dispose()
 
-
-def chunker(seq, size):
-    return (seq[pos:pos + size] for pos in range(0, len(seq), size))
```

### Comparing `lolpop-0.1.0a2/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a3/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a3/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a3/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_profiler/ydata_profiling_data_profiler.py` & `lolpop-0.1.0a3/lolpop/component/data_profiler/ydata_profiling_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a3/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a3/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a3/lolpop/component/data_connector/s3_data_connector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,99 @@
-from lolpop.component.data_transformer.base_data_transformer import BaseDataTransformer
+from lolpop.component.data_connector.base_data_connector import BaseDataConnector
 from lolpop.utils import common_utils as utils
-from omegaconf import OmegaConf 
 
-@utils.decorate_all_methods([utils.error_handler,utils.log_execution()])
-class dbtDataTransformer(BaseDataTransformer): 
-    
-    #use load_config to allow setting "DBT_TARGET", "DBT_PROFILE", "DBT_PROJECT_DIR", "DBT_PROFILES_DIR",  via env variables
-    __REQUIRED_CONF__ = {
-        "config" : ["data_connector"]
-    }
-
-    def __init__(self, components={}, *args, **kwargs): 
-        super().__init__(components=components, *args, **kwargs)
-
-        self.dbt_config = utils.load_config(["DBT_TARGET", "DBT_PROFILE", "DBT_PROJECT_DIR", "DBT_PROFILES_DIR"], self.config)
-
-        data_connector = self._get_config("data_connector")
-
-        #dbt doesn't actually retrieve data, so we have to use another data_transformer class to do that. 
-        # we'll read credentials for that in the dbt profile though, so you don't have to additionally include that
-        # in your dbt configuration
-        if data_connector is not None:
-            config = get_dw_config_from_profile(self.dbt_config)
-            obj = utils.register_component_class(self, config, "data_connector", data_connector, self.pipeline_conf, self.runner_conf,
-                                           parent_process=self.parent_process, problem_type=self.problem_type, dependent_components=components)
-
-    def get_data(self, source_table_name, *args, **kwargs): 
-        """Gets Data. Uses the specified data_connector to get the requested table.
-
-        Args:
-            source_table_name (String): Name of table to retrieve
-
-        Returns:
-            pd.DataFrame: The data
-        """
-        return self.data_connector.get_data(source_table_name, *args, **kwargs)
-
-    def transform(self, source_table_name, *args, **kwargs):
-        """Runs dbt workflow, specifid by dbt configuration provided. 
-
-        Args:
-            source_table_name (String): Name of the table to load and return. This should be a
-              table created in the dbt workflow.
-
-        Returns:
-            pd.DataFrame: the transformed data
-        """
-        command = ["dbt", "run", 
-                   "--target", self.dbt_config.get("DBT_TARGET"), 
-                   "--project-dir", self.dbt_config.get("DBT_PROJECT_DIR"), 
-                   "--profiles-dir", self.dbt_config.get("DBT_PROFILES_DIR"),
-                   "--profile", self.dbt_config.get("DBT_PROFILE")]
-
-        output, exit_code = utils.execute_cmd(command)
-
-        self.log("dbt output: \n%s" %output, "INFO")
-
-        if int(exit_code) == 0: #dbt ran successfully
-            data = self.data_connector.get_data(source_table_name)
-
-        return data 
-
-def get_dw_config_from_profile(dbt_config):
-    """Retrieves DW configurtion from dbt profile. 
-
-    Args:
-        dbt_config (dict): dictionary containing the dbt configuraiton
-
-    Returns:
-        dict: The DW configuration
-    """
-    conf = OmegaConf.load("%s/profiles.yml" %dbt_config.get("DBT_PROFILES_DIR")).get(dbt_config.get("DBT_PROFILE")).get("outputs").get(dbt_config.get("DBT_TARGET"))
-    config = {"%s_%s" %(conf.get("type").lower(), x.lower()):y 
-              for x,y in conf.items() 
-              if x.lower() in ["account", "database", "password", "schema", "user", "warehouse"]}
-    config = OmegaConf.create(
-        {"components": {}, "data_connector": {"config": config}})
-    
-    return config 
+import boto3
+from tqdm import tqdm
+
+import pandas as pd
+import io
+import os
+
+
+@utils.decorate_all_methods([utils.error_handler, utils.log_execution()])
+class S3DataConnector(BaseDataConnector):
+    __REQUIRED_CONF__ = {"config": ["GOOGLE_PROJECT"]}
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.aws_config = utils.load_config(
+            [
+                "AWS_S3_BUCKET", 
+                "AWS_ACCESS_KEY_ID", 
+                "AWS_SECRETE_KEY_ID", 
+                "AWS_SESSION_TOKEN",
+            ]
+        )
+
+    def get_data(self, path, *args, **kwargs):
+        df = self._load_data(path, self.aws_config)
+        return df
+
+    def save_data(self, data, path, *args, **kwargs):
+        self._save_data(data, path, self.aws_config)
+
+
+    @classmethod
+    def _load_data(self, path, config, **kwargs):
+        client = self._get_client(config)
+        bucket = config.get("AWs_S3_BUCKET")
+        extension = path.split(".")[-1]
+
+        response = client.get_object(Bucket=bucket, Key=path)
+        status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
+
+        if status == 200:
+            self.log(f"Successful S3 get_object response. Status - {status}")
+            source_data = response.get("Body").read()
+            if extension == "csv":
+                data = pd.read_csv(io.StringIO(source_data),
+                                encoding="utf-8", **kwargs)
+            elif extension == "parquet" or extension == "pq":
+                data = pd.read_parquet(io.BytesIO(source_data), **kwargs)
+            elif extension == "orc":
+                data = pd.read_orc(io.BytesIO(source_data), **kwargs)
+            else:
+                self.log("Unsupported file type provided: %s" % extension)
+            self.log("Successfully loaded data from %s into DataFrame." % path)
+
+        else:
+            self.log(f"Unsuccessful S3 get_object response. Status - {status}")
+
+        return data
+
+    def _save_data(self, data, path, config, *args, **kwargs):
+        # get client
+        client = self._get_client(config)
+        bucket = config.get("AWS_S3_BUCKET")
+        extension = path.split(".")[-1]
+
+        if extension == ".csv":
+            f = io.StringIO()
+            data.to_csv(f, index=False)
+        elif extension == ".pq" or extension == "parquet":
+            f = io.BytesIO()
+            data.to_parquet(f, index=False)
+        else:
+            raise Exception("Unsupported file type for path: %s" %(path))
+        f.seek(0)
+
+        response = client.put_object(
+            Bucket=bucket, Key=path, Body=f.getvalue()
+        )
+
+        status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
+
+        if status == 200:
+            self.log(f"Successful S3 put_object response. Status - {status}")
+        else:
+            self.log(f"Unsuccessful S3 put_object response. Status - {status}")
+
+
+    def _get_client(self, config):
+        client = boto3.client(
+            "s3",
+            aws_access_key_id=config.get("AWS_ACCESS_KEY_ID"),
+            aws_secret_access_key=config.get("AWS_SECRET_ACCESS_KEY"),
+            aws_session_token=config.get("AWS_SESSION_TOKEN"),
+        )
+ 
+        return client
```

### Comparing `lolpop-0.1.0a2/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a3/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a3/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 from lolpop.component.data_transformer.base_data_transformer import BaseDataTransformer
 from lolpop.utils import common_utils as utils
 from lolpop.component.data_connector.snowflake_data_connector import SnowflakeDataConnector
 
-import pandas as pd
-import snowflake.connector as snow_conn
-from snowflake.sqlalchemy import URL
-from snowflake.connector.pandas_tools import pd_writer
-from sqlalchemy import create_engine
-from tqdm import tqdm
-
 @utils.decorate_all_methods([utils.error_handler,utils.log_execution()])
 class SnowflakeDataTransformer(BaseDataTransformer): 
 
     def __init__(self, *args, **kwargs): 
         super().__init__(*args, **kwargs)
         self.snowflake_config = utils.load_config([
             "SNOWFLAKE_ACCOUNT",
```

### Comparing `lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a3/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a3/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a3/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a3/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a3/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a3/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a3/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_checker/base_model_checker.py` & `lolpop-0.1.0a3/lolpop/component/model_checker/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a3/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a3/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a3/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a3/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a3/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a3/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_trainer/base_model_trainer.py` & `lolpop-0.1.0a3/lolpop/component/model_trainer/base_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a3/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a3/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a3/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a3/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a3/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a3/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a3/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 
 def __map_pipelines__():
     from pathlib import Path
     import os
     from importlib import import_module
     from inspect import isclass
-    from .base_pipeline import BasePipeline
+    from lolpop.pipeline import BasePipeline
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
-    subdirs = ["%s/%s" %(path,x) for x in os.listdir(path) if ((x[0] != "_") and (".py" not in x) )]
+    subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
+               if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
-    for subdir in subdirs: 
-        files = [ x for x in os.listdir(subdir) if ((".py" in x) and ("__" not in x))]
-        #from each file, import all classes and register them in the global namespace. 
-        for file in files: 
-            module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
-            classes = [x for x in dir(module) if isclass(getattr(module,x))]
-            pipelines = [x for x in classes if issubclass(getattr(module, x), BasePipeline)]
-            globals().update({name: getattr(module,name) for name in pipelines})
+    for subdir in subdirs:
+        files = [x for x in os.listdir(subdir) if (
+            (".py" in x) and (x[0] != ".") and ("__" not in x))]
+        #from each file, import all classes and register them in the global namespace.
+        for file in files:
+            module = import_module("lolpop.extension.{{cookiecutter.project_name}}.%s.%s.%s" % (
+                subdir.split("/")[-2], subdir.split("/")[-1], file[:-3]))
+            classes = [x for x in dir(module) if isclass(getattr(module, x))]
+            pipelines = [x for x in classes if issubclass(
+                getattr(module, x), BasePipeline)]
+            globals().update({name: getattr(module, name)
+                              for name in pipelines})
 
     warnings.resetwarnings()
 
-__map_pipelines__()
+
+__map_pipelines__()
```

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a3/lolpop/pipeline/base_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from lolpop.utils import common_utils as utils
 from omegaconf import OmegaConf
-
+from inspect import currentframe
 class BasePipeline: 
 
     __REQUIRED_CONF__ = {
         "components": [], 
         "config": []
     }
     __DEFAULT_CONF__ = {
@@ -75,17 +75,18 @@
             if len(missing.get("components")) > 0: 
                 for component in missing.get("components"): 
                     if components.get(component, None) is not None: 
                         total_missing = total_missing - 1
             if total_missing > 0:   
                 raise Exception ("Missing the following from pipeline configuration: %s" %missing)
 
-    def log(self, msg, level="INFO"): 
+    def log(self, msg, level="INFO", **kwargs): 
         if not self.suppress_logger: 
-            utils.log(self, msg, level)
+            self.logger.log(msg, level, process_name=self.name,
+                            line_num=currentframe().f_back.f_lineno, **kwargs)
 
     def notify(self, msg, level="ERROR"): 
         if not self.suppress_notifier: 
             self.notifier.notify(msg, level)
             self.log("Notification Sent: %s" %msg, level)
 
     #helper function for lookup up config key in pipeline or runner conf
```

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a3/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a3/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a3/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a3/lolpop/pipeline/predict/offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/process/metaflow_offline_process.py` & `lolpop-0.1.0a3/lolpop/pipeline/process/metaflow_offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a3/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a3/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a3/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a3/lolpop/pipeline/train/offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py` & `lolpop-0.1.0a3/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/runner/__init__.py` & `lolpop-0.1.0a3/lolpop/runner/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,20 @@
     from inspect import isclass
     from .base_runner import BaseRunner
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
-    subdirs = ["%s/%s" %(path,x) for x in os.listdir(path) if ((x[0] != "_") and (".py" not in x) )]
+    subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
+               if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs: 
-        files = [ x for x in os.listdir(subdir) if ((".py" in x) and ("__" not in x))]
+        files = [x for x in os.listdir(subdir) if (
+            (".py" in x) and (x[0] != ".")  and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace. 
         for file in files: 
             module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
             classes = [x for x in dir(module) if isclass(getattr(module,x))]
             runners = [x for x in classes if issubclass(getattr(module, x), BaseRunner)]
             globals().update({name: getattr(module,name) for name in runners})
```

### Comparing `lolpop-0.1.0a2/lolpop/runner/base_runner.py` & `lolpop-0.1.0a3/lolpop/runner/base_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from omegaconf import OmegaConf
 from lolpop.utils import common_utils as utils
 import os 
 from pathlib import Path
-
+from inspect import currentframe
 class BaseRunner: 
 
     __REQUIRED_CONF__ = {
         "pipelines": [], 
         "components": ["metadata_tracker"], 
         "config": []
     }
@@ -102,17 +102,18 @@
         missing, total_missing = utils.validate_conf(conf, self.__REQUIRED_CONF__, conf.get("components"))
         if total_missing>0: 
             #logger is not necessarily set up yet
             #self.logger.log("Missing the following from runner configuration: %s" %missing)
             raise Exception("Missing the following from runner configuration: %s" %missing) 
         return conf
 
-    def log(self, msg, level="INFO"): 
+    def log(self, msg, level="INFO", **kwargs): 
         if not self.suppress_logger: 
-            utils.log(self, msg, level)
+            self.logger.log(msg, level, process_name=self.name,
+                            line_num=currentframe().f_back.f_lineno, **kwargs)
 
     def notify(self, msg, level="ERROR"): 
         if not self.suppress_notifier: 
             self.notifier.notify(msg, level)
             self.log("Notification Sent: %s" %msg, level)
 
     #helper function for lookup up config key
```

### Comparing `lolpop-0.1.0a2/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a3/lolpop/runner/classification_runner/classification_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a3/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/utils/common_utils.py` & `lolpop-0.1.0a3/lolpop/utils/common_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess 
 import os 
 import sys
-from importlib import import_module
+from importlib import import_module, util as import_util 
 from git import Repo
 from omegaconf import OmegaConf, dictconfig
 from datetime import datetime
 from functools import wraps 
 import pandas as pd 
 from pathlib import Path 
 import time
@@ -91,14 +91,22 @@
             cl = load_class(class_name, class_type=class_type, parent=plugin)
             break 
         except Exception as e: 
             #if multiple plugins are used, the one we are looking for will not be in most of them, so just ignore any errors
             continue 
     return cl
 
+#loads a module from a file
+def load_module_from_file(file_path): 
+    spec = import_util.spec_from_file_location(file_path.stem, file_path)
+    mod = import_util.module_from_spec(spec)
+    sys.modules[spec.name]=mod #need to do this to properly register module
+    spec.loader.exec_module(mod)
+    return mod 
+
 #register component class as an attribute of the provided object
 def register_component_class(self_obj, conf, component_type, default_class_name=None, pipeline_conf = {}, runner_conf = {}, parent_process = "runner", problem_type = None, dependent_components = {}, plugin_mods=[]): 
     obj = None
     component_class_name = conf.components.get(component_type, default_class_name)
     if component_class_name is not None:
         obj = None
         try: 
@@ -267,19 +275,14 @@
             if paths is not None: 
                 plugin_paths = plugin_paths + paths
     
     plugin_paths = [Path(path) for path in set(plugin_paths)]
 
     return plugin_paths
 
-def log(obj, msg, level): 
-    current_time = datetime.utcnow().strftime("%Y/%m/%d %H:%M:%S.%f")
-    msg = "%s [%s] <%s> ::: %s " %(current_time, level, obj.name, msg)
-    obj.logger.log(msg, level)
-
 #wraps logging calls around function execution
 def log_execution(level="DEBUG", start_msg = None, end_msg = None, timeit=True):
     def log_decorator(func):
         @wraps(func)
         def wrapper(obj, *args, **kwargs):
             start = start_msg
             end = end_msg
@@ -375,8 +378,11 @@
     if source_file_type == "csv":
         data = pd.read_csv(source_file, engine=engine, **kwargs)
     elif source_file_type in ["parquet", "pq"]:
         data = pd.read_parquet(source_file, engine=engine, **kwargs)
     else:
         raise Exception("Unsupported file type: %s" % source_file_type)
     
-    return data
+    return data
+
+def chunker(seq, size):
+    return (seq[pos:pos + size] for pos in range(0, len(seq), size))
```

### Comparing `lolpop-0.1.0a2/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a3/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a3/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a3/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/pyproject.toml` & `lolpop-0.1.0a3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,84 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.2"
+version = "v0.1.0-alpha.3"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
 packages = [
     {include = "lolpop"},
     ]
-include = ["templates", "cli"]
+#include = ["templates", "cli"]
 
 #should break this out into dependency groups/extras: 
 #https://python-poetry.org/docs/pyproject/#:~:text=See-,Dependency%20groups,-for%20a%20more
 #https://python-poetry.org/docs/pyproject/#extras
 [tool.poetry.dependencies]
-python = ">=3.9"
-google-auth="2.16.1"
-google-auth-oauthlib="1.0.0"
-google-auth-httplib2="0.1.0" 
-google-api-python-client="2.79.0"
-hydra-core="1.2.0"
-joblib="1.1.0"
-mlflow="2.2.2"
-numpy="1.22.4"
+python = ">=3.9,<3.11"
+google-auth="^2.16.1"
+google-auth-oauthlib="^1.0.0"
+google-auth-httplib2="^0.1.0" 
+google-api-python-client="^2.79.0"
+google-cloud-bigquery="^3.10.0"
+google-cloud-storage="^2.7.0"
+hydra-core="^1.2.0"
+joblib="^1.2.0"
+mlflow="^2.2.2"
+numpy="^1.23.3"
 omegaconf="2.2.3"
-pandas="1.4.2"
-prefect="2.6.6"
-scikit_learn="1.1.2"
-SQLAlchemy="1.4.37"
-xgboost="1.6.1"
-#prefect-dbt="0.2.6"
-dbt-core="1.3"
-dbt-snowflake="1.3"
-#prefect-snowflake="0.2.2"
-pyarrow="6.0.1"
-sweetviz="2.1.4"
-#pandas-profiling="3.5.0"
-dvc="2.37.0"
-dvc-gs="2.20.0"
+pandas="^1.4.2"
+prefect="^2.6.6"
+scikit_learn="1.2.2"
+SQLAlchemy="^1.4.37"
+xgboost="^1.6.1"
+#prefect-dbt="^0.2.6"
+dbt-core="^1.3"
+dbt-snowflake="^1.3"
+#prefect-snowflake="^0.2.2"
+pyarrow="^6.0.1"
+sweetviz="^2.1.4"
+#pandas-profiling="^3.5.0"
+dvc="^2.37.0"
+dvc-gs="^2.20.0"
 deepchecks="^0.13.0"
 evidently="^0.2.1"
-optuna="3.0.4"
-alibi = {version = "0.8.0", extras = ["shap"]}
-yellowbrick="1.4"
-aif360="0.5.0"
-#aif360[all] #fails if R is not installed
+optuna="^3.0.4"
+alibi = {version = "^0.8.0", extras = ["shap"]}
+yellowbrick="^1.4"
+aif360="^0.5.0"
 continual="^2.0.0a51"
-ydata-profiling="4.0.0"
-snowflake-sqlalchemy="1.4.6"
-tqdm="4.64.1"
-sdv="1.0.0b1"
-metaflow="2.8.3"
+ydata-profiling="^4.0.0"
+snowflake-sqlalchemy="^1.4.6"
+tqdm="^4.64.1"
+sdv={version="^1.0.1",optional=true}
+metaflow="^2.8.3"
+duckdb={version="^0.7.1", optional=true}
+databricks-sql-connector={version="^2.5.2", optional=true}
+boto3={version="^1.26.89", optional=true}
+db-dtypes={version="^1.1.1", optional=true}
+psychopg2={version="^2.9.6", optional=true}
+openai="^0.27.6"
+
+[tool.poetry.extras]
+duckdb = ["duckdb"]
+databricks = ["databricks-sql-connector"]
+cli = ["sdv", "openai"]
+aws = ["boto3"]
+google = ["google-cloud-bigquery", "google-cloud-storage", "db-dtypes"]
+redshift = ["psychopg2"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 faker = "^14.0"
 
 [tool.poetry.scripts]
-lolpop = "cli.cli:app"
+lolpop = "lolpop.cli.cli:app"
 
 #[tool.poetry.plugins]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lolpop-0.1.0a2/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a3/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a3/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/component/__init__.py` & `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,22 @@
     from lolpop.component import BaseComponent
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
     subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
-               if ((x[0] != "_") and (".py" not in x))]
+               if ((x[0] != "_") and (x[0] != ".")  and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs:
         files = [x for x in os.listdir(subdir) if (
-            (".py" in x) and ("__" not in x))]
+            (".py" in x) and (x[0] != ".")  and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace.
         for file in files:
-            module = import_module("{{cookiecutter.project_name}}.%s.%s.%s" % (
+            module = import_module("lolpop.extension.{{cookiecutter.project_name}}.%s.%s.%s" % (
                 subdir.split("/")[-2], subdir.split("/")[-1], file[:-3]))
             classes = [x for x in dir(module) if isclass(getattr(module, x))]
             components = [x for x in classes if issubclass(
                 getattr(module, x), BaseComponent)]
             globals().update({name: getattr(module, name)
                               for name in components})
```

### Comparing `lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/pipeline/__init__.py` & `lolpop-0.1.0a3/lolpop/pipeline/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 
 def __map_pipelines__():
     from pathlib import Path
     import os
     from importlib import import_module
     from inspect import isclass
-    from lolpop.pipeline import BasePipeline
+    from .base_pipeline import BasePipeline
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
     subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
-               if ((x[0] != "_") and (".py" not in x))]
+               if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
-    for subdir in subdirs:
+    for subdir in subdirs: 
         files = [x for x in os.listdir(subdir) if (
-            (".py" in x) and ("__" not in x))]
-        #from each file, import all classes and register them in the global namespace.
-        for file in files:
-            module = import_module("{{cookiecutter.project_name}}.%s.%s.%s" % (
-                subdir.split("/")[-2], subdir.split("/")[-1], file[:-3]))
-            classes = [x for x in dir(module) if isclass(getattr(module, x))]
-            pipelines = [x for x in classes if issubclass(
-                getattr(module, x), BasePipeline)]
-            globals().update({name: getattr(module, name)
-                              for name in pipelines})
+            (".py" in x) and (x[0] != ".") and ("__" not in x))]
+        #from each file, import all classes and register them in the global namespace. 
+        for file in files: 
+            module = import_module("lolpop.%s.%s.%s" %(subdir.split("/")[-2],subdir.split("/")[-1],file[:-3]))
+            classes = [x for x in dir(module) if isclass(getattr(module,x))]
+            pipelines = [x for x in classes if issubclass(getattr(module, x), BasePipeline)]
+            globals().update({name: getattr(module,name) for name in pipelines})
 
     warnings.resetwarnings()
 
-
-__map_pipelines__()
+__map_pipelines__()
```

### Comparing `lolpop-0.1.0a2/templates/project_template/{{cookiecutter.project_name}}/{{cookiecutter.project_name}}/runner/__init__.py` & `lolpop-0.1.0a3/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     from lolpop.runner import BaseRunner
     import warnings
 
     warnings.filterwarnings("ignore")
     #get current directory and all subdirectors. These represent the resource types
     path = Path(__file__).parent.resolve()
     subdirs = ["%s/%s" % (path, x) for x in os.listdir(path)
-               if ((x[0] != "_") and (".py" not in x))]
+               if ((x[0] != "_") and (x[0] != ".") and (".py" not in x))]
     #for each resource type (i.e. subdir), get all resources implemented in that type (i.e. python files in the subdir)
     for subdir in subdirs:
         files = [x for x in os.listdir(subdir) if (
-            (".py" in x) and ("__" not in x))]
+            (".py" in x) and (x[0] != ".") and ("__" not in x))]
         #from each file, import all classes and register them in the global namespace.
         for file in files:
-            module = import_module("{{cookiecutter.project_name}}.%s.%s.%s" % (
+            module = import_module("lolpop.extension.{{cookiecutter.project_name}}.%s.%s.%s" % (
                 subdir.split("/")[-2], subdir.split("/")[-1], file[:-3]))
             classes = [x for x in dir(module) if isclass(getattr(module, x))]
             runners = [x for x in classes if issubclass(
                 getattr(module, x), BaseRunner)]
             globals().update({name: getattr(module, name) for name in runners})
 
     warnings.resetwarnings()
```

### Comparing `lolpop-0.1.0a2/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a2/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a3/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

