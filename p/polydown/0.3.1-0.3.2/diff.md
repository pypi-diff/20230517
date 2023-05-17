# Comparing `tmp/polydown-0.3.1.tar.gz` & `tmp/polydown-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polydown-0.3.1.tar", max compression
+gzip compressed data, was "polydown-0.3.2.tar", max compression
```

## Comparing `polydown-0.3.1.tar` & `polydown-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1084 2023-01-27 19:32:31.295859 polydown-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2021-09-23 21:54:13.843999 polydown-0.3.1/polydown/__init__.py
--rw-r--r--   0        0        0     2010 2023-05-11 14:10:10.003943 polydown-0.3.1/polydown/__main__.py
--rw-r--r--   0        0        0     2586 2023-05-11 14:11:31.005921 polydown-0.3.1/polydown/cli.py
--rw-r--r--   0        0        0     5590 2023-05-17 19:00:50.214981 polydown-0.3.1/polydown/downloader.py
--rw-r--r--   0        0        0      617 2021-09-26 12:56:04.492884 polydown-0.3.1/polydown/hash_check.py
--rw-r--r--   0        0        0     6113 2023-05-17 19:00:46.223826 polydown-0.3.1/polydown/poly.py
--rw-r--r--   0        0        0     1137 2021-09-26 10:09:00.959542 polydown-0.3.1/polydown/report.py
--rw-r--r--   0        0        0      760 2021-09-26 10:41:14.957821 polydown-0.3.1/polydown/theme.py
--rw-r--r--   0        0        0     1113 2023-05-17 18:59:11.731350 polydown-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2786 2023-05-11 14:35:34.316063 polydown-0.3.1/README.MD
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 polydown-0.3.1/setup.py
--rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 polydown-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-01-27 19:32:31.295859 polydown-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2021-09-23 21:54:13.843999 polydown-0.3.2/polydown/__init__.py
+-rw-r--r--   0        0        0     2025 2023-05-17 19:33:22.106099 polydown-0.3.2/polydown/__main__.py
+-rw-r--r--   0        0        0     2671 2023-05-17 19:29:03.655687 polydown-0.3.2/polydown/cli.py
+-rw-r--r--   0        0        0     5652 2023-05-17 19:20:42.852352 polydown-0.3.2/polydown/downloader.py
+-rw-r--r--   0        0        0      617 2021-09-26 12:56:04.492884 polydown-0.3.2/polydown/hash_check.py
+-rw-r--r--   0        0        0     6328 2023-05-17 19:22:36.993028 polydown-0.3.2/polydown/poly.py
+-rw-r--r--   0        0        0     1137 2021-09-26 10:09:00.959542 polydown-0.3.2/polydown/report.py
+-rw-r--r--   0        0        0      760 2021-09-26 10:41:14.957821 polydown-0.3.2/polydown/theme.py
+-rw-r--r--   0        0        0     1113 2023-05-17 19:24:43.301574 polydown-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2839 2023-05-17 19:29:27.002167 polydown-0.3.2/README.MD
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 polydown-0.3.2/setup.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 polydown-0.3.2/PKG-INFO
```

### Comparing `polydown-0.3.1/LICENSE` & `polydown-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polydown-0.3.1/polydown/__main__.py` & `polydown-0.3.2/polydown/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import datetime
 from .cli import polycli
 
-__version__ = "0.2.2"
+__version__ = "0.3.2"
 
 ap = argparse.ArgumentParser()
 ap.add_argument(
     "asset_type",
     type=str,
     nargs="*",
     help='"hdris, textures, models"',
@@ -37,21 +37,22 @@
     "-it",
     "--iters",
     action="store",
     type=int,
     default=-1,
     help="amount of iterations.",
 )
-# ap.add_argument(
-#     "-ff",
-#     "--file_format",
-#     action="store",
-#     type=str,
-#     help="target download folder.",
-# )
+ap.add_argument(
+    "-ff",
+    "--fileformat",
+    action="store",
+    type=str,
+    default="hdr",
+    help="file format for hdris (hdr, exr).",
+)
 ap.add_argument(
     "-o",
     "--overwrite",
     action="store_true",
     default=False,
     help="Overwrite if the files already exists.  otherwise the current task will be skipped.",
 )
```

### Comparing `polydown-0.3.1/polydown/cli.py` & `polydown-0.3.2/polydown/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     folder = args.folder
     overwrite = args.overwrite
     sizes = args.sizes
     category = args.category
     noimgs = args.noimgs
     iters = args.iters
     tone = args.tone
+    fileformat = args.fileformat
     s = requests.Session()
 
     # ->🔒asset type->
     asset_type_list = list(json.loads(s.get("https://api.polyhaven.com/types").content))
     if asset_type not in asset_type_list:
         print(f"'{asset_type}' is not a valid asset type!")
         exit()
@@ -41,25 +42,23 @@
         if category not in asset_category_list:
             print(
                 f"[red]{category} is not a valid category.[/red]\nEnter empty '-c' argument to get the category list of the {asset_type}."
             )
             exit()
 
     # ->🔒file_format->
-    # if file_format == None:
-    #     pass
-    # elif asset_type == "hdris" and file_format not in ["exr", "hdr"]:
-    #     print(f"[red]{file_format} is not a valid file format for {asset_type}.[/red]")
-    #     exit()
-    # elif asset_type in ["models", "textures"] and file_format not in [
+    if asset_type == "hdris" and fileformat not in ["exr", "hdr"]:
+        print(f"[red]{fileformat} is not a valid file format for {asset_type}.[/red]")
+        exit()
+    # elif asset_type in ["models", "textures"] and fileformat not in [
     #     "jpg",
     #     "png",
     #     "exr",
     # ]:
-    #     print(f"[red]{file_format} is not a valid file format for {asset_type}.[/red]")
+    #     print(f"[red]{fileformat} is not a valid file format for {asset_type}.[/red]")
     #     exit()
 
     # ->🔒folder->
     down_folder = os.path.abspath(folder) + ("/" if folder[-1:] != "/" else "")
     if not os.path.exists(down_folder):
         try:
             os.mkdir(folder)
@@ -73,8 +72,19 @@
         + (f"/{category}" if category != None else "")
         + ("['all sizes']" if sizes == [] else str(sizes))
         + f")=>🏠"
         + (f"({folder})" if not folder == "" else "")
         + "\n"
     )
 
-    Poly(asset_type, s, category, down_folder, sizes, overwrite, noimgs, iters, tone)
+    Poly(
+        asset_type,
+        s,
+        category,
+        down_folder,
+        sizes,
+        overwrite,
+        noimgs,
+        iters,
+        tone,
+        fileformat,
+    )
```

### Comparing `polydown-0.3.1/polydown/downloader.py` & `polydown-0.3.2/polydown/downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
         asset,
         session,
         down_folder,
         subfolder,
         filename,
         overwrite,
         tone,
+        file_format,
         # --
         url=None,
         md5=None,
         # --
         k=None,
         b=None,
     ):
         self.type = type
         self.asset = asset
         self.s = session
         self.down_folder = down_folder
         self.overwrite = overwrite
         self.tone = tone
+        self.file_format = file_format
         self.md5 = md5
         self.url = url
         self.subfolder = subfolder
         self.filename = filename
         self.k = k
         self.b = b
```

### Comparing `polydown-0.3.1/polydown/hash_check.py` & `polydown-0.3.2/polydown/hash_check.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.1/polydown/poly.py` & `polydown-0.3.2/polydown/poly.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,28 +14,30 @@
         category,
         down_folder,
         sizes,
         overwrite,
         noimgs,
         iters,
         tone,
+        file_format,
     ):
         self.s = session
         self.type = type
         self.asset_url = f"https://api.polyhaven.com/assets?t={type}"
         if category != None:
             self.asset_url = f"https://api.polyhaven.com/assets?t={type}&c={category}"
         self.asset_list = [i for i in json.loads(self.s.get(self.asset_url).content)]
 
         self.down_folder = down_folder
         self.down_sizes = sizes
         self.overwrite = overwrite
         self.noimgs = noimgs
         self.iters = iters
         self.tone = tone
+        self.file_format = file_format
 
         self.corrupted_files = []
         self.exist_files = 0
         self.downloaded_files = 0
 
         self.report = Report()
         if type == "textures" or type == "models":
@@ -81,14 +83,15 @@
                         asset,
                         self.s,
                         self.down_folder,
                         self.subfolder,
                         filename,
                         self.overwrite,
                         self.tone,
+                        self.file_format,
                         bl_url,
                         bl_md5,
                         k,
                         True,
                     )
                     dw = Downloader(*args)
                     d = dw.file()
@@ -106,14 +109,15 @@
                             asset,
                             self.s,
                             self.down_folder,
                             self.subfolder,
                             filename,
                             self.overwrite,
                             self.tone,
+                            self.file_format,
                             url,
                             md5,
                             k,
                             False,
                         )
                         dw = Downloader(*args)
                         d = dw.file()
@@ -126,40 +130,42 @@
                 dw.img()
             count += 1
             if count == self.iters:
                 break
 
     def hdris(self):
         count = 0
+
         for asset in self.asset_list:
             files_url = "https://api.polyhaven.com/files/" + asset
             file_js = json.loads(self.s.get(files_url).content)
             file_sizes_list = [i for i in file_js["hdri"]]
             file_sizes_list.sort(key=lambda fname: int(fname.split("k")[0]))
 
             print(
                 theme.t_atitle
                 + " ".join([i.capitalize() for i in asset.split("_")])
                 + ":"
             )
             print(theme.t_file)
 
             for k in file_sizes_list if self.down_sizes == [] else self.down_sizes:
-                url = file_js["hdri"][k]["hdr"]["url"]
-                md5 = file_js["hdri"][k]["hdr"]["md5"]
+                url = file_js["hdri"][k][self.file_format]["url"]
+                md5 = file_js["hdri"][k][self.file_format]["md5"]
                 filename = url.split("/")[-1]
                 args = (
                     self.type,
                     asset,
                     self.s,
                     self.down_folder,
                     None,
                     filename,
                     self.overwrite,
                     self.tone,
+                    self.file_format,
                     url,
                     md5,
                 )
                 dw = Downloader(*args)
                 d = dw.file()
                 print(d[0])
                 self.report.add(d[1])
```

### Comparing `polydown-0.3.1/polydown/report.py` & `polydown-0.3.2/polydown/report.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.1/polydown/theme.py` & `polydown-0.3.2/polydown/theme.py`

 * *Files identical despite different names*

### Comparing `polydown-0.3.1/pyproject.toml` & `polydown-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polydown"
-version = "0.3.1"
+version = "0.3.2"
 description = "Batch downloader for polyhaven (polyhaven.com)"
 authors = ["Gökçe Merdun <agmmnn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/agmmnn/polydown"
 repository = "https://github.com/agmmnn/polydown"
 keywords = ["polyhaven", "download", "downloader", "scrape", "hdri", "batch"]
```

### Comparing `polydown-0.3.1/README.MD` & `polydown-0.3.2/README.MD`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 -f, --folder      target download folder.
 -c, --category    category to download.
 -s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
 -o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
 -no, --noimgs     do not download 'preview, render, thumbnail...' images.
 -it, --iters      amount of iterations.
 -t, --tone        Download 8K Tonemapped JPG (only HDRIs).
+-ff, --fileformat file format for hdris (hdr, exr).
 -v, --version     show program's version number and exit
 ```
 
 # To-Do
 
 - [ ] Unit Tests
 - [ ] Progressbar for current download task(s)
```

#### html2text {}

```diff
@@ -19,14 +19,15 @@
 c52b3cfcf8a2.png) ![file structure](https://user-images.githubusercontent.com/
 16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png) # Arguments: ```
 "hdris, textures, models" -h, --help show this help message and exit -f, --
 folder target download folder. -c, --category category to download. -s, --sizes
 size(s) of downloaded asset files. eg: 1k 2k 4k -o, --overwrite overwrite if
 the files already exists. otherwise the current task will be skipped. -no, --
 noimgs do not download 'preview, render, thumbnail...' images. -it, --iters
-amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -v, -
--version show program's version number and exit ``` # To-Do - [ ] Unit Tests -
-[ ] Progressbar for current download task(s) - [ ] Select the file format to
-download - [ ] Download a specific asset, "polydown hdris stuttgart_suburbs" #
-Requirements - Python>3.7 ## Dependencies - [requests](https://pypi.org/
-project/requests/) - [rich](https://github.com/willmcgugan/rich) # License
-[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
+amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -ff,
+--fileformat file format for hdris (hdr, exr). -v, --version show program's
+version number and exit ``` # To-Do - [ ] Unit Tests - [ ] Progressbar for
+current download task(s) - [ ] Select the file format to download - [ ]
+Download a specific asset, "polydown hdris stuttgart_suburbs" # Requirements -
+Python>3.7 ## Dependencies - [requests](https://pypi.org/project/requests/) -
+[rich](https://github.com/willmcgugan/rich) # License [MIT](https://github.com/
+agmmnn/polydown/blob/master/LICENSE)
```

### Comparing `polydown-0.3.1/setup.py` & `polydown-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['aiohttp>=3.8.3,<4.0.0', 'requests>=2.30.0,<3.0.0', 'rich>=13.3.0,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['polydown = polydown.__main__:cli']}
 
 setup_kwargs = {
     'name': 'polydown',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Batch downloader for polyhaven (polyhaven.com)',
-    'long_description': '![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)\n\n<div align="center">\n<a href="https://github.com/agmmnn/polydown">\n<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>\n<a href="https://pypi.org/project/polydown/">\n<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>\n\nBatch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven\'s [Public API](https://github.com/Poly-Haven/Public-API).\n\n</div>\n\n# Installation\n\n```\npip install polydown\n```\n\n# How to Use\n\n```\n$ polydown hdris\n\n# download all available sizes of all hdris into current folder.\n> 🔗(polyhaven.com/hdris[\'all sizes\'])=>🏠\n```\n\n```\n$ polydown <asset_type>\n\n# download all assets of this asset type to the current folder in all available sizes.\n# asset types: "hdris", "textures", "models".\n```\n\n```\n$ polydown textures -c\n\n# list of category in the given asset type.\n```\n\n```\n$ polydown hdris -f hdris_down -s 2k 4k\n\n# download all hdris with given sizes into "hdris_down" folder.\n# /if there is no such folder it will create it./\n> 🔗(polyhaven.com/hdris[\'2k\', \'4k\'])=>🏠(hdris_down)\n```\n\n## Example Usage\n\n```\n$ polydown models -c decorative -f folder -s 1k\n\n# download all "models" with "1k textures" in the "decorative" category into the "folder".\n```\n\n![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)\n\n![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)\n\n# Arguments:\n\n```\n<asset_type>      "hdris, textures, models"\n-h, --help        show this help message and exit\n-f, --folder      target download folder.\n-c, --category    category to download.\n-s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k\n-o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.\n-no, --noimgs     do not download \'preview, render, thumbnail...\' images.\n-it, --iters      amount of iterations.\n-t, --tone        Download 8K Tonemapped JPG (only HDRIs).\n-v, --version     show program\'s version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n- [ ] Progressbar for current download task(s)\n- [ ] Select the file format to download\n- [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"\n\n# Requirements\n\n- Python>3.7\n\n## Dependencies\n\n- [requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/willmcgugan/rich)\n\n# License\n\n[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)\n',
+    'long_description': '![screenshot](https://user-images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-9d189379d307.gif)\n\n<div align="center">\n<a href="https://github.com/agmmnn/polydown">\n<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/agmmnn/polydown"></a>\n<a href="https://pypi.org/project/polydown/">\n<img alt="PyPI" src="https://img.shields.io/pypi/v/polydown"></a>\n\nBatch downloader for [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in any sizes you want. This project uses Poly Haven\'s [Public API](https://github.com/Poly-Haven/Public-API).\n\n</div>\n\n# Installation\n\n```\npip install polydown\n```\n\n# How to Use\n\n```\n$ polydown hdris\n\n# download all available sizes of all hdris into current folder.\n> 🔗(polyhaven.com/hdris[\'all sizes\'])=>🏠\n```\n\n```\n$ polydown <asset_type>\n\n# download all assets of this asset type to the current folder in all available sizes.\n# asset types: "hdris", "textures", "models".\n```\n\n```\n$ polydown textures -c\n\n# list of category in the given asset type.\n```\n\n```\n$ polydown hdris -f hdris_down -s 2k 4k\n\n# download all hdris with given sizes into "hdris_down" folder.\n# /if there is no such folder it will create it./\n> 🔗(polyhaven.com/hdris[\'2k\', \'4k\'])=>🏠(hdris_down)\n```\n\n## Example Usage\n\n```\n$ polydown models -c decorative -f folder -s 1k\n\n# download all "models" with "1k textures" in the "decorative" category into the "folder".\n```\n\n![screenshot](https://user-images.githubusercontent.com/16024979/134804570-a01138e9-7fc0-4d22-b1b5-c52b3cfcf8a2.png)\n\n![file structure](https://user-images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png)\n\n# Arguments:\n\n```\n<asset_type>      "hdris, textures, models"\n-h, --help        show this help message and exit\n-f, --folder      target download folder.\n-c, --category    category to download.\n-s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k\n-o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.\n-no, --noimgs     do not download \'preview, render, thumbnail...\' images.\n-it, --iters      amount of iterations.\n-t, --tone        Download 8K Tonemapped JPG (only HDRIs).\n-ff, --fileformat file format for hdris (hdr, exr).\n-v, --version     show program\'s version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n- [ ] Progressbar for current download task(s)\n- [ ] Select the file format to download\n- [ ] Download a specific asset, "polydown hdris stuttgart_suburbs"\n\n# Requirements\n\n- Python>3.7\n\n## Dependencies\n\n- [requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/willmcgugan/rich)\n\n# License\n\n[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)\n',
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
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['polydown']
 package_data = \ {'': ['*']} install_requires = \ ['aiohttp>=3.8.3,<4.0.0',
 'requests>=2.30.0,<3.0.0', 'rich>=13.3.0,<14.0.0'] entry_points = \
 {'console_scripts': ['polydown = polydown.__main__:cli']} setup_kwargs =
-{ 'name': 'polydown', 'version': '0.3.1', 'description': 'Batch downloader for
+{ 'name': 'polydown', 'version': '0.3.2', 'description': 'Batch downloader for
 polyhaven (polyhaven.com)', 'long_description': '![screenshot](https://user-
 images.githubusercontent.com/16024979/134770914-bbc829ac-f1aa-43eb-adf4-
 9d189379d307.gif)\n\n
    \n\n[GitHub_release_(latest_by_date)]\n\n[PyPI]\n\nBatch downloader for
 [polyhaven.com](https://polyhaven.com/). Download hdris, textures and models in
    any sizes you want. This project uses Poly Haven\'s [Public API](https://
                     github.com/Poly-Haven/Public-API).\n\n
@@ -27,19 +27,20 @@
 images.githubusercontent.com/16024979/134737874-cc04a42e-5855-4acb-9394-
 dac08352efee.png)\n\n# Arguments:\n\n```\n "hdris, textures, models"\n-h, --
 help show this help message and exit\n-f, --folder target download folder.\n-c,
 --category category to download.\n-s, --sizes size(s) of downloaded asset
 files. eg: 1k 2k 4k\n-o, --overwrite overwrite if the files already exists.
 otherwise the current task will be skipped.\n-no, --noimgs do not download
 \'preview, render, thumbnail...\' images.\n-it, --iters amount of
-iterations.\n-t, --tone Download 8K Tonemapped JPG (only HDRIs).\n-v, --version
-show program\'s version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n-
-[ ] Progressbar for current download task(s)\n- [ ] Select the file format to
-download\n- [ ] Download a specific asset, "polydown hdris
-stuttgart_suburbs"\n\n# Requirements\n\n- Python>3.7\n\n## Dependencies\n\n-
-[requests](https://pypi.org/project/requests/)\n- [rich](https://github.com/
-willmcgugan/rich)\n\n# License\n\n[MIT](https://github.com/agmmnn/polydown/
-blob/master/LICENSE)\n', 'author': 'GÃ¶kÃ§e Merdun', 'author_email':
-'agmmnn@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/agmmnn/polydown', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+iterations.\n-t, --tone Download 8K Tonemapped JPG (only HDRIs).\n-ff, --
+fileformat file format for hdris (hdr, exr).\n-v, --version show program\'s
+version number and exit\n```\n\n# To-Do\n\n- [ ] Unit Tests\n- [ ] Progressbar
+for current download task(s)\n- [ ] Select the file format to download\n- [ ]
+Download a specific asset, "polydown hdris stuttgart_suburbs"\n\n#
+Requirements\n\n- Python>3.7\n\n## Dependencies\n\n- [requests](https://
+pypi.org/project/requests/)\n- [rich](https://github.com/willmcgugan/rich)\n\n#
+License\n\n[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)\n',
+'author': 'GÃ¶kÃ§e Merdun', 'author_email': 'agmmnn@gmail.com', 'maintainer':
+'None', 'maintainer_email': 'None', 'url': 'https://github.com/agmmnn/
+polydown', 'packages': packages, 'package_data': package_data,
+'install_requires': install_requires, 'entry_points': entry_points,
+'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `polydown-0.3.1/PKG-INFO` & `polydown-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polydown
-Version: 0.3.1
+Version: 0.3.2
 Summary: Batch downloader for polyhaven (polyhaven.com)
 Home-page: https://github.com/agmmnn/polydown
 License: MIT
 Keywords: polyhaven,download,downloader,scrape,hdri,batch
 Author: Gökçe Merdun
 Author-email: agmmnn@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -96,14 +96,15 @@
 -f, --folder      target download folder.
 -c, --category    category to download.
 -s, --sizes       size(s) of downloaded asset files. eg: 1k 2k 4k
 -o, --overwrite   overwrite if the files already exists. otherwise the current task will be skipped.
 -no, --noimgs     do not download 'preview, render, thumbnail...' images.
 -it, --iters      amount of iterations.
 -t, --tone        Download 8K Tonemapped JPG (only HDRIs).
+-ff, --fileformat file format for hdris (hdr, exr).
 -v, --version     show program's version number and exit
 ```
 
 # To-Do
 
 - [ ] Unit Tests
 - [ ] Progressbar for current download task(s)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polydown Version: 0.3.1 Summary: Batch downloader
+Metadata-Version: 2.1 Name: polydown Version: 0.3.2 Summary: Batch downloader
 for polyhaven (polyhaven.com) Home-page: https://github.com/agmmnn/polydown
 License: MIT Keywords: polyhaven,download,downloader,scrape,hdri,batch Author:
 GÃ¶kÃ§e Merdun Author-email: agmmnn@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -35,14 +35,15 @@
 c52b3cfcf8a2.png) ![file structure](https://user-images.githubusercontent.com/
 16024979/134737874-cc04a42e-5855-4acb-9394-dac08352efee.png) # Arguments: ```
 "hdris, textures, models" -h, --help show this help message and exit -f, --
 folder target download folder. -c, --category category to download. -s, --sizes
 size(s) of downloaded asset files. eg: 1k 2k 4k -o, --overwrite overwrite if
 the files already exists. otherwise the current task will be skipped. -no, --
 noimgs do not download 'preview, render, thumbnail...' images. -it, --iters
-amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -v, -
--version show program's version number and exit ``` # To-Do - [ ] Unit Tests -
-[ ] Progressbar for current download task(s) - [ ] Select the file format to
-download - [ ] Download a specific asset, "polydown hdris stuttgart_suburbs" #
-Requirements - Python>3.7 ## Dependencies - [requests](https://pypi.org/
-project/requests/) - [rich](https://github.com/willmcgugan/rich) # License
-[MIT](https://github.com/agmmnn/polydown/blob/master/LICENSE)
+amount of iterations. -t, --tone Download 8K Tonemapped JPG (only HDRIs). -ff,
+--fileformat file format for hdris (hdr, exr). -v, --version show program's
+version number and exit ``` # To-Do - [ ] Unit Tests - [ ] Progressbar for
+current download task(s) - [ ] Select the file format to download - [ ]
+Download a specific asset, "polydown hdris stuttgart_suburbs" # Requirements -
+Python>3.7 ## Dependencies - [requests](https://pypi.org/project/requests/) -
+[rich](https://github.com/willmcgugan/rich) # License [MIT](https://github.com/
+agmmnn/polydown/blob/master/LICENSE)
```

