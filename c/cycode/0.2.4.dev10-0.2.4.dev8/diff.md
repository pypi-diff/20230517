# Comparing `tmp/cycode-0.2.4.dev10.tar.gz` & `tmp/cycode-0.2.4.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycode-0.2.4.dev10.tar", max compression
+gzip compressed data, was "cycode-0.2.4.dev8.tar", max compression
```

## Comparing `cycode-0.2.4.dev10.tar` & `cycode-0.2.4.dev8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    31536 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/README.md
--rw-r--r--   0        0        0      103 2023-05-17 16:29:53.727352 cycode-0.2.4.dev10/cycode/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/auth/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/auth/auth_command.py
--rw-r--r--   0        0        0     4761 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/auth/auth_manager.py
--rw-r--r--   0        0        0     1652 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/ci_integrations.py
--rw-r--r--   0        0        0    47714 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/code_scanner.py
--rw-r--r--   0        0        0      453 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/config.py
--rw-r--r--   0        0        0      387 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/config.yaml
--rw-r--r--   0        0        0     4994 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/consts.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/exceptions/__init__.py
--rw-r--r--   0        0        0     1698 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/exceptions/custom_exceptions.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/maven/__init__.py
--rw-r--r--   0        0        0     2191 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
--rw-r--r--   0        0        0      992 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/maven/restore_gradle_dependencies.py
--rw-r--r--   0        0        0     2931 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/maven/restore_maven_dependencies.py
--rw-r--r--   0        0        0     5835 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/helpers/sca_code_scanner.py
--rw-r--r--   0        0        0     6734 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/main.py
--rw-r--r--   0        0        0     1106 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/models.py
--rw-r--r--   0        0        0      195 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/__init__.py
--rw-r--r--   0        0        0      356 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/base_printer.py
--rw-r--r--   0        0        0      982 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/json_printer.py
--rw-r--r--   0        0        0     1068 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/results_printer.py
--rw-r--r--   0        0        0     5826 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/table_printer.py
--rw-r--r--   0        0        0     8749 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/printers/text_printer.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/__init__.py
--rw-r--r--   0        0        0      533 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/base_file_manager.py
--rw-r--r--   0        0        0     4348 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/config_file_manager.py
--rw-r--r--   0        0        0     6470 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/configuration_manager.py
--rw-r--r--   0        0        0     1908 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/credentials_manager.py
--rw-r--r--   0        0        0     6853 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/user_settings/user_settings_commands.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/__init__.py
--rw-r--r--   0        0        0     2054 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/path_utils.py
--rw-r--r--   0        0        0      195 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/scan_utils.py
--rw-r--r--   0        0        0      910 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/shell_executor.py
--rw-r--r--   0        0        0     1217 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/string_utils.py
--rw-r--r--   0        0        0     2700 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/task_timer.py
--rw-r--r--   0        0        0      815 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      865 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cli/zip_file.py
--rw-r--r--   0        0        0       57 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/auth_client.py
--rw-r--r--   0        0        0     2458 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/config.py
--rw-r--r--   0        0        0      126 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/config.yaml
--rw-r--r--   0        0        0      119 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/config_dev.py
--rw-r--r--   0        0        0      220 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/cycode_client.py
--rw-r--r--   0        0        0     2706 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/cycode_client_base.py
--rw-r--r--   0        0        0      543 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/cycode_dev_based_client.py
--rw-r--r--   0        0        0     1596 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/cycode_token_based_client.py
--rw-r--r--   0        0        0     8126 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/models.py
--rw-r--r--   0        0        0     6222 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/scan_client.py
--rw-r--r--   0        0        0        0 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/scan_config/__init__.py
--rw-r--r--   0        0        0     1090 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/scan_config/scan_config_base.py
--rw-r--r--   0        0        0     1021 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/scan_config/scan_config_creator.py
--rw-r--r--   0        0        0      197 2023-05-17 16:29:23.217075 cycode-0.2.4.dev10/cycode/cyclient/utils.py
--rw-r--r--   0        0        0     1894 2023-05-17 16:29:53.723352 cycode-0.2.4.dev10/pyproject.toml
--rw-r--r--   0        0        0    33355 1970-01-01 00:00:00.000000 cycode-0.2.4.dev10/PKG-INFO
+-rw-r--r--   0        0        0    31536 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/README.md
+-rw-r--r--   0        0        0      102 2023-05-15 10:12:10.664827 cycode-0.2.4.dev8/cycode/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_command.py
+-rw-r--r--   0        0        0     4761 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py
+-rw-r--r--   0        0        0     1652 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/ci_integrations.py
+-rw-r--r--   0        0        0    47714 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/code_scanner.py
+-rw-r--r--   0        0        0      453 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.py
+-rw-r--r--   0        0        0      387 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/config.yaml
+-rw-r--r--   0        0        0     4994 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/consts.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/__init__.py
+-rw-r--r--   0        0        0     1698 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/__init__.py
+-rw-r--r--   0        0        0     2191 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py
+-rw-r--r--   0        0        0      992 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py
+-rw-r--r--   0        0        0     2931 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py
+-rw-r--r--   0        0        0     5835 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py
+-rw-r--r--   0        0        0     6734 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/main.py
+-rw-r--r--   0        0        0     1106 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/models.py
+-rw-r--r--   0        0        0      195 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/__init__.py
+-rw-r--r--   0        0        0      356 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/base_printer.py
+-rw-r--r--   0        0        0      982 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/json_printer.py
+-rw-r--r--   0        0        0     1068 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/results_printer.py
+-rw-r--r--   0        0        0     5670 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py
+-rw-r--r--   0        0        0     8749 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/__init__.py
+-rw-r--r--   0        0        0      533 2023-05-15 10:11:38.320579 cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py
+-rw-r--r--   0        0        0     4348 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py
+-rw-r--r--   0        0        0     6470 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py
+-rw-r--r--   0        0        0     1908 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py
+-rw-r--r--   0        0        0     6853 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/__init__.py
+-rw-r--r--   0        0        0     2054 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py
+-rw-r--r--   0        0        0      195 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/scan_utils.py
+-rw-r--r--   0        0        0      910 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py
+-rw-r--r--   0        0        0     1217 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py
+-rw-r--r--   0        0        0     2700 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py
+-rw-r--r--   0        0        0      815 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      865 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cli/zip_file.py
+-rw-r--r--   0        0        0       57 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/auth_client.py
+-rw-r--r--   0        0        0     2458 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.py
+-rw-r--r--   0        0        0      126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config.yaml
+-rw-r--r--   0        0        0      119 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/config_dev.py
+-rw-r--r--   0        0        0      220 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client.py
+-rw-r--r--   0        0        0     2706 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_client_base.py
+-rw-r--r--   0        0        0      543 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py
+-rw-r--r--   0        0        0     1596 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py
+-rw-r--r--   0        0        0     8126 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/models.py
+-rw-r--r--   0        0        0     6222 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_client.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/__init__.py
+-rw-r--r--   0        0        0     1090 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py
+-rw-r--r--   0        0        0     1021 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py
+-rw-r--r--   0        0        0      197 2023-05-15 10:11:38.324579 cycode-0.2.4.dev8/cycode/cyclient/utils.py
+-rw-r--r--   0        0        0     1893 2023-05-15 10:12:10.660827 cycode-0.2.4.dev8/pyproject.toml
+-rw-r--r--   0        0        0    33354 1970-01-01 00:00:00.000000 cycode-0.2.4.dev8/PKG-INFO
```

### Comparing `cycode-0.2.4.dev10/README.md` & `cycode-0.2.4.dev8/README.md`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/auth/auth_command.py` & `cycode-0.2.4.dev8/cycode/cli/auth/auth_command.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/auth/auth_manager.py` & `cycode-0.2.4.dev8/cycode/cli/auth/auth_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/ci_integrations.py` & `cycode-0.2.4.dev8/cycode/cli/ci_integrations.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/code_scanner.py` & `cycode-0.2.4.dev8/cycode/cli/code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/consts.py` & `cycode-0.2.4.dev8/cycode/cli/consts.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/exceptions/custom_exceptions.py` & `cycode-0.2.4.dev8/cycode/cli/exceptions/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/helpers/maven/base_restore_maven_dependencies.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/maven/base_restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/helpers/maven/restore_gradle_dependencies.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_gradle_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/helpers/maven/restore_maven_dependencies.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/maven/restore_maven_dependencies.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/helpers/sca_code_scanner.py` & `cycode-0.2.4.dev8/cycode/cli/helpers/sca_code_scanner.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/main.py` & `cycode-0.2.4.dev8/cycode/cli/main.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/models.py` & `cycode-0.2.4.dev8/cycode/cli/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/printers/json_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/json_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/printers/results_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/results_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/printers/table_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/table_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from cycode.cli.models import DocumentDetections, Detection
 from cycode.cli.printers.base_printer import BasePrinter
 
 SEVERITY_COLUMN = 'Severity'
 LICENSE_COLUMN = 'License'
 UPGRADE_COLUMN = 'Upgrade'
 REPOSITORY_COLUMN = 'Repository'
-CVE_COLUMN = 'CVE'
 PREVIEW_DETECTIONS_COMMON_HEADERS = ['File Path', 'Ecosystem', 'Dependency Name',
                                      'Direct Dependency',
                                      'Development Dependency']
 
 
 class TablePrinter(BasePrinter):
     RED_COLOR_NAME = 'red'
@@ -39,46 +38,44 @@
         detections_per_detection_type_id = self._extract_detections_per_detection_type_id(results)
 
         self._print_detection_per_detection_type_id(detections_per_detection_type_id)
 
         if self.context.obj.get('report_url'):
             click.secho(f"Report URL: {self.context.obj.get('report_url')}")
 
-    @staticmethod
-    def _extract_detections_per_detection_type_id(results: List[DocumentDetections]):
+    def _extract_detections_per_detection_type_id(self, results: List[DocumentDetections]):
         detections_per_detection_type_id = {}
 
         for document_detection in results:
             for detection in document_detection.detections:
                 if detection.detection_type_id not in detections_per_detection_type_id:
                     detections_per_detection_type_id[detection.detection_type_id] = []
                 detections_per_detection_type_id[detection.detection_type_id].append(detection)
 
         return detections_per_detection_type_id
 
     def _print_detection_per_detection_type_id(self, detections_per_detection_type_id: Dict[str, Detection]):
         for detection_type_id in detections_per_detection_type_id:
             detections = detections_per_detection_type_id[detection_type_id]
             headers = self._get_table_headers()
-            rows = []
-            title = ""
 
             if detection_type_id == PACKAGE_VULNERABILITY_POLICY_ID:
                 title = "Dependencies Vulnerabilities"
                 headers = [SEVERITY_COLUMN] + headers
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
-                headers.append(CVE_COLUMN)
                 headers.append(UPGRADE_COLUMN)
+                rows = []
                 for detection in detections:
                     rows.append(self._get_upgrade_package_vulnerability(detection))
 
             if detection_type_id == LICENSE_COMPLIANCE_POLICY_ID:
                 title = "License Compliance"
                 headers.extend(PREVIEW_DETECTIONS_COMMON_HEADERS)
                 headers.append(LICENSE_COLUMN)
+                rows = []
                 for detection in detections:
                     rows.append(self._get_license(detection))
 
             if len(rows) > 0:
                 self._print_table_detections(detections,
                                              headers,
                                              rows,
@@ -95,34 +92,31 @@
         text_table.header(headers)
 
         self.set_table_width(headers, text_table)
         for row in rows:
             text_table.add_row(row)
         click.echo(text_table.draw())
 
-    @staticmethod
-    def set_table_width(headers, text_table):
+    def set_table_width(self, headers, text_table):
         header_width_size_cols = []
         for header in headers:
             header_width_size_cols.append(len(header))
         text_table.set_cols_width(header_width_size_cols)
 
-    @staticmethod
-    def _print_summary_issues(detections: List, title: str):
+    def _print_summary_issues(self, detections: List, title: str):
         click.echo(
             f'⛔ Found {len(detections)} issues of type: {click.style(title, bold=True)}')
 
     def _get_common_detection_fields(self, detection: Detection):
         row = [
             detection.detection_details.get('file_name'),
             detection.detection_details.get('ecosystem'),
             detection.detection_details.get('package_name'),
             detection.detection_details.get('is_direct_dependency_str'),
-            detection.detection_details.get('is_dev_dependency_str'),
-            detection.detection_details.get('vulnerability_id')
+            detection.detection_details.get('is_dev_dependency_str')
         ]
 
         if self._is_git_repository():
             row = [detection.detection_details.get('repository_name')] + row
 
         return row
```

### Comparing `cycode-0.2.4.dev10/cycode/cli/printers/text_printer.py` & `cycode-0.2.4.dev8/cycode/cli/printers/text_printer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/user_settings/base_file_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/base_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/user_settings/config_file_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/config_file_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/user_settings/configuration_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/user_settings/credentials_manager.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/credentials_manager.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/user_settings/user_settings_commands.py` & `cycode-0.2.4.dev8/cycode/cli/user_settings/user_settings_commands.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/utils/path_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/utils/shell_executor.py` & `cycode-0.2.4.dev8/cycode/cli/utils/shell_executor.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/utils/string_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/utils/task_timer.py` & `cycode-0.2.4.dev8/cycode/cli/utils/task_timer.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/utils/yaml_utils.py` & `cycode-0.2.4.dev8/cycode/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cli/zip_file.py` & `cycode-0.2.4.dev8/cycode/cli/zip_file.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/auth_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/auth_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/config.py` & `cycode-0.2.4.dev8/cycode/cyclient/config.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/cycode_client_base.py` & `cycode-0.2.4.dev8/cycode/cyclient/cycode_client_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/cycode_dev_based_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/cycode_dev_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/cycode_token_based_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/cycode_token_based_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/models.py` & `cycode-0.2.4.dev8/cycode/cyclient/models.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/scan_client.py` & `cycode-0.2.4.dev8/cycode/cyclient/scan_client.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/scan_config/scan_config_base.py` & `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_base.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/cycode/cyclient/scan_config/scan_config_creator.py` & `cycode-0.2.4.dev8/cycode/cyclient/scan_config/scan_config_creator.py`

 * *Files identical despite different names*

### Comparing `cycode-0.2.4.dev10/pyproject.toml` & `cycode-0.2.4.dev8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycode"
-version = "0.2.4.dev10" # placeholder. Will be filled automatically on poetry build from Git Tag
+version = "0.2.4.dev8" # placeholder. Will be filled automatically on poetry build from Git Tag
 description = "Perform secrets/iac scans for your sources using Cycode's engine"
 keywords=["secret-scan", "cycode", "devops", "token", "secret", "security", "cycode", "code"]
 authors = ["Cycode <support@cycode.com>"]
 license = "MIT"
 repository = "https://github.com/cycodehq-public/cycode-cli"
 readme = "README.md"
 classifiers = [
```

### Comparing `cycode-0.2.4.dev10/PKG-INFO` & `cycode-0.2.4.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycode
-Version: 0.2.4.dev10
+Version: 0.2.4.dev8
 Summary: Perform secrets/iac scans for your sources using Cycode's engine
 Home-page: https://github.com/cycodehq-public/cycode-cli
 License: MIT
 Keywords: secret-scan,cycode,devops,token,secret,security,cycode,code
 Author: Cycode
 Author-email: support@cycode.com
 Requires-Python: >=3.7,<4.0
```

