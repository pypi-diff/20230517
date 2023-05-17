# Comparing `tmp/decore_base-0.0.10.tar.gz` & `tmp/decore-base-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decore_base-0.0.10.tar", last modified: Wed May 17 11:12:05 2023, max compression
+gzip compressed data, was "decore-base-0.0.11.tar", last modified: Wed May 17 11:33:09 2023, max compression
```

## Comparing `decore_base-0.0.10.tar` & `decore-base-0.0.11.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.326315 decore_base-0.0.10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.302315 decore_base-0.0.10/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.306316 decore_base-0.0.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-17 11:11:57.000000 decore_base-0.0.10/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:11:57.000000 decore_base-0.0.10/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.306316 decore_base-0.0.10/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 11:11:57.000000 decore_base-0.0.10/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 11:11:57.000000 decore_base-0.0.10/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-17 11:11:57.000000 decore_base-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-17 11:12:05.326315 decore_base-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-17 11:11:57.000000 decore_base-0.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-17 11:11:57.000000 decore_base-0.0.10/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:12:05.326315 decore_base-0.0.10/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.306316 decore_base-0.0.10/src/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_element.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/classes/decore_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/decore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/decore_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-17 11:12:05.000000 decore_base-0.0.10/src/decore_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-17 11:12:05.000000 decore_base-0.0.10/src/decore_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:12:05.000000 decore_base-0.0.10/src/decore_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-17 11:12:05.000000 decore_base-0.0.10/src/decore_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/docs/social_header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/documentation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/conform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/extensions/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/depricated/askform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/depricated/buyform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/depricated/conform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/depricated/deform_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/perform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/reform_client_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/extensions/reform_server_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.310315 decore_base-0.0.10/src/library/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/library/particl_market/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/particl_market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/particl_market/particl_market.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/powershell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/return_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/library/roaster/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/roaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/roaster/roaster_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/roaster/roaster_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/library/roaster/roaster_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/prepare/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/prepare/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/.vscode/launch.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.306316 decore_base-0.0.10/src/prepare/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/prepare/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.314315 decore_base-0.0.10/src/prepare/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/prepare/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/prepare/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/prepare/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/js/912.143d216d.js
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/js/app.329a4a89.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/prepare/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/prepare/spa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/readme_de_en.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.318316 decore_base-0.0.10/src/sample/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.322316 decore_base-0.0.10/src/sample/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/account_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/company_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/global_management_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/information_stytem_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/bases/person_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/language.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.322316 decore_base-0.0.10/src/sample/models/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/models/account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/models/company_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/models/person_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.306316 decore_base-0.0.10/src/sample/spa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.322316 decore_base-0.0.10/src/sample/spa/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.322316 decore_base-0.0.10/src/sample/spa/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/css/912.77e6bcbe.css
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/css/app.d398f07d.css
--rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/css/vendor.14c9ac7a.css
--rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.322316 decore_base-0.0.10/src/sample/spa/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
--rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.326315 decore_base-0.0.10/src/sample/spa/static/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/icons/favicon-96x96.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.326315 decore_base-0.0.10/src/sample/spa/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/js/65.940d9b80.js
--rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/js/912.143d216d.js
--rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/js/app.329a4a89.js
--rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/static/js/vendor.03c46c80.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.326315 decore_base-0.0.10/src/sample/spa/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/spa/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:12:05.326315 decore_base-0.0.10/src/sample/state/
--rw-r--r--   0 runner    (1001) docker     (123)  1290240 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/state/database.db
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/state/keybase.kdbx
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-17 11:11:57.000000 decore_base-0.0.10/src/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.392192 decore-base-0.0.11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.372192 decore-base-0.0.11/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.372192 decore-base-0.0.11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-17 11:32:59.000000 decore-base-0.0.11/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:32:59.000000 decore-base-0.0.11/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.372192 decore-base-0.0.11/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 11:32:59.000000 decore-base-0.0.11/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 11:32:59.000000 decore-base-0.0.11/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-17 11:32:59.000000 decore-base-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-17 11:33:09.392192 decore-base-0.0.11/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/classes/decore_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/decore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/docs/social_header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/documentation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/conform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/extensions/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/depricated/askform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/depricated/buyform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/depricated/conform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/depricated/deform_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/perform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/reform_client_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/extensions/reform_server_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base/library/particl_market/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/particl_market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/particl_market/particl_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90489 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/powershell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/library/roaster/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/roaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/roaster/roaster_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/roaster/roaster_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/library/roaster/roaster_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/prepare/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/prepare/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/.vscode/launch.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.372192 decore-base-0.0.11/decore_base/prepare/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/prepare/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/prepare/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.380192 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/prepare/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/prepare/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/js/912.143d216d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/js/app.329a4a89.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/prepare/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/prepare/spa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/readme_de_en.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/account_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/company_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/global_management_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/information_stytem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/bases/person_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/language.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/models/account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/models/company_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/models/person_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.372192 decore-base-0.0.11/decore_base/sample/spa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/spa/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.384192 decore-base-0.0.11/decore_base/sample/spa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/css/912.77e6bcbe.css
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/css/app.d398f07d.css
+-rw-r--r--   0 runner    (1001) docker     (123)   466611 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/css/vendor.14c9ac7a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    64483 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.388192 decore-base-0.0.11/decore_base/sample/spa/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   164912 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   128360 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   465188 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   325244 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.388192 decore-base-0.0.11/decore_base/sample/spa/static/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-96x96.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.388192 decore-base-0.0.11/decore_base/sample/spa/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/js/65.940d9b80.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29594 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/js/912.143d216d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17942 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/js/app.329a4a89.js
+-rw-r--r--   0 runner    (1001) docker     (123)   380277 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/static/js/vendor.03c46c80.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.388192 decore-base-0.0.11/decore_base/sample/spa/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/spa/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.392192 decore-base-0.0.11/decore_base/sample/state/
+-rw-r--r--   0 runner    (1001) docker     (123)  1290240 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/state/database.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/state/keybase.kdbx
+-rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-05-17 11:32:59.000000 decore-base-0.0.11/decore_base/sample/state/querybase.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 11:33:09.376192 decore-base-0.0.11/decore_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-17 11:33:09.000000 decore-base-0.0.11/decore_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-17 11:33:09.000000 decore-base-0.0.11/decore_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 11:33:09.000000 decore-base-0.0.11/decore_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-17 11:33:09.000000 decore-base-0.0.11/decore_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-17 11:32:59.000000 decore-base-0.0.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-17 11:32:59.000000 decore-base-0.0.11/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 11:33:09.392192 decore-base-0.0.11/setup.cfg
```

### Comparing `decore_base-0.0.10/.gitignore` & `decore-base-0.0.11/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/LICENSE` & `decore-base-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/pyproject.toml` & `decore-base-0.0.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=7.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version"]
-name = "decore_base"
+name = "decore-base"
 description = 'decore Base is a "Python to Vue.js" open source package that helps you go from idea to view in a few simple steps. It is targeted to those who want to focus on the results of their algorithms, do scientific work, perform promotional teaching or learning functions.'
 authors = [
     { name = "Kemo Panzah"}
 ]
 readme = "README.md"
 
 [tool.setuptools_scm]
```

### Comparing `decore_base-0.0.10/readme.md` & `decore-base-0.0.11/readme.md`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/__init__.py` & `decore-base-0.0.11/decore_base/__init__.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_base.py` & `decore-base-0.0.11/decore_base/classes/decore_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_list.py` & `decore-base-0.0.11/decore_base/classes/decore_list.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_model.py` & `decore-base-0.0.11/decore_base/classes/decore_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_pool.py` & `decore-base-0.0.11/decore_base/classes/decore_pool.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_prompt.py` & `decore-base-0.0.11/decore_base/classes/decore_prompt.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_query.py` & `decore-base-0.0.11/decore_base/classes/decore_query.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_return.py` & `decore-base-0.0.11/decore_base/classes/decore_return.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_translate.py` & `decore-base-0.0.11/decore_base/classes/decore_translate.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/classes/decore_view.py` & `decore-base-0.0.11/decore_base/classes/decore_view.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/decore.py` & `decore-base-0.0.11/decore_base/decore.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/docs/social_header.txt` & `decore-base-0.0.11/decore_base/docs/social_header.txt`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/documentation.md` & `decore-base-0.0.11/decore_base/documentation.md`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/conform_model.py` & `decore-base-0.0.11/decore_base/extensions/conform_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/depricated/askform_base.py` & `decore-base-0.0.11/decore_base/extensions/depricated/askform_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/depricated/buyform_base.py` & `decore-base-0.0.11/decore_base/extensions/depricated/buyform_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/depricated/conform_base.py` & `decore-base-0.0.11/decore_base/extensions/depricated/conform_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/depricated/deform_base.py` & `decore-base-0.0.11/decore_base/extensions/depricated/deform_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/perform_model.py` & `decore-base-0.0.11/decore_base/extensions/perform_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/reform_client_model.py` & `decore-base-0.0.11/decore_base/extensions/reform_client_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/extensions/reform_server_model.py` & `decore-base-0.0.11/decore_base/extensions/reform_server_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/globals.py` & `decore-base-0.0.11/decore_base/globals.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/particl_market/particl_market.py` & `decore-base-0.0.11/decore_base/library/particl_market/particl_market.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/powershell.py` & `decore-base-0.0.11/decore_base/library/powershell.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/powershell2.py` & `decore-base-0.0.11/decore_base/library/powershell2.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/return_value.py` & `decore-base-0.0.11/decore_base/library/return_value.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/roaster/roaster_client.py` & `decore-base-0.0.11/decore_base/library/roaster/roaster_client.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/roaster/roaster_functions.py` & `decore-base-0.0.11/decore_base/library/roaster/roaster_functions.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/library/roaster/roaster_server.py` & `decore-base-0.0.11/decore_base/library/roaster/roaster_server.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/.gitignore` & `decore-base-0.0.11/decore_base/prepare/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/css/912.77e6bcbe.css` & `decore-base-0.0.11/decore_base/prepare/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/css/app.d398f07d.css` & `decore-base-0.0.11/decore_base/prepare/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/css/vendor.14c9ac7a.css` & `decore-base-0.0.11/decore_base/prepare/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/favicon.ico` & `decore-base-0.0.11/decore_base/prepare/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore-base-0.0.11/decore_base/prepare/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/icons/favicon-128x128.png` & `decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/icons/favicon-16x16.png` & `decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/icons/favicon-32x32.png` & `decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/icons/favicon-96x96.png` & `decore-base-0.0.11/decore_base/prepare/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/js/65.940d9b80.js` & `decore-base-0.0.11/decore_base/prepare/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/js/912.143d216d.js` & `decore-base-0.0.11/decore_base/prepare/spa/static/js/912.143d216d.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/js/app.329a4a89.js` & `decore-base-0.0.11/decore_base/prepare/spa/static/js/app.329a4a89.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/static/js/vendor.03c46c80.js` & `decore-base-0.0.11/decore_base/prepare/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/prepare/spa/templates/index.html` & `decore-base-0.0.11/decore_base/prepare/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/readme_de_en.md` & `decore-base-0.0.11/decore_base/readme_de_en.md`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/.gitignore` & `decore-base-0.0.11/decore_base/sample/.gitignore`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/bases/account_base.py` & `decore-base-0.0.11/decore_base/sample/bases/account_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/bases/company_base.py` & `decore-base-0.0.11/decore_base/sample/bases/company_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/bases/global_management_base.py` & `decore-base-0.0.11/decore_base/sample/bases/global_management_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/bases/person_base.py` & `decore-base-0.0.11/decore_base/sample/bases/person_base.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/models/person_model.py` & `decore-base-0.0.11/decore_base/sample/models/person_model.py`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/css/912.77e6bcbe.css` & `decore-base-0.0.11/decore_base/sample/spa/static/css/912.77e6bcbe.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/css/app.d398f07d.css` & `decore-base-0.0.11/decore_base/sample/spa/static/css/app.d398f07d.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/css/vendor.14c9ac7a.css` & `decore-base-0.0.11/decore_base/sample/spa/static/css/vendor.14c9ac7a.css`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/favicon.ico` & `decore-base-0.0.11/decore_base/sample/spa/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.d8e8e0f7.woff`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2` & `decore-base-0.0.11/decore_base/sample/spa/static/fonts/materialdesignicons-webfont.e9db4005.woff2`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/icons/favicon-128x128.png` & `decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/icons/favicon-16x16.png` & `decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/icons/favicon-32x32.png` & `decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/icons/favicon-96x96.png` & `decore-base-0.0.11/decore_base/sample/spa/static/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/js/65.940d9b80.js` & `decore-base-0.0.11/decore_base/sample/spa/static/js/65.940d9b80.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/js/912.143d216d.js` & `decore-base-0.0.11/decore_base/sample/spa/static/js/912.143d216d.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/js/app.329a4a89.js` & `decore-base-0.0.11/decore_base/sample/spa/static/js/app.329a4a89.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/static/js/vendor.03c46c80.js` & `decore-base-0.0.11/decore_base/sample/spa/static/js/vendor.03c46c80.js`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/spa/templates/index.html` & `decore-base-0.0.11/decore_base/sample/spa/templates/index.html`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/state/database.db` & `decore-base-0.0.11/decore_base/sample/state/database.db`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/state/keybase.kdbx` & `decore-base-0.0.11/decore_base/sample/state/keybase.kdbx`

 * *Files identical despite different names*

### Comparing `decore_base-0.0.10/src/sample/state/querybase.db` & `decore-base-0.0.11/decore_base/sample/state/querybase.db`

 * *Files identical despite different names*

