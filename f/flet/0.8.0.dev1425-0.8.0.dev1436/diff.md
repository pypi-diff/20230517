# Comparing `tmp/flet-0.8.0.dev1425.tar.gz` & `tmp/flet-0.8.0.dev1436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-0.8.0.dev1425.tar", max compression
+gzip compressed data, was "flet-0.8.0.dev1436.tar", max compression
```

## Comparing `flet-0.8.0.dev1425.tar` & `flet-0.8.0.dev1436.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2145 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/README.md
--rw-r--r--   0        0        0     1066 2023-05-16 19:48:37.420513 flet-0.8.0.dev1425/pyproject.toml
--rw-r--r--   0        0        0      155 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__init__.py
--rw-r--r--   0        0        0       72 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/__init__.py
--rw-r--r--   0        0        0       20 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/config.py
--rw-r--r--   0        0        0      378 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/hook-flet.py
--rw-r--r--   0        0        0     2985 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/macos_utils.py
--rw-r--r--   0        0        0      187 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
--rw-r--r--   0        0        0       61 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/rthooks.dat
--rw-r--r--   0        0        0      562 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/utils.py
--rw-r--r--   0        0        0     3620 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/__pyinstaller/win_utils.py
--rw-r--r--   0        0        0     6194 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/async_local_socket_connection.py
--rw-r--r--   0        0        0     7202 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/async_websocket_connection.py
--rw-r--r--   0        0        0     9083 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/authorization.py
--rw-r--r--   0        0        0      128 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/group.py
--rw-r--r--   0        0        0     1499 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/oauth_token.py
--rw-r--r--   0        0        0      735 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      840 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3653 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      799 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      182 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/auth/user.py
--rw-r--r--   0        0        0       31 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/canvas/__init__.py
--rw-r--r--   0        0        0     2958 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/cli/cli.py
--rw-r--r--   0        0        0     1953 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/cli/commands/base.py
--rw-r--r--   0        0        0      673 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/cli/commands/options.py
--rw-r--r--   0        0        0     8468 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/cli/commands/pack.py
--rw-r--r--   0        0        0     9306 2023-05-16 19:47:54.156211 flet-0.8.0.dev1425/src/flet/cli/commands/publish.py
--rw-r--r--   0        0        0     7297 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/cli/commands/run.py
--rw-r--r--   0        0        0       52 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/constants.py
--rw-r--r--   0        0        0    22023 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/plotly_chart.py
--rw-r--r--   0        0        0    10239 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/pubsub.py
--rw-r--r--   0        0        0     3049 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/reconnecting_websocket.py
--rw-r--r--   0        0        0     1272 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/security.py
--rw-r--r--   0        0        0     6819 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/sync_local_socket_connection.py
--rw-r--r--   0        0        0     5396 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/sync_websocket_connection.py
--rw-r--r--   0        0        0     6955 2023-05-16 19:47:54.160211 flet-0.8.0.dev1425/src/flet/utils.py
--rw-r--r--   0        0        0     1431 2023-05-16 19:48:37.164500 flet-0.8.0.dev1425/src/flet/version.py
--rw-r--r--   0        0        0       32 2023-05-16 19:38:40.000000 flet-0.8.0.dev1425/src/flet/web/.last_build_id
--rw-r--r--   0        0        0      229 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/AssetManifest.bin
--rw-r--r--   0        0        0      455 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/AssetManifest.json
--rw-r--r--   0        0        0       82 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/FontManifest.json
--rw-r--r--   0        0        0  1736909 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/NOTICES
--rw-r--r--   0        0        0  1261080 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
--rw-r--r--   0        0        0      298 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
--rw-r--r--   0        0        0      271 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
--rw-r--r--   0        0        0      166 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
--rw-r--r--   0        0        0      366 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
--rw-r--r--   0        0        0     9242 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/assets/shaders/ink_sparkle.frag
--rw-r--r--   0        0        0     1028 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/favicon.png
--rw-r--r--   0        0        0    14240 2023-05-16 19:37:18.000000 flet-0.8.0.dev1425/src/flet/web/flutter.js
--rw-r--r--   0        0        0     8316 2023-05-16 19:38:40.000000 flet-0.8.0.dev1425/src/flet/web/flutter_service_worker.js
--rw-r--r--   0        0        0     4699 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/apple-touch-icon-192.png
--rw-r--r--   0        0        0     6622 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/icon-192.png
--rw-r--r--   0        0        0    18666 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/icon-512.png
--rw-r--r--   0        0        0     4128 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/icon-maskable-192.png
--rw-r--r--   0        0        0    11906 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/icon-maskable-512.png
--rw-r--r--   0        0        0    17040 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/icons/loading-animation.png
--rw-r--r--   0        0        0     3086 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/index.html
--rw-r--r--   0        0        0  5440153 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/main.dart.js
--rw-r--r--   0        0        0      789 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/manifest.json
--rw-r--r--   0        0        0     1573 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/python-worker.js
--rw-r--r--   0        0        0      744 2023-05-16 19:38:39.000000 flet-0.8.0.dev1425/src/flet/web/python.js
--rw-r--r--   0        0        0       92 2023-05-16 19:38:36.000000 flet-0.8.0.dev1425/src/flet/web/version.json
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.8.0.dev1425/PKG-INFO
+-rw-r--r--   0        0        0     2145 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/README.md
+-rw-r--r--   0        0        0     1066 2023-05-17 19:50:46.367714 flet-0.8.0.dev1436/pyproject.toml
+-rw-r--r--   0        0        0      198 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__init__.py
+-rw-r--r--   0        0        0       72 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0       20 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/config.py
+-rw-r--r--   0        0        0      378 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/hook-flet.py
+-rw-r--r--   0        0        0     2985 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/macos_utils.py
+-rw-r--r--   0        0        0      187 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/rthooks/pyi_rth_localhost_fletd.py
+-rw-r--r--   0        0        0       61 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/rthooks.dat
+-rw-r--r--   0        0        0      562 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/utils.py
+-rw-r--r--   0        0        0     3620 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/__pyinstaller/win_utils.py
+-rw-r--r--   0        0        0     6194 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/async_local_socket_connection.py
+-rw-r--r--   0        0        0     7202 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/async_websocket_connection.py
+-rw-r--r--   0        0        0     9083 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/authorization.py
+-rw-r--r--   0        0        0      128 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/group.py
+-rw-r--r--   0        0        0     1499 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/oauth_token.py
+-rw-r--r--   0        0        0      735 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      840 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3653 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      799 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      182 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/auth/user.py
+-rw-r--r--   0        0        0       31 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/canvas/__init__.py
+-rw-r--r--   0        0        0     2958 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/cli/cli.py
+-rw-r--r--   0        0        0     1953 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/cli/commands/base.py
+-rw-r--r--   0        0        0      673 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/cli/commands/options.py
+-rw-r--r--   0        0        0     8468 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/cli/commands/pack.py
+-rw-r--r--   0        0        0     9284 2023-05-17 19:50:08.661105 flet-0.8.0.dev1436/src/flet/cli/commands/publish.py
+-rw-r--r--   0        0        0     7297 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/cli/commands/run.py
+-rw-r--r--   0        0        0       52 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/constants.py
+-rw-r--r--   0        0        0    22157 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0    10239 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/pubsub.py
+-rw-r--r--   0        0        0     3049 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/reconnecting_websocket.py
+-rw-r--r--   0        0        0     1272 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/security.py
+-rw-r--r--   0        0        0     6819 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/sync_local_socket_connection.py
+-rw-r--r--   0        0        0     5396 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/sync_websocket_connection.py
+-rw-r--r--   0        0        0     6955 2023-05-17 19:50:08.665105 flet-0.8.0.dev1436/src/flet/utils.py
+-rw-r--r--   0        0        0     1431 2023-05-17 19:50:45.455722 flet-0.8.0.dev1436/src/flet/version.py
+-rw-r--r--   0        0        0       32 2023-05-17 19:42:02.000000 flet-0.8.0.dev1436/src/flet/web/.last_build_id
+-rw-r--r--   0        0        0      455 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/AssetManifest.json
+-rw-r--r--   0        0        0      229 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/AssetManifest.smcbin
+-rw-r--r--   0        0        0       82 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/FontManifest.json
+-rw-r--r--   0        0        0  1736909 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/NOTICES
+-rw-r--r--   0        0        0  1261080 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/assets/fonts/MaterialIcons-Regular.otf
+-rw-r--r--   0        0        0      298 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/packages/window_manager/images/ic_chrome_close.png
+-rw-r--r--   0        0        0      271 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/packages/window_manager/images/ic_chrome_maximize.png
+-rw-r--r--   0        0        0      166 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/packages/window_manager/images/ic_chrome_minimize.png
+-rw-r--r--   0        0        0      366 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/packages/window_manager/images/ic_chrome_unmaximize.png
+-rw-r--r--   0        0        0     9242 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/assets/shaders/ink_sparkle.frag
+-rw-r--r--   0        0        0     1028 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/favicon.png
+-rw-r--r--   0        0        0    14240 2023-05-17 19:40:48.000000 flet-0.8.0.dev1436/src/flet/web/flutter.js
+-rw-r--r--   0        0        0     8319 2023-05-17 19:42:02.000000 flet-0.8.0.dev1436/src/flet/web/flutter_service_worker.js
+-rw-r--r--   0        0        0     4699 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/apple-touch-icon-192.png
+-rw-r--r--   0        0        0     6622 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/icon-192.png
+-rw-r--r--   0        0        0    18666 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/icon-512.png
+-rw-r--r--   0        0        0     4128 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/icon-maskable-192.png
+-rw-r--r--   0        0        0    11906 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/icon-maskable-512.png
+-rw-r--r--   0        0        0    17040 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/icons/loading-animation.png
+-rw-r--r--   0        0        0     3158 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/index.html
+-rw-r--r--   0        0        0  5440180 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/main.dart.js
+-rw-r--r--   0        0        0      789 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/manifest.json
+-rw-r--r--   0        0        0     1573 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/python-worker.js
+-rw-r--r--   0        0        0      744 2023-05-17 19:42:01.000000 flet-0.8.0.dev1436/src/flet/web/python.js
+-rw-r--r--   0        0        0       92 2023-05-17 19:41:58.000000 flet-0.8.0.dev1436/src/flet/web/version.json
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 flet-0.8.0.dev1436/PKG-INFO
```

### Comparing `flet-0.8.0.dev1425/README.md` & `flet-0.8.0.dev1436/README.md`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/pyproject.toml` & `flet-0.8.0.dev1436/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet"
-version = "0.8.0.dev1425"
+version = "0.8.0.dev1436"
 description = "Flet for Python - easily build interactive multi-platform apps in Python"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.8.0.dev1425"
+flet-core = "0.8.0.dev1436"
 python = "^3.7"
 typing-extensions = { version = "^4.4.0", python = "<3.8" }
 websocket-client = "^1.4.2"
 watchdog = "^2.2.1"
 oauthlib = "^3.2.2"
 websockets = "^10.4"
 httpx = "^0.23.3"
```

### Comparing `flet-0.8.0.dev1425/src/flet/__pyinstaller/macos_utils.py` & `flet-0.8.0.dev1436/src/flet/__pyinstaller/macos_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/__pyinstaller/utils.py` & `flet-0.8.0.dev1436/src/flet/__pyinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/__pyinstaller/win_utils.py` & `flet-0.8.0.dev1436/src/flet/__pyinstaller/win_utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/async_local_socket_connection.py` & `flet-0.8.0.dev1436/src/flet/async_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/async_websocket_connection.py` & `flet-0.8.0.dev1436/src/flet/async_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/authorization.py` & `flet-0.8.0.dev1436/src/flet/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/oauth_provider.py` & `flet-0.8.0.dev1436/src/flet/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/oauth_token.py` & `flet-0.8.0.dev1436/src/flet/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/providers/auth0_oauth_provider.py` & `flet-0.8.0.dev1436/src/flet/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/providers/azure_oauth_provider.py` & `flet-0.8.0.dev1436/src/flet/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/providers/github_oauth_provider.py` & `flet-0.8.0.dev1436/src/flet/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/auth/providers/google_oauth_provider.py` & `flet-0.8.0.dev1436/src/flet/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/cli/cli.py` & `flet-0.8.0.dev1436/src/flet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/cli/commands/base.py` & `flet-0.8.0.dev1436/src/flet/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/cli/commands/options.py` & `flet-0.8.0.dev1436/src/flet/cli/commands/options.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/cli/commands/pack.py` & `flet-0.8.0.dev1436/src/flet/cli/commands/pack.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/cli/commands/publish.py` & `flet-0.8.0.dev1436/src/flet/cli/commands/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,20 +214,20 @@
             var pythonModuleName = "{module_name}";
         </script>
         <script src="python.js"></script>
         """
         index = index.replace("%FLET_WEB_PYODIDE%", "true")
         index = index.replace("<!-- pyodideCode -->", pyodideCode)
         index = index.replace(
-            "<!-- flutterWebRenderer -->",
-            f'<script>var flutterWebRenderer="{options.web_renderer}";</script>',
+            "<!-- webRenderer -->",
+            f'<script>webRenderer="{options.web_renderer}";</script>',
         )
         index = index.replace(
             "<!-- useColorEmoji -->",
-            f"<script>var useColorEmoji={str(options.use_color_emoji).lower()};</script>",
+            f"<script>useColorEmoji={str(options.use_color_emoji).lower()};</script>",
         )
         index = index.replace("%FLET_ROUTE_URL_STRATEGY%", options.route_url_strategy)
 
         if options.base_url:
             base_url = options.base_url.strip("/").strip()
             index = index.replace(
                 '<base href="/">',
```

### Comparing `flet-0.8.0.dev1425/src/flet/cli/commands/run.py` & `flet-0.8.0.dev1436/src/flet/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/flet.py` & `flet-0.8.0.dev1436/src/flet/flet.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,18 @@
     from typing_extensions import Literal
 
 
 logger = logging.getLogger(flet.__name__)
 
 WEB_BROWSER = "web_browser"
 FLET_APP = "flet_app"
+FLET_APP_WEB = "flet_app_web"
 FLET_APP_HIDDEN = "flet_app_hidden"
 
-AppViewer = Literal[None, "web_browser", "flet_app", "flet_app_hidden"]
+AppViewer = Literal[None, "web_browser", "flet_app", "flet_app_web", "flet_app_hidden"]
 
 WebRenderer = Literal[None, "auto", "html", "canvaskit"]
 
 
 def app(
     target,
     name="",
@@ -146,15 +147,15 @@
 
     logger.info("Connected to Flet app and handling user sessions...")
 
     fvp = None
     pid_file = None
 
     if (
-        (view == FLET_APP or view == FLET_APP_HIDDEN)
+        (view == FLET_APP or view == FLET_APP_HIDDEN or view == FLET_APP_WEB)
         and not is_linux_server()
         and url_prefix is None
     ):
         fvp, pid_file = open_flet_view(
             conn.page_url, assets_dir, view == FLET_APP_HIDDEN
         )
         try:
@@ -222,15 +223,15 @@
 
     logger.info("Connected to Flet app and handling user sessions...")
 
     fvp = None
     pid_file = None
 
     if (
-        (view == FLET_APP or view == FLET_APP_HIDDEN)
+        (view == FLET_APP or view == FLET_APP_HIDDEN or view == FLET_APP_WEB)
         and not is_linux_server()
         and url_prefix is None
     ):
         fvp, pid_file = await open_flet_view_async(
             conn.page_url, assets_dir, view == FLET_APP_HIDDEN
         )
         try:
@@ -278,16 +279,16 @@
 ):
     env_port = os.getenv("FLET_SERVER_PORT")
     if env_port is not None and env_port:
         port = int(env_port)
 
     uds_path = os.getenv("FLET_SERVER_UDS_PATH")
 
-    is_desktop = view == FLET_APP or view == FLET_APP_HIDDEN
-    if server is None and not is_desktop:
+    is_socket_server = server is None and (view == FLET_APP or view == FLET_APP_HIDDEN)
+    if not is_socket_server:
         server = __start_flet_server(
             host,
             port,
             assets_dir,
             upload_dir,
             web_renderer,
             use_color_emoji,
@@ -316,15 +317,15 @@
         except Exception as e:
             print(
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
             page.error(f"There was an error while processing your request: {e}")
 
-    if is_desktop:
+    if is_socket_server:
         conn = SyncLocalSocketConnection(
             port,
             uds_path,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     else:
@@ -356,16 +357,16 @@
 ):
     env_port = os.getenv("FLET_SERVER_PORT")
     if env_port is not None and env_port:
         port = int(env_port)
 
     uds_path = os.getenv("FLET_SERVER_UDS_PATH")
 
-    is_desktop = view == FLET_APP or view == FLET_APP_HIDDEN
-    if server is None and not is_desktop:
+    is_socket_server = server is None and (view == FLET_APP or view == FLET_APP_HIDDEN)
+    if not is_socket_server:
         server = __start_flet_server(
             host,
             port,
             assets_dir,
             upload_dir,
             web_renderer,
             use_color_emoji,
@@ -396,15 +397,15 @@
                 f"Unhandled error processing page session {page.session_id}:",
                 traceback.format_exc(),
             )
             await page.error_async(
                 f"There was an error while processing your request: {e}"
             )
 
-    if is_desktop:
+    if is_socket_server:
         conn = AsyncLocalSocketConnection(
             port,
             uds_path,
             on_event=on_event,
             on_session_created=on_session_created,
         )
     else:
```

### Comparing `flet-0.8.0.dev1425/src/flet/pubsub.py` & `flet-0.8.0.dev1436/src/flet/pubsub.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/reconnecting_websocket.py` & `flet-0.8.0.dev1436/src/flet/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/security.py` & `flet-0.8.0.dev1436/src/flet/security.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/sync_local_socket_connection.py` & `flet-0.8.0.dev1436/src/flet/sync_local_socket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/sync_websocket_connection.py` & `flet-0.8.0.dev1436/src/flet/sync_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/utils.py` & `flet-0.8.0.dev1436/src/flet/utils.py`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/version.py` & `flet-0.8.0.dev1436/src/flet/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess as sp
 from pathlib import Path
 
 import flet
 from flet.utils import is_windows, which
 
 # this value will be replaced by CI
-version = "0.8.0.dev1425"
+version = "0.8.0.dev1436"
 
 
 def update_version():
     """Return the current version or default."""
     working = Path().absolute()
     os.chdir(Path(flet.__file__).absolute().parent)
     in_repo = which("git.exe" if is_windows() else "git") and sp.run(
```

### Comparing `flet-0.8.0.dev1425/src/flet/web/assets/NOTICES` & `flet-0.8.0.dev1436/src/flet/web/assets/NOTICES`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/assets/fonts/MaterialIcons-Regular.otf` & `flet-0.8.0.dev1436/src/flet/web/assets/fonts/MaterialIcons-Regular.otf`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/assets/shaders/ink_sparkle.frag` & `flet-0.8.0.dev1436/src/flet/web/assets/shaders/ink_sparkle.frag`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/favicon.png` & `flet-0.8.0.dev1436/src/flet/web/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/flutter.js` & `flet-0.8.0.dev1436/src/flet/web/flutter.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/flutter_service_worker.js` & `flet-0.8.0.dev1436/src/flet/web/flutter_service_worker.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 'use strict';
 const MANIFEST = 'flutter-app-manifest';
 const TEMP = 'flutter-temp-cache';
 const CACHE_NAME = 'flutter-app-cache';
 
 const RESOURCES = {
     "assets/AssetManifest.json": "d9150da08bcab79647bb00a0700488d6",
+    "assets/AssetManifest.smcbin": "28ce9529363d3157175808e8bb3faba2",
     "assets/NOTICES": "7335396837d2bb6f3605b87107c4e292",
     "assets/packages/window_manager/images/ic_chrome_minimize.png": "4282cd84cb36edf2efb950ad9269ca62",
     "assets/packages/window_manager/images/ic_chrome_maximize.png": "af7499d7657c8b69d23b85156b60298c",
     "assets/packages/window_manager/images/ic_chrome_close.png": "75f4b8ab3608a05461a31fc18d6b47c2",
     "assets/packages/window_manager/images/ic_chrome_unmaximize.png": "4a90c1909cb74e8f0d35794e2f61d8bf",
     "assets/FontManifest.json": "7b2a36307916a9721811788013e65289",
     "assets/shaders/ink_sparkle.frag": "f8b80e740d33eb157090be4e995febdf",
-    "assets/AssetManifest.bin": "28ce9529363d3157175808e8bb3faba2",
     "assets/fonts/MaterialIcons-Regular.otf": "7ecc5db379e238f74e08718029577db8",
     "favicon.png": "302ac04c14db027d016d1fe74c6a80a0",
     "manifest.json": "7909dae66a9203092dc86b5a6162e79c",
     "flutter.js": "6fef97aeca90b426343ba6c5c9dc5d4a",
-    "main.dart.js": "6adfab0711b55d80f317e9da99ce5baf",
+    "main.dart.js": "50c2ec96e8a4e0e191e6d09b4bdf43b5",
     "version.json": "3fea9d9c7b4ca6955aa03e762e0d2e13",
     "icons/apple-touch-icon-192.png": "8cf0d5162941f467a77f023c414a1812",
     "icons/icon-maskable-512.png": "aa798e6d780ff109da17c3a98d5f2619",
     "icons/loading-animation.png": "41a96047dbd2463a50c46ad3bf6ff158",
     "icons/icon-192.png": "81c4311263d0cad60c1f0496b4fa7c8f",
     "icons/icon-maskable-192.png": "c1c2210feeb444cf800a5ce0d06eff16",
     "icons/icon-512.png": "06b219f171b5a1af6dd8299ea1e116f2",
@@ -30,16 +30,16 @@
     "canvaskit/skwasm.js": "1df4d741f441fa1a4d10530ced463ef8",
     "canvaskit/canvaskit.js": "76f7d822f42397160c5dfc69cbc9b2de",
     "canvaskit/skwasm.worker.js": "19659053a277272607529ef87acf9d8a",
     "canvaskit/skwasm.wasm": "6711032e17bf49924b2b001cef0d3ea3",
     "canvaskit/chromium/canvaskit.wasm": "fc18c3010856029414b70cae1afc5cd9",
     "canvaskit/chromium/canvaskit.js": "8c8392ce4a4364cbb240aa09b5652e05",
     "python-worker.js": "b961f261b9ad85e06369e83fd2e33bb7",
-    "index.html": "e0a6304cccf95b3630931783101c5e0d",
-    "/": "e0a6304cccf95b3630931783101c5e0d"
+    "index.html": "324bf64e37549f2fe31f28b8515bd366",
+    "/": "324bf64e37549f2fe31f28b8515bd366"
 };
 // The application shell files that are downloaded before a service worker can
 // start.
 const CORE = ["main.dart.js",
     "index.html",
     "assets/AssetManifest.json",
     "assets/FontManifest.json"
```

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/apple-touch-icon-192.png` & `flet-0.8.0.dev1436/src/flet/web/icons/apple-touch-icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/icon-192.png` & `flet-0.8.0.dev1436/src/flet/web/icons/icon-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/icon-512.png` & `flet-0.8.0.dev1436/src/flet/web/icons/icon-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/icon-maskable-192.png` & `flet-0.8.0.dev1436/src/flet/web/icons/icon-maskable-192.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/icon-maskable-512.png` & `flet-0.8.0.dev1436/src/flet/web/icons/icon-maskable-512.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/icons/loading-animation.png` & `flet-0.8.0.dev1436/src/flet/web/icons/loading-animation.png`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/index.html` & `flet-0.8.0.dev1436/src/flet/web/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -20,22 +20,27 @@
   <!-- Flet specific -->
   <meta name="flet-route-url-strategy" content="%FLET_ROUTE_URL_STRATEGY%">
   <meta name="flet-web-pyodide" content="%FLET_WEB_PYODIDE%">
 
   <title>Flet</title>
   <link rel="manifest" href="manifest.json">
 
-  <!-- flutterWebRenderer -->
+  <script>
+    var webRenderer = "auto";
+    var useColorEmoji = false;
+  </script>
+
+  <!-- webRenderer -->
   <!-- useColorEmoji -->
 
   <!-- pyodideCode -->
 
   <script>
     // The value below is injected by flutter build, do not touch.
-    var serviceWorkerVersion = "11431812";
+    var serviceWorkerVersion = "680719543";
   </script>
   <!-- This script adds the flutter initialization JS code -->
   <script src="flutter.js" defer></script>
 </head>
 
 <body>
   <div id="loading">
@@ -101,15 +106,15 @@
       _flutter.loader.loadEntrypoint({
         serviceWorker: {
           serviceWorkerVersion: serviceWorkerVersion,
         }
       }).then(function (engineInitializer) {
         loading.classList.add('main_done');
         return engineInitializer.initializeEngine({
-          renderer: flutterWebRenderer,
+          renderer: webRenderer,
           useColorEmoji: useColorEmoji,
         });
       }).then(function (appRunner) {
         loading.classList.add('init_done');
         return appRunner.runApp();
       }).then(function (app) {
         // Wait a few milliseconds so users can see the "zoooom" animation
```

### Comparing `flet-0.8.0.dev1425/src/flet/web/main.dart.js` & `flet-0.8.0.dev1436/src/flet/web/main.dart.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -19829,15 +19829,15 @@
                 _.e = e
             },
             ajy: function ajy(a, b) {
                 this.a = a
                 this.b = b
             },
             bj(a, b, c, d) {
-                return A.dm(new A.aXI(a, c, d), new A.aXJ(b), !0, new A.aXK(b), new A.dY(b, t.kK), t.V, t.Aq)
+                return A.dm(new A.aXI(a, c, d, b), new A.aXJ(b), !0, new A.aXK(b), new A.dY(b, t.kK), t.V, t.Aq)
             },
             byt(a, b, c, d, e) {
                 var s = null,
                     r = b.a,
                     q = r.c
                 switch (q) {
                     case "page":
@@ -20104,18 +20104,20 @@
             },
             aXJ: function aXJ(a) {
                 this.a = a
             },
             aXK: function aXK(a) {
                 this.a = a
             },
-            aXI: function aXI(a, b, c) {
-                this.a = a
-                this.b = b
-                this.c = c
+            aXI: function aXI(a, b, c, d) {
+                var _ = this
+                _.a = a
+                _.b = b
+                _.c = c
+                _.d = d
             },
             aXF: function aXF(a) {
                 this.a = a
             },
             aXL: function aXL(a, b, c) {
                 this.a = a
                 this.b = b
@@ -60079,15 +60081,15 @@
             var s = $.eU
             s = (s == null ? $.eU = A.lI(self.window.flutterConfiguration) : s).b
             if (s == null) s = null
             else {
                 s = s.canvasKitBaseUrl
                 if (s == null) s = null
             }
-            return (s == null ? "https://www.gstatic.com/flutter-canvaskit/d44b5a94c976fbb65815374f61ab5392a220b084/" : s) + a
+            return (s == null ? "https://www.gstatic.com/flutter-canvaskit/b4fb11214dd2dda6ce012dd98ea498e9e8b91262/" : s) + a
         },
         $S: 27
     }
     A.aWd.prototype = {
         $1(a) {
             this.a.remove()
             this.b.cX(0, !0)
@@ -103929,33 +103931,34 @@
         $1(a) {
             return J.ag(a.Q, this.a) == null
         },
         $S: 142
     }
     A.aXI.prototype = {
         $2(a, b) {
-            var s, r, q, p, o, n, m = null
+            var s, r, q, p, o, n, m = this,
+                l = null
             if (b == null) return B.ad
             s = b.a
             r = s.R("key", "")
             r.toString
             if (r !== "") {
-                q = new A.bA(m, t.A)
+                q = new A.bA(l, t.A)
                 p = a.L(t.l)
                 p.toString
                 p.z.q(0, r, q)
-            } else q = m
-            o = A.byt(q, b, this.a, this.b, this.c)
-            if (s.bf("theme") == null) return o
+            } else q = l
+            o = A.byt(q, b, m.a, m.b, m.c)
+            if (m.d === "page" || s.bf("theme") == null) return o
             n = A.i1(B.Bj, new A.aXF(b))
-            s = new A.aXL(b, n == null ? A.q(a) : m, o)
-            if (n === B.k3) return A.dm(new A.aXG(s), new A.aXH(), !0, m, m, t.V, t.Wy)
+            s = new A.aXL(b, n == null ? A.q(a) : l, o)
+            if (n === B.k3) return A.dm(new A.aXG(s), new A.aXH(), !0, l, l, t.V, t.Wy)
             else {
                 if (n === B.OL) r = B.aj
-                else r = n === B.rX ? B.a_ : m
+                else r = n === B.rX ? B.a_ : l
                 return s.$1(r)
             }
         },
         $S: 698
     }
     A.aXF.prototype = {
         $1(a) {
@@ -147092,15 +147095,15 @@
         },
         po(a) {
             var s, r = {},
                 q = a.a
             if (q == null) q = $.afP()
             r.a = r.b = null
             s = t.P
-            A.boI(q.aCW("AssetManifest.bin", A.bxD(), t.jo).bn(new A.agt(r, this, a, q), s), new A.agu(r), s, t.K)
+            A.boI(q.aCW("AssetManifest.smcbin", A.bxD(), t.jo).bn(new A.agt(r, this, a, q), s), new A.agu(r), s, t.K)
             s = r.a
             if (s != null) return s
             s = new A.ar($.ax, t.Lv)
             r.b = new A.bc(s, t.h8)
             return s
         },
         agb(a, b, c) {
```

### Comparing `flet-0.8.0.dev1425/src/flet/web/manifest.json` & `flet-0.8.0.dev1436/src/flet/web/manifest.json`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/python-worker.js` & `flet-0.8.0.dev1436/src/flet/web/python-worker.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/src/flet/web/python.js` & `flet-0.8.0.dev1436/src/flet/web/python.js`

 * *Files identical despite different names*

### Comparing `flet-0.8.0.dev1425/PKG-INFO` & `flet-0.8.0.dev1436/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet
-Version: 0.8.0.dev1425
+Version: 0.8.0.dev1436
 Summary: Flet for Python - easily build interactive multi-platform apps in Python
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.8.0.dev1425)
+Requires-Dist: flet-core (==0.8.0.dev1436)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: watchdog (>=2.2.1,<3.0.0)
 Requires-Dist: websocket-client (>=1.4.2,<2.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
```

