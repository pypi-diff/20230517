# Comparing `tmp/jupytercad-0.1.0b0.tar.gz` & `tmp/jupytercad-0.1.0rc0.tar.gz`

## Comparing `jupytercad-0.1.0b0.tar` & `jupytercad-0.1.0rc0.tar`

### file list

```diff
@@ -1,364 +1,364 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.eslintignore
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.prettierrc
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.yarnrc.yml
--rw-r--r--   0        0        0    15547 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/CHANGELOG.md
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/RELEASE.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/install.json
--rw-r--r--   0        0        0   340807 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad-screenshot.png
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/lerna.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/tsconfig.eslint.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/tsconfigbase.json
--rw-r--r--   0        0        0   431231 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/yarn.lock
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/etc/jupyter/jupyter_server_config.d/jupytercad.json
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/_version.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/fcstd_ydoc.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/jcad_ydoc.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/cadapp/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/cadapp/cadapp.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/cadapp/utils.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/cadapp/templates/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/__init__.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/loader.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/base_prop.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_angle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_bool.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_distance.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_geometrylist.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_length.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_link.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_link_list.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_map.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_partshape.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/property_placement.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/geometry/__init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/geometry/geom_circle.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/freecad/props/geometry/geom_linesegment.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/package.json
--rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/184.f67942d2a32b8bee8e5a.js
--rw-r--r--   0        0        0    85576 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/213.e34e5a84a96685d42bb8.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/268.f13adb88b2b07e571b26.js
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
--rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/422.39a95e19d3a414516796.js
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
--rw-r--r--   0        0        0   122782 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/544.b89e05aa19fe64ba7c4c.js
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/643.79ba7cf0e51f78fa228f.js
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/647.70d8d38a29b0cea56655.js
--rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
--rw-r--r--   0        0        0    12565 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/711.efce9e63ee6469afd671.js
--rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
--rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
--rw-r--r--   0        0        0   116736 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/733.16386271c81bb82d7032.js
--rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/816.f833ad40945917f858b9.js
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
--rw-r--r--   0        0        0   254928 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/842.b1819d35423472952117.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/842.b1819d35423472952117.js.LICENSE.txt
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
--rw-r--r--   0        0        0   623604 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js.LICENSE.txt
--rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
--rw-r--r--   0        0        0  5076021 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0    13057 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/remoteEntry.47104f3a5a3d3b4cf3f6.js
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/style.js
--rw-r--r--   0        0        0    67994 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/notebook/__init__.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/notebook/cad_document.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/notebook/utils.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/notebook/y_connector.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/jupytercad/notebook/objects/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/scripts/bump-version.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/package.json
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/tsconfig.json
--rw-r--r--   0        0        0    67548 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/webpack.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/bootstrap.js
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/main.d.ts
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/main.js
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/style.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/browser/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/mainmenu/widget.d.ts
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/mainmenu/widget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/paths/index.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/bootstrap.d.ts
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/bootstrap.js
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/main.d.ts
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/main.js
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/app.d.ts
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/app.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/shell.d.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/shell.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/browser/index.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/mainmenu/widget.d.ts
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/mainmenu/widget.js
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/paths/index.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/bootstrap.ts
--rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/main.ts
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/app.ts
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/shell.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/browser/index.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/mainmenu/widget.tsx
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/paths/index.ts
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-app/style/index.js
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/extension.webpack.config.js
--rw-r--r--   0        0        0     4799 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/schema.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/tsconfig.json
--rw-r--r--   0        0        0   187684 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/tsconfig.worker.json
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/worker.webpack.config.js
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/commands.d.ts
--rw-r--r--   0        0        0    20755 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/commands.js
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/factory.d.ts
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/factory.js
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/formdialog.d.ts
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/formdialog.js
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/index.d.ts
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/index.js
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/mainview.d.ts
--rw-r--r--   0        0        0    38055 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/mainview.js
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/model.d.ts
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/model.js
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/token.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/token.js
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/tools.d.ts
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/tools.js
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/types.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/types.js
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/widget.d.ts
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/widget.js
--rw-r--r--   0        0        0    85429 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker.js
--rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/_interface/forms.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/message.d.ts
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/message.js
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/model.d.ts
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/model.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/view.d.ts
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/view.js
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/plugins.js
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/plugins.js
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/index.js
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/model.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/token.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/view.js
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/annotations.d.ts
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/annotations.js
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/formbuilder.js
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/header.d.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/header.js
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/leftpanel.js
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/model.d.ts
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/model.js
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objectproperties.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
--rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objecttree.js
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/rightpanel.js
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/box.json
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cone.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cut.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cylinder.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/extrusion.json
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/fuse.json
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/geomCircle.json
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/geomLineSegment.json
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/intersection.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/jcad.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/placement.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/sketch.json
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/sphere.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/torus.json
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/helper.d.ts
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/helper.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/panzoom.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
--rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/types.js
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/circle.js
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/line.js
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/elements/point.js
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/widget.d.ts
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/widget.js
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/actions.d.ts
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/actions.js
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occapi.d.ts
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occapi.js
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occparser.d.ts
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occparser.js
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/types.d.ts
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/types.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/utils.d.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/utils.js
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/worker.d.ts
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/worker.js
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
--rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/commands.ts
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/factory.ts
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/formdialog.tsx
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/index.ts
--rw-r--r--   0        0        0    34616 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/mainview.tsx
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/svg.d.ts
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/token.ts
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/tools.ts
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/types.ts
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/widget.tsx
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/box.d.ts
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cone.d.ts
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cut.d.ts
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cylinder.d.ts
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/extrusion.d.ts
--rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/forms.json
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/fuse.d.ts
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/intersection.d.ts
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/jcad.d.ts
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/placement.d.ts
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/sketch.d.ts
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/sphere.d.ts
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/torus.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/message.tsx
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/model.ts
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/view.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/fcplugin/plugins.ts
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/jcadplugin/plugins.ts
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/index.ts
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/model.ts
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/token.ts
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/view.ts
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/annotations.tsx
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/formbuilder.tsx
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/header.tsx
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/leftpanel.tsx
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/model.ts
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/objectproperties.tsx
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/objecttree.tsx
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/rightpanel.tsx
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/box.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cone.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cut.json
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cylinder.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/extrusion.json
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/fuse.json
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/geomCircle.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/geomLineSegment.json
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/intersection.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/jcad.json
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/placement.json
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/sketch.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/sphere.json
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/torus.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/helper.tsx
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/panzoom.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
--rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/types.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/elements/circle.ts
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/elements/line.ts
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/elements/point.ts
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/toolbar/widget.tsx
--rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/actions.ts
--rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/occapi.ts
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/occparser.ts
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/types.ts
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/utils.ts
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/worker.ts
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/index.js
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/axes.svg
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/box.svg
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cone.svg
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cut.svg
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cylinder.svg
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/extrusion.svg
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/intersection.svg
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/jvcontrol.svg
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/minimize.svg
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/sphere.svg
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/torus.svg
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/union.svg
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/visibility.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/visibilityOff.svg
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/build.yml
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/build_opencascade.js
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/package.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/build.yml
--rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
--rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
--rwxr-xr-x   0        0        0  5076021 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/LICENSE
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/README.md
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     4363 2020-02-02 00:00:00.000000 jupytercad-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.eslintignore
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.prettierrc
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.yarnrc.yml
+-rw-r--r--   0        0        0    15575 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/CHANGELOG.md
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/RELEASE.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/install.json
+-rw-r--r--   0        0        0   340807 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad-screenshot.png
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/lerna.json
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/tsconfigbase.json
+-rw-r--r--   0        0        0   431227 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/yarn.lock
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/etc/jupyter/jupyter_server_config.d/jupytercad.json
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/_version.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/fcstd_ydoc.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/jcad_ydoc.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/cadapp/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/cadapp/cadapp.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/cadapp/utils.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/cadapp/templates/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/__init__.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/loader.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/base_prop.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_angle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_bool.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_distance.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_geometrylist.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_length.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_link.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_link_list.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_map.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_partshape.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/property_placement.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/geometry/__init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/geometry/geom_circle.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/freecad/props/geometry/geom_linesegment.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/package.json
+-rw-r--r--   0        0        0    52116 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/184.f67942d2a32b8bee8e5a.js
+-rw-r--r--   0        0        0    85576 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/213.e34e5a84a96685d42bb8.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/268.f13adb88b2b07e571b26.js
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js
+-rw-r--r--   0        0        0    59793 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/422.39a95e19d3a414516796.js
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js
+-rw-r--r--   0        0        0   122782 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/544.a56e146ce6205a7c3f5c.js
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/643.79ba7cf0e51f78fa228f.js
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/647.70d8d38a29b0cea56655.js
+-rw-r--r--   0        0        0    18686 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js.LICENSE.txt
+-rw-r--r--   0        0        0    12565 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/711.efce9e63ee6469afd671.js
+-rw-r--r--   0        0        0     8086 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js
+-rw-r--r--   0        0        0   183517 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js
+-rw-r--r--   0        0        0   116736 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/733.16386271c81bb82d7032.js
+-rw-r--r--   0        0        0    31683 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js.LICENSE.txt
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/816.f833ad40945917f858b9.js
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js
+-rw-r--r--   0        0        0   254928 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/842.b1819d35423472952117.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/842.b1819d35423472952117.js.LICENSE.txt
+-rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js
+-rw-r--r--   0        0        0   623604 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js.LICENSE.txt
+-rw-r--r--   0        0        0   114029 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js
+-rw-r--r--   0        0        0  5076021 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/remoteEntry.915ba599f76e726e9820.js
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/style.js
+-rw-r--r--   0        0        0    67994 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/notebook/__init__.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/notebook/cad_document.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/notebook/utils.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/notebook/y_connector.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/jupytercad/notebook/objects/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/scripts/bump-version.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/package.json
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/tsconfig.json
+-rw-r--r--   0        0        0    67548 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/webpack.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/bootstrap.js
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/main.d.ts
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/main.js
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/style.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/mainmenu/widget.d.ts
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/mainmenu/widget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/paths/index.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/bootstrap.d.ts
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/bootstrap.js
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/main.d.ts
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/main.js
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/app.d.ts
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/app.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/shell.d.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/shell.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/browser/index.d.ts
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/browser/index.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.d.ts
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/mainmenu/index.js
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/mainmenu/widget.d.ts
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/mainmenu/widget.js
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/paths/index.d.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/paths/index.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/bootstrap.ts
+-rw-r--r--   0        0        0     6205 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/main.ts
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/app.ts
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/shell.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/browser/index.ts
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/mainmenu/widget.tsx
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/paths/index.ts
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-app/style/index.js
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/extension.webpack.config.js
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/schema.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/tsconfig.json
+-rw-r--r--   0        0        0   187684 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/tsconfig.worker.json
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/worker.webpack.config.js
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/commands.d.ts
+-rw-r--r--   0        0        0    20755 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/commands.js
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/factory.d.ts
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/factory.js
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/formdialog.d.ts
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/formdialog.js
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/index.d.ts
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/index.js
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/mainview.d.ts
+-rw-r--r--   0        0        0    38055 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/mainview.js
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/model.d.ts
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/model.js
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/token.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/token.js
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/tools.d.ts
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/tools.js
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/types.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/types.js
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/widget.d.ts
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/widget.js
+-rw-r--r--   0        0        0    85429 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker.js
+-rw-r--r--   0        0        0    26960 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/_interface/forms.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/message.d.ts
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/message.js
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/model.d.ts
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/model.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/view.d.ts
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/view.js
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/plugins.js
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/plugins.d.ts
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/plugins.js
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/index.d.ts
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/index.js
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/model.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/token.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/view.js
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/annotations.d.ts
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/annotations.js
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/formbuilder.js
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/header.d.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/header.js
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/leftpanel.js
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/model.d.ts
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/model.js
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objectproperties.d.ts
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objectproperties.js
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objecttree.d.ts
+-rw-r--r--   0        0        0    12865 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objecttree.js
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/rightpanel.d.ts
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/rightpanel.js
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/box.json
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cone.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cut.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cylinder.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/extrusion.json
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/fuse.json
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/geomCircle.json
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/intersection.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/jcad.json
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/placement.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/sketch.json
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/sphere.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/torus.json
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/helper.d.ts
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/helper.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/panzoom.d.ts
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/panzoom.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.d.ts
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts
+-rw-r--r--   0        0        0    19357 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/types.js
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/circle.d.ts
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/circle.js
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/line.d.ts
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/line.js
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/point.d.ts
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/elements/point.js
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/widget.d.ts
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/widget.js
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/actions.d.ts
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/actions.js
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occapi.d.ts
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occapi.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occparser.d.ts
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occparser.js
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/types.d.ts
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/types.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/utils.d.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/utils.js
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/worker.d.ts
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/worker.js
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.d.ts
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/geometry/geomLineSegment.js
+-rw-r--r--   0        0        0    17493 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/commands.ts
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/factory.ts
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/formdialog.tsx
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/index.ts
+-rw-r--r--   0        0        0    34616 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/mainview.tsx
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/svg.d.ts
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/token.ts
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/tools.ts
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/types.ts
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/widget.tsx
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/box.d.ts
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cone.d.ts
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cut.d.ts
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cylinder.d.ts
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/extrusion.d.ts
+-rw-r--r--   0        0        0    19613 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/forms.json
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/fuse.d.ts
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/intersection.d.ts
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/jcad.d.ts
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/placement.d.ts
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/sketch.d.ts
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/sphere.d.ts
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/torus.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/message.tsx
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/model.ts
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/view.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/fcplugin/plugins.ts
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/jcadplugin/plugins.ts
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/index.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/model.ts
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/token.ts
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/view.ts
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/annotations.tsx
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/formbuilder.tsx
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/header.tsx
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/leftpanel.tsx
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/model.ts
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/objectproperties.tsx
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/objecttree.tsx
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/rightpanel.tsx
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/box.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cone.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cut.json
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cylinder.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/extrusion.json
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/fuse.json
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/geomCircle.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/geomLineSegment.json
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/intersection.json
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/jcad.json
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/placement.json
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/sketch.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/sphere.json
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/torus.json
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/helper.tsx
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/panzoom.ts
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts
+-rw-r--r--   0        0        0    16285 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/types.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/elements/circle.ts
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/elements/line.ts
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/elements/point.ts
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/toolbar/widget.tsx
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/actions.ts
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/occapi.ts
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/occparser.ts
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/types.ts
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/utils.ts
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/worker.ts
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/geometry/geomLineSegment.ts
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/index.js
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/axes.svg
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/box.svg
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cone.svg
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cut.svg
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cylinder.svg
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/extrusion.svg
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/intersection.svg
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/jvcontrol.svg
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/minimize.svg
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/sphere.svg
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/torus.svg
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/union.svg
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/visibility.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/visibilityOff.svg
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/build.yml
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/build_opencascade.js
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/package.json
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/build.yml
+-rw-r--r--   0        0        0   129654 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts
+-rw-r--r--   0        0        0   123823 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.version
+-rwxr-xr-x   0        0        0  5076021 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/README.md
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 jupytercad-0.1.0rc0/PKG-INFO
```

### Comparing `jupytercad-0.1.0b0/.eslintrc.js` & `jupytercad-0.1.0rc0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/CHANGELOG.md` & `jupytercad-0.1.0rc0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.0rc0
+
+No merged PRs
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.0b0
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.1.0a2...6fee6db19323c0c8d48d6e3f0060a0de0029f5c9))
 
 ### Enhancements made
 
 - Update to JupyterLab 4 [#147](https://github.com/QuantStack/jupytercad/pull/147) ([@martinRenou](https://github.com/martinRenou))
@@ -26,16 +32,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/QuantStack/jupytercad/graphs/contributors?from=2023-04-26&to=2023-05-17&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Agithub-actions+updated%3A2023-04-26..2023-05-17&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3AmartinRenou+updated%3A2023-04-26..2023-05-17&type=Issues) | [@trungleduc](https://github.com/search?q=repo%3AQuantStack%2Fjupytercad+involves%3Atrungleduc+updated%3A2023-04-26..2023-05-17&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.0a2
 
 ([Full Changelog](https://github.com/QuantStack/jupytercad/compare/v0.1.0a1...2f7b81060a1adab614bb6df1284382b0a1a5a546))
 
 ### Enhancements made
 
 - Hide source objects after executing operators [#117](https://github.com/QuantStack/jupytercad/pull/117) ([@trungleduc](https://github.com/trungleduc))
```

### Comparing `jupytercad-0.1.0b0/CONTRIBUTING.md` & `jupytercad-0.1.0rc0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/RELEASE.md` & `jupytercad-0.1.0rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad-screenshot.png` & `jupytercad-0.1.0rc0/jupytercad-screenshot.png`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/package.json` & `jupytercad-0.1.0rc0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.1.0-rc0'"}*

```diff
@@ -49,12 +49,12 @@
         "eslint:check": "eslint . --ext .ts,.tsx",
         "lint": "jlpm run prettier && jlpm run eslint",
         "lint:check": "jlpm run prettier:check && jlpm run eslint:check",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "prettier --list-different \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "test": "lerna run test"
     },
-    "version": "0.1.0-b0",
+    "version": "0.1.0-rc0",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `jupytercad-0.1.0b0/tsconfigbase.json` & `jupytercad-0.1.0rc0/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/yarn.lock` & `jupytercad-0.1.0rc0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -888,15 +888,15 @@
   dependencies:
     "@apidevtools/json-schema-ref-parser": ^9.0.9
     "@deathbeds/jupyterlab-rjsf": ^1.1.0
     "@jupyter-widgets/base": ^6.0.2
     "@jupyter/collaboration": ^1.0.0-alpha.7
     "@jupyter/docprovider": ^1.0.0-alpha.8
     "@jupyter/ydoc": ^0.3.4 || ^1.0.2
-    "@jupytercad/jupytercad-opencascade": ^0.1.1-beta.0
+    "@jupytercad/jupytercad-opencascade": ^0.1.1-rc.0
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/docregistry": ^4.0.0
     "@jupyterlab/filebrowser": ^4.0.0
     "@jupyterlab/launcher": ^4.0.0
@@ -928,15 +928,15 @@
     ts-loader: ^9.2.6
     typescript: ^5
     uuid: ^8.3.2
     webpack: ^5.76.3
   languageName: unknown
   linkType: soft
 
-"@jupytercad/jupytercad-opencascade@^0.1.1-beta.0, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
+"@jupytercad/jupytercad-opencascade@^0.1.1-rc.0, @jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade":
   version: 0.0.0-use.local
   resolution: "@jupytercad/jupytercad-opencascade@workspace:packages/jupytercad-opencascade"
   dependencies:
     js-yaml: ^4.1.0
     rimraf: ^3.0.2
   languageName: unknown
   linkType: soft
```

### Comparing `jupytercad-0.1.0b0/jupytercad/fcstd_ydoc.py` & `jupytercad-0.1.0rc0/jupytercad/fcstd_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/jcad_ydoc.py` & `jupytercad-0.1.0rc0/jupytercad/jcad_ydoc.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/cadapp/cadapp.py` & `jupytercad-0.1.0rc0/jupytercad/cadapp/cadapp.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/cadapp/utils.py` & `jupytercad-0.1.0rc0/jupytercad/cadapp/utils.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/cadapp/templates/index.html` & `jupytercad-0.1.0rc0/jupytercad/cadapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/loader.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/loader.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/base_prop.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/base_prop.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/property_geometrylist.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/property_geometrylist.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/property_partshape.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/property_partshape.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/property_placement.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/property_placement.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/geometry/geom_circle.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/geometry/geom_circle.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/freecad/props/geometry/geom_linesegment.py` & `jupytercad-0.1.0rc0/jupytercad/freecad/props/geometry/geom_linesegment.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/package.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969621212121212%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.1.1-rc.0'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.1.0-rc.0'"}*

```diff
@@ -7,15 +7,15 @@
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter-widgets/base": "^6.0.2",
         "@jupyter/collaboration": "^1.0.0-alpha.7",
         "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.1.1-beta.0",
+        "@jupytercad/jupytercad-opencascade": "^0.1.1-rc.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -55,19 +55,14 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/jupytercad",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.47104f3a5a3d3b4cf3f6.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "../../jupytercad/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             },
@@ -117,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0-beta.0"
+    "version": "0.1.0-rc.0"
 }
```

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/184.f67942d2a32b8bee8e5a.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/184.f67942d2a32b8bee8e5a.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/213.e34e5a84a96685d42bb8.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/213.e34e5a84a96685d42bb8.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/268.f13adb88b2b07e571b26.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/268.f13adb88b2b07e571b26.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/288.11fba3e29cc454c9c071.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/379.5df518c877987fc7ca0c.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/406.5ed89c99d9b3043c85c0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/422.39a95e19d3a414516796.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/422.39a95e19d3a414516796.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/52.477d969cb88d8007c4f0.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/544.b89e05aa19fe64ba7c4c.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/544.a56e146ce6205a7c3f5c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1534,15 +1534,15 @@
                     })), super({
                         title: e.title,
                         body: o,
                         buttons: [a.Dialog.cancelButton()]
                     }), this.addClass("jpcad-property-FormDialog")
                 }
             }
-            const me = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
+            const me = JSON.parse('{"Part::GeomCircle":{"type":"object","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},"Part::GeomLineSegment":{"type":"object","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}},"Placement of the box":{"type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Part::Box":{"type":"object","required":["Length","Width","Height","Placement"],"additionalProperties":false,"properties":{"Length":{"type":"number","description":"The length of the box"},"Width":{"type":"number","description":"The width of the box"},"Height":{"type":"number","description":"The height of the box"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cone":{"type":"object","required":["Radius1","Radius2","Height","Angle","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The bottom radius of the cone"},"Radius2":{"type":"number","description":"The top radius of the cone"},"Height":{"type":"number","description":"The height of the cone"},"Angle":{"type":"number","description":"The angle of the cone"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cut":{"type":"object","required":["Base","Tool","Refine","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"The base of the cut operator","fcType":"App::PropertyLink"},"Tool":{"type":"string","description":"The tool of the cut operator","fcType":"App::PropertyLink"},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Cylinder":{"type":"object","required":["Radius","Angle","Height","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"Radius of the cylinder"},"Height":{"type":"number","description":"Height of the cylinder"},"Angle":{"type":"number","description":"Angle of the cylinder"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Extrusion":{"type":"object","required":["Base","Dir","LengthFwd","LengthRev","Solid","Placement"],"additionalProperties":false,"properties":{"Base":{"type":"string","description":"Shape to extrude","fcType":"App::PropertyLink"},"Dir":{"type":"array","description":"Direction of extrusion","items":{"type":"number"}},"LengthFwd":{"type":"number","description":"Length of extrusion along the direction"},"LengthRev":{"type":"number","description":"Length of extrusion against the direction"},"Solid":{"type":"boolean","description":"If true, creating a solid"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiFuse":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The shapes of the individual elements","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::MultiCommon":{"type":"object","required":["Shapes","Refine","Placement"],"additionalProperties":false,"properties":{"Shapes":{"type":"array","description":"The objects to intersect","fcType":"App::PropertyLinkList","items":{"type":"string"}},"Refine":{"type":"boolean","description":"Refine shape"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Sketcher::SketchObject":{"type":"object","required":["AttachmentOffset","Geometry"],"additionalProperties":false,"properties":{"AttachmentOffset":{"description":"The attachment offset","type":"object","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}},"Geometry":{"type":"array","description":"The geometry list","items":{"anyOf":[{"type":"object","description":"Part::GeomCircle","title":"IGeomCircle","required":["TypeId","CenterX","CenterY","CenterZ","NormalX","NormalY","NormalZ","AngleXU","Radius"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomCircle","description":"Geometry type"},"CenterX":{"type":"number","description":"CenterX"},"CenterY":{"type":"number","description":"CenterY"},"CenterZ":{"type":"number","description":"CenterZ"},"NormalX":{"type":"number","description":"NormalX"},"NormalY":{"type":"number","description":"NormalY"},"NormalZ":{"type":"number","description":"NormalZ"},"AngleXU":{"type":"number","description":"AngleXU"},"Radius":{"type":"number","description":"Radius"}}},{"type":"object","description":"Part::GeomLineSegment","title":"IGeomLineSegment","required":["TypeId","StartX","StartY","StartZ","EndX","EndY","EndZ"],"additionalProperties":false,"properties":{"TypeId":{"const":"Part::GeomLineSegment","description":"Geometry type"},"StartX":{"type":"number","description":"StartX"},"StartY":{"type":"number","description":"StartY"},"StartZ":{"type":"number","description":"StartZ"},"EndX":{"type":"number","description":"EndX"},"EndY":{"type":"number","description":"EndY"},"EndZ":{"type":"number","description":"EndZ"}}}]}},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Sphere":{"type":"object","required":["Radius","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius":{"type":"number","description":"The radius of the sphere"},"Angle1":{"type":"number","description":"The angle of the sphere"},"Angle2":{"type":"number","description":"The angle of the sphere"},"Angle3":{"type":"number","description":"The angle of the sphere"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}},"Part::Torus":{"type":"object","required":["Radius1","Radius2","Angle1","Angle2","Angle3","Placement"],"additionalProperties":false,"properties":{"Radius1":{"type":"number","description":"The radius of the torus"},"Radius2":{"type":"number","description":"The radius of the torus"},"Angle1":{"type":"number","description":"The angle of the torus"},"Angle2":{"type":"number","description":"The angle of the torus"},"Angle3":{"type":"number","description":"The angle of the torus"},"Placement":{"type":"object","description":"Placement of the box","additionalProperties":false,"required":["Position","Axis","Angle"],"properties":{"Position":{"type":"array","description":"Position of the Placement","items":{"type":"number"}},"Axis":{"type":"array","description":"Axis of the Placement","items":{"type":"number"}},"Angle":{"type":"number","description":"Angle of the Placement"}}}}}}');
             var ue = function(e, t) {
                 var n = {};
                 for (var s in e) Object.prototype.hasOwnProperty.call(e, s) && t.indexOf(s) < 0 && (n[s] = e[s]);
                 if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                     var o = 0;
                     for (s = Object.getOwnPropertySymbols(e); o < s.length; o++) t.indexOf(s[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, s[o]) && (n[s[o]] = e[s[o]])
                 }
```

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/643.79ba7cf0e51f78fa228f.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/643.79ba7cf0e51f78fa228f.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/647.70d8d38a29b0cea56655.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/647.70d8d38a29b0cea56655.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/651.3736a4bd9cf2725cc067.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/711.efce9e63ee6469afd671.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/711.efce9e63ee6469afd671.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/712.3d4b32523dbb4dff584d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/730.5a8c1aad713514a0a596.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/733.16386271c81bb82d7032.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/733.16386271c81bb82d7032.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/761.1bd8bdc8d51f62af816d.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/78.8e87e13a67c31f2732c7.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/811.d1c8b6a87faba2d069bd.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/816.f833ad40945917f858b9.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/816.f833ad40945917f858b9.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/833.253bc84b61cd4e2beb80.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/842.b1819d35423472952117.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/842.b1819d35423472952117.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/847.6efcc69e25d704ee7090.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/860.9dcab30c320fd0b9cfe1.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/955.f2d085c56e6a6be87fcc.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/963.ba192cdc34bc5ccdfe40.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/jupytercad.opencascade.wasm` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/remoteEntry.47104f3a5a3d3b4cf3f6.js` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/remoteEntry.915ba599f76e726e9820.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, d, f, l, u, i, c, s, b, p, h, m, v, y, j, g, P, w, _, x, O, S = {
+    var e, r, t, a, n, d, o, f, l, u, i, c, s, b, p, h, m, v, y, j, g, P, w, _, x, O, S = {
             8634: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(277), t.e(930), t.e(726), t.e(995), t.e(544)]).then((() => () => t(38790))),
                         "./extension": () => Promise.all([t.e(651), t.e(78), t.e(963), t.e(29), t.e(277), t.e(930), t.e(726), t.e(995), t.e(544)]).then((() => () => t(38790))),
                         "./style": () => Promise.all([t.e(847), t.e(643)]).then((() => () => t(76643)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    d = (e, r) => {
                         if (t.S) {
                             var a = "default",
                                 n = t.S[a];
                             if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
                     get: () => n,
-                    init: () => o
+                    init: () => d
                 })
             }
         },
         E = {};
 
     function k(e) {
         var r = E[e];
@@ -46,19 +46,19 @@
         if (1 & a && (t = this(t)), 8 & a) return t;
         if ("object" == typeof t && t) {
             if (4 & a && t.__esModule) return t;
             if (16 & a && "function" == typeof t.then) return t
         }
         var n = Object.create(null);
         k.r(n);
-        var o = {};
+        var d = {};
         e = e || [null, r({}), r([]), r(r)];
-        for (var d = 2 & a && t;
-            "object" == typeof d && !~e.indexOf(d); d = r(d)) Object.getOwnPropertyNames(d).forEach((e => o[e] = () => t[e]));
-        return o.default = () => t, k.d(n, o), n
+        for (var o = 2 & a && t;
+            "object" == typeof o && !~e.indexOf(o); o = r(o)) Object.getOwnPropertyNames(o).forEach((e => d[e] = () => t[e]));
+        return d.default = () => t, k.d(n, d), n
     }, k.d = (e, r) => {
         for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
         29: "31e53f091cdbd8ff9f81",
@@ -68,15 +68,15 @@
         268: "f13adb88b2b07e571b26",
         277: "14c734342fd685e09584",
         288: "11fba3e29cc454c9c071",
         379: "5df518c877987fc7ca0c",
         391: "9d6532e5627314483b2a",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "b89e05aa19fe64ba7c4c",
+        544: "a56e146ce6205a7c3f5c",
         643: "79ba7cf0e51f78fa228f",
         647: "70d8d38a29b0cea56655",
         651: "3736a4bd9cf2725cc067",
         711: "efce9e63ee6469afd671",
         712: "3d4b32523dbb4dff584d",
         726: "fa8a171cbe517071fb0a",
         730: "5a8c1aad713514a0a596",
@@ -102,15 +102,15 @@
         268: "f13adb88b2b07e571b26",
         277: "14c734342fd685e09584",
         288: "11fba3e29cc454c9c071",
         379: "5df518c877987fc7ca0c",
         391: "9d6532e5627314483b2a",
         406: "5ed89c99d9b3043c85c0",
         422: "39a95e19d3a414516796",
-        544: "b89e05aa19fe64ba7c4c",
+        544: "a56e146ce6205a7c3f5c",
         643: "79ba7cf0e51f78fa228f",
         647: "70d8d38a29b0cea56655",
         651: "3736a4bd9cf2725cc067",
         711: "efce9e63ee6469afd671",
         712: "3d4b32523dbb4dff584d",
         726: "fa8a171cbe517071fb0a",
         730: "5a8c1aad713514a0a596",
@@ -131,37 +131,37 @@
     } [e], k.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupytercad/jupytercad-extension:", k.l = (e, r, n, o) => {
+    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupytercad/jupytercad-extension:", k.l = (e, r, n, d) => {
         if (t[e]) t[e].push(r);
         else {
-            var d, f;
+            var o, f;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
                     var i = l[u];
                     if (i.getAttribute("src") == e || i.getAttribute("data-webpack") == a + n) {
-                        d = i;
+                        o = i;
                         break
                     }
                 }
-            d || (f = !0, (d = document.createElement("script")).charset = "utf-8", d.timeout = 120, k.nc && d.setAttribute("nonce", k.nc), d.setAttribute("data-webpack", a + n), d.src = e), t[e] = [r];
+            o || (f = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, k.nc && o.setAttribute("nonce", k.nc), o.setAttribute("data-webpack", a + n), o.src = e), t[e] = [r];
             var c = (r, a) => {
-                    d.onerror = d.onload = null, clearTimeout(s);
+                    o.onerror = o.onload = null, clearTimeout(s);
                     var n = t[e];
-                    if (delete t[e], d.parentNode && d.parentNode.removeChild(d), n && n.forEach((e => e(a))), r) return r(a)
+                    if (delete t[e], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
-                    target: d
+                    target: o
                 }), 12e4);
-            d.onerror = c.bind(null, d.onerror), d.onload = c.bind(null, d.onload), f && document.head.appendChild(d)
+            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), f && document.head.appendChild(o)
         }
     }, k.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -171,27 +171,27 @@
             r = {};
         k.I = (t, a) => {
             a || (a = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
                 if (a.push(n), e[t]) return e[t];
                 k.o(k.S, t) || (k.S[t] = {});
-                var o = k.S[t],
-                    d = "@jupytercad/jupytercad-extension",
+                var d = k.S[t],
+                    o = "@jupytercad/jupytercad-extension",
                     f = (e, r, t, a) => {
-                        var n = o[e] = o[e] || {},
+                        var n = d[e] = d[e] || {},
                             f = n[r];
-                        (!f || !f.loaded && (!a != !f.eager ? a : d > f.from)) && (n[r] = {
+                        (!f || !f.loaded && (!a != !f.eager ? a : o > f.from)) && (n[r] = {
                             get: t,
-                            from: d,
+                            from: o,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(277), k.e(792), k.e(995)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([k.e(78), k.e(711), k.e(277), k.e(930), k.e(726)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.1.0-beta.0", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(277), k.e(930), k.e(726), k.e(995), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.23", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("@deathbeds/jupyterlab-rjsf", "1.1.0", (() => Promise.all([k.e(184), k.e(29), k.e(277), k.e(792), k.e(995)]).then((() => () => k(46184))))), f("@jupyter/docprovider", "1.0.0-alpha.8", (() => Promise.all([k.e(78), k.e(711), k.e(277), k.e(930), k.e(726)]).then((() => () => k(44711))))), f("@jupytercad/jupytercad-extension", "0.1.0-rc.0", (() => Promise.all([k.e(651), k.e(78), k.e(963), k.e(29), k.e(277), k.e(930), k.e(726), k.e(995), k.e(544)]).then((() => () => k(38790))))), f("@naisutech/react-tree", "3.1.0", (() => Promise.all([k.e(733), k.e(29), k.e(778), k.e(406)]).then((() => () => k(74733))))), f("@rjsf/core", "3.2.1", (() => Promise.all([k.e(651), k.e(842), k.e(29)]).then((() => () => k(28842))))), f("d3-color", "3.1.0", (() => k.e(52).then((() => () => k(37052))))), f("styled-components", "5.3.10", (() => Promise.all([k.e(761), k.e(29), k.e(816)]).then((() => () => k(69761))))), f("three-mesh-bvh", "0.5.23", (() => Promise.all([k.e(422), k.e(391)]).then((() => () => k(31422))))), f("three", "0.135.0", (() => k.e(955).then((() => () => k(12955))))), f("uuid", "8.3.2", (() => k.e(712).then((() => () => k(67712)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         k.g.importScripts && (e = k.g.location + "");
         var r = k.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -202,110 +202,110 @@
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
     })(), n = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             a = t[1] ? r(t[1]) : [];
         return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
-    }, o = (e, r) => {
+    }, d = (e, r) => {
         e = n(e), r = n(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
-                o = (typeof a)[0];
-            if (t >= r.length) return "u" == o;
-            var d = r[t],
-                f = (typeof d)[0];
-            if (o != f) return "o" == o && "n" == f || "s" == f || "u" == o;
-            if ("o" != o && "u" != o && a != d) return a < d;
+                d = (typeof a)[0];
+            if (t >= r.length) return "u" == d;
+            var o = r[t],
+                f = (typeof o)[0];
+            if (d != f) return "o" == d && "n" == f || "s" == f || "u" == d;
+            if ("o" != d && "u" != d && a != o) return a < o;
             t++
         }
-    }, d = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, n = 1; n < e.length; n++) a--, t += "u" == (typeof(f = e[n]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, f);
             return t
         }
-        var o = [];
+        var d = [];
         for (n = 1; n < e.length; n++) {
             var f = e[n];
-            o.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? o.pop() + " " + o.pop() : d(f))
+            d.push(0 === f ? "not(" + l() + ")" : 1 === f ? "(" + l() + " || " + l() + ")" : 2 === f ? d.pop() + " " + d.pop() : o(f))
         }
         return l();
 
         function l() {
-            return o.pop().replace(/^\((.+)\)$/, "$1")
+            return d.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, f = (e, r) => {
         if (0 in e) {
             r = n(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, i, c = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (i = (typeof(u = r[o]))[0])) return !l || ("u" == c ? d > t && !a : "" == c != a);
+            for (var d = 0, o = 1, l = !0;; o++, d++) {
+                var u, i, c = o < e.length ? (typeof e[o])[0] : "";
+                if (d >= r.length || "o" == (i = (typeof(u = r[d]))[0])) return !l || ("u" == c ? o > t && !a : "" == c != a);
                 if ("u" == i) {
                     if (!l || "u" != c) return !1
                 } else if (l)
                     if (c == i)
-                        if (d <= t) {
-                            if (u != e[d]) return !1
+                        if (o <= t) {
+                            if (u != e[o]) return !1
                         } else {
-                            if (a ? u > e[d] : u < e[d]) return !1;
-                            u != e[d] && (l = !1)
+                            if (a ? u > e[o] : u < e[o]) return !1;
+                            u != e[o] && (l = !1)
                         }
                 else if ("s" != c && "n" != c) {
-                    if (a || d <= t) return !1;
-                    l = !1, d--
+                    if (a || o <= t) return !1;
+                    l = !1, o--
                 } else {
-                    if (d <= t || i < c != a) return !1;
+                    if (o <= t || i < c != a) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, d--)
+                } else "s" != c && "n" != c && (l = !1, o--)
             }
         }
         var s = [],
             b = s.pop.bind(s);
-        for (o = 1; o < e.length; o++) {
-            var p = e[o];
+        for (d = 1; d < e.length; d++) {
+            var p = e[d];
             s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? f(p, r) : !b())
         }
         return !!b()
     }, l = (e, r) => {
         var t = k.S[e];
         if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
-        return (r = Object.keys(t).reduce(((e, r) => !e || o(e, r) ? r : e), 0)) && t[r]
+        return (r = Object.keys(t).reduce(((e, r) => !e || d(e, r) ? r : e), 0)) && t[r]
     }, i = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + d(a) + ")", s = (e, r, t, a) => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && d(e, r) ? r : e), 0)
+    }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(a) + ")", s = (e, r, t, a) => {
         var n = i(e, t);
         return f(a, n) || h(c(e, t, n, a)), v(e[t][n])
     }, b = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !o(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !f(t, r) || e && !d(e, r) ? e : r), 0)) && a[r]
     }, p = (e, r, t, a) => {
         var n = e[t];
-        return "No satisfying version (" + d(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
+        return "No satisfying version (" + o(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(n).map((e => e + " from " + n[e].from)).join(", ")
     }, h = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         h(p(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), j = (y = e => function(r, t, a, n) {
-        var o = k.I(r);
-        return o && o.then ? o.then(e.bind(e, r, k.S[r], t, a, n)) : e(r, k.S[r], t, a, n)
+        var d = k.I(r);
+        return d && d.then ? d.then(e.bind(e, r, k.S[r], t, a, n)) : e(r, k.S[r], t, a, n)
     })(((e, r, t, a) => r && k.o(r, t) ? v(u(r, t)) : a())), g = y(((e, r, t, a) => (l(e, t), v(b(r, t, a) || m(r, e, t, a) || u(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, n) => {
-        var o = r && k.o(r, t) && b(r, t, a);
-        return o ? v(o) : n()
+        var d = r && k.o(r, t) && b(r, t, a);
+        return d ? v(d) : n()
     })), _ = {}, x = {
         66029: () => P("default", "react", [1, 18, 2, 0]),
         68501: () => P("default", "@jupyterlab/apputils", [1, 4, 0, 0]),
         69406: () => P("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
         74901: () => P("default", "@lumino/signaling", [1, 2, 0, 0]),
         97930: () => P("default", "@lumino/coreutils", [1, 2, 0, 0]),
         43067: () => P("default", "@jupyterlab/services", [1, 7, 0, 0]),
@@ -376,33 +376,33 @@
             var a = k.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
                 else if (/^(7(26|78|92)|277|29|391|930|995)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
-                var o = k.p + k.u(r),
-                    d = new Error;
-                k.l(o, (t => {
+                var d = k.p + k.u(r),
+                    o = new Error;
+                k.l(d, (t => {
                     if (k.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        d.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", d.name = "ChunkLoadError", d.type = n, d.request = o, a[1](d)
+                            d = t && t.target && t.target.src;
+                        o.message = "Loading chunk " + r + " failed.\n(" + n + ": " + d + ")", o.name = "ChunkLoadError", o.type = n, o.request = d, a[1](o)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, n, [o, d, f] = t,
+                var a, n, [d, o, f] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
-                    for (a in d) k.o(d, a) && (k.m[a] = d[a]);
+                if (d.some((r => 0 !== e[r]))) {
+                    for (a in o) k.o(o, a) && (k.m[a] = o[a]);
                     f && f(k)
                 }
-                for (r && r(t); l < o.length; l++) n = o[l], k.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); l < d.length; l++) n = d[l], k.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_jupytercad_jupytercad_extension = self.webpackChunk_jupytercad_jupytercad_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), k.nc = void 0;
     var T = k(8634);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupytercad/jupytercad-extension"] = T
 })();
```

### Comparing `jupytercad-0.1.0b0/jupytercad/labextension/static/third-party-licenses.json` & `jupytercad-0.1.0rc0/jupytercad/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/notebook/cad_document.py` & `jupytercad-0.1.0rc0/jupytercad/notebook/cad_document.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/notebook/y_connector.py` & `jupytercad-0.1.0rc0/jupytercad/notebook/y_connector.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/jupytercad/notebook/objects/__init__.py` & `jupytercad-0.1.0rc0/jupytercad/notebook/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/scripts/bump-version.py` & `jupytercad-0.1.0rc0/scripts/bump-version.py`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/package.json` & `jupytercad-0.1.0rc0/packages/jupytercad-app/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0-rc.0'"}*

```diff
@@ -76,9 +76,9 @@
         "watch:webpack": "webpack --watch"
     },
     "sideEffects": [
         "style/**/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.1.0-beta.0"
+    "version": "0.1.0-rc.0"
 }
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/tsconfig.tsbuildinfo` & `jupytercad-0.1.0rc0/packages/jupytercad-app/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/webpack.config.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/build/main.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/build/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/build/style.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/build/style.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/build/app/app.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/build/app/app.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/build/app/plugins/browser/index.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/build/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/lib/main.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/lib/main.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/app.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/app.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/app.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/app.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/lib/app/plugins/browser/index.js` & `jupytercad-0.1.0rc0/packages/jupytercad-app/lib/app/plugins/browser/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/src/main.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/src/main.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/src/app/app.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/app.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/browser/index.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/browser/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-app/src/app/plugins/mainmenu/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-app/style/base.css` & `jupytercad-0.1.0rc0/packages/jupytercad-app/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/extension.webpack.config.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/extension.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/package.json` & `jupytercad-0.1.0rc0/jupytercad/labextension/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969621212121212%*

 * *Differences: {"'dependencies'": "{'@jupytercad/jupytercad-opencascade': '^0.1.1-rc.0'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.915ba599f76e726e9820.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.1.0-rc.0'"}*

```diff
@@ -7,15 +7,15 @@
     },
     "dependencies": {
         "@deathbeds/jupyterlab-rjsf": "^1.1.0",
         "@jupyter-widgets/base": "^6.0.2",
         "@jupyter/collaboration": "^1.0.0-alpha.7",
         "@jupyter/docprovider": "^1.0.0-alpha.8",
         "@jupyter/ydoc": "^0.3.4 || ^1.0.2",
-        "@jupytercad/jupytercad-opencascade": "^0.1.1-beta.0",
+        "@jupytercad/jupytercad-opencascade": "^0.1.1-rc.0",
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/apputils": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/docregistry": "^4.0.0",
         "@jupyterlab/filebrowser": "^4.0.0",
         "@jupyterlab/launcher": "^4.0.0",
         "@jupyterlab/mainmenu": "^4.0.0",
@@ -55,14 +55,19 @@
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/QuantStack/jupytercad",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.915ba599f76e726e9820.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "../../jupytercad/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             },
@@ -112,9 +117,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0-beta.0"
+    "version": "0.1.0-rc.0"
 }
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/schema.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/schema.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/tsconfig.tsbuildinfo` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/tsconfig.tsbuildinfo`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999728732638888%*

 * *Differences: {"'program'": "{'fileInfos': {insert: [(657, "*

 * *              "'804b1f55cc6092cbae7d61fd9eae3c8b8ecc49d4839ed508c4ed6977430c487e')], delete: "*

 * *              '[657]}}'}*

```diff
@@ -11784,15 +11784,15 @@
                 "signature": "51d8b50b8eae2a8d0f63c6c2c46a8b04f0863c678f84052165a0001d41f328b7",
                 "version": "d6f912fda0708dae9a75ebb954225509fe5ca7362734f2a5bd31c03a6eeec3ad"
             },
             {
                 "signature": "7b2d5be885bc8529df052b09cd46b2d783d292837815f61bbce6ea1c257c99bf",
                 "version": "2b3def2e55b1a604998b3d2b204ff5e64790974fcf9821564ec67222093337d4"
             },
-            "8c7176a89472fa1e07f221aa8ee0745e9ce6cf5632aa27e61b2de59e9de4289d",
+            "804b1f55cc6092cbae7d61fd9eae3c8b8ecc49d4839ed508c4ed6977430c487e",
             {
                 "signature": "5570335ff6452229406838ff2c0cf08a6736e1e1064d0c4c8dcef0dd0e490592",
                 "version": "07159ff2605484a663db7ce82f5d8b8be06633f4479b2fbbc9b8049f7d837009"
             },
             "9f3c5498245c38c9016a369795ec5ef1768d09db63643c8dba9656e5ab294825",
             "2d225e7bda2871c066a7079c88174340950fb604f624f2586d3ea27bb9e5f4ff",
             "6a785f84e63234035e511817dd48ada756d984dd8f9344e56eb8b2bdcd8fd001",
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/worker.webpack.config.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/worker.webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/commands.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/commands.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/commands.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/commands.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/factory.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/factory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/factory.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/factory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/formdialog.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/formdialog.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/formdialog.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/formdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/index.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/mainview.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/mainview.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/mainview.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/mainview.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/model.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/model.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/tools.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/tools.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/tools.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/tools.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/types.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/widget.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/widget.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/_interface/forms.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -233,35 +233,37 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cylinder": {
+    "Part::Cut": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle",
-            "Height",
+            "Base",
+            "Tool",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "Radius of the cylinder"
+            "Base": {
+                "type": "string",
+                "description": "The base of the cut operator",
+                "fcType": "App::PropertyLink"
             },
-            "Height": {
-                "type": "number",
-                "description": "Height of the cylinder"
+            "Tool": {
+                "type": "string",
+                "description": "The tool of the cut operator",
+                "fcType": "App::PropertyLink"
             },
-            "Angle": {
-                "type": "number",
-                "description": "Angle of the cylinder"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -287,37 +289,35 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cut": {
+    "Part::Cylinder": {
         "type": "object",
         "required": [
-            "Base",
-            "Tool",
-            "Refine",
+            "Radius",
+            "Angle",
+            "Height",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "The base of the cut operator",
-                "fcType": "App::PropertyLink"
+            "Radius": {
+                "type": "number",
+                "description": "Radius of the cylinder"
             },
-            "Tool": {
-                "type": "string",
-                "description": "The tool of the cut operator",
-                "fcType": "App::PropertyLink"
+            "Height": {
+                "type": "number",
+                "description": "Height of the cylinder"
             },
-            "Refine": {
-                "type": "boolean",
-                "description": "Refine shape"
+            "Angle": {
+                "type": "number",
+                "description": "Angle of the cylinder"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -343,34 +343,49 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
+    "Part::Extrusion": {
         "type": "object",
         "required": [
-            "Shapes",
-            "Refine",
+            "Base",
+            "Dir",
+            "LengthFwd",
+            "LengthRev",
+            "Solid",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Shapes": {
+            "Base": {
+                "type": "string",
+                "description": "Shape to extrude",
+                "fcType": "App::PropertyLink"
+            },
+            "Dir": {
                 "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
+                "description": "Direction of extrusion",
                 "items": {
-                    "type": "string"
+                    "type": "number"
                 }
             },
-            "Refine": {
+            "LengthFwd": {
+                "type": "number",
+                "description": "Length of extrusion along the direction"
+            },
+            "LengthRev": {
+                "type": "number",
+                "description": "Length of extrusion against the direction"
+            },
+            "Solid": {
                 "type": "boolean",
-                "description": "Refine shape"
+                "description": "If true, creating a solid"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -396,49 +411,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Extrusion": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
-            "Base",
-            "Dir",
-            "LengthFwd",
-            "LengthRev",
-            "Solid",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "Shape to extrude",
-                "fcType": "App::PropertyLink"
-            },
-            "Dir": {
+            "Shapes": {
                 "type": "array",
-                "description": "Direction of extrusion",
+                "description": "The shapes of the individual elements",
+                "fcType": "App::PropertyLinkList",
                 "items": {
-                    "type": "number"
+                    "type": "string"
                 }
             },
-            "LengthFwd": {
-                "type": "number",
-                "description": "Length of extrusion along the direction"
-            },
-            "LengthRev": {
-                "type": "number",
-                "description": "Length of extrusion against the direction"
-            },
-            "Solid": {
+            "Refine": {
                 "type": "boolean",
-                "description": "If true, creating a solid"
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/message.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/message.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/model.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/model.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/annotation/view.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/annotation/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/fcplugin/plugins.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/fcplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/modelfactory.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/jcadplugin/plugins.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/jcadplugin/plugins.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/index.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/index.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/model.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/token.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/view.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/view.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/view.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/widgetManager.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/notebookrenderer/yCommProvider.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/annotations.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/annotations.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/annotations.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/annotations.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/formbuilder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/formbuilder.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/formbuilder.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/leftpanel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/leftpanel.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/leftpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/model.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/model.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/model.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/model.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objectproperties.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objectproperties.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/objecttree.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/objecttree.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/panelview/rightpanel.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/panelview/rightpanel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/box.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cone.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cut.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/cylinder.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/extrusion.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/fuse.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/geomCircle.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/geomLineSegment.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/intersection.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/jcad.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/placement.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/sketch.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/sphere.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/schema/torus.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/helper.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/helper.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/helper.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/helper.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/panzoom.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/panzoom.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherdialog.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketchermodel.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketchermodel.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/sketcherwidget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/sketcher/types.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/sketcher/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/usertoolbaritem.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/widget.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/widget.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/toolbar/widget.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/toolbar/widget.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/actions.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/actions.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/actions.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/actions.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occapi.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occapi.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occapi.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occapi.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occparser.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occparser.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/occparser.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/occparser.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/types.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/types.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/worker.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/worker.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/lib/worker/geometry/geomCircle.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/commands.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/factory.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/formdialog.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/formdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/index.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/mainview.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/mainview.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/model.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/tools.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/tools.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/types.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/widget.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/box.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/box.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cone.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cone.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cut.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cut.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/cylinder.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/cylinder.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/extrusion.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/extrusion.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/forms.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/forms.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -233,35 +233,37 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cylinder": {
+    "Part::Cut": {
         "type": "object",
         "required": [
-            "Radius",
-            "Angle",
-            "Height",
+            "Base",
+            "Tool",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Radius": {
-                "type": "number",
-                "description": "Radius of the cylinder"
+            "Base": {
+                "type": "string",
+                "description": "The base of the cut operator",
+                "fcType": "App::PropertyLink"
             },
-            "Height": {
-                "type": "number",
-                "description": "Height of the cylinder"
+            "Tool": {
+                "type": "string",
+                "description": "The tool of the cut operator",
+                "fcType": "App::PropertyLink"
             },
-            "Angle": {
-                "type": "number",
-                "description": "Angle of the cylinder"
+            "Refine": {
+                "type": "boolean",
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -287,37 +289,35 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Cut": {
+    "Part::Cylinder": {
         "type": "object",
         "required": [
-            "Base",
-            "Tool",
-            "Refine",
+            "Radius",
+            "Angle",
+            "Height",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "The base of the cut operator",
-                "fcType": "App::PropertyLink"
+            "Radius": {
+                "type": "number",
+                "description": "Radius of the cylinder"
             },
-            "Tool": {
-                "type": "string",
-                "description": "The tool of the cut operator",
-                "fcType": "App::PropertyLink"
+            "Height": {
+                "type": "number",
+                "description": "Height of the cylinder"
             },
-            "Refine": {
-                "type": "boolean",
-                "description": "Refine shape"
+            "Angle": {
+                "type": "number",
+                "description": "Angle of the cylinder"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -343,34 +343,49 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::MultiFuse": {
+    "Part::Extrusion": {
         "type": "object",
         "required": [
-            "Shapes",
-            "Refine",
+            "Base",
+            "Dir",
+            "LengthFwd",
+            "LengthRev",
+            "Solid",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Shapes": {
+            "Base": {
+                "type": "string",
+                "description": "Shape to extrude",
+                "fcType": "App::PropertyLink"
+            },
+            "Dir": {
                 "type": "array",
-                "description": "The shapes of the individual elements",
-                "fcType": "App::PropertyLinkList",
+                "description": "Direction of extrusion",
                 "items": {
-                    "type": "string"
+                    "type": "number"
                 }
             },
-            "Refine": {
+            "LengthFwd": {
+                "type": "number",
+                "description": "Length of extrusion along the direction"
+            },
+            "LengthRev": {
+                "type": "number",
+                "description": "Length of extrusion against the direction"
+            },
+            "Solid": {
                 "type": "boolean",
-                "description": "Refine shape"
+                "description": "If true, creating a solid"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
@@ -396,49 +411,34 @@
                         "type": "number",
                         "description": "Angle of the Placement"
                     }
                 }
             }
         }
     },
-    "Part::Extrusion": {
+    "Part::MultiFuse": {
         "type": "object",
         "required": [
-            "Base",
-            "Dir",
-            "LengthFwd",
-            "LengthRev",
-            "Solid",
+            "Shapes",
+            "Refine",
             "Placement"
         ],
         "additionalProperties": false,
         "properties": {
-            "Base": {
-                "type": "string",
-                "description": "Shape to extrude",
-                "fcType": "App::PropertyLink"
-            },
-            "Dir": {
+            "Shapes": {
                 "type": "array",
-                "description": "Direction of extrusion",
+                "description": "The shapes of the individual elements",
+                "fcType": "App::PropertyLinkList",
                 "items": {
-                    "type": "number"
+                    "type": "string"
                 }
             },
-            "LengthFwd": {
-                "type": "number",
-                "description": "Length of extrusion along the direction"
-            },
-            "LengthRev": {
-                "type": "number",
-                "description": "Length of extrusion against the direction"
-            },
-            "Solid": {
+            "Refine": {
                 "type": "boolean",
-                "description": "If true, creating a solid"
+                "description": "Refine shape"
             },
             "Placement": {
                 "type": "object",
                 "description": "Placement of the box",
                 "additionalProperties": false,
                 "required": [
                     "Position",
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/fuse.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/fuse.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/geomCircle.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/geomLineSegment.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/intersection.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/intersection.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/jcad.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/jcad.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/sketch.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/sketch.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/sphere.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/sphere.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/_interface/torus.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/_interface/torus.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/message.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/message.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/model.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/annotation/view.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/annotation/view.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/fcplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/fcplugin/plugins.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/fcplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/jcadplugin/modelfactory.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/jcadplugin/plugins.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/jcadplugin/plugins.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/index.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/index.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/model.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/token.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/token.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/view.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/view.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/widgetManager.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/notebookrenderer/yCommProvider.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/annotations.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/annotations.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/formbuilder.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/formbuilder.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/leftpanel.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/leftpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/model.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/model.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/objectproperties.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/objectproperties.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/objecttree.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/objecttree.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/panelview/rightpanel.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/panelview/rightpanel.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/box.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/box.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cone.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cone.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cut.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cut.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/cylinder.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/cylinder.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/extrusion.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/extrusion.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/fuse.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/fuse.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/geomCircle.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/geomCircle.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/geomLineSegment.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/geomLineSegment.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/intersection.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/intersection.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/jcad.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/jcad.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/placement.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/placement.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/sketch.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/sketch.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/sphere.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/sphere.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/schema/torus.json` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/schema/torus.json`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/helper.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/helper.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/panzoom.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/panzoom.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketcherdialog.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketchermodel.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/sketcherwidget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/types.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/sketcher/elements/line.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/sketcher/elements/line.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/toolbar/usertoolbaritem.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/toolbar/widget.tsx` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/toolbar/widget.tsx`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/actions.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/actions.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/occapi.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/occapi.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/occparser.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/occparser.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/types.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/types.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/worker.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/worker.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/src/worker/geometry/geomCircle.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/base.css` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/base.css`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/axes.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/axes.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/box.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/box.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cone.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cone.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cut.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cut.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/cylinder.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/cylinder.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/extrusion.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/extrusion.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/intersection.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/intersection.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/jvcontrol.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/jvcontrol.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/sphere.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/sphere.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/torus.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/torus.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/union.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/union.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/visibility.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/visibility.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-extension/style/icon/visibilityOff.svg` & `jupytercad-0.1.0rc0/packages/jupytercad-extension/style/icon/visibilityOff.svg`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/build.yml` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/build_opencascade.js` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/build_opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/package.json` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.1.1-rc.0'"}*

```diff
@@ -33,9 +33,9 @@
     "scripts": {
         "build": "node build_opencascade.js",
         "build:prod": "node build_opencascade.js",
         "clean": "rimraf ./lib",
         "clean:all": "rimraf ./lib"
     },
     "types": "lib/jupytercad.opencascade.d.ts",
-    "version": "0.1.1-beta.0"
+    "version": "0.1.1-rc.0"
 }
```

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/build.yml` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/build.yml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.d.ts`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.js`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm` & `jupytercad-0.1.0rc0/packages/jupytercad-opencascade/lib/jupytercad.opencascade.wasm`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/.gitignore` & `jupytercad-0.1.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/LICENSE` & `jupytercad-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/README.md` & `jupytercad-0.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/pyproject.toml` & `jupytercad-0.1.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupytercad-0.1.0b0/PKG-INFO` & `jupytercad-0.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupytercad
-Version: 0.1.0b0
+Version: 0.1.0rc0
 Summary: A JupyterLab extension for 3D modelling.
 Project-URL: Homepage, https://github.com/QuantStack/jupytercad
 Project-URL: Bug Tracker, https://github.com/QuantStack/jupytercad/issues
 Project-URL: Repository, https://github.com/QuantStack/jupytercad.git
 Author: JupyterCad contributors
 License: BSD 3-Clause License
```

