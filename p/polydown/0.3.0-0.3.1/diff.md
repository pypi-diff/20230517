# Comparing `tmp/polydown-0.3.0.tar.gz` & `tmp/polydown-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polydown-0.3.0.tar", max compression
+gzip compressed data, was "polydown-0.3.1.tar", max compression
```

## Comparing `polydown-0.3.0.tar` & `polydown-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2023-01-27 19:32:31.295859 polydown-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2021-09-23 21:54:13.843999 polydown-0.3.0/polydown/__init__.py
--rw-r--r--   0        0        0     2010 2023-05-11 14:10:10.003943 polydown-0.3.0/polydown/__main__.py
--rw-r--r--   0        0        0     2586 2023-05-11 14:11:31.005921 polydown-0.3.0/polydown/cli.py
--rw-r--r--   0        0        0     5590 2023-05-11 14:30:31.183437 polydown-0.3.0/polydown/downloader.py
--rw-r--r--   0        0        0      617 2021-09-26 12:56:04.492884 polydown-0.3.0/polydown/hash_check.py
--rw-r--r--   0        0        0     6037 2023-05-11 14:24:28.458577 polydown-0.3.0/polydown/poly.py
--rw-r--r--   0        0        0     1137 2021-09-26 10:09:00.959542 polydown-0.3.0/polydown/report.py
--rw-r--r--   0        0        0      760 2021-09-26 10:41:14.957821 polydown-0.3.0/polydown/theme.py
--rw-r--r--   0        0        0     1113 2023-05-11 14:18:35.348630 polydown-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2701 2021-10-01 08:53:42.097440 polydown-0.3.0/README.MD
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 polydown-0.3.0/setup.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 polydown-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-27 19:32:31.295859 polydown-0.3.1/LICENSE
+-rw-r--r--   0        0        0        0 2021-09-23 21:54:13.843999 polydown-0.3.1/polydown/__init__.py
+-rw-r--r--   0        0        0     2010 2023-05-11 14:10:10.003943 polydown-0.3.1/polydown/__main__.py
+-rw-r--r--   0        0        0     2586 2023-05-11 14:11:31.005921 polydown-0.3.1/polydown/cli.py
+-rw-r--r--   0        0        0     5590 2023-05-17 19:00:50.214981 polydown-0.3.1/polydown/downloader.py
+-rw-r--r--   0        0        0      617 2021-09-26 12:56:04.492884 polydown-0.3.1/polydown/hash_check.py
+-rw-r--r--   0        0        0     6113 2023-05-17 19:00:46.223826 polydown-0.3.1/polydown/poly.py
+-rw-r--r--   0        0        0     1137 2021-09-26 10:09:00.959542 polydown-0.3.1/polydown/report.py
+-rw-r--r--   0        0        0      760 2021-09-26 10:41:14.957821 polydown-0.3.1/polydown/theme.py
+-rw-r--r--   0        0        0     1113 2023-05-17 18:59:11.731350 polydown-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2786 2023-05-11 14:35:34.316063 polydown-0.3.1/README.MD
+-rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 polydown-0.3.1/setup.py
+-rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 polydown-0.3.1/PKG-INFO
```

### Comparing `polydown-0.3.0/LICENSE` & `polydown-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/__main__.py` & `polydown-0.3.1/polydown/__main__.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/cli.py` & `polydown-0.3.1/polydown/cli.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/downloader.py` & `polydown-0.3.1/polydown/downloader.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/hash_check.py` & `polydown-0.3.1/polydown/hash_check.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/poly.py` & `polydown-0.3.1/polydown/poly.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                         self.type,
                         asset,
                         self.s,
                         self.down_folder,
                         self.subfolder,
                         filename,
                         self.overwrite,
+                        self.tone,
                         bl_url,
                         bl_md5,
                         k,
                         True,
                     )
                     dw = Downloader(*args)
                     d = dw.file()
@@ -104,14 +105,15 @@
                             self.type,
                             asset,
                             self.s,
                             self.down_folder,
                             self.subfolder,
                             filename,
                             self.overwrite,
+                            self.tone,
                             url,
                             md5,
                             k,
                             False,
                         )
                         dw = Downloader(*args)
                         d = dw.file()
```

### Comparing `polydown-0.3.0/polydown/report.py` & `polydown-0.3.1/polydown/report.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/polydown/theme.py` & `polydown-0.3.1/polydown/theme.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.0/pyproject.toml` & `polydown-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polydown"
-version = "0.3.0"
+version = "0.3.1"
 description = "Batch downloader for polyhaven (polyhaven.com)"
 authors = ["Gökçe Merdun <agmmnn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/agmmnn/polydown"
 repository = "https://github.com/agmmnn/polydown"
 keywords = ["polyhaven", "download", "downloader", "scrape", "hdri", "batch"]
```

### Comparing `polydown-0.3.0/README.MD` & `polydown-0.3.1/README.MD`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,94 @@
 ![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
+
 <div align="center">
 <a href="https://github.com/agmmnn/polydown">
 <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>
 <a href="https://pypi.org/project/polydown/">
 <img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>
 
 Batch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven's [Public API](https://github.com/Poly-Haven/Public-API).
+
 </div>
 
 # Installation
 
-- `pip install polydown`
+```
+pip install polydown
+```
 
 # How to Use
+
 ```
 $ polydown hdris
 
 # download all available sizes of all hdris into current folder.
 > 🔗(polyhaven.com/hdris['all sizes'])=>🏠
 ```
+
 ```
 $ polydown <asset_type>
 
 # download all assets of this asset type to the current folder in all available sizes.
 # asset types: "hdris", "textures", "models".
 ```
+
 ```
 $ polydown textures -c
 
 # list of category in the given asset type.
 ```
+
 ```
 $ polydown hdris -f hdris_down -s 2k 4k
 
 # download all hdris with given sizes into "hdris_down" folder.
 # /if there is no such folder it will create it./
 > 🔗(polyhaven.com/hdris['2k', '4k'])=>🏠(hdris_down)
 ```
+
 ## Example Usage
 
 ```
 $ polydown models -c decorative -f folder -s 1k
 
 # download all "models" with "1k textures" in the "decorative" category into the "folder".
 ```
+
 ![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)
+
 ![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)
 
 # Arguments:
 
 ```
 <asset_type>      "hdris, textures, models"
 -h, --help        show this help message and exit
 -f, --folder      target download folder.
 -c, --category    category to download.
 -s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
 -o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
 -no, --noimgs     do not download 'preview, render, thumbnail...' images.
 -it, --iters      amount of iterations.
+-t, --tone        Download 8K Tonemapped JPG (only HDRIs).
 -v, --version     show program's version number and exit
 ```
 
 # To-Do
--   [ ] Unit Tests
--   [ ] Progressbar for current download task(s)
--   [ ] Select the file format to download
--   [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
+
+- [ ] Unit Tests
+- [ ] Progressbar for current download task(s)
+- [ ] Select the file format to download
+- [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
 
 # Requirements
-- Python >3.5
+
+- Python>3.7
 
 ## Dependencies
+
 - [requests](https://pypi.org/project/requests/)
 - [rich](https://github.com/willmcgugan/rich)
 
 # License
-[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
+
+[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 ![screenshot](https://user-images.githubusercontent.com/16024979/134770914-
 bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
  [GitHub_release_(latest_by_date)] [PyPI] Batch downloader for [polyhaven.com]
 (https://polyhaven.com/). Download hdris, textures and models in any sizes you
   want. This project uses Poly Haven's [Public API](https://github.com/Poly-
                               Haven/Public-API).
-# Installation - `pip install polydown` # How to Use ``` $ polydown hdris #
+# Installation ``` pip install polydown ``` # How to Use ``` $ polydown hdris #
 download all available sizes of all hdris into current folder. > ð
 (polyhaven.com/hdris['all sizes'])=>ð  ``` ``` $ polydown  # download all
 assets of this asset type to the current folder in all available sizes. # asset
 types: "hdris", "textures", "models". ``` ``` $ polydown textures -c # list of
 category in the given asset type. ``` ``` $ polydown hdris -f hdris_down -s 2k
 4k # download all hdris with given sizes into "hdris_down" folder. # /if there
 is no such folder it will create it./ > ð(polyhaven.com/hdris['2k',
@@ -19,14 +19,14 @@
 c52b3cfcf8a2.png) ![file structure](https://user-images.githubusercontent.com/
 16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png) # Arguments: ```
 "hdris, textures, models" -h, --help show this help message and exit -f, --
 folder target download folder. -c, --category category to download. -s, --sizes
 size(s) of downloaded asset files. eg: 1k 2k 4k -o, --overwrite overwrite if
 the files already exists. otherwise the current task will be skipped. -no, --
 noimgs do not download 'preview, render, thumbnail...' images. -it, --iters
-amount of iterations. -v, --version show program's version number and exit ```
-# To-Do - [ ] Unit Tests - [ ] Progressbar for current download task(s) - [ ]
-Select the file format to download - [ ] Download a specific asset, "polydown
-hdris stuttgart_suburbs" # Requirements - Python >3.5 ## Dependencies -
-[requests](https://pypi.org/project/requests/) - [rich](https://github.com/
-willmcgugan/rich) # License [MIT](https://github.com/agmmnn/polydown/blob/
-master/LICENSE)
+amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -v, -
+-version show program's version number and exit ``` # To-Do - [ ] Unit Tests -
+[ ] Progressbar for current download task(s) - [ ] Select the file format to
+download - [ ] Download a specific asset, "polydown hdris stuttgart_suburbs" #
+Requirements - Python>3.7 ## Dependencies - [requests](https://pypi.org/
+project/requests/) - [rich](https://github.com/willmcgugan/rich) # License
+[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
```

### Comparing `polydown-0.3.0/setup.py` & `polydown-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['aiohttp>=3.8.3,<4.0.0', 'requests>=2.30.0,<3.0.0', 'rich>=13.3.0,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['polydown = polydown.__main__:cli']}
 
 setup_kwargs = {
     'name': 'polydown',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Batch downloader for polyhaven (polyhaven.com)',
-    'long_description': '![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)\n<div align="center">\n<a href="https://github.com/agmmnn/polydown">\n<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>\n<a href="https://pypi.org/project/polydown/">\n<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>\n\nBatch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven\'s [Public API](https://github.com/Poly-Haven/Public-API).\n</div>\n\n# Installation\n\n- `pip install polydown`\n\n# How to Use\n```\n$ polydown hdris\n\n# download all available sizes of all hdris into current folder.\n> 🔗(polyhaven.com/hdris[\'all sizes\'])=>🏠\n```\n```\n$ polydown <asset_type>\n\n# download all assets of this asset type to the current folder in all available sizes.\n# asset types: "hdris", "textures", "models".\n```\n```\n$ polydown textures -c\n\n# list of category in the given asset type.\n```\n```\n$ polydown hdris -f hdris_down -s 2k 4k\n\n# download all hdris with given sizes into "hdris_down" folder.\n# /if there is no such folder it will create it./\n> 🔗(polyhaven.com/hdris[\'2k\', \'4k\'])=>🏠(hdris_down)\n```\n## Example Usage\n\n```\n$ polydown models -c decorative -f folder -s 1k\n\n# download all "models" with "1k textures" in the "decorative" category into the "folder".\n```\n![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)\n![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)\n\n# Arguments:\n\n```\n<asset_type>      "hdris, textures, models"\n-h, --help        show this help message and exit\n-f, --folder      target download folder.\n-c, --category    category to download.\n-s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k\n-o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.\n-no, --noimgs     do not download \'preview, render, thumbnail...\' images.\n-it, --iters      amount of iterations.\n-v, --version     show program\'s version number and exit\n```\n\n# To-Do\n-   [ ] Unit Tests\n-   [ ] Progressbar for current download task(s)\n-   [ ] Select the file format to download\n-   [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"\n\n# Requirements\n- Python >3.5\n\n## Dependencies\n- [requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/willmcgugan/rich)\n\n# License\n[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)',
+    'long_description': '![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)\n\n<div align="center">\n<a href="https://github.com/agmmnn/polydown">\n<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>\n<a href="https://pypi.org/project/polydown/">\n<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>\n\nBatch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven\'s [Public API](https://github.com/Poly-Haven/Public-API).\n\n</div>\n\n# Installation\n\n```\npip install polydown\n```\n\n# How to Use\n\n```\n$ polydown hdris\n\n# download all available sizes of all hdris into current folder.\n> 🔗(polyhaven.com/hdris[\'all sizes\'])=>🏠\n```\n\n```\n$ polydown <asset_type>\n\n# download all assets of this asset type to the current folder in all available sizes.\n# asset types: "hdris", "textures", "models".\n```\n\n```\n$ polydown textures -c\n\n# list of category in the given asset type.\n```\n\n```\n$ polydown hdris -f hdris_down -s 2k 4k\n\n# download all hdris with given sizes into "hdris_down" folder.\n# /if there is no such folder it will create it./\n> 🔗(polyhaven.com/hdris[\'2k\', \'4k\'])=>🏠(hdris_down)\n```\n\n## Example Usage\n\n```\n$ polydown models -c decorative -f folder -s 1k\n\n# download all "models" with "1k textures" in the "decorative" category into the "folder".\n```\n\n![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)\n\n![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)\n\n# Arguments:\n\n```\n<asset_type>      "hdris, textures, models"\n-h, --help        show this help message and exit\n-f, --folder      target download folder.\n-c, --category    category to download.\n-s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k\n-o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.\n-no, --noimgs     do not download \'preview, render, thumbnail...\' images.\n-it, --iters      amount of iterations.\n-t, --tone        Download 8K Tonemapped JPG (only HDRIs).\n-v, --version     show program\'s version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n- [ ] Progressbar for current download task(s)\n- [ ] Select the file format to download\n- [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"\n\n# Requirements\n\n- Python>3.7\n\n## Dependencies\n\n- [requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/willmcgugan/rich)\n\n# License\n\n[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)\n',
     'author': 'Gökçe Merdun',
     'author_email': 'agmmnn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/agmmnn/polydown',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,43 +1,45 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['polydown']
 package_data = \ {'': ['*']} install_requires = \ ['aiohttp>=3.8.3,<4.0.0',
 'requests>=2.30.0,<3.0.0', 'rich>=13.3.0,<14.0.0'] entry_points = \
 {'console_scripts': ['polydown = polydown.__main__:cli']} setup_kwargs =
-{ 'name': 'polydown', 'version': '0.3.0', 'description': 'Batch downloader for
+{ 'name': 'polydown', 'version': '0.3.1', 'description': 'Batch downloader for
 polyhaven (polyhaven.com)', 'long_description': '![screenshot](https://user-
 images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-
-9d189379d307.gif)\n
+9d189379d307.gif)\n\n
    \n\n[GitHub_release_(latest_by_date)]\n\n[PyPI]\n\nBatch downloader for
 [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in
    any sizes you want. This project uses Poly Haven\'s [Public API](https://
-                     github.com/Poly-Haven/Public-API).\n
-\n\n# Installation\n\n- `pip install polydown`\n\n# How to Use\n```\n$ polydown
-hdris\n\n# download all available sizes of all hdris into current folder.\n>
-ð(polyhaven.com/hdris[\'all sizes\'])=>ð \n```\n```\n$ polydown \n\n#
-download all assets of this asset type to the current folder in all available
-sizes.\n# asset types: "hdris", "textures", "models".\n```\n```\n$ polydown
-textures -c\n\n# list of category in the given asset type.\n```\n```\n$
-polydown hdris -f hdris_down -s 2k 4k\n\n# download all hdris with given sizes
-into "hdris_down" folder.\n# /if there is no such folder it will create it./\n>
-ð(polyhaven.com/hdris[\'2k\', \'4k\'])=>ð (hdris_down)\n```\n## Example
-Usage\n\n```\n$ polydown models -c decorative -f folder -s 1k\n\n# download all
-"models" with "1k textures" in the "decorative" category into the
-"folder".\n```\n![screenshot](https://user-images.githubusercontent.com/
-16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)\n![file structure]
-(https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-
-4acb-9394-dac08352efee.png)\n\n# Arguments:\n\n```\n "hdris, textures,
-models"\n-h, --help show this help message and exit\n-f, --folder target
-download folder.\n-c, --category category to download.\n-s, --sizes size(s) of
-downloaded asset files. eg: 1k 2k 4k\n-o, --overwrite overwrite if the files
-already exists. otherwise the current task will be skipped.\n-no, --noimgs do
-not download \'preview, render, thumbnail...\' images.\n-it, --iters amount of
-iterations.\n-v, --version show program\'s version number and exit\n```\n\n#
-To-Do\n- [ ] Unit Tests\n- [ ] Progressbar for current download task(s)\n- [ ]
-Select the file format to download\n- [ ] Download a specific asset, "polydown
-hdris stuttgart_suburbs"\n\n# Requirements\n- Python >3.5\n\n## Dependencies\n-
+                    github.com/Poly-Haven/Public-API).\n\n
+\n\n# Installation\n\n```\npip install polydown\n```\n\n# How to Use\n\n```\n$
+polydown hdris\n\n# download all available sizes of all hdris into current
+folder.\n> ð(polyhaven.com/hdris[\'all sizes\'])=>ð \n```\n\n```\n$
+polydown \n\n# download all assets of this asset type to the current folder in
+all available sizes.\n# asset types: "hdris", "textures",
+"models".\n```\n\n```\n$ polydown textures -c\n\n# list of category in the
+given asset type.\n```\n\n```\n$ polydown hdris -f hdris_down -s 2k 4k\n\n#
+download all hdris with given sizes into "hdris_down" folder.\n# /if there is
+no such folder it will create it./\n> ð(polyhaven.com/hdris[\'2k\',
+\'4k\'])=>ð (hdris_down)\n```\n\n## Example Usage\n\n```\n$ polydown models -
+c decorative -f folder -s 1k\n\n# download all "models" with "1k textures" in
+the "decorative" category into the "folder".\n```\n\n![screenshot](https://
+user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-
+c52b3cfcf8a2.png)\n\n![file structure](https://user-
+images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-
+dac08352efee.png)\n\n# Arguments:\n\n```\n "hdris, textures, models"\n-h, --
+help show this help message and exit\n-f, --folder target download folder.\n-c,
+--category category to download.\n-s, --sizes size(s) of downloaded asset
+files. eg: 1k 2k 4k\n-o, --overwrite overwrite if the files already exists.
+otherwise the current task will be skipped.\n-no, --noimgs do not download
+\'preview, render, thumbnail...\' images.\n-it, --iters amount of
+iterations.\n-t, --tone Download 8K Tonemapped JPG (only HDRIs).\n-v, --version
+show program\'s version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n-
+[ ] Progressbar for current download task(s)\n- [ ] Select the file format to
+download\n- [ ] Download a specific asset, "polydown hdris
+stuttgart_suburbs"\n\n# Requirements\n\n- Python>3.7\n\n## Dependencies\n\n-
 [requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/
-willmcgugan/rich)\n\n# License\n[MIT](https://github.com/agmmnn/polydown/blob/
-master/LICENSE)', 'author': 'GÃ¶kÃ§e Merdun', 'author_email':
+willmcgugan/rich)\n\n# License\n\n[MIT](https://github.com/agmmnn/polydown/
+blob/master/LICENSE)\n', 'author': 'GÃ¶kÃ§e Merdun', 'author_email':
 'agmmnn@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'https://github.com/agmmnn/polydown', 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
 entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `polydown-0.3.0/PKG-INFO` & `polydown-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polydown
-Version: 0.3.0
+Version: 0.3.1
 Summary: Batch downloader for polyhaven (polyhaven.com)
 Home-page: https://github.com/agmmnn/polydown
 License: MIT
 Keywords: polyhaven,download,downloader,scrape,hdri,batch
 Author: Gökçe Merdun
 Author-email: agmmnn@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -25,84 +25,101 @@
 Project-URL: Bug Tracker, https://github.com/agmmnn/polydown/issues
 Project-URL: Changelog, https://github.com/agmmnn/polydown/releases
 Project-URL: Repository, https://github.com/agmmnn/polydown
 Project-URL: Source, https://github.com/agmmnn/polydown
 Description-Content-Type: text/markdown
 
 ![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
+
 <div align="center">
 <a href="https://github.com/agmmnn/polydown">
 <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>
 <a href="https://pypi.org/project/polydown/">
 <img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>
 
 Batch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven's [Public API](https://github.com/Poly-Haven/Public-API).
+
 </div>
 
 # Installation
 
-- `pip install polydown`
+```
+pip install polydown
+```
 
 # How to Use
+
 ```
 $ polydown hdris
 
 # download all available sizes of all hdris into current folder.
 > 🔗(polyhaven.com/hdris['all sizes'])=>🏠
 ```
+
 ```
 $ polydown <asset_type>
 
 # download all assets of this asset type to the current folder in all available sizes.
 # asset types: "hdris", "textures", "models".
 ```
+
 ```
 $ polydown textures -c
 
 # list of category in the given asset type.
 ```
+
 ```
 $ polydown hdris -f hdris_down -s 2k 4k
 
 # download all hdris with given sizes into "hdris_down" folder.
 # /if there is no such folder it will create it./
 > 🔗(polyhaven.com/hdris['2k', '4k'])=>🏠(hdris_down)
 ```
+
 ## Example Usage
 
 ```
 $ polydown models -c decorative -f folder -s 1k
 
 # download all "models" with "1k textures" in the "decorative" category into the "folder".
 ```
+
 ![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)
+
 ![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)
 
 # Arguments:
 
 ```
 <asset_type>      "hdris, textures, models"
 -h, --help        show this help message and exit
 -f, --folder      target download folder.
 -c, --category    category to download.
 -s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
 -o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
 -no, --noimgs     do not download 'preview, render, thumbnail...' images.
 -it, --iters      amount of iterations.
+-t, --tone        Download 8K Tonemapped JPG (only HDRIs).
 -v, --version     show program's version number and exit
 ```
 
 # To-Do
--   [ ] Unit Tests
--   [ ] Progressbar for current download task(s)
--   [ ] Select the file format to download
--   [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
+
+- [ ] Unit Tests
+- [ ] Progressbar for current download task(s)
+- [ ] Select the file format to download
+- [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"
 
 # Requirements
-- Python >3.5
+
+- Python>3.7
 
 ## Dependencies
+
 - [requests](https://pypi.org/project/requests/)
 - [rich](https://github.com/willmcgugan/rich)
 
 # License
+
 [MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polydown Version: 0.3.0 Summary: Batch downloader
+Metadata-Version: 2.1 Name: polydown Version: 0.3.1 Summary: Batch downloader
 for polyhaven (polyhaven.com) Home-page: https://github.com/agmmnn/polydown
 License: MIT Keywords: polyhaven,download,downloader,scrape,hdri,batch Author:
 GÃ¶kÃ§e Merdun Author-email: agmmnn@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -16,15 +16,15 @@
 URL: Source, https://github.com/agmmnn/polydown Description-Content-Type: text/
 markdown ![screenshot](https://user-images.githubusercontent.com/16024979/
 134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)
  [GitHub_release_(latest_by_date)] [PyPI] Batch downloader for [polyhaven.com]
 (https://polyhaven.com/). Download hdris, textures and models in any sizes you
   want. This project uses Poly Haven's [Public API](https://github.com/Poly-
                               Haven/Public-API).
-# Installation - `pip install polydown` # How to Use ``` $ polydown hdris #
+# Installation ``` pip install polydown ``` # How to Use ``` $ polydown hdris #
 download all available sizes of all hdris into current folder. > ð
 (polyhaven.com/hdris['all sizes'])=>ð  ``` ``` $ polydown  # download all
 assets of this asset type to the current folder in all available sizes. # asset
 types: "hdris", "textures", "models". ``` ``` $ polydown textures -c # list of
 category in the given asset type. ``` ``` $ polydown hdris -f hdris_down -s 2k
 4k # download all hdris with given sizes into "hdris_down" folder. # /if there
 is no such folder it will create it./ > ð(polyhaven.com/hdris['2k',
@@ -35,14 +35,14 @@
 c52b3cfcf8a2.png) ![file structure](https://user-images.githubusercontent.com/
 16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png) # Arguments: ```
 "hdris, textures, models" -h, --help show this help message and exit -f, --
 folder target download folder. -c, --category category to download. -s, --sizes
 size(s) of downloaded asset files. eg: 1k 2k 4k -o, --overwrite overwrite if
 the files already exists. otherwise the current task will be skipped. -no, --
 noimgs do not download 'preview, render, thumbnail...' images. -it, --iters
-amount of iterations. -v, --version show program's version number and exit ```
-# To-Do - [ ] Unit Tests - [ ] Progressbar for current download task(s) - [ ]
-Select the file format to download - [ ] Download a specific asset, "polydown
-hdris stuttgart_suburbs" # Requirements - Python >3.5 ## Dependencies -
-[requests](https://pypi.org/project/requests/) - [rich](https://github.com/
-willmcgugan/rich) # License [MIT](https://github.com/agmmnn/polydown/blob/
-master/LICENSE)
+amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -v, -
+-version show program's version number and exit ``` # To-Do - [ ] Unit Tests -
+[ ] Progressbar for current download task(s) - [ ] Select the file format to
+download - [ ] Download a specific asset, "polydown hdris stuttgart_suburbs" #
+Requirements - Python>3.7 ## Dependencies - [requests](https://pypi.org/
+project/requests/) - [rich](https://github.com/willmcgugan/rich) # License
+[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
```

