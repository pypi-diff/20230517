# Comparing `tmp/botxbingxuser-0.0.5.tar.gz` & `tmp/botxbingxuser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botxbingxuser-0.0.5.tar", last modified: Wed May 17 16:22:00 2023, max compression
+gzip compressed data, was "botxbingxuser-0.0.6.tar", last modified: Wed May 17 17:40:31 2023, max compression
```

## Comparing `botxbingxuser-0.0.5.tar` & `botxbingxuser-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 16:22:00.674415 botxbingxuser-0.0.5/
--rw-rw-rw-   0        0        0      566 2023-05-17 16:22:00.673190 botxbingxuser-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 16:22:00.666184 botxbingxuser-0.0.5/botxbingxuser.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-17 16:22:00.000000 botxbingxuser-0.0.5/botxbingxuser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-17 16:22:00.000000 botxbingxuser-0.0.5/botxbingxuser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 16:22:00.000000 botxbingxuser-0.0.5/botxbingxuser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 16:22:00.000000 botxbingxuser-0.0.5/botxbingxuser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 16:22:00.671194 botxbingxuser-0.0.5/botxbinxuser/
--rw-rw-rw-   0        0        0     6150 2023-05-17 16:18:41.000000 botxbingxuser-0.0.5/botxbinxuser/PrincipalMetodos.py
--rw-rw-rw-   0        0        0        0 2023-05-17 15:51:27.000000 botxbingxuser-0.0.5/botxbinxuser/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 16:22:00.675371 botxbingxuser-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-05-17 16:21:42.000000 botxbingxuser-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.560840 botxbingxuser-0.0.6/
+-rw-rw-rw-   0        0        0      566 2023-05-17 17:40:31.559839 botxbingxuser-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.552832 botxbingxuser-0.0.6/botxbingxuser.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 17:40:31.000000 botxbingxuser-0.0.6/botxbingxuser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 17:40:31.557838 botxbingxuser-0.0.6/botxbinxuser/
+-rw-rw-rw-   0        0        0     6630 2023-05-17 17:07:47.000000 botxbingxuser-0.0.6/botxbinxuser/PrincipalMetodos.py
+-rw-rw-rw-   0        0        0        0 2023-05-17 15:51:27.000000 botxbingxuser-0.0.6/botxbinxuser/__init__.py
+-rw-rw-rw-   0        0        0     4021 2023-05-17 17:07:33.000000 botxbingxuser-0.0.6/botxbinxuser/symbols.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 17:40:31.560840 botxbingxuser-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-05-17 17:39:52.000000 botxbingxuser-0.0.6/setup.py
```

### Comparing `botxbingxuser-0.0.5/PKG-INFO` & `botxbingxuser-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.5
+Version: 0.0.6
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.5/botxbingxuser.egg-info/PKG-INFO` & `botxbingxuser-0.0.6/botxbingxuser.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.5
+Version: 0.0.6
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.5/botxbinxuser/PrincipalMetodos.py` & `botxbingxuser-0.0.6/botxbinxuser/PrincipalMetodos.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 API_key         = 'yourAPI_Key'
 Secrect_Key     = 'yourSecrect_Key'
 
 infoGet         = 'GET'
 infoPost        = 'POST'
 infoDelete      ='DELETE'
 
-url_balance          =     '/openApi/swap/v2/user/balance'
-url_new_order        =     '/openApi/swap/v2/trade/order'
-url_cancel_order     =     '/openApi/swap/v2/trade/order'
-url_getopenorder     =     '/openApi/swap/v2/trade/openOrders'
-url_getIdopenorder   =     '/openApi/swap/v2/trade/order'
-url_getpositions     =     '/openApi/swap/v2/user/positions'
-url_cancelall_order  =     '/openApi/swap/v2/trade/allOpenOrders'
-url_getKlines        =     '/openApi/swap/v2/quote/klines'
-url_closeorder       =     '/openApi/swap/v2/trade/closeAllPositions'
-
+url_balance             =     '/openApi/swap/v2/user/balance'
+url_new_order           =     '/openApi/swap/v2/trade/order'
+url_cancel_order        =     '/openApi/swap/v2/trade/order'
+url_getopenorder        =     '/openApi/swap/v2/trade/openOrders'
+url_getIdopenorder      =     '/openApi/swap/v2/trade/order'
+url_getpositions        =     '/openApi/swap/v2/user/positions'
+url_cancelall_order     =     '/openApi/swap/v2/trade/allOpenOrders'
+url_getKlines           =     '/openApi/swap/v2/quote/klines'
+url_closeorder          =     '/openApi/swap/v2/trade/closeAllPositions'
+url_all_contrats        =     '/openApi/swap/v2/quote/contracts'
 
 class Client:
         def __init__(self,API_key,Secrect_Key):
             self.API_key = API_key
             self.Secrect_Key = Secrect_Key
 
 
@@ -154,14 +154,27 @@
                     "timestamp": time_stamp,
                     'recvWindow':   15000,
                     'symbol':symbol
                 }
             return self.xbingx_request(url_getpositions, data,self.API_key, self.Secrect_Key,infoGet) 
             
 
+        def get_all_contracts(self):
+            time_stamp=int(time.time() * 10 ** 3) 
+
+
+            data={
+                        'recvWindow':   15000,
+                        'timestamp' :   time_stamp,
+                        
+                }
+            
+            return self.xbingx_request(url_all_contrats, data, self.API_key, self.Secrect_Key,infoGet) 
+            
+
         def xbingx_request(self,uri_path, data, api_key, api_sec,info):
 
         
             req=''
             headers = {}
             headers['X-BX-APIKEY'] = api_key
             signature = self.get_xbingx_signature(data, api_sec)
@@ -189,10 +202,7 @@
         def get_xbingx_signature(self,data, secret):
             postdata = urllib.parse.urlencode(data)
             message = postdata.encode()
             byte_key = bytes(secret, 'UTF-8')
             mac = hmac.new(byte_key, message, hashlib.sha256).hexdigest()
             return mac
 
-
-
-
```

### Comparing `botxbingxuser-0.0.5/setup.py` & `botxbingxuser-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5' 
+VERSION = '0.0.6' 
 DESCRIPTION = 'API de acesso a Xbinx'
 LONG_DESCRIPTION = """ API de acesso a corretora XBINGX
                         Para automatizar os traders"""
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
```

