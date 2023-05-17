# Comparing `tmp/InvokeAI-2.3.5.post1.tar.gz` & `tmp/InvokeAI-2.3.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InvokeAI-2.3.5.post1.tar", last modified: Wed May 17 03:45:44 2023, max compression
+gzip compressed data, was "InvokeAI-2.3.5rc1.tar", last modified: Wed Apr 26 22:54:24 2023, max compression
```

## Comparing `InvokeAI-2.3.5.post1.tar` & `InvokeAI-2.3.5rc1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.656922 InvokeAI-2.3.5.post1/InvokeAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 03:45:44.000000 InvokeAI-2.3.5.post1/InvokeAI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 03:45:32.000000 InvokeAI-2.3.5.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13897 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-17 03:45:32.000000 InvokeAI-2.3.5.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.648922 InvokeAI-2.3.5.post1/invokeai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.648921 InvokeAI-2.3.5.post1/invokeai/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.656922 InvokeAI-2.3.5.post1/invokeai/assets/web/
--rw-r--r--   0 runner    (1001) docker     (123)    34023 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/assets/web/caution.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.656922 InvokeAI-2.3.5.post1/invokeai/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70498 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/invoke_ai_web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.656922 InvokeAI-2.3.5.post1/invokeai/backend/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/modules/create_cmd_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/modules/get_canvas_generation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/modules/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/backend/modules/parse_seed_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.656922 InvokeAI-2.3.5.post1/invokeai/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/INITIAL_MODELS.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/models.yaml.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.660922 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-finetune.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-finetune_style.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-m1-finetune.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v2-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.648922 InvokeAI-2.3.5.post1/invokeai/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.660922 InvokeAI-2.3.5.post1/invokeai/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.664922 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   316100 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/Inter-Bold-790c108b.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   803384 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/Inter-b9a8e5e2.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118734 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/favicon-0d253ced.ico
--rw-r--r--   0 runner    (1001) docker     (123)    51474 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/index-2ab0eb58.css
--rw-r--r--   0 runner    (1001) docker     (123)  1549115 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/index-b12e648e.js
--rw-r--r--   0 runner    (1001) docker     (123)    44115 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/logo-13003d72.png
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.664922 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/
--rw-r--r--   0 runner    (1001) docker     (123)    31098 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ar.json
--rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/de.json
--rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/en.json
--rw-r--r--   0 runner    (1001) docker     (123)    31063 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/es.json
--rw-r--r--   0 runner    (1001) docker     (123)    27064 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/fr.json
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/it.json
--rw-r--r--   0 runner    (1001) docker     (123)    22216 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ja.json
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/nl.json
--rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/pl.json
--rw-r--r--   0 runner    (1001) docker     (123)    25471 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/pt_BR.json
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ro.json
--rw-r--r--   0 runner    (1001) docker     (123)    33418 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ru.json
--rw-r--r--   0 runner    (1001) docker     (123)    33231 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/uk.json
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/zh_CN.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.668922 InvokeAI-2.3.5.post1/ldm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.668922 InvokeAI-2.3.5.post1/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/lsun.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/personalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/data/personalized_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    54889 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.672922 InvokeAI-2.3.5.post1/ldm/invoke/
--rw-r--r--   0 runner    (1001) docker     (123)    48344 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/CLI.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    51811 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    50246 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/ckpt_to_diffuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/concepts_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.672922 InvokeAI-2.3.5.post1/ldm/invoke/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29449 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/invokeai_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/invokeai_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/model_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/model_install_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/config/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/devices.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16832 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/dynamic_prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.676922 InvokeAI-2.3.5.post1/ldm/invoke/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    37307 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/diffusers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/embiggen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/omnibus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/generator/txt2img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/image_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/invokeai_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/merge_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    49832 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/offloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/patchmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/pngwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/readline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.676922 InvokeAI-2.3.5.post1/ldm/invoke/restoration/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/codeformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/outcrop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/restoration/vqgan_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/seamless.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/server_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.676922 InvokeAI-2.3.5.post1/ldm/invoke/training/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15779 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/training/textual_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35879 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/training/textual_inversion_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/invoke/txt2mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.676922 InvokeAI-2.3.5.post1/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.680923 InvokeAI-2.3.5.post1/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    28998 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/cross_attention_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/cross_attention_map_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    81805 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/ddpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/ksampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/models/diffusion/shared_invokeai_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.680923 InvokeAI-2.3.5.post1/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.680923 InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35512 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36213 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/embedding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/encoders/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/image_degradation/bsrgan_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    30058 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/image_degradation/utils_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/kohya_lora_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/lora_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/ldm/modules/losses/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/losses/contperceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/losses/vqperceptual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/peft_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18736 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/textual_inversion_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/modules/x_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/simplet2i.py
--rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 03:45:44.684923 InvokeAI-2.3.5.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-05-17 03:45:33.000000 InvokeAI-2.3.5.post1/tests/test_textual_inversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/InvokeAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 22:54:24.000000 InvokeAI-2.3.5rc1/InvokeAI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 22:54:09.000000 InvokeAI-2.3.5rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-26 22:54:09.000000 InvokeAI-2.3.5rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.202708 InvokeAI-2.3.5rc1/invokeai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.202708 InvokeAI-2.3.5rc1/invokeai/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/assets/web/
+-rw-r--r--   0 runner    (1001) docker     (123)    34023 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/assets/web/caution.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70512 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/invoke_ai_web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/backend/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/modules/create_cmd_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/modules/get_canvas_generation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/modules/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/backend/modules/parse_seed_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/INITIAL_MODELS.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/models.yaml.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-finetune.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-finetune_style.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-m1-finetune.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v2-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.202708 InvokeAI-2.3.5rc1/invokeai/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.206709 InvokeAI-2.3.5rc1/invokeai/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.210708 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   316100 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/Inter-Bold-790c108b.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   803384 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/Inter-b9a8e5e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118734 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/favicon-0d253ced.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    51474 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/index-2ab0eb58.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1549115 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/index-b12e648e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44115 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/logo-13003d72.png
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.214709 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)    31098 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ar.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27978 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31063 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27064 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22216 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/nl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22222 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/pl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25471 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/pt_BR.json
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ro.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33418 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33231 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/uk.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.214709 InvokeAI-2.3.5rc1/ldm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.214709 InvokeAI-2.3.5rc1/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/lsun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/personalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/data/personalized_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54627 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.218709 InvokeAI-2.3.5rc1/ldm/invoke/
+-rw-r--r--   0 runner    (1001) docker     (123)    48345 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51811 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50246 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/ckpt_to_diffuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/concepts_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.218709 InvokeAI-2.3.5rc1/ldm/invoke/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29449 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/invokeai_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/invokeai_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/model_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/model_install_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/config/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/devices.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16832 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/dynamic_prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.222709 InvokeAI-2.3.5rc1/ldm/invoke/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15960 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37104 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/diffusers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26074 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/embiggen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/omnibus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/generator/txt2img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/image_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      873 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/invokeai_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/merge_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49842 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/offloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/patchmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/pngwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/readline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.222709 InvokeAI-2.3.5rc1/ldm/invoke/restoration/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/codeformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/outcrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/restoration/vqgan_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/seamless.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/server_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.222709 InvokeAI-2.3.5rc1/ldm/invoke/training/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15779 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/training/textual_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35879 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/training/textual_inversion_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/invoke/txt2mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.222709 InvokeAI-2.3.5rc1/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.222709 InvokeAI-2.3.5rc1/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29061 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/cross_attention_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/cross_attention_map_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81805 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/ddpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/ksampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25852 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/models/diffusion/shared_invokeai_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35512 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36213 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/embedding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/encoders/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23359 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30058 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/image_degradation/utils_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/kohya_lora_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/lora_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/ldm/modules/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/losses/contperceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/losses/vqperceptual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/peft_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/textual_inversion_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/modules/x_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/simplet2i.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11287 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 22:54:24.226709 InvokeAI-2.3.5rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-04-26 22:54:10.000000 InvokeAI-2.3.5rc1/tests/test_textual_inversion.py
```

### Comparing `InvokeAI-2.3.5.post1/InvokeAI.egg-info/PKG-INFO` & `InvokeAI-2.3.5rc1/InvokeAI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvokeAI
-Version: 2.3.5.post1
+Version: 2.3.5rc1
 Summary: An implementation of Stable Diffusion which provides various new features and options to aid the image generation process
 Author-email: The InvokeAI Project <lincoln.stein@gmail.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/invoke-ai/InvokeAI/issues
 Project-URL: Discord, https://discord.gg/ZmtBAhwWhy
 Project-URL: Documentation, https://invoke-ai.github.io/InvokeAI/
 Project-URL: Homepage, https://invoke-ai.github.io/InvokeAI/
```

### Comparing `InvokeAI-2.3.5.post1/InvokeAI.egg-info/SOURCES.txt` & `InvokeAI-2.3.5rc1/InvokeAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/InvokeAI.egg-info/entry_points.txt` & `InvokeAI-2.3.5rc1/InvokeAI.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/InvokeAI.egg-info/requires.txt` & `InvokeAI-2.3.5rc1/InvokeAI.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 accelerate~=0.16
 albumentations
 click
 clip_anytorch
-compel~=1.1.5
+compel~=1.1.0
 datasets
-diffusers[torch]~=0.16.1
+diffusers[torch]==0.14
 dnspython==2.2.1
 einops
 eventlet
 facexlib
 fastapi==0.85.0
 fastapi-events==0.6.0
 fastapi-socketio==0.0.9
@@ -42,15 +42,15 @@
 safetensors~=0.3.0
 scikit-image>=0.19
 send2trash
 streamlit
 taming-transformers-rom1504
 test-tube>=0.7.5
 torch-fidelity
-torch~=2.0.0
+torch~=1.13.1
 torchmetrics
 torchvision>=0.14.1
 transformers~=4.26
 
 [:sys_platform == "win32"]
 windows-curses
 
@@ -75,11 +75,11 @@
 [test]
 pytest-cov
 pytest>6.0.0
 
 [xformers]
 
 [xformers:sys_platform != "darwin"]
-xformers~=0.0.19
+xformers~=0.0.16
 
 [xformers:sys_platform == "linux"]
 triton
```

### Comparing `InvokeAI-2.3.5.post1/LICENSE` & `InvokeAI-2.3.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/PKG-INFO` & `InvokeAI-2.3.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InvokeAI
-Version: 2.3.5.post1
+Version: 2.3.5rc1
 Summary: An implementation of Stable Diffusion which provides various new features and options to aid the image generation process
 Author-email: The InvokeAI Project <lincoln.stein@gmail.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/invoke-ai/InvokeAI/issues
 Project-URL: Discord, https://discord.gg/ZmtBAhwWhy
 Project-URL: Documentation, https://invoke-ai.github.io/InvokeAI/
 Project-URL: Homepage, https://invoke-ai.github.io/InvokeAI/
```

### Comparing `InvokeAI-2.3.5.post1/README.md` & `InvokeAI-2.3.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/assets/web/caution.png` & `InvokeAI-2.3.5rc1/invokeai/assets/web/caution.png`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/backend/invoke_ai_web_server.py` & `InvokeAI-2.3.5rc1/invokeai/backend/invoke_ai_web_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from invokeai.backend.modules.get_canvas_generation_mode import (
     get_canvas_generation_mode,
 )
 from invokeai.backend.modules.parameters import parameters_to_command
 import invokeai.frontend.dist as frontend
 from ldm.generate import Generate
 from ldm.invoke.args import Args, APP_ID, APP_VERSION, calculate_init_img_hash
-from ldm.invoke.concepts_lib import get_hf_concepts_lib
+from ldm.invoke.concepts_lib import HuggingFaceConceptsLibrary
 from ldm.invoke.conditioning import (
     get_tokens_for_prompt_object,
     get_prompt_structure,
     split_weighted_subprompts,
 )
 from ldm.invoke.generator.diffusers_pipeline import PipelineIntermediateState
 from ldm.invoke.generator.inpaint import infill_methods
@@ -534,15 +534,15 @@
                 self.handle_exceptions(e)
 
         @socketio.on("getTextualInversionTriggers")
         def get_ti_triggers():
             try:
                 local_triggers = self.generate.model.textual_inversion_manager.get_all_trigger_strings()
                 locals = [{'name': x} for x in sorted(local_triggers, key=str.casefold)]
-                concepts = get_hf_concepts_lib().list_concepts(minimum_likes=5)
+                concepts = HuggingFaceConceptsLibrary().list_concepts(minimum_likes=5)
                 concepts = [{'name': f'<{x}>'} for x in sorted(concepts, key=str.casefold) if f'<{x}>' not in local_triggers]
                 socketio.emit("foundTextualInversionTriggers", {'local_triggers': locals, 'huggingface_concepts': concepts})
             except Exception as e:
                 self.handle_exceptions(e)
 
         @socketio.on("requestEmptyTempFolder")
         def empty_temp_folder():
```

### Comparing `InvokeAI-2.3.5.post1/invokeai/backend/modules/create_cmd_parser.py` & `InvokeAI-2.3.5rc1/invokeai/backend/modules/create_cmd_parser.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/backend/modules/get_canvas_generation_mode.py` & `InvokeAI-2.3.5rc1/invokeai/backend/modules/get_canvas_generation_mode.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/backend/modules/parameters.py` & `InvokeAI-2.3.5rc1/invokeai/backend/modules/parameters.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/backend/modules/parse_seed_weights.py` & `InvokeAI-2.3.5rc1/invokeai/backend/modules/parse_seed_weights.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/INITIAL_MODELS.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/INITIAL_MODELS.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/models.yaml.example` & `InvokeAI-2.3.5rc1/invokeai/configs/models.yaml.example`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-finetune.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-finetune.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-finetune_style.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-finetune_style.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-inference.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-inpainting-inference.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v1-m1-finetune.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v1-m1-finetune.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v2-inference-v.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/configs/stable-diffusion/v2-inference.yaml` & `InvokeAI-2.3.5rc1/invokeai/configs/stable-diffusion/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/Inter-Bold-790c108b.ttf` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/Inter-Bold-790c108b.ttf`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/Inter-b9a8e5e2.ttf` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/Inter-b9a8e5e2.ttf`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/favicon-0d253ced.ico` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/favicon-0d253ced.ico`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/index-2ab0eb58.css` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/index-2ab0eb58.css`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/index-b12e648e.js` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/index-b12e648e.js`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/assets/logo-13003d72.png` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/assets/logo-13003d72.png`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ar.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ar.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/de.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/de.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/en.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/en.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/es.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/es.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/fr.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/fr.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/it.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/it.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ja.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ja.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/nl.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/nl.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/pl.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/pl.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/pt_BR.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/pt_BR.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/ru.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/ru.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/uk.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/uk.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/invokeai/frontend/dist/locales/zh_CN.json` & `InvokeAI-2.3.5rc1/invokeai/frontend/dist/locales/zh_CN.json`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/data/base.py` & `InvokeAI-2.3.5rc1/ldm/data/base.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/data/imagenet.py` & `InvokeAI-2.3.5rc1/ldm/data/imagenet.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/data/lsun.py` & `InvokeAI-2.3.5rc1/ldm/data/lsun.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/data/personalized.py` & `InvokeAI-2.3.5rc1/ldm/data/personalized.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/data/personalized_style.py` & `InvokeAI-2.3.5rc1/ldm/data/personalized_style.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/generate.py` & `InvokeAI-2.3.5rc1/ldm/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,19 @@
 import random
 import re
 import sys
 import time
 import traceback
 from typing import List
 
-import warnings
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=UserWarning)
-    import torch
-    
 import cv2
 import diffusers
 import numpy as np
 import skimage
-
+import torch
 import transformers
 from diffusers.pipeline_utils import DiffusionPipeline
 from diffusers.utils.import_utils import is_xformers_available
 from omegaconf import OmegaConf
 from pathlib import Path
 from PIL import Image, ImageOps
 from pytorch_lightning import logging, seed_everything
@@ -980,23 +975,21 @@
 
         # uncache generators so they pick up new models
         self.generators = {}
 
         seed_everything(random.randrange(0, np.iinfo(np.uint32).max))
         if self.embedding_path and not model_data.get("ti_embeddings_loaded"):
             print(f'>> Loading embeddings from {self.embedding_path}')
-            with warnings.catch_warnings():
-                warnings.filterwarnings("ignore", category=UserWarning)
-                for root, _, files in os.walk(self.embedding_path):
-                    for name in files:
-                        ti_path = os.path.join(root, name)
-                        self.model.textual_inversion_manager.load_textual_inversion(
-                            ti_path, defer_injecting_tokens=True
-                        )
-                model_data["ti_embeddings_loaded"] = True
+            for root, _, files in os.walk(self.embedding_path):
+                for name in files:
+                    ti_path = os.path.join(root, name)
+                    self.model.textual_inversion_manager.load_textual_inversion(
+                        ti_path, defer_injecting_tokens=True
+                    )
+            model_data["ti_embeddings_loaded"] = True
         print(
             f'>> Textual inversion triggers: {", ".join(sorted(self.model.textual_inversion_manager.get_all_trigger_strings()))}'
         )
 
         self.model_name = model_name
         self._set_sampler()  # requires self.model_name to be set first
         self._save_last_used_model(model_name)
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/CLI.py` & `InvokeAI-2.3.5rc1/ldm/invoke/CLI.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import traceback
 from argparse import Namespace
 from packaging import version
 from pathlib import Path
 from typing import Union
 
 import click
+
 from compel import PromptParser
 
 if sys.platform == "darwin":
     os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 import pyparsing  # type: ignore
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/args.py` & `InvokeAI-2.3.5rc1/ldm/invoke/args.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/ckpt_to_diffuser.py` & `InvokeAI-2.3.5rc1/ldm/invoke/ckpt_to_diffuser.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/concepts_lib.py` & `InvokeAI-2.3.5rc1/ldm/invoke/concepts_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 import re
 import traceback
 from typing import Callable
 from urllib import request, error as ul_error
 from huggingface_hub import HfFolder, hf_hub_url, ModelSearchArguments, ModelFilter, HfApi
 from ldm.invoke.globals import Globals
 
-singleton = None
-
-def get_hf_concepts_lib():
-    global singleton
-    if singleton is None:
-        singleton = HuggingFaceConceptsLibrary()
-    return singleton
-
 class HuggingFaceConceptsLibrary(object):
     def __init__(self, root=None):
         '''
         Initialize the Concepts object. May optionally pass a root directory.
         '''
         self.root = root or Globals.root
         self.hf_api = HfApi()
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/conditioning.py` & `InvokeAI-2.3.5rc1/ldm/invoke/conditioning.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/config/invokeai_configure.py` & `InvokeAI-2.3.5rc1/ldm/invoke/config/invokeai_configure.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/config/invokeai_update.py` & `InvokeAI-2.3.5rc1/ldm/invoke/config/invokeai_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     for p in psutil.process_iter():
         try:
             cmdline = p.cmdline()
             matches = [x for x in cmdline if x.endswith(('invokeai','invokeai.exe'))]
             if matches:
                 print(f':exclamation: [bold red]An InvokeAI instance appears to be running as process {p.pid}[/red bold]')
                 return True
-        except (psutil.AccessDenied,psutil.NoSuchProcess):
+        except psutil.AccessDenied:
             continue
     return False
         
     
 def welcome(versions: dict):
     
     @group()
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/config/model_install.py` & `InvokeAI-2.3.5rc1/ldm/invoke/config/model_install.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/config/model_install_backend.py` & `InvokeAI-2.3.5rc1/ldm/invoke/config/model_install_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     external_models = external_models or list()
     if scan_directory:
         external_models.append(str(scan_directory))
 
     if len(external_models)>0:
         print("== INSTALLING EXTERNAL MODELS ==")
         for path_url_or_repo in external_models:
+            print(f'DEBUG: path_url_or_repo = {path_url_or_repo}')
             try:
                 model_manager.heuristic_import(
                     path_url_or_repo,
                     config_file_callback=_pick_configuration_file,
                     commit_to_conf=config_file_path
                 )
             except KeyboardInterrupt:
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/config/widgets.py` & `InvokeAI-2.3.5rc1/ldm/invoke/config/widgets.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/devices.py` & `InvokeAI-2.3.5rc1/ldm/invoke/devices.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/dynamic_prompts.py` & `InvokeAI-2.3.5rc1/ldm/invoke/dynamic_prompts.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/base.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/base.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/diffusers_pipeline.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/diffusers_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,23 +396,16 @@
     @property
     def device(self) -> torch.device:
         return self._model_group.execution_device
 
     @property
     def _submodels(self) -> Sequence[torch.nn.Module]:
         module_names, _, _ = self.extract_init_dict(dict(self.config))
-        submodels = []
-        for name in module_names.keys():
-            if hasattr(self, name):
-                value = getattr(self, name)
-            else:
-                value = getattr(self.config, name)
-            if isinstance(value, torch.nn.Module):
-                submodels.append(value)
-        return submodels
+        values = [getattr(self, name) for name in module_names.keys()]
+        return [m for m in values if isinstance(m, torch.nn.Module)]
 
     def image_from_embeddings(self, latents: torch.Tensor, num_inference_steps: int,
                               conditioning_data: ConditioningData,
                               *,
                               noise: torch.Tensor,
                               callback: Callable[[PipelineIntermediateState], None]=None,
                               run_id=None) -> InvokeAIStableDiffusionPipelineOutput:
@@ -475,15 +468,15 @@
             additional_guidance = []
         extra_conditioning_info = conditioning_data.extra
         with InvokeAIDiffuserComponent.custom_attention_context(self.invokeai_diffuser.model,
                                                                 extra_conditioning_info=extra_conditioning_info,
                                                                 step_count=len(self.scheduler.timesteps)
                                                              ):
 
-            yield PipelineIntermediateState(run_id=run_id, step=-1, timestep=self.scheduler.config.num_train_timesteps,
+            yield PipelineIntermediateState(run_id=run_id, step=-1, timestep=self.scheduler.num_train_timesteps,
                                             latents=latents)
 
             batch_size = latents.shape[0]
             batched_t = torch.full((batch_size,), timesteps[0],
                                    dtype=timesteps.dtype, device=self._model_group.device_for(self.unet))
             latents = self.scheduler.add_noise(latents, noise, batched_t)
 
@@ -759,15 +752,15 @@
             truncation=True,
             return_tensors="pt",
         )
 
     @property
     def channels(self) -> int:
         """Compatible with DiffusionWrapper"""
-        return self.unet.config.in_channels
+        return self.unet.in_channels
 
     def decode_latents(self, latents):
         # Explicit call to get the vae loaded, since `decode` isn't the forward method.
         self._model_group.load(self.vae)
         return super().decode_latents(latents)
 
     def debug_latents(self, latents, msg):
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/embiggen.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/embiggen.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/img2img.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/img2img.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/inpaint.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/inpaint.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/omnibus.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/omnibus.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/txt2img.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/txt2img.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/generator/txt2img2img.py` & `InvokeAI-2.3.5rc1/ldm/invoke/generator/txt2img2img.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/globals.py` & `InvokeAI-2.3.5rc1/ldm/invoke/globals.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/image_util.py` & `InvokeAI-2.3.5rc1/ldm/invoke/image_util.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/invokeai_metadata.py` & `InvokeAI-2.3.5rc1/ldm/invoke/invokeai_metadata.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/log.py` & `InvokeAI-2.3.5rc1/ldm/invoke/log.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/merge_diffusers.py` & `InvokeAI-2.3.5rc1/ldm/invoke/merge_diffusers.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/model_manager.py` & `InvokeAI-2.3.5rc1/ldm/invoke/model_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
             try:
                 pipeline = StableDiffusionGeneratorPipeline.from_pretrained(
                     name_or_path,
                     **pipeline_args,
                     **fp_args,
                 )
             except OSError as e:
-                if 'Revision Not Found' in str(e):
+                if str(e).startswith("fp16 is not a valid"):
                     pass
                 else:
                     print(
                         f"** An unexpected error occurred while downloading the model: {e})"
                     )
             if pipeline:
                 break
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/offloading.py` & `InvokeAI-2.3.5rc1/ldm/invoke/offloading.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/patchmatch.py` & `InvokeAI-2.3.5rc1/ldm/invoke/patchmatch.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/pngwriter.py` & `InvokeAI-2.3.5rc1/ldm/invoke/pngwriter.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/readline.py` & `InvokeAI-2.3.5rc1/ldm/invoke/readline.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  completer.add_seed(9281839)
 """
 import os
 import re
 import atexit
 from typing import List
 from ldm.invoke.args import Args
-from ldm.invoke.concepts_lib import get_hf_concepts_lib
+from ldm.invoke.concepts_lib import HuggingFaceConceptsLibrary
 from ldm.invoke.globals import Globals
 from ldm.modules.lora_manager import LoraManager
 
 # ---------------readline utilities---------------------
 try:
     import readline
     readline_available = True
@@ -283,15 +283,15 @@
         self.embedding_terms = set(terms)
         if self.concepts:
             self.embedding_terms.update(set(self.concepts.list_concepts()))
 
     def _concept_completions(self, text, state):
         if self.concepts is None:
             # cache Concepts() instance so we can check for updates in concepts_list during runtime.
-            self.concepts = get_hf_concepts_lib()
+            self.concepts = HuggingFaceConceptsLibrary()
             self.embedding_terms.update(set(self.concepts.list_concepts()))
         else:
             self.embedding_terms.update(set(self.concepts.list_concepts()))
 
         partial = text[1:]  # this removes the leading '<'
         if len(partial) == 0:
             return list(self.embedding_terms)  # whole dump - think if user wants this!
```

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/base.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/base.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/codeformer.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/codeformer.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/codeformer_arch.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/codeformer_arch.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/gfpgan.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/gfpgan.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/outcrop.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/outcrop.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/outpaint.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/outpaint.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/realesrgan.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/realesrgan.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/restoration/vqgan_arch.py` & `InvokeAI-2.3.5rc1/ldm/invoke/restoration/vqgan_arch.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/seamless.py` & `InvokeAI-2.3.5rc1/ldm/invoke/seamless.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/server.py` & `InvokeAI-2.3.5rc1/ldm/invoke/server.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/server_legacy.py` & `InvokeAI-2.3.5rc1/ldm/invoke/server_legacy.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/training/textual_inversion.py` & `InvokeAI-2.3.5rc1/ldm/invoke/training/textual_inversion.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/training/textual_inversion_training.py` & `InvokeAI-2.3.5rc1/ldm/invoke/training/textual_inversion_training.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/invoke/txt2mask.py` & `InvokeAI-2.3.5rc1/ldm/invoke/txt2mask.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/lr_scheduler.py` & `InvokeAI-2.3.5rc1/ldm/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/autoencoder.py` & `InvokeAI-2.3.5rc1/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/classifier.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/classifier.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/cross_attention_control.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/cross_attention_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import psutil
 import torch
 import diffusers
 from torch import nn
 
 from compel.cross_attention_control import Arguments
 from diffusers.models.unet_2d_condition import UNet2DConditionModel
+from diffusers.models.cross_attention import AttnProcessor
 from ldm.invoke.devices import torch_dtype
 
 
 class CrossAttentionType(enum.Enum):
     SELF = 1
     TOKENS = 2
 
@@ -158,30 +159,30 @@
             for offset, slice in map_dict['slices'].items():
                 map_dict[offset] = slice.to('cpu')
 
 
 
 class InvokeAICrossAttentionMixin:
     """
-    Enable InvokeAI-flavoured Attention calculation, which does aggressive low-memory slicing and calls
+    Enable InvokeAI-flavoured CrossAttention calculation, which does aggressive low-memory slicing and calls
     through both to an attention_slice_wrangler and a slicing_strategy_getter for custom attention map wrangling
     and dymamic slicing strategy selection.
     """
     def __init__(self):
         self.mem_total_gb = psutil.virtual_memory().total // (1 << 30)
         self.attention_slice_wrangler = None
         self.slicing_strategy_getter = None
         self.attention_slice_calculated_callback = None
 
     def set_attention_slice_wrangler(self, wrangler: Optional[Callable[[nn.Module, torch.Tensor, int, int, int], torch.Tensor]]):
         '''
         Set custom attention calculator to be called when attention is calculated
         :param wrangler: Callback, with args (module, suggested_attention_slice, dim, offset, slice_size),
         which returns either the suggested_attention_slice or an adjusted equivalent.
-            `module` is the current Attention module for which the callback is being invoked.
+            `module` is the current CrossAttention module for which the callback is being invoked.
             `suggested_attention_slice` is the default-calculated attention slice
             `dim` is -1 if the attenion map has not been sliced, or 0 or 1 for dimension-0 or dimension-1 slicing.
                 If `dim` is >= 0, `offset` and `slice_size` specify the slice start and length.
 
         Pass None to use the default attention calculation.
         :return:
         '''
@@ -321,15 +322,15 @@
         # try to re-use an existing slice size
         default_slice_size = 4
         slice_size = next((p.slice_size for p in old_attn_processors.values() if type(p) is SlicedAttnProcessor), default_slice_size)
         unet.set_attn_processor(SlicedSwapCrossAttnProcesser(slice_size=slice_size))
 
 
 def get_cross_attention_modules(model, which: CrossAttentionType) -> list[tuple[str, InvokeAICrossAttentionMixin]]:
-    from ldm.modules.attention import CrossAttention # avoid circular import # TODO: rename as in diffusers?
+    from ldm.modules.attention import CrossAttention # avoid circular import
     cross_attention_class: type = InvokeAIDiffusersCrossAttention if isinstance(model,UNet2DConditionModel) else CrossAttention
     which_attn = "attn1" if which is CrossAttentionType.SELF else "attn2"
     attention_module_tuples = [(name,module) for name, module in model.named_modules() if
                 isinstance(module, cross_attention_class) and which_attn in name]
     cross_attention_modules_in_model_count = len(attention_module_tuples)
     expected_count = 16
     if cross_attention_modules_in_model_count != expected_count:
@@ -427,15 +428,15 @@
     mem_free_cuda, _ = torch.cuda.mem_get_info(device)
     mem_free_torch = mem_reserved - mem_active
     mem_free_total = mem_free_cuda + mem_free_torch
     return mem_free_total
 
 
 
-class InvokeAIDiffusersCrossAttention(diffusers.models.attention.Attention, InvokeAICrossAttentionMixin):
+class InvokeAIDiffusersCrossAttention(diffusers.models.attention.CrossAttention, InvokeAICrossAttentionMixin):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         InvokeAICrossAttentionMixin.__init__(self)
 
     def _attention(self, query, key, value, attention_mask=None):
         #default_result = super()._attention(query,  key, value)
@@ -452,16 +453,16 @@
 
 ## 🧨diffusers implementation follows
 
 
 """
 # base implementation
 
-class AttnProcessor:
-    def __call__(self, attn: Attention, hidden_states, encoder_hidden_states=None, attention_mask=None):
+class CrossAttnProcessor:
+    def __call__(self, attn: CrossAttention, hidden_states, encoder_hidden_states=None, attention_mask=None):
         batch_size, sequence_length, _ = hidden_states.shape
         attention_mask = attn.prepare_attention_mask(attention_mask, sequence_length)
 
         query = attn.to_q(hidden_states)
         query = attn.head_to_batch_dim(query)
 
         encoder_hidden_states = encoder_hidden_states if encoder_hidden_states is not None else hidden_states
@@ -482,15 +483,15 @@
         return hidden_states
 
 """
 from dataclasses import field, dataclass
 
 import torch
 
-from diffusers.models.attention_processor import Attention, AttnProcessor, SlicedAttnProcessor
+from diffusers.models.cross_attention import CrossAttention, CrossAttnProcessor, SlicedAttnProcessor
 
 
 @dataclass
 class SwapCrossAttnContext:
     modified_text_embeddings: torch.Tensor
     index_map: torch.Tensor # maps from original prompt token indices to the equivalent tokens in the modified prompt
     mask: torch.Tensor # in the target space of the index_map
@@ -527,15 +528,15 @@
         return mask, indices
 
 
 class SlicedSwapCrossAttnProcesser(SlicedAttnProcessor):
 
     # TODO: dynamically pick slice size based on memory conditions
 
-    def __call__(self, attn: Attention, hidden_states, encoder_hidden_states=None, attention_mask=None,
+    def __call__(self, attn: CrossAttention, hidden_states, encoder_hidden_states=None, attention_mask=None,
                  # kwargs
                  swap_cross_attn_context: SwapCrossAttnContext=None):
 
         attention_type = CrossAttentionType.SELF if encoder_hidden_states is None else CrossAttentionType.TOKENS
 
         # if cross-attention control is not in play, just call through to the base implementation.
         if attention_type is CrossAttentionType.SELF or \
```

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/cross_attention_map_saving.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/cross_attention_map_saving.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/ddim.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/ddpm.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/ksampler.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/ksampler.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/plms.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/sampler.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/models/diffusion/shared_invokeai_diffusion.py` & `InvokeAI-2.3.5rc1/ldm/models/diffusion/shared_invokeai_diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from contextlib import contextmanager
 from dataclasses import dataclass
 from math import ceil
 from typing import Callable, Optional, Union, Any
 
 import numpy as np
 import torch
+
 from diffusers import UNet2DConditionModel
 from typing_extensions import TypeAlias
 
 from ldm.invoke.globals import Globals
 from ldm.models.diffusion.cross_attention_control import (
     Arguments,
     setup_cross_attention_control_attention_processors,
```

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/attention.py` & `InvokeAI-2.3.5rc1/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/model.py` & `InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/openaimodel.py` & `InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/diffusionmodules/util.py` & `InvokeAI-2.3.5rc1/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/distributions/distributions.py` & `InvokeAI-2.3.5rc1/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/ema.py` & `InvokeAI-2.3.5rc1/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/embedding_manager.py` & `InvokeAI-2.3.5rc1/ldm/modules/embedding_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from cmath import log
 import torch
 from attr import dataclass
 from torch import nn
 
 import sys
 
-from ldm.invoke.concepts_lib import get_hf_concepts_lib
+from ldm.invoke.concepts_lib import HuggingFaceConceptsLibrary
 from ldm.data.personalized import per_img_token_list
 from transformers import CLIPTokenizer
 from functools import partial
 from picklescan.scanner import scan_file_path
 
 PROGRESSIVE_SCALE = 2000
 
@@ -35,15 +35,15 @@
         num_vectors_per_token=1,
         progressive_words=False,
         **kwargs,
     ):
         super().__init__()
 
         self.embedder = embedder
-        self.concepts_library=get_hf_concepts_lib()
+        self.concepts_library=HuggingFaceConceptsLibrary()
 
         self.string_to_token_dict = {}
         self.string_to_param_dict = nn.ParameterDict()
 
         self.initial_embeddings = (
             nn.ParameterDict()
         )   # These should not be optimized
```

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/encoders/modules.py` & `InvokeAI-2.3.5rc1/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/image_degradation/bsrgan.py` & `InvokeAI-2.3.5rc1/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/image_degradation/bsrgan_light.py` & `InvokeAI-2.3.5rc1/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/image_degradation/utils_image.py` & `InvokeAI-2.3.5rc1/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/kohya_lora_manager.py` & `InvokeAI-2.3.5rc1/ldm/modules/kohya_lora_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 from diffusers.models import UNet2DConditionModel
 from filelock import FileLock, Timeout
 from safetensors.torch import load_file
 from torch.utils.hooks import RemovableHandle
 from transformers import CLIPTextModel
 
-from ..invoke.globals import global_lora_models_dir, Globals
+from ..invoke.globals import global_lora_models_dir
 from ..invoke.devices import choose_torch_device
 
 """
 This module supports loading LoRA weights trained with https://github.com/kohya-ss/sd-scripts
 To be removed once support for diffusers LoRA weights is well supported
 """
 
@@ -452,33 +452,24 @@
                 )
                 return
 
             self.layers[stem] = layer
 
 
 class KohyaLoraManager:
+    lora_path = Path(global_lora_models_dir())
+    vector_length_cache_path = lora_path / '.vectorlength.cache'
     
     def __init__(self, pipe):
-        self.vector_length_cache_path = self.lora_path / '.vectorlength.cache'
         self.unet = pipe.unet
         self.wrapper = LoRAModuleWrapper(pipe.unet, pipe.text_encoder)
         self.text_encoder = pipe.text_encoder
         self.device = torch.device(choose_torch_device())
         self.dtype = pipe.unet.dtype
 
-    @classmethod
-    @property
-    def lora_path(cls)->Path:
-        return Path(global_lora_models_dir())
-
-    @classmethod
-    @property
-    def vector_length_cache_path(cls)->Path:
-        return cls.lora_path / '.vectorlength.cache'        
-
     def load_lora_module(self, name, path_file, multiplier: float = 1.0):
         print(f"   | Found lora {name} at {path_file}")
         if path_file.suffix == ".safetensors":
             checkpoint = load_file(path_file.absolute().as_posix(), device="cpu")
         else:
             checkpoint = torch.load(path_file, map_location="cpu")
```

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/lora_manager.py` & `InvokeAI-2.3.5rc1/ldm/modules/lora_manager.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/losses/contperceptual.py` & `InvokeAI-2.3.5rc1/ldm/modules/losses/contperceptual.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/losses/vqperceptual.py` & `InvokeAI-2.3.5rc1/ldm/modules/losses/vqperceptual.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/peft_manager.py` & `InvokeAI-2.3.5rc1/ldm/modules/peft_manager.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/textual_inversion_manager.py` & `InvokeAI-2.3.5rc1/ldm/modules/textual_inversion_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional, Union
 
-import warnings
-with warnings.catch_warnings():
-    warnings.filterwarnings("ignore", category=UserWarning)
-    import safetensors.torch
-    import torch
+import safetensors.torch
+import torch
 from picklescan.scanner import scan_file_path
 from transformers import CLIPTextModel, CLIPTokenizer
 
 from compel.embeddings_provider import BaseTextualInversionManager
-from ldm.invoke.concepts_lib import get_hf_concepts_lib
+from ldm.invoke.concepts_lib import HuggingFaceConceptsLibrary
+
 
 @dataclass
 class TextualInversion:
     trigger_string: str
     embedding: torch.Tensor
     trigger_token_id: Optional[int] = None
     pad_token_ids: Optional[list[int]] = None
@@ -32,15 +30,15 @@
         tokenizer: CLIPTokenizer,
         text_encoder: CLIPTextModel,
         full_precision: bool = True,
     ):
         self.tokenizer = tokenizer
         self.text_encoder = text_encoder
         self.full_precision = full_precision
-        self.hf_concepts_library = get_hf_concepts_lib()
+        self.hf_concepts_library = HuggingFaceConceptsLibrary()
         self.trigger_to_sourcefile = dict()
         default_textual_inversions: list[TextualInversion] = []
         self.textual_inversions = default_textual_inversions
 
     def load_huggingface_concepts(self, concepts: list[str]):
         for concept_name in concepts:
             if concept_name in self.hf_concepts_library.concepts_loaded:
```

### Comparing `InvokeAI-2.3.5.post1/ldm/modules/x_transformer.py` & `InvokeAI-2.3.5rc1/ldm/modules/x_transformer.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/ldm/util.py` & `InvokeAI-2.3.5rc1/ldm/util.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/pyproject.toml` & `InvokeAI-2.3.5rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,17 +28,17 @@
   "Topic :: Scientific/Engineering :: Image Processing",
 ]
 dependencies = [
   "accelerate~=0.16",
   "albumentations",
   "click",
   "clip_anytorch",
-  "compel~=1.1.5",
+  "compel~=1.1.0",
   "datasets",
-  "diffusers[torch]~=0.16.1",
+  "diffusers[torch]==0.14",
   "dnspython==2.2.1",
   "einops",
   "eventlet",
   "facexlib",
   "fastapi==0.85.0",
   "fastapi-events==0.6.0",
   "fastapi-socketio==0.0.9",
@@ -72,15 +72,15 @@
   "safetensors~=0.3.0",
   "scikit-image>=0.19",
   "send2trash",
   "streamlit",
   "taming-transformers-rom1504",
   "test-tube>=0.7.5",
   "torch-fidelity",
-  "torch~=2.0.0",
+  "torch~=1.13.1",
   "torchmetrics",
   "torchvision>=0.14.1",
   "transformers~=4.26",
   "windows-curses; sys_platform=='win32'",
 ]
 description = "An implementation of Stable Diffusion which provides various new features and options to aid the image generation process"
 dynamic = ["version"]
@@ -104,15 +104,15 @@
   "mkdocs-git-revision-date-localized-plugin",
   "mkdocs-material==9.*",
   "mkdocs-redirects==1.2.0",
 ]
 "test" = ["pytest-cov", "pytest>6.0.0"]
 "xformers" = [
   "triton; sys_platform=='linux'",
-  "xformers~=0.0.19; sys_platform!='darwin'",
+  "xformers~=0.0.16; sys_platform!='darwin'",
 ]
 
 [project.scripts]
 
 # legacy entrypoints; provided for backwards compatibility
 "configure_invokeai.py" = "ldm.invoke.config.invokeai_configure:main"
 "invoke.py" = "ldm.invoke.CLI:main"
```

### Comparing `InvokeAI-2.3.5.post1/tests/test_path.py` & `InvokeAI-2.3.5rc1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `InvokeAI-2.3.5.post1/tests/test_textual_inversion.py` & `InvokeAI-2.3.5rc1/tests/test_textual_inversion.py`

 * *Files identical despite different names*

