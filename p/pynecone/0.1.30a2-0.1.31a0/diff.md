# Comparing `tmp/pynecone-0.1.30a2.tar.gz` & `tmp/pynecone-0.1.31a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.30a2.tar", max compression
+gzip compressed data, was "pynecone-0.1.31a0.tar", max compression
```

## Comparing `pynecone-0.1.30a2.tar` & `pynecone-0.1.31a0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.30a2/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-15 02:04:07.603507 pynecone-0.1.30a2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.30a2/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-05-16 19:12:26.220987 pynecone-0.1.30a2/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.30a2/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.30a2/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.30a2/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.30a2/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-15 02:04:07.604581 pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     2345 2023-05-16 19:33:51.153974 pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     2999 2023-05-15 02:04:07.604822 pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.30a2/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.30a2/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.30a2/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.30a2/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      927 2023-05-15 02:04:07.606305 pynecone-0.1.30a2/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.30a2/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.30a2/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.30a2/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     7657 2023-05-16 19:33:51.154248 pynecone-0.1.30a2/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.30a2/pynecone/__init__.py
--rw-r--r--   0        0        0    20075 2023-05-15 02:04:07.606864 pynecone-0.1.30a2/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.30a2/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.30a2/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6290 2023-05-16 19:33:51.154440 pynecone-0.1.30a2/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.30a2/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.30a2/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6390 2023-05-15 17:32:17.391279 pynecone-0.1.30a2/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.30a2/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.30a2/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.30a2/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.30a2/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.30a2/pynecone/components/base/head.py
--rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.30a2/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.30a2/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    22653 2023-05-16 19:11:41.005106 pynecone-0.1.30a2/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.30a2/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.30a2/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.30a2/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.30a2/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.30a2/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.30a2/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.30a2/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.30a2/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.30a2/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.30a2/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.30a2/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.30a2/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.30a2/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.30a2/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.30a2/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.30a2/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.30a2/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.30a2/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.30a2/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1109 2023-05-16 05:05:39.515505 pynecone-0.1.30a2/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.30a2/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-16 19:11:41.005270 pynecone-0.1.30a2/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-16 19:11:41.005389 pynecone-0.1.30a2/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1949 2023-05-16 19:11:41.005504 pynecone-0.1.30a2/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2965 2023-05-16 19:11:41.005634 pynecone-0.1.30a2/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.30a2/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-05-16 19:11:41.005746 pynecone-0.1.30a2/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3897 2023-05-16 19:11:41.005870 pynecone-0.1.30a2/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.30a2/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-16 19:11:41.006022 pynecone-0.1.30a2/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-16 19:11:41.006148 pynecone-0.1.30a2/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-16 19:11:41.006264 pynecone-0.1.30a2/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3506 2023-05-16 19:11:41.006377 pynecone-0.1.30a2/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-16 19:11:41.006525 pynecone-0.1.30a2/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1552 2023-05-16 19:11:41.006661 pynecone-0.1.30a2/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1531 2023-05-16 19:11:41.006795 pynecone-0.1.30a2/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-16 19:11:41.006932 pynecone-0.1.30a2/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.30a2/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.30a2/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.30a2/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.30a2/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.30a2/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.30a2/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.30a2/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-16 19:11:41.007084 pynecone-0.1.30a2/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.30a2/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.30a2/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     2843 2023-05-16 19:11:41.007298 pynecone-0.1.30a2/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.30a2/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.30a2/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.30a2/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.30a2/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.30a2/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.30a2/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.30a2/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.30a2/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.30a2/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.30a2/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-16 19:11:41.007509 pynecone-0.1.30a2/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.30a2/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1400 2023-05-16 19:11:41.007692 pynecone-0.1.30a2/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.30a2/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.30a2/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.30a2/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.30a2/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.30a2/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.30a2/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-16 19:11:41.008011 pynecone-0.1.30a2/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4681 2023-05-16 19:11:41.008241 pynecone-0.1.30a2/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-16 19:11:41.008524 pynecone-0.1.30a2/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-16 19:11:41.008688 pynecone-0.1.30a2/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-05-16 19:11:41.008862 pynecone-0.1.30a2/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-16 19:11:41.009041 pynecone-0.1.30a2/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.30a2/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.30a2/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.30a2/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-05-16 19:11:41.009247 pynecone-0.1.30a2/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.30a2/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.30a2/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.30a2/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.30a2/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.30a2/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.30a2/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.30a2/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.30a2/pynecone/config.py
--rw-r--r--   0        0        0     8974 2023-05-17 00:07:29.187308 pynecone-0.1.30a2/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.30a2/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.30a2/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.30a2/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.30a2/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.30a2/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.30a2/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.30a2/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.30a2/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.30a2/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.30a2/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.30a2/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.30a2/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.30a2/pynecone/model.py
--rw-r--r--   0        0        0     7979 2023-05-15 17:32:17.393651 pynecone-0.1.30a2/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.30a2/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.30a2/pynecone/route.py
--rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.30a2/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.30a2/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.30a2/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     5318 2023-05-15 17:32:17.393927 pynecone-0.1.30a2/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.30a2/pynecone/utils/console.py
--rw-r--r--   0        0        0     3517 2023-05-15 02:04:07.622776 pynecone-0.1.30a2/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11346 2023-05-16 19:11:41.009451 pynecone-0.1.30a2/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.30a2/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.30a2/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10033 2023-05-16 04:11:28.941837 pynecone-0.1.30a2/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.30a2/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.30a2/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4389 2023-05-15 02:04:07.623635 pynecone-0.1.30a2/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.30a2/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30918 2023-05-16 19:11:41.009774 pynecone-0.1.30a2/pynecone/vars.py
--rw-r--r--   0        0        0     1798 2023-05-17 00:11:28.115554 pynecone-0.1.30a2/pyproject.toml
--rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.30a2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.31a0/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-17 17:15:44.662291 pynecone-0.1.31a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.31a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-05-16 19:12:26.220987 pynecone-0.1.31a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.31a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.31a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.31a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.31a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-15 02:04:07.604581 pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     2345 2023-05-17 03:31:04.693336 pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     2999 2023-05-15 02:04:07.604822 pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.31a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.31a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   254417 2023-05-15 02:04:07.606023 pynecone-0.1.31a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.31a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      927 2023-05-15 02:04:07.606305 pynecone-0.1.31a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.31a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.31a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.31a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     7657 2023-05-17 03:31:04.693493 pynecone-0.1.31a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1363 2023-05-15 02:04:07.606665 pynecone-0.1.31a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    20075 2023-05-15 02:04:07.606864 pynecone-0.1.31a0/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.31a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.31a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6290 2023-05-17 03:31:04.693642 pynecone-0.1.31a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2565 2023-05-15 02:04:07.607300 pynecone-0.1.31a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7384 2023-05-15 02:04:07.607425 pynecone-0.1.31a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6390 2023-05-15 17:32:17.391279 pynecone-0.1.31a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.31a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.31a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.31a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.31a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.31a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      930 2023-05-15 02:04:07.607989 pynecone-0.1.31a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1340 2023-05-15 02:04:07.608303 pynecone-0.1.31a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    22653 2023-05-17 03:31:04.693829 pynecone-0.1.31a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.31a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.31a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.31a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.31a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.31a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.31a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.31a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.31a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5157 2023-05-15 02:04:07.609333 pynecone-0.1.31a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.31a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2941 2023-05-15 02:04:07.609439 pynecone-0.1.31a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.31a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.31a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.31a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.31a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.31a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.31a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.31a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.31a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1109 2023-05-16 05:05:39.515505 pynecone-0.1.31a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.31a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-17 03:31:04.693986 pynecone-0.1.31a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-17 03:31:04.694099 pynecone-0.1.31a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1949 2023-05-17 03:31:04.694210 pynecone-0.1.31a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2965 2023-05-17 03:31:04.694346 pynecone-0.1.31a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.31a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-05-17 03:31:04.694475 pynecone-0.1.31a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3897 2023-05-17 03:31:04.694607 pynecone-0.1.31a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.31a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-17 03:31:04.694745 pynecone-0.1.31a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-17 03:31:04.694864 pynecone-0.1.31a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-17 03:31:04.694977 pynecone-0.1.31a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3506 2023-05-17 03:31:04.695098 pynecone-0.1.31a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-17 03:31:04.695208 pynecone-0.1.31a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1552 2023-05-17 03:31:04.695316 pynecone-0.1.31a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1531 2023-05-17 03:31:04.695426 pynecone-0.1.31a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-17 03:31:04.695540 pynecone-0.1.31a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.31a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.31a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.31a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.31a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.31a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      769 2023-05-15 02:04:07.614311 pynecone-0.1.31a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.31a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-17 03:31:04.695669 pynecone-0.1.31a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.31a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.31a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     2843 2023-05-17 03:31:04.695778 pynecone-0.1.31a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.31a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.31a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.31a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.31a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.31a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.31a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.31a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.31a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.31a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.31a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-17 03:31:04.695901 pynecone-0.1.31a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.31a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1400 2023-05-17 03:31:04.696029 pynecone-0.1.31a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.31a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.31a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1083 2023-05-15 02:04:07.616009 pynecone-0.1.31a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.31a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.31a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.31a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-17 03:31:04.696401 pynecone-0.1.31a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4681 2023-05-17 03:31:04.696630 pynecone-0.1.31a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-17 03:31:04.696777 pynecone-0.1.31a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-17 03:31:04.696908 pynecone-0.1.31a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-05-17 03:31:04.697043 pynecone-0.1.31a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-17 03:31:04.697172 pynecone-0.1.31a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.31a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.31a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.31a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-05-17 03:31:04.697339 pynecone-0.1.31a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.31a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.31a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.31a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      358 2023-05-15 02:04:07.618079 pynecone-0.1.31a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3288 2023-05-15 02:04:07.618181 pynecone-0.1.31a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.31a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.31a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.31a0/pynecone/config.py
+-rw-r--r--   0        0        0     8974 2023-05-17 17:15:44.662475 pynecone-0.1.31a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.31a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.31a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.31a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.31a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.31a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1283 2023-05-15 02:04:07.619213 pynecone-0.1.31a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.31a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.31a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10647 2023-05-15 17:32:17.393442 pynecone-0.1.31a0/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.31a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.31a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.31a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.31a0/pynecone/model.py
+-rw-r--r--   0        0        0     7979 2023-05-15 17:32:17.393651 pynecone-0.1.31a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.31a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.31a0/pynecone/route.py
+-rw-r--r--   0        0        0    29790 2023-05-15 02:04:07.621653 pynecone-0.1.31a0/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.31a0/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.31a0/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     6637 2023-05-17 17:59:43.752852 pynecone-0.1.31a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.31a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     4356 2023-05-17 17:15:44.662801 pynecone-0.1.31a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11320 2023-05-17 17:15:44.663013 pynecone-0.1.31a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.31a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.31a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10033 2023-05-17 03:31:04.698132 pynecone-0.1.31a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.31a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-05-15 02:04:07.623496 pynecone-0.1.31a0/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4389 2023-05-15 02:04:07.623635 pynecone-0.1.31a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.31a0/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30918 2023-05-17 03:31:04.698348 pynecone-0.1.31a0/pynecone/vars.py
+-rw-r--r--   0        0        0     1798 2023-05-17 18:00:07.740042 pynecone-0.1.31a0/pyproject.toml
+-rw-r--r--   0        0        0     9407 1970-01-01 00:00:00.000000 pynecone-0.1.31a0/PKG-INFO
```

### Comparing `pynecone-0.1.30a2/LICENSE` & `pynecone-0.1.31a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/README.md` & `pynecone-0.1.31a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 </div>
 
 ## 📦 1. Install
 
 Pynecone requires the following to get started:
 
 -   Python 3.7+
--   [Node.js 16.6.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
+-   [Node.js 16.8.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
 
 ```
 pip install pynecone
 ```
 
 ## 🥳 2. Create your first app
```

### Comparing `pynecone-0.1.30a2/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.31a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.31a0/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.31a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.31a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.31a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/web/package.json` & `pynecone-0.1.31a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.31a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.31a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.31a0/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/__init__.py` & `pynecone-0.1.31a0/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/app.py` & `pynecone-0.1.31a0/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/base.py` & `pynecone-0.1.31a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/compiler/compiler.py` & `pynecone-0.1.31a0/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/compiler/templates.py` & `pynecone-0.1.31a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/compiler/utils.py` & `pynecone-0.1.31a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/__init__.py` & `pynecone-0.1.31a0/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/base/bare.py` & `pynecone-0.1.31a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/base/document.py` & `pynecone-0.1.31a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/base/link.py` & `pynecone-0.1.31a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/base/meta.py` & `pynecone-0.1.31a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/component.py` & `pynecone-0.1.31a0/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/code.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/list.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/datadisplay/table.py` & `pynecone-0.1.31a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.31a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.31a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/feedback/alert.py` & `pynecone-0.1.31a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.31a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/feedback/progress.py` & `pynecone-0.1.31a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.31a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/feedback/spinner.py` & `pynecone-0.1.31a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/__init__.py` & `pynecone-0.1.31a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/button.py` & `pynecone-0.1.31a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/checkbox.py` & `pynecone-0.1.31a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.31a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/editable.py` & `pynecone-0.1.31a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.31a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.31a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/input.py` & `pynecone-0.1.31a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/numberinput.py` & `pynecone-0.1.31a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/pininput.py` & `pynecone-0.1.31a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/radio.py` & `pynecone-0.1.31a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.31a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/select.py` & `pynecone-0.1.31a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/slider.py` & `pynecone-0.1.31a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/switch.py` & `pynecone-0.1.31a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/textarea.py` & `pynecone-0.1.31a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/forms/upload.py` & `pynecone-0.1.31a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/graphing/plotly.py` & `pynecone-0.1.31a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/graphing/victory.py` & `pynecone-0.1.31a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/__init__.py` & `pynecone-0.1.31a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/box.py` & `pynecone-0.1.31a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/cond.py` & `pynecone-0.1.31a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/flex.py` & `pynecone-0.1.31a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/foreach.py` & `pynecone-0.1.31a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/grid.py` & `pynecone-0.1.31a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/html.py` & `pynecone-0.1.31a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/responsive.py` & `pynecone-0.1.31a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/stack.py` & `pynecone-0.1.31a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/layout/wrap.py` & `pynecone-0.1.31a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/media/avatar.py` & `pynecone-0.1.31a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/media/icon.py` & `pynecone-0.1.31a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/media/image.py` & `pynecone-0.1.31a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.31a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/navigation/link.py` & `pynecone-0.1.31a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.31a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/__init__.py` & `pynecone-0.1.31a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.31a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/drawer.py` & `pynecone-0.1.31a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/menu.py` & `pynecone-0.1.31a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/modal.py` & `pynecone-0.1.31a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/popover.py` & `pynecone-0.1.31a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.31a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.31a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/tags/tag.py` & `pynecone-0.1.31a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/tags/tagless.py` & `pynecone-0.1.31a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/components/typography/markdown.py` & `pynecone-0.1.31a0/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/config.py` & `pynecone-0.1.31a0/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/constants.py` & `pynecone-0.1.31a0/pynecone/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # App names and versions.
 # The name of the Pynecone package.
 MODULE_NAME = "pynecone"
 # The current version of Pynecone.
 VERSION = pkg_resources.get_distribution(MODULE_NAME).version
 # Minimum version of Node.js required to run Pynecone.
-MIN_NODE_VERSION = "16.6.0"
+MIN_NODE_VERSION = "16.8.0"
 
 # Valid bun versions.
 MIN_BUN_VERSION = "0.5.9"
 MAX_BUN_VERSION = "0.6.1"
 
 # Files and directories used to init a new project.
 # The root directory of the pynecone library.
```

### Comparing `pynecone-0.1.30a2/pynecone/el/constants/html.py` & `pynecone-0.1.31a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/el/constants/pynecone.py` & `pynecone-0.1.31a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/el/constants/react.py` & `pynecone-0.1.31a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/el/element.py` & `pynecone-0.1.31a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/el/elements/__init__.py` & `pynecone-0.1.31a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/el/precompile.py` & `pynecone-0.1.31a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/event.py` & `pynecone-0.1.31a0/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.31a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/middleware/middleware.py` & `pynecone-0.1.31a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/model.py` & `pynecone-0.1.31a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/pc.py` & `pynecone-0.1.31a0/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/route.py` & `pynecone-0.1.31a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/state.py` & `pynecone-0.1.31a0/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/style.py` & `pynecone-0.1.31a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/build.py` & `pynecone-0.1.31a0/pynecone/utils/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import subprocess
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Optional,
 )
 
+from rich.progress import Progress
+
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import path_ops, prerequisites
 
 if TYPE_CHECKING:
     from pynecone.app import App
 
@@ -91,18 +93,46 @@
     # Remove the static folder.
     path_ops.rm(constants.WEB_STATIC_DIR)
 
     # Generate the sitemap file.
     if deploy_url is not None:
         generate_sitemap(deploy_url)
 
-    # Export the Next app.
-    subprocess.run(
-        [prerequisites.get_package_manager(), "run", "export"], cwd=constants.WEB_DIR
-    )
+    # Create a progress object
+    progress = Progress()
+
+    # Add a single task to the progress object
+    task = progress.add_task("Building app... ", total=500)
+
+    # Start the progress bar
+    with progress:
+        # Run the subprocess command
+        process = subprocess.Popen(
+            [prerequisites.get_package_manager(), "run", "export"],
+            cwd=constants.WEB_DIR,
+            stderr=subprocess.DEVNULL,
+            stdout=subprocess.PIPE,  # Redirect stdout to a pipe
+            universal_newlines=True,  # Set universal_newlines to True for text mode
+        )
+
+        # Read the output of the subprocess line by line
+        if process.stdout:
+            for line in iter(process.stdout.readline, ""):
+                # Update the progress bar based on the output
+                if "Linting and checking " in line:
+                    progress.update(task, advance=100)
+                elif "Compiled successfully" in line:
+                    progress.update(task, advance=100)
+                elif "Route (pages)" in line:
+                    progress.update(task, advance=100)
+                elif "automatically rendered as static HTML" in line:
+                    progress.update(task, advance=100)
+                elif "Export successful" in line:
+                    progress.update(task, completed=500)
+                    break  # Exit the loop if the completion message is found
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
```

### Comparing `pynecone-0.1.30a2/pynecone/utils/console.py` & `pynecone-0.1.31a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/exec.py` & `pynecone-0.1.31a0/pynecone/utils/exec.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 import os
 import platform
 import subprocess
 from pathlib import Path
 from typing import TYPE_CHECKING
 
+import typer
 import uvicorn
+from rich import print
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import console, prerequisites, processes
 from pynecone.utils.build import export_app, setup_backend, setup_frontend
 from pynecone.utils.watch import AssetFolderWatch
 
@@ -26,14 +28,45 @@
     Args:
         root: root path of the project.
     """
     asset_watch = AssetFolderWatch(root)
     asset_watch.start()
 
 
+def run_process_and_launch_url(run_command: list[str], root: Path):
+    """Run the process and launch the URL.
+
+    Args:
+        run_command: The command to run.
+        root: root path of the project.
+    """
+    process = subprocess.Popen(
+        run_command,
+        cwd=constants.WEB_DIR,
+        env=os.environ,
+        stderr=subprocess.DEVNULL,
+        stdout=subprocess.PIPE,
+        universal_newlines=True,
+    )
+
+    message_found = False
+    if process.stdout:
+        for line in process.stdout:
+            if "ready started server on" in line:
+                url = line.split("url: ")[-1].strip()
+                print(f"App running at: [bold green]{url}")
+                typer.launch(url)
+                message_found = True
+                break
+
+    if not message_found and process.stdout:
+        for line in process.stdout:
+            print(line, end="")
+
+
 def run_frontend(app: App, root: Path, port: str):
     """Run the frontend.
 
     Args:
         app: The app.
         root: root path of the project.
         port: port of the app.
@@ -49,20 +82,16 @@
 
     # Compile the frontend.
     app.compile(force_compile=True)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().port if port is None else port
-
-    # Run the frontend in development mode.
-    subprocess.Popen(
-        [prerequisites.get_package_manager(), "run", "dev"],
-        cwd=constants.WEB_DIR,
-        env=os.environ,
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "dev"], root
     )
 
 
 def run_frontend_prod(app: App, root: Path, port: str):
     """Run the frontend.
 
     Args:
@@ -76,18 +105,17 @@
     # Export the app.
     export_app(app)
 
     # Set the port.
     os.environ["PORT"] = get_config().port if port is None else port
 
     # Run the frontend in production mode.
-    subprocess.Popen(
-        [prerequisites.get_package_manager(), "run", "prod"],
-        cwd=constants.WEB_DIR,
-        env=os.environ,
+    console.rule("[bold green]App Running")
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "prod"], root
     )
 
 
 def run_backend(
     app_name: str, port: int, loglevel: constants.LogLevel = constants.LogLevel.ERROR
 ):
     """Run the backend.
```

### Comparing `pynecone-0.1.30a2/pynecone/utils/format.py` & `pynecone-0.1.31a0/pynecone/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,16 +294,15 @@
             )
             for name, val in event_spec.args
         ]
     )
     event_args = [
         wrap(format_event_handler(event_spec.handler), '"'),
     ]
-    if len(args) > 0:
-        event_args.append(wrap(args, "{"))
+    event_args.append(wrap(args, "{"))
 
     if event_spec.client_handler_name:
         event_args.append(wrap(event_spec.client_handler_name, '"'))
     return f"E({', '.join(event_args)})"
 
 
 def format_full_control_event(event_chain: EventChain) -> str:
```

### Comparing `pynecone-0.1.30a2/pynecone/utils/imports.py` & `pynecone-0.1.31a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/path_ops.py` & `pynecone-0.1.31a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/prerequisites.py` & `pynecone-0.1.31a0/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/processes.py` & `pynecone-0.1.31a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/telemetry.py` & `pynecone-0.1.31a0/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/types.py` & `pynecone-0.1.31a0/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/utils/watch.py` & `pynecone-0.1.31a0/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pynecone/vars.py` & `pynecone-0.1.31a0/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.30a2/pyproject.toml` & `pynecone-0.1.31a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.30a2"
+version = "0.1.31a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.30a2/PKG-INFO` & `pynecone-0.1.31a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.30a2
+Version: 0.1.31a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -54,15 +54,15 @@
 </div>
 
 ## 📦 1. Install
 
 Pynecone requires the following to get started:
 
 -   Python 3.7+
--   [Node.js 16.6.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
+-   [Node.js 16.8.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
 
 ```
 pip install pynecone
 ```
 
 ## 🥳 2. Create your first app
```

