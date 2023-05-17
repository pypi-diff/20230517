# Comparing `tmp/aws-cfn-update-0.8.3.tar.gz` & `tmp/aws-cfn-update-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cfn-update-0.8.3.tar", last modified: Wed May 17 11:27:54 2023, max compression
+gzip compressed data, was "aws-cfn-update-0.8.4.tar", last modified: Wed May 17 12:01:09 2023, max compression
```

## Comparing `aws-cfn-update-0.8.3.tar` & `aws-cfn-update-0.8.4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.161460 aws-cfn-update-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.github/workflows/release-image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/aws-cfn-update.iml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/cfnlintPlugin.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.make-release-support
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/.release
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Makefile.mk
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    77208 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/add-new-resources/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.json
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/config-rule-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/template.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/config-rule-inline-code/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/container-image/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/container-image/paas-monitor.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/container-image/paas-monitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/cron-schedule-expression/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/cron-schedule-expression/cron.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/lambda-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn_listener_rule_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/latest-ami-update/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/latest-ami-update/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/latest-ami-update/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/oidc-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/oidc-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/oidc-provider/oidc-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/packer-latest-ami/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/packer-latest-ami/packer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/remove-resource/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/remove-resource/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/rest-api-body/
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.169460 aws-cfn-update-0.8.3/samples/state-machine-definition/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/definition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/samples/state-machine-definition/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.165460 aws-cfn-update-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.173460 aws-cfn-update-0.8.3/src/aws_cfn_update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/add_missing_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cfn_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/container_image_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/cron_schedule_expression_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/remove_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/src/aws_cfn_update/statemachine_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.173460 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 11:27:54.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:27:05.000000 aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/dummy_responses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_cron_schedule_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_oidc_provider_thumbprint_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_remove_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/test_statemachine_definition_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/update_packer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:27:54.177460 aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tests/update_packer/test_update_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 11:26:42.000000 aws-cfn-update-0.8.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.github/workflows/release-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/aws-cfn-update.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/cfnlintPlugin.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.make-release-support
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/.release
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Makefile.mk
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    75718 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/add-new-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/config-rule-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/config-rule-inline-code/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/container-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/container-image/paas-monitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/container-image/paas-monitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.199872 aws-cfn-update-0.8.4/samples/cron-schedule-expression/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/cron-schedule-expression/cron.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/lambda-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn_listener_rule_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/latest-ami-update/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/latest-ami-update/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/latest-ami-update/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/oidc-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/oidc-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/oidc-provider/oidc-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/packer-latest-ami/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/packer-latest-ami/packer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/remove-resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/remove-resource/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/rest-api-body/
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.203872 aws-cfn-update-0.8.4/samples/state-machine-definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/definition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/samples/state-machine-definition/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-17 12:01:09.211872 aws-cfn-update-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.195872 aws-cfn-update-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/src/aws_cfn_update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/add_missing_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cfn_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/container_image_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/cron_schedule_expression_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/remove_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/src/aws_cfn_update/statemachine_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 12:01:09.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:00:23.000000 aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/dummy_responses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_cron_schedule_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_oidc_provider_thumbprint_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_remove_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/test_statemachine_definition_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/update_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:01:09.207872 aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tests/update_packer/test_update_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-17 12:00:01.000000 aws-cfn-update-0.8.4/tox.ini
```

### Comparing `aws-cfn-update-0.8.3/.github/workflows/release-image.yaml` & `aws-cfn-update-0.8.4/.github/workflows/release-image.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/.github/workflows/release.yml` & `aws-cfn-update-0.8.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/.idea/aws-cfn-update.iml` & `aws-cfn-update-0.8.4/.idea/aws-cfn-update.iml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/.idea/codeStyles/Project.xml` & `aws-cfn-update-0.8.4/.idea/codeStyles/Project.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/.idea/inspectionProfiles/Project_Default.xml` & `aws-cfn-update-0.8.4/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/.make-release-support` & `aws-cfn-update-0.8.4/.make-release-support`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/LICENSE` & `aws-cfn-update-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/Makefile.mk` & `aws-cfn-update-0.8.4/Makefile.mk`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/PKG-INFO` & `aws-cfn-update-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.3
+Version: 0.8.4
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.3/Pipfile.lock` & `aws-cfn-update-0.8.4/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.973651747358644%*

 * *Differences: {"'default'": "{'boto3': {'hashes': "*

 * *              "['sha256:23523d5d6aa51bba2461d67f6eb458d83b6a52d18e3d953b1ce71209b66462ec', "*

 * *              "'sha256:ba7ca9215a1026620741273da10d0d3cceb9f7649f7c101e616a287071826f9d'], "*

 * *              "'version': '==1.26.135'}, 'botocore': {'hashes': "*

 * *              "['sha256:06502a4473924ef60ac0de908385a5afab9caee6c5b49cf6a330fab0d76ddf5f', "*

 * *              "'sha256:0c61d4e5e04fe5329fa65da6b31492ef9d0d5174d72fc2af69de2ed0f87804ca'], "*

 * *              "'version': '==1.29.13 […]*

```diff
@@ -26,35 +26,35 @@
         },
         "aws-cfn-update": {
             "editable": true,
             "path": "."
         },
         "boto3": {
             "hashes": [
-                "sha256:6648aff15d19927cd26db47eb56362ccd313a1ddbd7aaa3235ef05d05d398252",
-                "sha256:fe8248b80c4f0fdaed8b8779467c4431a5e52177e02ccd137d51ec51194ebb00"
+                "sha256:23523d5d6aa51bba2461d67f6eb458d83b6a52d18e3d953b1ce71209b66462ec",
+                "sha256:ba7ca9215a1026620741273da10d0d3cceb9f7649f7c101e616a287071826f9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.125"
+            "version": "==1.26.135"
         },
         "botocore": {
             "hashes": [
-                "sha256:3005a7ffee083315e69938acdf1bfeaf9e21fe1fe1643d6573ee817721f4ffcd",
-                "sha256:ac87b63e9aa4231cd28941945024a0c4470c184c60334ebe5e1cae3544c785ed"
+                "sha256:06502a4473924ef60ac0de908385a5afab9caee6c5b49cf6a330fab0d76ddf5f",
+                "sha256:0c61d4e5e04fe5329fa65da6b31492ef9d0d5174d72fc2af69de2ed0f87804ca"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.125"
+            "version": "==1.29.135"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -331,22 +331,14 @@
         "pytz": {
             "hashes": [
                 "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
                 "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
             "version": "==2023.3"
         },
-        "pytz-deprecation-shim": {
-            "hashes": [
-                "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6",
-                "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==0.1.0.post0"
-        },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -395,19 +387,19 @@
                 "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.30.0"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:b4c6e66d103d8af198aa6139580ab735169be4922eb4c515ac121bdabf6f9361",
-                "sha256:c22ec58aaca5105f771cb8f7ac45ad631b5e8b00454ebe1822d442fb696e9e62"
+                "sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693",
+                "sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.22"
+            "version": "==0.17.26"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
@@ -440,48 +432,40 @@
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
                 "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
                 "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
-            "markers": "python_version < '3.11' and platform_python_implementation == 'CPython'",
+            "markers": "python_version < '3.12' and platform_python_implementation == 'CPython'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
-                "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
+                "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
+                "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
-        "tzdata": {
-            "hashes": [
-                "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
-                "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2023.3"
-        },
         "tzlocal": {
             "hashes": [
-                "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355",
-                "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"
+                "sha256:46eb99ad4bdb71f3f72b7d24f4267753e240944ecfc16f25d2719ba89827a803",
+                "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.3"
+            "version": "==5.0.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
@@ -507,27 +491,27 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:6648aff15d19927cd26db47eb56362ccd313a1ddbd7aaa3235ef05d05d398252",
-                "sha256:fe8248b80c4f0fdaed8b8779467c4431a5e52177e02ccd137d51ec51194ebb00"
+                "sha256:23523d5d6aa51bba2461d67f6eb458d83b6a52d18e3d953b1ce71209b66462ec",
+                "sha256:ba7ca9215a1026620741273da10d0d3cceb9f7649f7c101e616a287071826f9d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.125"
+            "version": "==1.26.135"
         },
         "botocore": {
             "hashes": [
-                "sha256:3005a7ffee083315e69938acdf1bfeaf9e21fe1fe1643d6573ee817721f4ffcd",
-                "sha256:ac87b63e9aa4231cd28941945024a0c4470c184c60334ebe5e1cae3544c785ed"
+                "sha256:06502a4473924ef60ac0de908385a5afab9caee6c5b49cf6a330fab0d76ddf5f",
+                "sha256:0c61d4e5e04fe5329fa65da6b31492ef9d0d5174d72fc2af69de2ed0f87804ca"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.125"
+            "version": "==1.29.135"
         },
         "build": {
             "hashes": [
                 "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
@@ -539,19 +523,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -768,19 +752,19 @@
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
@@ -894,19 +878,19 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -995,22 +979,14 @@
         "pytz": {
             "hashes": [
                 "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
                 "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
             "version": "==2023.3"
         },
-        "pytz-deprecation-shim": {
-            "hashes": [
-                "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6",
-                "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==0.1.0.post0"
-        },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
@@ -1091,19 +1067,19 @@
                 "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.3.5"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:b4c6e66d103d8af198aa6139580ab735169be4922eb4c515ac121bdabf6f9361",
-                "sha256:c22ec58aaca5105f771cb8f7ac45ad631b5e8b00454ebe1822d442fb696e9e62"
+                "sha256:25d0ee82a0a9a6f44683dcf8c282340def4074a4562f3a24f55695bb254c1693",
+                "sha256:baa2d0a5aad2034826c439ce61c142c07082b76f4791d54145e131206e998059"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.22"
+            "version": "==0.17.26"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
@@ -1136,24 +1112,24 @@
                 "sha256:df5828871e6648db72d1c19b4bd24819b80a755c4541d3409f0f7acd0f335c80",
                 "sha256:ecdf1a604009bd35c674b9225a8fa609e0282d9b896c03dd441a91e5f53b534e",
                 "sha256:efa08d63ef03d079dcae1dfe334f6c8847ba8b645d08df286358b1f5293d24ab",
                 "sha256:f01da5790e95815eb5a8a138508c01c758e5f5bc0ce4286c4f7028b8dd7ac3d0",
                 "sha256:f34019dced51047d6f70cb9383b2ae2853b7fc4dce65129a5acd49f4f9256646",
                 "sha256:f6d3d39611ac2e4f62c3128a9eed45f19a6608670c5a2f4f07f24e8de3441d38"
             ],
-            "markers": "python_version < '3.11' and platform_python_implementation == 'CPython'",
+            "markers": "python_version < '3.12' and platform_python_implementation == 'CPython'",
             "version": "==0.2.7"
         },
         "s3transfer": {
             "hashes": [
-                "sha256:06176b74f3a15f61f1b4f25a1fc29a4429040b7647133a463da8fa5bd28d5ecd",
-                "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
+                "sha256:3c0da2d074bf35d6870ef157158641178a4204a6e689e82546083e31e0311346",
+                "sha256:640bb492711f4c0c0905e1f62b6aaeb771881935ad27884852411f8e9cacbca9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.6.0"
+            "version": "==0.6.1"
         },
         "setuptools": {
             "hashes": [
                 "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
                 "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
             "markers": "python_version >= '3.7'",
@@ -1203,29 +1179,21 @@
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
-        "tzdata": {
-            "hashes": [
-                "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
-                "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2023.3"
-        },
         "tzlocal": {
             "hashes": [
-                "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355",
-                "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"
+                "sha256:46eb99ad4bdb71f3f72b7d24f4267753e240944ecfc16f25d2719ba89827a803",
+                "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.3"
+            "version": "==5.0.1"
         },
         "urllib3": {
             "hashes": [
                 "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
```

### Comparing `aws-cfn-update-0.8.3/README.md` & `aws-cfn-update-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.json` & `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server-new.yaml` & `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server-new.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.json` & `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/add-new-resources/storage-server.yaml` & `aws-cfn-update-0.8.4/samples/add-new-resources/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/container-image/paas-monitor.json` & `aws-cfn-update-0.8.4/samples/container-image/paas-monitor.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.json` & `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn-listener-rule-provider.yaml` & `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn-listener-rule-provider.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/lambda-inline-code/cfn_listener_rule_provider.py` & `aws-cfn-update-0.8.4/samples/lambda-inline-code/cfn_listener_rule_provider.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/latest-ami-update/template.yaml` & `aws-cfn-update-0.8.4/samples/latest-ami-update/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/packer-latest-ami/packer.json` & `aws-cfn-update-0.8.4/samples/packer-latest-ami/packer.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/remove-resource/storage-server.json` & `aws-cfn-update-0.8.4/samples/remove-resource/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/remove-resource/storage-server.yaml` & `aws-cfn-update-0.8.4/samples/remove-resource/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/rest-api-body/api-specification.yaml` & `aws-cfn-update-0.8.4/samples/rest-api-body/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/rest-api-body/aws-extensions.yaml` & `aws-cfn-update-0.8.4/samples/rest-api-body/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/rest-api-body/rest-api.json` & `aws-cfn-update-0.8.4/samples/rest-api-body/rest-api.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/state-machine-definition/definition.json` & `aws-cfn-update-0.8.4/samples/state-machine-definition/definition.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/samples/state-machine-definition/definition.yaml` & `aws-cfn-update-0.8.4/samples/state-machine-definition/definition.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/add_new_resources.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/add_new_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,28 @@
 class AddNewResources(CfnUpdater):
     """
     add resources that exist in the new template and not in the existing template
     """
 
     def __init__(self):
         super(AddNewResources, self).__init__()
-        self.source:dict = {}
+        self.source: dict = {}
 
     def update_template(self):
         self.dirty = add_missing_resources(self.template, self.source)
 
 
-@click.command(name='add-new-resources', help=AddNewResources.__doc__)
-@click.option('--source', required=True, help='template to add resources from', type=click.Path(exists=True))
-@click.argument('path', nargs=1, required=True, type=click.Path(exists=True))
+@click.command(name="add-new-resources", help=AddNewResources.__doc__)
+@click.option(
+    "--source",
+    required=True,
+    help="template to add resources from",
+    type=click.Path(exists=True),
+)
+@click.argument("path", nargs=1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def add_new_resources(ctx, source, path):
     updater = AddNewResources()
-    updater.dry_run = ctx.obj['dry_run']
-    updater.verbose = ctx.obj['verbose']
+    updater.dry_run = ctx.obj["dry_run"]
+    updater.verbose = ctx.obj["verbose"]
     updater.source = read_template(source)
     updater.update(path)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/cfn_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/cfn_updater.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,44 @@
 import json
 import collections
 from ruamel.yaml import YAML
 
 
 class CfnUpdater(object):
     """
-    base class for a CloudFormation  update. To implement a specific updater: 
+    base class for a CloudFormation  update. To implement a specific updater:
 
     - inherit this class
     - override the method update_template()
     - call the method update(path)
 
-    it will read the template from files with extension .yaml, .yml and .json into 
+    it will read the template from files with extension .yaml, .yml and .json into
     the property `self.template`.
 
-    If the property `self.dirty` is set to True, the template will be written 
+    If the property `self.dirty` is set to True, the template will be written
     back to the originating file.
 
-    Please note that formatting and comments may be lost, when using this 
+    Please note that formatting and comments may be lost, when using this
     updater.
     """
 
     def __init__(self):
         self.basename = None
         self.template = False
         self.template = None
         self.template_format = None
         self.dirty = False
         self.dry_run = False
         self.verbose = False
         self._filename = None
+        self.yaml = YAML(typ="rt")
+        self.yaml.preserve_quotes = True
+        self.yaml.explicit_start = True
+        self.yaml.width = 4096
+        self.yaml.indent(mapping=2, sequence=4, offset=2)
 
     @property
     def filename(self):
         """
         current template filename
         """
         return self._filename
@@ -63,97 +68,97 @@
         """
         self._filename = filename
         parts = os.path.splitext(os.path.basename(filename))
         self.basename = parts[0]
         self.template_format = parts[1]
         self.template = None
         self.dirty = False
-        if self.template_format not in ('.json', '.yml', '.yaml'):
-            raise ValueError('%s has no .json, .yaml or .yml extension.' % filename)
+        if self.template_format not in (".json", ".yml", ".yaml"):
+            raise ValueError("%s has no .json, .yaml or .yml extension." % filename)
 
     def load(self):
         """
         loads `template` from `filename` as dictionary.
         """
         self.dirty = False
         self.template = None
-        with open(self.filename, 'r') as f:
-            if self.template_format == '.json':
+        with open(self.filename, "r") as f:
+            if self.template_format == ".json":
                 self.template = json.load(f, object_pairs_hook=collections.OrderedDict)
             else:
-                yaml = YAML(typ='rt')
-                yaml.preserve_quotes = True
-                yaml.explicit_start = True
-                yaml.width = 4096
-                self.template = yaml.load(f)
+                self.template = self.yaml.load(f)
 
     def is_cloudformation_template(self):
         """
         returns true if the `self.template` is a AWS CloudFormation template
         """
-        return self.template and 'AWSTemplateFormatVersion' in self.template
+        return self.template and "AWSTemplateFormatVersion" in self.template
 
     def write(self):
         """
         write modified content from `template` to `filename`. It will retain it's original
         format (yaml or json) but loose original formatting and comments.
         """
         if not self.dirty:
             if self.verbose:
-                sys.stderr.write('INFO: no changes in {}\n'.format(self.filename))
+                sys.stderr.write("INFO: no changes in {}\n".format(self.filename))
             return
 
         if self.dry_run:
             return
 
-        with open(self.filename, 'w') as f:
-            if self.template_format == '.yaml':
-                yaml = YAML()
-                yaml.explicit_start = True
-                yaml.indent(mapping=2, sequence=4, offset=2)
-                yaml.dump(self.template, f)
+        with open(self.filename, "w") as f:
+            if self.template_format == ".yaml":
+                self.yaml.dump(self.template, f)
             else:
-                json.dump(self.template, f, separators=(',', ': '), indent=2)
+                json.dump(self.template, f, separators=(",", ": "), indent=2)
 
     def update_template(self):
         """
         implement the update logic of `self.template`. Set self.dirty to True, if you modified.
         """
         pass
 
     @property
     def resources(self):
-        return self.template.get('Resources', {})
+        return self.template.get("Resources", {})
 
     def update(self, path):
         """
         recursively updates all the cloudformation templates in the specified `path`. `path` may be a file,
         a directory or a list of paths.
         """
         if isinstance(path, (list, tuple)):
             for p in path:
                 self.update(p)
         elif os.path.isfile(path):
-            if path.endswith('.yml') or path.endswith('.yaml') or path.endswith('.json'):
+            if (
+                path.endswith(".yml")
+                or path.endswith(".yaml")
+                or path.endswith(".json")
+            ):
                 self.filename = path
                 self.load()
                 if self.is_cloudformation_template():
                     self.update_template()
                     self.write()
                 else:
                     if self.verbose:
-                        sys.stderr.write('INFO: skipping {} as it is not a CloudFormation template\n'.format(path))
+                        sys.stderr.write(
+                            "INFO: skipping {} as it is not a CloudFormation template\n".format(
+                                path
+                            )
+                        )
         elif os.path.isdir(path):
             for root, dirs, files in os.walk(path):
                 for f in files:
                     self.update(os.path.join(root, f))
         else:
-            sys.stderr.write('ERROR: {} is not a file or directory\n'.format(path))
+            sys.stderr.write("ERROR: {} is not a file or directory\n".format(path))
             sys.exit(1)
 
+
 def read_template(filename: str) -> dict:
     src = CfnUpdater()
     src.filename = filename
     src.load()
     return src.template
-
-yaml = YAML()
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/cli.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,122 +18,202 @@
 from aws_cfn_update.packer_ami_updater import main as packer_latest_ami
 
 import click
 import pytz
 
 from aws_cfn_update.config_rule_inline_code_updater import ConfigRuleInlineCodeUpdater
 from aws_cfn_update.container_image_updater import ContainerImageUpdater
-from aws_cfn_update.cron_schedule_expression_updater import CronScheduleExpressionUpdater
+from aws_cfn_update.cron_schedule_expression_updater import (
+    CronScheduleExpressionUpdater,
+)
 from aws_cfn_update.latest_ami_updater import AMIUpdater
 from aws_cfn_update.rest_api_body_updater import RestAPIBodyUpdater
 from aws_cfn_update.lambda_inline_code_updater import LambdaInlineCodeUpdater
 from aws_cfn_update.statemachine_updater import update_state_machine_definition
 from aws_cfn_update.remove_resource import remove_resource
 from aws_cfn_update.add_new_resources import add_new_resources
-from aws_cfn_update.oidc_provider_thumbprints_updater import update_oidc_provider_thumbprint
+from aws_cfn_update.oidc_provider_thumbprints_updater import (
+    update_oidc_provider_thumbprint,
+)
 
 
 @click.group()
-@click.option('--dry-run', is_flag=True, default=False,
-              help='do not change anything, just show what is going to happen')
-@click.option('--verbose', is_flag=True, default=False, help='show more output')
+@click.option(
+    "--dry-run",
+    is_flag=True,
+    default=False,
+    help="do not change anything, just show what is going to happen",
+)
+@click.option("--verbose", is_flag=True, default=False, help="show more output")
 @click.pass_context
 def cli(ctx, dry_run, verbose):
     """Programmatically update CloudFormation templates"""
     ctx.obj = copy(ctx.params)
 
 
 def validate_image(ctx, param, value):
-    if re.match(r'(?:.+/)?([^:]+)(?::.+)?', value):
+    if re.match(r"(?:.+/)?([^:]+)(?::.+)?", value):
         return value
     else:
-        raise click.BadParameter('"{}" is not a valid docker image specification'.format(value))
+        raise click.BadParameter(
+            '"{}" is not a valid docker image specification'.format(value)
+        )
 
 
-@cli.command(name='container-image', help=ContainerImageUpdater.__doc__)
-@click.option('--image', required=True, callback=validate_image, help='to update to')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+@cli.command(name="container-image", help=ContainerImageUpdater.__doc__)
+@click.option("--image", required=True, callback=validate_image, help="to update to")
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def task_image(ctx, image, path):
     updater = ContainerImageUpdater()
-    updater.main(image, ctx.obj['dry_run'], ctx.obj['verbose'], list(path))
+    updater.main(image, ctx.obj["dry_run"], ctx.obj["verbose"], list(path))
 
 
-@cli.command(name='latest-ami', help=AMIUpdater.__doc__)
-@click.option('--ami-name-pattern', required=True, help='glob style pattern of the AMI image name to use')
-@click.option('--add-new-version', is_flag=True, default=False, help='of the AMI resource and replace all references')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+@cli.command(name="latest-ami", help=AMIUpdater.__doc__)
+@click.option(
+    "--ami-name-pattern",
+    required=True,
+    help="glob style pattern of the AMI image name to use",
+)
+@click.option(
+    "--add-new-version",
+    is_flag=True,
+    default=False,
+    help="of the AMI resource and replace all references",
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def ami_image_update(ctx, ami_name_pattern, add_new_version, path):
     updater = AMIUpdater()
-    updater.main(ami_name_pattern, ctx.obj['dry_run'], ctx.obj['verbose'], add_new_version, list(path))
-
-
-@cli.command(name='cron-schedule-expression', help=CronScheduleExpressionUpdater.__doc__)
-@click.option('--timezone', required=False, help='to use to calculate the UTC time', default="Europe/Amsterdam")
-@click.option('--date', type=click.DateTime(), default=datetime.now(),
-              help='to use as reference date')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+    updater.main(
+        ami_name_pattern,
+        ctx.obj["dry_run"],
+        ctx.obj["verbose"],
+        add_new_version,
+        list(path),
+    )
+
+
+@cli.command(
+    name="cron-schedule-expression", help=CronScheduleExpressionUpdater.__doc__
+)
+@click.option(
+    "--timezone",
+    required=False,
+    help="to use to calculate the UTC time",
+    default="Europe/Amsterdam",
+)
+@click.option(
+    "--date",
+    type=click.DateTime(),
+    default=datetime.now(),
+    help="to use as reference date",
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def cron_schedule_expression(ctx, timezone, date, path):
     updater = CronScheduleExpressionUpdater()
     try:
         tz = pytz.timezone(timezone)
-        updater.main(tz, date, ctx.obj['dry_run'], ctx.obj['verbose'], list(path))
+        updater.main(tz, date, ctx.obj["dry_run"], ctx.obj["verbose"], list(path))
     except pytz.exceptions.UnknownTimeZoneError:
-        raise click.BadParameter('invalid timezone specified', ctx=ctx, param='timezone')
-
-
-@cli.command(name='rest-api-body', help=RestAPIBodyUpdater.__doc__)
-@click.option('--resource', required=True, help='AWS::ApiGateway::RestApi body to update')
-@click.option('--open-api-specification', required=True, type=click.Path(exists=True), help='defining the interface')
-@click.option('--api-gateway-extensions', required=True, type=click.Path(exists=True),
-              help='to add the the specification')
-@click.option('--add-new-version', is_flag=True, default=False,
-              help='of the RestAPI resource and replace all references')
-@click.option('--keep', default=1, help='number of versions to keep, if --add-new-version is specified')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
-@click.pass_context
-def swagger_document(ctx, resource, open_api_specification, api_gateway_extensions, path, add_new_version, keep):
+        raise click.BadParameter(
+            "invalid timezone specified", ctx=ctx, param="timezone"
+        )
+
+
+@cli.command(name="rest-api-body", help=RestAPIBodyUpdater.__doc__)
+@click.option(
+    "--resource", required=True, help="AWS::ApiGateway::RestApi body to update"
+)
+@click.option(
+    "--open-api-specification",
+    required=True,
+    type=click.Path(exists=True),
+    help="defining the interface",
+)
+@click.option(
+    "--api-gateway-extensions",
+    required=True,
+    type=click.Path(exists=True),
+    help="to add the the specification",
+)
+@click.option(
+    "--add-new-version",
+    is_flag=True,
+    default=False,
+    help="of the RestAPI resource and replace all references",
+)
+@click.option(
+    "--keep",
+    default=1,
+    help="number of versions to keep, if --add-new-version is specified",
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
+@click.pass_context
+def swagger_document(
+    ctx,
+    resource,
+    open_api_specification,
+    api_gateway_extensions,
+    path,
+    add_new_version,
+    keep,
+):
     updater = RestAPIBodyUpdater()
-    updater.main(resource, open_api_specification, api_gateway_extensions, list(path), add_new_version, keep,
-                 ctx.obj['dry_run'], ctx.obj['verbose'])
-
-
-@cli.command(name='lambda-inline-code', help=LambdaInlineCodeUpdater.__doc__)
-@click.option('--resource', required=True, help='name of the AWS::Lambda::Function to update')
-@click.option('--file', required=True, type=click.Path(exists=True), help='containing the source')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+    updater.main(
+        resource,
+        open_api_specification,
+        api_gateway_extensions,
+        list(path),
+        add_new_version,
+        keep,
+        ctx.obj["dry_run"],
+        ctx.obj["verbose"],
+    )
+
+
+@cli.command(name="lambda-inline-code", help=LambdaInlineCodeUpdater.__doc__)
+@click.option(
+    "--resource", required=True, help="name of the AWS::Lambda::Function to update"
+)
+@click.option(
+    "--file", required=True, type=click.Path(exists=True), help="containing the source"
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def lambda_body(ctx, resource, file, path):
     updater = LambdaInlineCodeUpdater()
 
-    with open(file, 'r') as f:
+    with open(file, "r") as f:
         body = f.read()
-    updater.main(resource, body, list(path), ctx.obj['dry_run'], ctx.obj['verbose'])
+    updater.main(resource, body, list(path), ctx.obj["dry_run"], ctx.obj["verbose"])
 
 
-@cli.command(name='config-rule-inline-code', help=ConfigRuleInlineCodeUpdater.__doc__)
-@click.option('--resource', required=True, help='name of the AWS::Config::ConfigRule')
-@click.option('--file', required=True, type=click.Path(exists=True), help='containing the source')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+@cli.command(name="config-rule-inline-code", help=ConfigRuleInlineCodeUpdater.__doc__)
+@click.option("--resource", required=True, help="name of the AWS::Config::ConfigRule")
+@click.option(
+    "--file", required=True, type=click.Path(exists=True), help="containing the source"
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def config_rule_body(ctx, resource, file, path):
     updater = ConfigRuleInlineCodeUpdater()
 
-    with open(file, 'r') as f:
+    with open(file, "r") as f:
         body = f.read()
-    updater.main(resource, body, list(path), ctx.obj['dry_run'], ctx.obj['verbose'])
+    updater.main(resource, body, list(path), ctx.obj["dry_run"], ctx.obj["verbose"])
 
 
 cli.add_command(update_state_machine_definition)
 cli.add_command(remove_resource)
 cli.add_command(add_new_resources)
 cli.add_command(packer_latest_ami)
 cli.add_command(update_oidc_provider_thumbprint)
 
+
 def main():
     cli()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/config_rule_inline_code_updater.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,75 +15,83 @@
 import sys
 from .cfn_updater import CfnUpdater
 from ruamel.yaml.scalarstring import PreservedScalarString
 
 
 class ConfigRuleInlineCodeUpdater(CfnUpdater):
     """
-    Updates the inline code of an AWS::Config::ConfigRule resource.
+        Updates the inline code of an AWS::Config::ConfigRule resource.
 
-\b
-  ConfigRule:
-    Type: AWS::Config::ConfigRule
-    Properties:
-      Source:
-        Owner: CUSTOM_POLICY
-
-\b
-  ConfigRule:
-    Type: AWS::Config::ConfigRule
-    Properties:
-      Source:
-        Owner: CUSTOM_POLICY
-        CustomPolicyDetails:
-          EnableDebugLogDelivery: true
-          PolicyRuntime: guard-2.x.x
-          PolicyText: |-
-            rule name when resourceType == "AWS::S3::Bucket" {
-                ...
-            }
-          ...
+    \b
+      ConfigRule:
+        Type: AWS::Config::ConfigRule
+        Properties:
+          Source:
+            Owner: CUSTOM_POLICY
+
+    \b
+      ConfigRule:
+        Type: AWS::Config::ConfigRule
+        Properties:
+          Source:
+            Owner: CUSTOM_POLICY
+            CustomPolicyDetails:
+              EnableDebugLogDelivery: true
+              PolicyRuntime: guard-2.x.x
+              PolicyText: |-
+                rule name when resourceType == "AWS::S3::Bucket" {
+                    ...
+                }
+              ...
     """
 
     def __init__(self):
         super(ConfigRuleInlineCodeUpdater, self).__init__()
         self._image = []
         self.resource_name = None
         self.code = None
 
     def update_template(self):
         """
         updates the Code property of a AWS::Config::ConfigRule resource of name `self.resource` to `self.code`
         """
-        resource = self.template.get('Resources', {}).get(self.resource_name, None)
-        properties = resource.get('Properties', {})
+        resource = self.template.get("Resources", {}).get(self.resource_name, None)
+        properties = resource.get("Properties", {})
         if (
-                resource
-                and resource["Type"] == "AWS::Config::ConfigRule"
-                and properties.get("Source", {}).get("Owner") == "CUSTOM_POLICY"
+            resource
+            and resource["Type"] == "AWS::Config::ConfigRule"
+            and properties.get("Source", {}).get("Owner") == "CUSTOM_POLICY"
         ):
-            source = properties.get('Source', {})
-            details = source.get('CustomPolicyDetails', {})
-            old_code = details.get('PolicyText', None)
+            source = properties.get("Source", {})
+            details = source.get("CustomPolicyDetails", {})
+            old_code = details.get("PolicyText", None)
 
             if old_code != self.code:
                 sys.stderr.write(
-                    'INFO: updating policy text of config rule {} in {}\n'.format(self.resource_name, self.filename))
-                if 'Properties' not in resource:
-                    resource['Properties'] = {}
-                if 'Source' not in resource['Properties']:
-                    resource['Properties']['Source'] = {}
-                if 'CustomPolicyDetails' not in resource['Properties']['Source']:
-                    resource['Properties']['Source']['CustomPolicyDetails'] = {}
-
-                resource['Properties']['Source']['CustomPolicyDetails']['PolicyText'] = PreservedScalarString(self.code)
+                    "INFO: updating policy text of config rule {} in {}\n".format(
+                        self.resource_name, self.filename
+                    )
+                )
+                if "Properties" not in resource:
+                    resource["Properties"] = {}
+                if "Source" not in resource["Properties"]:
+                    resource["Properties"]["Source"] = {}
+                if "CustomPolicyDetails" not in resource["Properties"]["Source"]:
+                    resource["Properties"]["Source"]["CustomPolicyDetails"] = {}
+
+                resource["Properties"]["Source"]["CustomPolicyDetails"][
+                    "PolicyText"
+                ] = PreservedScalarString(self.code)
                 self.dirty = True
         elif resource:
             sys.stderr.write(
-                'WARN: resource {} in {} is not a CUSTOM_POLICY of type AWS::Config::ConfigRule\n'.format(self.resource_name, self.filename))
+                "WARN: resource {} in {} is not a CUSTOM_POLICY of type AWS::Config::ConfigRule\n".format(
+                    self.resource_name, self.filename
+                )
+            )
 
     def main(self, resource, code, paths, dry_run, verbose):
         self.resource_name = resource
         self.code = code
         self.dry_run = dry_run
         self.verbose = verbose
         self.update(paths)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/container_image_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/container_image_updater.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,89 +14,97 @@
 #   Copyright 2018 binx.io B.V.
 import sys
 from .cfn_updater import CfnUpdater
 
 
 class ContainerImageUpdater(CfnUpdater):
     """
-    Updates the Docker image of ECS Container Definitions.
+        Updates the Docker image of ECS Container Definitions.
 
-    it will update any container definition where the base image name matches
-    the specified image name excluding the tag.
+        it will update any container definition where the base image name matches
+        the specified image name excluding the tag.
 
-    For example, an image name of `mvanholsteijn/paas-monitor:0.6.0` will update:
+        For example, an image name of `mvanholsteijn/paas-monitor:0.6.0` will update:
 
-\b
-        Type: AWS::ECS::TaskDefinition
-        Properties:
-          ContainerDefinitions:
-            - Name: paas-monitor
-              Image: mvanholsteijn/paas-monitor:0.5.9
-
-    to:
-
-\b
-        Type: AWS::ECS::TaskDefinition
-        Properties:
-          ContainerDefinitions:
-            - Name: paas-monitor
-              Image: mvanholsteijn/paas-monitor:0.6.0
+    \b
+            Type: AWS::ECS::TaskDefinition
+            Properties:
+              ContainerDefinitions:
+                - Name: paas-monitor
+                  Image: mvanholsteijn/paas-monitor:0.5.9
+
+        to:
+
+    \b
+            Type: AWS::ECS::TaskDefinition
+            Properties:
+              ContainerDefinitions:
+                - Name: paas-monitor
+                  Image: mvanholsteijn/paas-monitor:0.6.0
 
     """
 
     def __init__(self):
         super(ContainerImageUpdater, self).__init__()
         self._image = []
 
     @property
     def image(self):
-        return ':'.join(self._image)
+        return ":".join(self._image)
 
     @image.setter
     def image(self, image):
-        self._image = image.split(':', 2) if image is not None else []
+        self._image = image.split(":", 2) if image is not None else []
 
     @property
     def base_image(self):
-        return self._image[0] if self._image is not None and len(self._image) > 0 else ''
+        return (
+            self._image[0] if self._image is not None and len(self._image) > 0 else ""
+        )
 
     @property
     def image_tag(self):
-        return self._image[1] if self._image is not None and len(self._image) > 1 else ''
+        return (
+            self._image[1] if self._image is not None and len(self._image) > 1 else ""
+        )
 
     @staticmethod
     def is_task_definition(resource):
         """
         returns true if the resource is of type AWS::ECS::TaskDefinition
         """
-        return resource.get('Type', '') == 'AWS::ECS::TaskDefinition'
+        return resource.get("Type", "") == "AWS::ECS::TaskDefinition"
 
     def is_matching_container(self, container):
         """
         returns true if there is a match on the image
         """
-        return container.get('Image', '').split(':')[0] == self.base_image
+        return container.get("Image", "").split(":")[0] == self.base_image
 
     def all_matching_task_definitions(self, resources):
         return filter(lambda n: self.is_task_definition(resources[n]), resources)
 
     def update_template(self):
         """
         updates the Image of container definitions in the CFN template `self.template`.
         """
-        resources = self.template.get('Resources', {})
+        resources = self.template.get("Resources", {})
         for task_name in self.all_matching_task_definitions(resources):
             task = resources[task_name]
-            containers = task.get('Properties', {}).get('ContainerDefinitions', [])
-            for container in filter(lambda c: self.is_matching_container(c), containers):
-                if container['Image'] != self.image:
+            containers = task.get("Properties", {}).get("ContainerDefinitions", [])
+            for container in filter(
+                lambda c: self.is_matching_container(c), containers
+            ):
+                if container["Image"] != self.image:
                     sys.stderr.write(
-                        'INFO: updating image of container definition {} for task {} in {}\n'.format(
-                            container['Name'], task_name, self.filename))
-                    container['Image'] = self.image
+                        "INFO: updating image of container definition {} for task {} in {}\n".format(
+                            container["Name"], task_name, self.filename
+                        )
+                    )
+                    container["Image"] = self.image
                     self.dirty = True
 
     def main(self, image, dry_run, verbose, paths):
         self.image = image
         self.dry_run = dry_run
         self.verbose = verbose
         self.update(paths)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/cron_schedule_expression_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/cron_schedule_expression_updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,49 +20,49 @@
 from tzlocal import get_localzone
 
 from .cfn_updater import CfnUpdater
 
 
 class CronScheduleExpressionUpdater(CfnUpdater):
     """
-    Updates the schedule expression of an AWS::Events::Rules resources to reflect the
-    scheduled time in UTC. The required cron rule is taken from the description. It will
-    update the following resource definition from:
-
-\b
-      DailyTaskSchedule:
-        Type: AWS::Events::Rule
-        Properties:
-          Description: run daily - cron(30 01 * * ? *)
-          Name: run daily
-          ScheduleExpression: cron(30 01 * * ? *)
-          State: ENABLED
-
-to
-
-\b
-      DailyTaskSchedule:
-        Type: AWS::Events::Rule
-        Properties:
-          Description: run daily - cron(30 01 * * ? *)
-          Name: run daily
-          ScheduleExpression: cron(30 23 * * ? *)
-          State: ENABLED
-
-with --timezone Europe/Amsterdam and --date 2018-08-01. If the updater is run with --date 2018-12-01, it
-will change it to:
-
-\b
-      DailyTaskSchedule:
-        Type: AWS::Events::Rule
-        Properties:
-          Description: run daily - cron(30 01 * * ? *)
-          Name: run daily
-          ScheduleExpression: cron(30 00 * * ? *)
-          State: ENABLED
+        Updates the schedule expression of an AWS::Events::Rules resources to reflect the
+        scheduled time in UTC. The required cron rule is taken from the description. It will
+        update the following resource definition from:
+
+    \b
+          DailyTaskSchedule:
+            Type: AWS::Events::Rule
+            Properties:
+              Description: run daily - cron(30 01 * * ? *)
+              Name: run daily
+              ScheduleExpression: cron(30 01 * * ? *)
+              State: ENABLED
+
+    to
+
+    \b
+          DailyTaskSchedule:
+            Type: AWS::Events::Rule
+            Properties:
+              Description: run daily - cron(30 01 * * ? *)
+              Name: run daily
+              ScheduleExpression: cron(30 23 * * ? *)
+              State: ENABLED
+
+    with --timezone Europe/Amsterdam and --date 2018-08-01. If the updater is run with --date 2018-12-01, it
+    will change it to:
+
+    \b
+          DailyTaskSchedule:
+            Type: AWS::Events::Rule
+            Properties:
+              Description: run daily - cron(30 01 * * ? *)
+              Name: run daily
+              ScheduleExpression: cron(30 00 * * ? *)
+              State: ENABLED
 
 
     """
 
     def __init__(self):
         super(CronScheduleExpressionUpdater, self).__init__()
         self._timezone = get_localzone()
@@ -88,112 +88,131 @@
     def today(self, dt):
         if dt.tzinfo:
             self._today = dt.replace(tzinfo=self.timezone)
         else:
             self._today = self.timezone.localize(dt)
 
     def is_matching_resource(self, resource):
-        aws_type = resource.get('Type', '')
-        description = resource.get('Properties', {}).get('Description', '')
-        expression = resource.get('Properties', {}).get('ScheduleExpression', None)
+        aws_type = resource.get("Type", "")
+        description = resource.get("Properties", {}).get("Description", "")
+        expression = resource.get("Properties", {}).get("ScheduleExpression", None)
 
-        if aws_type == 'AWS::Events::Rule' and aws_cron_pattern.search(description):
+        if aws_type == "AWS::Events::Rule" and aws_cron_pattern.search(description):
             return expression is None or aws_cron_pattern.search(expression)
 
         return False
 
     def all_matching_resources(self, resources):
         return {k: v for k, v in resources.items() if self.is_matching_resource(v)}
 
     def update_template(self):
         """
         converts the cron expression in `Description` into a UTC expression in `ScheduleExpression`.
         """
-        resources = self.all_matching_resources(self.template.get('Resources', {}))
+        resources = self.all_matching_resources(self.template.get("Resources", {}))
 
         for name, resource in resources.items():
-            description = resource.get('Properties', {}).get('Description', '')
+            description = resource.get("Properties", {}).get("Description", "")
             match = aws_cron_pattern.search(description)
             if match:
-                expression = '{minutes} {hours} {day_of_month} {month} {day_of_week} {year}'.format(**match.groupdict())
+                expression = "{minutes} {hours} {day_of_month} {month} {day_of_week} {year}".format(
+                    **match.groupdict()
+                )
                 new_expression = correct_cron_expression_for_utc(expression, self.today)
                 if expression != new_expression:
-                    properties = resource.get('Properties')
-                    properties['ScheduleExpression'] = 'cron({})'.format(new_expression)
+                    properties = resource.get("Properties")
+                    properties["ScheduleExpression"] = "cron({})".format(new_expression)
                     if self.verbose:
-                        print('INFO: updating {}'.format(name))
+                        print("INFO: updating {}".format(name))
                     self.dirty = True
 
     def main(self, tz, date, dry_run, verbose, paths):
         self.dry_run = dry_run
         self.verbose = verbose
         self.timezone = tz
         if date:
             self.today = date
         self.update(paths)
 
 
 aws_cron_pattern = re.compile(
-    r'cron\s*\(\s*(?P<minutes>[^\s]*)\s*(?P<hours>[^\s]*)\s*(?P<day_of_month>[^\s]*)\s*(?P<month>[^\s]*)\s*(?P<day_of_week>[^\s]*)\s*(?P<year>[^\s\)]*)\)')
+    r"cron\s*\(\s*(?P<minutes>[^\s]*)\s*(?P<hours>[^\s]*)\s*(?P<day_of_month>[^\s]*)\s*(?P<month>[^\s]*)\s*(?P<day_of_week>[^\s]*)\s*(?P<year>[^\s\)]*)\)"
+)
 cron_pattern = re.compile(
-    r'\s*(?P<minutes>[^\s]*)\s*(?P<hours>[^\s]*)\s*(?P<day_of_month>[^\s]*)\s*(?P<month>[^\s]*)\s*(?P<day_of_week>[^\s]*)\s*(?P<year>[^\s\)]*)')
+    r"\s*(?P<minutes>[^\s]*)\s*(?P<hours>[^\s]*)\s*(?P<day_of_month>[^\s]*)\s*(?P<month>[^\s]*)\s*(?P<day_of_week>[^\s]*)\s*(?P<year>[^\s\)]*)"
+)
 
 
 def correct_for_utc(hour, utcoffset):
     if utcoffset.seconds % 3600 == 0:
         return int((hour + 24 - (utcoffset.seconds / 3600)) % 24)
     else:
-        raise ValueError('UTC offset is not a multiple of hours.')
+        raise ValueError("UTC offset is not a multiple of hours.")
 
 
 def correct_cron_hours_expression_for_utc(expression, utcoffset):
-    if expression == '*' or expression == '?':
+    if expression == "*" or expression == "?":
         return expression
 
-    range = re.match(r'([0-9]+)-([0-9]+)', expression)
+    range = re.match(r"([0-9]+)-([0-9]+)", expression)
     if range:
         from_hour = int(range.group(1))
         to_hour = int(range.group(2))
-        return '{}-{}'.format(correct_for_utc(from_hour, utcoffset), correct_for_utc(to_hour, utcoffset))
+        return "{}-{}".format(
+            correct_for_utc(from_hour, utcoffset), correct_for_utc(to_hour, utcoffset)
+        )
 
-    repeat = re.match(r'([0-9]+)/([0-9]+)', expression)
+    repeat = re.match(r"([0-9]+)/([0-9]+)", expression)
     if repeat:
         from_hour = int(repeat.group(1))
         repetition = int(repeat.group(2))
-        return '{}/{}'.format(correct_for_utc(from_hour, utcoffset), repetition)
+        return "{}/{}".format(correct_for_utc(from_hour, utcoffset), repetition)
 
-    hours = list(filter(lambda n: re.match(r'[0-9]+', n), expression.split(',')))
-    if len(hours) == len(expression.split(',')):
-        hours = list(map(lambda h: '{}'.format(correct_for_utc(int(h), utcoffset)), hours))
-        return ','.join(hours)
+    hours = list(filter(lambda n: re.match(r"[0-9]+", n), expression.split(",")))
+    if len(hours) == len(expression.split(",")):
+        hours = list(
+            map(lambda h: "{}".format(correct_for_utc(int(h), utcoffset)), hours)
+        )
+        return ",".join(hours)
     else:
-        assert False, 'unsupported hour format {}'.format(expression)
+        assert False, "unsupported hour format {}".format(expression)
 
     return expression
 
 
 def correct_cron_expression_for_utc(expression, today):
     match = cron_pattern.search(expression)
     assert match, '"{}" is not a cron expression'.format(expression)
 
     cron = match.groupdict()
-    tomorrow_midnight = today.tzinfo.localize(datetime(today.year, today.month, today.day) + timedelta(days=1))
+    tomorrow_midnight = today.tzinfo.localize(
+        datetime(today.year, today.month, today.day) + timedelta(days=1)
+    )
 
     try:
-        ccron = {k: ('*' if v == '?' else v) for (k, v) in cron.items()}
-        expression = '{minutes} {hours} {day_of_month} {month} {day_of_week} {year}'.format(**ccron)
+        ccron = {k: ("*" if v == "?" else v) for (k, v) in cron.items()}
+        expression = (
+            "{minutes} {hours} {day_of_month} {month} {day_of_week} {year}".format(
+                **ccron
+            )
+        )
         next_time = croniter(expression, tomorrow_midnight).get_next(datetime)
     except ValueError as e:
-        sys.stderr.write('ERROR: {}'.format(e))
+        sys.stderr.write("ERROR: {}".format(e))
         sys.exit(1)
 
     utcoffset = next_time.tzinfo.utcoffset(next_time)
     if utcoffset.seconds % 3600 == 0:
-        cron['hours'] = correct_cron_hours_expression_for_utc(cron['hours'], utcoffset)
-        expression = '{minutes} {hours} {day_of_month} {month} {day_of_week} {year}'.format(**cron)
+        cron["hours"] = correct_cron_hours_expression_for_utc(cron["hours"], utcoffset)
+        expression = (
+            "{minutes} {hours} {day_of_month} {month} {day_of_week} {year}".format(
+                **cron
+            )
+        )
     else:
         sys.stderr.write(
-            'WARN: UTC offset for "{}" in timezone "{}" is not a multiple of hours but {} seconds.\n'.format(expression,
-                                                                                                             today.tzinfo,
-                                                                                                             utcoffset.seconds))
+            'WARN: UTC offset for "{}" in timezone "{}" is not a multiple of hours but {} seconds.\n'.format(
+                expression, today.tzinfo, utcoffset.seconds
+            )
+        )
 
     return expression
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/lambda_inline_code_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/lambda_inline_code_updater.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,56 +15,64 @@
 import sys
 from .cfn_updater import CfnUpdater
 from ruamel.yaml.scalarstring import PreservedScalarString
 
 
 class LambdaInlineCodeUpdater(CfnUpdater):
     """
-    Updates the inline code of an AWS::Lambda::Function resource.
+        Updates the inline code of an AWS::Lambda::Function resource.
 
-\b
-  ELBListenerRuleProvider:
-    Type: AWS::Lambda::Function
-
-\b
-  ELBListenerRuleProvider:
-    Type: AWS::Lambda::Function
-    Properties:
-      Code:
-        ZipFile:
-          import boto3
-          import cfnresponse
-          ELB = boto3.client('elbv2')
-          ...
+    \b
+      ELBListenerRuleProvider:
+        Type: AWS::Lambda::Function
+
+    \b
+      ELBListenerRuleProvider:
+        Type: AWS::Lambda::Function
+        Properties:
+          Code:
+            ZipFile:
+              import boto3
+              import cfnresponse
+              ELB = boto3.client('elbv2')
+              ...
     """
 
     def __init__(self):
         super(LambdaInlineCodeUpdater, self).__init__()
         self._image = []
 
     def update_template(self):
         """
         updates the Code property of a AWS::Lambda::Function resource of name `self.resource` to `self.code`
         """
-        resource = self.template.get('Resources', {}).get(self.resource, None)
-        if resource and resource['Type'] == 'AWS::Lambda::Function':
-            code = resource.get('Properties', {}).get('Code', {})
-            old_code = code['ZipFile'] if 'ZipFile' in code else None
+        resource = self.template.get("Resources", {}).get(self.resource, None)
+        if resource and resource["Type"] == "AWS::Lambda::Function":
+            code = resource.get("Properties", {}).get("Code", {})
+            old_code = code["ZipFile"] if "ZipFile" in code else None
             if old_code != self.code:
                 sys.stderr.write(
-                    'INFO: updating inline code of lambda {} in {}\n'.format(self.resource, self.filename))
-                if 'Properties' not in resource:
-                    resource['Properties'] = {}
-                if 'Code' not in resource['Properties']:
-                    resource['Properties']['Code'] = {}
-                resource['Properties']['Code'] = {'ZipFile': PreservedScalarString(self.code)}
+                    "INFO: updating inline code of lambda {} in {}\n".format(
+                        self.resource, self.filename
+                    )
+                )
+                if "Properties" not in resource:
+                    resource["Properties"] = {}
+                if "Code" not in resource["Properties"]:
+                    resource["Properties"]["Code"] = {}
+                resource["Properties"]["Code"] = {
+                    "ZipFile": PreservedScalarString(self.code)
+                }
                 self.dirty = True
         elif resource:
             sys.stderr.write(
-                'WARN: resource {} in {} is not of type AWS::Lambda::Function\n'.format(self.resource, self.filename))
+                "WARN: resource {} in {} is not of type AWS::Lambda::Function\n".format(
+                    self.resource, self.filename
+                )
+            )
 
     def main(self, resource, code, paths, dry_run, verbose):
         self.resource = resource
         self.code = code
         self.dry_run = dry_run
         self.verbose = verbose
         self.update(paths)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/latest_ami_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/latest_ami_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,109 +21,109 @@
 import sys
 
 from .cfn_updater import CfnUpdater
 from .replace_references import replace_references
 
 
 def split_resource_name(resource_name):
-    m = re.match(r'^(?P<base>.*)v(?P<version>[0-9]+)$', resource_name)
+    m = re.match(r"^(?P<base>.*)v(?P<version>[0-9]+)$", resource_name)
 
     if m is not None:
-        base = m.group('base')
-        version = int(m.group('version'))
+        base = m.group("base")
+        version = int(m.group("version"))
     else:
         base = resource_name
         version = 0
 
     return base, version
 
 
 def make_new_resource_name(resource_name):
     base, version = split_resource_name(resource_name)
-    return '{}v{}'.format(base, version + 1)
+    return "{}v{}".format(base, version + 1)
 
 
 class AMIUpdater(CfnUpdater):
     """
-    Updates the AMI name of Custom::AMI resources to the latest version. 
-    With an ami-name-pattern of `amzn-ami-*ecs-optimized` it will update
-    the following resource definition from:
-
-\b
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.a-amazon-ecs-optimized
-           Owners:
-             - amazon
-
-    to:
-
-\b
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.l-amazon-ecs-optimized
-           Owners:
-             - amazon
-
-
-    By specifying --add-new-version, a new Custom::AMI will be added
-    to the template with a new name. A suffix `v<version>` is appended
-    to create the new resource. Any reference to the highest Custom::AMI version
-    resource is replaced. It will change:
-
-\b
-      CustomAMI:
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.a-amazon-ecs-optimized
-           Owners:
-             - amazon
-      CustomAMIv2:
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.b-amazon-ecs-optimized
-           Owners:
-             - amazon
-      Instance:
-         Type: AWS::EC2::Instance
-         Properties:
-            ImageId: !Ref CustomAMI
-
-    to:
-
-\b
-      CustomAMI:
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.a-amazon-ecs-optimized
-           Owners:
-             - amazon
-      CustomAMIv2:
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.b-amazon-ecs-optimized
-           Owners:
-             - amazon
-      CustomAMIv3:
-         Type: Custom::AMI
-         Properties:
-           Filters:
-             name: amzn-ami-2017.09.l-amazon-ecs-optimized
-           Owners:
-             - amazon
-      Instance:
-         Type: AWS::EC2::Instance
-         Properties:
-            ImageId: !Ref CustomAMIv3
+        Updates the AMI name of Custom::AMI resources to the latest version.
+        With an ami-name-pattern of `amzn-ami-*ecs-optimized` it will update
+        the following resource definition from:
+
+    \b
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.a-amazon-ecs-optimized
+               Owners:
+                 - amazon
+
+        to:
+
+    \b
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.l-amazon-ecs-optimized
+               Owners:
+                 - amazon
+
+
+        By specifying --add-new-version, a new Custom::AMI will be added
+        to the template with a new name. A suffix `v<version>` is appended
+        to create the new resource. Any reference to the highest Custom::AMI version
+        resource is replaced. It will change:
+
+    \b
+          CustomAMI:
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.a-amazon-ecs-optimized
+               Owners:
+                 - amazon
+          CustomAMIv2:
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.b-amazon-ecs-optimized
+               Owners:
+                 - amazon
+          Instance:
+             Type: AWS::EC2::Instance
+             Properties:
+                ImageId: !Ref CustomAMI
+
+        to:
+
+    \b
+          CustomAMI:
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.a-amazon-ecs-optimized
+               Owners:
+                 - amazon
+          CustomAMIv2:
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.b-amazon-ecs-optimized
+               Owners:
+                 - amazon
+          CustomAMIv3:
+             Type: Custom::AMI
+             Properties:
+               Filters:
+                 name: amzn-ami-2017.09.l-amazon-ecs-optimized
+               Owners:
+                 - amazon
+          Instance:
+             Type: AWS::EC2::Instance
+             Properties:
+                ImageId: !Ref CustomAMIv3
     """
 
     def __init__(self):
         super(AMIUpdater, self).__init__()
         self._ami_name_pattern = None
         self.add_new_version = False
         self.latest_ami_name_pattern = None
@@ -134,70 +134,92 @@
 
     @ami_name_pattern.setter
     def ami_name_pattern(self, name):
         self._ami_name_pattern = name
 
     @staticmethod
     def is_ami_definition(resource):
-        return resource.get('Type', '') == 'Custom::AMI'
+        return resource.get("Type", "") == "Custom::AMI"
 
     def create_describe_image_request(self, ami):
         # copy the filters values, except for name and state.
-        properties = ami.get('Properties', {})
-        filters = [{'Name': 'name', 'Values': [self.ami_name_pattern]},
-                   {'Name': 'state', 'Values': ['available']}]
-        for k, v in properties.get('Filters', {}).items():
-            if k not in ['name', 'state']:
-                filters.append({'Name': k, 'Values': v if isinstance(v, list) else [v]})
+        properties = ami.get("Properties", {})
+        filters = [
+            {"Name": "name", "Values": [self.ami_name_pattern]},
+            {"Name": "state", "Values": ["available"]},
+        ]
+        for k, v in properties.get("Filters", {}).items():
+            if k not in ["name", "state"]:
+                filters.append({"Name": k, "Values": v if isinstance(v, list) else [v]})
 
         # copy the rest of the arguments
-        result = {n: (properties.get(n) if isinstance(properties.get(n), list) else [properties.get(n)])
-                  for n in filter(lambda n: properties.get(n) is not None, ['Owners', 'ImageIds', 'ExecutableUsers'])}
-        result['Filters'] = filters
+        result = {
+            n: (
+                properties.get(n)
+                if isinstance(properties.get(n), list)
+                else [properties.get(n)]
+            )
+            for n in filter(
+                lambda n: properties.get(n) is not None,
+                ["Owners", "ImageIds", "ExecutableUsers"],
+            )
+        }
+        result["Filters"] = filters
         return result
 
     def _describe_images(self, **kwargs):
-        return boto3.client('ec2').describe_images(**kwargs)
+        return boto3.client("ec2").describe_images(**kwargs)
 
     def load_latest_ami_name_pattern(self, resource):
         response = self._describe_images(**self.create_describe_image_request(resource))
 
-        images = sorted(response['Images'], key=lambda i: i['CreationDate'])
-        self.latest_ami_name_pattern = images[-1]['Name'] if len(images) > 0 else None
+        images = sorted(response["Images"], key=lambda i: i["CreationDate"])
+        self.latest_ami_name_pattern = images[-1]["Name"] if len(images) > 0 else None
         if len(images) > 0:
             sys.stderr.write(
-                'INFO: using {} matching {}, created on {}\n'.format(self.latest_ami_name_pattern,
-                                                                     self.ami_name_pattern,
-                                                                     images[-1]['CreationDate']))
+                "INFO: using {} matching {}, created on {}\n".format(
+                    self.latest_ami_name_pattern,
+                    self.ami_name_pattern,
+                    images[-1]["CreationDate"],
+                )
+            )
 
     def is_ami_name_pattern_match(self, name):
         regex = re.compile(fnmatch.translate(self.ami_name_pattern))
         return regex.match(name)
 
     def all_custom_ami_resources(self):
         r = self.resources
-        return filter(lambda n: self.is_ami_definition(r[n]) and self.is_name_filter_match(r[n]), r)
+        return filter(
+            lambda n: self.is_ami_definition(r[n]) and self.is_name_filter_match(r[n]),
+            r,
+        )
 
     def is_name_filter_match(self, ami):
-        if 'Properties' in ami and 'Filters' in ami['Properties'] and 'name' in ami['Properties']['Filters']:
-            return self.is_ami_name_pattern_match(ami['Properties']['Filters']['name'])
+        if (
+            "Properties" in ami
+            and "Filters" in ami["Properties"]
+            and "name" in ami["Properties"]["Filters"]
+        ):
+            return self.is_ami_name_pattern_match(ami["Properties"]["Filters"]["name"])
         return False
 
     def custom_ami_resources_partitions(self):
         partitions = {}
         ami_resources = self.all_custom_ami_resources()
         for resource_name in ami_resources:
             base, _ = split_resource_name(resource_name)
             if base not in partitions:
                 partitions[base] = {}
             partitions[base][resource_name] = self.resources[resource_name]
 
-
         for base in partitions:
-            resource_names = sorted(partitions[base].keys(), key=lambda n: split_resource_name(n)[1])
+            resource_names = sorted(
+                partitions[base].keys(), key=lambda n: split_resource_name(n)[1]
+            )
             yield OrderedDict({name: partitions[base][name] for name in resource_names})
 
     @staticmethod
     def latest_custom_ami_resource(ami_resources):
         result = None
         highest_version = -1
         for resource_name in ami_resources:
@@ -205,29 +227,36 @@
             if version > highest_version:
                 result = resource_name
                 highest_version = version
 
         return result
 
     def ami_requires_update(self, ami):
-        name = ami['Properties']['Filters']['name']
-        return self.latest_ami_name_pattern is not None and name != self.latest_ami_name_pattern
+        name = ami["Properties"]["Filters"]["name"]
+        return (
+            self.latest_ami_name_pattern is not None
+            and name != self.latest_ami_name_pattern
+        )
 
     def update_ami(self, resource_name, ami):
         if self.ami_requires_update(ami):
-            ami['Properties']['Filters']['name'] = self.latest_ami_name_pattern
+            ami["Properties"]["Filters"]["name"] = self.latest_ami_name_pattern
             sys.stderr.write(
                 'INFO: updating AMI definition "{}" name filter to {} in {}\n'.format(
-                    resource_name, self.latest_ami_name_pattern, self.filename))
+                    resource_name, self.latest_ami_name_pattern, self.filename
+                )
+            )
             self.dirty = True
         else:
             if self.verbose:
                 sys.stderr.write(
                     'INFO: AMI definition "{}" name already up to date in {}\n'.format(
-                        resource_name, self.filename))
+                        resource_name, self.filename
+                    )
+                )
 
     def update_inplace(self):
         """
         updates the name filter of AMI resource definitions in `self.template`.
         """
         for resource_name in self.all_custom_ami_resources():
             ami = self.resources[resource_name]
@@ -244,15 +273,17 @@
                 ami = copy.deepcopy(self.resources[resource_name])
                 self.load_latest_ami_name_pattern(ami)
                 if self.ami_requires_update(ami):
                     new_resource_name = make_new_resource_name(resource_name)
                     self.resources[new_resource_name] = ami
                     self.update_ami(new_resource_name, ami)
                     for old_resource_name in reversed(ami_resources):
-                        if replace_references(self.template, old_resource_name, new_resource_name):
+                        if replace_references(
+                            self.template, old_resource_name, new_resource_name
+                        ):
                             break
 
     def update_template(self):
         if self.add_new_version:
             self.add_new_ami_resource()
         else:
             self.update_inplace()
@@ -260,11 +291,15 @@
     def main(self, ami_name_pattern, dry_run, verbose, add_new_version, path):
         self.dry_run = dry_run
         self.verbose = verbose
         self.ami_name_pattern = ami_name_pattern
         self.add_new_version = add_new_version
         self.load_latest_ami_name_pattern({})
         if self.latest_ami_name_pattern is None:
-            sys.stderr.write('ERROR: image name {} does not resolve to an active AMI \n'.format(self.ami_name_pattern))
+            sys.stderr.write(
+                "ERROR: image name {} does not resolve to an active AMI \n".format(
+                    self.ami_name_pattern
+                )
+            )
             sys.exit(1)
 
         self.update(path)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/oidc_provider_thumbprints_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/oidc_provider_thumbprints_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,17 @@
     def update_thumbprints(self, name, provider):
 
         url = provider.get("Properties", {}).get("Url")
         public_key = self.get_public_key(url)
         sha1 = public_key.fingerprint(hashes.SHA1())
         fingerprint = binascii.hexlify(sha1).decode("ascii").lower()
 
-        thumbprints = provider.get("Properties", {}).get("ThumbprintList", CommentedSeq())
+        thumbprints = provider.get("Properties", {}).get(
+            "ThumbprintList", CommentedSeq()
+        )
         exists = list(filter(lambda f: f.lower() == fingerprint, thumbprints))
         if exists:
             if self.verbose:
                 sys.stderr.write(
                     f"INFO: fingerprint of {url} for OIDC provider {name} already in thumbprint list\n"
                 )
             return
@@ -143,23 +145,24 @@
             )
 
         sys.stderr.write(
             f"INFO: updating fingerprint of {url}, for OIDC provider {name} to {fingerprint}, valid until {public_key.not_valid_after}\n"
         )
         self.dirty = True
 
-
         if not isinstance(thumbprints, CommentedSeq):
             new_thumbprints = CommentedSeq()
             if self.append:
                 new_thumbprints.extend(thumbprints)
             thumbprints = new_thumbprints
 
         thumbprints.append(fingerprint)
-        thumbprints.yaml_add_eol_comment(f"valid until {public_key.not_valid_after}", len(thumbprints)-1)
+        thumbprints.yaml_add_eol_comment(
+            f"valid until {public_key.not_valid_after}", len(thumbprints) - 1
+        )
         provider["Properties"]["ThumbprintList"] = thumbprints
 
 
 @click.command(
     name="oidc-provider-thumbprints", help=OIDCProviderThumbprintsUpdater.__doc__
 )
 @click.option("--url", required=False, type=str, help="of the OIDC provider to update")
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/packer_ami_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/packer_ami_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 import boto3
 import click
 import sys
 
 
 class PackerAMIUpdater(object):
     """
-    Updates a packer.json source_ami_filter to the latest AMI version.
-    With an ami-name-pattern of `Windows_Server-2016-English-Full-Base-*` it will
-    update the following from:
-\b
-      "source_ami_filter": {
-        "filters": {
-          "virtualization-type": "hvm",
-          "name": ""Windows_Server-2016-English-Full-Base-2020.01.15",
-          "root-device-type": "ebs"
-        },
-        "owners": [ "801119661308" ],
-      },
-\b
-    to:
-\b
-      "source_ami_filter": {
-        "filters": {
-          "virtualization-type": "hvm",
-          "name": "Windows_Server-2016-English-Full-Base-2020.02.12",
-          "root-device-type": "ebs"l
-        },
-        "owners": [ "801119661308" ],
-      },
+        Updates a packer.json source_ami_filter to the latest AMI version.
+        With an ami-name-pattern of `Windows_Server-2016-English-Full-Base-*` it will
+        update the following from:
+    \b
+          "source_ami_filter": {
+            "filters": {
+              "virtualization-type": "hvm",
+              "name": ""Windows_Server-2016-English-Full-Base-2020.01.15",
+              "root-device-type": "ebs"
+            },
+            "owners": [ "801119661308" ],
+          },
+    \b
+        to:
+    \b
+          "source_ami_filter": {
+            "filters": {
+              "virtualization-type": "hvm",
+              "name": "Windows_Server-2016-English-Full-Base-2020.02.12",
+              "root-device-type": "ebs"l
+            },
+            "owners": [ "801119661308" ],
+          },
     """
 
     def __init__(self):
         self.packer: dict = None
         self.filename: str = None
         self.dirty: bool = False
         self.verbose: bool = False
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/remove_resource.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/remove_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,147 +21,144 @@
 from typing import List
 from ruamel.yaml.comments import TaggedScalar, CommentedSeq
 
 from .cfn_updater import CfnUpdater
 
 import logging
 
+
 def is_reference(obj, fld, name):
     if isinstance(obj, dict):
         if fld == "Ref":
             return obj["Ref"] == name
         elif fld == "FN::GetAtt":
             return len(obj[fld]) > 0 and obj[fld][0] == name
         elif fld == "FN::Sub":
             return isinstance(obj[fld], str) and references_in_sub(obj[fld], name)
 
+
 def references_in_sub(sub, name):
-    return list(filter(lambda n : n == name, map(lambda n: n.split('.')[0], re.findall(r'\${([^!][^}]*)}', sub))))
+    return list(
+        filter(
+            lambda n: n == name,
+            map(lambda n: n.split(".")[0], re.findall(r"\${([^!][^}]*)}", sub)),
+        )
+    )
+
 
 def is_tag_reference(obj, name):
     if isinstance(obj, TaggedScalar):
-        if obj.tag.value == '!Ref':
+        if obj.tag.value == "!Ref":
             return str(obj.value) == name
-        elif obj.tag.value == '!Sub':
+        elif obj.tag.value == "!Sub":
             return references_in_sub(obj.value, name)
-        elif obj.tag.value == '!GetAtt':
-            return str(obj.value).split('.')[0] == name
+        elif obj.tag.value == "!GetAtt":
+            return str(obj.value).split(".")[0] == name
     elif isinstance(obj, CommentedSeq):
-        if obj.tag.value == '!GetAtt':
+        if obj.tag.value == "!GetAtt":
             return len(obj) > 1 and obj[0] == name
     return False
 
-def remove_resource_from_template(template:dict, name:str):
-    resources:dict = template.get("Resources")
+
+def remove_resource_from_template(template: dict, name: str):
+    resources: dict = template.get("Resources")
     if resources and name in resources:
         resources.pop(name)
         remove_all_references(template, name)
         return True
-    outputs:dict = template.get("Resources")
+    outputs: dict = template.get("Resources")
     if outputs and name in outputs:
         remove_all_references(template, name)
         return True
     return False
 
     return False
 
+
 def remove_all_references(template, name):
     to_remove = {}
     for toplevel in template:
         if isinstance(template[toplevel], dict):
             to_remove[toplevel] = []
 
     for toplevel in to_remove:
         for obj in template[toplevel]:
-            if has_reference(
-                    template[toplevel][obj], name, []
-            ):
+            if has_reference(template[toplevel][obj], name, []):
                 to_remove[toplevel].append(obj)
     for toplevel in to_remove:
         for obj in to_remove[toplevel]:
             logging.info(
-                "Removing object %s from %s, as it references %s",
-                obj, toplevel, name
+                "Removing object %s from %s, as it references %s", obj, toplevel, name
             )
             template[toplevel].pop(obj)
 
+
 def has_reference(obj, name, path):
     result = False
     if isinstance(obj, dict):
         for fld in obj:
             if is_reference(obj, fld, name):
-                logging.info(
-                    "INFO: %s to %s found in %s",
-                    fld, name, ".".join(path)
-                )
+                logging.info("INFO: %s to %s found in %s", fld, name, ".".join(path))
                 result = True
             else:
                 nested_path = path[:]
                 nested_path.append(fld)
-                result = result or has_reference(
-                    obj[fld], name, nested_path
-                )
+                result = result or has_reference(obj[fld], name, nested_path)
     elif isinstance(obj, TaggedScalar):
         if is_tag_reference(obj, name):
-            logging.info(
-                "INFO: %s to %s found in %s",
-                obj.tag, name, ".".join(path)
-            )
+            logging.info("INFO: %s to %s found in %s", obj.tag, name, ".".join(path))
             result = True
 
     elif isinstance(obj, CommentedSeq):
         if is_tag_reference(obj, name):
-            logging.info(
-                "INFO: %s to %s found in %s",
-                obj.tag, name, ".".join(path)
-            )
+            logging.info("INFO: %s to %s found in %s", obj.tag, name, ".".join(path))
             result = True
         else:
             for i in range(len(obj)):
                 nested_path = path[:]
                 nested_path.append("[%d]" % i)
                 if has_reference(obj[i], name, nested_path):
                     logging.info(
                         "INFO: %s too %s found in array %s",
-                        obj[i], name, ".".join(nested_path)
+                        obj[i],
+                        name,
+                        ".".join(nested_path),
                     )
                     result = True
 
     elif isinstance(obj, list):
         for i in range(len(obj)):
             nested_path = path[:]
             nested_path.append("[%d]" % i)
             if has_reference(obj[i], name, nested_path):
                 logging.info(
-                    "INFO: Ref:%s found in array %s",
-                    name, ".".join(nested_path)
+                    "INFO: Ref:%s found in array %s", name, ".".join(nested_path)
                 )
                 result = True
 
     return result
 
 
-
 class ResourceRemover(CfnUpdater):
     """
     Removes the specified CloudFormation resource and all resources that reference it.
     """
 
     def __init__(self):
         super(ResourceRemover, self).__init__()
         self.resource_name = None
 
     def update_template(self):
         if remove_resource_from_template(self.template, self.resource_name):
             self.dirty = True
 
 
-@click.command(name='remove-resource', help=ResourceRemover.__doc__)
-@click.option('--resource', required=True, help='to remove from the template')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+@click.command(name="remove-resource", help=ResourceRemover.__doc__)
+@click.option("--resource", required=True, help="to remove from the template")
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def remove_resource(ctx, resource, path):
     updater = ResourceRemover()
-    updater.dry_run = ctx.obj['dry_run']
-    updater.verbose = ctx.obj['verbose']
+    updater.dry_run = ctx.obj["dry_run"]
+    updater.verbose = ctx.obj["verbose"]
     updater.resource_name = resource
     updater.update(path)
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/replace_references.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/replace_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,27 @@
     """
     replaces CloudFormation references { "Ref": old_reference } with { "Ref": new_reference } in `template`.
     returns True if one or more references where made.
     """
     result = False
     if isinstance(template, dict):
         for name, value in template.items():
-            if name == 'Ref' and value == old_reference:
-                template['Ref'] = new_reference
+            if name == "Ref" and value == old_reference:
+                template["Ref"] = new_reference
                 result = True
-            elif isinstance(value, TaggedScalar) and value.tag and value.tag.value == '!Ref' and value.value == old_reference:
+            elif (
+                isinstance(value, TaggedScalar)
+                and value.tag
+                and value.tag.value == "!Ref"
+                and value.value == old_reference
+            ):
                 value.value = new_reference
                 result = True
             else:
-                result = replace_references(template[name], old_reference, new_reference) or result
+                result = (
+                    replace_references(template[name], old_reference, new_reference)
+                    or result
+                )
     elif isinstance(template, list):
         for i, value in enumerate(template):
             result = replace_references(value, old_reference, new_reference) or result
     return result
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/rest_api_body_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/rest_api_body_updater.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,57 +55,67 @@
         self.verbose = False
         self.dry_run = False
         self.keep = 1
         self.yaml = YAML()
         self._body = {}
 
     def load_and_merge_swagger_body(self):
-        with open(self.open_api_specification, 'r') as f:
+        with open(self.open_api_specification, "r") as f:
             body = self.yaml.load(f)
-        with open(self.api_gateway_extensions, 'r') as f:
+        with open(self.api_gateway_extensions, "r") as f:
             extensions = self.yaml.load(f)
 
         self.body = jsonmerge.merge(body, extensions)
 
     @property
     def body(self):
         return self._body
 
     @body.setter
     def body(self, body):
         self._body = body
-        self.body_as_string = self.yaml_dump_to_str(self.body) if body else ''
+        self.body_as_string = self.yaml_dump_to_str(self.body) if body else ""
 
     def yaml_dump_to_str(self, dict):
         s = StringIO()
         self.yaml.dump(dict, s)
         return s.getvalue()
 
     def resource_name_pattern(self):
-        return re.compile('^(?P<basename>{})(v(?P<version>[0-9]+))?$'.format(self.resource_name))
+        return re.compile(
+            "^(?P<basename>{})(v(?P<version>[0-9]+))?$".format(self.resource_name)
+        )
 
     def find_matching_resources(self):
         """
         find all resources matching the pattern `<resource_name>v[0-9]+`, sort listed
         """
         pattern = self.resource_name_pattern()
 
         result = []
-        resources = self.template['Resources'] if 'Resources' in self.template else None
+        resources = self.template["Resources"] if "Resources" in self.template else None
         if resources:
-            result = list(filter(lambda name: 'Type' in resources[name] and resources[name][
-                'Type'] == 'AWS::ApiGateway::RestApi', filter(lambda name: pattern.match(name), resources)))
+            result = list(
+                filter(
+                    lambda name: "Type" in resources[name]
+                    and resources[name]["Type"] == "AWS::ApiGateway::RestApi",
+                    filter(lambda name: pattern.match(name), resources),
+                )
+            )
             result.sort(
-                key=lambda n: int(pattern.match(n).group('version')) if pattern.match(n).group('version') else -1)
+                key=lambda n: int(pattern.match(n).group("version"))
+                if pattern.match(n).group("version")
+                else -1
+            )
         return result
 
     def new_resource_name(self, name):
         match = self.resource_name_pattern().match(name)
-        version = int(match.group('version')) if match.group('version') else 0
-        return '{}v{}'.format(match.group('basename'), version + 1)
+        version = int(match.group("version")) if match.group("version") else 0
+        return "{}v{}".format(match.group("basename"), version + 1)
 
     def copy_resource(self, resource):
         """
         Copy the resource using dump and reload. dictionary deepcopy() did not work on yaml dictionaries.
         """
         bytes = BytesIO()
         self.yaml.dump(resource, bytes)
@@ -115,55 +125,80 @@
 
     def update_template(self):
         resources = self.find_matching_resources()
         if not resources:
             return
 
         name = resources[-1]
-        rest_api_gateway = self.template['Resources'][name]
-        current_body = rest_api_gateway.get('Properties', {}).get('Body', {})
+        rest_api_gateway = self.template["Resources"][name]
+        current_body = rest_api_gateway.get("Properties", {}).get("Body", {})
 
-        current_body_as_string = self.yaml_dump_to_str(current_body) if current_body else ''
+        current_body_as_string = (
+            self.yaml_dump_to_str(current_body) if current_body else ""
+        )
         if self.body_as_string != current_body_as_string:
 
             if self.verbose:
-                for text in difflib.unified_diff(current_body_as_string.split("\n"), self.body_as_string.split("\n")):
-                    if text[:3] not in ['---', '+++']:
-                        sys.stderr.write('{}\n'.format(text))
+                for text in difflib.unified_diff(
+                    current_body_as_string.split("\n"), self.body_as_string.split("\n")
+                ):
+                    if text[:3] not in ["---", "+++"]:
+                        sys.stderr.write("{}\n".format(text))
 
             rest_api_gateway = self.copy_resource(rest_api_gateway)
-            if not 'Properties' in rest_api_gateway:
-                rest_api_gateway['Properties'] = {}
+            if not "Properties" in rest_api_gateway:
+                rest_api_gateway["Properties"] = {}
 
-            rest_api_gateway['Properties']['Body'] = self.body
+            rest_api_gateway["Properties"]["Body"] = self.body
 
             if self.add_new_version:
                 new_name = self.new_resource_name(name)
                 sys.stderr.write(
-                    'INFO: adding resource {} with new swagger body in template {}\n'.format(new_name, self.filename))
+                    "INFO: adding resource {} with new swagger body in template {}\n".format(
+                        new_name, self.filename
+                    )
+                )
             else:
                 new_name = name
                 sys.stderr.write(
-                    'INFO: updating resource {} with swagger body in template {}\n'.format(new_name, self.filename))
+                    "INFO: updating resource {} with swagger body in template {}\n".format(
+                        new_name, self.filename
+                    )
+                )
 
             if self.add_new_version:
                 replace_references(self.template, name, new_name)
                 for i in range(0, len(resources) - (self.keep - 1)):
                     sys.stderr.write(
-                        'INFO: removing resource {} from template {}\n'.format(resources[i], self.filename))
-                    del self.template['Resources'][resources[i]]
-            self.template['Resources'][new_name] = rest_api_gateway
+                        "INFO: removing resource {} from template {}\n".format(
+                            resources[i], self.filename
+                        )
+                    )
+                    del self.template["Resources"][resources[i]]
+            self.template["Resources"][new_name] = rest_api_gateway
 
             self.dirty = True
         else:
             sys.stderr.write(
-                'INFO: no changes of swagger body of {} in template {}\n'.format(self.resource_name, self.filename))
-
-    def main(self, resource_name, open_api_specification, api_gateway_extensions, path, add_new_version, keep, dry_run,
-             verbose):
+                "INFO: no changes of swagger body of {} in template {}\n".format(
+                    self.resource_name, self.filename
+                )
+            )
+
+    def main(
+        self,
+        resource_name,
+        open_api_specification,
+        api_gateway_extensions,
+        path,
+        add_new_version,
+        keep,
+        dry_run,
+        verbose,
+    ):
         self.dry_run = dry_run
         self.verbose = verbose
         self.resource_name = resource_name
         self.open_api_specification = open_api_specification
         self.api_gateway_extensions = api_gateway_extensions
         self.add_new_version = add_new_version
         self.keep = keep if keep > 0 else 1
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update/statemachine_updater.py` & `aws-cfn-update-0.8.4/src/aws_cfn_update/statemachine_updater.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,73 +27,107 @@
     The definition is read from the file specified by --definition.
     By default, the content will be passed into the Fn::Sub function to
     allow references to parameters and resource attributes in the template.
 
     If you do not want substitution for your definition, specify --no-fn-sub.
 
     """
+
     def __init__(self):
         super(StateMachineDefinitionUpdater, self).__init__()
         self.resource_name = None
         self._definition = None
         self.definition_file = None
         self.template = None
         self.with_fn_sub = True
         self.verbose = False
         self.dry_run = False
 
     def new_value(self, definition):
         if self.with_fn_sub:
-            return isinstance(definition, dict) and definition.get('Fn::Sub') == self.definition, {'Fn::Sub': self.definition}
+            return isinstance(definition, dict) and definition.get(
+                "Fn::Sub"
+            ) == self.definition, {"Fn::Sub": self.definition}
         else:
             return definition == self.definition, self.definition
 
     def update_template(self):
         """
         updates the Definition of Step Function StateMachine.
         """
-        resources = self.template.get('Resources', {})
-        for name, resource in map(lambda n: (n, resources[n]), filter(lambda n: n == self.resource_name, resources)):
-            if 'Properties' not in resource:
-                resource['Properties'] = {}
-
-            same, new_definition = self.new_value(resource['Properties'].get('DefinitionString'))
+        resources = self.template.get("Resources", {})
+        for name, resource in map(
+            lambda n: (n, resources[n]),
+            filter(lambda n: n == self.resource_name, resources),
+        ):
+            if "Properties" not in resource:
+                resource["Properties"] = {}
+
+            same, new_definition = self.new_value(
+                resource["Properties"].get("DefinitionString")
+            )
             if not same:
-                sys.stderr.write('INFO: updating definition of state machine {}\n'.format(self.resource_name))
-                resource['Properties']['DefinitionString'] = new_definition
+                sys.stderr.write(
+                    "INFO: updating definition of state machine {}\n".format(
+                        self.resource_name
+                    )
+                )
+                resource["Properties"]["DefinitionString"] = new_definition
                 self.dirty = True
             else:
                 if self.verbose:
                     sys.stderr.write(
-                        'INFO: no changes to definition of state machine {}\n'.format(self.resource_name))
+                        "INFO: no changes to definition of state machine {}\n".format(
+                            self.resource_name
+                        )
+                    )
 
     @property
     def definition(self):
         return self._definition
 
     @definition.setter
     def definition(self, definition):
-        self._definition = LiteralScalarString(definition) if not isinstance(definition, LiteralScalarString) else definition
+        self._definition = (
+            LiteralScalarString(definition)
+            if not isinstance(definition, LiteralScalarString)
+            else definition
+        )
 
     def read_definition(self, filename):
         self.definition_file = filename
-        with open(self.definition_file, 'r') as f:
+        with open(self.definition_file, "r") as f:
             self.definition = LiteralScalarString(f.read())
 
     def main(self, resource_name, definition_file, with_fn_sub, path, dry_run, verbose):
         self.dry_run = dry_run
         self.verbose = verbose
         self.resource_name = resource_name
         self.with_fn_sub = with_fn_sub
         self.read_definition(definition_file)
         self.update(path)
 
 
-@click.command(name='state-machine-definition', help=StateMachineDefinitionUpdater.__doc__)
-@click.option('--resource', required=True, help='AWS::StepFunctions::StateMachine definition to update')
-@click.option('--definition', required=True, type=click.Path(exists=True), help='of the state machine')
-@click.option('--fn-sub/--no-fn-sub', required=False, default=True, help='for the definition')
-@click.argument('path', nargs=-1, required=True, type=click.Path(exists=True))
+@click.command(
+    name="state-machine-definition", help=StateMachineDefinitionUpdater.__doc__
+)
+@click.option(
+    "--resource",
+    required=True,
+    help="AWS::StepFunctions::StateMachine definition to update",
+)
+@click.option(
+    "--definition",
+    required=True,
+    type=click.Path(exists=True),
+    help="of the state machine",
+)
+@click.option(
+    "--fn-sub/--no-fn-sub", required=False, default=True, help="for the definition"
+)
+@click.argument("path", nargs=-1, required=True, type=click.Path(exists=True))
 @click.pass_context
 def update_state_machine_definition(ctx, resource, definition, fn_sub, path):
     updater = StateMachineDefinitionUpdater()
-    updater.main(resource, definition, fn_sub, list(path), ctx.obj['dry_run'], ctx.obj['verbose'])
+    updater.main(
+        resource, definition, fn_sub, list(path), ctx.obj["dry_run"], ctx.obj["verbose"]
+    )
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/PKG-INFO` & `aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.3
+Version: 0.8.4
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.3/src/aws_cfn_update.egg-info/SOURCES.txt` & `aws-cfn-update-0.8.4/src/aws_cfn_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/api-specification.yaml` & `aws-cfn-update-0.8.4/tests/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/aws-extensions.yaml` & `aws-cfn-update-0.8.4/tests/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/dummy_responses.json` & `aws-cfn-update-0.8.4/tests/dummy_responses.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_add_new_resources.py` & `aws-cfn-update-0.8.4/tests/test_add_new_resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from aws_cfn_update.rest_api_body_updater import RestAPIBodyUpdater
 import json
 
 from aws_cfn_update.add_missing_resources import add_missing_resources
-from aws_cfn_update.cfn_updater import yaml
+from aws_cfn_update.cfn_updater import CfnUpdater
 
 
 def test_simple():
     source = {"Resources": {"AMI": {}, "EC2Instance": {"ImageId": {"Ref": "AMI"}}}}
     target = {"Resources": {"AMI": {}}}
     result = add_missing_resources(target, source)
     assert result
```

### Comparing `aws-cfn-update-0.8.3/tests/test_config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.4/tests/test_config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_cron_schedule_expression.py` & `aws-cfn-update-0.8.4/tests/test_cron_schedule_expression.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_lambda_inline_code_updater.py` & `aws-cfn-update-0.8.4/tests/test_lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_latest_ami_updater.py` & `aws-cfn-update-0.8.4/tests/test_latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_oidc_provider_thumbprint_updater.py` & `aws-cfn-update-0.8.4/tests/test_oidc_provider_thumbprint_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_packer_ami_updater.py` & `aws-cfn-update-0.8.4/tests/test_packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_remove_resources.py` & `aws-cfn-update-0.8.4/tests/test_remove_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from aws_cfn_update.remove_resource import remove_resource_from_template
-from aws_cfn_update.cfn_updater import yaml
+from aws_cfn_update.cfn_updater import CfnUpdater
 from io import StringIO
+from ruamel.yaml import YAML
 
 
 def test_simple():
     template = {"Resources": {"AMI": {}}}
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
 
@@ -41,27 +42,29 @@
     }
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
     assert template.get("AMI") is None
 
 
 def test_yaml():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: !Ref Old
 """
     )
 
     assert template.get("Resources", {}).get("AMI")
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
 
 
 def test_yaml_simple_ref():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !Ref AMI
@@ -77,14 +80,15 @@
     assert resources.get("AMI") is None
     assert resources.get("EC2Instance") is None
     outputs = template.get("Outputs")
     assert outputs.get("Arn") is None
 
 
 def test_yaml_simple_getatt():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !GetAtt
@@ -96,14 +100,15 @@
     assert template.get("Resources", {}).get("AMI")
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
     assert template.get("Resources", {}).get("EC2Instance") is None
 
 
 def test_yaml_nested_ref():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !GetAtt
@@ -115,14 +120,15 @@
     assert template.get("Resources", {}).get("AMI")
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
     assert template.get("Resources", {}).get("EC2Instance") is None
 
 
 def test_yaml_ref_in_sub():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !Sub '${AMI}'
@@ -132,14 +138,15 @@
     assert template.get("Resources", {}).get("AMI")
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
     assert template.get("Resources", {}).get("EC2Instance") is None
 
 
 def test_yaml_no_ref_in_sub():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !Sub '${!AMI}'
@@ -149,14 +156,15 @@
     assert template.get("Resources", {}).get("AMI")
     remove_resource_from_template(template, "AMI")
     assert template.get("Resources", {}).get("AMI") is None
     assert template.get("Resources", {}).get("EC2Instance")
 
 
 def test_yaml_ref_in_sub_array_style():
+    yaml = CfnUpdater().yaml
     template = yaml.load(
         """
 Resources:
   AMI: 
     Type: Custom::AMI
   EC2Instance:
     ImageId: !Sub
```

### Comparing `aws-cfn-update-0.8.3/tests/test_replace_references.py` & `aws-cfn-update-0.8.4/tests/test_replace_references.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from aws_cfn_update.replace_references import replace_references
-from aws_cfn_update.cfn_updater import yaml
+from aws_cfn_update.cfn_updater import CfnUpdater
 from io import StringIO
 
 
 def test_simple():
     template = {"Ref": "Old"}
     assert replace_references(template, "Old", "New")
     assert template["Ref"] == "New"
@@ -18,13 +18,14 @@
 
     template = {"DependsOn": [{"Ref": "Old"}]}
     assert not replace_references(template, "Oud", "New")
     assert template["DependsOn"][0]["Ref"] == "Old"
 
 
 def test_yaml():
-    template = yaml.load("AMI: !Ref Old")
+    yaml = CfnUpdater().yaml
+    template = yaml.load("---\nAMI: !Ref Old")
     assert replace_references(template, "Old", "New")
 
     result = StringIO()
     yaml.dump(template, result)
-    assert result.getvalue() == "AMI: !Ref New\n"
+    assert result.getvalue() == "---\nAMI: !Ref New\n"
```

### Comparing `aws-cfn-update-0.8.3/tests/test_rest_api_body_updater.py` & `aws-cfn-update-0.8.4/tests/test_rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/test_statemachine_definition_updater.py` & `aws-cfn-update-0.8.4/tests/test_statemachine_definition_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/update_packer/base.py` & `aws-cfn-update-0.8.4/tests/update_packer/base.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/update_packer/call_00001_describe_images/__init__.py` & `aws-cfn-update-0.8.4/tests/update_packer/call_00001_describe_images/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.3/tests/update_packer/test_update_packer.py` & `aws-cfn-update-0.8.4/tests/update_packer/test_update_packer.py`

 * *Files identical despite different names*

