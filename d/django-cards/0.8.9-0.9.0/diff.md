# Comparing `tmp/django-cards-0.8.9.tar.gz` & `tmp/django-cards-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cards-0.8.9.tar", last modified: Thu Mar 16 15:08:48 2023, max compression
+gzip compressed data, was "django-cards-0.9.0.tar", last modified: Wed May 17 09:16:05 2023, max compression
```

## Comparing `django-cards-0.8.9.tar` & `django-cards-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.963661 django-cards-0.8.9/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.8.9/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.8.9/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-16 15:08:48.963506 django-cards-0.8.9/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.8.9/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.920722 django-cards-0.8.9/cards/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/apps.py
--rw-r--r--   0 tom        (501) staff       (20)    25744 2023-03-16 15:07:28.000000 django-cards-0.8.9/cards/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.922731 django-cards-0.8.9/cards/card_list/
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/base.py
--rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.8.9/cards/card_list/main.py
--rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/card_list/tree.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/includes.py
--rw-r--r--   0 tom        (501) staff       (20)     5204 2023-02-21 09:19:57.000000 django-cards-0.8.9/cards/standard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.912636 django-cards-0.8.9/cards/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.912796 django-cards-0.8.9/cards/static/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.914224 django-cards-0.8.9/cards/static/cards/jstree/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913134 django-cards-0.8.9/cards/static/cards/jstree/css/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913660 django-cards-0.8.9/cards/static/cards/jstree/css/themes/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.925265 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/
--rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.927591 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.css
--rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.930275 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/
--rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/30px.png
--rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/32px.png
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.913998 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.948120 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
--rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.955730 django-cards-0.8.9/cards/static/cards/jstree/js/
--rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/js/jstree.js
--rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/static/cards/jstree/js/jstree.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.914737 django-cards-0.8.9/cards/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.915494 django-cards-0.8.9/cards/templates/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.958148 django-cards-0.8.9/cards/templates/cards/groups/
--rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.8.9/cards/templates/cards/groups/groups.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.961840 django-cards-0.8.9/cards/templates/cards/standard/
--rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/blank.html
--rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/card_group.html
--rw-r--r--   0 tom        (501) staff       (20)      980 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/datatable.html
--rw-r--r--   0 tom        (501) staff       (20)      767 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/default.html
--rw-r--r--   0 tom        (501) staff       (20)     1528 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/default_body.html
--rw-r--r--   0 tom        (501) staff       (20)      917 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/html.html
--rw-r--r--   0 tom        (501) staff       (20)     2541 2023-02-20 15:01:01.000000 django-cards-0.8.9/cards/templates/cards/standard/list_selection.html
--rw-r--r--   0 tom        (501) staff       (20)      565 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/message.html
--rw-r--r--   0 tom        (501) staff       (20)      848 2023-01-26 20:53:02.000000 django-cards-0.8.9/cards/templates/cards/standard/table.html
--rw-r--r--   0 tom        (501) staff       (20)     1231 2023-03-14 15:05:03.000000 django-cards-0.8.9/cards/templates/cards/standard/table_body.html
--rw-r--r--   0 tom        (501) staff       (20)     2132 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templates/cards/standard/tree_selection.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.962333 django-cards-0.8.9/cards/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/templatetags/django_cards_tags.py
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.8.9/cards/url_converters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-16 15:08:48.963251 django-cards-0.8.9/django_cards.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3065 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-03-16 15:08:48.000000 django-cards-0.8.9/django_cards.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-16 15:08:48.963702 django-cards-0.8.9/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      645 2023-03-16 15:08:06.000000 django-cards-0.8.9/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.996986 django-cards-0.9.0/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.9.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.9.0/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-05-17 09:16:05.996742 django-cards-0.9.0/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.9.0/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.931190 django-cards-0.9.0/cards/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)    26056 2023-05-17 09:12:45.000000 django-cards-0.9.0/cards/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.933457 django-cards-0.9.0/cards/card_list/
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/card_list/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/card_list/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.9.0/cards/card_list/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/card_list/tree.py
+-rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/includes.py
+-rw-r--r--   0 tom        (501) staff       (20)     5204 2023-02-21 09:19:57.000000 django-cards-0.9.0/cards/standard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919009 django-cards-0.9.0/cards/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919092 django-cards-0.9.0/cards/static/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919969 django-cards-0.9.0/cards/static/cards/jstree/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919304 django-cards-0.9.0/cards/static/cards/jstree/css/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919670 django-cards-0.9.0/cards/static/cards/jstree/css/themes/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.940165 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/
+-rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.943761 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.946900 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/
+-rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/30px.png
+-rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/32px.png
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.919863 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.957661 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
+-rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.959340 django-cards-0.9.0/cards/static/cards/jstree/js/
+-rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/js/jstree.js
+-rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/static/cards/jstree/js/jstree.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.920160 django-cards-0.9.0/cards/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.920572 django-cards-0.9.0/cards/templates/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.960384 django-cards-0.9.0/cards/templates/cards/groups/
+-rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.9.0/cards/templates/cards/groups/groups.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.989996 django-cards-0.9.0/cards/templates/cards/standard/
+-rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/templates/cards/standard/blank.html
+-rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.9.0/cards/templates/cards/standard/card_group.html
+-rw-r--r--   0 tom        (501) staff       (20)     1158 2023-05-05 13:55:45.000000 django-cards-0.9.0/cards/templates/cards/standard/datatable.html
+-rw-r--r--   0 tom        (501) staff       (20)      778 2023-05-05 10:39:41.000000 django-cards-0.9.0/cards/templates/cards/standard/default.html
+-rw-r--r--   0 tom        (501) staff       (20)     1661 2023-05-17 09:02:56.000000 django-cards-0.9.0/cards/templates/cards/standard/default_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     1079 2023-05-05 13:55:45.000000 django-cards-0.9.0/cards/templates/cards/standard/html.html
+-rw-r--r--   0 tom        (501) staff       (20)     2606 2023-05-05 13:55:45.000000 django-cards-0.9.0/cards/templates/cards/standard/list_selection.html
+-rw-r--r--   0 tom        (501) staff       (20)      576 2023-05-05 11:16:16.000000 django-cards-0.9.0/cards/templates/cards/standard/message.html
+-rw-r--r--   0 tom        (501) staff       (20)      859 2023-05-05 11:16:16.000000 django-cards-0.9.0/cards/templates/cards/standard/table.html
+-rw-r--r--   0 tom        (501) staff       (20)     1546 2023-05-17 09:11:50.000000 django-cards-0.9.0/cards/templates/cards/standard/table_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     2198 2023-05-05 13:55:45.000000 django-cards-0.9.0/cards/templates/cards/standard/tree_selection.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.991215 django-cards-0.9.0/cards/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/templatetags/django_cards_tags.py
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.0/cards/url_converters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-17 09:16:05.996076 django-cards-0.9.0/django_cards.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-05-17 09:16:05.000000 django-cards-0.9.0/django_cards.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3065 2023-05-17 09:16:05.000000 django-cards-0.9.0/django_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-17 09:16:05.000000 django-cards-0.9.0/django_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-05-17 09:16:05.000000 django-cards-0.9.0/django_cards.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-17 09:16:05.997044 django-cards-0.9.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      645 2023-05-17 09:15:51.000000 django-cards-0.9.0/setup.py
```

### Comparing `django-cards-0.8.9/LICENSE` & `django-cards-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/PKG-INFO` & `django-cards-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.8.9
+Version: 0.9.0
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.8.9/cards/base.py` & `django-cards-0.9.0/cards/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,21 @@
                                          value_method=value_method,
                                          value_type=value_type,
                                          default_if=default_if,
                                          **kwargs)
         if entry is not None:
             self.rows.append({'type': 'standard', 'entries': [entry]})
 
+    def add_html_entry(self, template_name, context=None, **kwargs):
+        if context is None:
+            context = {}
+        context = {**context, **kwargs}
+        html = render_to_string(template_name=template_name, context=context)
+        self.rows.append({'type': 'html', 'html': html, **kwargs})
+
     def get_field_value(self, value, field, label):
         field_type = None
         if value is None and field is not None:
             if isinstance(field, (list, tuple)):
                 values = []
                 field_type = []
                 for _field in field:
@@ -425,15 +432,15 @@
 
     def datatable_sort(self, **kwargs):
         order_field = self.extra_card_info['order_field']
         ids = [x[1] for x in kwargs['sort']]
         current_sort = dict(self.extra_card_info['datatable_model'].objects.filter(id__in=ids).
                             values_list('id', order_field))
         for s in kwargs['sort']:
-            if current_sort[s[1]] != s[0]:
+            if current_sort.get(s[1]) != s[0]:
                 o = self.extra_card_info['datatable_model'].objects.get(id=s[1])
                 setattr(o, order_field, s[0])
                 o.save()
         return self.command_response('null')
 
     @staticmethod
     def label_from_field(field, field_type):
```

### Comparing `django-cards-0.8.9/cards/card_list/base.py` & `django-cards-0.9.0/cards/card_list/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/card_list/main.py` & `django-cards-0.9.0/cards/card_list/main.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/card_list/tree.py` & `django-cards-0.9.0/cards/card_list/tree.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/includes.py` & `django-cards-0.9.0/cards/includes.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/standard.py` & `django-cards-0.9.0/cards/standard.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/32px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/40px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/style.min.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default/throbber.gif` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/32px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/40px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/style.min.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/default-dark/throbber.gif` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/30px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/30px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/32px.png` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/style.min.css` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/css/themes/proton/throbber.gif` & `django-cards-0.9.0/cards/static/cards/jstree/css/themes/proton/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/js/jstree.js` & `django-cards-0.9.0/cards/static/cards/jstree/js/jstree.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/static/cards/jstree/js/jstree.min.js` & `django-cards-0.9.0/cards/static/cards/jstree/js/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/card_group.html` & `django-cards-0.9.0/cards/templates/cards/standard/card_group.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/datatable.html` & `django-cards-0.9.0/cards/templates/cards/standard/table.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-{% load datatable_tags %}
 
-    <div class="{{ card_css_class }}" id="list" data-title="">
+    <div class="{{ card_css_class }}" id="{{ card.code }}" data-title="">
         <div class="card-header">
             <div class="d-flex align-items-center">
                 <h5 class="mr-auto">{{ card.title }}</h5>
                 {{ card.menu.render }}
             </div>
         </div>
-        {{ card.tab_menu.render }}
-        <div class="{{ card_body_css_class }}">
-            {{ card.extra_card_info.datatable.render|safe }}
-        </div>
+
+    {% include 'cards/standard/table_body.html' %}
+
         {% if card.footer %}
             <div class="card-footer">
                 <small style="text-align: left">{{ card.footer|safe }}</small>
             </div>
         {% endif %}
         {% if card.created_modified_dates %}
             <div class="card-footer">
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/default.html` & `django-cards-0.9.0/cards/templates/cards/standard/default.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<div class="{{ card_css_class }}" id="list" data-title="">
+<div class="{{ card_css_class }}" id="{{ card.code }}" data-title="">
     <div class="card-header">
         <div class="d-flex align-items-center">
             <h5 class="mr-auto">{{ card.title }}</h5>
             {{ card.menu.render }}
         </div>
     </div>
     {% include 'cards/standard/default_body.html' %}
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/default_body.html` & `django-cards-0.9.0/cards/templates/cards/standard/default_body.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 {{ card.tab_menu.render }}
 <div class="{{ card_body_css_class }}">
     <div class="list-group">
         {% for row in card.rows %}
+            {% if row.type == 'html' %}<div class="{{ item_css_class }}">{{ row.html|safe }}</div>{% else %}
             {% if row.type == 'multiple' %}<div class="row">{% endif %}
             {% for entry in row.entries %}
                 {% if entry.entry_css_class %}<div class="{{ entry.entry_css_class }}">{% endif %}
                 {% if entry.link %}<a class="{{ item_css_class }} cards-list-group-item" href="{{ entry.link }}" style="{{ item_css }}">{% else %}<div class="{{ item_css_class }}" style="{{ item_css }}">{% endif %}
                     {% if entry.label %}
                         <div class="d-flex"><label class="mr-auto">{{ entry.label|safe }}</label>{{ entry.menu.render }}</div>
                         {% if entry.multiple_lines %}
@@ -19,10 +20,11 @@
                     {% else %}
                         {{ entry.html|safe }}
                     {% endif %}
             {% if entry.link %}</a>{% else %}</div>{% endif %}
              {% if entry.entry_css_class %}</div>{% endif %}
             {% endfor %}
             {% if row.type == 'multiple' %}</div>{% endif %}
+            {% endif %}
         {% endfor %}
     </div>
 </div>
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/html.html` & `django-cards-0.9.0/cards/templates/cards/standard/datatable.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-    <div class="{{ card_css_class }}" id="{{ card.code }}" data-title="">
+{% load datatable_tags %}
+
+    <div class="{{ card_css_class }}" id="{{ card.code }}_card" {% if card_css_style %}style="{{ card_css_style }}"{% endif %} data-title="">
         <div class="card-header">
             <div class="d-flex align-items-center">
                 <h5 class="mr-auto">{{ card.title }}</h5>
                 {{ card.menu.render }}
             </div>
         </div>
-        <div class="{{ card_body_css_class }}">
-            {{ card.extra_card_info.html|safe }}
+        {{ card.tab_menu.render }}
+        <div class="{{ card_body_css_class }}" id="{{ card.code }}_body" {% if card_body_css_style %}style="{{ card_body_css_style }}"{% endif %}>
+            {{ card.extra_card_info.datatable.render|safe }}
         </div>
         {% if card.footer %}
             <div class="card-footer">
                 <small style="text-align: left">{{ card.footer|safe }}</small>
             </div>
         {% endif %}
         {% if card.created_modified_dates %}
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/list_selection.html` & `django-cards-0.9.0/cards/templates/cards/standard/list_selection.html`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 <div class="{{ card_css_class }}" id="{{ card.code }}" data-title="">
     <div class="card-header">
         <div class="d-flex align-items-center">
             <h5 class="mr-auto">{{ card.title }}</h5>
             {{ card.menu.render }}
         </div>
     </div>
-    <div class="{{ card_body_css_class }}" style="{{ card_body_css_style }}">
+    <div class="{{ card_body_css_class }}" id="{{ card.code }}_body" {% if card_body_css_style %}style="{{ card_body_css_style }}"{% endif %}>
     {% for entry in entries %}
         <a class="{{ card_link_css_class }}" id="list_{{ entry.pk }}"
            href="javascript:load_details({{ entry.pk }})">
             <div class="row">
                 <div class="col-sm-12">
                     <h4 class="list-group-item-heading {{ entry.class }}">
                         {% if entry.colour %}<i class="fa fa-square"
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/message.html` & `django-cards-0.9.0/cards/templates/cards/standard/message.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load datatable_tags %}
 
-    <div class="{{ card_css_class }}" id="list" data-title="">
+    <div class="{{ card_css_class }}" id="{{ card.code }}" data-title="">
         {% if card.title %}
             <div class="card-header">
                 <div class="d-flex align-items-center">
                     <h5 class="mr-auto">{{ card.title|safe }}</h5>
                     {{ card.menu.render }}
                 </div>
             </div>
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/table_body.html` & `django-cards-0.9.0/cards/templates/cards/standard/table_body.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 {{ card.tab_menu.render }}
 <div class="{{ card_body_css_class }}">
-    <div class="list-group">
+    <td class="list-group">
         <table class="{{ table_css_class }}">
             {% for row in card.rows %}
                 <tr>
+                    {% if row.type == 'html' %}{% if not row.exclude_td %}<td class="{{ table_td_css_class }}"{% if row.colspan %} colspan="{{ row.colspan }}"{% endif %} {% if row.rowspan %} rowspan="{{ row.rowspan }}"{% endif %}>{{ row.html|safe }}</td>{% else %}{{ row.html|safe }}{% endif %}{% else %}
                     {% for entry in row.entries %}
                         {% if forloop.first %}<th class="{{ table_th_css_class }}">{{ entry.label|safe }}</th>{% endif %}
                         <td class="{{ table_td_css_class }}"{% if entry.colspan %} colspan="{{ entry.colspan }}"{% endif %}{% if entry.rowspan %} rowspan="{{ entry.rowspan }}"{% endif %}>{% if entry.link %}
                             <a class="list-group-item cards-list-group-item" href="{{ entry.link }}">{% endif %}
                             {% if entry.multiple_lines %}
                                 {% for x in entry.html %}
                                     {{ entry.css_class }}">{{ x|safe }}<br/>
                                 {% endfor %}
                             {% else %}
                                 {{ entry.html|safe }}
                             {% endif %}
                             {% if entry.link %}</a>{% endif %}</td>
-                    {% endfor %}</tr>
+                    {% endfor %}{% endif %}</tr>
             {% endfor %}
         </table>
     </div>
 </div>
```

### Comparing `django-cards-0.8.9/cards/templates/cards/standard/tree_selection.html` & `django-cards-0.9.0/cards/templates/cards/standard/tree_selection.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     <div class="card-header">
         <div class="d-flex align-items-center">
             <h5 class="mr-auto">{{ card.title }}</h5>
             {{ card.menu.render }}
         </div>
     </div>
     {{ card.tab_menu.render }}
-    <div class="{{ card_body_css_class }}" style="{{ card_body_css_style }}">
+
+    <div class="{{ card_body_css_class }}" id="{{ card.code }}_body" {% if card_body_css_style %}style="{{ card_body_css_style }}"{% endif %}>
         <div id="{{ card.code }}_tree"></div>
         <script>
             $('#{{ card.code }}_tree').jstree({
                 'core': {
                     'data': {{ data|safe }},
                     'themes': {{ tree_themes|safe }}
                 }{% if tree_plugins %}, 'plugins':{{ tree_plugins|safe }}{% endif %}
```

### Comparing `django-cards-0.8.9/django_cards.egg-info/PKG-INFO` & `django-cards-0.9.0/django_cards.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.8.9
+Version: 0.9.0
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.8.9/django_cards.egg-info/SOURCES.txt` & `django-cards-0.9.0/django_cards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cards-0.8.9/setup.py` & `django-cards-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-cards",
-    version="0.8.9",
+    version="0.9.0",
     author="Thomas Turner",
     description="Django app that allows you make cards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-cards",
     include_package_data=True,
     packages=['cards'],
```

