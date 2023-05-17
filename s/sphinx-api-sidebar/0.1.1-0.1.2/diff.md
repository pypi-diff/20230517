# Comparing `tmp/sphinx_api_sidebar-0.1.1.tar.gz` & `tmp/sphinx_api_sidebar-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_api_sidebar-0.1.1.tar", last modified: Thu May  4 23:41:32 2023, max compression
+gzip compressed data, was "sphinx_api_sidebar-0.1.2.tar", last modified: Wed May 10 09:20:49 2023, max compression
```

## Comparing `sphinx_api_sidebar-0.1.1.tar` & `sphinx_api_sidebar-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.847503 sphinx_api_sidebar-0.1.1/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-04 06:26:37.000000 sphinx_api_sidebar-0.1.1/LICENSE
--rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-04 06:32:13.000000 sphinx_api_sidebar-0.1.1/MANIFEST.in
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4730 2023-05-04 23:41:32.846940 sphinx_api_sidebar-0.1.1/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)     2805 2023-05-04 23:38:29.000000 sphinx_api_sidebar-0.1.1/README.md
--rw-r--r--   0 yihengxiong   (501) staff       (20)      358 2023-05-04 23:39:35.000000 sphinx_api_sidebar-0.1.1/pyproject.toml
--rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-04 23:41:32.847670 sphinx_api_sidebar-0.1.1/setup.cfg
--rw-r--r--   0 yihengxiong   (501) staff       (20)      934 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.1/setup.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.837836 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/
--rw-r--r--   0 yihengxiong   (501) staff       (20)       37 2023-05-04 06:28:19.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/__init__.py
--rw-r--r--   0 yihengxiong   (501) staff       (20)     1526 2023-05-04 23:02:49.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar/sphinx_api_sidebar.py
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.845482 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/
--rw-r--r--   0 yihengxiong   (501) staff       (20)     4730 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/PKG-INFO
--rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/SOURCES.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/dependency_links.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/entry_points.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       12 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/requires.txt
--rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-04 23:41:32.000000 sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/top_level.txt
-drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-04 23:41:32.845994 sphinx_api_sidebar-0.1.1/tests/
--rw-r--r--   0 yihengxiong   (501) staff       (20)      555 2023-05-04 16:40:41.000000 sphinx_api_sidebar-0.1.1/tests/test_sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-10 09:20:49.650855 sphinx_api_sidebar-0.1.2/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     1069 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.1.2/LICENSE
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        0 2023-05-10 08:31:45.000000 sphinx_api_sidebar-0.1.2/MANIFEST.in
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4193 2023-05-10 09:20:49.650736 sphinx_api_sidebar-0.1.2/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2248 2023-05-10 09:18:16.000000 sphinx_api_sidebar-0.1.2/README.md
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      441 2023-05-10 09:20:32.000000 sphinx_api_sidebar-0.1.2/pyproject.toml
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-10 09:20:49.650897 sphinx_api_sidebar-0.1.2/setup.cfg
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      899 2023-05-10 09:20:39.000000 sphinx_api_sidebar-0.1.2/setup.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-10 09:20:49.649001 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       38 2023-05-10 08:59:33.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar/__init__.py
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     2437 2023-05-10 09:00:08.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar/sphinx_api_sidebar.py
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-10 09:20:49.650243 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)     4193 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/PKG-INFO
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      412 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/SOURCES.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)        1 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/dependency_links.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       66 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/entry_points.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       47 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/requires.txt
+-rw-r--r--   0 yihengxiong   (501) staff       (20)       19 2023-05-10 09:20:49.000000 sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/top_level.txt
+drwxr-xr-x   0 yihengxiong   (501) staff       (20)        0 2023-05-10 09:20:49.650422 sphinx_api_sidebar-0.1.2/tests/
+-rw-r--r--   0 yihengxiong   (501) staff       (20)      557 2023-05-10 09:00:08.000000 sphinx_api_sidebar-0.1.2/tests/test_sphinx_api_sidebar.py
```

### Comparing `sphinx_api_sidebar-0.1.1/LICENSE` & `sphinx_api_sidebar-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_api_sidebar-0.1.1/PKG-INFO` & `sphinx_api_sidebar-0.1.2/sphinx_api_sidebar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sphinx_api_sidebar
-Version: 0.1.1
+Name: sphinx-api-sidebar
+Version: 0.1.2
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -31,25 +31,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Sphinx API Sidebar
 
 A Sphinx extension for displaying any generated static API documentation in a sidebar.
 
 ## Overview
 
-This Sphinx extension allows you to include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used in the API sidebar template.
+This Sphinx extension allows you to include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used to render the API documentation sidebar template.
 
-This extension serves as an immediate workaround to make Sphinx consume API docs from various languages without building additional extensions.
+This extension serves as an immediate workaround to make Sphinx consume API docs in HTML format from various languages without building additional deeply integrated extensions for each type of API docs.
 
 ## Installation
 
 To install the `sphinx-api-sidebar` extension, you can use pip:
 
 ```sh
 pip install sphinx-api-sidebar
@@ -61,15 +62,15 @@
 ```python
 extensions = [
     'sphinx_api_sidebar',
     # Other extensions...
 ]
 ```
 
-2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
+2. To use a custom command to generate your API documentation or specify different directories, you can set the `api_docs_generators` configuration value in your conf.py file:
 
 ```python
 api_docs_generators = [
   {
     'command': '<your_api_docs_build_command_1>',
     'outputs': [
             {
@@ -93,33 +94,19 @@
             # ...
         ]
   },
   # more groups of generated api docs
 ]
 ```
 
-Replace <your_custom_build_command_*>, <generated_api_doc_name_*>, and <path_to_generated_api_doc_*> with the appropriate values for your project.
+Replace `<your_custom_build_command_*>`, `<generated_api_doc_name_*>`, and `<path_to_generated_api_doc_*>` with the appropriate values for your project.
 
-
-3. To make the different api documentation show up in the sidebar, you will need to copy the `api_docs_sidebar.html` template file from the `sphinx_api_sidebar/templates` folder of the installed package to your Sphinx project's _templates folder. Alternatively, you can create a new file in your project's _templates folder with the following content:
-
-```html
-{% if api_docs %}
-  <h3>{{ _('API Documentation') }}</h3>
-  <ul style="list-style-type: none;">
-    {%- for item in api_docs %}
-      <li style="margin-bottom: 10px;"><a href="{{ pathto('_static/api-docs/{}'.format(item), 1) }}">{{ item }}</a></li>
-    {%- endfor %}
-  </ul>
-{% endif %}
-```
-
-4. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
+3. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
 
 ```python
 html_sidebars = {
     '**': [
         # ... other sidebars ...
-        'api_docs_sidebar.html',
+        'sidebar/api_docs_sidebar.html',
     ]
 }
 ```
```

### Comparing `sphinx_api_sidebar-0.1.1/README.md` & `sphinx_api_sidebar-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,161 +16,126 @@
 000000f0: 7369 6465 6261 7220 6f66 2079 6f75 7220  sidebar of your 
 00000100: 5370 6869 6e78 2064 6f63 756d 656e 7461  Sphinx documenta
 00000110: 7469 6f6e 2e20 4974 2075 7064 6174 6573  tion. It updates
 00000120: 2074 6865 2060 6874 6d6c 5f63 6f6e 7465   the `html_conte
 00000130: 7874 6020 7769 7468 2074 6865 2041 5049  xt` with the API
 00000140: 2064 6f63 756d 656e 7461 7469 6f6e 2070   documentation p
 00000150: 6174 6873 2c20 7768 6963 6820 6361 6e20  aths, which can 
-00000160: 7468 656e 2062 6520 7573 6564 2069 6e20  then be used in 
-00000170: 7468 6520 4150 4920 7369 6465 6261 7220  the API sidebar 
-00000180: 7465 6d70 6c61 7465 2e0a 0a54 6869 7320  template...This 
-00000190: 6578 7465 6e73 696f 6e20 7365 7276 6573  extension serves
-000001a0: 2061 7320 616e 2069 6d6d 6564 6961 7465   as an immediate
-000001b0: 2077 6f72 6b61 726f 756e 6420 746f 206d   workaround to m
-000001c0: 616b 6520 5370 6869 6e78 2063 6f6e 7375  ake Sphinx consu
-000001d0: 6d65 2041 5049 2064 6f63 7320 6672 6f6d  me API docs from
-000001e0: 2076 6172 696f 7573 206c 616e 6775 6167   various languag
-000001f0: 6573 2077 6974 686f 7574 2062 7569 6c64  es without build
-00000200: 696e 6720 6164 6469 7469 6f6e 616c 2065  ing additional e
-00000210: 7874 656e 7369 6f6e 732e 0a0a 2323 2049  xtensions...## I
-00000220: 6e73 7461 6c6c 6174 696f 6e0a 0a54 6f20  nstallation..To 
-00000230: 696e 7374 616c 6c20 7468 6520 6073 7068  install the `sph
-00000240: 696e 782d 6170 692d 7369 6465 6261 7260  inx-api-sidebar`
-00000250: 2065 7874 656e 7369 6f6e 2c20 796f 7520   extension, you 
-00000260: 6361 6e20 7573 6520 7069 703a 0a0a 6060  can use pip:..``
-00000270: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
-00000280: 7370 6869 6e78 2d61 7069 2d73 6964 6562  sphinx-api-sideb
-00000290: 6172 0a60 6060 0a0a 2323 2055 7361 6765  ar.```..## Usage
-000002a0: 0a31 2e20 546f 2065 6e61 626c 6520 7468  .1. To enable th
-000002b0: 6520 7370 6869 6e78 2d61 7069 2d73 6964  e sphinx-api-sid
-000002c0: 6562 6172 2065 7874 656e 7369 6f6e 2069  ebar extension i
-000002d0: 6e20 796f 7572 2053 7068 696e 7820 646f  n your Sphinx do
-000002e0: 6375 6d65 6e74 6174 696f 6e20 7072 6f6a  cumentation proj
-000002f0: 6563 742c 2061 6464 2069 7420 746f 2074  ect, add it to t
-00000300: 6865 2065 7874 656e 7369 6f6e 7320 6c69  he extensions li
-00000310: 7374 2069 6e20 796f 7572 2063 6f6e 662e  st in your conf.
-00000320: 7079 2066 696c 653a 0a0a 6060 6070 7974  py file:..```pyt
-00000330: 686f 6e0a 6578 7465 6e73 696f 6e73 203d  hon.extensions =
-00000340: 205b 0a20 2020 2027 7370 6869 6e78 5f61   [.    'sphinx_a
-00000350: 7069 5f73 6964 6562 6172 272c 0a20 2020  pi_sidebar',.   
-00000360: 2023 204f 7468 6572 2065 7874 656e 7369   # Other extensi
-00000370: 6f6e 732e 2e2e 0a5d 0a60 6060 0a0a 322e  ons....].```..2.
-00000380: 2054 6f20 7573 6520 6120 6375 7374 6f6d   To use a custom
-00000390: 2063 6f6d 6d61 6e64 2074 6f20 6765 6e65   command to gene
-000003a0: 7261 7465 2079 6f75 7220 4150 4920 646f  rate your API do
-000003b0: 6375 6d65 6e74 6174 696f 6e20 6f72 2073  cumentation or s
-000003c0: 7065 6369 6679 2064 6966 6665 7265 6e74  pecify different
-000003d0: 2064 6972 6563 746f 7269 6573 2c20 796f   directories, yo
-000003e0: 7520 6361 6e20 7365 7420 7468 6520 6170  u can set the ap
-000003f0: 695f 646f 6373 5f67 656e 6572 6174 6f72  i_docs_generator
-00000400: 2063 6f6e 6669 6775 7261 7469 6f6e 2076   configuration v
-00000410: 616c 7565 2069 6e20 796f 7572 2063 6f6e  alue in your con
-00000420: 662e 7079 2066 696c 653a 0a0a 6060 6070  f.py file:..```p
-00000430: 7974 686f 6e0a 6170 695f 646f 6373 5f67  ython.api_docs_g
-00000440: 656e 6572 6174 6f72 7320 3d20 5b0a 2020  enerators = [.  
-00000450: 7b0a 2020 2020 2763 6f6d 6d61 6e64 273a  {.    'command':
-00000460: 2027 3c79 6f75 725f 6170 695f 646f 6373   '<your_api_docs
-00000470: 5f62 7569 6c64 5f63 6f6d 6d61 6e64 5f31  _build_command_1
-00000480: 3e27 2c0a 2020 2020 276f 7574 7075 7473  >',.    'outputs
-00000490: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
-000004a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000004b0: 2020 2027 6e61 6d65 273a 2027 3c67 656e     'name': '<gen
-000004c0: 6572 6174 6564 5f61 7069 5f64 6f63 5f6e  erated_api_doc_n
-000004d0: 616d 655f 313e 272c 0a20 2020 2020 2020  ame_1>',.       
-000004e0: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
-000004f0: 2027 3c70 6174 685f 746f 5f67 656e 6572   '<path_to_gener
-00000500: 6174 6564 5f61 7069 5f64 6f63 5f31 3e27  ated_api_doc_1>'
-00000510: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00000520: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00000530: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-00000540: 616d 6527 3a20 273c 6765 6e65 7261 7465  ame': '<generate
-00000550: 645f 6170 695f 646f 635f 6e61 6d65 5f32  d_api_doc_name_2
-00000560: 3e27 2c0a 2020 2020 2020 2020 2020 2020  >',.            
-00000570: 2020 2020 2770 6174 6827 3a20 273c 7061      'path': '<pa
-00000580: 7468 5f74 6f5f 6765 6e65 7261 7465 645f  th_to_generated_
-00000590: 6170 695f 646f 635f 323e 270a 2020 2020  api_doc_2>'.    
-000005a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000005b0: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
-000005c0: 2020 2020 205d 0a20 207d 2c0a 2020 7b0a       ].  },.  {.
-000005d0: 2020 2020 2763 6f6d 6d61 6e64 273a 2027      'command': '
-000005e0: 3c79 6f75 725f 6375 7374 6f6d 5f62 7569  <your_custom_bui
-000005f0: 6c64 5f63 6f6d 6d61 6e64 5f32 3e27 2c0a  ld_command_2>',.
-00000600: 2020 2020 276f 7574 7075 7473 273a 205b      'outputs': [
-00000610: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-00000620: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00000630: 6e61 6d65 273a 2027 3c67 656e 6572 6174  name': '<generat
-00000640: 6564 5f61 7069 5f64 6f63 5f6e 616d 655f  ed_api_doc_name_
-00000650: 333e 272c 0a20 2020 2020 2020 2020 2020  3>',.           
-00000660: 2020 2020 2027 7061 7468 273a 2027 3c70       'path': '<p
-00000670: 6174 685f 746f 5f67 656e 6572 6174 6564  ath_to_generated
-00000680: 5f61 7069 5f64 6f63 5f33 3e27 0a20 2020  _api_doc_3>'.   
-00000690: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000006a0: 2020 2020 2020 2020 2320 2e2e 2e0a 2020          # ....  
-000006b0: 2020 2020 2020 5d0a 2020 7d2c 0a20 2023        ].  },.  #
-000006c0: 206d 6f72 6520 6772 6f75 7073 206f 6620   more groups of 
-000006d0: 6765 6e65 7261 7465 6420 6170 6920 646f  generated api do
-000006e0: 6373 0a5d 0a60 6060 0a0a 5265 706c 6163  cs.].```..Replac
-000006f0: 6520 3c79 6f75 725f 6375 7374 6f6d 5f62  e <your_custom_b
-00000700: 7569 6c64 5f63 6f6d 6d61 6e64 5f2a 3e2c  uild_command_*>,
-00000710: 203c 6765 6e65 7261 7465 645f 6170 695f   <generated_api_
-00000720: 646f 635f 6e61 6d65 5f2a 3e2c 2061 6e64  doc_name_*>, and
-00000730: 203c 7061 7468 5f74 6f5f 6765 6e65 7261   <path_to_genera
-00000740: 7465 645f 6170 695f 646f 635f 2a3e 2077  ted_api_doc_*> w
-00000750: 6974 6820 7468 6520 6170 7072 6f70 7269  ith the appropri
-00000760: 6174 6520 7661 6c75 6573 2066 6f72 2079  ate values for y
-00000770: 6f75 7220 7072 6f6a 6563 742e 0a0a 0a33  our project....3
-00000780: 2e20 546f 206d 616b 6520 7468 6520 6469  . To make the di
-00000790: 6666 6572 656e 7420 6170 6920 646f 6375  fferent api docu
-000007a0: 6d65 6e74 6174 696f 6e20 7368 6f77 2075  mentation show u
-000007b0: 7020 696e 2074 6865 2073 6964 6562 6172  p in the sidebar
-000007c0: 2c20 796f 7520 7769 6c6c 206e 6565 6420  , you will need 
-000007d0: 746f 2063 6f70 7920 7468 6520 6061 7069  to copy the `api
-000007e0: 5f64 6f63 735f 7369 6465 6261 722e 6874  _docs_sidebar.ht
-000007f0: 6d6c 6020 7465 6d70 6c61 7465 2066 696c  ml` template fil
-00000800: 6520 6672 6f6d 2074 6865 2060 7370 6869  e from the `sphi
-00000810: 6e78 5f61 7069 5f73 6964 6562 6172 2f74  nx_api_sidebar/t
-00000820: 656d 706c 6174 6573 6020 666f 6c64 6572  emplates` folder
-00000830: 206f 6620 7468 6520 696e 7374 616c 6c65   of the installe
-00000840: 6420 7061 636b 6167 6520 746f 2079 6f75  d package to you
-00000850: 7220 5370 6869 6e78 2070 726f 6a65 6374  r Sphinx project
-00000860: 2773 205f 7465 6d70 6c61 7465 7320 666f  's _templates fo
-00000870: 6c64 6572 2e20 416c 7465 726e 6174 6976  lder. Alternativ
-00000880: 656c 792c 2079 6f75 2063 616e 2063 7265  ely, you can cre
-00000890: 6174 6520 6120 6e65 7720 6669 6c65 2069  ate a new file i
-000008a0: 6e20 796f 7572 2070 726f 6a65 6374 2773  n your project's
-000008b0: 205f 7465 6d70 6c61 7465 7320 666f 6c64   _templates fold
-000008c0: 6572 2077 6974 6820 7468 6520 666f 6c6c  er with the foll
-000008d0: 6f77 696e 6720 636f 6e74 656e 743a 0a0a  owing content:..
-000008e0: 6060 6068 746d 6c0a 7b25 2069 6620 6170  ```html.{% if ap
-000008f0: 695f 646f 6373 2025 7d0a 2020 3c68 333e  i_docs %}.  <h3>
-00000900: 7b7b 205f 2827 4150 4920 446f 6375 6d65  {{ _('API Docume
-00000910: 6e74 6174 696f 6e27 2920 7d7d 3c2f 6833  ntation') }}</h3
-00000920: 3e0a 2020 3c75 6c20 7374 796c 653d 226c  >.  <ul style="l
-00000930: 6973 742d 7374 796c 652d 7479 7065 3a20  ist-style-type: 
-00000940: 6e6f 6e65 3b22 3e0a 2020 2020 7b25 2d20  none;">.    {%- 
-00000950: 666f 7220 6974 656d 2069 6e20 6170 695f  for item in api_
-00000960: 646f 6373 2025 7d0a 2020 2020 2020 3c6c  docs %}.      <l
-00000970: 6920 7374 796c 653d 226d 6172 6769 6e2d  i style="margin-
-00000980: 626f 7474 6f6d 3a20 3130 7078 3b22 3e3c  bottom: 10px;"><
-00000990: 6120 6872 6566 3d22 7b7b 2070 6174 6874  a href="{{ patht
-000009a0: 6f28 275f 7374 6174 6963 2f61 7069 2d64  o('_static/api-d
-000009b0: 6f63 732f 7b7d 272e 666f 726d 6174 2869  ocs/{}'.format(i
-000009c0: 7465 6d29 2c20 3129 207d 7d22 3e7b 7b20  tem), 1) }}">{{ 
-000009d0: 6974 656d 207d 7d3c 2f61 3e3c 2f6c 693e  item }}</a></li>
-000009e0: 0a20 2020 207b 252d 2065 6e64 666f 7220  .    {%- endfor 
-000009f0: 257d 0a20 203c 2f75 6c3e 0a7b 2520 656e  %}.  </ul>.{% en
-00000a00: 6469 6620 257d 0a60 6060 0a0a 342e 2055  dif %}.```..4. U
-00000a10: 7064 6174 6520 796f 7572 2060 636f 6e66  pdate your `conf
-00000a20: 2e70 7960 2066 696c 6520 746f 2069 6e63  .py` file to inc
-00000a30: 6c75 6465 2074 6865 2060 6170 695f 646f  lude the `api_do
-00000a40: 6373 5f73 6964 6562 6172 2e68 746d 6c60  cs_sidebar.html`
-00000a50: 2074 656d 706c 6174 6520 696e 2074 6865   template in the
-00000a60: 2068 746d 6c5f 7369 6465 6261 7273 2063   html_sidebars c
-00000a70: 6f6e 6669 6775 7261 7469 6f6e 3a0a 0a60  onfiguration:..`
-00000a80: 6060 7079 7468 6f6e 0a68 746d 6c5f 7369  ``python.html_si
-00000a90: 6465 6261 7273 203d 207b 0a20 2020 2027  debars = {.    '
-00000aa0: 2a2a 273a 205b 0a20 2020 2020 2020 2023  **': [.        #
-00000ab0: 202e 2e2e 206f 7468 6572 2073 6964 6562   ... other sideb
-00000ac0: 6172 7320 2e2e 2e0a 2020 2020 2020 2020  ars ....        
-00000ad0: 2761 7069 5f64 6f63 735f 7369 6465 6261  'api_docs_sideba
-00000ae0: 722e 6874 6d6c 272c 0a20 2020 205d 0a7d  r.html',.    ].}
-00000af0: 0a60 6060 0a                             .```.
+00000160: 7468 656e 2062 6520 7573 6564 2074 6f20  then be used to 
+00000170: 7265 6e64 6572 2074 6865 2041 5049 2064  render the API d
+00000180: 6f63 756d 656e 7461 7469 6f6e 2073 6964  ocumentation sid
+00000190: 6562 6172 2074 656d 706c 6174 652e 0a0a  ebar template...
+000001a0: 5468 6973 2065 7874 656e 7369 6f6e 2073  This extension s
+000001b0: 6572 7665 7320 6173 2061 6e20 696d 6d65  erves as an imme
+000001c0: 6469 6174 6520 776f 726b 6172 6f75 6e64  diate workaround
+000001d0: 2074 6f20 6d61 6b65 2053 7068 696e 7820   to make Sphinx 
+000001e0: 636f 6e73 756d 6520 4150 4920 646f 6373  consume API docs
+000001f0: 2069 6e20 4854 4d4c 2066 6f72 6d61 7420   in HTML format 
+00000200: 6672 6f6d 2076 6172 696f 7573 206c 616e  from various lan
+00000210: 6775 6167 6573 2077 6974 686f 7574 2062  guages without b
+00000220: 7569 6c64 696e 6720 6164 6469 7469 6f6e  uilding addition
+00000230: 616c 2064 6565 706c 7920 696e 7465 6772  al deeply integr
+00000240: 6174 6564 2065 7874 656e 7369 6f6e 7320  ated extensions 
+00000250: 666f 7220 6561 6368 2074 7970 6520 6f66  for each type of
+00000260: 2041 5049 2064 6f63 732e 0a0a 2323 2049   API docs...## I
+00000270: 6e73 7461 6c6c 6174 696f 6e0a 0a54 6f20  nstallation..To 
+00000280: 696e 7374 616c 6c20 7468 6520 6073 7068  install the `sph
+00000290: 696e 782d 6170 692d 7369 6465 6261 7260  inx-api-sidebar`
+000002a0: 2065 7874 656e 7369 6f6e 2c20 796f 7520   extension, you 
+000002b0: 6361 6e20 7573 6520 7069 703a 0a0a 6060  can use pip:..``
+000002c0: 6073 680a 7069 7020 696e 7374 616c 6c20  `sh.pip install 
+000002d0: 7370 6869 6e78 2d61 7069 2d73 6964 6562  sphinx-api-sideb
+000002e0: 6172 0a60 6060 0a0a 2323 2055 7361 6765  ar.```..## Usage
+000002f0: 0a31 2e20 546f 2065 6e61 626c 6520 7468  .1. To enable th
+00000300: 6520 7370 6869 6e78 2d61 7069 2d73 6964  e sphinx-api-sid
+00000310: 6562 6172 2065 7874 656e 7369 6f6e 2069  ebar extension i
+00000320: 6e20 796f 7572 2053 7068 696e 7820 646f  n your Sphinx do
+00000330: 6375 6d65 6e74 6174 696f 6e20 7072 6f6a  cumentation proj
+00000340: 6563 742c 2061 6464 2069 7420 746f 2074  ect, add it to t
+00000350: 6865 2065 7874 656e 7369 6f6e 7320 6c69  he extensions li
+00000360: 7374 2069 6e20 796f 7572 2063 6f6e 662e  st in your conf.
+00000370: 7079 2066 696c 653a 0a0a 6060 6070 7974  py file:..```pyt
+00000380: 686f 6e0a 6578 7465 6e73 696f 6e73 203d  hon.extensions =
+00000390: 205b 0a20 2020 2027 7370 6869 6e78 5f61   [.    'sphinx_a
+000003a0: 7069 5f73 6964 6562 6172 272c 0a20 2020  pi_sidebar',.   
+000003b0: 2023 204f 7468 6572 2065 7874 656e 7369   # Other extensi
+000003c0: 6f6e 732e 2e2e 0a5d 0a60 6060 0a0a 322e  ons....].```..2.
+000003d0: 2054 6f20 7573 6520 6120 6375 7374 6f6d   To use a custom
+000003e0: 2063 6f6d 6d61 6e64 2074 6f20 6765 6e65   command to gene
+000003f0: 7261 7465 2079 6f75 7220 4150 4920 646f  rate your API do
+00000400: 6375 6d65 6e74 6174 696f 6e20 6f72 2073  cumentation or s
+00000410: 7065 6369 6679 2064 6966 6665 7265 6e74  pecify different
+00000420: 2064 6972 6563 746f 7269 6573 2c20 796f   directories, yo
+00000430: 7520 6361 6e20 7365 7420 7468 6520 6061  u can set the `a
+00000440: 7069 5f64 6f63 735f 6765 6e65 7261 746f  pi_docs_generato
+00000450: 7273 6020 636f 6e66 6967 7572 6174 696f  rs` configuratio
+00000460: 6e20 7661 6c75 6520 696e 2079 6f75 7220  n value in your 
+00000470: 636f 6e66 2e70 7920 6669 6c65 3a0a 0a60  conf.py file:..`
+00000480: 6060 7079 7468 6f6e 0a61 7069 5f64 6f63  ``python.api_doc
+00000490: 735f 6765 6e65 7261 746f 7273 203d 205b  s_generators = [
+000004a0: 0a20 207b 0a20 2020 2027 636f 6d6d 616e  .  {.    'comman
+000004b0: 6427 3a20 273c 796f 7572 5f61 7069 5f64  d': '<your_api_d
+000004c0: 6f63 735f 6275 696c 645f 636f 6d6d 616e  ocs_build_comman
+000004d0: 645f 313e 272c 0a20 2020 2027 6f75 7470  d_1>',.    'outp
+000004e0: 7574 7327 3a20 5b0a 2020 2020 2020 2020  uts': [.        
+000004f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00000500: 2020 2020 2020 276e 616d 6527 3a20 273c        'name': '<
+00000510: 6765 6e65 7261 7465 645f 6170 695f 646f  generated_api_do
+00000520: 635f 6e61 6d65 5f31 3e27 2c0a 2020 2020  c_name_1>',.    
+00000530: 2020 2020 2020 2020 2020 2020 2770 6174              'pat
+00000540: 6827 3a20 273c 7061 7468 5f74 6f5f 6765  h': '<path_to_ge
+00000550: 6e65 7261 7465 645f 6170 695f 646f 635f  nerated_api_doc_
+00000560: 313e 270a 2020 2020 2020 2020 2020 2020  1>'.            
+00000570: 7d2c 0a20 2020 2020 2020 2020 2020 207b  },.            {
+00000580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000590: 2027 6e61 6d65 273a 2027 3c67 656e 6572   'name': '<gener
+000005a0: 6174 6564 5f61 7069 5f64 6f63 5f6e 616d  ated_api_doc_nam
+000005b0: 655f 323e 272c 0a20 2020 2020 2020 2020  e_2>',.         
+000005c0: 2020 2020 2020 2027 7061 7468 273a 2027         'path': '
+000005d0: 3c70 6174 685f 746f 5f67 656e 6572 6174  <path_to_generat
+000005e0: 6564 5f61 7069 5f64 6f63 5f32 3e27 0a20  ed_api_doc_2>'. 
+000005f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000600: 2020 2020 2020 2020 2020 2320 2e2e 2e0a            # ....
+00000610: 2020 2020 2020 2020 5d0a 2020 7d2c 0a20          ].  },. 
+00000620: 207b 0a20 2020 2027 636f 6d6d 616e 6427   {.    'command'
+00000630: 3a20 273c 796f 7572 5f63 7573 746f 6d5f  : '<your_custom_
+00000640: 6275 696c 645f 636f 6d6d 616e 645f 323e  build_command_2>
+00000650: 272c 0a20 2020 2027 6f75 7470 7574 7327  ',.    'outputs'
+00000660: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00000670: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000680: 2020 276e 616d 6527 3a20 273c 6765 6e65    'name': '<gene
+00000690: 7261 7465 645f 6170 695f 646f 635f 6e61  rated_api_doc_na
+000006a0: 6d65 5f33 3e27 2c0a 2020 2020 2020 2020  me_3>',.        
+000006b0: 2020 2020 2020 2020 2770 6174 6827 3a20          'path': 
+000006c0: 273c 7061 7468 5f74 6f5f 6765 6e65 7261  '<path_to_genera
+000006d0: 7465 645f 6170 695f 646f 635f 333e 270a  ted_api_doc_3>'.
+000006e0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000006f0: 2020 2020 2020 2020 2020 2023 202e 2e2e             # ...
+00000700: 0a20 2020 2020 2020 205d 0a20 207d 2c0a  .        ].  },.
+00000710: 2020 2320 6d6f 7265 2067 726f 7570 7320    # more groups 
+00000720: 6f66 2067 656e 6572 6174 6564 2061 7069  of generated api
+00000730: 2064 6f63 730a 5d0a 6060 600a 0a52 6570   docs.].```..Rep
+00000740: 6c61 6365 2060 3c79 6f75 725f 6375 7374  lace `<your_cust
+00000750: 6f6d 5f62 7569 6c64 5f63 6f6d 6d61 6e64  om_build_command
+00000760: 5f2a 3e60 2c20 603c 6765 6e65 7261 7465  _*>`, `<generate
+00000770: 645f 6170 695f 646f 635f 6e61 6d65 5f2a  d_api_doc_name_*
+00000780: 3e60 2c20 616e 6420 603c 7061 7468 5f74  >`, and `<path_t
+00000790: 6f5f 6765 6e65 7261 7465 645f 6170 695f  o_generated_api_
+000007a0: 646f 635f 2a3e 6020 7769 7468 2074 6865  doc_*>` with the
+000007b0: 2061 7070 726f 7072 6961 7465 2076 616c   appropriate val
+000007c0: 7565 7320 666f 7220 796f 7572 2070 726f  ues for your pro
+000007d0: 6a65 6374 2e0a 0a33 2e20 5570 6461 7465  ject...3. Update
+000007e0: 2079 6f75 7220 6063 6f6e 662e 7079 6020   your `conf.py` 
+000007f0: 6669 6c65 2074 6f20 696e 636c 7564 6520  file to include 
+00000800: 7468 6520 6061 7069 5f64 6f63 735f 7369  the `api_docs_si
+00000810: 6465 6261 722e 6874 6d6c 6020 7465 6d70  debar.html` temp
+00000820: 6c61 7465 2069 6e20 7468 6520 6874 6d6c  late in the html
+00000830: 5f73 6964 6562 6172 7320 636f 6e66 6967  _sidebars config
+00000840: 7572 6174 696f 6e3a 0a0a 6060 6070 7974  uration:..```pyt
+00000850: 686f 6e0a 6874 6d6c 5f73 6964 6562 6172  hon.html_sidebar
+00000860: 7320 3d20 7b0a 2020 2020 272a 2a27 3a20  s = {.    '**': 
+00000870: 5b0a 2020 2020 2020 2020 2320 2e2e 2e20  [.        # ... 
+00000880: 6f74 6865 7220 7369 6465 6261 7273 202e  other sidebars .
+00000890: 2e2e 0a20 2020 2020 2020 2027 7369 6465  ...        'side
+000008a0: 6261 722f 6170 695f 646f 6373 5f73 6964  bar/api_docs_sid
+000008b0: 6562 6172 2e68 746d 6c27 2c0a 2020 2020  ebar.html',.    
+000008c0: 5d0a 7d0a 6060 600a                      ].}.```.
```

### Comparing `sphinx_api_sidebar-0.1.1/setup.py` & `sphinx_api_sidebar-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
-    name='sphinx_api_sidebar',
-    description='Display any generated static API documentation in a sidebar',
-    version='0.1.0',
-    author='Yiheng Xiong',
-    author_email='georgex8866@gmail.com',
-    url='https://github.com/Yihengxiong6/sphinx_api_sidebar',
-    packages=['sphinx_api_sidebar'],
+    name="sphinx_api_sidebar",
+    description="Display any generated static API documentation in a sidebar",
+    version="0.1.2",
+    author="Yiheng Xiong",
+    author_email="georgex8866@gmail.com",
+    url="https://github.com/Yihengxiong6/sphinx_api_sidebar",
+    packages=["sphinx_api_sidebar"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10"
-    ],
-    install_requires=[
-        "sphinx >= 2.1"
+        "Programming Language :: Python :: 3.10",
     ],
+    install_requires=["sphinx >= 2.1"],
     entry_points={
-        'sphinx.extensions': [
-            'sphinx_api_sidebar = sphinx_api_sidebar:setup'
-        ]
-    }
+        "sphinx.extensions": ["sphinx_api_sidebar = sphinx_api_sidebar:setup"]
+    },
 )
-
```

### Comparing `sphinx_api_sidebar-0.1.1/sphinx_api_sidebar.egg-info/PKG-INFO` & `sphinx_api_sidebar-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sphinx-api-sidebar
-Version: 0.1.1
+Name: sphinx_api_sidebar
+Version: 0.1.2
 Summary: Display any generated static API documentation in a sidebar
 Home-page: https://github.com/Yihengxiong6/sphinx_api_sidebar
 Author: Yiheng Xiong
 Author-email: Yiheng Xiong <georgex8866@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yiheng Xiong
@@ -31,25 +31,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Sphinx API Sidebar
 
 A Sphinx extension for displaying any generated static API documentation in a sidebar.
 
 ## Overview
 
-This Sphinx extension allows you to include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used in the API sidebar template.
+This Sphinx extension allows you to include and display static API documentation (e.g., `JavaDoc`, `Doxygen`) in the sidebar of your Sphinx documentation. It updates the `html_context` with the API documentation paths, which can then be used to render the API documentation sidebar template.
 
-This extension serves as an immediate workaround to make Sphinx consume API docs from various languages without building additional extensions.
+This extension serves as an immediate workaround to make Sphinx consume API docs in HTML format from various languages without building additional deeply integrated extensions for each type of API docs.
 
 ## Installation
 
 To install the `sphinx-api-sidebar` extension, you can use pip:
 
 ```sh
 pip install sphinx-api-sidebar
@@ -61,15 +62,15 @@
 ```python
 extensions = [
     'sphinx_api_sidebar',
     # Other extensions...
 ]
 ```
 
-2. To use a custom command to generate your API documentation or specify different directories, you can set the api_docs_generator configuration value in your conf.py file:
+2. To use a custom command to generate your API documentation or specify different directories, you can set the `api_docs_generators` configuration value in your conf.py file:
 
 ```python
 api_docs_generators = [
   {
     'command': '<your_api_docs_build_command_1>',
     'outputs': [
             {
@@ -93,33 +94,19 @@
             # ...
         ]
   },
   # more groups of generated api docs
 ]
 ```
 
-Replace <your_custom_build_command_*>, <generated_api_doc_name_*>, and <path_to_generated_api_doc_*> with the appropriate values for your project.
+Replace `<your_custom_build_command_*>`, `<generated_api_doc_name_*>`, and `<path_to_generated_api_doc_*>` with the appropriate values for your project.
 
-
-3. To make the different api documentation show up in the sidebar, you will need to copy the `api_docs_sidebar.html` template file from the `sphinx_api_sidebar/templates` folder of the installed package to your Sphinx project's _templates folder. Alternatively, you can create a new file in your project's _templates folder with the following content:
-
-```html
-{% if api_docs %}
-  <h3>{{ _('API Documentation') }}</h3>
-  <ul style="list-style-type: none;">
-    {%- for item in api_docs %}
-      <li style="margin-bottom: 10px;"><a href="{{ pathto('_static/api-docs/{}'.format(item), 1) }}">{{ item }}</a></li>
-    {%- endfor %}
-  </ul>
-{% endif %}
-```
-
-4. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
+3. Update your `conf.py` file to include the `api_docs_sidebar.html` template in the html_sidebars configuration:
 
 ```python
 html_sidebars = {
     '**': [
         # ... other sidebars ...
-        'api_docs_sidebar.html',
+        'sidebar/api_docs_sidebar.html',
     ]
 }
 ```
```

### Comparing `sphinx_api_sidebar-0.1.1/tests/test_sphinx_api_sidebar.py` & `sphinx_api_sidebar-0.1.2/tests/test_sphinx_api_sidebar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import unittest
+
 from sphinx_api_sidebar.sphinx_api_sidebar import update_html_context
 
-class TestSphinxApiSidebar(unittest.TestCase):
 
+class TestSphinxApiSidebar(unittest.TestCase):
     def test_update_html_context(self):
-        config = type('', (), {})()  # Create a simple object to act as the config
+        config = type("", (), {})()  # Create a simple object to act as the config
         config.html_context = {}
 
         api_docs = ["project1", "project2"]
 
         update_html_context(config, api_docs)
 
         self.assertIn("api_docs", config.html_context)
         self.assertEqual(api_docs, config.html_context["api_docs"])
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

