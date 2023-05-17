# Comparing `tmp/aws-cfn-update-0.8.2.tar.gz` & `tmp/aws-cfn-update-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cfn-update-0.8.2.tar", last modified: Wed May  3 17:42:40 2023, max compression
+gzip compressed data, was "aws-cfn-update-0.8.3.tar", last modified: Wed May 17 11:27:54 2023, max compression
```

## Comparing `aws-cfn-update-0.8.2.tar` & `aws-cfn-update-0.8.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.github/workflows/release-image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/aws-cfn-update.iml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/cfnlintPlugin.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.make-release-support
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.release
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Makefile.mk
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    77208 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/add-new-resources/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.json
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/config-rule-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/template.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/container-image/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/container-image/paas-monitor.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/container-image/paas-monitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/cron-schedule-expression/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/cron-schedule-expression/cron.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/lambda-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn_listener_rule_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/latest-ami-update/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/latest-ami-update/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/latest-ami-update/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/oidc-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/oidc-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/oidc-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/packer-latest-ami/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/packer-latest-ami/packer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/remove-resource/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/rest-api-body/
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/state-machine-definition/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/definition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/src/aws_cfn_update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/add_missing_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cfn_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/container_image_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cron_schedule_expression_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/remove_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/statemachine_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:41:54.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/dummy_responses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_cron_schedule_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_oidc_provider_thumbprint_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_remove_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_statemachine_definition_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/tests/update_packer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/test_update_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.161460 aws-cfn-update-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.github/workflows/release-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/aws-cfn-update.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/cfnlintPlugin.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.make-release-support
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.release
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Makefile.mk
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77208 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/add-new-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/config-rule-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/container-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/container-image/paas-monitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/container-image/paas-monitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/cron-schedule-expression/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/cron-schedule-expression/cron.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/lambda-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn_listener_rule_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/latest-ami-update/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/latest-ami-update/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/latest-ami-update/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/oidc-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/oidc-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/oidc-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/packer-latest-ami/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/packer-latest-ami/packer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/remove-resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/rest-api-body/
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/state-machine-definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/definition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.173460 aws-cfn-update-0.8.3/src/aws_cfn_update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/add_missing_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cfn_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/container_image_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cron_schedule_expression_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/remove_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/statemachine_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.173460 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:27:05.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/dummy_responses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_cron_schedule_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_oidc_provider_thumbprint_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_remove_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_statemachine_definition_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/update_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/test_update_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tox.ini
```

### Comparing `aws-cfn-update-0.8.2/.github/workflows/release-image.yaml` & `aws-cfn-update-0.8.3/.github/workflows/release-image.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/.github/workflows/release.yml` & `aws-cfn-update-0.8.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/.idea/aws-cfn-update.iml` & `aws-cfn-update-0.8.3/.idea/aws-cfn-update.iml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/.idea/codeStyles/Project.xml` & `aws-cfn-update-0.8.3/.idea/codeStyles/Project.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/.idea/inspectionProfiles/Project_Default.xml` & `aws-cfn-update-0.8.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/.make-release-support` & `aws-cfn-update-0.8.3/.make-release-support`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/LICENSE` & `aws-cfn-update-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/Makefile.mk` & `aws-cfn-update-0.8.3/Makefile.mk`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/PKG-INFO` & `aws-cfn-update-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.2
+Version: 0.8.3
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.2/Pipfile.lock` & `aws-cfn-update-0.8.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/README.md` & `aws-cfn-update-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.json` & `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.yaml` & `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.json` & `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.yaml` & `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/container-image/paas-monitor.json` & `aws-cfn-update-0.8.3/samples/container-image/paas-monitor.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.json` & `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.yaml` & `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn_listener_rule_provider.py` & `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn_listener_rule_provider.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/latest-ami-update/template.yaml` & `aws-cfn-update-0.8.3/samples/latest-ami-update/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/packer-latest-ami/packer.json` & `aws-cfn-update-0.8.3/samples/packer-latest-ami/packer.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/remove-resource/storage-server.json` & `aws-cfn-update-0.8.3/samples/remove-resource/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/remove-resource/storage-server.yaml` & `aws-cfn-update-0.8.3/samples/remove-resource/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/rest-api-body/api-specification.yaml` & `aws-cfn-update-0.8.3/samples/rest-api-body/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/rest-api-body/aws-extensions.yaml` & `aws-cfn-update-0.8.3/samples/rest-api-body/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.json` & `aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/state-machine-definition/definition.json` & `aws-cfn-update-0.8.3/samples/state-machine-definition/definition.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/samples/state-machine-definition/definition.yaml` & `aws-cfn-update-0.8.3/samples/state-machine-definition/definition.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/setup.cfg` & `aws-cfn-update-0.8.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aws-cfn-update
-version = 0.8.2
+version = 0.8.3
 author = Mark van Holsteijn
 url = https://github.com/binxio/aws-cfn-update
 author_email = mark.vanholsteijn@xebia.com
 description = Programmatically update CloudFormation templates
 long_description = file: README.md
 long_description_content_type = text/markdown
 test_suite = tests
```

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/add_new_resources.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/cfn_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/cfn_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         with open(self.filename, 'r') as f:
             if self.template_format == '.json':
                 self.template = json.load(f, object_pairs_hook=collections.OrderedDict)
             else:
                 yaml = YAML(typ='rt')
                 yaml.preserve_quotes = True
                 yaml.explicit_start = True
+                yaml.width = 4096
                 self.template = yaml.load(f)
 
     def is_cloudformation_template(self):
         """
         returns true if the `self.template` is a AWS CloudFormation template
         """
         return self.template and 'AWSTemplateFormatVersion' in self.template
```

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/cli.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/cli.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/container_image_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/container_image_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/cron_schedule_expression_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/cron_schedule_expression_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/lambda_inline_code_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/latest_ami_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/oidc_provider_thumbprints_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/oidc_provider_thumbprints_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/packer_ami_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/remove_resource.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/remove_resource.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/replace_references.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/replace_references.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/rest_api_body_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update/statemachine_updater.py` & `aws-cfn-update-0.8.3/src/aws_cfn_update/statemachine_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/PKG-INFO` & `aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.2
+Version: 0.8.3
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/SOURCES.txt` & `aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/api-specification.yaml` & `aws-cfn-update-0.8.3/tests/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/aws-extensions.yaml` & `aws-cfn-update-0.8.3/tests/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/dummy_responses.json` & `aws-cfn-update-0.8.3/tests/dummy_responses.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_add_new_resources.py` & `aws-cfn-update-0.8.3/tests/test_add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.3/tests/test_config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_cron_schedule_expression.py` & `aws-cfn-update-0.8.3/tests/test_cron_schedule_expression.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_lambda_inline_code_updater.py` & `aws-cfn-update-0.8.3/tests/test_lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_latest_ami_updater.py` & `aws-cfn-update-0.8.3/tests/test_latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_oidc_provider_thumbprint_updater.py` & `aws-cfn-update-0.8.3/tests/test_oidc_provider_thumbprint_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_packer_ami_updater.py` & `aws-cfn-update-0.8.3/tests/test_packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_remove_resources.py` & `aws-cfn-update-0.8.3/tests/test_remove_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_replace_references.py` & `aws-cfn-update-0.8.3/tests/test_replace_references.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_rest_api_body_updater.py` & `aws-cfn-update-0.8.3/tests/test_rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/test_statemachine_definition_updater.py` & `aws-cfn-update-0.8.3/tests/test_statemachine_definition_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/update_packer/base.py` & `aws-cfn-update-0.8.3/tests/update_packer/base.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/__init__.py` & `aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.2/tests/update_packer/test_update_packer.py` & `aws-cfn-update-0.8.3/tests/update_packer/test_update_packer.py`

 * *Files identical despite different names*

