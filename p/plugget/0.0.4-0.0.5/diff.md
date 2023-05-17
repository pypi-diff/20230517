# Comparing `tmp/plugget-0.0.4.tar.gz` & `tmp/plugget-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget-0.0.4.tar", last modified: Mon Mar 27 13:45:14 2023, max compression
+gzip compressed data, was "plugget-0.0.5.tar", last modified: Wed May 17 21:21:50 2023, max compression
```

## Comparing `plugget-0.0.4.tar` & `plugget-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.382008 plugget-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.378008 plugget-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.378008 plugget-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-27 13:44:52.000000 plugget-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-03-27 13:44:52.000000 plugget-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-27 13:45:14.382008 plugget-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-27 13:44:52.000000 plugget-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.378008 plugget-0.0.4/plugget/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.382008 plugget-0.0.4/plugget/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/blender_addon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/blender_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/blender_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/krita_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/krita_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/actions/max_macroscript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.382008 plugget-0.0.4/plugget/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/apps/blender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.382008 plugget-0.0.4/plugget/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.382008 plugget-0.0.4/plugget/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-27 13:44:52.000000 plugget-0.0.4/plugget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:45:14.378008 plugget-0.0.4/plugget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-27 13:45:14.000000 plugget-0.0.4/plugget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 13:45:14.000000 plugget-0.0.4/plugget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:45:14.000000 plugget-0.0.4/plugget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 13:45:14.000000 plugget-0.0.4/plugget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 13:45:14.000000 plugget-0.0.4/plugget.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-27 13:44:52.000000 plugget-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 13:44:52.000000 plugget-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 13:45:14.382008 plugget-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-27 13:44:52.000000 plugget-0.0.4/testcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.078225 plugget-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-17 21:21:38.000000 plugget-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-17 21:21:38.000000 plugget-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-17 21:21:50.086225 plugget-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-17 21:21:38.000000 plugget-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/blender_addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/blender_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/krita_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/krita_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/max_macroscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/unreal_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/actions/unreal_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/apps/blender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/data/packages_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/github/async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.086225 plugget-0.0.5/plugget/gumroad/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/gumroad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 21:21:38.000000 plugget-0.0.5/plugget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:21:50.082225 plugget-0.0.5/plugget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 21:21:50.000000 plugget-0.0.5/plugget.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-17 21:21:38.000000 plugget-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 21:21:38.000000 plugget-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:21:50.086225 plugget-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-17 21:21:38.000000 plugget-0.0.5/testcode.py
```

### Comparing `plugget-0.0.4/.github/workflows/python-publish.yml` & `plugget-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/.gitignore` & `plugget-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/PKG-INFO` & `plugget-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.4
+Version: 0.0.5
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
-# PlugGet
+<h1>
+<img src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" data-canonical-src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" width="70" />
+Plugget: Plugin Package Manager
+</h1>
 
 [![PyPI Downloads](https://img.shields.io/pypi/v/plugget?color=0)](https://pypi.org/project/plugget/)
 
 Install app packages (plugins, addons, icons, ...) from a repo with a single Python command: 
 ```python
 import plugget
 plugget.install("my_package")
 ```
 
 ![machinetoolsinstall](https://user-images.githubusercontent.com/3758308/227316999-adf32b7f-4232-46f5-b0db-1b3dbe26d755.gif)
 
 also check out
 - [plugget blender addon](https://github.com/hannesdelbeke/plugget-blender-addon)
 - [plugget manifest repo](https://github.com/hannesdelbeke/plugget-pkgs)
+- [plugget unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)
 
 ## requirements
 - pip installed
 - git installed
 (aim to auto handle requirements in future)
 
 ## not to confuse with
```

### Comparing `plugget-0.0.4/README.md` & `plugget-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# PlugGet
+<h1>
+<img src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" data-canonical-src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" width="70" />
+Plugget: Plugin Package Manager
+</h1>
 
 [![PyPI Downloads](https://img.shields.io/pypi/v/plugget?color=0)](https://pypi.org/project/plugget/)
 
 Install app packages (plugins, addons, icons, ...) from a repo with a single Python command: 
 ```python
 import plugget
 plugget.install("my_package")
 ```
 
 ![machinetoolsinstall](https://user-images.githubusercontent.com/3758308/227316999-adf32b7f-4232-46f5-b0db-1b3dbe26d755.gif)
 
 also check out
 - [plugget blender addon](https://github.com/hannesdelbeke/plugget-blender-addon)
 - [plugget manifest repo](https://github.com/hannesdelbeke/plugget-pkgs)
+- [plugget unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)
 
 ## requirements
 - pip installed
 - git installed
 (aim to auto handle requirements in future)
 
 ## not to confuse with 
@@ -32,8 +36,8 @@
 
 ## manifest repo
 - package manifests live in the [manifest repo](https://github.com/hannesdelbeke/plugget-pkgs)
 
 ## issues
 If the install fails. It likely is a bad manifest, a bad install, or a bug with Plugget.
 Report the issue in issues.
-There's a small chance the GitHub servers are down, you can check the [github status](https://www.githubstatus.com/).
+There's a small chance the GitHub servers are down, you can check the [github status](https://www.githubstatus.com/).
```

### Comparing `plugget-0.0.4/plugget/actions/_template.py` & `plugget-0.0.5/plugget/actions/_template.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/plugget/actions/blender_addon.py` & `plugget-0.0.5/plugget/actions/blender_addon.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/plugget/actions/blender_module.py` & `plugget-0.0.5/plugget/apps/blender.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,91 @@
+import bpy
+import addon_utils
+from pathlib import Path
+import shutil
+import logging
+
+
 """
-install a python module from a repo to the blender module folder
+Blender plugins are named addons
+addons in Blender are folders of scripts, and can be enabled/disabled
 """
 
-from pathlib import Path
-import logging
-import shutil
-import bpy
 
+def is_installed(name):
+    """check if plugin is installed, use plugin_name from manifest, checking folder name in addons"""
+    local_script_dir = bpy.utils.script_path_user()
+    local_addons_dir = Path(local_script_dir) / "addons"
+    return (local_addons_dir / name).exists()
 
-# todo merge dupe code
-def default_plugin_name(package_url, repo_url):
-    """
-    use the repo name as the default plugin name
-    e.g. https://github.com/SavMartin/TexTools-Blender -> TexTools-Blender
-    """
-    if package_url:
-        return package_url.rsplit("/", 1)[1].split(".")[0]
-    else:
-        return repo_url.rsplit("/", 1)[1].split(".")[0]
 
+def installed_plugins():
+    """return list of installed plugins"""
+    # Blender names returned are from the operator, but plugin_name in the manifest refers to the blender folder name
+    # todo ideally we return a name thats useable in the pluggest install commands
+    return [mod.bl_info.get("name") for mod in addon_utils.modules()]
 
-def __clash_import_name(name):
-    """check there isn't a py module with the same name as our addon"""
-    try:
-        __import__(name)
-        logging.warning(f"Failed to install addon {name}, a py module with same name exists")
-        return True
-    except ImportError:
-        return False
 
+def enabled_plugins() -> list[str]:
+    """return list of enabled plugins"""
+    # Blender names returned are from the operator, but plugin_name in the manifest refers to the blender folder name
+    # todo ideally we return a name thats useable in the pluggest install commands
+    return bpy.context.preferences.addons.keys()
 
-def install(package: "plugget.data.Package", force=False, enable=True, **kwargs) -> bool:  # todo , force=False, enable=True):
-    # If the “force” parameter is True, the add-on will be reinstalled, even if it has not been previously removed.
 
-    # foldername and addon (operator) name are different!
-    # operator name is tracked in plugin_name in manifest
+def disabled_plugins() -> list[str]:
+    """return list of disabled plugins"""
+    # Blender names returned are from the operator, but plugin_name in the manifest refers to the blender folder name
+    # todo ideally we return a name thats useable in the pluggest install commands
+    return [p for p in installed_plugins() if p not in enabled_plugins()]
 
-    # if a repo has plugin in root. we get the repo files content
-    # if the repo has plugin in subdir, that file lives in repo_paths
 
-    addon_paths: list[Path] = package.get_content()  # get paths to plugin files in cloned repo
-    # copy addons to local addons dir
-    local_script_dir = Path(bpy.utils.script_path_user())
-    local_modules_dir = Path(local_script_dir) / "addons/modules"
-    # if force:
-    #     from plugget.utils import rmdir
-    #     rmdir(new_plugin_path)
-    # shutil.move(str(plugin_path), str(new_plugin_path.parent), )  # copy plugin_path to local_addons_dir
-    # todo filter repo paths
-    for addon_path in addon_paths:
-
-        if __clash_import_name(addon_path.name):
-            continue
-
-        new_addon_path = local_modules_dir / addon_path.name
-        # new_addon_path.mkdir(parents=True, exist_ok=True)
-        # from plugget.utils import rmdir
-        # rmdir(local_modules_dir / addon_path.name)
-        shutil.move(str(addon_path), str(local_modules_dir))
-
-        # todo clean up empty folders
-
-        # check if plugin folder was copied, by checking if any files are in new_plugin_path
-        if not any(new_addon_path.iterdir()):
-            logging.warning(f"Failed to install plugin {addon_path.name}")
-            return False
-
-    # if enable:
-    #     addon_name = package.plugin_name or default_plugin_name(package.package_url, package.repo_url)
-    #     if not addon_name:
-    #         raise ValueError(f"No plugin name found for package '{package.package_name}'")
-    #     bpy.ops.preferences.addon_enable(module=addon_name)
+def disable_plugin(name):
+    """disable plugin by name"""
+    bpy.ops.preferences.addon_disable(module=name)
 
-    return True
 
+def enable_plugin(name):
+    """enable plugin by name"""
+    bpy.ops.preferences.addon_enable(module=name)
 
-def uninstall(package: "plugget.data.Package", **kwargs):
+
+def install_plugin(plugin_paths: list[Path]) -> bool:  # todo , force=False, enable=True):
+    """install plugin from path"""
+    # If the “overwrite” parameter is True, the add-on will be reinstalled, even if it has not been previously removed.
+
+    # manifest is named io_xray
+    # but subdir is io_scene_xray
+    # resulting in clashes. we cant just rename the subdir, might break code inside.
+    # so we need to track the "name" with plugin_name in the manifest
+
+    # todo fix only support 1 plugin
+    plugin_path = plugin_paths[0]
+    if len(plugin_paths) > 1:
+        raise NotImplemented("Only 1 plugin can be installed at a time for now")
+
+    local_script_dir = bpy.utils.script_path_user()
+    local_addons_dir = Path(local_script_dir) / "addons"
+    new_plugin_path = local_addons_dir / plugin_path.name
+    shutil.move(str(plugin_path), str(new_plugin_path.parent))  # copy plugin_path to local_addons_dir
+
+    # check if plugin folder was copied, by checking if any files are in new_plugin_path
+    if not any(new_plugin_path.iterdir()):
+        logging.warning(f"Failed to install plugin {plugin_path.name}")
+        return False
+    else:
+        return True
+
+
+def uninstall_plugin(name):
     """uninstall plugin by name"""
-    # todo make plugin name an action kwarg
-    pass
-    # plugin_name = package.plugin_name or default_plugin_name(package.package_url, package.repo_url)
-    # bpy.ops.preferences.addon_remove(module=plugin_name)
-    # print("PLUGGET uninstalled plugin_name ", plugin_name)
+    if not name:
+        logging.warning("No plugin name given")
+        return
+    bpy.ops.preferences.addon_remove(module=name)
+
+
+def open_install_dir():
+    """Open the directory where plugins are installed"""
+    local_script_dir = bpy.utils.script_path_user()
+    local_addons_dir = Path(local_script_dir) / "addons"
+    bpy.ops.wm.path_open(filepath=str(local_addons_dir))
```

### Comparing `plugget-0.0.4/plugget/actions/blender_pip.py` & `plugget-0.0.5/plugget/actions/blender_pip.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/plugget/actions/krita_pip.py` & `plugget-0.0.5/plugget/actions/krita_pip.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/plugget/actions/krita_plugin.py` & `plugget-0.0.5/plugget/actions/krita_plugin.py`

 * *Files identical despite different names*

### Comparing `plugget-0.0.4/plugget/commands/__init__.py` & `plugget-0.0.5/plugget/commands/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """
 Plugget is a plugin-manager for various applications.
 """
-import importlib
 import logging
 import subprocess
 import datetime
-import os
 import pprint
-from pathlib import Path
-import shutil
 
 from plugget.utils import rmdir
-from plugget.data import Package
+from plugget.data import Package, PackagesMeta
 from plugget import settings
-import detect_app
+
+from pathlib import Path
 
 
 # plugget / cache
 # plugget / installed / blender / io_xray.
 
 
 # def _plugin_name_from_manifest(package_name):
@@ -28,34 +25,37 @@
 #         package = search(package_name, verbose=False)[0]
 #         print("found plugin name from manifest", package.package_name)
 #         plugin_name = package.plugin_name
 #
 #         return plugin_name
 
 
-def _clone_manifest_repo(source_url):
+def _clone_manifest_repo(source_url) -> "pathlib.Path":
+    """clone git repo containing plugget manifests, from a git URL"""
     source_name = source_url.split("/")[-1].split(".")[0]
     source_dir = settings.TEMP_PLUGGET / source_name
 
     # CACHING: check when repo was last updated
     if (source_dir / "_LAST_UPDATED").exists():
         with open(source_dir / "_LAST_UPDATED", "r") as f:
             last_updated = datetime.datetime.strptime(f.read(), "%Y-%m-%d %H:%M:%S")
         if last_updated > datetime.datetime.now() - datetime.timedelta(days=1):
             print("using cached manifest repo, last updated less than a day ago")
             return source_dir
 
+    # remove old manifest repo
     rmdir(source_dir)  # todo catch if this failed
-
     # check if dir exists
     if source_dir.exists():
         raise Exception(f"Failed to remove source_dir {source_dir}")
 
     # clone repo
     subprocess.run(["git", "clone", "--depth", "1", "--progress", source_url, str(source_dir)])
+    # todo check if command errored / catch exception
+    # todo check if clone was successful
 
     # CACHING: make a file inside named _LAST_UPDATED with the current date
     source_dir.mkdir(parents=True, exist_ok=True)
     with open(source_dir / "_LAST_UPDATED", "w") as f:
         f.write(datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
 
     return source_dir
@@ -64,107 +64,111 @@
 def _clone_manifest_repos():
     """
     clone the manifest repos that are registered, defaults to ['github.com/hannesdelbeke/plugget-pkgs']
     """
     # if repo doesn't exist, clone it
     source_dirs = []
     for source_url in settings.sources:
-        source_dir = _clone_manifest_repo(source_url)
-        source_dirs.append(source_dir)
-    return source_dirs
 
+        # first check if path is a local path
+        source_dir = Path(source_url)
+        if not source_dir.exists():  # todo fix this naive impicit approach
+            # else assume it's a git URL
+            source_dir = _clone_manifest_repo(source_url)
+
+        source_dirs.append(source_dir)
 
-def _add_repo(repo_url):
-    settings.sources.append(repo_url)
-    # TODO save to config file
+    return source_dirs
 
 
 def _detect_app_id():
-    app = None
-    if not app:
-        app_found = detect_app.detect_app()
-        return app_found.id if app_found else None
+    try:
+        import detect_app
+        app = None
+        if not app:
+            app_found = detect_app.detect_app()
+            return app_found.id if app_found else None
+    except:
+        None
 
 
-def search(name=None, app=None, verbose=True):
+def search(name=None, app=None, verbose=True, version=None, source_dirs=None):
     """
     search if package is in sources
     :param name: pacakge name to search in manifest repo, return all packages if not set
     :param app: app name to search in, return all apps if not set
     :param verbose: print results if True
     """
 
+    # todo curr returns package and version
+    #  return package meta. latest, name, author, description
+    #  search will return all package names, and then plugin needs to read all versions from this package name.
+    #  ideally i can do .versions
+
     app = _detect_app_id() if not app else app
 
     plugins = []
-    source_dirs = _clone_manifest_repos()
+    source_dirs = source_dirs or _clone_manifest_repos()
     for source_dir in source_dirs:  # go through all cloned manifest repos
-        if app and app != 'all':  # filter by app
+
+        # filter by app
+        if app and app != 'all':
             source_dir = source_dir / app
-        for plugin_manifest in source_dir.rglob("*.json"):
-            source_name = plugin_manifest.parent.name  # this checks for manifest name, not name in package todo
-            if name is None or name.lower() in source_name.lower():
-                plugins.append(Package.from_json(plugin_manifest))
+
+        # todo correctly parse if app is all or None
+        
+        # go through folders
+        for _path in source_dir.glob("*"):
+
+            # ensure we iter folders and not files
+            if not _path.is_dir():
+                continue
+            package_dir = _path
+
+            # create a packages meta to collect all versions
+            meta = PackagesMeta()
+
+            # iter through jsons in folder
+            for plugin_manifest in package_dir.rglob("*.json"):
+                source_name = package_dir.name  # this checks for manifest name, not name in package todo
+                if name is None or name.lower() in source_name.lower():
+                    meta.packages.append(Package.from_json(plugin_manifest))
+
+            # if package meta contains any packages, we add it to search results
+            if meta.packages:
+                plugins.append(meta)
 
     if verbose:
         print(f"{len(plugins)} plugins found in repo:")
         print(f"{'-' * 20}")
         for plugin in plugins:
             print(f"{plugin}")
+
     return plugins
 
 
 # # WARNING we overwrite build in type list here, careful when using list in this module!
 # open package manager
+# todo do we need this or can this be mergeed w search
 def list(package_name:str = None, enabled=False, disabled=False, verbose=True, app=None):  # , source=None):
     """
     list all installed packages
     if run from an app, only list the apps installed packages, with option to list all app installed packages
 
     :param enabled: list enabled packages only if True
     :param disabled: list disabled packages only if True
     TODO :param source: list packages from specific source only if set
     """
-    # todo print installed packages in INSTALLED_DIR, instead of app plugins
+    results = search(name=package_name, app=app, verbose=verbose, source_dirs=[settings.INSTALLED_DIR])
 
-    # module = _get_app_module()
-
-    # if enabled:
-    #     plugins = module.enabled_plugins()
-    # elif disabled:
-    #     plugins = module.disabled_plugins()
-    # else:  # list all installed
-    #     plugins = module.installed_plugins()
-
-    # list all installed in settings.INSTALLED_DIR
-    plugins = []
-    app = _detect_app_id() if not app else app
-
-    if app and app != "all":
-        app_manifest_dir = settings.INSTALLED_DIR / app
-    else:
-        app_manifest_dir = settings.INSTALLED_DIR
-
-    for plugin_manifest in app_manifest_dir.rglob("*.json"):
-        package = Package.from_json(plugin_manifest)
-        if package_name and package_name.lower() not in package.package_name.lower():  #  plugin_manifest.parent.name.lower():
-            continue
-        plugins.append(package)
-
-    if verbose:
-        print(f"{len(plugins)} installed plugins")
-        print(f"{'-' * 20}")
-        for plugin in plugins:
-            print(f"{plugin}")
-
-    return plugins
+    return results
 
 
 #    plugin_name = plugin_name or plugin_name_from_manifest(package_name)
-def install(package_name, enable=True, app=None, **kwargs):
+def install(package_name, enable=True, app=None, version=None, **kwargs):
     """
     install package
     :param name: name of the manifest folder in the manifest repo
     :param enable: enable plugin after install
     """
     # todo
     #  get package (manifest)
@@ -172,15 +176,17 @@
     #  install package, by running action(s) from manifest
     #  save manifest to installed packages dir
 
     # copy package to blender package folder
     # module = _get_app_module()
 
     # get package manifest from package repo
-    package = search(name=package_name, app=app, verbose=False)[0]
+    meta_collection = search(name=package_name, app=app, verbose=False, version=version)[0]
+    package = meta_collection.get_version(version)
+
     if not package:
         logging.warning("Package not found, cancelling install")
         return
 
     package.install(enable=enable, **kwargs)
     # uninstall if unsuccessful?
 
@@ -217,14 +223,18 @@
         logging.warning("Package not found")
         return
     if len(packages) > 1:
         logging.warning(f"Multiple packages found: {packages}")
         return
     package = packages[0]
     pprint.pp(package.to_dict())
+    import plugget.github as github
+    favorited = github.is_starred(package.repo_url)
+    star_count = github.get_repo_stars(package.repo_url)
+    print(f"starred by hannes: {favorited}, star-count ⭐:", star_count)
 
 
 # # todo this is a plugin command, exposed to plugget. maybe we want to do this for all commands?
 # def disable(package_name=None, plugin_name=None):
 #     """
 #     disable package
 #     :param name: name of the manifest folder in the manifest repo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `plugget-0.0.4/plugget/data/__init__.py` & `plugget-0.0.5/plugget/data/package.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __repr__(self):
         return f"Package({self.package_name} {self.version})"
 
     def __init__(self, app=None, name=None, display_name=None, plugin_name=None, id=None, version=None,
                  description=None, author=None, repo_url=None, package_url=None, license=None, tags=None,
                  dependencies=None, repo_paths=None, docs_url=None, package_name=None, manifest_path=None,
-                 actions=None, installed_paths=None, **kwargs):
+                 actions=None, installed_paths=None, repo_SHA=None, **kwargs):
         """
         :param app: the application this plugin is for e.g. blender
 
         :param name: the name of the plugin e.g. bqt (currently same as display_name)
         :param display_name: the display name of the plugin e.g. BQT (not used)
 
         :param plugin_name: the (unique) name of the plugin used by the app e.g. bqt
@@ -51,28 +51,30 @@
         self.version = version  # set from manifest name
         self.manifest_path = Path(manifest_path)  # set before _set_data_from_manifest_path()
         self._set_data_from_manifest_path()  # populate above attributes to their default values
 
         # manifest settings
         self.repo_url = repo_url  # set before plugin name
         self.repo_paths: "list[str]" = repo_paths  # subdir(s)
+        self.repo_SHA = repo_SHA
         self.package_url = package_url  # set before self.plugin_name
          # self.name = name #or self.plugin_name
         self.docs_url = None
         self._actions = actions  # todo default app action
         self.dependencies = dependencies or []  # todo
         # self.id = id or plugin_name  # unique id  # todo for now same as name
         description = ""
         # author = ""
         # license = ""
         # tags = []
-        # dependencies = []
 
         self.installed_paths = set() if installed_paths is None else set(installed_paths)   # list of files cloned locally
-
+        self._starred = None
+        self._stars = None
+        self._clone_dir = None
     # @property
     # def app(self):
     #     return self._app
     #
     # @app.setter
     # def app(self, value):
     #     self._app = value
@@ -107,31 +109,52 @@
         self.version = self.version or self._manifest_path.stem
         self.app = self.app or self._manifest_path.parent.parent.name  # todo change this to be more robust
         self.package_name = self.package_name or self._manifest_path.parent.name
 
     @property
     def clone_dir(self):
         """return the path we clone to on install e.g C:/Users/username/AppData/Local/Temp/plugget/bqt/0.1.0"""
-        return settings.TEMP_PLUGGET / self.app / self.package_name / self.version / self.package_name
+        if not self._clone_dir:
+            self._clone_dir = settings.TEMP_PLUGGET / self.app / self.package_name / self.version / self.package_name
+        return self._clone_dir
 
     @property
     def is_installed(self):
         """a plugin is installed, if the manifest is in the installed packages folder"""
         return (settings.INSTALLED_DIR / self.app / self.package_name / f"{self.version}.json").exists()
 
     @property
     def default_actions(self):
         """get the default action for the app"""
-        DefaultActions = {
-            "blender": ["blender_addon", "blender_pip"],
-            "max": ["max_macroscript"],  # todo pip
-            "krita": ["krita_plugin", "krita_pip"],
+        DefaultActions = {  # ppip actions before addon, install dependenies first else bug
+            "blender": ["blender_pip", "blender_addon"],
+            "max3ds": ["max_macroscript"],  # todo pip
+            "krita": ["krita_pip", "krita_plugin"],
+            "unreal": ["unreal_pip", "unreal_plugin"],
             # "maya": "maya_module",
         }
-        return DefaultActions.get(self.app)
+        actions = DefaultActions.get(self.app)
+        if not actions:
+            raise Exception(f"no default action for app {self.app}")
+        return actions
+
+    def get_stars(self):
+        """get the number of stars on the repo"""
+        import plugget.github
+        if self._stars is None:
+            self._stars =plugget.github.get_repo_stars(self.repo_url)
+        return self._stars
+
+    def is_starred(self):
+        """get the number of stars on the repo"""
+
+        import plugget.github
+        if self._starred is None:
+            self._starred = plugget.github.is_starred(self.repo_url)
+        return self._starred
 
     @property
     def actions(self):
         """
         get the action for the plugin, used for install, uninstall
         if the manifest doesn't specify an action, get the default action for the app
         """
@@ -184,14 +207,15 @@
         :param empty_keys: if True, include keys with None values
         """
         output = {'app': self.app,
                   'package_name': self.package_name,
                   'version': self.version,
                   'repo_url': self.repo_url,
                   'repo_paths': self.repo_paths,
+                  'self.repo_SHA': self.repo_SHA,
                   'package_url': self.package_url,
                   'docs_url': self.docs_url,
                   'actions': self._actions,
                   'dependencies': self.dependencies,
                   'installed_paths': [str(x) for x in self.installed_paths]
                   }
         if not empty_keys:
@@ -204,54 +228,67 @@
         """save the plugin to a json file"""
 
         output = self.to_dict()
         Path(json_path).parent.mkdir(exist_ok=True, parents=True)
         with open(json_path, "w") as f:
             json.dump(output, f, indent=4)
 
-    def get_content(self) -> "list[Path]":
+    def get_content(self, target_dir=None) -> "list[Path]":
         """download the plugin content from the repo, and return the paths to the files"""
-        return self._clone_repo()
+        return self._clone_repo(target_dir=target_dir)
+    # todo instead of clone can we download the files directly?
+    # cant clone to non empty folder, so we need to move files instead. but unreal had permission issues with that
 
-    def _clone_repo(self) -> "list[Path]":
+
+    def _clone_repo(self, target_dir=None) -> "list[Path]":
         """
         returns either the files in repo (sparse) or the folder containing the repo
         """
+
+        target_dir = target_dir or self.clone_dir
+        self._clone_dir = target_dir
+        # todo save target_dir in self.clone_dir ?
+
         # clone package repo to temp folder
-        rmdir(self.clone_dir)
+        rmdir(target_dir)
 
-        print("cloning", self.repo_url, "to", self.clone_dir)
+        print("cloning", self.repo_url, "to", target_dir)
         # todo sparse checkout, support multiple entries in self.repo_paths
-        if self.repo_paths:
-            # logging.debug(f"cloning {self.repo_url} to {self.clone_dir}")
-            subprocess.run(["git", "clone", "--depth", "1", "--progress", self.repo_url, str(self.clone_dir)])
-
-            # delete .git folder
-            rmdir(self.clone_dir / ".git")
 
-            # confirm folder was created
-            if not self.clone_dir.exists():
-                raise Exception(f"Failed to clone repo to {self.clone_dir}")
+        # logging.debug(f"cloning {self.repo_url} to {target_dir}")
+        subprocess.run(["git", "clone", "--depth", "1", "--progress", self.repo_url, str(target_dir)])
+        # todo this doesnt always print the error, see unreal plugget for example with errors
+
+        if self.repo_SHA:
+            # todo check if repo_SHA is valid
+            subprocess.run(["git", "fetch", "--depth", "1", "origin", self.repo_SHA], cwd=target_dir)
+            subprocess.run(["git", "checkout", self.repo_SHA], cwd=target_dir)
+
+        # delete .git folder
+        rmdir(target_dir / ".git")
+
+        # confirm folder was created
+        # todo check if target_dir / repo file or foldername(s) exist
+        #  target dir always exists
+        # if not target_dir.exists():
+        #     raise Exception(f"Failed to clone repo to {target_dir}")
 
-            return [self.clone_dir / p for p in self.repo_paths]
+        if self.repo_paths:
+            return [target_dir / p for p in self.repo_paths]
         else:
-            # clone repo
-            subprocess.run(["git", "clone", "--depth", "1", "--progress", self.repo_url, str(self.clone_dir)])
+            return [target_dir]
 
-            # delete .git folder
-            rmdir(self.clone_dir / ".git")
-
-            # app_dir = Path("C:/Users/hanne/OneDrive/Documents/repos/plugget-pkgs") / "blender"
-            return [self.clone_dir]
 
     def install(self, force=False, *args, **kwargs):
         from plugget import commands
 
         if self.is_installed and not force:
-            raise Exception(f"{self.package_name} is already installed")
+            logging.warning(f"{self.package_name} is already installed")
+            return
+            # raise Exception(f"{self.package_name} is already installed")
         for action in self.actions:
             # action install implicitly adds to self.install_paths
             action.install(self, *args, force=force, **kwargs)
 
         i = 0
         for d in self.dependencies:
             i += 1
@@ -278,29 +315,14 @@
                 d.setdefault("app", self.app)
                 d.setdefault("version", self.version)
                 d.setdefault("package_name", f"{self.package_name}_dependency_{i}")
                 package = Package(**d)
 
             package.install(force=force, *args, **kwargs)
 
-        # # if requirements.txt exists in self.repo_paths, install requirements
-        # requirements_paths = []
-        # if (self.clone_dir / "requirements.txt").exists():
-        #     requirements_paths.append(self.clone_dir / "requirements.txt")
-        # if self.repo_paths:
-        #     for p in self.repo_paths:
-        #         if p.endswith("requirements.txt"):
-        #             requirements_paths.append(self.clone_dir / p)
-        # for p in requirements_paths:
-        #     if p.exists():
-        #         print("requirements.txt found, installing requirements")
-        #         subprocess.run(["pip", "install", "-r", self.clone_dir / p])
-        #     else:
-        #         logging.warning(f"expected requirements.txt not found: '{p}'")
-
         # copy manifest to installed packages dir
         # todo check if install was successful
         manifest_path = settings.INSTALLED_DIR / self.app / self.package_name / self.manifest_path.name
         self.to_json(manifest_path)
 
     def uninstall(self, dependencies=False, **kwargs):
         for action in self.actions:
```

### Comparing `plugget-0.0.4/plugget.egg-info/PKG-INFO` & `plugget-0.0.5/plugget.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: plugget
-Version: 0.0.4
+Version: 0.0.5
 Summary: detect which app the python interpreter is running in
 Author: Hannes
 Project-URL: Homepage, https://github.com/hannesdelbeke/plugget
 Project-URL: Source, https://github.com/hannesdelbeke/plugget
 Keywords: plugin,addon,add-on,extension,package,manager,resource,studio,dcc,app,application,pipeline,blender,krita,max
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 
-# PlugGet
+<h1>
+<img src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" data-canonical-src="https://user-images.githubusercontent.com/3758308/231004489-25ce30d9-c534-4d10-8773-8e6f80f36dd2.png" width="70" />
+Plugget: Plugin Package Manager
+</h1>
 
 [![PyPI Downloads](https://img.shields.io/pypi/v/plugget?color=0)](https://pypi.org/project/plugget/)
 
 Install app packages (plugins, addons, icons, ...) from a repo with a single Python command: 
 ```python
 import plugget
 plugget.install("my_package")
 ```
 
 ![machinetoolsinstall](https://user-images.githubusercontent.com/3758308/227316999-adf32b7f-4232-46f5-b0db-1b3dbe26d755.gif)
 
 also check out
 - [plugget blender addon](https://github.com/hannesdelbeke/plugget-blender-addon)
 - [plugget manifest repo](https://github.com/hannesdelbeke/plugget-pkgs)
+- [plugget unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)
 
 ## requirements
 - pip installed
 - git installed
 (aim to auto handle requirements in future)
 
 ## not to confuse with
```

### Comparing `plugget-0.0.4/pyproject.toml` & `plugget-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
 dependencies = ['importlib-metadata; python_version<"3.7"', "detect-app"]
 #dynamic = ["version"]
-version = "0.0.4"
+version = "0.0.5"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `plugget-0.0.4/testcode.py` & `plugget-0.0.5/testcode.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # import sys
 # C:\Users\hanne\OneDrive\Documents\repos\pluginmanager
 # sys.path.append("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\plugget")
 import site
 site.addsitedir("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\plugget")
-site.addsitedir("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\plugget")
+site.addsitedir("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\detect-app")
 
 import plugget
 import plugget.commands as cmd
 import plugget.data as da
 import plugget.actions.blender_addon as ba
-import plugget.apps.blender as b
+# import plugget.apps.blender as b
 
 from importlib import reload
 reload(plugget)
-reload(b)
+# reload(b)
 reload(cmd)
 reload(da)
 reload(ba)
 
 cmd.install("textools")
```

