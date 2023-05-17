# Comparing `tmp/botxbingxuser-0.0.3.tar.gz` & `tmp/botxbingxuser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botxbingxuser-0.0.3.tar", last modified: Wed May 17 15:44:42 2023, max compression
+gzip compressed data, was "botxbingxuser-0.0.4.tar", last modified: Wed May 17 16:12:54 2023, max compression
```

## Comparing `botxbingxuser-0.0.3.tar` & `botxbingxuser-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:44:42.216813 botxbingxuser-0.0.3/
--rw-rw-rw-   0        0        0      566 2023-05-17 15:44:42.216813 botxbingxuser-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 15:44:42.209810 botxbingxuser-0.0.3/botxbingxuser.egg-info/
--rw-rw-rw-   0        0        0      566 2023-05-17 15:44:42.000000 botxbingxuser-0.0.3/botxbingxuser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-17 15:44:42.000000 botxbingxuser-0.0.3/botxbingxuser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:44:42.000000 botxbingxuser-0.0.3/botxbingxuser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 15:44:42.000000 botxbingxuser-0.0.3/botxbingxuser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 15:44:42.214813 botxbingxuser-0.0.3/botxbinxuser/
--rw-rw-rw-   0        0        0     4966 2023-05-17 01:36:05.000000 botxbingxuser-0.0.3/botxbinxuser/PrincipalMetodos.py
--rw-rw-rw-   0        0        0      467 2023-05-17 02:22:37.000000 botxbingxuser-0.0.3/botxbinxuser/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-17 15:44:42.217813 botxbingxuser-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-05-17 15:43:31.000000 botxbingxuser-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:12:54.365258 botxbingxuser-0.0.4/
+-rw-rw-rw-   0        0        0      566 2023-05-17 16:12:54.364257 botxbingxuser-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 16:12:54.357252 botxbingxuser-0.0.4/botxbingxuser.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-05-17 16:12:54.000000 botxbingxuser-0.0.4/botxbingxuser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-17 16:12:54.000000 botxbingxuser-0.0.4/botxbingxuser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:12:54.000000 botxbingxuser-0.0.4/botxbingxuser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-17 16:12:54.000000 botxbingxuser-0.0.4/botxbingxuser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 16:12:54.361255 botxbingxuser-0.0.4/botxbinxuser/
+-rw-rw-rw-   0        0        0     6447 2023-05-17 16:11:23.000000 botxbingxuser-0.0.4/botxbinxuser/PrincipalMetodos.py
+-rw-rw-rw-   0        0        0        0 2023-05-17 15:51:27.000000 botxbingxuser-0.0.4/botxbinxuser/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:12:54.366259 botxbingxuser-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-05-17 16:12:22.000000 botxbingxuser-0.0.4/setup.py
```

### Comparing `botxbingxuser-0.0.3/PKG-INFO` & `botxbingxuser-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.3
+Version: 0.0.4
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.3/botxbingxuser.egg-info/PKG-INFO` & `botxbingxuser-0.0.4/botxbingxuser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botxbingxuser
-Version: 0.0.3
+Version: 0.0.4
 Summary: API de acesso a Xbinx
 Author: Thiago Ventura
 Author-email: <tigoluthi@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `botxbingxuser-0.0.3/botxbinxuser/PrincipalMetodos.py` & `botxbingxuser-0.0.4/botxbinxuser/PrincipalMetodos.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,170 +24,179 @@
 url_getIdopenorder   =     '/openApi/swap/v2/trade/order'
 url_getpositions     =     '/openApi/swap/v2/user/positions'
 url_cancelall_order  =     '/openApi/swap/v2/trade/allOpenOrders'
 url_getKlines        =     '/openApi/swap/v2/quote/klines'
 url_closeorder       =     '/openApi/swap/v2/trade/closeAllPositions'
 
 
+class Client:
+        def __init__(self,API_key,Secrect_Key):
+            self.API_key = API_key
+            self.Secrect_Key = Secrect_Key
 
 
+        
+        
 
-def get_xbingx_signature(data, secret):
-    postdata = urllib.parse.urlencode(data)
-    message = postdata.encode()
-    byte_key = bytes(secret, 'UTF-8')
-    mac = hmac.new(byte_key, message, hashlib.sha256).hexdigest()
-    return mac
-
-
-
-def xbingx_request(uri_path, data, api_key, api_sec,info):
-   
-    req=''
-    headers = {}
-    headers['X-BX-APIKEY'] = api_key
-    signature = get_xbingx_signature(data, api_sec)
-   
-    params={
-            **data, 
-            "signature": signature
-            }
-    
-    if info=="GET":
-        req = requests.get((api_url + uri_path), params=params, headers=headers)
-        return req.json()
-
-    elif info=='DELETE':
-        req = requests.delete((api_url + uri_path), headers=headers, params=params)
-        return req.json()
-
-
-    elif info=='POST':
-
-        req = requests.post((api_url + uri_path), headers=headers, data=params)
-        return req.json()
-    
-
-
-def getbalance(self):
-
-   time_stamp=int(time.time() * 10 ** 3) 
-   data = {
-            'recvWindow':   15000,
-            "timestamp": time_stamp
-        }
-   
-   return xbingx_request(url_balance, data, self.API_key, self.Secrect_Key,infoGet) 
-
-
-
-def neworder(self,type,side,symbol,**params):
-
-    time_stamp=int(time.time() * 10 ** 3) 
-    
-    """exemplos de new order:
-    #preco =float(envio['price'])*0.98
-    #resposta = neworder(type = "LIMIT",side="BUY",quantity=0.001,price=preco,symbol="BTC-USDT")
-    #resposta=neworder(type=envio['type'],price=envio['price'],quantity=envio['quantity'],side=envio['side'],symbol=envio['symbol'])
-    #print(resposta)"""
-    
-    """LIMIT	quantity, price
-       MARKET	quantity
-       TRIGGER_LIMIT	quantity, stopPrice, price
-       STOP_MARKET, TAKE_PROFIT_MARKET, TRIGGER_MARKET	quantity, stopPrice"""
-    
-    """De acordo com a opção escolhida, o neworder() recebe parametros adicionais"""
-    
-    data = {
-            'recvWindow':   15000,
-            'timestamp' :   time_stamp,
-            'symbol'    :   symbol,
-            'type'      :   type,
-            'side'      :   side,
-            **params  
-            
-            }
-    return xbingx_request(url_new_order, data,self.API_key, self.Secrect_Key,infoPost) 
-    
- 
-
-def getopenorder(self):
-       
-       time_stamp=int(time.time() * 10 ** 3) 
-
-   
-    
-       data = {
-                    
-                    "timestamp": time_stamp,
+
+        def getbalance(self):
+
+
+            time_stamp=int(time.time() * 10 ** 3) 
+            data = {
+                        'recvWindow':   15000,
+                        "timestamp": time_stamp
+                    }
+            
+            return self.xbingx_request(url_balance, data, self.API_key, self.Secrect_Key,infoGet) 
+
+
+
+        def neworder(self,type,side,symbol,**params):
+
+            time_stamp=int(time.time() * 10 ** 3) 
+            
+            """exemplos de new order:
+            #preco =float(envio['price'])*0.98
+            #resposta = neworder(type = "LIMIT",side="BUY",quantity=0.001,price=preco,symbol="BTC-USDT")
+            #resposta=neworder(type=envio['type'],price=envio['price'],quantity=envio['quantity'],side=envio['side'],symbol=envio['symbol'])
+            #print(resposta)"""
+            
+            """LIMIT	quantity, price
+            MARKET	quantity
+            TRIGGER_LIMIT	quantity, stopPrice, price
+            STOP_MARKET, TAKE_PROFIT_MARKET, TRIGGER_MARKET	quantity, stopPrice"""
+            
+            """De acordo com a opção escolhida, o neworder() recebe parametros adicionais"""
+            
+            data = {
                     'recvWindow':   15000,
+                    'timestamp' :   time_stamp,
+                    'symbol'    :   symbol,
+                    'type'      :   type,
+                    'side'      :   side,
+                    **params  
                     
-                }
+                    }
+            return self.xbingx_request(url_new_order, data,self.API_key, self.Secrect_Key,infoPost) 
+            
         
-       return xbingx_request(url_getopenorder, data,self.API_key, self.Secrect_Key,infoGet) 
 
+        def getopenorder(self):
+            
+            time_stamp=int(time.time() * 10 ** 3) 
 
+        
+            
+            data = {
+                            
+                            "timestamp": time_stamp,
+                            'recvWindow':   15000,
+                            
+                        }
+                
+            return self.xbingx_request(url_getopenorder, data,self.API_key, self.Secrect_Key,infoGet) 
 
-def Closeordens(self,**params):
-   time_stamp=int(time.time() * 10 ** 3) 
 
-   data={
-            'recvWindow':   15000,
-            'timestamp' :   time_stamp,
-            **params
-         
-        }
-   
-   return xbingx_request(url_closeorder, data, self.API_key, self.Secrect_Key,infoPost)
 
+        def Closeordens(self,**params):
+            time_stamp=int(time.time() * 10 ** 3) 
 
+            data={
+                        'recvWindow':   15000,
+                        'timestamp' :   time_stamp,
+                        **params
+                    
+                    }
+            
+            return self.xbingx_request(url_closeorder, data, self.API_key, self.Secrect_Key,infoPost)
 
-def cancelarorder(self,id,symbol):
-    
-    time_stamp=int(time.time() * 10 ** 3) 
 
 
-    data={
-                'recvWindow':   15000,
-                'timestamp' :   time_stamp,
-                'symbol'    :   symbol,
-                'orderId'   :   id
+        def cancelarorder(self,id,symbol):
             
-            }
-   
-    return xbingx_request(url_cancel_order, data,self.API_key, self.Secrect_Key,infoDelete) 
+            time_stamp=int(time.time() * 10 ** 3) 
+
+
+            data={
+                        'recvWindow':   15000,
+                        'timestamp' :   time_stamp,
+                        'symbol'    :   symbol,
+                        'orderId'   :   id
+                    
+                    }
+        
+            return self.xbingx_request(url_cancel_order, data,self.API_key, self.Secrect_Key,infoDelete) 
 
 
 
-def cancelallordens(self,symbol):
+        def cancelallordens(self,symbol):
 
-    time_stamp=int(time.time() * 10 ** 3) 
+            time_stamp=int(time.time() * 10 ** 3) 
 
 
-    data={
-                'recvWindow':   15000,
-                'timestamp' :   time_stamp,
-                'symbol'    :   symbol
-                
+            data={
+                        'recvWindow':   15000,
+                        'timestamp' :   time_stamp,
+                        'symbol'    :   symbol
+                        
+                    
+                    }
+            
+            return self.xbingx_request(url_cancelall_order, data, self.API_key, self.Secrect_Key,infoDelete) 
+
+
+
+        def getpositions(self,symbol):
+            
+            time_stamp=int(time.time() * 10 ** 3) 
             
-            }
-    
-    return xbingx_request(url_cancelall_order, data, self.API_key, self.Secrect_Key,infoDelete) 
+            data={
+                    "timestamp": time_stamp,
+                    'recvWindow':   15000,
+                    'symbol':symbol
+                }
+            return self.xbingx_request(url_getpositions, data,self.API_key, self.Secrect_Key,infoGet) 
+            
+
+        def xbingx_request(self,uri_path, data, api_key, api_sec,info):
+
+        
+            req=''
+            headers = {}
+            headers['X-BX-APIKEY'] = api_key
+            signature = self.get_xbingx_signature(data, api_sec)
+        
+            params={
+                    **data, 
+                    "signature": signature
+                    }
+            
+            if info=="GET":
+                req = requests.get((api_url + uri_path), params=params, headers=headers)
+                return req.json()
+
+            elif info=='DELETE':
+                req = requests.delete((api_url + uri_path), headers=headers, params=params)
+                return req.json()
+
 
+            elif info=='POST':
 
+                req = requests.post((api_url + uri_path), headers=headers, data=params)
+                return req.json()
+               
 
-def getpositions(self,symbol):
-    
-    time_stamp=int(time.time() * 10 ** 3) 
-    
-    data={
-            "timestamp": time_stamp,
-            'recvWindow':   15000,
-            'symbol':symbol
-        }
-    return xbingx_request(url_getpositions, data,self.API_key, self.Secrect_Key,infoGet) 
-    
-    
+        def get_xbingx_signature(self,data, secret):
+            postdata = urllib.parse.urlencode(data)
+            message = postdata.encode()
+            byte_key = bytes(secret, 'UTF-8')
+            mac = hmac.new(byte_key, message, hashlib.sha256).hexdigest()
+            return mac
 
 
 
 
+API_key         = 'HN907NfGrLGDjCrZxlWuhs5epIF4jW2mNjrIrUIUquX5e9HP4N0TP4Zg9tF8Rp6EqZG9WJZAqm8LZAiu8Q'
+Secrect_Key     = 'OAhCzm5hKqHgmrhoUNiDWghmfSNMuRgj5tfB2MQrBbAvRTg9BfmdBpQn5mjWMc1yRaVvDDdnK2IGBxh6RoXg'
+thiago  = Client(API_key=API_key,Secrect_Key=Secrect_Key)
+print(thiago.getbalance())
```

### Comparing `botxbingxuser-0.0.3/setup.py` & `botxbingxuser-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3' 
+VERSION = '0.0.4' 
 DESCRIPTION = 'API de acesso a Xbinx'
 LONG_DESCRIPTION = """ API de acesso a corretora XBINGX
                         Para automatizar os traders"""
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
```

