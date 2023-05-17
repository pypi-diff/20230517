# Comparing `tmp/ayx_plugin_cli-1.0.4-py3-none-any.whl.zip` & `tmp/ayx_plugin_cli-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,51 +1,53 @@
-Zip file size: 74623 bytes, number of entries: 49
--rw-r--r--  2.0 unx      642 b- defN 22-Dec-07 23:27 ayx_plugin_cli/__init__.py
--rw-r--r--  2.0 unx    17023 b- defN 22-Dec-07 23:27 ayx_plugin_cli/__main__.py
--rw-r--r--  2.0 unx      836 b- defN 22-Dec-07 23:27 ayx_plugin_cli/exceptions.py
--rw-r--r--  2.0 unx     1609 b- defN 22-Dec-07 23:27 ayx_plugin_cli/node_js_helpers.py
--rw-r--r--  2.0 unx     6745 b- defN 22-Dec-07 23:27 ayx_plugin_cli/validation.py
--rw-r--r--  2.0 unx      218 b- defN 22-Dec-07 23:32 ayx_plugin_cli/version.py
--rw-r--r--  2.0 unx      640 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/__init__.py
--rw-rw-rw-  2.0 unx     7497 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/README_tests.md
--rw-rw-rw-  2.0 unx      782 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/__init__.j2
--rw-rw-rw-  2.0 unx     9731 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/clean_plugin_tests.j2
--rw-rw-rw-  2.0 unx     6523 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/plugin.j2
--rw-rw-rw-  2.0 unx     9067 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/plugin_tests.j2
--rw-rw-rw-  2.0 unx        1 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/requirements-local.j2
--rw-rw-rw-  2.0 unx       38 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/requirements-thirdparty.j2
--rw-rw-rw-  2.0 unx     1255 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/setup.j2
--rw-rw-rw-  2.0 unx     1778 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/input.j2
--rw-rw-rw-  2.0 unx     2256 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/multi_conn.j2
--rw-rw-rw-  2.0 unx     1549 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/multi_input.j2
--rw-rw-rw-  2.0 unx     2210 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/multi_output.j2
--rw-rw-rw-  2.0 unx     1965 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/optional.j2
--rw-rw-rw-  2.0 unx     1366 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/output.j2
--rw-rw-rw-  2.0 unx     1351 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/templates/python/macros/passthrough.j2
--rw-rw-rw-  2.0 unx        8 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/workspace_files/.gitignore
--rw-rw-rw-  2.0 unx        0 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/workspace_files/README.md
--rw-rw-rw-  2.0 unx    12141 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/workspace_files/default_package_icon.png
--rw-rw-rw-  2.0 unx      774 b- defN 22-Dec-07 23:27 ayx_plugin_cli/assets/workspace_files/ui_template/README.md
--rw-r--r--  2.0 unx      664 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/__init__.py
--rw-r--r--  2.0 unx     2770 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/constants.py
--rw-r--r--  2.0 unx     7379 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/template_engine.py
--rw-r--r--  2.0 unx     3307 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/template_tool_settings.py
--rw-r--r--  2.0 unx      648 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/__init__.py
--rw-r--r--  2.0 unx     1291 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/dodo.py
--rw-r--r--  2.0 unx     1281 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/__init__.py
--rw-r--r--  2.0 unx     5859 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_plugin.py
--rw-r--r--  2.0 unx     4093 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_yxi.py
--rw-r--r--  2.0 unx     3603 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_artifact.py
--rw-r--r--  2.0 unx    11183 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py
--rw-r--r--  2.0 unx     1799 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py
--rw-r--r--  2.0 unx     4469 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py
--rw-r--r--  2.0 unx     2303 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/doit/build_tasks/install_yxi.py
--rw-r--r--  2.0 unx      655 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/models/__init__.py
--rw-r--r--  2.0 unx     4455 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/models/cloud_manifest.py
--rw-r--r--  2.0 unx     4941 b- defN 22-Dec-07 23:27 ayx_plugin_cli/ayx_workspace/models/v1.py
--rw-rw-rw-  2.0 unx    22092 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1769 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       95 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5132 b- defN 22-Dec-07 23:32 ayx_plugin_cli-1.0.4.dist-info/RECORD
-49 files, 177900 bytes uncompressed, 66047 bytes compressed:  62.9%
+Zip file size: 192336 bytes, number of entries: 51
+-rw-r--r--  2.0 unx      642 b- defN 23-May-17 04:42 ayx_plugin_cli/__init__.py
+-rw-r--r--  2.0 unx    18505 b- defN 23-May-17 04:42 ayx_plugin_cli/__main__.py
+-rw-r--r--  2.0 unx      836 b- defN 23-May-17 04:42 ayx_plugin_cli/exceptions.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-May-17 04:42 ayx_plugin_cli/node_js_helpers.py
+-rw-r--r--  2.0 unx     6992 b- defN 23-May-17 04:42 ayx_plugin_cli/validation.py
+-rw-r--r--  2.0 unx      218 b- defN 23-May-17 04:45 ayx_plugin_cli/version.py
+-rw-r--r--  2.0 unx      640 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/__init__.py
+-rw-rw-rw-  2.0 unx     7497 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/README_tests.md
+-rw-rw-rw-  2.0 unx      782 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/__init__.j2
+-rw-rw-rw-  2.0 unx     9731 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/clean_plugin_tests.j2
+-rw-rw-rw-  2.0 unx     6523 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/plugin.j2
+-rw-rw-rw-  2.0 unx     9067 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/plugin_tests.j2
+-rw-rw-rw-  2.0 unx        1 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/requirements-local.j2
+-rw-rw-rw-  2.0 unx       38 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/requirements-thirdparty.j2
+-rw-rw-rw-  2.0 unx     1255 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/setup.j2
+-rw-rw-rw-  2.0 unx     1778 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/input.j2
+-rw-rw-rw-  2.0 unx     2256 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/multi_conn.j2
+-rw-rw-rw-  2.0 unx     1549 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/multi_input.j2
+-rw-rw-rw-  2.0 unx     2210 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/multi_output.j2
+-rw-rw-rw-  2.0 unx     1965 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/optional.j2
+-rw-rw-rw-  2.0 unx     1366 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/output.j2
+-rw-rw-rw-  2.0 unx     1351 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/templates/python/macros/passthrough.j2
+-rw-rw-rw-  2.0 unx        8 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/workspace_files/.gitignore
+-rw-rw-rw-  2.0 unx        0 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/workspace_files/README.md
+-rw-rw-rw-  2.0 unx    12141 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/workspace_files/default_package_icon.png
+-rw-r--r--  2.0 unx   118540 b- defN 23-May-17 04:43 ayx_plugin_cli/assets/workspace_files/ui_artifact.zip
+-rw-rw-rw-  2.0 unx      774 b- defN 23-May-17 04:42 ayx_plugin_cli/assets/workspace_files/ui_template/README.md
+-rw-r--r--  2.0 unx      664 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/__init__.py
+-rw-r--r--  2.0 unx     2833 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/constants.py
+-rw-r--r--  2.0 unx     7379 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/template_engine.py
+-rw-r--r--  2.0 unx     3307 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/template_tool_settings.py
+-rw-r--r--  2.0 unx      648 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/__init__.py
+-rw-r--r--  2.0 unx     1291 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/dodo.py
+-rw-r--r--  2.0 unx     1419 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/__init__.py
+-rw-r--r--  2.0 unx     4091 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_plugin.py
+-rw-r--r--  2.0 unx     4463 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_yxi.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_artifact.py
+-rw-r--r--  2.0 unx    11255 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py
+-rw-r--r--  2.0 unx     1780 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py
+-rw-r--r--  2.0 unx     2796 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_ui.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py
+-rw-r--r--  2.0 unx     2303 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/doit/build_tasks/install_yxi.py
+-rw-r--r--  2.0 unx      655 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/models/__init__.py
+-rw-r--r--  2.0 unx     4455 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/models/cloud_manifest.py
+-rw-r--r--  2.0 unx     4941 b- defN 23-May-17 04:42 ayx_plugin_cli/ayx_workspace/models/v1.py
+-rw-rw-rw-  2.0 unx    22092 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1799 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     5361 b- defN 23-May-17 04:45 ayx_plugin_cli-1.1.0.dist-info/RECORD
+51 files, 300281 bytes uncompressed, 183382 bytes compressed:  38.9%
```

## zipnote {}

```diff
@@ -69,14 +69,17 @@
 
 Filename: ayx_plugin_cli/assets/workspace_files/README.md
 Comment: 
 
 Filename: ayx_plugin_cli/assets/workspace_files/default_package_icon.png
 Comment: 
 
+Filename: ayx_plugin_cli/assets/workspace_files/ui_artifact.zip
+Comment: 
+
 Filename: ayx_plugin_cli/assets/workspace_files/ui_template/README.md
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/__init__.py
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/constants.py
@@ -108,14 +111,17 @@
 
 Filename: ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py
 Comment: 
 
+Filename: ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_ui.py
+Comment: 
+
 Filename: ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/doit/build_tasks/install_yxi.py
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/models/__init__.py
@@ -123,26 +129,26 @@
 
 Filename: ayx_plugin_cli/ayx_workspace/models/cloud_manifest.py
 Comment: 
 
 Filename: ayx_plugin_cli/ayx_workspace/models/v1.py
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/LICENSE
+Filename: ayx_plugin_cli-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/METADATA
+Filename: ayx_plugin_cli-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/WHEEL
+Filename: ayx_plugin_cli-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/entry_points.txt
+Filename: ayx_plugin_cli-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/top_level.txt
+Filename: ayx_plugin_cli-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ayx_plugin_cli-1.0.4.dist-info/RECORD
+Filename: ayx_plugin_cli-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ayx_plugin_cli/__main__.py

```diff
@@ -72,26 +72,25 @@
     return decorator
 
 
 @app.callback()
 @_handle_cli_errors
 def _validate_all(ctx: typer.Context) -> None:
     CLIValidator.check_for_updates()
-    node_subcommands = ["sdk-workspace-init"]
+    node_subcommands = ["generate-ui"]  # don't require use_ui parameters
     workspace_subcommands = [
         "create-ayx-plugin",
         "generate-config-files",
         "generate-tests",
+        "generate-ui",
         "test",
+        "create-yxi",
     ]
     nonzero_tools_subcommands = ["create-yxpe", "create-yxi", "designer-install"]
-    if (
-        ctx.invoked_subcommand
-        in node_subcommands + workspace_subcommands + nonzero_tools_subcommands
-    ):
+    if ctx.invoked_subcommand in node_subcommands:
         CLIValidator.validate_node()
     if ctx.invoked_subcommand in workspace_subcommands + nonzero_tools_subcommands:
         CLIValidator.validate_json_exists()
     if ctx.invoked_subcommand in nonzero_tools_subcommands:
         CLIValidator.validate_nonzero_tools()
 
 
@@ -141,22 +140,24 @@
 
     workspace_file_path = AYX_WORKSPACE_JSON_PATH
     configuration_directory = cur_dir / "configuration"
     build_directory = cur_dir / "build_tasks"
     dodo_file = cur_dir / "dodo.py"
     backend_directory = cur_dir / "backend"
     ui_directory = cur_dir / "ui"
+    schemas_dir = cur_dir / "DCMSchemas"
 
     paths_to_be_created = [
         workspace_file_path,
         configuration_directory,
         dodo_file,
         build_directory,
         backend_directory,
         ui_directory,
+        schemas_dir,
     ]
 
     existing_paths = [path for path in paths_to_be_created if path.exists()]
     if existing_paths:
         _overwrite_paths_with_prompt(existing_paths)
 
     workspace_model = AyxWorkspaceV1(
@@ -190,14 +191,37 @@
     typer.echo(f"Workspace settings can be modified in: {workspace_file_path}")
 
     generate_config_files()
 
 
 @app.command()
 @_handle_cli_errors
+def generate_ui(
+    tool_name: Optional[List[str]] = typer.Option(
+        None,
+        prompt="Tool Name",
+        help="The specific tool(s) you want to generate UI components for. If no arguments are passed,"
+        "UI components will be generated for all tools in this workspace"
+        "(Be warned, this may take a while for multi-tool workspaces)."
+        "You can specify multiple individual tools as well",
+    )
+) -> None:
+    """Generate UI components for tools in this workspace."""
+    tool_names = _check_tool_name(
+        tool_name, "Attempted to generate UI for nonexistent tool"
+    )
+    for _tool_name in tool_names:
+        _run_doit(
+            ["generate_ui", "--tool_name", _tool_name],
+            f"Generating UI component for {_tool_name}",
+        )
+
+
+@app.command()
+@_handle_cli_errors
 def create_ayx_plugin(
     tool_name: str = typer.Option(
         ..., prompt="Tool Name", help="Name of the tool to create."
     ),
     tool_type: TemplateToolTypes = typer.Option(
         default=TemplateToolTypes.SingleInputSingleOutput,
         prompt="Tool Type",
@@ -214,14 +238,19 @@
         help="The version of the tool to generate.",
     ),
     dcm_namespace: str = typer.Option(
         default="",
         prompt="DCM Namespace",
         help="Namespace to register plugin's schemas into.",
     ),
+    use_ui: bool = typer.Option(
+        False,
+        help="Generate a UI component for this tool",
+        callback=CLIValidator.validate_node_param,
+    ),
 ) -> None:
     """Create a new Alteryx plugin in this workspace."""
     workspace = AyxWorkspaceV1.load()
 
     class_name = _remove_whitespace(tool_name)
 
     if class_name in [
@@ -279,14 +308,33 @@
             "--tool_folder",
             tool_settings.get_tool_folder_name(),
         ],
         "Create plugin",
     )
     generate_config_files()
     generate_tests(tool_name=[tool_name], warn_possible_failures=False)
+    if use_ui:
+        generate_ui(tool_name=[tool_name])
+
+
+def _check_tool_name(tool_name: Optional[List[str]], error_msg: str) -> List[str]:
+    workspace = AyxWorkspaceV1.load()
+
+    tool_names = tool_name or []
+    workspace_tool_names = [
+        _remove_whitespace(_tool_name) for _tool_name in list(workspace.tools.keys())
+    ]
+    for _tool_name in tool_names:
+        if _remove_whitespace(_tool_name) not in workspace_tool_names:
+            raise CliError(error_msg)
+    return (
+        workspace_tool_names
+        if len(tool_names) == 0
+        else [_remove_whitespace(_tool_name) for _tool_name in tool_names]
+    )
 
 
 @app.command()
 @_handle_cli_errors
 def generate_tests(
     warn_possible_failures: bool = typer.Option(True),
     tool_name: Optional[List[str]] = typer.Option(
@@ -294,26 +342,16 @@
         prompt="Tool Name",
         help="The specific tools you want to generate tests for. If no arguments are passed,"
         "tests will be generated for all tools in this workspace."
         "You can specify multiple individual tools as well.",
     ),
 ) -> None:
     """Generate the test files for tools in this workspace."""
-    workspace = AyxWorkspaceV1.load()
-    tool_names = tool_name or []
-    workspace_tool_names = [
-        _remove_whitespace(_tool_name) for _tool_name in list(workspace.tools.keys())
-    ]
-    for _tool_name in tool_names:
-        if _remove_whitespace(_tool_name) not in workspace_tool_names:
-            raise CliError("Attempted to generate tests for nonexistent tool")
-    tool_names = (
-        workspace_tool_names
-        if len(tool_names) == 0
-        else [_remove_whitespace(_tool_name) for _tool_name in tool_names]
+    tool_names = _check_tool_name(
+        tool_name, "Attempted to generate tests for nonexistent tool"
     )
     for _tool_name in tool_names:
         _run_doit(
             ["generate_tests", "--tool_name", _tool_name],
             f"Generating test files for {_tool_name}",
         )
     if warn_possible_failures:
@@ -330,34 +368,40 @@
 def generate_config_files() -> None:
     """Generate the config files for the tools in this workspace."""
     _run_doit(["generate_config_files"], "Generating config files")
 
 
 @app.command()
 @_handle_cli_errors
-def create_yxi() -> None:
+def create_yxi(
+    use_ui: bool = typer.Option(False, callback=CLIValidator.validate_node_param)
+) -> None:
     """Create a YXI from the tools in this workspace."""
-    _run_doit(["create_yxi"], "Creating YXI")
+    if use_ui:
+        _run_doit(["create_yxi", "--use_ui"], "Creating YXI")
+    else:
+        _run_doit(["create_yxi"], "Creating YXI")
 
 
 @app.command()
 @_handle_cli_errors
 def designer_install(
     install_type: YxiInstallType = typer.Option(
         YxiInstallType.USER,
         prompt="Install Type",
         help="The type of install to perform.\n"
         "\nuser -> %APPDATA%\\Alteryx\\Tools"
         "\n, admin -> %ALLUSERSPROFILE%\\Alteryx\\Tools",
-    )
+    ),
+    use_ui: bool = typer.Option(False, callback=CLIValidator.validate_node_param),
 ) -> None:
     """Install the tools from this workspace into Alteryx Designer."""
     yxi_name = AyxWorkspaceV1.load().name
     Path(f"build/yxi/{yxi_name}.yxi").unlink(missing_ok=True)
-    create_yxi()
+    create_yxi(use_ui)
     install_yxi(YXI_OUTPUT_DIR.resolve() / f"{yxi_name}.yxi", install_type)
     typer.echo(
         "If this is your first time installing these tools, or you have made modifications to your ayx_workspace.json file, please restart Designer for these changes to take effect."
     )
 
 
 @app.command()
@@ -396,15 +440,15 @@
             files_to_overwrite.append(install_dir / tool_name)
 
     if files_to_overwrite:
         _overwrite_paths_with_prompt(files_to_overwrite)
 
     _run_doit(
         ["install_yxi", "--yxi_path", str(yxi_path), "--install_dir", str(install_dir)],
-        f"Installing yxi {str(yxi_path)} into designer",
+        f"Installing YXI",
     )
 
 
 @app.command()
 def test() -> None:
     """Run the tests command for the language in question."""
     workspace = AyxWorkspaceV1.load()
```

## ayx_plugin_cli/node_js_helpers.py

```diff
@@ -12,24 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Helper methods for running Node JS."""
 import subprocess
 from typing import Any, List
 
 
-def run_node_js(args: List[str], **kwargs: Any) -> subprocess.CompletedProcess:
-    """Run a node subprocess."""
-    return _run_node_subprocess(["node"] + args, **kwargs)
+class NodeHelper:
+    """Helper class for running Node JS."""
 
-
-def run_npm(args: List[str], **kwargs: Any) -> subprocess.CompletedProcess:
-    """Run an NPM subprocess."""
-    return _run_node_subprocess(["npm"] + args, **kwargs)
-
-
-def _run_node_subprocess(args: List[str], **kwargs: Any) -> subprocess.CompletedProcess:
-    """Run a node js subprocess."""
-    # We have to use `shell=True` here because node/npm frequently use nested environment
-    # variables to resolve their install locations, which is a feature that is only present
-    # with shell=True. As a result, it is recommended to use a single string as the command
-    # instead of a list of string arguments, which is why we join them here.
-    return subprocess.run(" ".join(args), capture_output=True, shell=True, **kwargs)
+    @classmethod
+    def run_node_js(cls, *args: Any, **kwargs: Any) -> subprocess.CompletedProcess:
+        """Run a node subprocess."""
+        return cls._run_node_subprocess(["node"] + [str(i) for i in args], **kwargs)
+
+    @classmethod
+    def run_npm(cls, *args: Any, **kwargs: Any) -> subprocess.CompletedProcess:
+        """Run an NPM subprocess."""
+        return cls._run_node_subprocess(["npm"] + [str(i) for i in args], **kwargs)
+
+    @staticmethod
+    def _run_node_subprocess(
+        args: List[str], **kwargs: Any
+    ) -> subprocess.CompletedProcess:
+        """Run a node js subprocess."""
+        # We have to use `shell=True` here because node/npm frequently use nested environment
+        # variables to resolve their install locations, which is a feature that is only present
+        # with shell=True. As a result, it is recommended to use a single string as the command
+        # instead of a list of string arguments, which is why we join them here.
+        return subprocess.run(" ".join(args), capture_output=True, shell=True, **kwargs)
```

## ayx_plugin_cli/validation.py

```diff
@@ -19,15 +19,15 @@
     AYX_WORKSPACE_JSON_PATH,
     MIN_NODE_JS_VERSION,
     MIN_NPM_VERSION,
     PYPI_URL,
 )
 from ayx_plugin_cli.ayx_workspace.models.v1 import AyxWorkspaceV1
 from ayx_plugin_cli.exceptions import CliError
-from ayx_plugin_cli.node_js_helpers import run_node_js, run_npm
+from ayx_plugin_cli.node_js_helpers import NodeHelper
 from ayx_plugin_cli.version import version as cli_version
 
 import packaging
 from packaging import version
 
 import requests
 
@@ -134,14 +134,22 @@
                 package = "npm"
 
             raise CliError(
                 f"Incompatible version of {package} found ({e.bad_version}). "
                 f"The minimum required version is {e.min_version}."
             )
 
+    @classmethod
+    def validate_node_param(cls, value: bool) -> bool:
+        """Validate node as parameter of create-ayx-plugin."""
+        if value:
+            cls.validate_node()
+            return True
+        return False
+
 
 class NodeJsNotFoundError(Exception):
     """NodeJS not found error."""
 
     pass
 
 
@@ -167,32 +175,34 @@
 
 
 def validate_node_js(
     min_version: Union[version.LegacyVersion, version.Version]
 ) -> None:
     """Validate that node is installed with a minimum version."""
     _validate_js_package(
-        run_node_js, min_version, NodeJsNotFoundError, NodeJsVersionError
+        NodeHelper.run_node_js, min_version, NodeJsNotFoundError, NodeJsVersionError
     )
 
 
 def validate_npm(min_version: Union[version.LegacyVersion, version.Version]) -> None:
     """Validate that npm is installed with a minimum version."""
-    _validate_js_package(run_npm, min_version, NpmNotFoundError, NpmVersionError)
+    _validate_js_package(
+        NodeHelper.run_npm, min_version, NpmNotFoundError, NpmVersionError
+    )
 
 
 def _validate_js_package(
-    runner: Callable[[List[str]], "subprocess.CompletedProcess"],
+    runner: Callable[..., "subprocess.CompletedProcess"],
     min_version: Union[version.LegacyVersion, version.Version],
     not_found_error: Type[NodeJsNotFoundError],
     version_error: Type[NodeJsVersionError],
 ) -> None:
     """Validate that JS packages are all available."""
     try:
-        completed_process = runner(["--version"])
+        completed_process = runner("--version")
     except Exception:
         raise not_found_error()
 
     if completed_process.returncode != 0:
         raise not_found_error()
 
     package_version = version.parse(completed_process.stdout.decode("utf-8"))
```

## ayx_plugin_cli/version.py

```diff
@@ -1,9 +1,9 @@
 """FILE GENERATED FROM SETUP.PY."""
-short_version = "1.0.4"
-version = "1.0.4"
-full_version = "1.0.4"
-git_revision = "d807750a29e67223a1e0b13f99edba88bc527f29"
+short_version = "1.1.0"
+version = "1.1.0"
+full_version = "1.1.0"
+git_revision = "4397ecaf305f97eaf72a77e22f2daa8fd96d0f9a"
 release = True
 
 if not release:
     version = full_version
```

## ayx_plugin_cli/ayx_workspace/constants.py

```diff
@@ -44,28 +44,29 @@
     ADMIN = "admin"
 
 
 BACKEND_PATH = Path("backend")
 AYX_WORKSPACE_JSON_PATH = Path("ayx_workspace.json")
 AYX_WORKSPACE_FILES = {
     BackendLanguage.Python: [
-        BACKEND_PATH / "requirements.txt",
+        BACKEND_PATH / "requirements-thirdparty.txt",
+        BACKEND_PATH / "requirements-local.txt",
         BACKEND_PATH / "setup.py",
         BACKEND_PATH / "ayx_plugins" / "__init__.py",
     ]
 }
 AYX_WORKSPACE_ARTIFACT_EXTENSIONS = {BackendLanguage.Python: ".pyz"}
 AYX_CLI_INSTALL_PATH = Path(__file__).parent.parent
 AYX_CLI_ASSETS_PATH = AYX_CLI_INSTALL_PATH / "assets"
 AYX_CLI_TEMPLATES_PATH = AYX_CLI_ASSETS_PATH / "templates"
 AYX_CLI_WORKSPACE_FILES_PATH = AYX_CLI_ASSETS_PATH / "workspace_files"
 TEMPLATE_ICON_PATH = AYX_CLI_WORKSPACE_FILES_PATH / "default_package_icon.png"
 AYX_CLI_UI_TEMPLATE = AYX_CLI_WORKSPACE_FILES_PATH / "ui_template"
-MIN_NODE_JS_VERSION = version.parse("10.0.0")
-MIN_NPM_VERSION = version.parse("5.6.0")
+MIN_NODE_JS_VERSION = version.parse("14.21.3")
+MIN_NPM_VERSION = version.parse("6.14.18")
 BUILD_CACHE_DIR = Path(".ayx_cli.cache")
 YXPE_CACHE_DIR = BUILD_CACHE_DIR / "YXPE"
 UI_TEMPLATE_CACHE_DIR = BUILD_CACHE_DIR / "ui_tool_template"
 WORKSPACE_CONFIG_DIR = Path("configuration")
 DCM_SCHEMAS_DIR = Path("DcmSchemas")
 TESTS_DIR = BACKEND_PATH / "tests"
 TEMPLATE_TOOL_CONFIG_DIR = os.path.join("configuration", "%(tool_name)s")
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/__init__.py

```diff
@@ -1,32 +1,35 @@
-# Copyright (C) 2022 Alteryx, Inc. All rights reserved.
+# Copyright (C) 2023 Alteryx, Inc. All rights reserved.
 #
 # Licensed under the ALTERYX SDK AND API LICENSE AGREEMENT;
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    https://www.alteryx.com/alteryx-sdk-and-api-license-agreement
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Alteryx CLI build tasks."""
-from .create_plugin import task__download_ui_tool_template, task_create_plugin
+from .create_plugin import task_create_plugin
 from .create_yxi import task_create_yxi
-from .generate_artifact import task_generate_artifact
+from .generate_artifact import task_generate_backend_artifact, task_generate_ui_artifact
 from .generate_config_files import task_generate_config_files
 from .generate_tests import task_generate_tests
+from .generate_ui import task__unpack_ui_tool_template, task_generate_ui
 from .initialize_workspace import task_initialize_workspace
 from .install_yxi import task_install_yxi
 
 __all__ = [
-    "task__download_ui_tool_template",
+    "task__unpack_ui_tool_template",
     "task_create_plugin",
     "task_create_yxi",
-    "task_generate_artifact",
+    "task_generate_backend_artifact",
+    "task_generate_ui_artifact",
     "task_generate_config_files",
     "task_generate_tests",
+    "task_generate_ui",
     "task_initialize_workspace",
     "task_install_yxi",
 ]
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_plugin.py

```diff
@@ -10,95 +10,78 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Task definition for creating plugin for the specified tool."""
 import os
 import shutil
-import stat
-import subprocess
 from pathlib import Path
 from typing import Dict
 
 from ayx_plugin_cli.ayx_workspace.constants import (
     AYX_WORKSPACE_JSON_PATH,
     BackendLanguage,
     DCM_SCHEMAS_DIR,
     TEMPLATE_ICON_PATH,
     TEMPLATE_TOOL_CONFIG_DIR,
     TEMPLATE_TOOL_ICON_PATH,
-    TEMPLATE_TOOL_UI_DIR,
     TemplateToolTypes,
-    UI_GIT_REPO_URL,
-    UI_TEMPLATE_CACHE_DIR,
 )
 from ayx_plugin_cli.ayx_workspace.models.v1 import AyxWorkspaceV1
 from ayx_plugin_cli.ayx_workspace.template_engine import TemplateEngine
-from ayx_plugin_cli.node_js_helpers import run_npm
-
-from doit.tools import run_once
-
-
-def task__download_ui_tool_template() -> Dict:
-    """Task to download the UI tool template."""
-    return {
-        "title": lambda task: "Download Tool Template",
-        "actions": [(git_clone_ui_tool_template, [UI_TEMPLATE_CACHE_DIR])],
-        "targets": [UI_TEMPLATE_CACHE_DIR],
-        "uptodate": [run_once],
-    }
 
 
 def task_create_plugin() -> Dict:
     """Create a plugin for the specified tool."""
-    tool_type_choices = tuple((tool_type, "") for tool_type in TemplateToolTypes)
+    tool_type_choices = tuple(
+        (tool_type, tool_type.value) for tool_type in TemplateToolTypes
+    )
 
     return {
         "title": lambda task: "Create plugin",
         "actions": [
-            copy_ui_tool_template,
-            ui_npm_install,
             build_backend_action(AyxWorkspaceV1.load().backend_language),
             generate_tool_configuration,
             generate_schemas_dir,
         ],
         "file_dep": [AYX_WORKSPACE_JSON_PATH],
-        "task_dep": ["_download_ui_tool_template"],
         "params": [
             {
                 "name": "tool_name",
                 "long": "tool_name",
                 "type": str,
                 "default": "PlaceholderToolName",
             },
             {
                 "name": "tool_type",
                 "long": "tool_type",
                 "type": str,
-                "default": tool_type_choices[0][0],
+                "default": tool_type_choices[0][1],
                 "choices": tool_type_choices,
             },
             {
                 "name": "tool_config",
                 "long": "tool_config",
                 "type": AyxWorkspaceV1,
-                "default": AyxWorkspaceV1.load()
+                "default": AyxWorkspaceV1.load(),
             },
             {
                 "name": "tool_folder",
                 "long": "tool_folder",
                 "type": str,
                 "default": "PlaceholderToolName_1_0",
-            }
+            },
         ],
         "uptodate": [False],
     }
 
 
-def generate_plugin_code_from_templates(tool_name: str, tool_config: AyxWorkspaceV1) -> None:
+def generate_plugin_code_from_templates(
+    tool_name: str, tool_config: AyxWorkspaceV1
+) -> None:
     """Generate plugin code using the templating engine."""
     TemplateEngine(tool_config.backend_language).generate_plugin(tool_name, tool_config)
 
 
 def build_backend_action(language: BackendLanguage) -> str:
     """Build action to create a plugin."""
     try:
@@ -118,15 +101,17 @@
         }[language]
     except KeyError:
         raise NotImplementedError(f"{language} is not supported as a backend language.")
 
 
 def generate_tool_configuration(tool_folder: str) -> None:
     """Generate default icons for each tool."""
-    tool_config_dir = Path(".") / (TEMPLATE_TOOL_CONFIG_DIR % {"tool_name": tool_folder})
+    tool_config_dir = Path(".") / (
+        TEMPLATE_TOOL_CONFIG_DIR % {"tool_name": tool_folder}
+    )
     tool_config_dir.mkdir()
 
     shutil.copy(
         TEMPLATE_ICON_PATH,
         Path(".") / (TEMPLATE_TOOL_ICON_PATH % {"tool_name": tool_folder}),
     )
 
@@ -134,39 +119,7 @@
 def generate_schemas_dir(tool_folder: str) -> None:
     """Generate DCM Schemas directory for each tool."""
     tool_schemas_dir = DCM_SCHEMAS_DIR / tool_folder
     tool_schemas_dir.mkdir()
     (tool_schemas_dir / "Connections").mkdir()
     (tool_schemas_dir / "Credentials").mkdir()
     (tool_schemas_dir / "DataSources").mkdir()
-
-
-def copy_ui_tool_template(tool_name: str) -> None:
-    """Copy the UI tool template to the new tool location."""
-    shutil.copytree(
-        UI_TEMPLATE_CACHE_DIR,
-        Path(".") / (TEMPLATE_TOOL_UI_DIR % {"tool_name": tool_name}),
-    )
-
-
-def ui_npm_install(tool_name: str) -> None:
-    """Copy the UI tool template to the new tool location."""
-    print("Installing UI components via npm")
-    run_npm(
-        ["install"], cwd=Path(".") / (TEMPLATE_TOOL_UI_DIR % {"tool_name": tool_name})
-    )
-
-
-def git_clone_ui_tool_template(path: Path = UI_TEMPLATE_CACHE_DIR) -> None:
-    """Download the UI template from github to the specified location."""
-    print("Downloading UI components via git")
-    if path.exists():
-        raise FileExistsError("UI Tool template path specified already exists.")
-    path.mkdir(exist_ok=True, parents=True)
-    subprocess.run(["git", "clone", UI_GIT_REPO_URL, path], timeout=100)
-    git_path = path / ".git"
-    for root, dirs, files in os.walk(git_path):
-        for _dir in dirs:
-            os.chmod(Path(root) / _dir, stat.S_IRWXU)
-        for file in files:
-            os.chmod(Path(root) / file, stat.S_IRWXU)
-    shutil.rmtree(git_path)
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_yxi.py

```diff
@@ -26,25 +26,28 @@
     YXI_OUTPUT_DIR,
 )
 from ayx_plugin_cli.ayx_workspace.models.v1 import (
     AyxWorkspaceV1,
     ToolSettingsV1,
 )
 
+from doit import task_params
 
-def task_create_yxi() -> Generator[Dict, None, None]:
+
+@task_params([{"name": "use_ui", "default": False, "type": bool, "long": "use_ui"}])  # type: ignore
+def task_create_yxi(use_ui: bool) -> Generator[Dict, None, None]:
     """Create a YXI from the tools in the workspace."""
     workspace = AyxWorkspaceV1.load()
     backend_artifact_path = Path(
         "main" + AYX_WORKSPACE_ARTIFACT_EXTENSIONS[workspace.backend_language]
     )
 
     yield {
         "file_dep": [backend_artifact_path, AYX_WORKSPACE_JSON_PATH],
-        "task_dep": ["generate_config_files", "generate_artifact"],
+        "task_dep": ["generate_config_files", "generate_ui_artifact", "generate_backend_artifact"] if use_ui else ["generate_config_files", "generate_backend_artifact"],
         "actions": [(create_yxi, [workspace, backend_artifact_path])],
         "targets": [YXI_OUTPUT_DIR / f"{workspace.name}.yxi"],
         "clean": True,
         "name": "create_yxi",
     }
 
 
@@ -64,38 +67,48 @@
     top_level_config = WORKSPACE_CONFIG_DIR / "Config.xml"
     shutil.copy(top_level_config, temp_dir)
     shutil.copy(workspace.package_icon_path, temp_dir)
 
 
 def copy_tool(tool: ToolSettingsV1, temp_dir: Path) -> None:
     """Copy tool files from workspace directory into temp directory for yxi creation."""
-    tool_config_dir = Path(TEMPLATE_TOOL_CONFIG_DIR % {"tool_name": tool.get_tool_folder_name()})
+    tool_config_dir = Path(
+        TEMPLATE_TOOL_CONFIG_DIR % {"tool_name": tool.get_tool_folder_name()}
+    )
     tool_schemas_dir = Path("DcmSchemas") / tool.get_tool_folder_name()
     tool_config_file = tool_config_dir / f"{tool.get_tool_folder_name()}Config.xml"
     tool_config_icon = Path(tool.configuration.icon_path).resolve()
 
     manifest_json = tool_config_dir / "manifest.json"
 
     tool_folder = temp_dir / tool.get_tool_folder_name()
     tool_folder.mkdir()
     shutil.copy(tool_config_file, tool_folder)
     if tool_schemas_dir.exists():
-        shutil.copytree(tool_schemas_dir, tool_folder / "DcmSchemas", dirs_exist_ok=True)
+        shutil.copytree(
+            tool_schemas_dir, tool_folder / "DcmSchemas", dirs_exist_ok=True
+        )
     shutil.copy(manifest_json, tool_folder)
     shutil.copy(tool_config_icon, tool_folder)
 
     tool_ui_artifact_dir = (
-        Path(".") / (TEMPLATE_TOOL_UI_DIR % {"tool_name": tool.backend.tool_class_name}) / "dist"
+        Path(".")
+        / (TEMPLATE_TOOL_UI_DIR % {"tool_name": tool.backend.tool_class_name})
+        / "dist"
     )
-    for path in tool_ui_artifact_dir.iterdir():
-        if path.is_file() and path.suffix != ".gz":
-            shutil.copy(path, tool_folder)
+    if tool_ui_artifact_dir.is_dir():
+        for path in tool_ui_artifact_dir.iterdir():
+            if path.is_file() and path.suffix != ".gz":
+                shutil.copy(path, tool_folder)
 
 
 def make_archive(
     artifact_path: Path, workspace: AyxWorkspaceV1, temp_dir: Path
 ) -> None:
     """Zip workspace and rename to yxi file."""
     YXI_OUTPUT_DIR.mkdir(parents=True, exist_ok=True)
-    shutil.copy(artifact_path, Path(temp_dir) / list(workspace.tools.values())[0].get_tool_folder_name())
+    shutil.copy(
+        artifact_path,
+        Path(temp_dir) / list(workspace.tools.values())[0].get_tool_folder_name(),
+    )
     shutil.make_archive(f"{workspace.name}.yxi", "zip", temp_dir)
     shutil.move(f"{workspace.name}.yxi.zip", YXI_OUTPUT_DIR / f"{workspace.name}.yxi")
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_artifact.py

```diff
@@ -18,25 +18,33 @@
 from ayx_plugin_cli.ayx_workspace.constants import (
     AYX_WORKSPACE_ARTIFACT_EXTENSIONS,
     BUILD_CACHE_DIR,
     BackendLanguage,
     TEMPLATE_TOOL_UI_DIR,
 )
 from ayx_plugin_cli.ayx_workspace.models.v1 import AyxWorkspaceV1
-from ayx_plugin_cli.node_js_helpers import run_npm
+from ayx_plugin_cli.node_js_helpers import NodeHelper
 
 
-def generate_artifact_actions(
-    workspace: AyxWorkspaceV1, backend_artifact_path: Path
+def generate_ui_artifact_actions(
+    workspace: AyxWorkspaceV1
 ) -> List[Any]:
     """Generate the list of actions that generate UI and backend artifacts."""
     all_tools = [tool.backend.tool_class_name for _, tool in workspace.tools.items()]
     return [
-        lambda: print(f"Creating {workspace.name}.yxi..."),
         (_build_action, [all_tools]),
+    ]
+
+
+def generate_backend_artifact_actions(
+    workspace: AyxWorkspaceV1, backend_artifact_path: Path
+) -> List[Any]:
+    """Generate the list of actions that generate UI and backend artifacts."""
+    return [
+        lambda: print(f"Creating {workspace.name}.yxi..."),
         generate_build_artifact_command(
             workspace.backend_language, BUILD_CACHE_DIR, backend_artifact_path
         ),
     ]
 
 
 def generate_build_artifact_command(
@@ -57,38 +65,45 @@
     except KeyError:
         raise NotImplementedError(f"{language} is not supported as a backend language.")
 
 
 def _build_action(all_tools: List[str]) -> None:
     for tool_name in all_tools:
         ui_dir = TEMPLATE_TOOL_UI_DIR % {"tool_name": tool_name}
-        completed_process = run_npm(["install"], cwd=Path(".") / ui_dir,)
-        if completed_process.returncode != 0:
-            raise RuntimeError(
-                f"'npm install' on directory {ui_dir} failed with:\n"
-                f"stdout:\n{completed_process.stdout}\n\n"
-                f"stderr:{completed_process.stderr}"
-            )
-        completed_process = run_npm(["run", "build"], cwd=Path(".") / ui_dir,)
+        if not Path(ui_dir).is_dir():
+            continue
 
+        completed_process = NodeHelper.run_npm(
+            "run", "build", cwd=Path(".") / ui_dir,
+        )
         if completed_process.returncode != 0:
             raise RuntimeError(
                 f"'npm run build' on directory {ui_dir} failed with:\n"
                 f"stdout:\n{completed_process.stdout}\n\n"
                 f"stderr:{completed_process.stderr}"
             )
 
 
-def task_generate_artifact() -> Generator[Dict, None, None]:
+def task_generate_ui_artifact() -> Generator[Dict, None, None]:
+    """Create ui artifact from the tools in the workspace."""
+    workspace = AyxWorkspaceV1.load()
+    yield {
+        "task_dep": ["generate_config_files", "generate_ui"],
+        "actions": generate_ui_artifact_actions(workspace),
+        "name": "build_ui_artifacts",
+    }
+
+
+def task_generate_backend_artifact() -> Generator[Dict, None, None]:
     """Create a language-specific backend artifact from the tools in the workspace."""
     workspace = AyxWorkspaceV1.load()
     backend_artifact_path = Path(
         "main" + AYX_WORKSPACE_ARTIFACT_EXTENSIONS[workspace.backend_language]
     )
 
     yield {
         "task_dep": ["generate_config_files"],
-        "actions": generate_artifact_actions(workspace, backend_artifact_path),
+        "actions": generate_backend_artifact_actions(workspace, backend_artifact_path),
         "targets": [backend_artifact_path],
         "clean": True,
-        "name": "build_artifacts",
+        "name": "build_backend_artifacts",
     }
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py

```diff
@@ -139,16 +139,16 @@
                     "@EngineDllEntryPoint": "SdkEnginePlugin",
                     "@SDKVersion": "10.1",
                 },
                 "SdkSettings": {
                     "@Manifest": "True",
                     "@Language": "Python",
                     "CustomParameters": {
-                        "Version": {"@Value": short_version, },
-                        "ToolVersion": {"@Value": tool_config.version, },
+                        "Version": {"@Value": short_version},
+                        "ToolVersion": {"@Value": tool_config.version},
                     },
                 },
                 "GuiSettings": {
                     "@Html": "index.html",
                     "@Icon": tool_config.icon_path.name,
                     "@SDKVersion": "10.1",
                     "@Help": tool_config.help_url,
@@ -168,21 +168,27 @@
                         "Company": workspace.company,
                         "Copyright": workspace.copyright,
                     }
                 },
             }
         }
 
-        config_xml_path = WORKSPACE_CONFIG_DIR / tool.get_tool_folder_name() / f"{tool.get_tool_folder_name()}Config.xml"
+        config_xml_path = (
+            WORKSPACE_CONFIG_DIR
+            / tool.get_tool_folder_name()
+            / f"{tool.get_tool_folder_name()}Config.xml"
+        )
         _output_dict_to_xml(config_xml, config_xml_path)
 
     print("Done!")
 
 
-def generate_desktop_manifest(tool_name: str, entrypoint: str, tool_folder_name: str) -> None:
+def generate_desktop_manifest(
+    tool_name: str, entrypoint: str, tool_folder_name: str
+) -> None:
     """Generate a manifest file for Designer Desktop."""
     print(f"Generating manifest.json for {tool_name}...")
     manifest = ManifestV1(
         version="3.8",
         entry_point=Path(entrypoint) / f"main.pyz",
         tool_package="ayx_plugins",
         tool_name=tool_name,
@@ -225,15 +231,17 @@
 def generate_manifest_jsons() -> None:
     """Parse the ayx_workspace.json to generate the manifest.json that corresponds to each tool."""
     workspace = AyxWorkspaceV1.load()
     tools = workspace.tools
 
     entrypoint = tools[list(tools.keys())[0]].get_tool_folder_name()
     for _, tool in tools.items():
-        generate_desktop_manifest(tool.backend.tool_class_name, entrypoint, tool.get_tool_folder_name())
+        generate_desktop_manifest(
+            tool.backend.tool_class_name, entrypoint, tool.get_tool_folder_name()
+        )
 
     print("Done!")
 
 
 def _get_runtime_from_language(language: str, tool_name: str) -> Runtime:
     runtimes = {
         "python": Runtime(
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py

```diff
@@ -19,32 +19,30 @@
 from ayx_plugin_cli.ayx_workspace.template_engine import TemplateEngine
 
 
 def task_generate_tests() -> Dict:
     """Generate tests for a specified tool."""
     return {
         "title": lambda task: "Generate tests",
-        "actions": [
-            generate_tests
-        ],
+        "actions": [generate_tests],
         "file_dep": [AYX_WORKSPACE_JSON_PATH],
         "params": [
             {
                 "name": "tool_name",
                 "long": "tool_name",
                 "type": str,
                 "default": "PlaceholderToolName",
             },
             {
                 "name": "tool_config",
                 "long": "tool_config",
                 "type": AyxWorkspaceV1,
-                "default": AyxWorkspaceV1.load()
-            }
+                "default": AyxWorkspaceV1.load(),
+            },
         ],
-        "uptodate": [False]
+        "uptodate": [False],
     }
 
 
 def generate_tests(tool_name: str, tool_config: AyxWorkspaceV1) -> None:
     """Generate unit tests for a plugin."""
     TemplateEngine(tool_config.backend_language).generate_tests(tool_name, tool_config)
```

## ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py

```diff
@@ -15,15 +15,14 @@
 import os
 import shutil
 import sys
 from pathlib import Path
 from typing import Dict, Generator
 
 from ayx_plugin_cli.ayx_workspace.constants import (
-    AYX_CLI_UI_TEMPLATE,
     AYX_CLI_WORKSPACE_FILES_PATH,
     AYX_WORKSPACE_FILES,
     AYX_WORKSPACE_JSON_PATH,
     DCM_SCHEMAS_DIR,
     TESTS_DIR,
     WORKSPACE_CONFIG_DIR,
 )
@@ -98,20 +97,14 @@
     yield {
         "name": "tests",
         "title": lambda task: "Create tests directory",
         "actions": [(create_directory, [TESTS_DIR])],
         "targets": [TESTS_DIR],
     }
 
-    yield {
-        "name": "ui",
-        "title": lambda task: "Initialize UI",
-        "actions": [(initialize_ui, [Path("ui")])],
-    }
-
 
 def create_config_directory(path: Path) -> None:
     """Create the config directory."""
     create_directory(path)
     _write_package_icon(path / "default_package_icon.png")
 
 
@@ -139,12 +132,7 @@
     """Initialize the backend workspace using ayx_workspace.json."""
     if workspace_info.backend_language == BackendLanguage.Python:
         return f"ayx_python_sdk init-workspace --workspace-directory {os.getcwd()} --y"
     else:
         raise NotImplementedError(
             f"{workspace_info.backend_language} is not a supported backend."
         )
-
-
-def initialize_ui(path: Path) -> None:
-    """Initialize the UI directory."""
-    shutil.copytree(AYX_CLI_UI_TEMPLATE, path)
```

## Comparing `ayx_plugin_cli-1.0.4.dist-info/LICENSE` & `ayx_plugin_cli-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ayx_plugin_cli-1.0.4.dist-info/RECORD` & `ayx_plugin_cli-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ayx_plugin_cli/__init__.py,sha256=gImMP7_Q5qUg3ZLWaUx8BZNAgRWsmh532R4hGWQYCU4,642
-ayx_plugin_cli/__main__.py,sha256=C04thlaXaLAOtAE3aBE5w5HxsLXn7RtHy-Yok6rE-ds,17023
+ayx_plugin_cli/__main__.py,sha256=nIuCzec3MOBGH7HKpo2_X-q_ORbp-FKsx9JwZ5P9DLo,18505
 ayx_plugin_cli/exceptions.py,sha256=SGAyQ9oH6hYaHEp2tk3C8chI1x-a7JMtYio10Nlv230,836
-ayx_plugin_cli/node_js_helpers.py,sha256=FZcGJ7yoc1wf3SoTy65EEJWViEID24Bny489UcWA708,1609
-ayx_plugin_cli/validation.py,sha256=k0V3k9tD9zk0TFtVP_LSl00vz6oycSuPG7I8aEr_vaE,6745
-ayx_plugin_cli/version.py,sha256=a2bcsfSMkk80Bp6L34szFZ6ScVcDdQOeTumSfDmMpH0,218
+ayx_plugin_cli/node_js_helpers.py,sha256=VZfZk7IBrO5BeOf1-p_okdR4pEu9PbOU4x9WxVstr1Q,1832
+ayx_plugin_cli/validation.py,sha256=E7JcMGo6SKLURSCCz8PeBJz8cCdjfQNJ9abAUpy-5Js,6992
+ayx_plugin_cli/version.py,sha256=6hm6-D-WWiiag_aJIUBO-gs_38x3ax3gBbsRlKO8S4g,218
 ayx_plugin_cli/assets/__init__.py,sha256=4c-S87I-ya60huSl_zaKBqyE93Rc88HSW32Kd0WX8MQ,640
 ayx_plugin_cli/assets/templates/python/README_tests.md,sha256=fOmeKqOQM7ImPyVVBHhSvFht_gBV5y-ckpnM-ge76Zg,7497
 ayx_plugin_cli/assets/templates/python/__init__.j2,sha256=GfHjiAM2Hlhgi-Gv21dJqzCGdGixqdxh4z6nYYFam5A,782
 ayx_plugin_cli/assets/templates/python/clean_plugin_tests.j2,sha256=Vs4-yYMzz76JD6TPg3u1jQaBwfYbIcof1jQ--Op_72M,9731
 ayx_plugin_cli/assets/templates/python/plugin.j2,sha256=IE6b3BZlUvrr7mI45n5q_db0dVOG9HUykXXEgYJiGz8,6523
 ayx_plugin_cli/assets/templates/python/plugin_tests.j2,sha256=x52gpqGQmNCp504M7sIJcR1qb5Gj4PDSRe77cBiC8Cc,9067
 ayx_plugin_cli/assets/templates/python/requirements-local.j2,sha256=zbTuKuppzGqDMxu-ltwsqpopnSEynvsDNvwCqC4YOag,1
@@ -19,31 +19,33 @@
 ayx_plugin_cli/assets/templates/python/macros/multi_output.j2,sha256=E8UpbFixcFk3JtVUMPQDojuZoNHQZwMIS8xaMXPOSmA,2210
 ayx_plugin_cli/assets/templates/python/macros/optional.j2,sha256=2qUjl9VEFyT0x98wr7NbdsIdzTLXaBgLbQK4rELI_po,1965
 ayx_plugin_cli/assets/templates/python/macros/output.j2,sha256=KFl9UZs6w8nJDuLSXzreRwteKtNbwTW77xDZZXM13u8,1366
 ayx_plugin_cli/assets/templates/python/macros/passthrough.j2,sha256=cXhpMlMHVsIA3PaYIJjOyjd8zLIJMBrqusHoZkwx2uc,1351
 ayx_plugin_cli/assets/workspace_files/.gitignore,sha256=Cot2-C_azHSFz0tJ7IvaPMPAMqUCtIG1Ha-NA527aRc,8
 ayx_plugin_cli/assets/workspace_files/README.md,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ayx_plugin_cli/assets/workspace_files/default_package_icon.png,sha256=oQ8p_fO6rXW2Mwpp2pNxKFKXkcUIz6Z83G6yHovluu8,12141
+ayx_plugin_cli/assets/workspace_files/ui_artifact.zip,sha256=-fAvTC_Nxq9GPJwJlAqJsZzq4B1c2zBMWLZCeYpJHs8,118540
 ayx_plugin_cli/assets/workspace_files/ui_template/README.md,sha256=nvvFjatdAVdRuG8DvQdKZAM99h6sRwDkwHlwYI2Y_u0,774
 ayx_plugin_cli/ayx_workspace/__init__.py,sha256=f7HgNcP8lEiq3POXYUcMd4Xy3jUenu7oTXFir75qWdY,664
-ayx_plugin_cli/ayx_workspace/constants.py,sha256=iYnuszJUhPDS4cg3vdTYoVEY187sxQvjX6UWlX_A2mc,2770
+ayx_plugin_cli/ayx_workspace/constants.py,sha256=SLjcTXgsaeoKCVCyx7xSAW6qK-PByA_-CRe-S5eKjlk,2833
 ayx_plugin_cli/ayx_workspace/template_engine.py,sha256=Hrli7KTXoH0xFZWYIfr6dUwBkh2jULuJPnUOkPc7H0M,7379
 ayx_plugin_cli/ayx_workspace/template_tool_settings.py,sha256=2w7VPKDQh25ndIXB5F9PGuzgFnkHoDi_yh0HtY5T3c4,3307
 ayx_plugin_cli/ayx_workspace/doit/__init__.py,sha256=6ujru9HbPidMhUnUo20NNjNvfyDuOnVq1pENHTgxsDE,648
 ayx_plugin_cli/ayx_workspace/doit/dodo.py,sha256=ZHVwWK4ETnhQzGkth0xqQ0Wmdbr3aj9KZdsxnadnKyA,1291
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/__init__.py,sha256=vFXlmTieqX9X9yVG2_CxTw6ug1coCf8PJNzdaydtufU,1281
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_plugin.py,sha256=okCqgrjpUoK4l7JIm_churSkhr9jmEWvqjKefhrkUjo,5859
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_yxi.py,sha256=8r_5PFAtbiLshEKUOFDx7K-0iRAoHmRGucW8_g1AYZA,4093
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_artifact.py,sha256=6I1Ch4MGZeOmGE1S7s1HbIcEGU6HEJ608BYqgT-XdfM,3603
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py,sha256=ePJUxU01Po3_gehYQ5Sr73BYL9IrTC3u-L_tVb0LZWw,11183
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py,sha256=SjxKXxikfbpVgd83jnkErEvxSRL-0dcK6EC10HCF8so,1799
-ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py,sha256=c_gQMoCJb2Hef05-oHUcaVuy2hTFTqFC9nnaw4vSbHo,4469
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/__init__.py,sha256=B-v9iZlUWZjG0vcrKjxRPWsmQJ6YymSmIhuutpfrC7c,1419
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_plugin.py,sha256=kV3zu2skP7YpDsx-b6JpHrfGglULBVGIL-pW9eAvXSA,4091
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/create_yxi.py,sha256=cWwhRwQDWskbBiOTArQlknEZMdKCSmxqH23f1y9dWGw,4463
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_artifact.py,sha256=1MBGMQQ5e3TqAA9ftOiOoqCHrbKWSRG5F12V7FticZk,3904
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_config_files.py,sha256=FNfhY5UaY_qtTUncO90n2XbF82Z-vPc2dxcOwLIFuVM,11255
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_tests.py,sha256=CfPAzWBbktSBQst8JKWRRbODbCbNDMb99TZ24ZOsWKo,1780
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/generate_ui.py,sha256=_9iedwnuCLU3cCL7Ure3yjXFnE_81wgHFUDhOQrN34c,2796
+ayx_plugin_cli/ayx_workspace/doit/build_tasks/initialize_workspace.py,sha256=oGiqQLQLQcVB3JDQ-S7HMR_UI2xUuXKRnoidopMe2sk,4177
 ayx_plugin_cli/ayx_workspace/doit/build_tasks/install_yxi.py,sha256=zRwy_vNfqz2OlD9VcBmOweTPOPF8MXtAEsW1uWQNAvU,2303
 ayx_plugin_cli/ayx_workspace/models/__init__.py,sha256=uzlJdEHaBh6fj2vXW_jA5glHqu9dS9LGdw5QFmjW0rU,655
 ayx_plugin_cli/ayx_workspace/models/cloud_manifest.py,sha256=X44huXMoiPH79XLMS-S4Yy6XLf4-O6h3ojr_Cap_cvE,4455
 ayx_plugin_cli/ayx_workspace/models/v1.py,sha256=NWDZ_CA-PCOQKbdD0Vx7xrDq2xMufdYk7bNNbrbj7EE,4941
-ayx_plugin_cli-1.0.4.dist-info/LICENSE,sha256=5rzFyimk4IDNUaoytK0rupETUnATLze0EMsFBjHezkY,22092
-ayx_plugin_cli-1.0.4.dist-info/METADATA,sha256=cgYe_FuagrRJGmOnmGhCIWtZNBYxqNVyudLxo65vYd8,1769
-ayx_plugin_cli-1.0.4.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-ayx_plugin_cli-1.0.4.dist-info/entry_points.txt,sha256=M_EJ6fdhk8yQ7cjIu0cDsT7zs32YnLzzuQ28qX0CXkM,95
-ayx_plugin_cli-1.0.4.dist-info/top_level.txt,sha256=kED56nFirgbz_nv1Ksu-YATwuEPVtTy4-ACFK1-3bHk,15
-ayx_plugin_cli-1.0.4.dist-info/RECORD,,
+ayx_plugin_cli-1.1.0.dist-info/LICENSE,sha256=5rzFyimk4IDNUaoytK0rupETUnATLze0EMsFBjHezkY,22092
+ayx_plugin_cli-1.1.0.dist-info/METADATA,sha256=dZjDnyDtTKt_AcretX3co6Y4jWMksZQVk3NANl2BbSM,1799
+ayx_plugin_cli-1.1.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+ayx_plugin_cli-1.1.0.dist-info/entry_points.txt,sha256=9ri_MqWKVaX3upi6uwFFK5bopMJTrHekghWw-Y5PgYQ,64
+ayx_plugin_cli-1.1.0.dist-info/top_level.txt,sha256=kED56nFirgbz_nv1Ksu-YATwuEPVtTy4-ACFK1-3bHk,15
+ayx_plugin_cli-1.1.0.dist-info/RECORD,,
```

