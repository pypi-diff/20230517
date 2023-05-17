# Comparing `tmp/HTTP-PyServer-0.1.3.2.tar.gz` & `tmp/HTTP-PyServer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.3.2.tar", last modified: Fri May  5 16:46:06 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.4.tar", last modified: Wed May 17 20:26:35 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.3.2.tar` & `HTTP-PyServer-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.887152 HTTP-PyServer-0.1.3.2/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.3.2/LICENSE
--rw-rw-rw-   0        0        0     2043 2023-05-05 16:46:06.883416 HTTP-PyServer-0.1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.3.2/README.md
--rw-rw-rw-   0        0        0      643 2023-05-05 16:43:56.000000 HTTP-PyServer-0.1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 16:46:06.887689 HTTP-PyServer-0.1.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.781257 HTTP-PyServer-0.1.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.817711 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2043 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.876435 HTTP-PyServer-0.1.3.2/src/server/
--rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.3.2/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-05 03:22:33.000000 HTTP-PyServer-0.1.3.2/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.3.2/src/server/render.py
--rw-rw-rw-   0        0        0     2778 2023-05-05 16:43:20.000000 HTTP-PyServer-0.1.3.2/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.3.2/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.3.2/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.3.2/src/server/response_messages.py
--rw-rw-rw-   0        0        0     5060 2023-05-05 01:54:35.000000 HTTP-PyServer-0.1.3.2/src/server/routes.py
--rw-rw-rw-   0        0        0     6923 2023-05-05 01:45:04.000000 HTTP-PyServer-0.1.3.2/src/server/server.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.3.2/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-05-17 20:26:35.168905 HTTP-PyServer-0.1.4/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2091 2023-05-17 20:26:35.167909 HTTP-PyServer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1530 2023-05-17 20:22:16.000000 HTTP-PyServer-0.1.4/README.md
+-rw-rw-rw-   0        0        0      641 2023-05-17 20:22:03.000000 HTTP-PyServer-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-17 20:26:35.169903 HTTP-PyServer-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 20:26:35.096101 HTTP-PyServer-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-17 20:26:35.127022 HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2091 2023-05-17 20:26:35.000000 HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-05-17 20:26:35.000000 HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 20:26:35.000000 HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-17 20:26:35.000000 HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 20:26:35.164915 HTTP-PyServer-0.1.4/src/server/
+-rw-rw-rw-   0        0        0      414 2023-05-17 19:41:28.000000 HTTP-PyServer-0.1.4/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-17 19:49:23.000000 HTTP-PyServer-0.1.4/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.4/src/server/render.py
+-rw-rw-rw-   0        0        0     2800 2023-05-17 19:26:23.000000 HTTP-PyServer-0.1.4/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.4/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.4/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.4/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     8864 2023-05-17 20:18:32.000000 HTTP-PyServer-0.1.4/src/server/routes.py
+-rw-rw-rw-   0        0        0     7565 2023-05-17 02:18:10.000000 HTTP-PyServer-0.1.4/src/server/server.py
+-rw-rw-rw-   0        0        0     3608 2023-05-17 19:38:59.000000 HTTP-PyServer-0.1.4/src/server/sessions.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.4/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.3.2/LICENSE` & `HTTP-PyServer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/PKG-INFO` & `HTTP-PyServer-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.3.2
+Version: 0.1.4
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
-HTTP-PyServer is a simple, and extremly light-weight solution to create powerful projects relying on the web with few lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
+HTTP-PyServer is a simple, and extremely light-weight solution to create powerful projects relying on the web with the fewest lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
 
 HTTP-PyServer is also very flexible on your project layout. It ensures security by allowing you to specify which files to send, and to where. HTTP-PyServer allows you to do everything you need whilst keeping hands relaxed with as few lines of code as possible.
 
 # Installing
 
 Install HTTP-PyServer using pip from the command line.
 
@@ -37,20 +37,20 @@
 @app.route('/')
 def _(request):
 
     return 'Hello, world!'
 
 with app:
     
-    app.wait()
+    app.wait('Press Enter to continue...')
 ```
 
 ```
 $ python main.py
-Press enter to exit...
+Press Enter to continue...
 
 ```
 
 # Contributing
 
 Look on github, and create a fork of HTTP-PyServer. Submit, pull requests, and any features will be looked at, and potentially implemented.
 
@@ -60,12 +60,13 @@
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
 - `re`
+- `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
```

### Comparing `HTTP-PyServer-0.1.3.2/README.md` & `HTTP-PyServer-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Project Description
 
-HTTP-PyServer is a simple, and extremly light-weight solution to create powerful projects relying on the web with few lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
+HTTP-PyServer is a simple, and extremely light-weight solution to create powerful projects relying on the web with the fewest lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
 
 HTTP-PyServer is also very flexible on your project layout. It ensures security by allowing you to specify which files to send, and to where. HTTP-PyServer allows you to do everything you need whilst keeping hands relaxed with as few lines of code as possible.
 
 # Installing
 
 Install HTTP-PyServer using pip from the command line.
 
@@ -23,20 +23,20 @@
 @app.route('/')
 def _(request):
 
     return 'Hello, world!'
 
 with app:
     
-    app.wait()
+    app.wait('Press Enter to continue...')
 ```
 
 ```
 $ python main.py
-Press enter to exit...
+Press Enter to continue...
 
 ```
 
 # Contributing
 
 Look on github, and create a fork of HTTP-PyServer. Submit, pull requests, and any features will be looked at, and potentially implemented.
 
@@ -46,12 +46,13 @@
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
 - `re`
+- `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
-- `ssl`
+- `ssl`
```

### Comparing `HTTP-PyServer-0.1.3.2/pyproject.toml` & `HTTP-PyServer-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.3.2"
+version = "0.1.4"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.4/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.3.2
+Version: 0.1.4
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Description
 
-HTTP-PyServer is a simple, and extremly light-weight solution to create powerful projects relying on the web with few lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
+HTTP-PyServer is a simple, and extremely light-weight solution to create powerful projects relying on the web with the fewest lines of code. It uses python built-in packages to host server's and then handle http requests, as well as responses. It's extremely customizable, and allows you do to almost everything you might want.
 
 HTTP-PyServer is also very flexible on your project layout. It ensures security by allowing you to specify which files to send, and to where. HTTP-PyServer allows you to do everything you need whilst keeping hands relaxed with as few lines of code as possible.
 
 # Installing
 
 Install HTTP-PyServer using pip from the command line.
 
@@ -37,20 +37,20 @@
 @app.route('/')
 def _(request):
 
     return 'Hello, world!'
 
 with app:
     
-    app.wait()
+    app.wait('Press Enter to continue...')
 ```
 
 ```
 $ python main.py
-Press enter to exit...
+Press Enter to continue...
 
 ```
 
 # Contributing
 
 Look on github, and create a fork of HTTP-PyServer. Submit, pull requests, and any features will be looked at, and potentially implemented.
 
@@ -60,12 +60,13 @@
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
 - `re`
+- `time`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
```

### Comparing `HTTP-PyServer-0.1.3.2/src/server/cache.py` & `HTTP-PyServer-0.1.4/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/src/server/render.py` & `HTTP-PyServer-0.1.4/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/src/server/request.py` & `HTTP-PyServer-0.1.4/src/server/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                    headers = headers,
                    body = body,
                    query = query)
     
     def __str__(self):
         '''Returns the request as an HTTP request string.'''
 
-        return f'{self.method} {self.path} {self.version}\r\n' + \
+        return f'{self.method} {self.path if self.path else "/"} {self.version}\r\n' + \
 '\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) + \
 '\r\n\r\n' + \
 self.body
 
     def cookies(self):
         '''Returns the request cookies as a dictionary.'''
```

### Comparing `HTTP-PyServer-0.1.3.2/src/server/response.py` & `HTTP-PyServer-0.1.4/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/src/server/response_codes.py` & `HTTP-PyServer-0.1.4/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/src/server/response_messages.py` & `HTTP-PyServer-0.1.4/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.2/src/server/server.py` & `HTTP-PyServer-0.1.4/src/server/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,38 @@
 import logging
 from typing import Self
 import ssl
 import pathlib
 
 from . import request
 from . import routes
+from . import sessions
 
 class Server(routes.Routes):
     '''HTTP server running on a specified host and port.'''
 
     def __init__(self,
                  *,
                  host: str = '127.0.0.1',
                  port: int = 80,
                  logger: logging.Logger = None,
                  _404route: str = '/404',
                  _500route: str = '/500',
                  static_dir: str = 'static/',
-                 ssl_context: ssl.SSLContext = None) -> None:
-        '''Initializes the server class.'''
+                 ssl_context: ssl.SSLContext = None,
+                 sessions_expire_after: float = 900) -> None:
+        '''Initializes the server class.
+        
+        :param host: The IP address to run the server on.
+        :param port: The port to run the server on.
+        :param logger: The logger to use for logging.
+        :param _404route: The route to use for 404 errors.
+        :param _500route: The route to use for 500 errors.
+        :param static_dir: The directory to use for static files.
+        :param ssl_context: The SSL context to use for HTTPS.'''
         
         self._host: str = host
 
         self._port: int = port
 
         self._logger: logging.Logger = logger
 
@@ -38,32 +48,36 @@
 
             if self._logger:
 
                 self._logger.warning(f'Static directory "{static_dir}" does not exist.')
 
         self._ssl_context: ssl.SSLContext = ssl_context
 
+        self.sessions: sessions.Sessions = \
+        sessions.Sessions(remove_after = sessions_expire_after)
+
         super().__init__()
 
     def start(self) -> None:
         '''Starts the server.'''
 
         if self._logger:
 
             self._logger.info('Starting server...')
         
         threading.Thread(target = self._listen,
                         daemon = True).start()
         
-    def wait(self) -> None:
+    def wait(self,
+             msg: str = '') -> None:
         '''Waits for Enter key press or KeyboardInterrupt.'''
 
         try:
 
-            input('Press Enter to continue...\n')
+            input(msg + '\n' if msg else '')
 
         except (KeyboardInterrupt, EOFError):
 
             pass
 
     def stop(self) -> None:
         '''Stops the server.'''
```

### Comparing `HTTP-PyServer-0.1.3.2/src/server/template.py` & `HTTP-PyServer-0.1.4/src/server/template.py`

 * *Files identical despite different names*

