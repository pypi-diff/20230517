# Comparing `tmp/uidom-0.2a2.tar.gz` & `tmp/uidom-0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.2a2.tar", max compression
+gzip compressed data, was "uidom-0.2a3.tar", max compression
```

## Comparing `uidom-0.2a2.tar` & `uidom-0.2a3.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.2a2/LICENSE
--rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.2a2/README.md
--rw-r--r--   0        0        0     1271 2023-05-10 16:33:49.218202 uidom-0.2a2/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-10 16:33:41.398101 uidom-0.2a2/uidom/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.2a2/uidom/cli/__init__.py
--rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.2a2/uidom/cli/_cli.py
--rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.2a2/uidom/cli/cli.py
--rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.2a2/uidom/dom/__init__.py
--rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.2a2/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     5924 2023-05-09 16:54:51.261005 uidom-0.2a2/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.2a2/uidom/dom/icons.py
--rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.2a2/uidom/dom/jinja.py
--rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.2a2/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0    14512 2023-05-10 11:50:34.948921 uidom-0.2a2/uidom/dom/src/component.py
--rw-r--r--   0        0        0     2188 2023-04-30 13:08:13.941319 uidom-0.2a2/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.2a2/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    16849 2023-05-09 16:40:11.620271 uidom-0.2a2/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    31872 2023-05-08 10:55:40.270991 uidom-0.2a2/uidom/dom/src/ext.py
--rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.2a2/uidom/dom/src/html_string.py
--rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.2a2/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5048 2023-04-28 12:53:57.974327 uidom-0.2a2/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.2a2/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.2a2/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.2a2/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.2a2/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.2a2/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.2a2/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.2a2/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.2a2/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.2a2/uidom/dom/src/ws_rpc.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.2a2/uidom/dom/src/xmltags.py
--rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.2a2/uidom/dom/ui.py
--rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.2a2/uidom/dom/uniqueid.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.2a2/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.2a2/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.2a2/uidom/elements/__init__.py
--rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.2a2/uidom/elements/booleans.py
--rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.2a2/uidom/elements/buttons.py
--rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.2a2/uidom/elements/chars.py
--rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.2a2/uidom/elements/dates.py
--rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.2a2/uidom/elements/enums.py
--rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.2a2/uidom/elements/floats.py
--rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.2a2/uidom/elements/integers.py
--rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.2a2/uidom/examples/links.py
--rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.2a2/uidom/examples/toggle.py
--rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.2a2/uidom/reloader/__init__.py
--rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.2a2/uidom/reloader/_app.py
--rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.2a2/uidom/reloader/_models.py
--rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.2a2/uidom/reloader/_notify.py
--rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.2a2/uidom/reloader/_types.py
--rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.2a2/uidom/reloader/_watch.py
--rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.2a2/uidom/reloader/script/reloader.js
--rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.2a2/uidom/response/__init__.py
--rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.2a2/uidom/response/starlette.py
--rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.2a2/uidom/routing/__init__.py
--rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.2a2/uidom/routing/fastapi.py
--rw-r--r--   0        0        0      768 2023-04-12 16:05:27.697495 uidom-0.2a2/uidom/scripts/__init__.py
--rw-r--r--   0        0        0     4560 2023-04-22 05:04:01.008470 uidom-0.2a2/uidom/scripts/cdn.py
--rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.2a2/uidom/scripts/xcomponent.js
--rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.2a2/uidom/settings/__init__.py
--rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.2a2/uidom/settings/commands.py
--rw-r--r--   0        0        0     8691 2023-05-05 06:53:34.240389 uidom-0.2a2/uidom/settings/document.py
--rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.2a2/uidom/settings/paths.py
--rw-r--r--   0        0        0      219 2023-03-16 11:20:30.258980 uidom-0.2a2/uidom/slots/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.2a2/uidom/slots/custom_element_slot.py
--rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.2a2/uidom/slots/web_component_slot.py
--rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.2a2/uidom/utils/__init__.py
--rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.2a2/uidom/utils/functional.py
--rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.2a2/uidom/utils/logger.py
--rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.2a2/uidom/utils/parameters.py
--rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.2a2/uidom/web_io/__init__.py
--rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.2a2/uidom/web_io/_adapter.py
--rw-r--r--   0        0        0     7291 2023-05-03 18:18:45.850893 uidom-0.2a2/uidom/web_io/_events.py
--rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.2a2/uidom/web_io/_protocol.py
--rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.2a2/uidom/web_io/_types.py
--rw-r--r--   0        0        0     6849 1970-01-01 00:00:00.000000 uidom-0.2a2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.2a3/LICENSE
+-rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.2a3/README.md
+-rw-r--r--   0        0        0     1274 2023-05-17 11:15:17.401237 uidom-0.2a3/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-17 10:27:01.597117 uidom-0.2a3/uidom/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.2a3/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.2a3/uidom/cli/_cli.py
+-rw-r--r--   0        0        0     6774 2023-05-10 16:28:25.006037 uidom-0.2a3/uidom/cli/cli.py
+-rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.2a3/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.2a3/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     5936 2023-05-17 19:09:09.830246 uidom-0.2a3/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.2a3/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.2a3/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.2a3/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    14512 2023-05-10 11:50:34.948921 uidom-0.2a3/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     3594 2023-05-17 05:54:56.304356 uidom-0.2a3/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.2a3/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    16797 2023-05-16 15:42:38.161310 uidom-0.2a3/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31315 2023-05-17 18:54:56.506273 uidom-0.2a3/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.2a3/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.2a3/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5072 2023-05-17 19:09:09.607096 uidom-0.2a3/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.2a3/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.2a3/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.2a3/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.2a3/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.2a3/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.2a3/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.2a3/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.2a3/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.2a3/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.2a3/uidom/dom/src/xmltags.py
+-rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.2a3/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.2a3/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.2a3/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.2a3/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.2a3/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.2a3/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.2a3/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.2a3/uidom/elements/chars.py
+-rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.2a3/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.2a3/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.2a3/uidom/elements/floats.py
+-rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.2a3/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.2a3/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.2a3/uidom/examples/toggle.py
+-rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.2a3/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.2a3/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.2a3/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.2a3/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.2a3/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.2a3/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.2a3/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.2a3/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.2a3/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.2a3/uidom/routing/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.2a3/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      723 2023-05-17 09:43:23.116452 uidom-0.2a3/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.2a3/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.2a3/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.2a3/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8691 2023-05-05 06:53:34.240389 uidom-0.2a3/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.2a3/uidom/settings/paths.py
+-rw-r--r--   0        0        0      219 2023-03-16 11:20:30.258980 uidom-0.2a3/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.2a3/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.2a3/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.2a3/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.2a3/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.2a3/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.2a3/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.2a3/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.2a3/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7496 2023-05-17 18:36:02.616227 uidom-0.2a3/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.2a3/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.2a3/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 uidom-0.2a3/PKG-INFO
```

### Comparing `uidom-0.2a2/LICENSE` & `uidom-0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/README.md` & `uidom-0.2a3/README.md`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/pyproject.toml` & `uidom-0.2a3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 [tool.poetry]
 name = "uidom"
-version = "0.2a2"
+version = "0.2a3"
 description = "HTML library"
 authors = ["bitplorer <bitplorer@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.0.1"
-aiofiles = "^0.7.0"
-python-multipart = "^0.0.5"
 valio = "^0.1.0-beta.5"
-httpx = "^0.24.0"
 marko = "^1.3.0"
 anyio = "^3.6.2"
 typer = "^0.9.0"
 
 # Dependencies below are required for devtools only
 pytailwindcss = { version = ">=0.1.4", optional = true }
 watchgod = { version = ">=0.8.2", optional = true }
@@ -33,14 +30,17 @@
 black = "^21.6b0"
 mypy = "^0.942"
 uvicorn = {extras = ["standard"], version = "^0.18.2"}
 starlette = "0.19.1"
 fastapi = "^0.79.0"
 watchgod = "^0.8.2"
 pytailwindcss = "^0.1.4"
+deptry = "^0.11.0"
+pipdeptree = "^2.7.1"
+python-multipart = "^0.0.6"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 toml = "^0.10.2"
 types-toml = "^0.10.8"
 
 [tool.poetry.scripts]
```

### Comparing `uidom-0.2a2/uidom/cli/__init__.py` & `uidom-0.2a3/uidom/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/cli/_cli.py` & `uidom-0.2a3/uidom/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/cli/cli.py` & `uidom-0.2a3/uidom/cli/cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/__init__.py` & `uidom-0.2a3/uidom/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/htmldocument.py` & `uidom-0.2a3/uidom/dom/htmldocument.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/htmlelement.py` & `uidom-0.2a3/uidom/dom/htmlelement.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 from dataclasses import dataclass
 
 from uidom.dom.src import DoubleTags, component
-from uidom.dom.src.jinjatags import render
+from uidom.dom.src.jinjatags import render_jinja
 
 __all__ = [
     "HTMLElement",
     "AMPElement",
     "XComponent",
     "CustomElement",
     "WebComponent",
@@ -191,15 +191,15 @@
 class JinjaElement(component.Component):
     escape_string = False
 
     def render(self, elem_or_str_or_path):
         return elem_or_str_or_path
 
     def __call__(self, **options):
-        return render(self, **options)
+        return render_jinja(self, **options)
 
 
 class MarkdownElement(component.Component):
     escape_string = False
     string_is_markdown = True
 
     def render(self, md_str_or_path):
```

### Comparing `uidom-0.2a2/uidom/dom/icons.py` & `uidom-0.2a3/uidom/dom/icons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/jinja.py` & `uidom-0.2a3/uidom/dom/jinja.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/component.py` & `uidom-0.2a3/uidom/dom/src/component.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/dom1core.py` & `uidom-0.2a3/uidom/dom/src/dom1core.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/dom_tag.py` & `uidom-0.2a3/uidom/dom/src/dom_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,14 @@
         thread_id = _get_thread_context()
         stack = dom_tag._with_contexts[thread_id]
         frame = stack.pop()
 
         for item in frame.items:
             if item in frame.used:
                 continue
-            # if not hasattr(item, "_entry"):
             self.add(item)
         if not stack:
             del dom_tag._with_contexts[thread_id]
 
     def __call__(self, func):
         """
         tag instance is being used as a decorator.
@@ -510,12 +509,12 @@
     """
     Set attributes on the current active tag context
     """
     c = get_current()
     dicts = args + (kwargs,)
     for d in dicts:
         for attr, value in d.items():
-            c.set_attribute(*dom_tag.clean_pair(attr, value))
+            c.set_attribute(*c.clean_pair(attr, value))
 
 
 # escape() is used in render
 from uidom.dom.src.utils.dom_util import escape
```

### Comparing `uidom-0.2a2/uidom/dom/src/ext.py` & `uidom-0.2a3/uidom/dom/src/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -660,17 +660,16 @@
             self.add(*dom_elements)
 
 
 class StyleTags(Tags):
     left_delimiter = "{"
     right_delimiter = "}"
     self_dedent = False
-    is_class = False
-    is_id = False
-    is_apply = False
+    tagname_prefix = ""
+    attribute_joiner = "%s: %s;"
 
     def _render_open_tag(
         self,
         /,
         sb,
         name,
         open_tag,
@@ -689,31 +688,24 @@
         sb = self._render_attribute(
             sb=sb,
             indent_level=indent_level,
             indent_str=indent_str,
             pretty=pretty,
             xhtml=xhtml,
         )
-        # sb.append(''.join(["/", self.right_delimiter]) if self.is_single and xhtml else self.right_delimiter)
         return sb
 
     def _render_attribute(self, /, sb, indent_level, indent_str, pretty, xhtml):
-        if not self.is_apply:
-            attribute_joiner = (
-                "%s:%s;"
-                if not pretty
-                else f"{indent_str}%s: %s;\n" + (indent_str * indent_level)
-            )
-        else:
-            attribute_joiner = (
-                "@%s %s;"
-                if not pretty
-                else f"{indent_str}@%s %s;\n" + (indent_str * indent_level)
-            )
-        attribute_items = sorted(self.attributes.items())
+        attribute_joiner = (
+            f"{self.attribute_joiner}".replace(" ", "")
+            if not pretty
+            else f"{indent_str}{self.attribute_joiner}\n" + (indent_str * indent_level)
+        )
+
+        attribute_items = self.attributes.items()
 
         for attribute, value in attribute_items:
             if (
                 value is not False and value is not None
             ):  # False values must be omitted completely
                 sb.append(attribute_joiner % (attribute, escape(unicode(value), True)))
 
@@ -730,39 +722,32 @@
         # (del, object, input)
         if any(name):  # to handle the case when tagname = ""
             if name[-1] == "_":
                 name = name[:-1]
             if name[0] == "_":
                 name = name[1:]
 
-        if all([self.is_class, self.is_id]):
-            raise AttributeError(f"{name} can not have both is_class and is_id as True")
-
-        if self.is_class:
-            name = "".join([".", name])
-
-        if self.is_id:
-            name = "".join(["#", name])
+        name = "".join([self.tagname_prefix, name])
 
         return name
 
     @property
     def attr(self):
         r = []
-        attribute_joiner = "%s:%s;" if not self.is_apply else "@%s %s;"
+        attribute_joiner = self.attribute_joiner
 
-        for attribute, value in sorted(self.attributes.items()):
+        for attribute, value in self.attributes.items():
             if (
                 value is not False and value is not None
             ):  # False values must be omitted completely
                 r.append(attribute_joiner % (attribute, escape(unicode(value), True)))
 
             if value is None:  # minified xhtml attributes are added
                 r.append(" %s" % attribute)
-        return "".join(r)
+        return " ".join(r)
 
     @classmethod
     def clean_attribute(cls, attribute):
         """
         Normalize attribute names for shorthand and work around for limitations
         in Python's syntax.
         """
```

### Comparing `uidom-0.2a2/uidom/dom/src/html_string.py` & `uidom-0.2a3/uidom/dom/src/html_string.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/htmltags.py` & `uidom-0.2a3/uidom/dom/src/htmltags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/jinjatags.py` & `uidom-0.2a3/uidom/dom/src/jinjatags.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Cycle",
     "Comment",
     "Extends",
     "Load",
     "CSRFToken",
     "Block",
     "Var",
-    "render",
+    "render_jinja",
     "JinjaSingleTags",
     "JinjaDoubleTags",
     "JinjaBaseTag",
 ]
 
 
 class JinjaBaseTag(object):
@@ -37,25 +37,25 @@
 class JinjaDoubleTags(JinjaBaseTag, extension.DoubleTemplates):
     self_dedent = False
     child_dedent = False
     enable_left_delimiter_space = True
     enable_right_delimiter_space = True
 
     def __call__(self, **options):
-        return render(self, **options)
+        return render_jinja(self, **options)
 
 
 class JinjaSingleTags(JinjaBaseTag, extension.SingleTemplates):
     self_dedent = False
     child_dedent = True
     enable_left_delimiter_space = True
     enable_right_delimiter_space = True
 
     def __call__(self, **options):
-        return render(self, **options)
+        return render_jinja(self, **options)
 
 
 class Block(JinjaDoubleTags):
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
@@ -191,15 +191,15 @@
         :param template_text:
         :param dom_elements: [optional] template
         """
 
         super(Var, self).__init__("", template_text, *dom_elements)
 
 
-def render(template, **options):
+def render_jinja(template, **options):
     return raw(
         Template(
             template.__render__() if isinstance(template, dom_tag) else template,
             lstrip_blocks=True,
             trim_blocks=True,
             enable_async=True,
         ).render(**options)
```

### Comparing `uidom-0.2a2/uidom/dom/src/parse_html.py` & `uidom-0.2a3/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/pythontags.py` & `uidom-0.2a3/uidom/dom/src/pythontags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/sphinxtags.py` & `uidom-0.2a3/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/svgtags.py` & `uidom-0.2a3/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/utils/dom_util.py` & `uidom-0.2a3/uidom/dom/src/utils/dom_util.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/utils/sheets.py` & `uidom-0.2a3/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/src/ws_rpc.py` & `uidom-0.2a3/uidom/dom/src/ws_rpc.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/ui.py` & `uidom-0.2a3/uidom/dom/ui.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/dom/uniqueid.py` & `uidom-0.2a3/uidom/dom/uniqueid.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/edge_db/ql.py` & `uidom-0.2a3/uidom/edge_db/ql.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/booleans.py` & `uidom-0.2a3/uidom/elements/booleans.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/buttons.py` & `uidom-0.2a3/uidom/elements/buttons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/chars.py` & `uidom-0.2a3/uidom/elements/chars.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/dates.py` & `uidom-0.2a3/uidom/elements/dates.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/enums.py` & `uidom-0.2a3/uidom/elements/enums.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/floats.py` & `uidom-0.2a3/uidom/elements/floats.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/elements/integers.py` & `uidom-0.2a3/uidom/elements/integers.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/examples/links.py` & `uidom-0.2a3/uidom/examples/links.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/examples/toggle.py` & `uidom-0.2a3/uidom/examples/toggle.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/reloader/_app.py` & `uidom-0.2a3/uidom/reloader/_app.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/reloader/_notify.py` & `uidom-0.2a3/uidom/reloader/_notify.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/reloader/_watch.py` & `uidom-0.2a3/uidom/reloader/_watch.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/reloader/script/reloader.js` & `uidom-0.2a3/uidom/reloader/script/reloader.js`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/response/starlette.py` & `uidom-0.2a3/uidom/response/starlette.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/routing/fastapi.py` & `uidom-0.2a3/uidom/routing/fastapi.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/scripts/__init__.py` & `uidom-0.2a3/uidom/scripts/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # Copyright (c) 2023 UiDOM
 #
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
-from functools import lru_cache
 from pathlib import Path
 
 from uidom.dom import raw
 from uidom.dom.src.component import Component
 
 __all__ = ["x_component_js_text", "x_component_js"]
 
 
-# @lru_cache
 def x_component_js_text():
     X_COMPONENT_SCRIPT_FILE = Path(__file__).parent / "xcomponent.js"
     if not X_COMPONENT_SCRIPT_FILE.exists():
         raise FileNotFoundError(f"{X_COMPONENT_SCRIPT_FILE=} doesn't exists")
     return X_COMPONENT_SCRIPT_FILE.read_text()
```

### Comparing `uidom-0.2a2/uidom/scripts/xcomponent.js` & `uidom-0.2a3/uidom/scripts/xcomponent.js`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/settings/commands.py` & `uidom-0.2a3/uidom/settings/commands.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/settings/document.py` & `uidom-0.2a3/uidom/settings/document.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/settings/paths.py` & `uidom-0.2a3/uidom/settings/paths.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/slots/custom_element_slot.py` & `uidom-0.2a3/uidom/slots/custom_element_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/slots/web_component_slot.py` & `uidom-0.2a3/uidom/slots/web_component_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/utils/functional.py` & `uidom-0.2a3/uidom/utils/functional.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/utils/logger.py` & `uidom-0.2a3/uidom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/utils/parameters.py` & `uidom-0.2a3/uidom/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/web_io/_adapter.py` & `uidom-0.2a3/uidom/web_io/_adapter.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/uidom/web_io/_events.py` & `uidom-0.2a3/uidom/web_io/_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 
 class BaseEventManager(object):
     def __init__(self):
         # events registered in registered_events list will be allowed to be added
         self.__registered_events: list[str] = []
 
         # __original_method_registry keeps the track of the original methods that are decorated and are going to be
-        # added to the __events_when_activity and if the method has been already added to it then it won't
+        # added to the __events_with_activity and if the method has been already added to it then it won't
         # be added again as its the same method for the same event_name
         self.__original_method_registry: defaultdict = defaultdict(
             partial(defaultdict, list)
         )
-        self.__events_with_activity: defaultdict = defaultdict(
+        self.__events_with_activities: defaultdict = defaultdict(
             partial(defaultdict, list)
         )
 
-        # this _event_queue is used to signal that the
+        # this _event_queue can be used to signal for any purpose
         self._event_queue: Queue = Queue()
 
         # now adding the queue to the relay event so that anything that is pushed can be
 
     async def __aiter__(self):
-        for activity in self.__events_with_activity:
-            for event_name in self.__events_with_activity[activity]:
-                yield activity, event_name, self.__events_with_activity[activity][
+        for activity in self.__events_with_activities:
+            for event_name in self.__events_with_activities[activity]:
+                yield activity, event_name, self.__events_with_activities[activity][
                     event_name
                 ]
 
     def _on(self, activity: str, event_name: str):
         def callback_decorator(method: CALLABLE) -> CALLABLE:
             if event_name not in self.__registered_events:
                 raise ValueError(
@@ -56,56 +56,62 @@
 
                 @wraps(method)
                 async def event_callback(*args, **kwargs):
                     if iscoroutinefunction(method):
                         return await method(*args, **kwargs)
                     return method(*args, **kwargs)
 
-                self.__events_with_activity[activity][event_name].append(event_callback)
+                self.__events_with_activities[activity][event_name].append(
+                    event_callback
+                )
             else:
                 warn(
                     message=f"{activity} already added event {event_name} to method {method!r}"
                 )
             return method
 
         return callback_decorator
 
     def _event_callbacks(self, event_name: str):
         callbacks = []
-        for activity in self.__events_with_activity:
-            if event_name in self.__events_with_activity[activity]:
-                callbacks.extend(self.__events_with_activity[activity][event_name])
+        for activity in self.__events_with_activities:
+            if event_name in self.__events_with_activities[activity]:
+                callbacks.extend(self.__events_with_activities[activity][event_name])
 
         return callbacks
 
     def __getitem__(self, event_name: str):
         # returns an async iterator of the event handlers
         # which can be used as follows:
         # event_mgr = EventManager()
         # for callback in event_mgr[event_name]:
         #     yield callback
         return self._event_callbacks(event_name)
 
     def __contains__(self, event_name):
-        for activity in self.__events_with_activity:
-            if event_name in self.__events_with_activity[activity]:
+        for activity in self.__events_with_activities:
+            if event_name in self.__events_with_activities[activity]:
                 return True
         return False
 
     @property
     def registered_events(self):
         return self.__registered_events
 
     def register_event(self, event_name):
         if event_name in self.__registered_events:
             raise ValueError(
                 f"event {event_name} already added to the registered_events list"
             )
         self.__registered_events.append(event_name)
 
+    @property
+    def registered_activities(self) -> Dict[str, Dict[str, List[Callable]]]:
+        return self.__events_with_activities
+
     def _set_event_with_activity(
         self, activity: str, event_name_or_method: Union[str, CALLABLE]
     ) -> CALLABLE:
         method = None
         event_name = None
         if callable(event_name_or_method):
             event_name = event_name_or_method.__name__
@@ -119,15 +125,15 @@
             self.__registered_events.append(event_name)
 
         if method:
             return self._on(activity, event_name)(method)
         return self._on(activity, event_name)
 
     def _get_events_with_activity(self, activity: str) -> Dict[str, List[Callable]]:
-        return self.__events_with_activity[activity]
+        return self.registered_activities[activity]
 
     def set_event(
         self, activity: str, event_name_or_method: Union[str, CALLABLE]
     ) -> CALLABLE:
         return self._set_event_with_activity(activity, event_name_or_method)
 
     def get_events(self, activity: str) -> Dict[str, List[Callable]]:
```

### Comparing `uidom-0.2a2/uidom/web_io/_protocol.py` & `uidom-0.2a3/uidom/web_io/_protocol.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a2/PKG-INFO` & `uidom-0.2a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: uidom
-Version: 0.2a2
+Version: 0.2a3
 Summary: HTML library
 License: MIT
 Author: bitplorer
 Author-email: bitplorer@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
 Provides-Extra: fastapi
 Provides-Extra: fastapidev
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
-Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
 Requires-Dist: fastapi (>=0.79.0) ; extra == "fastapi" or extra == "fastapidev"
-Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: marko (>=1.3.0,<2.0.0)
 Requires-Dist: pytailwindcss (>=0.1.4) ; extra == "dev" or extra == "fastapidev"
-Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn[standard] (>=0.18.2,<0.19.0) ; extra == "dev" or extra == "fastapi" or extra == "fastapidev"
 Requires-Dist: valio (>=0.1.0-beta.5,<0.2.0)
 Requires-Dist: watchgod (>=0.8.2) ; extra == "dev" or extra == "fastapidev"
 Description-Content-Type: text/markdown
 
 <!--
```

