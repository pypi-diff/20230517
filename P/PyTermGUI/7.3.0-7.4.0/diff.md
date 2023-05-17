# Comparing `tmp/pytermgui-7.3.0.tar.gz` & `tmp/pytermgui-7.4.0.tar.gz`

## Comparing `pytermgui-7.3.0.tar` & `pytermgui-7.4.0.tar`

### file list

```diff
@@ -1,72 +1,78 @@
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/__init__.py
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/animations.py
--rw-r--r--   0        0        0    19812 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/ansi_interface.py
--rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/cmd.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/color_info.py
--rw-r--r--   0        0        0    26447 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/colors.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/context_managers.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/enums.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/exceptions.py
--rw-r--r--   0        0        0    18757 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/exporters.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/fancy_repr.py
--rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/file_loaders.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/helpers.py
--rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/highlighters.py
--rw-r--r--   0        0        0    11580 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/input.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/inspector.py
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/palettes.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/prettifiers.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/pretty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/py.typed
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/regex.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/serialization.py
--rw-r--r--   0        0        0    16815 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/term.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/aliases.py
--rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/language.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/macros.py
--rw-r--r--   0        0        0    21389 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/parsing.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/style_maps.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/markup/tokens.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/__init__.py
--rw-r--r--   0        0        0    24155 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/base.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/boxes.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/button.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/checkbox.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/collapsible.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/color_picker.py
--rw-r--r--   0        0        0    32656 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/containers.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/fancy_repr.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/inline.py
--rw-r--r--   0        0        0    13058 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/input_field.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/keyboard_button.py
--rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/pixel_matrix.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/slider.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/styles.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/widgets/toggle.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/window_manager/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/window_manager/compositor.py
--rw-r--r--   0        0        0    11517 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/window_manager/layouts.py
--rw-r--r--   0        0        0    19674 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/window_manager/manager.py
--rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pytermgui/window_manager/window.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/__init__.py
--rw-r--r--   0        0        0   142990 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/_exporter_targets.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/colorgrids.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test.yaml
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_animations.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_auto.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_colors.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_dump_n_load.py
--rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_exporters.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_fancy_repr.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_helpers.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_highlight_markup_literal.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_layouts.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_parser.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_regex.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.3.0/tests/test_styles.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.3.0/.gitignore
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.3.0/LICENSE
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 pytermgui-7.3.0/pyproject.toml
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 pytermgui-7.3.0/PKG-INFO
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 pytermgui-7.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     7429 2020-02-02 00:00:00.000000 pytermgui-7.4.0/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pytermgui-7.4.0/examples/README.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/__init__.py
+-rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/animations.py
+-rw-r--r--   0        0        0    19812 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/ansi_interface.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/cell.py
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/cmd.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/color_info.py
+-rw-r--r--   0        0        0    26454 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/colors.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/context_managers.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/enums.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/exceptions.py
+-rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/exporters.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/fancy_repr.py
+-rw-r--r--   0        0        0    12057 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/file_loaders.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/helpers.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/highlighters.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/input.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/inspector.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/palettes.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/prettifiers.py
+-rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/pretty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/py.typed
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/regex.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/serialization.py
+-rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/term.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/aliases.py
+-rw-r--r--   0        0        0    14551 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/language.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/macros.py
+-rw-r--r--   0        0        0    22738 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/parsing.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/style_maps.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/markup/tokens.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/__init__.py
+-rw-r--r--   0        0        0    25604 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/base.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/boxes.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/button.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/checkbox.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/collapsible.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/color_picker.py
+-rw-r--r--   0        0        0    33128 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/containers.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/fancy_repr.py
+-rw-r--r--   0        0        0     7950 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/frames.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/inline.py
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/input_field.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/keyboard_button.py
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/pixel_matrix.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/slider.py
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/styles.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/widgets/toggle.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/compositor.py
+-rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/layouts.py
+-rw-r--r--   0        0        0    19429 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/manager.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pytermgui/window_manager/window.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/__init__.py
+-rw-r--r--   0        0        0   138485 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/_exporter_targets.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/colorgrids.py
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/not_test_cell.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test.yaml
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_animations.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_auto.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_colors.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_dump_n_load.py
+-rw-r--r--   0        0        0    16036 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_exporters.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_fancy_repr.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_helpers.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_highlight_markup_literal.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_layouts.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_parser.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_regex.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytermgui-7.4.0/tests/test_styles.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 pytermgui-7.4.0/.gitignore
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytermgui-7.4.0/LICENSE
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 pytermgui-7.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 pytermgui-7.4.0/PKG-INFO
```

### Comparing `pytermgui-7.3.0/pytermgui/__init__.py` & `pytermgui-7.4.0/pytermgui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # Silence warning if running as standalone module
 if "-m" in sys.argv:  # pragma: no cover
     import warnings
 
     warnings.filterwarnings("ignore")
 
-__version__ = "7.3.0"
+__version__ = "7.4.0"
 
 
 def auto(data: Any, **widget_args: Any) -> Optional[Widget | list[Splitter]]:
     """Creates a widget from specific data structures.
 
     This conversion includes various widget classes, as well as some shorthands for
     more complex objects.  This method is called implicitly whenever a non-widget is
```

### Comparing `pytermgui-7.3.0/pytermgui/animations.py` & `pytermgui-7.4.0/pytermgui/animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/ansi_interface.py` & `pytermgui-7.4.0/pytermgui/ansi_interface.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/cmd.py` & `pytermgui-7.4.0/pytermgui/cmd.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/color_info.py` & `pytermgui-7.4.0/pytermgui/color_info.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/colors.py` & `pytermgui-7.4.0/pytermgui/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,30 +827,31 @@
     redmean = (red1 + red2) // 2
 
     delta_red = red1 - red2
     delta_green = green1 - green2
     delta_blue = blue1 - blue2
 
     return sqrt(
-        (2 + (redmean / 256)) * (delta_red**2)
-        + 4 * (delta_green**2)
-        + (2 + (255 - redmean) / 256) * (delta_blue**2)
+        (2 + (redmean / 256)) * (delta_red ** 2)
+        + 4 * (delta_green ** 2)
+        + (2 + (255 - redmean) / 256) * (delta_blue ** 2)
     )
 
 
 @lru_cache(maxsize=1024)
 def str_to_color(
     text: str,
     is_background: bool = False,
     localize: bool = True,
     use_cache: bool = True,
 ) -> Color:
     """Creates a `Color` from the given text.
 
     Accepted formats:
+
     - 0-255: `IndexedColor`.
     - 'rrr;ggg;bbb': `RGBColor`.
     - '(#)rrggbb': `HEXColor`. Leading hash is optional.
 
     You can also add a leading '@' into the string to make the output represent a
     background color, such as `@#123abc`.
```

### Comparing `pytermgui-7.3.0/pytermgui/context_managers.py` & `pytermgui-7.4.0/pytermgui/context_managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             show_cursor()
             cursor_up()
 
 
 @contextmanager
 def mouse_handler(
     events: list[str], method: str = "decimal_xterm"
-) -> Generator[MouseTranslator | None, None, None]:
+) -> Generator[MouseTranslator, None, None]:
     """Return a mouse handler function
 
     See `help(report_mouse)` for help about all of the methods.
 
     Args:
         events: A list of `pytermgui.ansi_interface.report_mouse` events.
         method: The method to use for reporting. Only `decimal_urxvt` and
@@ -141,9 +141,10 @@
     try:
         for event in events:
             report_mouse(event, method=method)
 
         yield lambda code: translate_mouse(code, method=method)
 
     finally:
+        input(event)
         if event is not None:
             report_mouse(event, method=method, stop=True)
```

### Comparing `pytermgui-7.3.0/pytermgui/enums.py` & `pytermgui-7.4.0/pytermgui/enums.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/exceptions.py` & `pytermgui-7.4.0/pytermgui/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/exporters.py` & `pytermgui-7.4.0/pytermgui/exporters.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
     return f"{prefix}-{index}"
 
 
 def _generate_stylesheet(document_styles: list[list[str]], prefix: str | None) -> str:
     """Generates a '\\n' joined CSS stylesheet from the given styles."""
 
     stylesheet = ""
+    prefix = prefix or ""
+
     for i, styles in enumerate(document_styles):
         stylesheet += (
             "\n        ." + _get_cls(prefix, i) + " {" + "; ".join(styles) + "}"
         )
 
     return stylesheet
 
@@ -323,15 +325,15 @@
                 document_styles.append(styles)
 
             if inline_styles:
                 stylesheet = ";".join(styles)
                 line += span.format(f" styles='{stylesheet}'")
 
             else:
-                line += span.format(" class='" + _get_cls(prefix, index) + "'")
+                line += span.format(" class='" + _get_cls(prefix or "", index) + "'")
 
         # Close any previously not closed divs
         line += "</div>" * (line.count("<div") - line.count("</div"))
         lines.append(line)
 
     stylesheet = ""
     if not inline_styles:
```

### Comparing `pytermgui-7.3.0/pytermgui/fancy_repr.py` & `pytermgui-7.4.0/pytermgui/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/file_loaders.py` & `pytermgui-7.4.0/pytermgui/file_loaders.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/helpers.py` & `pytermgui-7.4.0/pytermgui/helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/highlighters.py` & `pytermgui-7.4.0/pytermgui/highlighters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/input.py` & `pytermgui-7.4.0/pytermgui/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             string: Any string or bytes object.
 
         Returns:
             The string argument, converted to `str`.
         """
 
         if isinstance(string, bytes):
-            return string.decode("utf-8")
+            return string.decode("utf-8", "ignore")
 
         return string
 
     def get_chars(self) -> str:
         """Reads characters from sys.stdin.
 
         Returns:
@@ -365,19 +365,23 @@
         "ALT_DOWN": "\x1b[1;3B",
         "ALT_RIGHT": "\x1b[1;3C",
         "ALT_LEFT": "\x1b[1;3D",
         "ALT_SHIFT_UP": "\x1b[1;4A",
         "ALT_SHIFT_DOWN": "\x1b[1;4B",
         "ALT_SHIFT_RIGHT": "\x1b[1;4C",
         "ALT_SHIFT_LEFT": "\x1b[1;4D",
+        "ALT_BACKSPACE": "\x08",
+        "CTRL_BACKSPACE": "\x1b\x7f",
         "CTRL_UP": "\x1b[1;5A",
         "CTRL_DOWN": "\x1b[1;5B",
         "CTRL_RIGHT": "\x1b[1;5C",
         "CTRL_LEFT": "\x1b[1;5D",
         "BACKSPACE": "\x7f",
+        "END": "\x1b[H",
+        "HOME": "\x1b[F",
         "INSERT": "\x1b[2~",
         "DELETE": "\x1b[3~",
         "BACKTAB": "\x1b[Z",
         "F1": "\x1b[11~",
         "F2": "\x1b[12~",
         "F3": "\x1b[13~",
         "F4": "\x1b[14~",
```

### Comparing `pytermgui-7.3.0/pytermgui/inspector.py` & `pytermgui-7.4.0/pytermgui/inspector.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/palettes.py` & `pytermgui-7.4.0/pytermgui/palettes.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/prettifiers.py` & `pytermgui-7.4.0/pytermgui/prettifiers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/pretty.py` & `pytermgui-7.4.0/pytermgui/pretty.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/regex.py` & `pytermgui-7.4.0/pytermgui/regex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """This modules contains all of the regex-related names and utilites."""
 
 import re
 from functools import lru_cache
+from typing import Match
 
-RE_LINK = re.compile(r"(?:\x1b\]8;;([^\\]*)\x1b\\([^\\]*)\x1b\]8;;\x1b\\)")
+RE_LINK = re.compile(r"(?:\x1b\]8;;([^\\]*)\x1b\\([^\\]*?)\x1b\]8;;\x1b\\)")
 RE_ANSI_NEW = re.compile(rf"(\x1b\[(.*?)[mH])|{RE_LINK.pattern}|(\x1b_G(.*?)\x1b\\)")
 RE_ANSI = re.compile(r"(?:\x1b\[(.*?)[mH])|(?:\x1b\](.*?)\x1b\\)|(?:\x1b_G(.*?)\x1b\\)")
 RE_MACRO = re.compile(r"(![a-z0-9_\-]+)(?:\(([\w\/\.?\-=:]+)\))?")
 RE_MARKUP = re.compile(r"((\\*)\[([^\[\]]*)\])")
 RE_POSITION = re.compile(r"\x1b\[(\d*?)(?:;(\d*))?H")
 RE_PIXEL_SIZE = re.compile(r"\x1b\[4;([\d]+);([\d]+)t")
 
 RE_256 = re.compile(r"^([\d]{1,3})$")
 RE_HEX = re.compile(r"#?([0-9a-fA-F]{6})")
 RE_RGB = re.compile(r"(\d{1,3};\d{1,3};\d{1,3})")
 
 __all__ = [
     "strip_ansi",
     "strip_markup",
+    "escape_markup",
     "real_length",
 ]
 
 
 @lru_cache()
 def strip_ansi(text: str) -> str:
     """Removes ANSI sequences from text.
@@ -66,14 +68,28 @@
     Returns:
         The display-length of text.
     """
 
     return len(strip_ansi(text))
 
 
+def escape_markup(text: str) -> str:
+    """Escapes any potential markup to avoid double-parsing.
+
+    Use this when treating already parsed markup.
+    """
+
+    def _escape(mtch: Match) -> str:
+        full, *_ = mtch.groups()
+
+        return full.replace("[", r"\[")
+
+    return RE_MARKUP.sub(_escape, text)
+
+
 @lru_cache(maxsize=1024)
 def has_open_sequence(text: str) -> bool:
     """Figures out if the given text has any unclosed ANSI sequences.
 
     It supports standard SGR (`\\x1b[1mHello`), OSC (`\\x1b[30;2ST\\x1b\\\\`) and Kitty APC codes
     (`\x1b_Garguments;hex_data\\x1b\\\\`). It also recognizes incorrect syntax; it only considers
     a tag closed when it is using the right closing sequence, e.g. `m` or `H` for SGR, `\\x1b\\\\`
```

### Comparing `pytermgui-7.3.0/pytermgui/serialization.py` & `pytermgui-7.4.0/pytermgui/serialization.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/term.py` & `pytermgui-7.4.0/pytermgui/term.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,20 +533,22 @@
             return sliced
 
         if "\x1b[2J" in data:
             self.clear_stream()
 
         if pos is not None:
             xpos, ypos = pos
+            xpos += self.origin[0]
+            ypos += self.origin[1]
 
             if slice_too_long:
                 if not self.height + self.origin[1] + 1 > ypos >= 0:
                     return
 
-                maximum = self.width - xpos + self.origin[0]
+                maximum = self.width - xpos
 
                 if xpos < self.origin[0]:
                     xpos = self.origin[0]
 
                 sliced = _slice(data, maximum) if len(data) > maximum else data
 
                 data = f"\x1b[{ypos};{xpos}H{sliced}\x1b[0m"
```

### Comparing `pytermgui-7.3.0/pytermgui/markup/aliases.py` & `pytermgui-7.4.0/pytermgui/markup/aliases.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/markup/language.py` & `pytermgui-7.4.0/pytermgui/markup/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     def __init__(
         self,
         *,
         strict: bool = False,
         default_aliases: bool = True,
         default_macros: bool = True,
     ) -> None:
-        self._cache: dict[tuple[str, bool, bool], tuple[list[Token], str, bool]] = {}
+        self._cache: dict[tuple[str, bool, bool], tuple[str, list[Token], bool]] = {}
 
         self.context = create_context_dict()
         self._aliases = self.context["aliases"]
         self._macros = self.context["macros"]
 
         if default_aliases:
             apply_default_aliases(self)
```

### Comparing `pytermgui-7.3.0/pytermgui/markup/macros.py` & `pytermgui-7.4.0/pytermgui/markup/macros.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/markup/parsing.py` & `pytermgui-7.4.0/pytermgui/markup/parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,25 @@
     Token,
 )
 
 # TODO: Improve first-run performance.
 
 filterwarnings("always")
 
+STATE_COPY = "#stash"
+STATE_CUT = "#stash/"
+
+STATE_RESTORE = "#pop"
+STATE_REPLACE = "#/pop"
 
 LINK_TEMPLATE = "\x1b]8;;{uri}\x1b\\{label}\x1b]8;;\x1b\\"
 
+STATE_PSEUDOS = [STATE_CUT, STATE_COPY, STATE_REPLACE, STATE_RESTORE]
+PSEUDO_TOKENS = ["#auto", *STATE_PSEUDOS]
+
 __all__ = [
     "ContextDict",
     "create_context_dict",
     "consume_tag",
     "tokenize_markup",
     "tokenize_ansi",
     "optimize_tokens",
@@ -112,16 +120,16 @@
                 tag,
                 f"should have exactly 2 values separated by `;`, not {len(values)}",
                 "",
             )
 
         return CursorToken(tag[1:-1], *map(int, values))
 
-    if tag == "#auto":
-        return PseudoToken("#auto")
+    if tag in PSEUDO_TOKENS:
+        return PseudoToken(tag)
 
     token: Token
     try:
         token = ColorToken(tag, Color.parse(tag, localize=False))
 
     except ColorSyntaxError:
         token = AliasToken(tag)
@@ -197,28 +205,29 @@
 
     for matchobj in RE_ANSI.finditer(text):
         start, end = matchobj.span()
 
         csi = matchobj.groups()[0:2]
         link_osc = matchobj.groups()[2:4]
 
+        if cursor < start:
+            yield PlainToken(text[cursor:start])
+
         if link_osc != (None, None):
             cursor = end
             uri, label = link_osc
 
             yield HLinkToken(uri)
             yield PlainToken(label)
+            yield ClearToken("/~")
 
             continue
 
         full, content = csi
 
-        if cursor < start:
-            yield PlainToken(text[cursor:start])
-
         cursor = end
 
         code = ""
 
         # Position
         posmatch = RE_POSITION.match(full)
 
@@ -376,14 +385,17 @@
 
     return eval_alias(meaning, context).rstrip(" ")
 
 
 def parse_clear(token: ClearToken, _: ContextDict, get_full: Callable[[], str]) -> str:
     """Parses a clearer token."""
 
+    if token.value == "/~":
+        return "\x1b]8;;\x1b\\"
+
     index = CLEARERS.get(token.value)
     if index is None:
         raise MarkupSyntaxError(
             token.value, "not a recognized clearer or alias", get_full()
         )
 
     return f"\x1b[{index}m"
@@ -393,14 +405,51 @@
     """Parses a cursor token."""
 
     ypos, xpos = map(lambda i: "" if i is None else i, token)
 
     return f"\x1b[{ypos};{xpos}H"
 
 
+def parse_state_pseudo(
+    token: PseudoToken,
+    tokens: list[Token],
+    index: int,
+    save_state: list[Token],
+    context: ContextDict,
+) -> str:
+    """Parses a state pseudo tokens"""
+
+    tag = token.value
+
+    parsed = ""
+
+    if tag.startswith(STATE_CUT):
+        save_state.clear()
+        save_state.extend(filter(lambda tkn: not tkn.is_plain(), tokens[:index]))
+
+        if not tag == STATE_COPY:
+            parsed += "\x1b[0m"
+
+    # Restore
+    else:
+        local_state = save_state.copy()
+
+        if tag == STATE_REPLACE:
+            local_state.insert(0, ClearToken("/"))
+
+        parsed = parse_tokens(
+            local_state,
+            context=context,
+            optimize=False,
+            append_reset=False,
+        )
+
+    return parsed
+
+
 def optimize_tokens(tokens: list[Token]) -> Iterator[Token]:
     """Optimizes a stream of tokens, only yielding functionally relevant ones.
 
     Args:
         tokens: Any list of Token objects. Usually obtained from `tokenize_markup`
             or `tokenize_ansi`.
 
@@ -509,14 +558,15 @@
 
     for token in tokens:
         if token.is_plain():
             if len(tags) > 0:
                 markup += f"[{' '.join(tag.markup for tag in tags)}]"
 
             markup += token.value
+
             tags = []
 
         else:
             tags.append(token)
 
     if len(tags) > 0:
         markup += f"[{' '.join(tag.markup for tag in tags)}]"
@@ -671,15 +721,17 @@
     link = None
     output = ""
     segment = ""
     background = Color.parse("#000000")
     macros: list[MacroToken] = []
     unknown_aliases: list[Token] = []
 
-    for token in token_list:
+    save_state: list[Token] = []
+
+    for i, token in enumerate(token_list):
         if token.is_plain():
             value = _apply_macros(
                 token.value, (parse_macro(macro, context, get_full) for macro in macros)
             )
 
             if len(unknown_aliases) > 0:
                 output += f"[{' '.join(tkn.value for tkn in unknown_aliases)}]"
@@ -700,14 +752,17 @@
             macros.append(token)
             continue
 
         if Token.is_clear(token):
             if token.value in ("/", "/~"):
                 link = None
 
+                if token.value == "/~":
+                    continue
+
             found = False
             for macro in macros.copy():
                 if token.targets(macro):
                     macros.remove(macro)
                     found = True
                     break
 
@@ -719,14 +774,18 @@
                     token.value, "has nothing to target", get_full()
                 )
 
         if Token.is_color(token) and token.color.background:
             background = token.color
 
         if Token.is_pseudo(token):
+            if token.value in STATE_PSEUDOS:
+                segment += parse_state_pseudo(token, tokens, i, save_state, context)
+                continue
+
             if token.value == "#auto":
                 token = ColorToken("#auto", background.contrast)
 
         try:
             segment += PARSERS[type(token)](token, context, get_full)  # type: ignore
 
         except MarkupSyntaxError:
```

### Comparing `pytermgui-7.3.0/pytermgui/markup/style_maps.py` & `pytermgui-7.4.0/pytermgui/markup/style_maps.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/markup/tokens.py` & `pytermgui-7.4.0/pytermgui/markup/tokens.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/__init__.py` & `pytermgui-7.4.0/pytermgui/widgets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .base import *
 from .button import Button
 from .checkbox import Checkbox
 from .collapsible import *
 from .color_picker import ColorPicker
 from .containers import *
 from .fancy_repr import FancyReprWidget
+from .frames import *
 from .inline import inline
 from .input_field import InputField
 from .keyboard_button import KeyboardButton
 from .pixel_matrix import *
 from .slider import Slider
 from .styles import *
 from .toggle import Toggle
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/base.py` & `pytermgui-7.4.0/pytermgui/widgets/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -300,14 +300,49 @@
 
     @property
     def terminal(self) -> Terminal:
         """Returns the current global terminal instance."""
 
         return get_terminal()
 
+    def _align(self, lines: list[str]) -> list[str]:
+        """Aligns the given lines based on this widget's `parent_align` attribute."""
+
+        width = self.width
+
+        def _align_left(line: str) -> str:
+            return line + (width - real_length(line)) * " "
+
+        def _align_center(line: str) -> str:
+            right, extra = divmod(width - real_length(line), 2)
+            left = right + extra
+
+            return left * " " + line + right * " "
+
+        def _align_right(line: str) -> str:
+            return (width - real_length(line)) * " " + line
+
+        if self.parent_align is None:
+            raise TypeError("Horizontal alignment cannot be None.")
+
+        assert isinstance(self.parent_align, HorizontalAlignment)
+
+        aligner = {
+            HorizontalAlignment.LEFT: _align_left,
+            HorizontalAlignment.CENTER: _align_center,
+            HorizontalAlignment.RIGHT: _align_right,
+        }[self.parent_align]
+
+        aligned = []
+
+        for line in lines:
+            aligned.append(aligner(line))
+
+        return aligned
+
     def get_change(self) -> WidgetChange | None:
         """Determines whether widget lines changed since the last call to this function."""
 
         lines = self.get_lines()
 
         if self._previous_state is None:
             self._previous_state = (self.width, self.height), lines
@@ -541,14 +576,25 @@
         Raises:
             NotImplementedError: As this method is required for **all** widgets, not
                 having it defined will raise NotImplementedError.
         """
 
         raise NotImplementedError(f"get_lines() is not defined for type {type(self)}.")
 
+    def move(self, diff_x: int, diff_y: int) -> None:
+        """Moves the widget by the given x and y changes."""
+
+        self.pos = (self.pos[0] + diff_x, self.pos[1] + diff_y)
+
+        adjusted = []
+        for pos, line in self.positioned_line_buffer:
+            adjusted.append(((pos[0] + diff_x, pos[1] + diff_y), line))
+
+        self.positioned_line_buffer = adjusted
+
     def bind(
         self, key: str, action: BoundCallback, description: Optional[str] = None
     ) -> None:
         """Binds an action to a keypress.
 
         This function is only called by implementations above this layer. To use this
         functionality use `pytermgui.window_manager.WindowManager`, or write your own
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/boxes.py` & `pytermgui-7.4.0/pytermgui/widgets/boxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 ```
 
 Boxes are also settable as a property of `pytermgui.widgets.Container`, and can
 be referenced & defined in markup file definitions. For more info, check out
 `pytermgui.file_loaders`.
 """
 
+# This module is to be replaced with Frame, so the duplication won't be for long.
+# pylint: disable=duplicate-code
+
 from __future__ import annotations
 
 from typing import Tuple
 
 from ..regex import real_length
 from .base import WidgetType
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/button.py` & `pytermgui-7.4.0/pytermgui/widgets/button.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     styles = w_styles.StyleManager(
         label="@surface dim #auto",
         highlight="@surface+1 dim #auto",
         _current=None,
     )
 
-    chars: dict[str, w_styles.CharType] = {"delimiter": ["[ ", " ]"]}
+    chars: dict[str, w_styles.CharType] = {"delimiter": ["  ", "  "]}
 
     def __init__(
         self,
         label: str = "Button",
         onclick: Optional[Callable[[Button], Any]] = None,
         padding: int = 0,
         centered: bool = False,
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/checkbox.py` & `pytermgui-7.4.0/pytermgui/widgets/checkbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # TODO: Rewrite this to also have a label
 class Checkbox(Button):
     """A simple checkbox"""
 
     chars = {
         **Button.chars,
-        **{"delimiter": ["[", "]"], "checked": "X", "unchecked": " "},
+        **{"delimiter": [" ", " "], "checked": "▣", "unchecked": "□"},
     }
 
     def __init__(
         self,
         callback: Callable[[Any], Any] | None = None,
         checked: bool = False,
         **attrs: Any,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/collapsible.py` & `pytermgui-7.4.0/pytermgui/widgets/collapsible.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/color_picker.py` & `pytermgui-7.4.0/pytermgui/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/containers.py` & `pytermgui-7.4.0/pytermgui/widgets/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,14 +501,22 @@
 
         Args:
             other: The object to add.
         """
 
         self._add_widget(other, run_get_lines=False)
 
+    def move(self, diff_x: int, diff_y: int) -> None:
+        """Moves the widget and its children by the given x and y changes."""
+
+        super().move(diff_x, diff_y)
+
+        for child in self._widgets:
+            child.move(diff_x, diff_y)
+
     def get_lines(self) -> list[str]:
         """Gets all lines by spacing out inner widgets.
 
         This method reflects & applies both width settings, as well as
         the `parent_align` field.
 
         Returns:
@@ -579,23 +587,17 @@
             self.height = len(lines) + sum(has_top_bottom)
 
         vertical_offset, lines = self._apply_vertalign(
             lines, self.height - len(lines) - sum(has_top_bottom), align("")
         )
 
         for widget in self._widgets:
-            widget.pos = (widget.pos[0], widget.pos[1] + vertical_offset)
-
-            if widget.is_selectable:
-                # This buffer will be out of position, so we must clear it.
-                widget.positioned_line_buffer = []
-                widget.get_lines()
+            widget.move(0, vertical_offset)
 
             self.positioned_line_buffer.extend(widget.positioned_line_buffer)
-
             widget.positioned_line_buffer = []
 
         if has_top_bottom[0]:
             lines.insert(0, _get_border(corners[0], borders[1], corners[1]))
 
         if has_top_bottom[1]:
             lines.append(_get_border(corners[3], borders[3], corners[2]))
@@ -983,15 +985,15 @@
     keys = {
         "previous": {keys.LEFT, "h", keys.CTRL_B},
         "next": {keys.RIGHT, "l", keys.CTRL_F},
     }
 
     parent_align = HorizontalAlignment.RIGHT
 
-    def _align(
+    def _align_line(
         self, alignment: HorizontalAlignment, target_width: int, line: str
     ) -> tuple[int, str]:
         """Align a line
 
         r/wordavalanches"""
 
         available = target_width - real_length(line)
@@ -1011,25 +1013,26 @@
 
     @property
     def content_dimensions(self) -> tuple[int, int]:
         """Returns the available area for widgets."""
 
         return self.height, self.width
 
-    def get_lines(self) -> list[str]:
+    def get_lines(self) -> list[str]:  # pylint: disable=too-many-locals
         """Join all widgets horizontally."""
 
         # An error will be raised if `separator` is not the correct type (str).
         separator = self._get_style("separator")(self._get_char("separator"))  # type: ignore
         separator_length = real_length(separator)
 
         target_width, error = divmod(
             self.width - (len(self._widgets) - 1) * separator_length, len(self._widgets)
         )
 
+        self.positioned_line_buffer = []
         vertical_lines = []
         total_offset = 0
 
         for widget in self._widgets:
             inner = []
 
             if widget.size_policy is SizePolicy.STATIC:
@@ -1039,24 +1042,36 @@
                 widget.width = target_width + error
                 width = widget.width
                 error = 0
 
             aligned: str | None = None
             for line in widget.get_lines():
                 # See `enums.py` for information about this ignore
-                padding, aligned = self._align(
+                padding, aligned = self._align_line(
                     cast(HorizontalAlignment, widget.parent_align), width, line
                 )
                 inner.append(aligned)
 
-            widget.pos = (
+            new_pos = (
                 self.pos[0] + padding + total_offset,
                 self.pos[1] + (1 if type(widget).__name__ == "Container" else 0),
             )
 
+            diff_x = new_pos[0] - widget.pos[0]
+            diff_y = new_pos[1] - widget.pos[1]
+
+            widget.pos = new_pos
+
+            for pos, line in widget.positioned_line_buffer:
+                self.positioned_line_buffer.append(
+                    ((pos[0] + diff_x, pos[1] + diff_y), line)
+                )
+
+            widget.positioned_line_buffer = []
+
             if aligned is not None:
                 total_offset += real_length(inner[-1]) + separator_length
 
             vertical_lines.append(inner)
 
         lines = []
         for horizontal in zip_longest(*vertical_lines, fillvalue=" " * target_width):
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/fancy_repr.py` & `pytermgui-7.4.0/pytermgui/widgets/fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/inline.py` & `pytermgui-7.4.0/pytermgui/widgets/inline.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,18 @@
 
     if width is not None:
         widget.width = width
 
     if exit_on is None:
         exit_on = [keys.CTRL_C, keys.ENTER]
 
-    widget.pos = report_cursor()
+    cursor = report_cursor()
+
+    if cursor is not None:
+        widget.pos = cursor
 
     def _print_widget() -> None:
         save_cursor()
 
         for line in widget.get_lines():
             print(line)
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/input_field.py` & `pytermgui-7.4.0/pytermgui/widgets/input_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module contains the `InputField` class."""
 
 from __future__ import annotations
 
 import string
 from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Any, Iterator
+from typing import Any, Iterator, Literal
 
 from ..ansi_interface import MouseAction, MouseEvent
 from ..enums import HorizontalAlignment
 from ..helpers import break_line
 from ..input import keys
 from . import styles as w_styles
 from .base import Widget
@@ -47,20 +47,25 @@
         prompt="surface+2",
         cursor="@primary dim #auto",
     )
 
     keys = {
         "move_left": {keys.LEFT},
         "move_right": {keys.RIGHT},
+        "move_word_left": {keys.ALT_LEFT, keys.CTRL_LEFT},
+        "move_word_right": {keys.ALT_RIGHT, keys.CTRL_RIGHT},
         "move_up": {keys.UP},
         "move_down": {keys.DOWN},
+        "move_end": {keys.END},
+        "move_home": {keys.HOME},
         "select_left": {keys.SHIFT_LEFT},
         "select_right": {keys.SHIFT_RIGHT},
         "select_up": {keys.SHIFT_UP},
         "select_down": {keys.SHIFT_DOWN},
+        "word_remove": {keys.ALT_BACKSPACE, keys.CTRL_BACKSPACE},
     }
 
     parent_align = HorizontalAlignment.LEFT
 
     def __init__(
         self,
         value: str = "",
@@ -172,15 +177,15 @@
         start, end = sorted([col, col - count])
         start = max(0, start)
         self._lines[row] = line[:start] + line[end:]
 
         self._styled_cache = None
 
         if self._lines[row] == "":
-            self.move_cursor((-1, len(self._lines[row - 1])))
+            self.move_cursor((0, -2))
 
             return self._lines.pop(row)
 
         if count > 0:
             self.move_cursor((0, -count))
 
         return line[col - count : col]
@@ -196,14 +201,45 @@
         line = self._lines[row]
 
         self._lines[row] = line[:col] + text + line[col:]
         self.move_cursor((0, len(text)))
 
         self._styled_cache = None
 
+    def get_word_pos(self, direction: Literal[-1, 1]) -> int:
+        """Gets the column offset to the next word in the given direction.
+
+        Args:
+            direction: Which direction we need to look for.
+
+        Returns:
+            The column offset.
+        """
+
+        row, col = self.cursor
+        if len(self._lines) <= row:
+            return direction
+
+        # Consistent with unix shell behaviour:
+        # * Always delete first char, then remove any non-punctuation
+        # Note that the exact behaviour isn't standardized:
+        # * Python repl: until change in letter+digit & punctionation
+        # * Unix shells: only removes letter+digit
+        word_chars = string.ascii_letters + string.digits
+
+        if direction == -1:
+            line = self._lines[row][: col - 1]
+            strip_line = line.rstrip(word_chars)
+
+        else:
+            line = self._lines[row][col:]
+            strip_line = line.lstrip(word_chars)
+
+        return -direction * (len(strip_line) - len(line)) + direction
+
     def handle_action(self, action: str) -> bool:
         """Handles some action.
 
         This will be expanded in the future to allow using all behaviours with
         just their actions.
         """
 
@@ -211,14 +247,28 @@
             "move_left": (0, -1),
             "move_right": (0, 1),
             "move_up": (-1, 0),
             "move_down": (1, 0),
         }
 
         if action.startswith("move_"):
+            if action.endswith(("word_left", "word_right")):
+                col = self.get_word_pos(-1 if action == "move_word_left" else 1)
+                self.move_cursor((0, col))
+                return True
+
+            if action.endswith(("end", "home")):
+                crow, ccol = self.cursor
+                if action == "move_end":
+                    ccol = len(self._lines[crow])
+                else:
+                    ccol = 0
+                self.move_cursor((crow, ccol), absolute=True)
+                return True
+
             row, col = cursors[action]
 
             if self.cursor.row + row > len(self._lines):
                 self._lines.append("")
 
             col += self._selection_length
             if self._selection_length > 0:
@@ -233,14 +283,19 @@
                 self.update_selection(1)
 
             elif action == "select_left":
                 self.update_selection(-1)
 
             return True
 
+        if action == "word_remove":
+            row, col = self.cursor
+            self.delete_back(-self.get_word_pos(-1))
+            return True
+
         return False
 
     # TODO: This could probably be simplified by a wider adoption of the action pattern.
     def handle_key(  # pylint: disable=too-many-return-statements, too-many-branches
         self, key: str
     ) -> bool:
         """Adds text to the field, or moves the cursor."""
@@ -268,14 +323,17 @@
             return True
 
         if key in string.printable and key not in "\x0c\x0b":
             if key == keys.ENTER:
                 if not self.multiline:
                     return False
 
+                if len(self._lines) <= self.cursor.row:
+                    self._lines.append("")
+
                 line = self._lines[self.cursor.row]
                 left, right = line[: self.cursor.col], line[self.cursor.col :]
 
                 self._lines[self.cursor.row] = left
                 self._lines.insert(self.cursor.row + 1, right)
 
                 self.move_cursor((1, -self.cursor.col))
@@ -292,23 +350,25 @@
 
         if key == keys.BACKSPACE:
             if self._selection_length == 1:
                 self.delete_back(1)
             else:
                 self.delete_back(-self._selection_length)
 
-            # self.handle_action("move_left")
-
-            # if self._selection_length == 1:
-
             self._selection_length = 1
             self._styled_cache = None
 
             return True
 
+        if len(key) > 1 and not key.startswith("\x1b["):
+            for char in key:
+                self.handle_key(char)
+
+            return True
+
         return False
 
     def handle_mouse(self, event: MouseEvent) -> bool:
         """Allows point-and-click selection."""
 
         x_offset = event.position[0] - self.pos[0]
         y_offset = event.position[1] - self.pos[1]
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/keyboard_button.py` & `pytermgui-7.4.0/pytermgui/widgets/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/pixel_matrix.py` & `pytermgui-7.4.0/pytermgui/widgets/pixel_matrix.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/slider.py` & `pytermgui-7.4.0/pytermgui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/widgets/styles.py` & `pytermgui-7.4.0/pytermgui/widgets/styles.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
         if len(shorthand) == 0:
             return MarkupFormatter("{item}")
 
         if RE_MARKUP.match(shorthand) is not None:
             return MarkupFormatter(shorthand)
 
-        tokens = _sub_aliases(tokenize_markup(f"[{shorthand}]"), tim.context)
+        tokens = _sub_aliases(list(tokenize_markup(f"[{shorthand}]")), tim.context)
 
         colors = [tkn for tkn in tokens if Token.is_color(tkn)]
 
         if any(tkn.color.background for tkn in colors) and not any(
             not tkn.color.background for tkn in colors
         ):
             shorthand += " #auto"
```

### Comparing `pytermgui-7.3.0/pytermgui/widgets/toggle.py` & `pytermgui-7.4.0/pytermgui/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/window_manager/__init__.py` & `pytermgui-7.4.0/pytermgui/window_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/window_manager/compositor.py` & `pytermgui-7.4.0/pytermgui/window_manager/compositor.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pytermgui/window_manager/layouts.py` & `pytermgui-7.4.0/pytermgui/window_manager/layouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,19 @@
 
     @property
     def terminal(self) -> Terminal:
         """Returns the current global terminal instance."""
 
         return get_terminal()
 
+    def __len__(self) -> int:
+        """Gets the slot count of this layout."""
+
+        return len(self.slots)
+
     def _to_rows(self) -> list[list[Slot]]:
         """Breaks `self.slots` into a list of list of slots.
 
         The terminal's remaining width is kept track of, and when a slot doesn't have enough
         space left it is pushed to a new row. Additionally, `ROW_BREAK` will force a new
         row to be created, starting with the next slot.
         """
```

### Comparing `pytermgui-7.3.0/pytermgui/window_manager/manager.py` & `pytermgui-7.4.0/pytermgui/window_manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             self.autorun = autorun
 
         self.layout = layout_type()
         self.compositor = Compositor(self._windows, framerate=framerate)
         self.mouse_translator: MouseTranslator | None = None
 
         self._mouse_target: Window | None = None
+        self._focus_index = 0
         self._drag_offsets: tuple[int, int] = (0, 0)
         self._drag_target: tuple[Window, Edge] | None = None
 
         # This isn't quite implemented at the moment.
         self.restrict_within_bounds = True
 
         terminal.subscribe(terminal.RESIZE, self.on_resize)
@@ -110,16 +111,17 @@
     def __exit__(self, _: Any, exception: Exception, __: Any) -> bool:
         """Ends context manager."""
 
         # Run the manager if it hasnt been run before.
         if self.autorun and exception is None and self.mouse_translator is None:
             self.run()
 
+        self.stop()
+
         if exception is not None:
-            self.stop()
             raise exception
 
         return True
 
     def __iter__(self) -> Iterator[Window]:
         """Iterates this manager's windows."""
 
@@ -128,15 +130,14 @@
     def _run_input_loop(self) -> None:
         """The main input loop of the WindowManager."""
 
         while self._is_running:
             key = getch(interrupts=False)
 
             if key == chr(3):
-                self.stop()
                 break
 
             if self.handle_key(key):
                 continue
 
             self.process_mouse(key)
 
@@ -289,46 +290,39 @@
 
         if self.focused is not None:
             self.focused.blur()
 
         self.focused = window
 
         if window is not None:
-            self._windows.remove(window)
-            self._windows.insert(0, window)
+            self._focus_index = self._windows.index(window)
 
             window.focus()
 
-    def focus_next(self) -> Window | None:
-        """Focuses the next window in focus order, looping to first at the end."""
+    def focus_next(self, step: int = 1) -> Window | None:
+        """Focuses the next window in focus order, looping to first at the end.
 
-        if self.focused is None:
-            self.focus(self._windows[0])
-            return self.focused
+        Args:
+            step: The direction to step through windows. +1 for next, -1 for previous.
+        """
 
-        index = self._windows.index(self.focused)
-        if index == len(self._windows) - 1:
-            index = 0
+        self._focus_index += step
 
-        window = self._windows[index]
-        traversed = 0
-        while window.is_persistent or window is self.focused:
-            if index >= len(self._windows):
-                index = 0
+        if self._focus_index >= len(self._windows):
+            self._focus_index = 0
 
-            window = self._windows[index]
+        if self.focused is not None:
+            self.focused.blur()
 
-            index += 1
-            traversed += 1
-            if traversed >= len(self._windows):
-                return self.focused
+        window = self._windows[-self._focus_index]
 
-        self.focus(self._windows[index])
+        window.focus()
+        self.focused = window
 
-        return self.focused
+        return window
 
     def handle_key(self, key: str) -> bool:
         """Processes a keypress.
 
         Args:
             key: The key to handle.
```

### Comparing `pytermgui-7.3.0/pytermgui/window_manager/window.py` & `pytermgui-7.4.0/pytermgui/window_manager/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,22 +253,27 @@
             title: The string to set as the window title.
             position: An integer indexing into ["left", "top", "right", "bottom"],
                 determining where the title is applied.
             pad: Whether there should be an extra space before and after the given title.
                 defaults to True.
         """
 
+        corners = self._get_char("corner")
+        assert isinstance(corners, list)
+
+        # Delete (both cases) of current title from the corner
+        corners[position] = (
+            corners[position].replace(f" {self.title} ", "").replace(self.title, "")
+        )
+
         self.title = title
 
         if pad:
             title = " " + title + " "
 
-        corners = self._get_char("corner")
-        assert isinstance(corners, list)
-
         if position % 2 == 0:
             corners[position] += title
 
         else:
             current = corners[position]
             corners[position] = title + current
```

### Comparing `pytermgui-7.3.0/tests/_exporter_targets.py` & `pytermgui-7.4.0/tests/_exporter_targets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1166,481 +1166,481 @@
                 font-family: Menlo, 'DejaVu Sans Mono', consolas, 'Courier New', monospace;
                 line-height: 1.2em;
             }
             .ptg-position {
                 position: absolute;
             }
 
-        .None-0 {background-color: var(--ptg-background); background-color:#afaf00; color:#ffd787}
-        .None-1 {background-color: var(--ptg-background); background-color:#875f87; color:#5fff00}
-        .None-2 {background-color: var(--ptg-background); background-color:#af87af; color:#afaf5f}
-        .None-3 {background-color: var(--ptg-background); background-color:#0087d7; color:#ff00af}
-        .None-4 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ffd75f}
-        .None-5 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#5faf00}
-        .None-6 {background-color: var(--ptg-background); background-color:#ffaf00; color:#5f005f}
-        .None-7 {background-color: var(--ptg-background); background-color:#af00af; color:#00ffaf}
-        .None-8 {background-color: var(--ptg-background); background-color:#ff87af; color:#87ffd7}
-        .None-9 {background-color: var(--ptg-background); background-color:#005faf; color:#00af5f}
-        .None-10 {background-color: var(--ptg-background); background-color:#8700ff; color:#5f87ff}
-        .None-11 {background-color: var(--ptg-background); background-color:#5f5faf; color:#d70087}
-        .None-12 {background-color: var(--ptg-background); background-color:#5f5f87; color:#d75f5f}
-        .None-13 {background-color: var(--ptg-background); background-color:#8787af; color:#afafd7}
-        .None-14 {background-color: var(--ptg-background); background-color:#87afaf; color:#87d787}
-        .None-15 {background-color: var(--ptg-background); background-color:#afd787; color:#ff87ff}
-        .None-16 {background-color: var(--ptg-background); background-color:#00af87; color:#d7d75f}
-        .None-17 {background-color: var(--ptg-background); background-color:#d700ff; color:#d75f5f}
-        .None-18 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#87ff00}
-        .None-19 {background-color: var(--ptg-background); background-color:#8787af; color:#5f5fd7}
-        .None-20 {background-color: var(--ptg-background); background-color:#5f00af; color:#ff0000}
-        .None-21 {background-color: var(--ptg-background); background-color:#d75f5f; color:#d75fd7}
-        .None-22 {background-color: var(--ptg-background); background-color:#ff87d7; color:#00afd7}
-        .None-23 {background-color: var(--ptg-background); background-color:#5f0000; color:#ff5f87}
-        .None-24 {background-color: var(--ptg-background); background-color:#afd7af; color:#8700d7}
-        .None-25 {background-color: var(--ptg-background); background-color:#87d787; color:#00ff5f}
-        .None-26 {background-color: var(--ptg-background); background-color:#ff87ff; color:#ffafaf}
-        .None-27 {background-color: var(--ptg-background); background-color:#5f875f; color:#0000ff}
-        .None-28 {background-color: var(--ptg-background); background-color:#5f5f00; color:#00ffff}
-        .None-29 {background-color: var(--ptg-background); background-color:#87875f; color:#d75f5f}
-        .None-30 {background-color: var(--ptg-background); background-color:#d7af00; color:#d78787}
-        .None-31 {background-color: var(--ptg-background); background-color:#5fff5f; color:#ff0000}
-        .None-32 {background-color: var(--ptg-background); background-color:#d75f87; color:#5f5f5f}
-        .None-33 {background-color: var(--ptg-background); background-color:#ff87af; color:#afd700}
-        .None-34 {background-color: var(--ptg-background); background-color:#000087; color:#af5f00}
-        .None-35 {background-color: var(--ptg-background); background-color:#875f5f; color:#af0087}
-        .None-36 {background-color: var(--ptg-background); background-color:#ffd787; color:#005fff}
-        .None-37 {background-color: var(--ptg-background); background-color:#5f0000; color:#00ffff}
-        .None-38 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7af87}
-        .None-39 {background-color: var(--ptg-background); background-color:#d78700; color:#00ff5f}
-        .None-40 {background-color: var(--ptg-background); background-color:#5fff00; color:#afaf00}
-        .None-41 {background-color: var(--ptg-background); background-color:#afafff; color:#5f0087}
-        .None-42 {background-color: var(--ptg-background); background-color:#d7afaf; color:#8787d7}
-        .None-43 {background-color: var(--ptg-background); background-color:#d70087; color:#5f5fff}
-        .None-44 {background-color: var(--ptg-background); background-color:#87005f; color:#0000ff}
-        .None-45 {background-color: var(--ptg-background); background-color:#ffff00; color:#5fffff}
-        .None-46 {background-color: var(--ptg-background); background-color:#af8700; color:#87d75f}
-        .None-47 {background-color: var(--ptg-background); background-color:#8700d7; color:#d7d787}
-        .None-48 {background-color: var(--ptg-background); background-color:#008787; color:#afafd7}
-        .None-49 {background-color: var(--ptg-background); background-color:#5fff87; color:#ff87d7}
-        .None-50 {background-color: var(--ptg-background); background-color:#5f8787; color:#5f87ff}
-        .None-51 {background-color: var(--ptg-background); background-color:#d7afff; color:#af5fd7}
-        .None-52 {background-color: var(--ptg-background); background-color:#ffffaf; color:#afffaf}
-        .None-53 {background-color: var(--ptg-background); background-color:#878700; color:#87d7d7}
-        .None-54 {background-color: var(--ptg-background); background-color:#d70000; color:#ffff00}
-        .None-55 {background-color: var(--ptg-background); background-color:#5fff00; color:#5f5fff}
-        .None-56 {background-color: var(--ptg-background); background-color:#ffafd7; color:#ff0087}
-        .None-57 {background-color: var(--ptg-background); background-color:#ffd7af; color:#ffffff}
-        .None-58 {background-color: var(--ptg-background); background-color:#0087d7; color:#ffafff}
-        .None-59 {background-color: var(--ptg-background); background-color:#afd7ff; color:#ff00af}
-        .None-60 {background-color: var(--ptg-background); background-color:#d7af00; color:#00ff5f}
-        .None-61 {background-color: var(--ptg-background); background-color:#5f875f; color:#00d7d7}
-        .None-62 {background-color: var(--ptg-background); background-color:#00afff; color:#000087}
-        .None-63 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#00d7ff}
-        .None-64 {background-color: var(--ptg-background); background-color:#ffff00; color:#d7d7d7}
-        .None-65 {background-color: var(--ptg-background); background-color:#5fafff; color:#00ffaf}
-        .None-66 {background-color: var(--ptg-background); background-color:#afffff; color:#0087ff}
-        .None-67 {background-color: var(--ptg-background); background-color:#00d787; color:#5f0000}
-        .None-68 {background-color: var(--ptg-background); background-color:#afaf5f; color:#87ffff}
-        .None-69 {background-color: var(--ptg-background); background-color:#afff00; color:#ff87af}
-        .None-70 {background-color: var(--ptg-background); background-color:#ffff87; color:#5fff87}
-        .None-71 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ff8787}
-        .None-72 {background-color: var(--ptg-background); background-color:#8787d7; color:#afffff}
-        .None-73 {background-color: var(--ptg-background); background-color:#5fffaf; color:#d7ffff}
-        .None-74 {background-color: var(--ptg-background); background-color:#af00d7; color:#ffaf5f}
-        .None-75 {background-color: var(--ptg-background); background-color:#00ff87; color:#d78787}
-        .None-76 {background-color: var(--ptg-background); background-color:#d7ffff; color:#ff5fd7}
-        .None-77 {background-color: var(--ptg-background); background-color:#d7afff; color:#ffafff}
-        .None-78 {background-color: var(--ptg-background); background-color:#00d7af; color:#ff8700}
-        .None-79 {background-color: var(--ptg-background); background-color:#005f00; color:#00005f}
-        .None-80 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#ffd75f}
-        .None-81 {background-color: var(--ptg-background); background-color:#5f00af; color:#d75f5f}
-        .None-82 {background-color: var(--ptg-background); background-color:#d7ff00; color:#875f00}
-        .None-83 {background-color: var(--ptg-background); background-color:#5fffd7; color:#afffff}
-        .None-84 {background-color: var(--ptg-background); background-color:#0087af; color:#0000ff}
-        .None-85 {background-color: var(--ptg-background); background-color:#af87af; color:#d787af}
-        .None-86 {background-color: var(--ptg-background); background-color:#ffff87; color:#ffff00}
-        .None-87 {background-color: var(--ptg-background); background-color:#5f00af; color:#afd75f}
-        .None-88 {background-color: var(--ptg-background); background-color:#87d7ff; color:#d70000}
-        .None-89 {background-color: var(--ptg-background); background-color:#d7afd7; color:#d7af5f}
-        .None-90 {background-color: var(--ptg-background); background-color:#87afd7; color:#000087}
-        .None-91 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffd75f}
-        .None-92 {background-color: var(--ptg-background); background-color:#87ff87; color:#5fffaf}
-        .None-93 {background-color: var(--ptg-background); background-color:#af87af; color:#5f00af}
-        .None-94 {background-color: var(--ptg-background); background-color:#af00ff; color:#af0087}
-        .None-95 {background-color: var(--ptg-background); background-color:#87ffd7; color:#ff8787}
-        .None-96 {background-color: var(--ptg-background); background-color:#d7d7ff; color:#005f5f}
-        .None-97 {background-color: var(--ptg-background); background-color:#5faf87; color:#afaf00}
-        .None-98 {background-color: var(--ptg-background); background-color:#ff5faf; color:#5f5f5f}
-        .None-99 {background-color: var(--ptg-background); background-color:#afd787; color:#ffff87}
-        .None-100 {background-color: var(--ptg-background); background-color:#afd75f; color:#00ffaf}
-        .None-101 {background-color: var(--ptg-background); background-color:#ff00af; color:#af00d7}
-        .None-102 {background-color: var(--ptg-background); background-color:#00d7d7; color:#5f00ff}
-        .None-103 {background-color: var(--ptg-background); background-color:#5f5f87; color:#5fd7ff}
-        .None-104 {background-color: var(--ptg-background); background-color:#5fffaf; color:#5fd7af}
-        .None-105 {background-color: var(--ptg-background); background-color:#0087ff; color:#87ff87}
-        .None-106 {background-color: var(--ptg-background); background-color:#afafaf; color:#ffffff}
-        .None-107 {background-color: var(--ptg-background); background-color:#ff5fff; color:#87d700}
-        .None-108 {background-color: var(--ptg-background); background-color:#00afaf; color:#00afaf}
-        .None-109 {background-color: var(--ptg-background); background-color:#870000; color:#87ffff}
-        .None-110 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffafd7}
-        .None-111 {background-color: var(--ptg-background); background-color:#5faf00; color:#005f5f}
-        .None-112 {background-color: var(--ptg-background); background-color:#af87af; color:#af8787}
-        .None-113 {background-color: var(--ptg-background); background-color:#87d7af; color:#d75faf}
-        .None-114 {background-color: var(--ptg-background); background-color:#ff8700; color:#87005f}
-        .None-115 {background-color: var(--ptg-background); background-color:#d7d75f; color:#5fffd7}
-        .None-116 {background-color: var(--ptg-background); background-color:#5fd7d7; color:#00af5f}
-        .None-117 {background-color: var(--ptg-background); background-color:#d7005f; color:#d7ffaf}
-        .None-118 {background-color: var(--ptg-background); background-color:#afaf00; color:#d7d700}
-        .None-119 {background-color: var(--ptg-background); background-color:#00d7ff; color:#af0087}
-        .None-120 {background-color: var(--ptg-background); background-color:#ff0087; color:#8700ff}
-        .None-121 {background-color: var(--ptg-background); background-color:#afff00; color:#5fff87}
-        .None-122 {background-color: var(--ptg-background); background-color:#afffaf; color:#d7ffd7}
-        .None-123 {background-color: var(--ptg-background); background-color:#af00ff; color:#87d7af}
-        .None-124 {background-color: var(--ptg-background); background-color:#ff00af; color:#005f87}
-        .None-125 {background-color: var(--ptg-background); background-color:#5faf5f; color:#00ffaf}
-        .None-126 {background-color: var(--ptg-background); background-color:#87afaf; color:#af5f87}
-        .None-127 {background-color: var(--ptg-background); background-color:#ffafaf; color:#afffaf}
-        .None-128 {background-color: var(--ptg-background); background-color:#d7d787; color:#afd7af}
-        .None-129 {background-color: var(--ptg-background); background-color:#8700af; color:#afafaf}
-        .None-130 {background-color: var(--ptg-background); background-color:#87af5f; color:#afff00}
-        .None-131 {background-color: var(--ptg-background); background-color:#af005f; color:#5fafd7}
-        .None-132 {background-color: var(--ptg-background); background-color:#00af87; color:#00d75f}
-        .None-133 {background-color: var(--ptg-background); background-color:#afff87; color:#ffafd7}
-        .None-134 {background-color: var(--ptg-background); background-color:#ffafd7; color:#5fff00}
-        .None-135 {background-color: var(--ptg-background); background-color:#008787; color:#d7af5f}
-        .None-136 {background-color: var(--ptg-background); background-color:#ffaf87; color:#005f87}
-        .None-137 {background-color: var(--ptg-background); background-color:#ffafd7; color:#d7d787}
-        .None-138 {background-color: var(--ptg-background); background-color:#87af00; color:#00d7ff}
-        .None-139 {background-color: var(--ptg-background); background-color:#af00af; color:#875faf}
-        .None-140 {background-color: var(--ptg-background); background-color:#d787af; color:#87afff}
-        .None-141 {background-color: var(--ptg-background); background-color:#875f5f; color:#ff8787}
-        .None-142 {background-color: var(--ptg-background); background-color:#5f5faf; color:#878700}
-        .None-143 {background-color: var(--ptg-background); background-color:#d78787; color:#d7ffd7}
-        .None-144 {background-color: var(--ptg-background); background-color:#af0000; color:#87ff5f}
-        .None-145 {background-color: var(--ptg-background); background-color:#ff00d7; color:#d7ffaf}
-        .None-146 {background-color: var(--ptg-background); background-color:#5f0000; color:#ffaf00}
-        .None-147 {background-color: var(--ptg-background); background-color:#5faf87; color:#5f005f}
-        .None-148 {background-color: var(--ptg-background); background-color:#00ffaf; color:#005fff}
-        .None-149 {background-color: var(--ptg-background); background-color:#00875f; color:#5f0087}
-        .None-150 {background-color: var(--ptg-background); background-color:#000087; color:#d70087}
-        .None-151 {background-color: var(--ptg-background); background-color:#d7af00; color:#5fd7d7}
-        .None-152 {background-color: var(--ptg-background); background-color:#d75fff; color:#87d7d7}
-        .None-153 {background-color: var(--ptg-background); background-color:#ffff87; color:#87d7af}
-        .None-154 {background-color: var(--ptg-background); background-color:#d75f87; color:#ff87af}
-        .None-155 {background-color: var(--ptg-background); background-color:#afffaf; color:#87875f}
-        .None-156 {background-color: var(--ptg-background); background-color:#af5f5f; color:#5fd787}
-        .None-157 {background-color: var(--ptg-background); background-color:#afd787; color:#87afff}
-        .None-158 {background-color: var(--ptg-background); background-color:#5faf5f; color:#00ffd7}
-        .None-159 {background-color: var(--ptg-background); background-color:#ffd787; color:#d75faf}
-        .None-160 {background-color: var(--ptg-background); background-color:#870000; color:#5fffaf}
-        .None-161 {background-color: var(--ptg-background); background-color:#ffd700; color:#00ffd7}
-        .None-162 {background-color: var(--ptg-background); background-color:#87ff5f; color:#ffaf87}
-        .None-163 {background-color: var(--ptg-background); background-color:#d7d7af; color:#5fd787}
-        .None-164 {background-color: var(--ptg-background); background-color:#d70000; color:#d7afff}
-        .None-165 {background-color: var(--ptg-background); background-color:#afd7af; color:#0087ff}
-        .None-166 {background-color: var(--ptg-background); background-color:#87ff5f; color:#ffd700}
-        .None-167 {background-color: var(--ptg-background); background-color:#875f00; color:#afd7ff}
-        .None-168 {background-color: var(--ptg-background); background-color:#87ffaf; color:#ffff87}
-        .None-169 {background-color: var(--ptg-background); background-color:#ff5f87; color:#00afff}
-        .None-170 {background-color: var(--ptg-background); background-color:#5f8787; color:#af5f5f}
-        .None-171 {background-color: var(--ptg-background); background-color:#870000; color:#5fd7ff}
-        .None-172 {background-color: var(--ptg-background); background-color:#5fafaf; color:#875fff}
-        .None-173 {background-color: var(--ptg-background); background-color:#87d7af; color:#ffd7af}
-        .None-174 {background-color: var(--ptg-background); background-color:#878787; color:#ffff5f}
-        .None-175 {background-color: var(--ptg-background); background-color:#87d7af; color:#d7af00}
-        .None-176 {background-color: var(--ptg-background); background-color:#d7ff00; color:#5f0087}
-        .None-177 {background-color: var(--ptg-background); background-color:#ff00d7; color:#5f0000}
-        .None-178 {background-color: var(--ptg-background); background-color:#5f0000; color:#00afd7}
-        .None-179 {background-color: var(--ptg-background); background-color:#5fafff; color:#ff875f}
-        .None-180 {background-color: var(--ptg-background); background-color:#af00af; color:#8787ff}
-        .None-181 {background-color: var(--ptg-background); background-color:#00d787; color:#87af5f}
-        .None-182 {background-color: var(--ptg-background); background-color:#af0000; color:#5fffd7}
-        .None-183 {background-color: var(--ptg-background); background-color:#87af00; color:#af5f5f}
-        .None-184 {background-color: var(--ptg-background); background-color:#afaf00; color:#af87d7}
-        .None-185 {background-color: var(--ptg-background); background-color:#d7ff00; color:#af00af}
-        .None-186 {background-color: var(--ptg-background); background-color:#005f00; color:#5f8700}
-        .None-187 {background-color: var(--ptg-background); background-color:#080808; color:#005f87}
-        .None-188 {background-color: var(--ptg-background); background-color:#87005f; color:#ffffd7}
-        .None-189 {background-color: var(--ptg-background); background-color:#ffafaf; color:#0000af}
-        .None-190 {background-color: var(--ptg-background); background-color:#d7ff87; color:#878700}
-        .None-191 {background-color: var(--ptg-background); background-color:#ff87ff; color:#87af5f}
-        .None-192 {background-color: var(--ptg-background); background-color:#87005f; color:#87d700}
-        .None-193 {background-color: var(--ptg-background); background-color:#875f87; color:#ff5fff}
-        .None-194 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffaf00}
-        .None-195 {background-color: var(--ptg-background); background-color:#87d75f; color:#af0000}
-        .None-196 {background-color: var(--ptg-background); background-color:#d75f87; color:#af00d7}
-        .None-197 {background-color: var(--ptg-background); background-color:#87ff5f; color:#5fd7d7}
-        .None-198 {background-color: var(--ptg-background); background-color:#87ff00; color:#ff5f00}
-        .None-199 {background-color: var(--ptg-background); background-color:#5f5f5f; color:#af5f5f}
-        .None-200 {background-color: var(--ptg-background); background-color:#5fff5f; color:#d7af87}
-        .None-201 {background-color: var(--ptg-background); background-color:#d7d700; color:#005faf}
-        .None-202 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff875f}
-        .None-203 {background-color: var(--ptg-background); background-color:#87d700; color:#ff5fff}
-        .None-204 {background-color: var(--ptg-background); background-color:#5f5f87; color:#87afd7}
-        .None-205 {background-color: var(--ptg-background); background-color:#d7af5f; color:#af5f00}
-        .None-206 {background-color: var(--ptg-background); background-color:#d7ffaf; color:#5f87d7}
-        .None-207 {background-color: var(--ptg-background); background-color:#d75fd7; color:#0000af}
-        .None-208 {background-color: var(--ptg-background); background-color:#afafd7; color:#ffffff}
-        .None-209 {background-color: var(--ptg-background); background-color:#afd700; color:#af00d7}
-        .None-210 {background-color: var(--ptg-background); background-color:#875f5f; color:#ffaf5f}
-        .None-211 {background-color: var(--ptg-background); background-color:#5fafff; color:#af005f}
-        .None-212 {background-color: var(--ptg-background); background-color:#5fff5f; color:#d7d7ff}
-        .None-213 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ffff00}
-        .None-214 {background-color: var(--ptg-background); background-color:#d7d7af; color:#008787}
-        .None-215 {background-color: var(--ptg-background); background-color:#875f00; color:#5fd7ff}
-        .None-216 {background-color: var(--ptg-background); background-color:#5fafaf; color:#ff0087}
-        .None-217 {background-color: var(--ptg-background); background-color:#ff00d7; color:#080808}
-        .None-218 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#00005f}
-        .None-219 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#00af5f}
-        .None-220 {background-color: var(--ptg-background); background-color:#d7ffff; color:#00afaf}
-        .None-221 {background-color: var(--ptg-background); background-color:#ffff00; color:#d7af87}
-        .None-222 {background-color: var(--ptg-background); background-color:#5f5faf; color:#87d7d7}
-        .None-223 {background-color: var(--ptg-background); background-color:#d75f87; color:#d70000}
-        .None-224 {background-color: var(--ptg-background); background-color:#af00d7; color:#87d75f}
-        .None-225 {background-color: var(--ptg-background); background-color:#5f875f; color:#d787af}
-        .None-226 {background-color: var(--ptg-background); background-color:#87ffff; color:#00875f}
-        .None-227 {background-color: var(--ptg-background); background-color:#8700d7; color:#5fd700}
-        .None-228 {background-color: var(--ptg-background); background-color:#d7afff; color:#0087ff}
-        .None-229 {background-color: var(--ptg-background); background-color:#d70000; color:#00ff00}
-        .None-230 {background-color: var(--ptg-background); background-color:#00afff; color:#d787af}
-        .None-231 {background-color: var(--ptg-background); background-color:#ffff5f; color:#005fd7}
-        .None-232 {background-color: var(--ptg-background); background-color:#5faf00; color:#d7af00}
-        .None-233 {background-color: var(--ptg-background); background-color:#00afaf; color:#00ff87}
-        .None-234 {background-color: var(--ptg-background); background-color:#afffd7; color:#5f8787}
-        .None-235 {background-color: var(--ptg-background); background-color:#ffd75f; color:#5f8700}
-        .None-236 {background-color: var(--ptg-background); background-color:#afd7d7; color:#008787}
-        .None-237 {background-color: var(--ptg-background); background-color:#870087; color:#ff87af}
-        .None-238 {background-color: var(--ptg-background); background-color:#d787ff; color:#87ffff}
-        .None-239 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#ffaf5f}
-        .None-240 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7d7ff}
-        .None-241 {background-color: var(--ptg-background); background-color:#d7af00; color:#d700ff}
-        .None-242 {background-color: var(--ptg-background); background-color:#af00af; color:#ffd7d7}
-        .None-243 {background-color: var(--ptg-background); background-color:#87ffff; color:#d7af87}
-        .None-244 {background-color: var(--ptg-background); background-color:#87d700; color:#af5faf}
-        .None-245 {background-color: var(--ptg-background); background-color:#ff875f; color:#00d7af}
-        .None-246 {background-color: var(--ptg-background); background-color:#af87ff; color:#ff5f87}
-        .None-247 {background-color: var(--ptg-background); background-color:#0000af; color:#5fff5f}
-        .None-248 {background-color: var(--ptg-background); background-color:#875f00; color:#5fd787}
-        .None-249 {background-color: var(--ptg-background); background-color:#ffafd7; color:#5fff87}
-        .None-250 {background-color: var(--ptg-background); background-color:#d75fd7; color:#875fff}
-        .None-251 {background-color: var(--ptg-background); background-color:#5faf5f; color:#000087}
-        .None-252 {background-color: var(--ptg-background); background-color:#d75f5f; color:#ff87d7}
-        .None-253 {background-color: var(--ptg-background); background-color:#5f5f5f; color:#afaf87}
-        .None-254 {background-color: var(--ptg-background); background-color:#af5f5f; color:#87ff87}
-        .None-255 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#af5f00}
-        .None-256 {background-color: var(--ptg-background); background-color:#afafff; color:#87d700}
-        .None-257 {background-color: var(--ptg-background); background-color:#5f0000; color:#00ff5f}
-        .None-258 {background-color: var(--ptg-background); background-color:#005f00; color:#8787af}
-        .None-259 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#8787af}
-        .None-260 {background-color: var(--ptg-background); background-color:#afd787; color:#875faf}
-        .None-261 {background-color: var(--ptg-background); background-color:#005fd7; color:#00ffd7}
-        .None-262 {background-color: var(--ptg-background); background-color:#875f5f; color:#afaf5f}
-        .None-263 {background-color: var(--ptg-background); background-color:#00af00; color:#87afd7}
-        .None-264 {background-color: var(--ptg-background); background-color:#ff87d7; color:#875f87}
-        .None-265 {background-color: var(--ptg-background); background-color:#878787; color:#5faf87}
-        .None-266 {background-color: var(--ptg-background); background-color:#87ffaf; color:#5fff5f}
-        .None-267 {background-color: var(--ptg-background); background-color:#5f8787; color:#af5f00}
-        .None-268 {background-color: var(--ptg-background); background-color:#af5f87; color:#87afff}
-        .None-269 {background-color: var(--ptg-background); background-color:#00875f; color:#d7ffd7}
-        .None-270 {background-color: var(--ptg-background); background-color:#d7af87; color:#5fd75f}
-        .None-271 {background-color: var(--ptg-background); background-color:#875f87; color:#d70087}
-        .None-272 {background-color: var(--ptg-background); background-color:#5f5fff; color:#8700d7}
-        .None-273 {background-color: var(--ptg-background); background-color:#8700af; color:#5f875f}
-        .None-274 {background-color: var(--ptg-background); background-color:#ffffaf; color:#d7d787}
-        .None-275 {background-color: var(--ptg-background); background-color:#8787d7; color:#5f87d7}
-        .None-276 {background-color: var(--ptg-background); background-color:#00005f; color:#5fd7d7}
-        .None-277 {background-color: var(--ptg-background); background-color:#d7ffff; color:#d7d700}
-        .None-278 {background-color: var(--ptg-background); background-color:#ff87ff; color:#afafaf}
-        .None-279 {background-color: var(--ptg-background); background-color:#000087; color:#ffafaf}
-        .None-280 {background-color: var(--ptg-background); background-color:#5fafd7; color:#af0087}
-        .None-281 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#8787af}
-        .None-282 {background-color: var(--ptg-background); background-color:#5fafd7; color:#87afd7}
-        .None-283 {background-color: var(--ptg-background); background-color:#5f87ff; color:#005f87}
-        .None-284 {background-color: var(--ptg-background); background-color:#ff8787; color:#005faf}
-        .None-285 {background-color: var(--ptg-background); background-color:#ff5f87; color:#00ff87}
-        .None-286 {background-color: var(--ptg-background); background-color:#d7afff; color:#5fd7d7}
-        .None-287 {background-color: var(--ptg-background); background-color:#d75f00; color:#5fafd7}
-        .None-288 {background-color: var(--ptg-background); background-color:#5faf5f; color:#ff87d7}
-        .None-289 {background-color: var(--ptg-background); background-color:#00d75f; color:#870000}
-        .None-290 {background-color: var(--ptg-background); background-color:#afffff; color:#afd787}
-        .None-291 {background-color: var(--ptg-background); background-color:#080808; color:#d7d787}
-        .None-292 {background-color: var(--ptg-background); background-color:#af87ff; color:#00d75f}
-        .None-293 {background-color: var(--ptg-background); background-color:#00d7ff; color:#00ff87}
-        .None-294 {background-color: var(--ptg-background); background-color:#af5fff; color:#005f87}
-        .None-295 {background-color: var(--ptg-background); background-color:#d7005f; color:#d7ffd7}
-        .None-296 {background-color: var(--ptg-background); background-color:#ff005f; color:#ffafaf}
-        .None-297 {background-color: var(--ptg-background); background-color:#878700; color:#875f87}
-        .None-298 {background-color: var(--ptg-background); background-color:#ffff87; color:#5f5faf}
-        .None-299 {background-color: var(--ptg-background); background-color:#d75fd7; color:#0000d7}
-        .None-300 {background-color: var(--ptg-background); background-color:#87ff5f; color:#af87ff}
-        .None-301 {background-color: var(--ptg-background); background-color:#afd7af; color:#afaf00}
-        .None-302 {background-color: var(--ptg-background); background-color:#5fd7d7; color:#ffff87}
-        .None-303 {background-color: var(--ptg-background); background-color:#afffaf; color:#d75faf}
-        .None-304 {background-color: var(--ptg-background); background-color:#5fd75f; color:#00afff}
-        .None-305 {background-color: var(--ptg-background); background-color:#af00ff; color:#afd7af}
-        .None-306 {background-color: var(--ptg-background); background-color:#d7afff; color:#0000ff}
-        .None-307 {background-color: var(--ptg-background); background-color:#00d7af; color:#87d7ff}
-        .None-308 {background-color: var(--ptg-background); background-color:#d70087; color:#00d787}
-        .None-309 {background-color: var(--ptg-background); background-color:#d75f5f; color:#00d787}
-        .None-310 {background-color: var(--ptg-background); background-color:#ffff00; color:#87afd7}
-        .None-311 {background-color: var(--ptg-background); background-color:#5f87af; color:#d787af}
-        .None-312 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff5f00}
-        .None-313 {background-color: var(--ptg-background); background-color:#87d7ff; color:#080808}
-        .None-314 {background-color: var(--ptg-background); background-color:#af5f87; color:#ff8787}
-        .None-315 {background-color: var(--ptg-background); background-color:#875faf; color:#af00ff}
-        .None-316 {background-color: var(--ptg-background); background-color:#afd787; color:#5f00ff}
-        .None-317 {background-color: var(--ptg-background); background-color:#5fff87; color:#870000}
-        .None-318 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ffff5f}
-        .None-319 {background-color: var(--ptg-background); background-color:#5f8787; color:#5f00af}
-        .None-320 {background-color: var(--ptg-background); background-color:#ffd787; color:#5fd700}
-        .None-321 {background-color: var(--ptg-background); background-color:#00ff5f; color:#00af5f}
-        .None-322 {background-color: var(--ptg-background); background-color:#ff87ff; color:#ffd7af}
-        .None-323 {background-color: var(--ptg-background); background-color:#87d7ff; color:#87afff}
-        .None-324 {background-color: var(--ptg-background); background-color:#ff0087; color:#875f87}
-        .None-325 {background-color: var(--ptg-background); background-color:#87ff5f; color:#5fff00}
-        .None-326 {background-color: var(--ptg-background); background-color:#d7afaf; color:#00ff5f}
-        .None-327 {background-color: var(--ptg-background); background-color:#5faf87; color:#ffd7d7}
-        .None-328 {background-color: var(--ptg-background); background-color:#d7ff00; color:#5fafaf}
-        .None-329 {background-color: var(--ptg-background); background-color:#af5fd7; color:#87d75f}
-        .None-330 {background-color: var(--ptg-background); background-color:#af5faf; color:#87d7ff}
-        .None-331 {background-color: var(--ptg-background); background-color:#d7ffaf; color:#af87ff}
-        .None-332 {background-color: var(--ptg-background); background-color:#ffd700; color:#005f00}
-        .None-333 {background-color: var(--ptg-background); background-color:#d78787; color:#ffd700}
-        .None-334 {background-color: var(--ptg-background); background-color:#afffaf; color:#af5fff}
-        .None-335 {background-color: var(--ptg-background); background-color:#ff00d7; color:#5fff5f}
-        .None-336 {background-color: var(--ptg-background); background-color:#00ff87; color:#d7d75f}
-        .None-337 {background-color: var(--ptg-background); background-color:#ffffff; color:#ff8787}
-        .None-338 {background-color: var(--ptg-background); background-color:#afffaf; color:#005fd7}
-        .None-339 {background-color: var(--ptg-background); background-color:#ffff00; color:#5fafd7}
-        .None-340 {background-color: var(--ptg-background); background-color:#afff5f; color:#5f87af}
-        .None-341 {background-color: var(--ptg-background); background-color:#af00d7; color:#ffff5f}
-        .None-342 {background-color: var(--ptg-background); background-color:#afaf87; color:#af87af}
-        .None-343 {background-color: var(--ptg-background); background-color:#00d7d7; color:#080808}
-        .None-344 {background-color: var(--ptg-background); background-color:#5fafaf; color:#870087}
-        .None-345 {background-color: var(--ptg-background); background-color:#5fd7af; color:#d7ff87}
-        .None-346 {background-color: var(--ptg-background); background-color:#ff87af; color:#ffd7af}
-        .None-347 {background-color: var(--ptg-background); background-color:#afaf87; color:#d7ffd7}
-        .None-348 {background-color: var(--ptg-background); background-color:#00875f; color:#afaf00}
-        .None-349 {background-color: var(--ptg-background); background-color:#00d7d7; color:#87d7ff}
-        .None-350 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ff875f}
-        .None-351 {background-color: var(--ptg-background); background-color:#d7af00; color:#d7d700}
-        .None-352 {background-color: var(--ptg-background); background-color:#ff87ff; color:#5f5f5f}
-        .None-353 {background-color: var(--ptg-background); background-color:#87ffd7; color:#ffafff}
-        .None-354 {background-color: var(--ptg-background); background-color:#875f87; color:#5f5f5f}
-        .None-355 {background-color: var(--ptg-background); background-color:#ffffd7; color:#afafaf}
-        .None-356 {background-color: var(--ptg-background); background-color:#870087; color:#ffaf00}
-        .None-357 {background-color: var(--ptg-background); background-color:#87875f; color:#af5fd7}
-        .None-358 {background-color: var(--ptg-background); background-color:#ffaf87; color:#d7ff87}
-        .None-359 {background-color: var(--ptg-background); background-color:#5fd7ff; color:#5fafaf}
-        .None-360 {background-color: var(--ptg-background); background-color:#ff87d7; color:#00afff}
-        .None-361 {background-color: var(--ptg-background); background-color:#00005f; color:#d75faf}
-        .None-362 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#af0087}
-        .None-363 {background-color: var(--ptg-background); background-color:#875f5f; color:#5fd7d7}
-        .None-364 {background-color: var(--ptg-background); background-color:#af875f; color:#0000af}
-        .None-365 {background-color: var(--ptg-background); background-color:#5fffd7; color:#d7ff5f}
-        .None-366 {background-color: var(--ptg-background); background-color:#ff5fff; color:#d7d700}
-        .None-367 {background-color: var(--ptg-background); background-color:#ffd75f; color:#ffd75f}
-        .None-368 {background-color: var(--ptg-background); background-color:#afaf87; color:#af87ff}
-        .None-369 {background-color: var(--ptg-background); background-color:#ff00af; color:#d78700}
-        .None-370 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ffd7d7}
-        .None-371 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7afff}
-        .None-372 {background-color: var(--ptg-background); background-color:#af00af; color:#ffafff}
-        .None-373 {background-color: var(--ptg-background); background-color:#af87ff; color:#0000ff}
-        .None-374 {background-color: var(--ptg-background); background-color:#875faf; color:#d7afaf}
-        .None-375 {background-color: var(--ptg-background); background-color:#ffaf87; color:#00d7ff}
-        .None-376 {background-color: var(--ptg-background); background-color:#87ffaf; color:#d7ff5f}
-        .None-377 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#af5f87}
-        .None-378 {background-color: var(--ptg-background); background-color:#af8700; color:#d75fff}
-        .None-379 {background-color: var(--ptg-background); background-color:#00afff; color:#ff5f5f}
-        .None-380 {background-color: var(--ptg-background); background-color:#afaf00; color:#afff5f}
-        .None-381 {background-color: var(--ptg-background); background-color:#ff0087; color:#5f00ff}
-        .None-382 {background-color: var(--ptg-background); background-color:#878787; color:#af87ff}
-        .None-383 {background-color: var(--ptg-background); background-color:#d7afaf; color:#875fd7}
-        .None-384 {background-color: var(--ptg-background); background-color:#ffafd7; color:#00af87}
-        .None-385 {background-color: var(--ptg-background); background-color:#5f5fd7; color:#5f5faf}
-        .None-386 {background-color: var(--ptg-background); background-color:#5f5faf; color:#5f5fff}
-        .None-387 {background-color: var(--ptg-background); background-color:#5f87d7; color:#87d787}
-        .None-388 {background-color: var(--ptg-background); background-color:#d78787; color:#ff5f5f}
-        .None-389 {background-color: var(--ptg-background); background-color:#d78700; color:#d7ffd7}
-        .None-390 {background-color: var(--ptg-background); background-color:#d7ff87; color:#005faf}
-        .None-391 {background-color: var(--ptg-background); background-color:#af8787; color:#875f00}
-        .None-392 {background-color: var(--ptg-background); background-color:#5fff87; color:#875faf}
-        .None-393 {background-color: var(--ptg-background); background-color:#af875f; color:#00ffff}
-        .None-394 {background-color: var(--ptg-background); background-color:#d787af; color:#0087ff}
-        .None-395 {background-color: var(--ptg-background); background-color:#87afaf; color:#ff00af}
-        .None-396 {background-color: var(--ptg-background); background-color:#870000; color:#d75fd7}
-        .None-397 {background-color: var(--ptg-background); background-color:#8787af; color:#5f00ff}
-        .None-398 {background-color: var(--ptg-background); background-color:#d70087; color:#d700af}
-        .None-399 {background-color: var(--ptg-background); background-color:#5f87ff; color:#ffaf5f}
-        .None-400 {background-color: var(--ptg-background); background-color:#afff5f; color:#af00d7}
-        .None-401 {background-color: var(--ptg-background); background-color:#d7afff; color:#005fff}
-        .None-402 {background-color: var(--ptg-background); background-color:#0000d7; color:#afd7ff}
-        .None-403 {background-color: var(--ptg-background); background-color:#8700ff; color:#8787ff}
-        .None-404 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff87af}
-        .None-405 {background-color: var(--ptg-background); background-color:#5fffaf; color:#d75f87}
-        .None-406 {background-color: var(--ptg-background); background-color:#5f5fff; color:#080808}
-        .None-407 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#008700}
-        .None-408 {background-color: var(--ptg-background); background-color:#000087; color:#afafd7}
-        .None-409 {background-color: var(--ptg-background); background-color:#8700ff; color:#d7ffaf}
-        .None-410 {background-color: var(--ptg-background); background-color:#5f5faf; color:#5faf00}
-        .None-411 {background-color: var(--ptg-background); background-color:#00afd7; color:#d7af87}
-        .None-412 {background-color: var(--ptg-background); background-color:#ff87ff; color:#5f5faf}
-        .None-413 {background-color: var(--ptg-background); background-color:#00af00; color:#5f0087}
-        .None-414 {background-color: var(--ptg-background); background-color:#5f00d7; color:#d75f00}
-        .None-415 {background-color: var(--ptg-background); background-color:#5fffd7; color:#d7d7d7}
-        .None-416 {background-color: var(--ptg-background); background-color:#5f00af; color:#00d787}
-        .None-417 {background-color: var(--ptg-background); background-color:#ff00af; color:#5f5f00}
-        .None-418 {background-color: var(--ptg-background); background-color:#080808; color:#d7ffd7}
-        .None-419 {background-color: var(--ptg-background); background-color:#af8787; color:#d700ff}
-        .None-420 {background-color: var(--ptg-background); background-color:#5fafd7; color:#d7ff5f}
-        .None-421 {background-color: var(--ptg-background); background-color:#d7d7af; color:#00af87}
-        .None-422 {background-color: var(--ptg-background); background-color:#ff87af; color:#d75fff}
-        .None-423 {background-color: var(--ptg-background); background-color:#87afff; color:#d7afd7}
-        .None-424 {background-color: var(--ptg-background); background-color:#af5faf; color:#af00af}
-        .None-425 {background-color: var(--ptg-background); background-color:#af8787; color:#ffaf5f}
-        .None-426 {background-color: var(--ptg-background); background-color:#00afaf; color:#ff5fff}
-        .None-427 {background-color: var(--ptg-background); background-color:#ffd75f; color:#87d7af}
-        .None-428 {background-color: var(--ptg-background); background-color:#af875f; color:#af0000}
-        .None-429 {background-color: var(--ptg-background); background-color:#00afff; color:#008700}
-        .None-430 {background-color: var(--ptg-background); background-color:#5f8787; color:#87ffd7}
-        .None-431 {background-color: var(--ptg-background); background-color:#00ff87; color:#afafff}
-        .None-432 {background-color: var(--ptg-background); background-color:#ffaf00; color:#875fff}
-        .None-433 {background-color: var(--ptg-background); background-color:#ff8700; color:#875fd7}
-        .None-434 {background-color: var(--ptg-background); background-color:#ff875f; color:#ff5f5f}
-        .None-435 {background-color: var(--ptg-background); background-color:#87d7af; color:#005f5f}
-        .None-436 {background-color: var(--ptg-background); background-color:#87d7ff; color:#005fff}
-        .None-437 {background-color: var(--ptg-background); background-color:#ff5f00; color:#87af5f}
-        .None-438 {background-color: var(--ptg-background); background-color:#87ff87; color:#af8787}
-        .None-439 {background-color: var(--ptg-background); background-color:#005f87; color:#ff5fff}
-        .None-440 {background-color: var(--ptg-background); background-color:#d7d7ff; color:#87ffd7}
-        .None-441 {background-color: var(--ptg-background); background-color:#af875f; color:#d7afaf}
-        .None-442 {background-color: var(--ptg-background); background-color:#afd7af; color:#d7005f}
-        .None-443 {background-color: var(--ptg-background); background-color:#d75fd7; color:#5f005f}
-        .None-444 {background-color: var(--ptg-background); background-color:#ffd787; color:#5f5fd7}
-        .None-445 {background-color: var(--ptg-background); background-color:#5f00d7; color:#5f0000}
-        .None-446 {background-color: var(--ptg-background); background-color:#87d7ff; color:#00af5f}
-        .None-447 {background-color: var(--ptg-background); background-color:#af87ff; color:#5f5faf}
-        .None-448 {background-color: var(--ptg-background); color: var(--ptg-background);; background-color: var(--ptg-foreground); color:#af87ff; background-color:#5f5faf}
+        .0 {background-color: var(--ptg-background); background-color:#afaf00; color:#ffd787}
+        .1 {background-color: var(--ptg-background); background-color:#875f87; color:#5fff00}
+        .2 {background-color: var(--ptg-background); background-color:#af87af; color:#afaf5f}
+        .3 {background-color: var(--ptg-background); background-color:#0087d7; color:#ff00af}
+        .4 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ffd75f}
+        .5 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#5faf00}
+        .6 {background-color: var(--ptg-background); background-color:#ffaf00; color:#5f005f}
+        .7 {background-color: var(--ptg-background); background-color:#af00af; color:#00ffaf}
+        .8 {background-color: var(--ptg-background); background-color:#ff87af; color:#87ffd7}
+        .9 {background-color: var(--ptg-background); background-color:#005faf; color:#00af5f}
+        .10 {background-color: var(--ptg-background); background-color:#8700ff; color:#5f87ff}
+        .11 {background-color: var(--ptg-background); background-color:#5f5faf; color:#d70087}
+        .12 {background-color: var(--ptg-background); background-color:#5f5f87; color:#d75f5f}
+        .13 {background-color: var(--ptg-background); background-color:#8787af; color:#afafd7}
+        .14 {background-color: var(--ptg-background); background-color:#87afaf; color:#87d787}
+        .15 {background-color: var(--ptg-background); background-color:#afd787; color:#ff87ff}
+        .16 {background-color: var(--ptg-background); background-color:#00af87; color:#d7d75f}
+        .17 {background-color: var(--ptg-background); background-color:#d700ff; color:#d75f5f}
+        .18 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#87ff00}
+        .19 {background-color: var(--ptg-background); background-color:#8787af; color:#5f5fd7}
+        .20 {background-color: var(--ptg-background); background-color:#5f00af; color:#ff0000}
+        .21 {background-color: var(--ptg-background); background-color:#d75f5f; color:#d75fd7}
+        .22 {background-color: var(--ptg-background); background-color:#ff87d7; color:#00afd7}
+        .23 {background-color: var(--ptg-background); background-color:#5f0000; color:#ff5f87}
+        .24 {background-color: var(--ptg-background); background-color:#afd7af; color:#8700d7}
+        .25 {background-color: var(--ptg-background); background-color:#87d787; color:#00ff5f}
+        .26 {background-color: var(--ptg-background); background-color:#ff87ff; color:#ffafaf}
+        .27 {background-color: var(--ptg-background); background-color:#5f875f; color:#0000ff}
+        .28 {background-color: var(--ptg-background); background-color:#5f5f00; color:#00ffff}
+        .29 {background-color: var(--ptg-background); background-color:#87875f; color:#d75f5f}
+        .30 {background-color: var(--ptg-background); background-color:#d7af00; color:#d78787}
+        .31 {background-color: var(--ptg-background); background-color:#5fff5f; color:#ff0000}
+        .32 {background-color: var(--ptg-background); background-color:#d75f87; color:#5f5f5f}
+        .33 {background-color: var(--ptg-background); background-color:#ff87af; color:#afd700}
+        .34 {background-color: var(--ptg-background); background-color:#000087; color:#af5f00}
+        .35 {background-color: var(--ptg-background); background-color:#875f5f; color:#af0087}
+        .36 {background-color: var(--ptg-background); background-color:#ffd787; color:#005fff}
+        .37 {background-color: var(--ptg-background); background-color:#5f0000; color:#00ffff}
+        .38 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7af87}
+        .39 {background-color: var(--ptg-background); background-color:#d78700; color:#00ff5f}
+        .40 {background-color: var(--ptg-background); background-color:#5fff00; color:#afaf00}
+        .41 {background-color: var(--ptg-background); background-color:#afafff; color:#5f0087}
+        .42 {background-color: var(--ptg-background); background-color:#d7afaf; color:#8787d7}
+        .43 {background-color: var(--ptg-background); background-color:#d70087; color:#5f5fff}
+        .44 {background-color: var(--ptg-background); background-color:#87005f; color:#0000ff}
+        .45 {background-color: var(--ptg-background); background-color:#ffff00; color:#5fffff}
+        .46 {background-color: var(--ptg-background); background-color:#af8700; color:#87d75f}
+        .47 {background-color: var(--ptg-background); background-color:#8700d7; color:#d7d787}
+        .48 {background-color: var(--ptg-background); background-color:#008787; color:#afafd7}
+        .49 {background-color: var(--ptg-background); background-color:#5fff87; color:#ff87d7}
+        .50 {background-color: var(--ptg-background); background-color:#5f8787; color:#5f87ff}
+        .51 {background-color: var(--ptg-background); background-color:#d7afff; color:#af5fd7}
+        .52 {background-color: var(--ptg-background); background-color:#ffffaf; color:#afffaf}
+        .53 {background-color: var(--ptg-background); background-color:#878700; color:#87d7d7}
+        .54 {background-color: var(--ptg-background); background-color:#d70000; color:#ffff00}
+        .55 {background-color: var(--ptg-background); background-color:#5fff00; color:#5f5fff}
+        .56 {background-color: var(--ptg-background); background-color:#ffafd7; color:#ff0087}
+        .57 {background-color: var(--ptg-background); background-color:#ffd7af; color:#ffffff}
+        .58 {background-color: var(--ptg-background); background-color:#0087d7; color:#ffafff}
+        .59 {background-color: var(--ptg-background); background-color:#afd7ff; color:#ff00af}
+        .60 {background-color: var(--ptg-background); background-color:#d7af00; color:#00ff5f}
+        .61 {background-color: var(--ptg-background); background-color:#5f875f; color:#00d7d7}
+        .62 {background-color: var(--ptg-background); background-color:#00afff; color:#000087}
+        .63 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#00d7ff}
+        .64 {background-color: var(--ptg-background); background-color:#ffff00; color:#d7d7d7}
+        .65 {background-color: var(--ptg-background); background-color:#5fafff; color:#00ffaf}
+        .66 {background-color: var(--ptg-background); background-color:#afffff; color:#0087ff}
+        .67 {background-color: var(--ptg-background); background-color:#00d787; color:#5f0000}
+        .68 {background-color: var(--ptg-background); background-color:#afaf5f; color:#87ffff}
+        .69 {background-color: var(--ptg-background); background-color:#afff00; color:#ff87af}
+        .70 {background-color: var(--ptg-background); background-color:#ffff87; color:#5fff87}
+        .71 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ff8787}
+        .72 {background-color: var(--ptg-background); background-color:#8787d7; color:#afffff}
+        .73 {background-color: var(--ptg-background); background-color:#5fffaf; color:#d7ffff}
+        .74 {background-color: var(--ptg-background); background-color:#af00d7; color:#ffaf5f}
+        .75 {background-color: var(--ptg-background); background-color:#00ff87; color:#d78787}
+        .76 {background-color: var(--ptg-background); background-color:#d7ffff; color:#ff5fd7}
+        .77 {background-color: var(--ptg-background); background-color:#d7afff; color:#ffafff}
+        .78 {background-color: var(--ptg-background); background-color:#00d7af; color:#ff8700}
+        .79 {background-color: var(--ptg-background); background-color:#005f00; color:#00005f}
+        .80 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#ffd75f}
+        .81 {background-color: var(--ptg-background); background-color:#5f00af; color:#d75f5f}
+        .82 {background-color: var(--ptg-background); background-color:#d7ff00; color:#875f00}
+        .83 {background-color: var(--ptg-background); background-color:#5fffd7; color:#afffff}
+        .84 {background-color: var(--ptg-background); background-color:#0087af; color:#0000ff}
+        .85 {background-color: var(--ptg-background); background-color:#af87af; color:#d787af}
+        .86 {background-color: var(--ptg-background); background-color:#ffff87; color:#ffff00}
+        .87 {background-color: var(--ptg-background); background-color:#5f00af; color:#afd75f}
+        .88 {background-color: var(--ptg-background); background-color:#87d7ff; color:#d70000}
+        .89 {background-color: var(--ptg-background); background-color:#d7afd7; color:#d7af5f}
+        .90 {background-color: var(--ptg-background); background-color:#87afd7; color:#000087}
+        .91 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffd75f}
+        .92 {background-color: var(--ptg-background); background-color:#87ff87; color:#5fffaf}
+        .93 {background-color: var(--ptg-background); background-color:#af87af; color:#5f00af}
+        .94 {background-color: var(--ptg-background); background-color:#af00ff; color:#af0087}
+        .95 {background-color: var(--ptg-background); background-color:#87ffd7; color:#ff8787}
+        .96 {background-color: var(--ptg-background); background-color:#d7d7ff; color:#005f5f}
+        .97 {background-color: var(--ptg-background); background-color:#5faf87; color:#afaf00}
+        .98 {background-color: var(--ptg-background); background-color:#ff5faf; color:#5f5f5f}
+        .99 {background-color: var(--ptg-background); background-color:#afd787; color:#ffff87}
+        .100 {background-color: var(--ptg-background); background-color:#afd75f; color:#00ffaf}
+        .101 {background-color: var(--ptg-background); background-color:#ff00af; color:#af00d7}
+        .102 {background-color: var(--ptg-background); background-color:#00d7d7; color:#5f00ff}
+        .103 {background-color: var(--ptg-background); background-color:#5f5f87; color:#5fd7ff}
+        .104 {background-color: var(--ptg-background); background-color:#5fffaf; color:#5fd7af}
+        .105 {background-color: var(--ptg-background); background-color:#0087ff; color:#87ff87}
+        .106 {background-color: var(--ptg-background); background-color:#afafaf; color:#ffffff}
+        .107 {background-color: var(--ptg-background); background-color:#ff5fff; color:#87d700}
+        .108 {background-color: var(--ptg-background); background-color:#00afaf; color:#00afaf}
+        .109 {background-color: var(--ptg-background); background-color:#870000; color:#87ffff}
+        .110 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffafd7}
+        .111 {background-color: var(--ptg-background); background-color:#5faf00; color:#005f5f}
+        .112 {background-color: var(--ptg-background); background-color:#af87af; color:#af8787}
+        .113 {background-color: var(--ptg-background); background-color:#87d7af; color:#d75faf}
+        .114 {background-color: var(--ptg-background); background-color:#ff8700; color:#87005f}
+        .115 {background-color: var(--ptg-background); background-color:#d7d75f; color:#5fffd7}
+        .116 {background-color: var(--ptg-background); background-color:#5fd7d7; color:#00af5f}
+        .117 {background-color: var(--ptg-background); background-color:#d7005f; color:#d7ffaf}
+        .118 {background-color: var(--ptg-background); background-color:#afaf00; color:#d7d700}
+        .119 {background-color: var(--ptg-background); background-color:#00d7ff; color:#af0087}
+        .120 {background-color: var(--ptg-background); background-color:#ff0087; color:#8700ff}
+        .121 {background-color: var(--ptg-background); background-color:#afff00; color:#5fff87}
+        .122 {background-color: var(--ptg-background); background-color:#afffaf; color:#d7ffd7}
+        .123 {background-color: var(--ptg-background); background-color:#af00ff; color:#87d7af}
+        .124 {background-color: var(--ptg-background); background-color:#ff00af; color:#005f87}
+        .125 {background-color: var(--ptg-background); background-color:#5faf5f; color:#00ffaf}
+        .126 {background-color: var(--ptg-background); background-color:#87afaf; color:#af5f87}
+        .127 {background-color: var(--ptg-background); background-color:#ffafaf; color:#afffaf}
+        .128 {background-color: var(--ptg-background); background-color:#d7d787; color:#afd7af}
+        .129 {background-color: var(--ptg-background); background-color:#8700af; color:#afafaf}
+        .130 {background-color: var(--ptg-background); background-color:#87af5f; color:#afff00}
+        .131 {background-color: var(--ptg-background); background-color:#af005f; color:#5fafd7}
+        .132 {background-color: var(--ptg-background); background-color:#00af87; color:#00d75f}
+        .133 {background-color: var(--ptg-background); background-color:#afff87; color:#ffafd7}
+        .134 {background-color: var(--ptg-background); background-color:#ffafd7; color:#5fff00}
+        .135 {background-color: var(--ptg-background); background-color:#008787; color:#d7af5f}
+        .136 {background-color: var(--ptg-background); background-color:#ffaf87; color:#005f87}
+        .137 {background-color: var(--ptg-background); background-color:#ffafd7; color:#d7d787}
+        .138 {background-color: var(--ptg-background); background-color:#87af00; color:#00d7ff}
+        .139 {background-color: var(--ptg-background); background-color:#af00af; color:#875faf}
+        .140 {background-color: var(--ptg-background); background-color:#d787af; color:#87afff}
+        .141 {background-color: var(--ptg-background); background-color:#875f5f; color:#ff8787}
+        .142 {background-color: var(--ptg-background); background-color:#5f5faf; color:#878700}
+        .143 {background-color: var(--ptg-background); background-color:#d78787; color:#d7ffd7}
+        .144 {background-color: var(--ptg-background); background-color:#af0000; color:#87ff5f}
+        .145 {background-color: var(--ptg-background); background-color:#ff00d7; color:#d7ffaf}
+        .146 {background-color: var(--ptg-background); background-color:#5f0000; color:#ffaf00}
+        .147 {background-color: var(--ptg-background); background-color:#5faf87; color:#5f005f}
+        .148 {background-color: var(--ptg-background); background-color:#00ffaf; color:#005fff}
+        .149 {background-color: var(--ptg-background); background-color:#00875f; color:#5f0087}
+        .150 {background-color: var(--ptg-background); background-color:#000087; color:#d70087}
+        .151 {background-color: var(--ptg-background); background-color:#d7af00; color:#5fd7d7}
+        .152 {background-color: var(--ptg-background); background-color:#d75fff; color:#87d7d7}
+        .153 {background-color: var(--ptg-background); background-color:#ffff87; color:#87d7af}
+        .154 {background-color: var(--ptg-background); background-color:#d75f87; color:#ff87af}
+        .155 {background-color: var(--ptg-background); background-color:#afffaf; color:#87875f}
+        .156 {background-color: var(--ptg-background); background-color:#af5f5f; color:#5fd787}
+        .157 {background-color: var(--ptg-background); background-color:#afd787; color:#87afff}
+        .158 {background-color: var(--ptg-background); background-color:#5faf5f; color:#00ffd7}
+        .159 {background-color: var(--ptg-background); background-color:#ffd787; color:#d75faf}
+        .160 {background-color: var(--ptg-background); background-color:#870000; color:#5fffaf}
+        .161 {background-color: var(--ptg-background); background-color:#ffd700; color:#00ffd7}
+        .162 {background-color: var(--ptg-background); background-color:#87ff5f; color:#ffaf87}
+        .163 {background-color: var(--ptg-background); background-color:#d7d7af; color:#5fd787}
+        .164 {background-color: var(--ptg-background); background-color:#d70000; color:#d7afff}
+        .165 {background-color: var(--ptg-background); background-color:#afd7af; color:#0087ff}
+        .166 {background-color: var(--ptg-background); background-color:#87ff5f; color:#ffd700}
+        .167 {background-color: var(--ptg-background); background-color:#875f00; color:#afd7ff}
+        .168 {background-color: var(--ptg-background); background-color:#87ffaf; color:#ffff87}
+        .169 {background-color: var(--ptg-background); background-color:#ff5f87; color:#00afff}
+        .170 {background-color: var(--ptg-background); background-color:#5f8787; color:#af5f5f}
+        .171 {background-color: var(--ptg-background); background-color:#870000; color:#5fd7ff}
+        .172 {background-color: var(--ptg-background); background-color:#5fafaf; color:#875fff}
+        .173 {background-color: var(--ptg-background); background-color:#87d7af; color:#ffd7af}
+        .174 {background-color: var(--ptg-background); background-color:#878787; color:#ffff5f}
+        .175 {background-color: var(--ptg-background); background-color:#87d7af; color:#d7af00}
+        .176 {background-color: var(--ptg-background); background-color:#d7ff00; color:#5f0087}
+        .177 {background-color: var(--ptg-background); background-color:#ff00d7; color:#5f0000}
+        .178 {background-color: var(--ptg-background); background-color:#5f0000; color:#00afd7}
+        .179 {background-color: var(--ptg-background); background-color:#5fafff; color:#ff875f}
+        .180 {background-color: var(--ptg-background); background-color:#af00af; color:#8787ff}
+        .181 {background-color: var(--ptg-background); background-color:#00d787; color:#87af5f}
+        .182 {background-color: var(--ptg-background); background-color:#af0000; color:#5fffd7}
+        .183 {background-color: var(--ptg-background); background-color:#87af00; color:#af5f5f}
+        .184 {background-color: var(--ptg-background); background-color:#afaf00; color:#af87d7}
+        .185 {background-color: var(--ptg-background); background-color:#d7ff00; color:#af00af}
+        .186 {background-color: var(--ptg-background); background-color:#005f00; color:#5f8700}
+        .187 {background-color: var(--ptg-background); background-color:#080808; color:#005f87}
+        .188 {background-color: var(--ptg-background); background-color:#87005f; color:#ffffd7}
+        .189 {background-color: var(--ptg-background); background-color:#ffafaf; color:#0000af}
+        .190 {background-color: var(--ptg-background); background-color:#d7ff87; color:#878700}
+        .191 {background-color: var(--ptg-background); background-color:#ff87ff; color:#87af5f}
+        .192 {background-color: var(--ptg-background); background-color:#87005f; color:#87d700}
+        .193 {background-color: var(--ptg-background); background-color:#875f87; color:#ff5fff}
+        .194 {background-color: var(--ptg-background); background-color:#5f005f; color:#ffaf00}
+        .195 {background-color: var(--ptg-background); background-color:#87d75f; color:#af0000}
+        .196 {background-color: var(--ptg-background); background-color:#d75f87; color:#af00d7}
+        .197 {background-color: var(--ptg-background); background-color:#87ff5f; color:#5fd7d7}
+        .198 {background-color: var(--ptg-background); background-color:#87ff00; color:#ff5f00}
+        .199 {background-color: var(--ptg-background); background-color:#5f5f5f; color:#af5f5f}
+        .200 {background-color: var(--ptg-background); background-color:#5fff5f; color:#d7af87}
+        .201 {background-color: var(--ptg-background); background-color:#d7d700; color:#005faf}
+        .202 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff875f}
+        .203 {background-color: var(--ptg-background); background-color:#87d700; color:#ff5fff}
+        .204 {background-color: var(--ptg-background); background-color:#5f5f87; color:#87afd7}
+        .205 {background-color: var(--ptg-background); background-color:#d7af5f; color:#af5f00}
+        .206 {background-color: var(--ptg-background); background-color:#d7ffaf; color:#5f87d7}
+        .207 {background-color: var(--ptg-background); background-color:#d75fd7; color:#0000af}
+        .208 {background-color: var(--ptg-background); background-color:#afafd7; color:#ffffff}
+        .209 {background-color: var(--ptg-background); background-color:#afd700; color:#af00d7}
+        .210 {background-color: var(--ptg-background); background-color:#875f5f; color:#ffaf5f}
+        .211 {background-color: var(--ptg-background); background-color:#5fafff; color:#af005f}
+        .212 {background-color: var(--ptg-background); background-color:#5fff5f; color:#d7d7ff}
+        .213 {background-color: var(--ptg-background); background-color:#d7af5f; color:#ffff00}
+        .214 {background-color: var(--ptg-background); background-color:#d7d7af; color:#008787}
+        .215 {background-color: var(--ptg-background); background-color:#875f00; color:#5fd7ff}
+        .216 {background-color: var(--ptg-background); background-color:#5fafaf; color:#ff0087}
+        .217 {background-color: var(--ptg-background); background-color:#ff00d7; color:#080808}
+        .218 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#00005f}
+        .219 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#00af5f}
+        .220 {background-color: var(--ptg-background); background-color:#d7ffff; color:#00afaf}
+        .221 {background-color: var(--ptg-background); background-color:#ffff00; color:#d7af87}
+        .222 {background-color: var(--ptg-background); background-color:#5f5faf; color:#87d7d7}
+        .223 {background-color: var(--ptg-background); background-color:#d75f87; color:#d70000}
+        .224 {background-color: var(--ptg-background); background-color:#af00d7; color:#87d75f}
+        .225 {background-color: var(--ptg-background); background-color:#5f875f; color:#d787af}
+        .226 {background-color: var(--ptg-background); background-color:#87ffff; color:#00875f}
+        .227 {background-color: var(--ptg-background); background-color:#8700d7; color:#5fd700}
+        .228 {background-color: var(--ptg-background); background-color:#d7afff; color:#0087ff}
+        .229 {background-color: var(--ptg-background); background-color:#d70000; color:#00ff00}
+        .230 {background-color: var(--ptg-background); background-color:#00afff; color:#d787af}
+        .231 {background-color: var(--ptg-background); background-color:#ffff5f; color:#005fd7}
+        .232 {background-color: var(--ptg-background); background-color:#5faf00; color:#d7af00}
+        .233 {background-color: var(--ptg-background); background-color:#00afaf; color:#00ff87}
+        .234 {background-color: var(--ptg-background); background-color:#afffd7; color:#5f8787}
+        .235 {background-color: var(--ptg-background); background-color:#ffd75f; color:#5f8700}
+        .236 {background-color: var(--ptg-background); background-color:#afd7d7; color:#008787}
+        .237 {background-color: var(--ptg-background); background-color:#870087; color:#ff87af}
+        .238 {background-color: var(--ptg-background); background-color:#d787ff; color:#87ffff}
+        .239 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#ffaf5f}
+        .240 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7d7ff}
+        .241 {background-color: var(--ptg-background); background-color:#d7af00; color:#d700ff}
+        .242 {background-color: var(--ptg-background); background-color:#af00af; color:#ffd7d7}
+        .243 {background-color: var(--ptg-background); background-color:#87ffff; color:#d7af87}
+        .244 {background-color: var(--ptg-background); background-color:#87d700; color:#af5faf}
+        .245 {background-color: var(--ptg-background); background-color:#ff875f; color:#00d7af}
+        .246 {background-color: var(--ptg-background); background-color:#af87ff; color:#ff5f87}
+        .247 {background-color: var(--ptg-background); background-color:#0000af; color:#5fff5f}
+        .248 {background-color: var(--ptg-background); background-color:#875f00; color:#5fd787}
+        .249 {background-color: var(--ptg-background); background-color:#ffafd7; color:#5fff87}
+        .250 {background-color: var(--ptg-background); background-color:#d75fd7; color:#875fff}
+        .251 {background-color: var(--ptg-background); background-color:#5faf5f; color:#000087}
+        .252 {background-color: var(--ptg-background); background-color:#d75f5f; color:#ff87d7}
+        .253 {background-color: var(--ptg-background); background-color:#5f5f5f; color:#afaf87}
+        .254 {background-color: var(--ptg-background); background-color:#af5f5f; color:#87ff87}
+        .255 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#af5f00}
+        .256 {background-color: var(--ptg-background); background-color:#afafff; color:#87d700}
+        .257 {background-color: var(--ptg-background); background-color:#5f0000; color:#00ff5f}
+        .258 {background-color: var(--ptg-background); background-color:#005f00; color:#8787af}
+        .259 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#8787af}
+        .260 {background-color: var(--ptg-background); background-color:#afd787; color:#875faf}
+        .261 {background-color: var(--ptg-background); background-color:#005fd7; color:#00ffd7}
+        .262 {background-color: var(--ptg-background); background-color:#875f5f; color:#afaf5f}
+        .263 {background-color: var(--ptg-background); background-color:#00af00; color:#87afd7}
+        .264 {background-color: var(--ptg-background); background-color:#ff87d7; color:#875f87}
+        .265 {background-color: var(--ptg-background); background-color:#878787; color:#5faf87}
+        .266 {background-color: var(--ptg-background); background-color:#87ffaf; color:#5fff5f}
+        .267 {background-color: var(--ptg-background); background-color:#5f8787; color:#af5f00}
+        .268 {background-color: var(--ptg-background); background-color:#af5f87; color:#87afff}
+        .269 {background-color: var(--ptg-background); background-color:#00875f; color:#d7ffd7}
+        .270 {background-color: var(--ptg-background); background-color:#d7af87; color:#5fd75f}
+        .271 {background-color: var(--ptg-background); background-color:#875f87; color:#d70087}
+        .272 {background-color: var(--ptg-background); background-color:#5f5fff; color:#8700d7}
+        .273 {background-color: var(--ptg-background); background-color:#8700af; color:#5f875f}
+        .274 {background-color: var(--ptg-background); background-color:#ffffaf; color:#d7d787}
+        .275 {background-color: var(--ptg-background); background-color:#8787d7; color:#5f87d7}
+        .276 {background-color: var(--ptg-background); background-color:#00005f; color:#5fd7d7}
+        .277 {background-color: var(--ptg-background); background-color:#d7ffff; color:#d7d700}
+        .278 {background-color: var(--ptg-background); background-color:#ff87ff; color:#afafaf}
+        .279 {background-color: var(--ptg-background); background-color:#000087; color:#ffafaf}
+        .280 {background-color: var(--ptg-background); background-color:#5fafd7; color:#af0087}
+        .281 {background-color: var(--ptg-background); background-color:#d7d7d7; color:#8787af}
+        .282 {background-color: var(--ptg-background); background-color:#5fafd7; color:#87afd7}
+        .283 {background-color: var(--ptg-background); background-color:#5f87ff; color:#005f87}
+        .284 {background-color: var(--ptg-background); background-color:#ff8787; color:#005faf}
+        .285 {background-color: var(--ptg-background); background-color:#ff5f87; color:#00ff87}
+        .286 {background-color: var(--ptg-background); background-color:#d7afff; color:#5fd7d7}
+        .287 {background-color: var(--ptg-background); background-color:#d75f00; color:#5fafd7}
+        .288 {background-color: var(--ptg-background); background-color:#5faf5f; color:#ff87d7}
+        .289 {background-color: var(--ptg-background); background-color:#00d75f; color:#870000}
+        .290 {background-color: var(--ptg-background); background-color:#afffff; color:#afd787}
+        .291 {background-color: var(--ptg-background); background-color:#080808; color:#d7d787}
+        .292 {background-color: var(--ptg-background); background-color:#af87ff; color:#00d75f}
+        .293 {background-color: var(--ptg-background); background-color:#00d7ff; color:#00ff87}
+        .294 {background-color: var(--ptg-background); background-color:#af5fff; color:#005f87}
+        .295 {background-color: var(--ptg-background); background-color:#d7005f; color:#d7ffd7}
+        .296 {background-color: var(--ptg-background); background-color:#ff005f; color:#ffafaf}
+        .297 {background-color: var(--ptg-background); background-color:#878700; color:#875f87}
+        .298 {background-color: var(--ptg-background); background-color:#ffff87; color:#5f5faf}
+        .299 {background-color: var(--ptg-background); background-color:#d75fd7; color:#0000d7}
+        .300 {background-color: var(--ptg-background); background-color:#87ff5f; color:#af87ff}
+        .301 {background-color: var(--ptg-background); background-color:#afd7af; color:#afaf00}
+        .302 {background-color: var(--ptg-background); background-color:#5fd7d7; color:#ffff87}
+        .303 {background-color: var(--ptg-background); background-color:#afffaf; color:#d75faf}
+        .304 {background-color: var(--ptg-background); background-color:#5fd75f; color:#00afff}
+        .305 {background-color: var(--ptg-background); background-color:#af00ff; color:#afd7af}
+        .306 {background-color: var(--ptg-background); background-color:#d7afff; color:#0000ff}
+        .307 {background-color: var(--ptg-background); background-color:#00d7af; color:#87d7ff}
+        .308 {background-color: var(--ptg-background); background-color:#d70087; color:#00d787}
+        .309 {background-color: var(--ptg-background); background-color:#d75f5f; color:#00d787}
+        .310 {background-color: var(--ptg-background); background-color:#ffff00; color:#87afd7}
+        .311 {background-color: var(--ptg-background); background-color:#5f87af; color:#d787af}
+        .312 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff5f00}
+        .313 {background-color: var(--ptg-background); background-color:#87d7ff; color:#080808}
+        .314 {background-color: var(--ptg-background); background-color:#af5f87; color:#ff8787}
+        .315 {background-color: var(--ptg-background); background-color:#875faf; color:#af00ff}
+        .316 {background-color: var(--ptg-background); background-color:#afd787; color:#5f00ff}
+        .317 {background-color: var(--ptg-background); background-color:#5fff87; color:#870000}
+        .318 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ffff5f}
+        .319 {background-color: var(--ptg-background); background-color:#5f8787; color:#5f00af}
+        .320 {background-color: var(--ptg-background); background-color:#ffd787; color:#5fd700}
+        .321 {background-color: var(--ptg-background); background-color:#00ff5f; color:#00af5f}
+        .322 {background-color: var(--ptg-background); background-color:#ff87ff; color:#ffd7af}
+        .323 {background-color: var(--ptg-background); background-color:#87d7ff; color:#87afff}
+        .324 {background-color: var(--ptg-background); background-color:#ff0087; color:#875f87}
+        .325 {background-color: var(--ptg-background); background-color:#87ff5f; color:#5fff00}
+        .326 {background-color: var(--ptg-background); background-color:#d7afaf; color:#00ff5f}
+        .327 {background-color: var(--ptg-background); background-color:#5faf87; color:#ffd7d7}
+        .328 {background-color: var(--ptg-background); background-color:#d7ff00; color:#5fafaf}
+        .329 {background-color: var(--ptg-background); background-color:#af5fd7; color:#87d75f}
+        .330 {background-color: var(--ptg-background); background-color:#af5faf; color:#87d7ff}
+        .331 {background-color: var(--ptg-background); background-color:#d7ffaf; color:#af87ff}
+        .332 {background-color: var(--ptg-background); background-color:#ffd700; color:#005f00}
+        .333 {background-color: var(--ptg-background); background-color:#d78787; color:#ffd700}
+        .334 {background-color: var(--ptg-background); background-color:#afffaf; color:#af5fff}
+        .335 {background-color: var(--ptg-background); background-color:#ff00d7; color:#5fff5f}
+        .336 {background-color: var(--ptg-background); background-color:#00ff87; color:#d7d75f}
+        .337 {background-color: var(--ptg-background); background-color:#ffffff; color:#ff8787}
+        .338 {background-color: var(--ptg-background); background-color:#afffaf; color:#005fd7}
+        .339 {background-color: var(--ptg-background); background-color:#ffff00; color:#5fafd7}
+        .340 {background-color: var(--ptg-background); background-color:#afff5f; color:#5f87af}
+        .341 {background-color: var(--ptg-background); background-color:#af00d7; color:#ffff5f}
+        .342 {background-color: var(--ptg-background); background-color:#afaf87; color:#af87af}
+        .343 {background-color: var(--ptg-background); background-color:#00d7d7; color:#080808}
+        .344 {background-color: var(--ptg-background); background-color:#5fafaf; color:#870087}
+        .345 {background-color: var(--ptg-background); background-color:#5fd7af; color:#d7ff87}
+        .346 {background-color: var(--ptg-background); background-color:#ff87af; color:#ffd7af}
+        .347 {background-color: var(--ptg-background); background-color:#afaf87; color:#d7ffd7}
+        .348 {background-color: var(--ptg-background); background-color:#00875f; color:#afaf00}
+        .349 {background-color: var(--ptg-background); background-color:#00d7d7; color:#87d7ff}
+        .350 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ff875f}
+        .351 {background-color: var(--ptg-background); background-color:#d7af00; color:#d7d700}
+        .352 {background-color: var(--ptg-background); background-color:#ff87ff; color:#5f5f5f}
+        .353 {background-color: var(--ptg-background); background-color:#87ffd7; color:#ffafff}
+        .354 {background-color: var(--ptg-background); background-color:#875f87; color:#5f5f5f}
+        .355 {background-color: var(--ptg-background); background-color:#ffffd7; color:#afafaf}
+        .356 {background-color: var(--ptg-background); background-color:#870087; color:#ffaf00}
+        .357 {background-color: var(--ptg-background); background-color:#87875f; color:#af5fd7}
+        .358 {background-color: var(--ptg-background); background-color:#ffaf87; color:#d7ff87}
+        .359 {background-color: var(--ptg-background); background-color:#5fd7ff; color:#5fafaf}
+        .360 {background-color: var(--ptg-background); background-color:#ff87d7; color:#00afff}
+        .361 {background-color: var(--ptg-background); background-color:#00005f; color:#d75faf}
+        .362 {background-color: var(--ptg-background); background-color:#d7ffd7; color:#af0087}
+        .363 {background-color: var(--ptg-background); background-color:#875f5f; color:#5fd7d7}
+        .364 {background-color: var(--ptg-background); background-color:#af875f; color:#0000af}
+        .365 {background-color: var(--ptg-background); background-color:#5fffd7; color:#d7ff5f}
+        .366 {background-color: var(--ptg-background); background-color:#ff5fff; color:#d7d700}
+        .367 {background-color: var(--ptg-background); background-color:#ffd75f; color:#ffd75f}
+        .368 {background-color: var(--ptg-background); background-color:#afaf87; color:#af87ff}
+        .369 {background-color: var(--ptg-background); background-color:#ff00af; color:#d78700}
+        .370 {background-color: var(--ptg-background); background-color:#00d7ff; color:#ffd7d7}
+        .371 {background-color: var(--ptg-background); background-color:#ff5faf; color:#d7afff}
+        .372 {background-color: var(--ptg-background); background-color:#af00af; color:#ffafff}
+        .373 {background-color: var(--ptg-background); background-color:#af87ff; color:#0000ff}
+        .374 {background-color: var(--ptg-background); background-color:#875faf; color:#d7afaf}
+        .375 {background-color: var(--ptg-background); background-color:#ffaf87; color:#00d7ff}
+        .376 {background-color: var(--ptg-background); background-color:#87ffaf; color:#d7ff5f}
+        .377 {background-color: var(--ptg-background); background-color:#ffd7d7; color:#af5f87}
+        .378 {background-color: var(--ptg-background); background-color:#af8700; color:#d75fff}
+        .379 {background-color: var(--ptg-background); background-color:#00afff; color:#ff5f5f}
+        .380 {background-color: var(--ptg-background); background-color:#afaf00; color:#afff5f}
+        .381 {background-color: var(--ptg-background); background-color:#ff0087; color:#5f00ff}
+        .382 {background-color: var(--ptg-background); background-color:#878787; color:#af87ff}
+        .383 {background-color: var(--ptg-background); background-color:#d7afaf; color:#875fd7}
+        .384 {background-color: var(--ptg-background); background-color:#ffafd7; color:#00af87}
+        .385 {background-color: var(--ptg-background); background-color:#5f5fd7; color:#5f5faf}
+        .386 {background-color: var(--ptg-background); background-color:#5f5faf; color:#5f5fff}
+        .387 {background-color: var(--ptg-background); background-color:#5f87d7; color:#87d787}
+        .388 {background-color: var(--ptg-background); background-color:#d78787; color:#ff5f5f}
+        .389 {background-color: var(--ptg-background); background-color:#d78700; color:#d7ffd7}
+        .390 {background-color: var(--ptg-background); background-color:#d7ff87; color:#005faf}
+        .391 {background-color: var(--ptg-background); background-color:#af8787; color:#875f00}
+        .392 {background-color: var(--ptg-background); background-color:#5fff87; color:#875faf}
+        .393 {background-color: var(--ptg-background); background-color:#af875f; color:#00ffff}
+        .394 {background-color: var(--ptg-background); background-color:#d787af; color:#0087ff}
+        .395 {background-color: var(--ptg-background); background-color:#87afaf; color:#ff00af}
+        .396 {background-color: var(--ptg-background); background-color:#870000; color:#d75fd7}
+        .397 {background-color: var(--ptg-background); background-color:#8787af; color:#5f00ff}
+        .398 {background-color: var(--ptg-background); background-color:#d70087; color:#d700af}
+        .399 {background-color: var(--ptg-background); background-color:#5f87ff; color:#ffaf5f}
+        .400 {background-color: var(--ptg-background); background-color:#afff5f; color:#af00d7}
+        .401 {background-color: var(--ptg-background); background-color:#d7afff; color:#005fff}
+        .402 {background-color: var(--ptg-background); background-color:#0000d7; color:#afd7ff}
+        .403 {background-color: var(--ptg-background); background-color:#8700ff; color:#8787ff}
+        .404 {background-color: var(--ptg-background); background-color:#5fd75f; color:#ff87af}
+        .405 {background-color: var(--ptg-background); background-color:#5fffaf; color:#d75f87}
+        .406 {background-color: var(--ptg-background); background-color:#5f5fff; color:#080808}
+        .407 {background-color: var(--ptg-background); background-color:#d7ff5f; color:#008700}
+        .408 {background-color: var(--ptg-background); background-color:#000087; color:#afafd7}
+        .409 {background-color: var(--ptg-background); background-color:#8700ff; color:#d7ffaf}
+        .410 {background-color: var(--ptg-background); background-color:#5f5faf; color:#5faf00}
+        .411 {background-color: var(--ptg-background); background-color:#00afd7; color:#d7af87}
+        .412 {background-color: var(--ptg-background); background-color:#ff87ff; color:#5f5faf}
+        .413 {background-color: var(--ptg-background); background-color:#00af00; color:#5f0087}
+        .414 {background-color: var(--ptg-background); background-color:#5f00d7; color:#d75f00}
+        .415 {background-color: var(--ptg-background); background-color:#5fffd7; color:#d7d7d7}
+        .416 {background-color: var(--ptg-background); background-color:#5f00af; color:#00d787}
+        .417 {background-color: var(--ptg-background); background-color:#ff00af; color:#5f5f00}
+        .418 {background-color: var(--ptg-background); background-color:#080808; color:#d7ffd7}
+        .419 {background-color: var(--ptg-background); background-color:#af8787; color:#d700ff}
+        .420 {background-color: var(--ptg-background); background-color:#5fafd7; color:#d7ff5f}
+        .421 {background-color: var(--ptg-background); background-color:#d7d7af; color:#00af87}
+        .422 {background-color: var(--ptg-background); background-color:#ff87af; color:#d75fff}
+        .423 {background-color: var(--ptg-background); background-color:#87afff; color:#d7afd7}
+        .424 {background-color: var(--ptg-background); background-color:#af5faf; color:#af00af}
+        .425 {background-color: var(--ptg-background); background-color:#af8787; color:#ffaf5f}
+        .426 {background-color: var(--ptg-background); background-color:#00afaf; color:#ff5fff}
+        .427 {background-color: var(--ptg-background); background-color:#ffd75f; color:#87d7af}
+        .428 {background-color: var(--ptg-background); background-color:#af875f; color:#af0000}
+        .429 {background-color: var(--ptg-background); background-color:#00afff; color:#008700}
+        .430 {background-color: var(--ptg-background); background-color:#5f8787; color:#87ffd7}
+        .431 {background-color: var(--ptg-background); background-color:#00ff87; color:#afafff}
+        .432 {background-color: var(--ptg-background); background-color:#ffaf00; color:#875fff}
+        .433 {background-color: var(--ptg-background); background-color:#ff8700; color:#875fd7}
+        .434 {background-color: var(--ptg-background); background-color:#ff875f; color:#ff5f5f}
+        .435 {background-color: var(--ptg-background); background-color:#87d7af; color:#005f5f}
+        .436 {background-color: var(--ptg-background); background-color:#87d7ff; color:#005fff}
+        .437 {background-color: var(--ptg-background); background-color:#ff5f00; color:#87af5f}
+        .438 {background-color: var(--ptg-background); background-color:#87ff87; color:#af8787}
+        .439 {background-color: var(--ptg-background); background-color:#005f87; color:#ff5fff}
+        .440 {background-color: var(--ptg-background); background-color:#d7d7ff; color:#87ffd7}
+        .441 {background-color: var(--ptg-background); background-color:#af875f; color:#d7afaf}
+        .442 {background-color: var(--ptg-background); background-color:#afd7af; color:#d7005f}
+        .443 {background-color: var(--ptg-background); background-color:#d75fd7; color:#5f005f}
+        .444 {background-color: var(--ptg-background); background-color:#ffd787; color:#5f5fd7}
+        .445 {background-color: var(--ptg-background); background-color:#5f00d7; color:#5f0000}
+        .446 {background-color: var(--ptg-background); background-color:#87d7ff; color:#00af5f}
+        .447 {background-color: var(--ptg-background); background-color:#af87ff; color:#5f5faf}
+        .448 {background-color: var(--ptg-background); color: var(--ptg-background);; background-color: var(--ptg-foreground); color:#af87ff; background-color:#5f5faf}
         </style>
     </head>
     <body>
         <pre class="ptg">
             <code>
-<span class='None-0'>▄</span><span class='None-1'>▄</span><span class='None-2'>▄</span><span class='None-3'>▄</span><span class='None-4'>▄</span><span class='None-5'>▄</span><span class='None-6'>▄</span><span class='None-7'>▄</span><span class='None-8'>▄</span><span class='None-9'>▄</span><span class='None-10'>▄</span><span class='None-11'>▄</span><span class='None-12'>▄</span><span class='None-13'>▄</span><span class='None-14'>▄</span><span class='None-15'>▄</span><span class='None-16'>▄</span><span class='None-17'>▄</span><span class='None-18'>▄</span><span class='None-19'>▄</span><span class='None-20'>▄</span><span class='None-21'>▄</span><span class='None-22'>▄</span><span class='None-23'>▄</span><span class='None-24'>▄</span><span class='None-25'>▄</span><span class='None-26'>▄</span><span class='None-27'>▄</span><span class='None-28'>▄</span><span class='None-29'>▄</span>
-<span class='None-30'>▄</span><span class='None-31'>▄</span><span class='None-32'>▄</span><span class='None-33'>▄</span><span class='None-34'>▄</span><span class='None-35'>▄</span><span class='None-36'>▄</span><span class='None-37'>▄</span><span class='None-38'>▄</span><span class='None-39'>▄</span><span class='None-40'>▄</span><span class='None-41'>▄</span><span class='None-42'>▄</span><span class='None-43'>▄</span><span class='None-44'>▄</span><span class='None-45'>▄</span><span class='None-46'>▄</span><span class='None-47'>▄</span><span class='None-48'>▄</span><span class='None-49'>▄</span><span class='None-50'>▄</span><span class='None-51'>▄</span><span class='None-52'>▄</span><span class='None-53'>▄</span><span class='None-54'>▄</span><span class='None-55'>▄</span><span class='None-56'>▄</span><span class='None-57'>▄</span><span class='None-58'>▄</span><span class='None-59'>▄</span>
-<span class='None-60'>▄</span><span class='None-61'>▄</span><span class='None-62'>▄</span><span class='None-63'>▄</span><span class='None-64'>▄</span><span class='None-65'>▄</span><span class='None-66'>▄</span><span class='None-67'>▄</span><span class='None-68'>▄</span><span class='None-69'>▄</span><span class='None-70'>▄</span><span class='None-71'>▄</span><span class='None-72'>▄</span><span class='None-73'>▄</span><span class='None-74'>▄</span><span class='None-75'>▄</span><span class='None-76'>▄</span><span class='None-77'>▄</span><span class='None-78'>▄</span><span class='None-79'>▄</span><span class='None-80'>▄</span><span class='None-81'>▄</span><span class='None-82'>▄</span><span class='None-83'>▄</span><span class='None-84'>▄</span><span class='None-85'>▄</span><span class='None-86'>▄</span><span class='None-87'>▄</span><span class='None-88'>▄</span><span class='None-89'>▄</span>
-<span class='None-90'>▄</span><span class='None-91'>▄</span><span class='None-92'>▄</span><span class='None-93'>▄</span><span class='None-94'>▄</span><span class='None-95'>▄</span><span class='None-96'>▄</span><span class='None-97'>▄</span><span class='None-98'>▄</span><span class='None-99'>▄</span><span class='None-100'>▄</span><span class='None-101'>▄</span><span class='None-102'>▄</span><span class='None-103'>▄</span><span class='None-104'>▄</span><span class='None-105'>▄</span><span class='None-106'>▄</span><span class='None-107'>▄</span><span class='None-108'>▄</span><span class='None-109'>▄</span><span class='None-110'>▄</span><span class='None-111'>▄</span><span class='None-112'>▄</span><span class='None-113'>▄</span><span class='None-114'>▄</span><span class='None-115'>▄</span><span class='None-116'>▄</span><span class='None-117'>▄</span><span class='None-118'>▄</span><span class='None-119'>▄</span>
-<span class='None-120'>▄</span><span class='None-121'>▄</span><span class='None-122'>▄</span><span class='None-123'>▄</span><span class='None-124'>▄</span><span class='None-125'>▄</span><span class='None-126'>▄</span><span class='None-127'>▄</span><span class='None-128'>▄</span><span class='None-129'>▄</span><span class='None-130'>▄</span><span class='None-131'>▄</span><span class='None-132'>▄</span><span class='None-133'>▄</span><span class='None-134'>▄</span><span class='None-135'>▄</span><span class='None-136'>▄</span><span class='None-137'>▄</span><span class='None-138'>▄</span><span class='None-139'>▄</span><span class='None-140'>▄</span><span class='None-141'>▄</span><span class='None-142'>▄</span><span class='None-143'>▄</span><span class='None-144'>▄</span><span class='None-145'>▄</span><span class='None-146'>▄</span><span class='None-147'>▄</span><span class='None-148'>▄</span><span class='None-149'>▄</span>
-<span class='None-150'>▄</span><span class='None-151'>▄</span><span class='None-152'>▄</span><span class='None-153'>▄</span><span class='None-154'>▄</span><span class='None-155'>▄</span><span class='None-156'>▄</span><span class='None-157'>▄</span><span class='None-158'>▄</span><span class='None-159'>▄</span><span class='None-160'>▄</span><span class='None-161'>▄</span><span class='None-162'>▄</span><span class='None-163'>▄</span><span class='None-164'>▄</span><span class='None-165'>▄</span><span class='None-166'>▄</span><span class='None-167'>▄</span><span class='None-168'>▄</span><span class='None-169'>▄</span><span class='None-170'>▄</span><span class='None-171'>▄</span><span class='None-172'>▄</span><span class='None-173'>▄</span><span class='None-174'>▄</span><span class='None-175'>▄</span><span class='None-176'>▄</span><span class='None-177'>▄</span><span class='None-178'>▄</span><span class='None-179'>▄</span>
-<span class='None-180'>▄</span><span class='None-181'>▄</span><span class='None-182'>▄</span><span class='None-183'>▄</span><span class='None-184'>▄</span><span class='None-185'>▄</span><span class='None-186'>▄</span><span class='None-187'>▄</span><span class='None-188'>▄</span><span class='None-189'>▄</span><span class='None-190'>▄</span><span class='None-191'>▄</span><span class='None-192'>▄</span><span class='None-193'>▄</span><span class='None-194'>▄</span><span class='None-195'>▄</span><span class='None-196'>▄</span><span class='None-197'>▄</span><span class='None-198'>▄</span><span class='None-199'>▄</span><span class='None-200'>▄</span><span class='None-201'>▄</span><span class='None-202'>▄</span><span class='None-203'>▄</span><span class='None-204'>▄</span><span class='None-205'>▄</span><span class='None-206'>▄</span><span class='None-207'>▄</span><span class='None-208'>▄</span><span class='None-209'>▄</span>
-<span class='None-210'>▄</span><span class='None-211'>▄</span><span class='None-212'>▄</span><span class='None-213'>▄</span><span class='None-214'>▄</span><span class='None-215'>▄</span><span class='None-216'>▄</span><span class='None-217'>▄</span><span class='None-218'>▄</span><span class='None-219'>▄</span><span class='None-220'>▄</span><span class='None-221'>▄</span><span class='None-222'>▄</span><span class='None-223'>▄</span><span class='None-224'>▄</span><span class='None-225'>▄</span><span class='None-226'>▄</span><span class='None-227'>▄</span><span class='None-228'>▄</span><span class='None-229'>▄</span><span class='None-230'>▄</span><span class='None-231'>▄</span><span class='None-232'>▄</span><span class='None-233'>▄</span><span class='None-234'>▄</span><span class='None-235'>▄</span><span class='None-236'>▄</span><span class='None-237'>▄</span><span class='None-238'>▄</span><span class='None-239'>▄</span>
-<span class='None-240'>▄</span><span class='None-241'>▄</span><span class='None-242'>▄</span><span class='None-243'>▄</span><span class='None-244'>▄</span><span class='None-245'>▄</span><span class='None-246'>▄</span><span class='None-247'>▄</span><span class='None-248'>▄</span><span class='None-249'>▄</span><span class='None-250'>▄</span><span class='None-251'>▄</span><span class='None-252'>▄</span><span class='None-253'>▄</span><span class='None-254'>▄</span><span class='None-255'>▄</span><span class='None-256'>▄</span><span class='None-257'>▄</span><span class='None-258'>▄</span><span class='None-259'>▄</span><span class='None-260'>▄</span><span class='None-261'>▄</span><span class='None-262'>▄</span><span class='None-263'>▄</span><span class='None-264'>▄</span><span class='None-265'>▄</span><span class='None-266'>▄</span><span class='None-267'>▄</span><span class='None-268'>▄</span><span class='None-269'>▄</span>
-<span class='None-270'>▄</span><span class='None-271'>▄</span><span class='None-272'>▄</span><span class='None-273'>▄</span><span class='None-37'>▄</span><span class='None-274'>▄</span><span class='None-275'>▄</span><span class='None-276'>▄</span><span class='None-277'>▄</span><span class='None-278'>▄</span><span class='None-279'>▄</span><span class='None-280'>▄</span><span class='None-281'>▄</span><span class='None-282'>▄</span><span class='None-283'>▄</span><span class='None-284'>▄</span><span class='None-285'>▄</span><span class='None-286'>▄</span><span class='None-287'>▄</span><span class='None-288'>▄</span><span class='None-289'>▄</span><span class='None-290'>▄</span><span class='None-291'>▄</span><span class='None-292'>▄</span><span class='None-293'>▄</span><span class='None-294'>▄</span><span class='None-295'>▄</span><span class='None-296'>▄</span><span class='None-297'>▄</span><span class='None-298'>▄</span>
-<span class='None-299'>▄</span><span class='None-300'>▄</span><span class='None-301'>▄</span><span class='None-302'>▄</span><span class='None-303'>▄</span><span class='None-304'>▄</span><span class='None-305'>▄</span><span class='None-306'>▄</span><span class='None-307'>▄</span><span class='None-308'>▄</span><span class='None-309'>▄</span><span class='None-310'>▄</span><span class='None-311'>▄</span><span class='None-312'>▄</span><span class='None-313'>▄</span><span class='None-314'>▄</span><span class='None-315'>▄</span><span class='None-316'>▄</span><span class='None-248'>▄</span><span class='None-317'>▄</span><span class='None-318'>▄</span><span class='None-319'>▄</span><span class='None-320'>▄</span><span class='None-321'>▄</span><span class='None-322'>▄</span><span class='None-323'>▄</span><span class='None-324'>▄</span><span class='None-325'>▄</span><span class='None-326'>▄</span><span class='None-327'>▄</span>
-<span class='None-328'>▄</span><span class='None-329'>▄</span><span class='None-330'>▄</span><span class='None-331'>▄</span><span class='None-332'>▄</span><span class='None-333'>▄</span><span class='None-334'>▄</span><span class='None-335'>▄</span><span class='None-336'>▄</span><span class='None-337'>▄</span><span class='None-338'>▄</span><span class='None-339'>▄</span><span class='None-340'>▄</span><span class='None-341'>▄</span><span class='None-342'>▄</span><span class='None-337'>▄</span><span class='None-343'>▄</span><span class='None-344'>▄</span><span class='None-345'>▄</span><span class='None-346'>▄</span><span class='None-347'>▄</span><span class='None-348'>▄</span><span class='None-349'>▄</span><span class='None-350'>▄</span><span class='None-351'>▄</span><span class='None-352'>▄</span><span class='None-353'>▄</span><span class='None-354'>▄</span><span class='None-355'>▄</span><span class='None-356'>▄</span>
-<span class='None-357'>▄</span><span class='None-358'>▄</span><span class='None-359'>▄</span><span class='None-360'>▄</span><span class='None-361'>▄</span><span class='None-362'>▄</span><span class='None-363'>▄</span><span class='None-364'>▄</span><span class='None-365'>▄</span><span class='None-366'>▄</span><span class='None-367'>▄</span><span class='None-368'>▄</span><span class='None-369'>▄</span><span class='None-370'>▄</span><span class='None-371'>▄</span><span class='None-372'>▄</span><span class='None-373'>▄</span><span class='None-374'>▄</span><span class='None-375'>▄</span><span class='None-376'>▄</span><span class='None-377'>▄</span><span class='None-378'>▄</span><span class='None-379'>▄</span><span class='None-380'>▄</span><span class='None-381'>▄</span><span class='None-382'>▄</span><span class='None-383'>▄</span><span class='None-384'>▄</span><span class='None-385'>▄</span><span class='None-386'>▄</span>
-<span class='None-387'>▄</span><span class='None-388'>▄</span><span class='None-389'>▄</span><span class='None-390'>▄</span><span class='None-391'>▄</span><span class='None-392'>▄</span><span class='None-393'>▄</span><span class='None-394'>▄</span><span class='None-395'>▄</span><span class='None-396'>▄</span><span class='None-397'>▄</span><span class='None-398'>▄</span><span class='None-399'>▄</span><span class='None-400'>▄</span><span class='None-401'>▄</span><span class='None-402'>▄</span><span class='None-403'>▄</span><span class='None-404'>▄</span><span class='None-405'>▄</span><span class='None-406'>▄</span><span class='None-407'>▄</span><span class='None-408'>▄</span><span class='None-409'>▄</span><span class='None-410'>▄</span><span class='None-411'>▄</span><span class='None-412'>▄</span><span class='None-413'>▄</span><span class='None-414'>▄</span><span class='None-415'>▄</span><span class='None-416'>▄</span>
-<span class='None-417'>▄</span><span class='None-418'>▄</span><span class='None-419'>▄</span><span class='None-420'>▄</span><span class='None-421'>▄</span><span class='None-422'>▄</span><span class='None-423'>▄</span><span class='None-424'>▄</span><span class='None-425'>▄</span><span class='None-426'>▄</span><span class='None-427'>▄</span><span class='None-428'>▄</span><span class='None-429'>▄</span><span class='None-430'>▄</span><span class='None-431'>▄</span><span class='None-432'>▄</span><span class='None-433'>▄</span><span class='None-434'>▄</span><span class='None-435'>▄</span><span class='None-436'>▄</span><span class='None-437'>▄</span><span class='None-438'>▄</span><span class='None-439'>▄</span><span class='None-440'>▄</span><span class='None-441'>▄</span><span class='None-442'>▄</span><span class='None-443'>▄</span><span class='None-444'>▄</span><span class='None-445'>▄</span><span class='None-446'>▄</span>
-<span class='None-447'>Hello</span><span class='None-448'>There</span>
+<span class='0'>▄</span><span class='1'>▄</span><span class='2'>▄</span><span class='3'>▄</span><span class='4'>▄</span><span class='5'>▄</span><span class='6'>▄</span><span class='7'>▄</span><span class='8'>▄</span><span class='9'>▄</span><span class='10'>▄</span><span class='11'>▄</span><span class='12'>▄</span><span class='13'>▄</span><span class='14'>▄</span><span class='15'>▄</span><span class='16'>▄</span><span class='17'>▄</span><span class='18'>▄</span><span class='19'>▄</span><span class='20'>▄</span><span class='21'>▄</span><span class='22'>▄</span><span class='23'>▄</span><span class='24'>▄</span><span class='25'>▄</span><span class='26'>▄</span><span class='27'>▄</span><span class='28'>▄</span><span class='29'>▄</span>
+<span class='30'>▄</span><span class='31'>▄</span><span class='32'>▄</span><span class='33'>▄</span><span class='34'>▄</span><span class='35'>▄</span><span class='36'>▄</span><span class='37'>▄</span><span class='38'>▄</span><span class='39'>▄</span><span class='40'>▄</span><span class='41'>▄</span><span class='42'>▄</span><span class='43'>▄</span><span class='44'>▄</span><span class='45'>▄</span><span class='46'>▄</span><span class='47'>▄</span><span class='48'>▄</span><span class='49'>▄</span><span class='50'>▄</span><span class='51'>▄</span><span class='52'>▄</span><span class='53'>▄</span><span class='54'>▄</span><span class='55'>▄</span><span class='56'>▄</span><span class='57'>▄</span><span class='58'>▄</span><span class='59'>▄</span>
+<span class='60'>▄</span><span class='61'>▄</span><span class='62'>▄</span><span class='63'>▄</span><span class='64'>▄</span><span class='65'>▄</span><span class='66'>▄</span><span class='67'>▄</span><span class='68'>▄</span><span class='69'>▄</span><span class='70'>▄</span><span class='71'>▄</span><span class='72'>▄</span><span class='73'>▄</span><span class='74'>▄</span><span class='75'>▄</span><span class='76'>▄</span><span class='77'>▄</span><span class='78'>▄</span><span class='79'>▄</span><span class='80'>▄</span><span class='81'>▄</span><span class='82'>▄</span><span class='83'>▄</span><span class='84'>▄</span><span class='85'>▄</span><span class='86'>▄</span><span class='87'>▄</span><span class='88'>▄</span><span class='89'>▄</span>
+<span class='90'>▄</span><span class='91'>▄</span><span class='92'>▄</span><span class='93'>▄</span><span class='94'>▄</span><span class='95'>▄</span><span class='96'>▄</span><span class='97'>▄</span><span class='98'>▄</span><span class='99'>▄</span><span class='100'>▄</span><span class='101'>▄</span><span class='102'>▄</span><span class='103'>▄</span><span class='104'>▄</span><span class='105'>▄</span><span class='106'>▄</span><span class='107'>▄</span><span class='108'>▄</span><span class='109'>▄</span><span class='110'>▄</span><span class='111'>▄</span><span class='112'>▄</span><span class='113'>▄</span><span class='114'>▄</span><span class='115'>▄</span><span class='116'>▄</span><span class='117'>▄</span><span class='118'>▄</span><span class='119'>▄</span>
+<span class='120'>▄</span><span class='121'>▄</span><span class='122'>▄</span><span class='123'>▄</span><span class='124'>▄</span><span class='125'>▄</span><span class='126'>▄</span><span class='127'>▄</span><span class='128'>▄</span><span class='129'>▄</span><span class='130'>▄</span><span class='131'>▄</span><span class='132'>▄</span><span class='133'>▄</span><span class='134'>▄</span><span class='135'>▄</span><span class='136'>▄</span><span class='137'>▄</span><span class='138'>▄</span><span class='139'>▄</span><span class='140'>▄</span><span class='141'>▄</span><span class='142'>▄</span><span class='143'>▄</span><span class='144'>▄</span><span class='145'>▄</span><span class='146'>▄</span><span class='147'>▄</span><span class='148'>▄</span><span class='149'>▄</span>
+<span class='150'>▄</span><span class='151'>▄</span><span class='152'>▄</span><span class='153'>▄</span><span class='154'>▄</span><span class='155'>▄</span><span class='156'>▄</span><span class='157'>▄</span><span class='158'>▄</span><span class='159'>▄</span><span class='160'>▄</span><span class='161'>▄</span><span class='162'>▄</span><span class='163'>▄</span><span class='164'>▄</span><span class='165'>▄</span><span class='166'>▄</span><span class='167'>▄</span><span class='168'>▄</span><span class='169'>▄</span><span class='170'>▄</span><span class='171'>▄</span><span class='172'>▄</span><span class='173'>▄</span><span class='174'>▄</span><span class='175'>▄</span><span class='176'>▄</span><span class='177'>▄</span><span class='178'>▄</span><span class='179'>▄</span>
+<span class='180'>▄</span><span class='181'>▄</span><span class='182'>▄</span><span class='183'>▄</span><span class='184'>▄</span><span class='185'>▄</span><span class='186'>▄</span><span class='187'>▄</span><span class='188'>▄</span><span class='189'>▄</span><span class='190'>▄</span><span class='191'>▄</span><span class='192'>▄</span><span class='193'>▄</span><span class='194'>▄</span><span class='195'>▄</span><span class='196'>▄</span><span class='197'>▄</span><span class='198'>▄</span><span class='199'>▄</span><span class='200'>▄</span><span class='201'>▄</span><span class='202'>▄</span><span class='203'>▄</span><span class='204'>▄</span><span class='205'>▄</span><span class='206'>▄</span><span class='207'>▄</span><span class='208'>▄</span><span class='209'>▄</span>
+<span class='210'>▄</span><span class='211'>▄</span><span class='212'>▄</span><span class='213'>▄</span><span class='214'>▄</span><span class='215'>▄</span><span class='216'>▄</span><span class='217'>▄</span><span class='218'>▄</span><span class='219'>▄</span><span class='220'>▄</span><span class='221'>▄</span><span class='222'>▄</span><span class='223'>▄</span><span class='224'>▄</span><span class='225'>▄</span><span class='226'>▄</span><span class='227'>▄</span><span class='228'>▄</span><span class='229'>▄</span><span class='230'>▄</span><span class='231'>▄</span><span class='232'>▄</span><span class='233'>▄</span><span class='234'>▄</span><span class='235'>▄</span><span class='236'>▄</span><span class='237'>▄</span><span class='238'>▄</span><span class='239'>▄</span>
+<span class='240'>▄</span><span class='241'>▄</span><span class='242'>▄</span><span class='243'>▄</span><span class='244'>▄</span><span class='245'>▄</span><span class='246'>▄</span><span class='247'>▄</span><span class='248'>▄</span><span class='249'>▄</span><span class='250'>▄</span><span class='251'>▄</span><span class='252'>▄</span><span class='253'>▄</span><span class='254'>▄</span><span class='255'>▄</span><span class='256'>▄</span><span class='257'>▄</span><span class='258'>▄</span><span class='259'>▄</span><span class='260'>▄</span><span class='261'>▄</span><span class='262'>▄</span><span class='263'>▄</span><span class='264'>▄</span><span class='265'>▄</span><span class='266'>▄</span><span class='267'>▄</span><span class='268'>▄</span><span class='269'>▄</span>
+<span class='270'>▄</span><span class='271'>▄</span><span class='272'>▄</span><span class='273'>▄</span><span class='37'>▄</span><span class='274'>▄</span><span class='275'>▄</span><span class='276'>▄</span><span class='277'>▄</span><span class='278'>▄</span><span class='279'>▄</span><span class='280'>▄</span><span class='281'>▄</span><span class='282'>▄</span><span class='283'>▄</span><span class='284'>▄</span><span class='285'>▄</span><span class='286'>▄</span><span class='287'>▄</span><span class='288'>▄</span><span class='289'>▄</span><span class='290'>▄</span><span class='291'>▄</span><span class='292'>▄</span><span class='293'>▄</span><span class='294'>▄</span><span class='295'>▄</span><span class='296'>▄</span><span class='297'>▄</span><span class='298'>▄</span>
+<span class='299'>▄</span><span class='300'>▄</span><span class='301'>▄</span><span class='302'>▄</span><span class='303'>▄</span><span class='304'>▄</span><span class='305'>▄</span><span class='306'>▄</span><span class='307'>▄</span><span class='308'>▄</span><span class='309'>▄</span><span class='310'>▄</span><span class='311'>▄</span><span class='312'>▄</span><span class='313'>▄</span><span class='314'>▄</span><span class='315'>▄</span><span class='316'>▄</span><span class='248'>▄</span><span class='317'>▄</span><span class='318'>▄</span><span class='319'>▄</span><span class='320'>▄</span><span class='321'>▄</span><span class='322'>▄</span><span class='323'>▄</span><span class='324'>▄</span><span class='325'>▄</span><span class='326'>▄</span><span class='327'>▄</span>
+<span class='328'>▄</span><span class='329'>▄</span><span class='330'>▄</span><span class='331'>▄</span><span class='332'>▄</span><span class='333'>▄</span><span class='334'>▄</span><span class='335'>▄</span><span class='336'>▄</span><span class='337'>▄</span><span class='338'>▄</span><span class='339'>▄</span><span class='340'>▄</span><span class='341'>▄</span><span class='342'>▄</span><span class='337'>▄</span><span class='343'>▄</span><span class='344'>▄</span><span class='345'>▄</span><span class='346'>▄</span><span class='347'>▄</span><span class='348'>▄</span><span class='349'>▄</span><span class='350'>▄</span><span class='351'>▄</span><span class='352'>▄</span><span class='353'>▄</span><span class='354'>▄</span><span class='355'>▄</span><span class='356'>▄</span>
+<span class='357'>▄</span><span class='358'>▄</span><span class='359'>▄</span><span class='360'>▄</span><span class='361'>▄</span><span class='362'>▄</span><span class='363'>▄</span><span class='364'>▄</span><span class='365'>▄</span><span class='366'>▄</span><span class='367'>▄</span><span class='368'>▄</span><span class='369'>▄</span><span class='370'>▄</span><span class='371'>▄</span><span class='372'>▄</span><span class='373'>▄</span><span class='374'>▄</span><span class='375'>▄</span><span class='376'>▄</span><span class='377'>▄</span><span class='378'>▄</span><span class='379'>▄</span><span class='380'>▄</span><span class='381'>▄</span><span class='382'>▄</span><span class='383'>▄</span><span class='384'>▄</span><span class='385'>▄</span><span class='386'>▄</span>
+<span class='387'>▄</span><span class='388'>▄</span><span class='389'>▄</span><span class='390'>▄</span><span class='391'>▄</span><span class='392'>▄</span><span class='393'>▄</span><span class='394'>▄</span><span class='395'>▄</span><span class='396'>▄</span><span class='397'>▄</span><span class='398'>▄</span><span class='399'>▄</span><span class='400'>▄</span><span class='401'>▄</span><span class='402'>▄</span><span class='403'>▄</span><span class='404'>▄</span><span class='405'>▄</span><span class='406'>▄</span><span class='407'>▄</span><span class='408'>▄</span><span class='409'>▄</span><span class='410'>▄</span><span class='411'>▄</span><span class='412'>▄</span><span class='413'>▄</span><span class='414'>▄</span><span class='415'>▄</span><span class='416'>▄</span>
+<span class='417'>▄</span><span class='418'>▄</span><span class='419'>▄</span><span class='420'>▄</span><span class='421'>▄</span><span class='422'>▄</span><span class='423'>▄</span><span class='424'>▄</span><span class='425'>▄</span><span class='426'>▄</span><span class='427'>▄</span><span class='428'>▄</span><span class='429'>▄</span><span class='430'>▄</span><span class='431'>▄</span><span class='432'>▄</span><span class='433'>▄</span><span class='434'>▄</span><span class='435'>▄</span><span class='436'>▄</span><span class='437'>▄</span><span class='438'>▄</span><span class='439'>▄</span><span class='440'>▄</span><span class='441'>▄</span><span class='442'>▄</span><span class='443'>▄</span><span class='444'>▄</span><span class='445'>▄</span><span class='446'>▄</span>
+<span class='447'>Hello</span><span class='448'>There</span>
             </code>
         </pre>
     </body>
 </html>"""
```

### Comparing `pytermgui-7.3.0/tests/colorgrids.py` & `pytermgui-7.4.0/tests/colorgrids.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test.json` & `pytermgui-7.4.0/tests/test.json`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test.yaml` & `pytermgui-7.4.0/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_animations.py` & `pytermgui-7.4.0/tests/test_animations.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_auto.py` & `pytermgui-7.4.0/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_colors.py` & `pytermgui-7.4.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_dump_n_load.py` & `pytermgui-7.4.0/tests/test_dump_n_load.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_exporters.py` & `pytermgui-7.4.0/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_fancy_repr.py` & `pytermgui-7.4.0/tests/test_fancy_repr.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_helpers.py` & `pytermgui-7.4.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_layouts.py` & `pytermgui-7.4.0/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_parser.py` & `pytermgui-7.4.0/tests/test_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 
 import random
 import string
 from itertools import zip_longest
 
 import pytest
 
-from pytermgui import StyledText, pretty, tim, tokenize_ansi, tokens_to_markup
+from pytermgui import (
+    StyledText,
+    pretty,
+    tim,
+    tokenize_ansi,
+    tokens_to_markup,
+    tokenize_markup,
+)
 from pytermgui.colors import Color, str_to_color
 from pytermgui.markup import StyledText, Token
 from pytermgui.markup import tokens as tkns
+from pytermgui.markup.parsing import parse_tokens
 from pytermgui.markup.style_maps import CLEARERS, STYLES
 
 
 def random_plain() -> tkns.PlainToken:
     value = "".join(random.choices(string.ascii_letters, k=5))
     value = (
         value.replace("\n", " ")
@@ -94,14 +102,28 @@
 
     def test_get_markup(self):
         base = "[141 @61 bold]Hello[/]"
         ansi = tim.parse("[141 @61 bold]Hello")
         markup = tim.get_markup(ansi)
         assert base == markup
 
+    def test_mutiline_markup(self):
+        base = "[141 @61 bold]Hello[/]\nWhat a beautifull day to look a this [~https://example.com]website[/~] !\nOh and this [~https://example.com]website also[/~]\nHave a nice day !"
+        opti_base = "[141 @61 bold]Hello[/]\nWhat a beautifull day to look a this [~https://example.com]website[/~] !\nOh and this [~https://example.com]website also[/~]\nHave a nice day ![/]"
+
+        tokens = tokenize_markup(base)
+        ansi = parse_tokens(list(tokens))
+        tokens2 = tokenize_ansi(ansi)
+        markup = tokens_to_markup(list(tokens2))
+        assert opti_base == markup
+
+        ansi = tim.parse(base)
+        markup = tim.get_markup(ansi)
+        assert opti_base == markup
+
     def test_parse(self):
         assert (
             tim.parse("[141 @61 bold !upper]Hello")
             == "\x1b[38;5;141m\x1b[48;5;61m\x1b[1mHELLO\x1b[0m"
         ), repr(tim.parse("[141 @61 bold !upper]Hello"))
```

### Comparing `pytermgui-7.3.0/tests/test_regex.py` & `pytermgui-7.4.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/tests/test_styles.py` & `pytermgui-7.4.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/.gitignore` & `pytermgui-7.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/LICENSE` & `pytermgui-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytermgui-7.3.0/pyproject.toml` & `pytermgui-7.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 [tool.hatch.version]
 path = "pytermgui/__init__.py"
 
 [tool.hatch.build]
 include = [
     "/pytermgui",
     "/tests",
+    "README.md",
+    "CHANGELOG.md",
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
```

### Comparing `pytermgui-7.3.0/PKG-INFO` & `pytermgui-7.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTermGUI
-Version: 7.3.0
+Version: 7.4.0
 Summary: Python TUI framework with mouse support, modular widget system, customizable and rapid terminal markup language and more!
 Project-URL: homepage, https://github.com/bczsalba/PyTermGUI
 Project-URL: repository, https://github.com/bczsalba/PyTermGUI
 Project-URL: documentation, https://ptg.bczsalba.com
 Author-email: Balázs Cene <bczsalba@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -123,37 +123,14 @@
 - Start generating semantic colors (success, warning, error) by blending with the primary
 
 ### Removals
 
 - Remove `is_bindable` widget attribute
 
 
-## [7.2.0] - 2022-08-05
-
-### Additions
-
-- Add various color manipulation utilities
-- Add `#auto` TIM pseudo-tag that always gives properly contrasted foreground text
-- Add `palettes` module for framework-wide color generation & configuration
-- Add `Synchronized Output` support
-- Add `FancyReprWidget`
-- Add `ptg --palette` flag
-
-### Bugfixes
-
-- Fix markup aliases getting literalized during `parsing.eval_alias` & `MarkupLanguage.alias`
-- Fix background colors creating vertical seams in SVG exports
-- Fix colors getting localized pre-maturely
-
-### Refactors
-
-- Make all the `ptg` program & all builting widgets use the global palette
-- Prefix all ANSI colors with `ansi-`
-
-
 Read the full changelog [here](https://github.com/bczsalba/pytermgui/blob/master/CHANGELOG.md).
 
 
 
 [7.3.0]: https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0
 [7.2.0]: https://github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0
 [7.1.0]: https://github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyTermGUI Version: 7.3.0 Summary: Python TUI
+Metadata-Version: 2.1 Name: PyTermGUI Version: 7.4.0 Summary: Python TUI
 framework with mouse support, modular widget system, customizable and rapid
 terminal markup language and more! Project-URL: homepage, https://github.com/
 bczsalba/PyTermGUI Project-URL: repository, https://github.com/bczsalba/
 PyTermGUI Project-URL: documentation, https://ptg.bczsalba.com Author-email:
 BalÃ¡zs Cene
 gmail.com> License: MIT License-File: LICENSE Keywords:
 ANSI,TUI,UI,framework,markup,terminal,user-interface,xterm Classifier:
@@ -45,38 +45,29 @@
 number indicators to `Palette.print` - Add `inline` widget runner ### Bugfixes
 - Fix incorrect macro caching behaviour - Fix various issues and misbehaviours
 with SVG exports - Fix incorrect placement of `InputField` cursor ### Refactors
 - New `MkDocs` based documentation - Change `terminal.py` -> `term.py` and
 `serializer.py` -> `serialization.py` to avoid naming conflicts - Improve
 pseudo token behaviour by parsing it as a new token type - Start generating
 semantic colors (success, warning, error) by blending with the primary ###
-Removals - Remove `is_bindable` widget attribute ## [7.2.0] - 2022-08-05 ###
-Additions - Add various color manipulation utilities - Add `#auto` TIM pseudo-
-tag that always gives properly contrasted foreground text - Add `palettes`
-module for framework-wide color generation & configuration - Add `Synchronized
-Output` support - Add `FancyReprWidget` - Add `ptg --palette` flag ### Bugfixes
-- Fix markup aliases getting literalized during `parsing.eval_alias` &
-`MarkupLanguage.alias` - Fix background colors creating vertical seams in SVG
-exports - Fix colors getting localized pre-maturely ### Refactors - Make all
-the `ptg` program & all builting widgets use the global palette - Prefix all
-ANSI colors with `ansi-` Read the full changelog [here](https://github.com/
-bczsalba/pytermgui/blob/master/CHANGELOG.md). [7.3.0]: https://github.com/
-bczsalba/pytermgui/compare/v7.2.0...v7.3.0 [7.2.0]: https://github.com/
-bczsalba/pytermgui/compare/v7.1.0...v7.2.0 [7.1.0]: https://github.com/
-bczsalba/pytermgui/compare/v7.0.0...v7.1.0 [7.0.0]: https://github.com/
-bczsalba/pytermgui/compare/v6.4.0...v7.0.0 [6.4.0]: https://github.com/
-bczsalba/pytermgui/compare/v6.0.0...v6.4.0 [6.3.0]: https://github.com/
-bczsalba/pytermgui/compare/v6.2.2...v6.3.0 [6.2.2]: https://github.com/
-bczsalba/pytermgui/compare/v6.2.1...v6.2.2 [6.2.1]: https://github.com/
-bczsalba/pytermgui/compare/v6.2.0...v6.2.1 [6.2.0]: https://github.com/
-bczsalba/pytermgui/compare/v6.1.0...v6.2.0 [6.1.0]: https://github.com/
-bczsalba/pytermgui/compare/v6.0.0...v6.1.0 [6.0.0]: https://github.com/
-bczsalba/pytermgui/compare/v5.0.0...v6.0.0 [5.0.0]: https://github.com/
-bczsalba/pytermgui/compare/v4.3.2...v5.0.0 [4.3.2]: https://github.com/
-bczsalba/pytermgui/compare/v4.3.1...v4.3.2 [4.3.1]: https://github.com/
-bczsalba/pytermgui/compare/v4.3.0...v4.3.1 [4.3.0]: https://github.com/
-bczsalba/pytermgui/compare/v4.2.0...v4.3.0 [4.2.1]: https://github.com/
-bczsalba/pytermgui/compare/v4.2.0...v4.2.1 [4.2.0]: https://github.com/
-bczsalba/pytermgui/compare/v4.1.0...v4.2.0 [4.1.0]: https://github.com/
-bczsalba/pytermgui/compare/v4.0.0...v4.1.0 [4.0.1]: https://github.com/
-bczsalba/pytermgui/compare/v4.0.0...v4.0.1 [4.0.0]: https://github.com/
-bczsalba/pytermgui/compare/v3.2.1...v4.0.0
+Removals - Remove `is_bindable` widget attribute Read the full changelog [here]
+(https://github.com/bczsalba/pytermgui/blob/master/CHANGELOG.md). [7.3.0]:
+https://github.com/bczsalba/pytermgui/compare/v7.2.0...v7.3.0 [7.2.0]: https://
+github.com/bczsalba/pytermgui/compare/v7.1.0...v7.2.0 [7.1.0]: https://
+github.com/bczsalba/pytermgui/compare/v7.0.0...v7.1.0 [7.0.0]: https://
+github.com/bczsalba/pytermgui/compare/v6.4.0...v7.0.0 [6.4.0]: https://
+github.com/bczsalba/pytermgui/compare/v6.0.0...v6.4.0 [6.3.0]: https://
+github.com/bczsalba/pytermgui/compare/v6.2.2...v6.3.0 [6.2.2]: https://
+github.com/bczsalba/pytermgui/compare/v6.2.1...v6.2.2 [6.2.1]: https://
+github.com/bczsalba/pytermgui/compare/v6.2.0...v6.2.1 [6.2.0]: https://
+github.com/bczsalba/pytermgui/compare/v6.1.0...v6.2.0 [6.1.0]: https://
+github.com/bczsalba/pytermgui/compare/v6.0.0...v6.1.0 [6.0.0]: https://
+github.com/bczsalba/pytermgui/compare/v5.0.0...v6.0.0 [5.0.0]: https://
+github.com/bczsalba/pytermgui/compare/v4.3.2...v5.0.0 [4.3.2]: https://
+github.com/bczsalba/pytermgui/compare/v4.3.1...v4.3.2 [4.3.1]: https://
+github.com/bczsalba/pytermgui/compare/v4.3.0...v4.3.1 [4.3.0]: https://
+github.com/bczsalba/pytermgui/compare/v4.2.0...v4.3.0 [4.2.1]: https://
+github.com/bczsalba/pytermgui/compare/v4.2.0...v4.2.1 [4.2.0]: https://
+github.com/bczsalba/pytermgui/compare/v4.1.0...v4.2.0 [4.1.0]: https://
+github.com/bczsalba/pytermgui/compare/v4.0.0...v4.1.0 [4.0.1]: https://
+github.com/bczsalba/pytermgui/compare/v4.0.0...v4.0.1 [4.0.0]: https://
+github.com/bczsalba/pytermgui/compare/v3.2.1...v4.0.0
```

