# Comparing `tmp/python-heatclient-3.2.0.tar.gz` & `tmp/python-heatclient-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-heatclient-3.2.0.tar", last modified: Fri Feb 24 09:40:58 2023, max compression
+gzip compressed data, was "python-heatclient-3.3.0.tar", last modified: Wed May 17 11:16:22 2023, max compression
```

## Comparing `python-heatclient-3.2.0.tar` & `python-heatclient-3.3.0.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7311 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38305 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/cli/orchestration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/cli/software_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/cli/software_deployment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2801 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/cli/stack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8239 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/contributor/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/source/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/ext/gen_ref.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/doc/source/man/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/doc/source/man/heat.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.855065 python-heatclient-3.2.0/heatclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17200 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/deployment_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/environment_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/event_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/format_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3016 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/hook_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14042 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/resource_formatter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/template_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14980 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/template_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13872 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/build_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8469 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10076 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4686 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8024 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7453 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/software_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13006 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/software_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49806 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/stack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/stack_failures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6060 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/osc/v1/template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26084 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4451 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5073 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/test_readonly.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/test_stack.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/functional/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/templates/heat_minimal.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/templates/heat_minimal_hot.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3950 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/functional/test_readonly_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/inline_templates.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.859065 python-heatclient-3.2.0/heatclient/tests/test_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/test_templates/adopt.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/test_templates/adopt_with_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/test_templates/empty.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/test_templates/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.863065 python-heatclient-3.2.0/heatclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.863065 python-heatclient-3.2.0/heatclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_build_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9927 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13765 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7594 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7045 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_software_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17416 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_software_deployment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59387 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_stack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8973 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_stack_failures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_build_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32955 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_common_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13119 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_deployment_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_environment_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15769 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_event_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6259 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5300 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_format_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_openstack_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_resource_formatter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4170 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7303 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   155469 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4301 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_software_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6770 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_software_deployments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12787 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_stacks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_template_format.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42021 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_template_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_template_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18854 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/heatclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13280 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/v1/test_hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/heatclient/tests/unit/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/var/adopt_stack_data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9443 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/var/dot_test.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/var/environment.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/tests/unit/var/minimal.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/heatclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/build_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3036 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5186 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71764 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/software_configs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/software_deployments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/stacks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/heatclient/v1/template_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/python_heatclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5581 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4000 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-02-24 09:40:58.000000 python-heatclient-3.2.0/python_heatclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.851065 python-heatclient-3.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.867065 python-heatclient-3.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/notes/add-converge-in-osc-stack-update-10f256589f628d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/notes/add-files-container-stack-create-update-324b931f8f474b3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/notes/bug-1643492-2d7537b55f347722.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.851065 python-heatclient-3.2.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.851065 python-heatclient-3.2.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5338 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-24 09:40:58.871065 python-heatclient-3.2.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/tools/heat.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2023-02-24 09:40:34.000000 python-heatclient-3.2.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.787010 python-heatclient-3.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7311 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38456 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2023-05-17 11:16:22.787010 python-heatclient-3.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/cli/orchestration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/cli/software_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/cli/software_deployment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2801 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/cli/stack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8239 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2009 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/contributor/contributing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/source/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/ext/gen_ref.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.755006 python-heatclient-3.3.0/doc/source/man/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/doc/source/man/heat.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.759007 python-heatclient-3.3.0/heatclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.759007 python-heatclient-3.3.0/heatclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17200 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/deployment_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/environment_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10504 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/event_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2689 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/format_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3016 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/hook_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14042 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/resource_formatter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/template_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14980 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/template_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13872 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4674 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.759007 python-heatclient-3.3.0/heatclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.763007 python-heatclient-3.3.0/heatclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/build_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8469 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10076 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4686 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1385 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8024 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7453 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/software_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13006 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/software_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49806 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/stack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/stack_failures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6060 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/osc/v1/template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26084 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.763007 python-heatclient-3.3.0/heatclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.763007 python-heatclient-3.3.0/heatclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.767008 python-heatclient-3.3.0/heatclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.767008 python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4451 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5073 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/test_readonly.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/test_stack.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.767008 python-heatclient-3.3.0/heatclient/tests/functional/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/templates/heat_minimal.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/templates/heat_minimal_hot.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3950 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/functional/test_readonly_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/inline_templates.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.767008 python-heatclient-3.3.0/heatclient/tests/test_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/test_templates/adopt.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/test_templates/adopt_with_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       34 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/test_templates/empty.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/test_templates/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.775009 python-heatclient-3.3.0/heatclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.775009 python-heatclient-3.3.0/heatclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1291 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.779009 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_build_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9927 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13765 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7594 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7045 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_software_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17416 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_software_deployment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59387 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_stack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8973 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_stack_failures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_build_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32955 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_common_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13119 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_deployment_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3302 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_environment_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15769 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_event_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6259 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5300 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_format_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_openstack_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3128 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_resource_formatter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4170 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7303 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   155469 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4301 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_software_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6770 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_software_deployments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12787 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_stacks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_template_format.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42021 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_template_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_template_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18854 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.779009 python-heatclient-3.3.0/heatclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13280 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/v1/test_hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.779009 python-heatclient-3.3.0/heatclient/tests/unit/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/var/adopt_stack_data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9443 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/var/dot_test.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/var/environment.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/tests/unit/var/minimal.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.783010 python-heatclient-3.3.0/heatclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/build_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2408 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3036 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5186 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71764 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/software_configs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/software_deployments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12114 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/stacks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/heatclient/v1/template_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.783010 python-heatclient-3.3.0/python_heatclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2937 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5612 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4000 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-17 11:16:22.000000 python-heatclient-3.3.0/python_heatclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.751006 python-heatclient-3.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.783010 python-heatclient-3.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/notes/add-converge-in-osc-stack-update-10f256589f628d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/notes/add-files-container-stack-create-update-324b931f8f474b3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/notes/bug-1643492-2d7537b55f347722.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.787010 python-heatclient-3.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5767 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.751006 python-heatclient-3.3.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.751006 python-heatclient-3.3.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.787010 python-heatclient-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3145 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5378 2023-05-17 11:16:22.791011 python-heatclient-3.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-17 11:16:22.787010 python-heatclient-3.3.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/tools/heat.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2023-05-17 11:15:59.000000 python-heatclient-3.3.0/tox.ini
```

### Comparing `python-heatclient-3.2.0/.zuul.yaml` & `python-heatclient-3.3.0/.zuul.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       - ^.*\.rst$
       - ^releasenotes/.*$
       - ^heatclient/tests/.*$
 
 - project:
     templates:
       - openstack-cover-jobs
-      - openstack-python3-zed-jobs
+      - openstack-python3-jobs
       - check-requirements
       - openstackclient-plugin-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - heatclient-functional
```

### Comparing `python-heatclient-3.2.0/AUTHORS` & `python-heatclient-3.3.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/CONTRIBUTING.rst` & `python-heatclient-3.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/ChangeLog` & `python-heatclient-3.3.0/ChangeLog`

 * *Files identical despite different names*

```diff
@@ -1,14 +1,21 @@
 CHANGES
 =======
 
+3.3.0
+-----
+
+* Add Python 3.10 to supported runtime
+* Update master for stable/2023.1
+
 3.2.0
 -----
 
 * Adapt to tox 4
+* Switch to 2023.1 Python3 unit tests and generic template name
 * Imported Translations from Zanata
 * Update master for stable/zed
 
 3.1.0
 -----
 
 * Accept sha256 hash for swift tempurl
```

### Comparing `python-heatclient-3.2.0/LICENSE` & `python-heatclient-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/PKG-INFO` & `python-heatclient-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-heatclient
-Version: 3.2.0
+Version: 3.3.0
 Summary: OpenStack Orchestration API Client Library
 Home-page: https://docs.openstack.org/python-heatclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -60,10 +60,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `python-heatclient-3.2.0/README.rst` & `python-heatclient-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/Makefile` & `python-heatclient-3.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/cli/orchestration.rst` & `python-heatclient-3.3.0/doc/source/cli/orchestration.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/cli/software_deployment.rst` & `python-heatclient-3.3.0/doc/source/cli/software_deployment.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/cli/stack.rst` & `python-heatclient-3.3.0/doc/source/cli/stack.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/conf.py` & `python-heatclient-3.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/contributor/contributing.rst` & `python-heatclient-3.3.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/ext/gen_ref.py` & `python-heatclient-3.3.0/doc/source/ext/gen_ref.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/index.rst` & `python-heatclient-3.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/doc/source/man/heat.rst` & `python-heatclient-3.3.0/doc/source/man/heat.rst`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/__init__.py` & `python-heatclient-3.3.0/heatclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/_i18n.py` & `python-heatclient-3.3.0/heatclient/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/client.py` & `python-heatclient-3.3.0/heatclient/client.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/base.py` & `python-heatclient-3.3.0/heatclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/deployment_utils.py` & `python-heatclient-3.3.0/heatclient/common/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/environment_format.py` & `python-heatclient-3.3.0/heatclient/common/environment_format.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/event_utils.py` & `python-heatclient-3.3.0/heatclient/common/event_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/format_utils.py` & `python-heatclient-3.3.0/heatclient/common/format_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/hook_utils.py` & `python-heatclient-3.3.0/heatclient/common/hook_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/http.py` & `python-heatclient-3.3.0/heatclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/resource_formatter.py` & `python-heatclient-3.3.0/heatclient/common/resource_formatter.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/template_format.py` & `python-heatclient-3.3.0/heatclient/common/template_format.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/template_utils.py` & `python-heatclient-3.3.0/heatclient/common/template_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/common/utils.py` & `python-heatclient-3.3.0/heatclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/exc.py` & `python-heatclient-3.3.0/heatclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/plugin.py` & `python-heatclient-3.3.0/heatclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/build_info.py` & `python-heatclient-3.3.0/heatclient/osc/v1/build_info.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/event.py` & `python-heatclient-3.3.0/heatclient/osc/v1/event.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/resource.py` & `python-heatclient-3.3.0/heatclient/osc/v1/resource.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/resource_type.py` & `python-heatclient-3.3.0/heatclient/osc/v1/resource_type.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/service.py` & `python-heatclient-3.3.0/heatclient/osc/v1/service.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/snapshot.py` & `python-heatclient-3.3.0/heatclient/osc/v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/software_config.py` & `python-heatclient-3.3.0/heatclient/osc/v1/software_config.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/software_deployment.py` & `python-heatclient-3.3.0/heatclient/osc/v1/software_deployment.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/stack.py` & `python-heatclient-3.3.0/heatclient/osc/v1/stack.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/stack_failures.py` & `python-heatclient-3.3.0/heatclient/osc/v1/stack_failures.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/osc/v1/template.py` & `python-heatclient-3.3.0/heatclient/osc/v1/template.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/shell.py` & `python-heatclient-3.3.0/heatclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/base.py` & `python-heatclient-3.3.0/heatclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/config.py` & `python-heatclient-3.3.0/heatclient/tests/functional/config.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/base.py` & `python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/test_readonly.py` & `python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/test_readonly.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/osc/v1/test_stack.py` & `python-heatclient-3.3.0/heatclient/tests/functional/osc/v1/test_stack.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/functional/test_readonly_heat.py` & `python-heatclient-3.3.0/heatclient/tests/functional/test_readonly_heat.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/inline_templates.py` & `python-heatclient-3.3.0/heatclient/tests/inline_templates.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/test_templates/adopt.json` & `python-heatclient-3.3.0/heatclient/tests/test_templates/adopt.json`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/test_templates/adopt_with_file.json` & `python-heatclient-3.3.0/heatclient/tests/test_templates/adopt_with_file.json`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/fakes.py` & `python-heatclient-3.3.0/heatclient/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/fakes.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/fakes.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_build_info.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_build_info.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_event.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_event.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_resource.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_resource.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_resource_type.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_resource_type.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_service.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_snapshot.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_software_config.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_software_config.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_software_deployment.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_software_deployment.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_stack.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_stack.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_stack_failures.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_stack_failures.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/osc/v1/test_template.py` & `python-heatclient-3.3.0/heatclient/tests/unit/osc/v1/test_template.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_actions.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_build_info.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_build_info.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_common_http.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_common_http.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_deployment_utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_deployment_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_environment_format.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_environment_format.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_event_utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_event_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_events.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_format_utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_format_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_openstack_common.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_openstack_common.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_resource_formatter.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_resource_formatter.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_resource_types.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_resources.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_service.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_shell.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_software_configs.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_software_configs.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_software_deployments.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_software_deployments.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_stacks.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_stacks.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_template_format.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_template_format.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_template_utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_template_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_template_versions.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_template_versions.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/test_utils.py` & `python-heatclient-3.3.0/heatclient/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/v1/test_hooks.py` & `python-heatclient-3.3.0/heatclient/tests/unit/v1/test_hooks.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/tests/unit/var/dot_test.json` & `python-heatclient-3.3.0/heatclient/tests/unit/var/dot_test.json`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/__init__.py` & `python-heatclient-3.3.0/heatclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/actions.py` & `python-heatclient-3.3.0/heatclient/v1/actions.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/build_info.py` & `python-heatclient-3.3.0/heatclient/v1/build_info.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/client.py` & `python-heatclient-3.3.0/heatclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/events.py` & `python-heatclient-3.3.0/heatclient/v1/events.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/resource_types.py` & `python-heatclient-3.3.0/heatclient/v1/resource_types.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/resources.py` & `python-heatclient-3.3.0/heatclient/v1/resources.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/services.py` & `python-heatclient-3.3.0/heatclient/v1/services.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/shell.py` & `python-heatclient-3.3.0/heatclient/v1/shell.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/software_configs.py` & `python-heatclient-3.3.0/heatclient/v1/software_configs.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/software_deployments.py` & `python-heatclient-3.3.0/heatclient/v1/software_deployments.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/stacks.py` & `python-heatclient-3.3.0/heatclient/v1/stacks.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/heatclient/v1/template_versions.py` & `python-heatclient-3.3.0/heatclient/v1/template_versions.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/python_heatclient.egg-info/PKG-INFO` & `python-heatclient-3.3.0/python_heatclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-heatclient
-Version: 3.2.0
+Version: 3.3.0
 Summary: OpenStack Orchestration API Client Library
 Home-page: https://docs.openstack.org/python-heatclient/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -60,10 +60,11 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
```

### Comparing `python-heatclient-3.2.0/python_heatclient.egg-info/SOURCES.txt` & `python-heatclient-3.3.0/python_heatclient.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 python_heatclient.egg-info/pbr.json
 python_heatclient.egg-info/requires.txt
 python_heatclient.egg-info/top_level.txt
 releasenotes/notes/add-converge-in-osc-stack-update-10f256589f628d13.yaml
 releasenotes/notes/add-files-container-stack-create-update-324b931f8f474b3d.yaml
 releasenotes/notes/bug-1643492-2d7537b55f347722.yaml
 releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
```

### Comparing `python-heatclient-3.2.0/python_heatclient.egg-info/entry_points.txt` & `python-heatclient-3.3.0/python_heatclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/releasenotes/source/conf.py` & `python-heatclient-3.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `python-heatclient-3.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/requirements.txt` & `python-heatclient-3.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/setup.cfg` & `python-heatclient-3.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	heatclient
```

### Comparing `python-heatclient-3.2.0/setup.py` & `python-heatclient-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/test-requirements.txt` & `python-heatclient-3.3.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/tools/heat.bash_completion` & `python-heatclient-3.3.0/tools/heat.bash_completion`

 * *Files identical despite different names*

### Comparing `python-heatclient-3.2.0/tox.ini` & `python-heatclient-3.3.0/tox.ini`

 * *Files identical despite different names*

