# Comparing `tmp/houdini_package_manager-1.0.8.tar.gz` & `tmp/houdini_package_manager-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houdini_package_manager-1.0.8.tar", max compression
+gzip compressed data, was "houdini_package_manager-1.0.9.tar", max compression
```

## Comparing `houdini_package_manager-1.0.8.tar` & `houdini_package_manager-1.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    34523 2023-05-13 05:18:26.037374 houdini_package_manager-1.0.8/LICENSE
--rw-r--r--   0        0        0     3842 2023-05-13 05:18:26.037374 houdini_package_manager-1.0.8/README.md
--rw-r--r--   0        0        0       22 2023-05-13 05:18:26.041374 houdini_package_manager-1.0.8/houdini_package_manager/__init__.py
--rw-r--r--   0        0        0     1149 2023-05-13 05:18:26.041374 houdini_package_manager-1.0.8/houdini_package_manager/main.py
--rw-r--r--   0        0        0     1975 2023-05-13 05:18:26.041374 houdini_package_manager-1.0.8/houdini_package_manager/meta/meta_tools.py
--rw-r--r--   0        0        0   614544 2023-05-13 05:18:26.045374 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Black.ttf
--rw-r--r--   0        0        0   672480 2023-05-13 05:18:26.053375 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
--rw-r--r--   0        0        0   657188 2023-05-13 05:18:26.057375 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Bold.ttf
--rw-r--r--   0        0        0   699008 2023-05-13 05:18:26.061375 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0        0        0   723544 2023-05-13 05:18:26.069376 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Italic.ttf
--rw-r--r--   0        0        0   644556 2023-05-13 05:18:26.073376 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Light.ttf
--rw-r--r--   0        0        0   658212 2023-05-13 05:18:26.081377 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
--rw-r--r--   0        0        0   637068 2023-05-13 05:18:26.085377 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Medium.ttf
--rw-r--r--   0        0        0   695588 2023-05-13 05:18:26.089377 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
--rw-r--r--   0        0        0   657212 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Regular.ttf
--rw-r--r--   0        0        0      332 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add.svg
--rw-r--r--   0        0        0      329 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_hover.svg
--rw-r--r--   0        0        0    10421 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages.svg
--rw-r--r--   0        0        0    10472 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_confirm.svg
--rw-r--r--   0        0        0    10475 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
--rw-r--r--   0        0        0    10424 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_hover.svg
--rw-r--r--   0        0        0     1991 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/bug.svg
--rw-r--r--   0        0        0     1988 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/bug_hover.svg
--rw-r--r--   0        0        0      803 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/clear_selection.svg
--rw-r--r--   0        0        0      800 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/clear_selection_hover.svg
--rw-r--r--   0        0        0      427 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/delete.svg
--rw-r--r--   0        0        0      424 2023-05-13 05:18:26.093377 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/delete_hover.svg
--rw-r--r--   0        0        0      505 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/docs.svg
--rw-r--r--   0        0        0      502 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/docs_hover.svg
--rw-r--r--   0        0        0      455 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/file.svg
--rw-r--r--   0        0        0      452 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/file_hover.svg
--rw-r--r--   0        0        0      382 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/folder.svg
--rw-r--r--   0        0        0      379 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/folder_hover.svg
--rw-r--r--   0        0        0     4286 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm.ico
--rw-r--r--   0        0        0      566 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm.svg
--rw-r--r--   0        0        0      598 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_ICO.svg
--rw-r--r--   0        0        0      591 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_grey.svg
--rw-r--r--   0        0        0      588 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_grey_hover.svg
--rw-r--r--   0        0        0      569 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_hover.svg
--rw-r--r--   0        0        0      571 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_icon.svg
--rw-r--r--   0        0        0      696 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/invert_selection.svg
--rw-r--r--   0        0        0      693 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/invert_selection_hover.svg
--rw-r--r--   0        0        0      323 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/migrate.svg
--rw-r--r--   0        0        0      320 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/migrate_hover.svg
--rw-r--r--   0        0        0     1455 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh.svg
--rw-r--r--   0        0        0     1625 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_all.svg
--rw-r--r--   0        0        0     1622 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_all_hover.svg
--rw-r--r--   0        0        0     1452 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_hover.svg
--rw-r--r--   0        0        0      484 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/remove.svg
--rw-r--r--   0        0        0      390 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/remove_all_items.svg
--rw-r--r--   0        0        0      387 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/remove_all_items_hover.svg
--rw-r--r--   0        0        0      502 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/remove_hover.svg
--rw-r--r--   0        0        0      837 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/repo.svg
--rw-r--r--   0        0        0      834 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/repo_hover.svg
--rw-r--r--   0        0        0      224 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/toggle_off.svg
--rw-r--r--   0        0        0      221 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/toggle_off_hover.svg
--rw-r--r--   0        0        0      334 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/toggle_on.svg
--rw-r--r--   0        0        0      331 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/toggle_on_hover.svg
--rw-r--r--   0        0        0      677 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/warning.svg
--rw-r--r--   0        0        0      680 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/warning_hover.svg
--rw-r--r--   0        0        0     2936 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/update.py
--rw-r--r--   0        0        0      868 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/utils.py
--rw-r--r--   0        0        0      655 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/actions.py
--rw-r--r--   0        0        0    22508 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/add_packages_layout.py
--rw-r--r--   0        0        0     3574 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/custom_widgets.py
--rw-r--r--   0        0        0     7351 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/main_window.py
--rw-r--r--   0        0        0    21983 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/packages_layout.py
--rw-r--r--   0        0        0    12686 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/widgets/packages_table.py
--rw-r--r--   0        0        0    28576 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/wrangle/config_control.py
--rw-r--r--   0        0        0     1079 2023-05-13 05:18:26.097378 houdini_package_manager-1.0.8/houdini_package_manager/wrangle/package_templates.py
--rw-r--r--   0        0        0     2104 2023-05-13 05:19:00.315457 houdini_package_manager-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4670 1970-01-01 00:00:00.000000 houdini_package_manager-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-16 22:14:57.382121 houdini_package_manager-1.0.9/LICENSE
+-rw-r--r--   0        0        0     4028 2023-05-16 22:14:57.382121 houdini_package_manager-1.0.9/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 22:14:57.386121 houdini_package_manager-1.0.9/houdini_package_manager/__init__.py
+-rw-r--r--   0        0        0     3767 2023-05-16 22:14:57.386121 houdini_package_manager-1.0.9/houdini_package_manager/dialogs.py
+-rw-r--r--   0        0        0     1775 2023-05-16 22:14:57.386121 houdini_package_manager-1.0.9/houdini_package_manager/main.py
+-rw-r--r--   0        0        0     1975 2023-05-16 22:14:57.386121 houdini_package_manager-1.0.9/houdini_package_manager/meta/meta_tools.py
+-rw-r--r--   0        0        0   614544 2023-05-16 22:14:57.390121 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Black.ttf
+-rw-r--r--   0        0        0   672480 2023-05-16 22:14:57.394122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf
+-rw-r--r--   0        0        0   657188 2023-05-16 22:14:57.398121 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Bold.ttf
+-rw-r--r--   0        0        0   699008 2023-05-16 22:14:57.406122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0        0        0   723544 2023-05-16 22:14:57.410122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Italic.ttf
+-rw-r--r--   0        0        0   644556 2023-05-16 22:14:57.414122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Light.ttf
+-rw-r--r--   0        0        0   658212 2023-05-16 22:14:57.418122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0        0        0   637068 2023-05-16 22:14:57.422122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Medium.ttf
+-rw-r--r--   0        0        0   695588 2023-05-16 22:14:57.430122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf
+-rw-r--r--   0        0        0   657212 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Regular.ttf
+-rw-r--r--   0        0        0      332 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add.svg
+-rw-r--r--   0        0        0      329 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_hover.svg
+-rw-r--r--   0        0        0    10421 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages.svg
+-rw-r--r--   0        0        0    10472 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_confirm.svg
+-rw-r--r--   0        0        0    10475 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg
+-rw-r--r--   0        0        0    10424 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_hover.svg
+-rw-r--r--   0        0        0     1991 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/bug.svg
+-rw-r--r--   0        0        0     1988 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/bug_hover.svg
+-rw-r--r--   0        0        0      803 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/clear_selection.svg
+-rw-r--r--   0        0        0      800 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/clear_selection_hover.svg
+-rw-r--r--   0        0        0      427 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/delete.svg
+-rw-r--r--   0        0        0      424 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/delete_hover.svg
+-rw-r--r--   0        0        0      505 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/docs.svg
+-rw-r--r--   0        0        0      502 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/docs_hover.svg
+-rw-r--r--   0        0        0      455 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/file.svg
+-rw-r--r--   0        0        0      452 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/file_hover.svg
+-rw-r--r--   0        0        0      382 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/folder.svg
+-rw-r--r--   0        0        0      379 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/folder_hover.svg
+-rw-r--r--   0        0        0     4286 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm.ico
+-rw-r--r--   0        0        0      566 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm.svg
+-rw-r--r--   0        0        0      598 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_ICO.svg
+-rw-r--r--   0        0        0      591 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_grey.svg
+-rw-r--r--   0        0        0      588 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_grey_hover.svg
+-rw-r--r--   0        0        0      569 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_hover.svg
+-rw-r--r--   0        0        0      571 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_icon.svg
+-rw-r--r--   0        0        0      696 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/invert_selection.svg
+-rw-r--r--   0        0        0      693 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/invert_selection_hover.svg
+-rw-r--r--   0        0        0      323 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/migrate.svg
+-rw-r--r--   0        0        0      320 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/migrate_hover.svg
+-rw-r--r--   0        0        0     1455 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh.svg
+-rw-r--r--   0        0        0     1625 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_all.svg
+-rw-r--r--   0        0        0     1622 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_all_hover.svg
+-rw-r--r--   0        0        0     1452 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_hover.svg
+-rw-r--r--   0        0        0      484 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/remove.svg
+-rw-r--r--   0        0        0      390 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/remove_all_items.svg
+-rw-r--r--   0        0        0      387 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/remove_all_items_hover.svg
+-rw-r--r--   0        0        0      502 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/remove_hover.svg
+-rw-r--r--   0        0        0      837 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/repo.svg
+-rw-r--r--   0        0        0      834 2023-05-16 22:14:57.434122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/repo_hover.svg
+-rw-r--r--   0        0        0      224 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/toggle_off.svg
+-rw-r--r--   0        0        0      221 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/toggle_off_hover.svg
+-rw-r--r--   0        0        0      334 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/toggle_on.svg
+-rw-r--r--   0        0        0      331 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/toggle_on_hover.svg
+-rw-r--r--   0        0        0      677 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/warning.svg
+-rw-r--r--   0        0        0      680 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/warning_hover.svg
+-rw-r--r--   0        0        0      868 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/utils.py
+-rw-r--r--   0        0        0      655 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/actions.py
+-rw-r--r--   0        0        0    22508 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/add_packages_layout.py
+-rw-r--r--   0        0        0     3574 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     7216 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/main_window.py
+-rw-r--r--   0        0        0    21983 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/packages_layout.py
+-rw-r--r--   0        0        0    12686 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/widgets/packages_table.py
+-rw-r--r--   0        0        0    28576 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/wrangle/config_control.py
+-rw-r--r--   0        0        0     1079 2023-05-16 22:14:57.438122 houdini_package_manager-1.0.9/houdini_package_manager/wrangle/package_templates.py
+-rw-r--r--   0        0        0     2104 2023-05-16 22:15:38.734447 houdini_package_manager-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4856 1970-01-01 00:00:00.000000 houdini_package_manager-1.0.9/PKG-INFO
```

### Comparing `houdini_package_manager-1.0.8/LICENSE` & `houdini_package_manager-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/README.md` & `houdini_package_manager-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 <p align="center">
   <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
 </p style = "margin-bottom: 2rem;">
 
+<p align="center">
+  <img width="700" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm_screenshot.png">
+</p style = "margin-bottom: 2rem;">
+
 # Houdini Package Manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
```

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/meta/meta_tools.py` & `houdini_package_manager-1.0.9/houdini_package_manager/meta/meta_tools.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Black.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Bold.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Italic.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Light.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Medium.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Medium.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/fonts/Lato-Regular.ttf` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_confirm.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_confirm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_confirm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/add_packages_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/add_packages_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/bug.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/bug.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/bug_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/bug_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/clear_selection.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/clear_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/clear_selection_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/clear_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm.ico` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm.ico`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_ICO.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_ICO.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_grey.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_grey.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_grey_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_grey_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/hpm_icon.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/hpm_icon.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/invert_selection.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/invert_selection.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/invert_selection_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/invert_selection_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_all.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_all.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_all_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_all_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/refresh_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/refresh_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/repo.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/repo.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/repo_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/repo_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/warning.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/warning.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/resources/icons/warning_hover.svg` & `houdini_package_manager-1.0.9/houdini_package_manager/resources/icons/warning_hover.svg`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/update.py` & `houdini_package_manager-1.0.9/houdini_package_manager/dialogs.py`

 * *Files 26% similar despite different names*

```diff
@@ -88,7 +88,38 @@
         no_button = QPushButton("No")
         no_button.clicked.connect(self.reject)
         button_layout.addWidget(no_button)
 
     def upgrade(self) -> None:
         QDesktopServices.openUrl(self.dist_url)
         self.accept()
+
+
+class ErrorDialog(QDialog):
+    """
+    A standard error dialog that contains a message and an OK button.
+    """
+
+    def __init__(self, error_message):
+        super().__init__()
+        self.setWindowTitle("Error: Houdini not installed")
+        self.setFixedWidth(300)
+        self.setFixedHeight(150)
+        self.layout_main = QVBoxLayout()
+        self.setLayout(self.layout_main)
+
+        label = QLabel(error_message)
+        label.setWordWrap(True)
+        self.layout_main.addWidget(label)
+
+        ok_button = QPushButton("OK")
+        ok_button.setMaximumWidth(85)
+        ok_button.clicked.connect(self.accept)
+        self.layout_main.addWidget(ok_button)
+
+        self.setStyleSheet(
+            """
+            background-color: #303030;
+            color: white;
+            padding: 5px;
+        """
+        )
```

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/utils.py` & `houdini_package_manager-1.0.9/houdini_package_manager/utils.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/actions.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/add_packages_layout.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/add_packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/custom_widgets.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/main_window.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 
 class MainWindow(QMainWindow):
     """
     The main window containing all of HPM's functionality.
     """
 
-    def __init__(self, app: QApplication) -> None:
+    def __init__(self, app: QApplication, houdini_data: HoudiniManager) -> None:
         super().__init__()
+
         self.app = app  # declare an app member
+        self.houdini_data = houdini_data
 
         TITLE = f"Houdini Package Manager {__version__}"
         self.setWindowTitle(TITLE)
 
         self.setWindowIcon(QIcon(epath("resources/icons/hpm_icon.svg", True)))
 
         self.setMinimumSize(1000, 550)
@@ -51,19 +53,14 @@
             """
             QToolTip {
                 border: 1px solid #3A3939;
             }
         """
         )
 
-        # MANAGE HOUDINI DATA
-        # get packages and their HOUDINI_PATH data for each installed Houdini version
-        self.houdini_data = HoudiniManager()
-        self.houdini_data.get_houdini_data()
-
         # if no package data (PackageCollection object) for a houdini install, then there's no way to know where
         # the Houdini /packages directory is, so remove the whole houdini install from the data
         valid_installs = {}
         for version, hou_install in self.houdini_data.hou_installs.items():
             if hou_install.packages:
                 valid_installs[version] = hou_install
         self.houdini_data.hou_installs = valid_installs
```

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/packages_layout.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/packages_layout.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/widgets/packages_table.py` & `houdini_package_manager-1.0.9/houdini_package_manager/widgets/packages_table.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/wrangle/config_control.py` & `houdini_package_manager-1.0.9/houdini_package_manager/wrangle/config_control.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/houdini_package_manager/wrangle/package_templates.py` & `houdini_package_manager-1.0.9/houdini_package_manager/wrangle/package_templates.py`

 * *Files identical despite different names*

### Comparing `houdini_package_manager-1.0.8/pyproject.toml` & `houdini_package_manager-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "houdini_package_manager"
-version = "1.0.8"
+version = "1.0.9"
 description = "GUI package manager for Houdini"
 authors = ["Ariff Jeff <ariffjeff@icloud.com>"]
 repository = "https://github.com/ariffjeff/houdini-package-manager"
 documentation = "https://ariffjeff.github.io/houdini-package-manager/"
 readme = "README.md"
 packages = [
   {include = "houdini_package_manager"}
```

### Comparing `houdini_package_manager-1.0.8/PKG-INFO` & `houdini_package_manager-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: houdini-package-manager
-Version: 1.0.8
+Version: 1.0.9
 Summary: GUI package manager for Houdini
 Home-page: https://github.com/ariffjeff/houdini-package-manager
 Author: Ariff Jeff
 Author-email: ariffjeff@icloud.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,18 @@
 Project-URL: Repository, https://github.com/ariffjeff/houdini-package-manager
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="125" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm.svg">
 </p style = "margin-bottom: 2rem;">
 
+<p align="center">
+  <img width="700" src="https://raw.githubusercontent.com/ariffjeff/houdini-package-manager/main/docs/static/hpm_screenshot.png">
+</p style = "margin-bottom: 2rem;">
+
 # Houdini Package Manager
 
 [![Release](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)](https://img.shields.io/github/v/release/ariffjeff/houdini-package-manager)
 [![Build status](https://img.shields.io/github/actions/workflow/status/ariffjeff/houdini-package-manager/main.yml?branch=main)](https://github.com/ariffjeff/houdini-package-manager/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/ariffjeff/houdini-package-manager/branch/main/graph/badge.svg)](https://codecov.io/gh/ariffjeff/houdini-package-manager)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)](https://img.shields.io/github/commit-activity/m/ariffjeff/houdini-package-manager)
 [![License](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)](https://img.shields.io/github/license/ariffjeff/houdini-package-manager)
```

