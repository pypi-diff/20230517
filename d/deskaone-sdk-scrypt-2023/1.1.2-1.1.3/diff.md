# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.2.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.2.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.3.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.2.tar` & `deskaone_sdk_scrypt_2023-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-05-13 09:45:13.059942 deskaone_sdk_scrypt_2023-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.2/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-13 09:45:15.532297 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    26146 2023-05-13 09:45:06.777751 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.2/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-17 18:46:18.061771 deskaone_sdk_scrypt_2023-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.3/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-09 16:58:57.983045 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-09 16:39:36.272506 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-17 18:46:25.201118 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    29850 2023-05-17 18:46:06.589963 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.3/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.3/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -167,58 +167,63 @@
                 USERNAME        = Proxy.get('username')
                 PASSWORD        = Proxy.get('password')
                 IP              = Proxy.get('proxy_address')
                 PORT            = Proxy.get('port')
                 #ABC         = ['http', 'socks5']
                 SCHEMA      = 'http'# ABC[random.randint(0, len(ABC) - 1)]
                 try:
-                    Set = __ProxyBase__.Proxys.SaveProxy().Set(
-                        country         = '',
-                        countryCode     = '',
-                        IpPort          = f'{IP}:{PORT}',
-                        Proxies         = dict(
-                            http    = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
-                            https   = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
-                        ),
-                        BProgrammers    = False,
-                        Givvy           = False,
-                        Viker           = False,
-                        PlayFabapi      = False,
-                        Zebedee         = False
-                    )
-                    if Set is False:
-                        __ProxyBase__.Proxys.SaveProxy().Up(
+                    while True:
+                        Set = __ProxyBase__.Proxys.SaveProxy().Set(
+                            country         = '',
+                            countryCode     = '',
                             IpPort          = f'{IP}:{PORT}',
-                            Values          = dict(
-                                country         = '',
-                                countryCode     = '',
-                                Proxies         = dict(
-                                    http    = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
-                                    https   = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
-                                ),
-                                BProgrammers    = False,
-                                Givvy           = False,
-                                Viker           = False,
-                                PlayFabapi      = False,
-                                Zebedee         = False
-                            )
+                            Proxies         = dict(
+                                http    = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
+                                https   = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
+                            ),
+                            BProgrammers    = False,
+                            Givvy           = False,
+                            Viker           = False,
+                            PlayFabapi      = False,
+                            Zebedee         = False
                         )
+                        if Set is False:
+                            __ProxyBase__.Proxys.SaveProxy().Del(f'{IP}:{PORT}')
+                        else: break
+                            #__ProxyBase__.Proxys.SaveProxy().Up(
+                            #    IpPort          = f'{IP}:{PORT}',
+                            #    Values          = dict(
+                            #        country         = '',
+                            #        countryCode     = '',
+                            #        Proxies         = dict(
+                            #            http    = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
+                            #            https   = f'{SCHEMA}://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
+                            #        ),
+                            #        BProgrammers    = False,
+                            #        Givvy           = False,
+                            #        Viker           = False,
+                            #        PlayFabapi      = False,
+                            #        Zebedee         = False
+                        #    )
+                        #)
                 except Error:pass
         return __ProxyBase__.Proxys.SaveProxy().Get()
 
 class __ProxyScrape__:
     
     def __init__(self) -> None:
         self.Session    = requests.Session()
     
     @property
     def __proxy__(self):
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=http&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
-        for Proxy in Result.replace(' ', '').replace('\r', '').split('\n'):
+        Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = Proxy,
                     Proxies         = dict(
                         http    = f'http://{Proxy}',
@@ -226,19 +231,22 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks4&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
-        for Proxy in Result.replace(' ', '').replace('\r', '').split('\n'):
+        Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = Proxy,
                     Proxies         = dict(
                         http    = f'socks4://{Proxy}',
@@ -246,19 +254,22 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks5&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
-        for Proxy in Result.replace(' ', '').replace('\r', '').split('\n'):
+        Saves = [Proxy for Proxy in Result.replace(' ', '').replace('\r', '').split('\n')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = Proxy,
                     Proxies         = dict(
                         http    = f'socks5://{Proxy}',
@@ -266,14 +277,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -283,18 +295,20 @@
         self.Session    = requests.Session()
         self.BASE_URL   = 'https://proxylist.geonode.com/api/proxy-list?limit=500&page=1&sort_by=lastChecked&sort_type=desc&speed=medium&protocols=http%2Chttps%2Csocks4%2Csocks5'
     
     @property
     def __proxy__(self):
         Result  = self.Session.get(self.BASE_URL).json()
         data    = list(Result.get('data'))
-        for List in data:
-            IP      = List.get('ip')
-            PORT    = List.get('port')
-            SCHEMA  = List.get('protocols')[0]
+        Saves: List[dict] = [List for List in data]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            IP      = Proxy.get('ip')
+            PORT    = Proxy.get('port')
+            SCHEMA  = Proxy.get('protocols')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
                     Proxies         = dict(
                         http    = f'{SCHEMA.lower()}://{IP}:{PORT}',
@@ -302,14 +316,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -319,16 +334,18 @@
         self.Session    = requests.Session()
         self.BASE_URL   = 'https://free-proxy-list.net/'
     
     @property
     def __proxy__(self):
         r  = self.Session.get(self.BASE_URL)
         Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody')[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
+        Saves = [List for List in Result.findAll('tbody')[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            SPLIT   = str(Proxy).split('td>')
             IP      = SPLIT[1].split('</')[0]
             PORT    = SPLIT[3].split('</')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
@@ -338,14 +355,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
@@ -354,16 +372,18 @@
     def __init__(self) -> None:
         self.Session    = requests.Session()
     
     @property
     def __http__(self):
         r  = self.Session.get('https://www.proxy-list.download/HTTP')
         Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
+        Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            SPLIT   = str(Proxy).split('td>')
             IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
@@ -373,22 +393,25 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
     
     @property
     def __https__(self):
         r  = self.Session.get('https://www.proxy-list.download/HTTPS')
         Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
+        Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            SPLIT   = str(Proxy).split('td>')
             IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
@@ -398,22 +421,25 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
         
     @property
     def __socks4__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS4')
         Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
+        Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            SPLIT   = str(Proxy).split('td>')
             IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
@@ -423,22 +449,25 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
         
     @property
     def __socks5__(self):
         r  = self.Session.get('https://www.proxy-list.download/SOCKS5')
         Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
+        Saves = [List for List in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            SPLIT   = str(Proxy).split('td>')
             IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
                     IpPort          = f'{IP}:{PORT}',
@@ -448,14 +477,15 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
     
     @property
     def __proxy__(self):
         self.__http__
         self.__https__
         self.__socks4__
@@ -472,17 +502,18 @@
         URL = 'https://hidemy.name/en/proxy-list/'
         r = requests.get(URL, headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'})
         return BeautifulSoup(r.content, 'html5lib')
 
     @property
     def __proxy__(self):
         SOUP = self.First()
-        for row in SOUP.findAll('tbody')[0].findAll('tr'):
-            #print(row.td.text)
-            TD = str(row).split('td>')
+        Saves = [List for List in SOUP.findAll('tbody')[0].findAll('tr')]
+        for i in range(len(Saves)):
+            Proxy = Saves[random.randint(0, len(Saves) - 1)]
+            TD = str(Proxy).split('td>')
             IP = TD[1].split('</')[0]
             PORT = TD[3].split('</')[0]
             TYPE = 'http' if TD[9].split('</')[0].lower() == 'https' else TD[9].split('</')[0].lower()
             try:
                 __ProxyBase__.Proxys.SaveProxy().Set(
                     country         = '',
                     countryCode     = '',
@@ -493,66 +524,106 @@
                     ),
                     BProgrammers    = False,
                     Givvy           = False,
                     Viker           = False,
                     PlayFabapi      = False,
                     Zebedee         = False
                 )
+                if i == 20: break
             except Error:pass
+            
     
     def Main(self, New: bool) -> List[Dict[str, str]]:
         if New is True:
             self.__proxy__
         return __ProxyBase__.Proxys.SaveProxy().Get()
 
 class Proxy:
     
     def __init__(self, Authorization: Optional[str] = None, New = True, *args, **kwargs) -> None:
         if New is True:
             Typer.Print(f'{Color.RED}=> {Color.WHITE}Please Wait {Color.GREEN}Scraping New Proxy', Refresh=True)
             self.__get__(Authorization, New, **kwargs)
     
+        
+    def ProxyError(self, IpPort: Optional[str] = None, Add = False):
+        if Add is True:
+            open('Database/ProxyError.txt', 'a').write(f'{IpPort}\n')
+        else:
+            if os.path.exists('Database/ProxyError.txt') is True:
+                return set(open('Database/ProxyError.txt').read().split())
+            else:
+                return set(list())
+        
+    def ProxyDetect(self, IpPort: Optional[str] = None, Add = False):
+        if Add is True:
+            open('Database/ProxyDetect.txt', 'a').write(f'{IpPort}\n')
+        else:
+            if os.path.exists('Database/ProxyDetect.txt') is True:
+                return set(open('Database/ProxyDetect.txt').read().split())
+            else:
+                return set(list())
+    
     @property
     def ListProxy(self) -> List[Dict[str, str]]:
         return __ProxyBase__.Proxys.SaveProxy().Get()
     
     def __get__(self, Authorization: Optional[str] = None, New = True, *args, **kwargs):
         if Authorization is not None and Authorization != '':__WebShare__(Authorization).Main(New)
         if kwargs.get('ProxyScrape') is True or kwargs.get('ProxyScrape') is None:__ProxyScrape__().Main(New)
         if kwargs.get('Geonode') is True or kwargs.get('Geonode') is None:__Geonode__().Main(New)
         if kwargs.get('FreeProxyList') is True or kwargs.get('FreeProxyList') is None:__FreeProxyList__().Main(New)
         if kwargs.get('ProxyList') is True or kwargs.get('ProxyList') is None:__ProxyList__().Main(New)
         if kwargs.get('HideMy') is True or kwargs.get('HideMy') is None:__HideMy__().Main(New)
     
     def __check__(self, *args, **kwargs):
         if kwargs.get('IpPort') is None: raise Error('IpPort Required')
+        ListProxy, Count = self.ListProxy, 0
         while True:
+            Count += 1
             try:
-                PROXY   = self.ListProxy[random.randint(0, len(self.ListProxy) - 1)]
-                if kwargs.get('IpPort') != PROXY.get("IpPort"):
-                    API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
-                    Typer.Print(f'{Color.RED}=> {Color.WHITE}Check New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
-                    MYIP    = dict(requests.get("https://kin4u.com/test").json())
-                    S1 = requests.Session()
-                    CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')), timeout=30).json())
-                    if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
-                        S1.close()
-                        __ProxyBase__.Proxys.SaveProxy().Up(IpPort = PROXY.get("IpPort"), Values = dict(countryCode = API.get("countryCode"), country = API.get("country")))
-                        return dict(
-                            PROXY   = PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')),
-                            DATA    = API,
-                            IpPort  = PROXY.get('IpPort')
-                        )
-            except ProxyError as e:pass
-            except ConnectTimeout as e:pass
-            except ConnectionError as e:pass
-            except ReadTimeout as e:pass
-            except JSONDecodeError:pass
-            except TooManyRedirects as e:pass
-            except Exception as e:pass
+                ProxyErrorGO = False
+                ProxyDetectGO = False
+                PROXY   = ListProxy[random.randint(0, len(ListProxy) - 1)]
+                IpPort = PROXY.get("IpPort")
+                if IpPort in self.ProxyError(Add=False): ProxyErrorGO = True
+                if IpPort in self.ProxyDetect(Add=False): ProxyDetectGO = True
+                Typer.Print(f'{Color.RED}=> {Color.WHITE}Generate New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Count {Color.GREEN}{Count}', Refresh=True) 
+                if ProxyDetectGO is False and ProxyErrorGO is False:
+                    Count = 0
+                    if kwargs.get('IpPort') != PROXY.get("IpPort"):
+                        API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
+                        Typer.Print(f'{Color.RED}=> {Color.WHITE}Check New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
+                        MYIP    = dict(requests.get("https://kin4u.com/test").json())
+                        S1 = requests.Session()
+                        CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')), timeout=15).json())
+                        if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
+                            S1.close()
+                            __ProxyBase__.Proxys.SaveProxy().Up(IpPort = PROXY.get("IpPort"), Values = dict(countryCode = API.get("countryCode"), country = API.get("country")))
+                            return dict(
+                                PROXY   = PROXY.get('Proxies') if PROXY.get('Proxies') == dict else json.loads(PROXY.get('Proxies')),
+                                DATA    = API,
+                                IpPort  = PROXY.get('IpPort')
+                            )
+                if Count >= 100:
+                    raise Error('No Proxy Scan Again')
+            except ProxyError as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ConnectTimeout as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ConnectionError as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except ReadTimeout as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except JSONDecodeError:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except TooManyRedirects as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
+            except Exception as e:
+                self.ProxyError(IpPort=IpPort, Add=True)
     
     def Generate(self, *args, **kwargs) -> Tuple[bool, dict]:
         if len(self.ListProxy) != 0:return True,  self.__check__(**kwargs)
         return False, dict()
     
     def Show(self):
         return self.ListProxy
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.3/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/setup.py` & `deskaone_sdk_scrypt_2023-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.2/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

