# Comparing `tmp/tc_pdf-0.0.7.tar.gz` & `tmp/tc_pdf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tc_pdf-0.0.7.tar", last modified: Fri Dec 15 17:22:15 2017, max compression
+gzip compressed data, was "tc_pdf-1.0.0.tar", last modified: Wed May 17 09:56:54 2023, max compression
```

## Comparing `tc_pdf-0.0.7.tar` & `tc_pdf-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 aamiradnan   (501) staff       (20)        0 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/
--rw-r--r--   0 aamiradnan   (501) staff       (20)     1922 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/PKG-INFO
--rw-r--r--   0 aamiradnan   (501) staff       (20)      990 2017-12-14 01:03:43.000000 tc_pdf-0.0.7/README.rst
--rw-r--r--   0 aamiradnan   (501) staff       (20)      108 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/setup.cfg
--rw-r--r--   0 aamiradnan   (501) staff       (20)      965 2017-12-15 17:22:12.000000 tc_pdf-0.0.7/setup.py
-drwxr-xr-x   0 aamiradnan   (501) staff       (20)        0 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf/
--rw-r--r--   0 aamiradnan   (501) staff       (20)      225 2017-12-14 17:06:51.000000 tc_pdf-0.0.7/tc_pdf/__init__.py
-drwxr-xr-x   0 aamiradnan   (501) staff       (20)        0 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf/handlers/
--rw-r--r--   0 aamiradnan   (501) staff       (20)        0 2017-12-12 20:09:51.000000 tc_pdf-0.0.7/tc_pdf/handlers/__init__.py
--rw-r--r--   0 aamiradnan   (501) staff       (20)     7634 2017-12-15 16:48:53.000000 tc_pdf-0.0.7/tc_pdf/handlers/pdf.py
--rw-r--r--   0 aamiradnan   (501) staff       (20)     1445 2017-12-13 23:14:55.000000 tc_pdf-0.0.7/tc_pdf/pdf.py
-drwxr-xr-x   0 aamiradnan   (501) staff       (20)        0 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/
--rw-r--r--   0 aamiradnan   (501) staff       (20)        1 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 aamiradnan   (501) staff       (20)        1 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/not-zip-safe
--rw-r--r--   0 aamiradnan   (501) staff       (20)     1922 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/PKG-INFO
--rw-r--r--   0 aamiradnan   (501) staff       (20)       58 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/requires.txt
--rw-r--r--   0 aamiradnan   (501) staff       (20)      291 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 aamiradnan   (501) staff       (20)        7 2017-12-15 17:22:15.000000 tc_pdf-0.0.7/tc_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 aamir      (501) staff       (20)        0 2023-05-17 09:56:54.063435 tc_pdf-1.0.0/
+-rw-r--r--   0 aamir      (501) staff       (20)     1083 2023-05-07 22:19:22.000000 tc_pdf-1.0.0/LICENSE
+-rw-r--r--   0 aamir      (501) staff       (20)     2121 2023-05-17 09:56:54.063503 tc_pdf-1.0.0/PKG-INFO
+-rw-r--r--   0 aamir      (501) staff       (20)     1566 2023-05-07 22:19:22.000000 tc_pdf-1.0.0/README.rst
+-rw-r--r--   0 aamir      (501) staff       (20)      108 2023-05-17 09:56:54.063744 tc_pdf-1.0.0/setup.cfg
+-rw-r--r--   0 aamir      (501) staff       (20)      965 2023-05-16 19:51:12.000000 tc_pdf-1.0.0/setup.py
+drwxr-xr-x   0 aamir      (501) staff       (20)        0 2023-05-17 09:56:54.062037 tc_pdf-1.0.0/tc_pdf/
+-rw-r--r--   0 aamir      (501) staff       (20)      225 2023-05-07 22:19:22.000000 tc_pdf-1.0.0/tc_pdf/__init__.py
+drwxr-xr-x   0 aamir      (501) staff       (20)        0 2023-05-17 09:56:54.063051 tc_pdf-1.0.0/tc_pdf/handlers/
+-rw-r--r--   0 aamir      (501) staff       (20)        0 2023-05-07 22:19:22.000000 tc_pdf-1.0.0/tc_pdf/handlers/__init__.py
+-rw-r--r--   0 aamir      (501) staff       (20)     7596 2023-05-16 20:01:28.000000 tc_pdf-1.0.0/tc_pdf/handlers/pdf.py
+-rw-r--r--   0 aamir      (501) staff       (20)     1445 2023-05-07 22:40:26.000000 tc_pdf-1.0.0/tc_pdf/pdf.py
+drwxr-xr-x   0 aamir      (501) staff       (20)        0 2023-05-17 09:56:54.062866 tc_pdf-1.0.0/tc_pdf.egg-info/
+-rw-r--r--   0 aamir      (501) staff       (20)     2121 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 aamir      (501) staff       (20)      299 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 aamir      (501) staff       (20)        1 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 aamir      (501) staff       (20)        1 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/not-zip-safe
+-rw-r--r--   0 aamir      (501) staff       (20)       58 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/requires.txt
+-rw-r--r--   0 aamir      (501) staff       (20)        7 2023-05-17 09:56:54.000000 tc_pdf-1.0.0/tc_pdf.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tc_pdf-0.0.7/setup.py` & `tc_pdf-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='tc_pdf',
-    version='0.0.7',
+    version='1.0.0',
     url='http://github.com/intellisense/tc_pdf',
     license='MIT',
     author='Aamir Rind',
     author_email='aamir.adnan.rind@gmail.com',
     description='PDF Preview',
     long_description=open('README.rst').read(),
     packages=find_packages(),
```

### Comparing `tc_pdf-0.0.7/tc_pdf/handlers/pdf.py` & `tc_pdf-1.0.0/tc_pdf/handlers/pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 from __future__ import absolute_import
 
 import os
-from urllib import quote, unquote
+from urllib.parse import quote, unquote
 from io import BytesIO
-try:
-    from urllib2 import urlopen, HTTPError
-except ImportError:
-    from urllib.request import urlopen
-    from urllib.error import HTTPError
 
 from thumbor.context import RequestParameters
 from thumbor.handlers.imaging import ImagingHandler
 from thumbor.url import Url
 from thumbor.utils import logger
-import tornado.gen as gen
 import tornado
 from tornado import httputil, httpclient
 
 from wand.image import Image, Color
 from wand.exceptions import WandException
 from libthumbor import CryptoURL
 from tc_core.web import RequestParser
@@ -52,41 +46,48 @@
         reg.append(Url.valign)
         reg.append(Url.smart)
         reg.append(Url.filters)
         reg.append(cls.pdf)
 
         return ''.join(reg)
 
-    @gen.coroutine
-    def get(self, **kwargs):
+    async def get(self, **kwargs):
         # check if request is valid
-        yield gen.maybe_future(self.check_pdf(kwargs.copy()))
+        await self.check_pdf(kwargs.copy())
+        # return early if at this point the request isn't valid
+        status = self.get_status()
+        if status != 200:
+            return
 
         pdf = PDF(self.context)
         pdf_path = kwargs.pop('pdf')
         url_parts, pdf_url = pdf.url_parts(pdf_path)
         preview_path = pdf_path.replace('/pdf/', '').replace('.pdf', '.png')
 
         # Check if preview image already exists
         path = quote(preview_path.encode('utf-8'))
-        exists = yield gen.maybe_future(pdf.get(path))
+        exists = await pdf.get(path)
         if not exists:
             # create a new preview
-            data = yield self.create_preview(pdf_url)
+            data = await self.create_preview(pdf_url)
             if not data:
                 raise tornado.web.HTTPError(400)
             # store it in storage
-            yield gen.maybe_future(pdf.put(path, data))
+            await pdf.put(path, data)
         else:
             logger.debug('PDF preview already exists..')
 
         crypto = CryptoURL(key=self.context.server.security_key)
         options = {k: v for k, v in kwargs.items() if v and k != 'hash'}
         preview_url = crypto.generate(image_url=preview_path, **options)
-        kwargs['hash'] = RequestParser.path_to_parameters(preview_url)['hash']
+        parameters = RequestParser.path_to_parameters(preview_url)
+        for parameter in parameters:
+            if parameter[0] == 'hash' and parameter[1]:
+                kwargs['hash'] = parameter[1].decode()
+                break
 
         # Patch the request uri to allow normal thumbor operations
         self.request.uri = preview_url
         self.request.path = preview_url
 
         kwargs['request'] = self.request
         kwargs['image'] = preview_path
@@ -99,55 +100,52 @@
                 'Content-Disposition',
                 'inline; filename="{name}"'.format(
                     name=name
                 )
             )
 
         # Call the original ImageHandler.get method to serve the image.
-        super(PDFHandler, self).get(**kwargs)
+        return await super(PDFHandler, self).get(**kwargs)
 
-    @gen.coroutine
-    def create_preview(self, url, resolution=200):
+    async def create_preview(self, url, resolution=200):
         out_io = BytesIO()
         try:
             http_client = httpclient.AsyncHTTPClient()
-            response = yield http_client.fetch(url)
+            response = await http_client.fetch(url)
             if not response.error:
                 try:
                     with(Image(blob=response.body, resolution=resolution)) as source:
                         single_image = source.sequence[0]  # Just work on first page
                         with Image(single_image) as i:
                             i.format = 'png'
                             i.background_color = Color('white')  # Set white background.
                             i.alpha_channel = 'remove'  # Remove transparency and replace with bg.
                             i.save(file=out_io)
-                            raise gen.Return(out_io.getvalue())
+                            return out_io.getvalue()
 
                 except WandException as e:
-                    logger.exception('[PDFHander.create_preview] %s', e)
-                    raise gen.Return(None)
+                    logger.exception('[PDFHandler.create_preview] %s', e)
+                    return None
             else:
                 logger.error('STATUS: %s - Failed to get pdf from url %s' % (str(400), url))
                 raise tornado.web.HTTPError(400)
         except httpclient.HTTPError as e:
             logger.error('STATUS: %s - Failed to get pdf from url %s' % (str(e.code), url))
             valid_status_code = httputil.responses.get(e.code)
             if valid_status_code:
                 self._error(e.code)
             else:
                 raise tornado.web.HTTPError(400)
         finally:
             out_io.close()
 
-    @gen.coroutine  # NOQA
-    def check_pdf(self, kw):
+    async def check_pdf(self, kw):
         if self.context.config.MAX_ID_LENGTH > 0:
             # Check if pdf with an uuid exists in storage
-            exists = yield gen.maybe_future(
-                self.context.modules.storage.exists(kw['pdf'][:self.context.config.MAX_ID_LENGTH]))
+            exists = await self.context.modules.storage.exists(kw['pdf'][:self.context.config.MAX_ID_LENGTH])
             if exists:
                 kw['pdf'] = kw['pdf'][:self.context.config.MAX_ID_LENGTH]
 
         url = self.request.path
 
         kw['pdf'] = quote(kw['pdf'].encode('utf-8'))
         if not self.validate(kw['pdf']):
@@ -165,15 +163,15 @@
             return
 
         if self.context.request.unsafe and not self.context.config.ALLOW_UNSAFE_URL:
             self._error(400, 'URL has unsafe but unsafe is not allowed by the config: %s' % url)
             return
 
         if self.context.config.USE_BLACKLIST:
-            blacklist = yield self.get_blacklist_contents()
+            blacklist = await self.get_blacklist_contents()
             if self.context.request.pdf_url in blacklist:
                 self._error(400, 'Source pdf url has been blacklisted: %s' % self.context.request.pdf_url)
                 return
 
         url_signature = self.context.request.hash
         if url_signature:
             signer = self.context.modules.url_signer(self.context.server.security_key)
@@ -183,20 +181,19 @@
             except KeyError:
                 self._error(400, 'Invalid hash: %s' % self.context.request.hash)
                 return
 
             url_to_validate = url.replace('/%s/' % self.context.request.hash, '') \
                 .replace('/%s/' % quoted_hash, '')
 
-            valid = signer.validate(unquote(url_signature), url_to_validate)
+            valid = signer.validate(unquote(url_signature).encode(), url_to_validate)
 
             if not valid and self.context.config.STORES_CRYPTO_KEY_FOR_EACH_IMAGE:
                 # Retrieves security key for this pdf if it has been seen before
-                security_key = yield gen.maybe_future(
-                    self.context.modules.storage.get_crypto(self.context.request.pdf_url))
+                security_key = await self.context.modules.storage.get_crypto(self.context.request.pdf_url)
                 if security_key is not None:
                     signer = self.context.modules.url_signer(security_key)
                     valid = signer.validate(url_signature, url_to_validate)
 
             if not valid:
                 self._error(400, 'Malformed URL: %s' % url)
                 return
```

### Comparing `tc_pdf-0.0.7/tc_pdf/pdf.py` & `tc_pdf-1.0.0/tc_pdf/pdf.py`

 * *Files identical despite different names*

