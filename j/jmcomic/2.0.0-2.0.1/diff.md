# Comparing `tmp/jmcomic-2.0.0.tar.gz` & `tmp/jmcomic-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-h6zzdcfs/jmcomic-2.0.0.tar", last modified: Wed May 10 14:07:59 2023, max compression
+gzip compressed data, was "/home/runner/work/JMComic-Crawler-Python/JMComic-Crawler-Python/dist/.tmp-rs7emeuk/jmcomic-2.0.1.tar", last modified: Wed May 17 15:51:44 2023, max compression
```

## Comparing `jmcomic-2.0.0.tar` & `jmcomic-2.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 14:07:44.000000 jmcomic-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-10 14:07:59.000000 jmcomic-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-10 14:07:44.000000 jmcomic-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:07:59.000000 jmcomic-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 14:07:44.000000 jmcomic-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-05-10 14:07:44.000000 jmcomic-2.0.0/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 14:07:59.000000 jmcomic-2.0.0/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-17 15:51:34.000000 jmcomic-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 15:51:44.000000 jmcomic-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-17 15:51:34.000000 jmcomic-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 15:51:44.000000 jmcomic-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-17 15:51:34.000000 jmcomic-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-17 15:51:34.000000 jmcomic-2.0.1/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 15:51:44.000000 jmcomic-2.0.1/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.0/LICENSE` & `jmcomic-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.0/PKG-INFO` & `jmcomic-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
 # 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
 ```
 
-进一步的使用可以参考usage文件夹下的示例代码: `jmcomic_getting_started.py` `jmcomic_usage.py`
+进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
 
@@ -68,15 +68,14 @@
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
 * 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
-* JM不是前后端分离的网站，因此本api是通过正则表达式解析HTML网页的信息（详见`JmcomicText`），进而实现的下载图片。
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
@@ -84,10 +83,10 @@
 
   * jmcomic：`jmcomic`模块
 * tests：测试目录，存放测试代码，使用unittest
 * usage：用法目录，存放示例/使用代码
 
 ## 感谢以下项目
 
-### 图片分割算法的来源
+### 图片分割算法代码+禁漫移动端API
 
 [![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=tonquer&repo=JMComic-qt)](https://github.com/tonquer/JMComic-qt)
```

### Comparing `jmcomic-2.0.0/README.md` & `jmcomic-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
 # 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
 ```
 
-进一步的使用可以参考usage文件夹下的示例代码: `jmcomic_getting_started.py` `jmcomic_usage.py`
+进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
 
@@ -46,15 +46,14 @@
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
 * 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
-* JM不是前后端分离的网站，因此本api是通过正则表达式解析HTML网页的信息（详见`JmcomicText`），进而实现的下载图片。
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
@@ -62,10 +61,10 @@
 
   * jmcomic：`jmcomic`模块
 * tests：测试目录，存放测试代码，使用unittest
 * usage：用法目录，存放示例/使用代码
 
 ## 感谢以下项目
 
-### 图片分割算法的来源
+### 图片分割算法代码+禁漫移动端API
 
 [![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=tonquer&repo=JMComic-qt)](https://github.com/tonquer/JMComic-qt)
```

### Comparing `jmcomic-2.0.0/setup.py` & `jmcomic-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.0/src/jmcomic/api.py` & `jmcomic-2.0.1/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.1/src/jmcomic/jm_client_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -245,23 +245,38 @@
                              + (f'URL=[{url}]' if url is not None else '')
                              )
 
 
 class JmApiClient(AbstractJmClient):
     API_SEARCH = '/search'
 
-    def __init__(self,
-                 base_url,
-                 postman: Postman,
-                 retry_times=5,
-                 ):
-        super().__init__(postman, retry_times)
-        self.base_url: str = base_url
-
     def search_album(self, search_query: str, main_tag=0) -> JmApiResp:
+        """
+        model_data: {
+          "search_query": "MANA",
+          "total": "177",
+          "content": [
+            {
+              "id": "441923",
+              "author": "MANA",
+              "description": "",
+              "name": "[MANA] 神里绫华5",
+              "image": "",
+              "category": {
+                "id": "1",
+                "title": "同人"
+              },
+              "category_sub": {
+                "id": "1",
+                "title": "同人"
+              }
+            }
+          ]
+        }
+        """
         return self.get(
             self.API_SEARCH,
             params={
                 'search_query': search_query,
             }
         )
```

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.1/src/jmcomic/jm_client_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,37 +63,37 @@
 
     def __init__(self, resp, key_ts):
         super().__init__(resp)
         self.key_ts = key_ts
         self.cache_decode_data = None
 
     @staticmethod
-    def parseData(text, time):
-        import hashlib
+    def parse_data(text, time) -> str:
+        # 1. base64解码
         import base64
-        from Crypto.Cipher import AES
-        # key为时间+18comicAPPContent的md5结果
-        key = hashlib.md5(f"{time}18comicAPPContent".encode()).hexdigest().encode()
-        cipher = AES.new(key, AES.MODE_ECB)
-        # 先将数据进行base64解码
         data = base64.b64decode(text)
-        # 再进行AES-ECB解密
-        paddedPlainText = cipher.decrypt(data)
-        # 将得到的数据进行Utf8解码
-        res = paddedPlainText.decode('utf-8')
-        # 得到的数据再末尾有一些乱码
-        i = len(res) - 1
-        while i >= 0 and res[i] == '\x0c':
-            i -= 1
-        return res[:i + 1]
+
+        # 2. AES-ECB解密
+        # key = 时间戳拼接 '18comicAPPContent' 的md5
+        import hashlib
+        key = hashlib.md5(f"{time}18comicAPPContent".encode("utf-8")).hexdigest().encode("utf-8")
+        from Crypto.Cipher import AES
+        data = AES.new(key, AES.MODE_ECB).decrypt(data)
+
+        # 3. 移除末尾的一些特殊字符
+        data = data[:-data[-1]]
+
+        # 4. 解码为字符串 (json)
+        res = data.decode('utf-8')
+        return res
 
     @property
     def decoded_data(self) -> str:
         if self.cache_decode_data is None:
-            self.cache_decode_data = self.parseData(self.encoded_data, self.key_ts)
+            self.cache_decode_data = self.parse_data(self.encoded_data, self.key_ts)
 
         return self.cache_decode_data
 
     @property
     def encoded_data(self) -> str:
         return self.json()['data']
```

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_config.py` & `jmcomic-2.0.1/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_entity.py` & `jmcomic-2.0.1/src/jmcomic/jm_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                  page_arr=None,
                  data_original_domain=None,
                  author=None,
                  from_album=None,
                  ):
         self.photo_id: str = photo_id
         self.scramble_id: str = scramble_id
-        self.title: str = title
+        self.title: str = str(title).strip()
         self.sort: int = int(sort)
         self._keywords: str = keywords
         self._series_id: int = int(series_id)
 
         self._author: StrNone = author
         self.from_album: Optional[JmAlbumDetail] = from_album
 
@@ -131,14 +131,18 @@
     def keywords(self) -> List[str]:
         if self.from_album is not None:
             return self.from_album.keywords
 
         return self._keywords.split(',')
 
     @property
+    def indextitle(self):
+        return f'第{self.album_index}話 {self.title}'
+
+    @property
     def album_id(self) -> str:
         return self.photo_id if self.is_single_album else str(self._series_id)
 
     @property
     def album_index(self) -> int:
         """
         返回这个章节在本子中的序号，从1开始
```

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_option.py` & `jmcomic-2.0.1/src/jmcomic/jm_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,18 @@
 
 class DirRule:
     rule_sample = [
         # 根目录 / Album-id / Photo-序号 /
         'Bd_Aid_Pindex',  # 禁漫网站的默认下载方式
         # 根目录 / Album-作者 / Album-标题 / Photo-序号 /
         'Bd_Aauthor_Atitle_Pindex',
+        # 根目录 / Photo-序号&标题 /
+        'Bd_Pindextitle',
+        # 根目录 / Photo-自定义类属性 /
+        'Bd_Aauthor_Atitle_Pcustomfield',  # 使用自定义类属性前，需替换 JmcomicText的 PhotoClass / AlbumClass
     ]
 
     RuleFunc = Callable[[Union[JmAlbumDetail, JmPhotoDetail, None]], str]
     RuleSolver = List[Tuple[int, RuleFunc]]
 
     rule_solver_cache: Dict[Tuple[str, str], RuleSolver] = dict()
```

### Comparing `jmcomic-2.0.0/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.1/src/jmcomic/jm_toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     pattern_html_photo_series_id = compile('var series_id = (\d+);')
     pattern_html_photo_sort = compile('var sort = (\d+);')
     pattern_html_photo_page_arr = compile('var page_arr = (.*?);')
 
     pattern_html_album_album_id = compile('<span class="number">.*?：JM(\d+)</span>')
     pattern_html_album_scramble_id = compile('var scramble_id = (\d+);')
     pattern_html_album_title = compile('panel-heading[\s\S]*?<h1>(.*?)</h1>')
-    pattern_html_album_episode_list = compile('<a href=".*?" data-album="(\d+)">\n'
-                                              '<li.*>\n第(\d+)話\n(.*)\n'
+    pattern_html_album_episode_list = compile('data-album="(\d+)">\n *?<li.*?>\n *'
+                                              '第(\d+)話\n(.*)\n *'
                                               '<[\s\S]*?>(\d+-\d+-\d+).*?')
     pattern_html_album_page_count = compile('<span class="pagecount">.*?:(\d+)</span>')
     pattern_html_album_pub_date = compile('>上架日期 : (.*?)</span>')
     pattern_html_album_update_date = compile('>更新日期 : (.*?)</span>')
     pattern_html_album_keywords_list = [
         compile('<span itemprop="genre" data-type="tags">([\s\S]*?)</span>'),
         compile('<a[\s\S]*?>(.*?)</a>')
@@ -83,28 +83,32 @@
         domain_ls = cls.pattern_html_jm_pub_domain.findall(html)
 
         return list(filter(
             lambda domain: any(kw in domain for kw in domain_keyword),
             domain_ls
         ))
 
+    # 可以替换下面两个类为用户自定义的、二次继承的类
+    PhotoClass = JmPhotoDetail
+    AlbumClass = JmAlbumDetail
+
     @classmethod
-    def analyse_jm_photo_html(cls, html: str) -> JmPhotoDetail:
+    def analyse_jm_photo_html(cls, html: str) -> PhotoClass:
         return cls.reflect_new_instance(
             html,
             "pattern_html_photo_",
-            JmPhotoDetail
+            cls.PhotoClass
         )
 
     @classmethod
-    def analyse_jm_album_html(cls, html: str) -> JmAlbumDetail:
+    def analyse_jm_album_html(cls, html: str) -> AlbumClass:
         return cls.reflect_new_instance(
             html,
             "pattern_html_album_",
-            JmAlbumDetail
+            cls.AlbumClass
         )
 
     @classmethod
     def reflect_new_instance(cls, html: str, cls_field_prefix: str, clazz: type):
 
         def match_field(field_key: str, pattern: Union[Pattern, List[Pattern]], text):
```

### Comparing `jmcomic-2.0.0/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.1/src/jmcomic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -50,15 +50,15 @@
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
 # 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
 ```
 
-进一步的使用可以参考usage文件夹下的示例代码: `jmcomic_getting_started.py` `jmcomic_usage.py`
+进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
 
@@ -68,15 +68,14 @@
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
 * 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
-* JM不是前后端分离的网站，因此本api是通过正则表达式解析HTML网页的信息（详见`JmcomicText`），进而实现的下载图片。
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
@@ -84,10 +83,10 @@
 
   * jmcomic：`jmcomic`模块
 * tests：测试目录，存放测试代码，使用unittest
 * usage：用法目录，存放示例/使用代码
 
 ## 感谢以下项目
 
-### 图片分割算法的来源
+### 图片分割算法代码+禁漫移动端API
 
 [![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=tonquer&repo=JMComic-qt)](https://github.com/tonquer/JMComic-qt)
```

