# Comparing `tmp/reportbro_lib-3.1.0.tar.gz` & `tmp/reportbro_lib-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportbro_lib-3.1.0.tar", max compression
+gzip compressed data, was "reportbro_lib-3.2.0.tar", max compression
```

## Comparing `reportbro_lib-3.1.0.tar` & `reportbro_lib-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34520 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/README.rst
--rw-r--r--   0        0        0     1327 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      122 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/__init__.py
--rw-r--r--   0        0        0     7046 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/barcode128.py
--rw-r--r--   0        0        0    10728 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/containers.py
--rw-r--r--   0        0        0    15158 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/context.py
--rw-r--r--   0        0        0        0 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/data/__init__.py
--rw-r--r--   0        0        0    10193 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/data/logo_watermark.png
--rw-r--r--   0        0        0     5928 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/docelement.py
--rw-r--r--   0        0        0    80968 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/elements.py
--rw-r--r--   0        0        0     1143 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/enums.py
--rw-r--r--   0        0        0      698 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/errors.py
--rw-r--r--   0        0        0    13346 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/rendering.py
--rw-r--r--   0        0        0    46361 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/reportbro.py
--rw-r--r--   0        0        0     7085 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/structs.py
--rw-r--r--   0        0        0     1515 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/utils.py
--rw-r--r--   0        0        0       22 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/version.py
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 reportbro_lib-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/LICENSE
+-rw-r--r--   0        0        0     1868 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/README.rst
+-rw-r--r--   0        0        0     1458 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/__init__.py
+-rw-r--r--   0        0        0     7046 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/barcode128.py
+-rw-r--r--   0        0        0    10788 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/containers.py
+-rw-r--r--   0        0        0    15158 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/context.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/data/__init__.py
+-rw-r--r--   0        0        0    10193 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/data/logo_watermark.png
+-rw-r--r--   0        0        0     5962 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/docelement.py
+-rw-r--r--   0        0        0    86135 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/elements.py
+-rw-r--r--   0        0        0     1143 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/enums.py
+-rw-r--r--   0        0        0      698 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/errors.py
+-rw-r--r--   0        0        0    20604 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/rendering.py
+-rw-r--r--   0        0        0    46999 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/reportbro.py
+-rw-r--r--   0        0        0    12201 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/structs.py
+-rw-r--r--   0        0        0     1515 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/utils.py
+-rw-r--r--   0        0        0       22 2023-05-12 18:07:50.679225 reportbro_lib-3.2.0/reportbro/version.py
+-rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 reportbro_lib-3.2.0/PKG-INFO
```

### Comparing `reportbro_lib-3.1.0/LICENSE` & `reportbro_lib-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/README.rst` & `reportbro_lib-3.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 For pull requests the same coding styles should be used.
 
 License
 -------
 
 - Commercial license
 
-If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index.
+If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index
+
+This license includes ReportBro PLUS with additional features.
 
 - Open-source license
 
 If you are creating an open-source application under a license compatible with the `GNU AGPL license v3 <https://www.gnu.org/licenses/agpl-3.0.html>`_, you may use ReportBro under the terms of the AGPLv3.
 
 Read more about ReportBro's license options at https://www.reportbro.com/license/index.
```

### Comparing `reportbro_lib-3.1.0/pyproject.toml` & `reportbro_lib-3.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reportbro-lib"
-version = "3.1.0"
+version = "3.2.0"
 description = "Generate PDF and Excel reports from visually designed templates"
 authors = ["jobsta <alex@reportbro.com>"]
 license = "AGPL-3.0"
 readme = "README.rst"
 
 homepage = "https://www.reportbro.com"
 repository = "https://github.com/jobsta/reportbro-lib"
@@ -29,18 +29,22 @@
 ]
 
 include = ["data/logo_watermark.png"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Babel = "^2.10.2"
-reportbro-fpdf2 = "^0.9.1"
+python-barcode = "^0.14.0"
+reportbro-fpdf2 = "^2.7.1"
+# reportbro-fpdf2 = { path = "../fpdf2/", develop = true}
 reportbro-simpleeval = "^0.9.11"
 Pillow = "^9.2.0"
-qrcode = "^7.3.1"
+qrcode = "^7.4.2"
 XlsxWriter = "^3.0.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `reportbro_lib-3.1.0/reportbro/barcode128.py` & `reportbro_lib-3.2.0/reportbro/barcode128.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/reportbro/containers.py` & `reportbro_lib-3.2.0/reportbro/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
 
                     if elem.is_printed(ctx):
                         if offset_y >= container_height:
                             new_page = True
                         if not new_page:
                             render_elem, complete = elem.get_next_render_element(
                                 offset_y, container_top=container_top,
-                                container_height=container_height, ctx=ctx, pdf_doc=pdf_doc)
+                                container_width=self.width, container_height=container_height,
+                                ctx=ctx, pdf_doc=pdf_doc)
                             if complete:
                                 processed_elements.append(elem)
                             if render_elem:
                                 self.render_elements.append(render_elem)
                                 self.render_elements_created = True
                                 if elem.bottom > self.max_bottom:
                                     self.max_bottom = elem.bottom
```

### Comparing `reportbro_lib-3.1.0/reportbro/context.py` & `reportbro_lib-3.2.0/reportbro/context.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/reportbro/data/logo_watermark.png` & `reportbro_lib-3.2.0/reportbro/data/logo_watermark.png`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/reportbro/docelement.py` & `reportbro_lib-3.2.0/reportbro/docelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     def finish_empty_element(self, offset_y):
         if self.remove_empty_element:
             self.render_bottom = offset_y
         else:
             self.render_bottom = offset_y + self.height
         self.rendering_complete = True
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         self.rendering_complete = True
         return None, True
 
     def render_pdf(self, container_offset_x, container_offset_y, pdf_doc):
         pass
 
     def render_spreadsheet(self, row, col, ctx, renderer):
@@ -101,15 +101,15 @@
         DocElementBase.__init__(self, report, data)
         self.id = get_int_value(data, 'id')
         self.x = get_int_value(data, 'x')
         self.width = get_int_value(data, 'width')
         self.height = get_int_value(data, 'height')
         self.bottom = self.y + self.height
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         if offset_y + self.height <= container_height:
             self.render_y = offset_y
             self.render_bottom = offset_y + self.height
             self.rendering_complete = True
             return self, True
         return None, False
```

### Comparing `reportbro_lib-3.1.0/reportbro/elements.py` & `reportbro_lib-3.2.0/reportbro/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from babel.numbers import format_decimal
 from babel.dates import format_datetime
+from barcode import Code128, Code39, EAN8, EAN13, UPCA
+from barcode.errors import BarcodeError
 from io import BytesIO
 import copy
 import datetime
 import decimal
 import PIL
 import qrcode
-import tempfile
-import urllib
+import qrcode.image.svg
 
-from .barcode128 import code128_image
 from .context import Context
 from .docelement import DocElementBase, DocElement
 from .enums import *
 from .errors import Error, ReportBroError, ReportBroInternalError
-from .rendering import ImageRenderElement, BarCodeRenderElement, TableRenderElement,\
+from .rendering import BarCodeRenderElement, BarcodeSVGWriter, ImageRenderElement, TableRenderElement,\
     FrameRenderElement, SectionRenderElement
 from .structs import Color, BorderStyle, TextStyle
 from .utils import get_float_value, get_int_value, get_str_value, to_string, get_image_display_size
 
 
 class ImageElement(DocElement):
     def __init__(self, report, data):
@@ -34,14 +34,19 @@
         self.link = get_str_value(data, 'link')
         self.spreadsheet_hide = bool(data.get('spreadsheet_hide'))
         self.spreadsheet_column = get_int_value(data, 'spreadsheet_column')
         self.spreadsheet_add_empty_row = bool(data.get('spreadsheet_addEmptyRow'))
         self.image_key = None
         self.prepared_link = None
 
+    def is_printed(self, ctx):
+        if self.remove_empty_element and not self.image_key:
+            return False
+        return super().is_printed(ctx)
+
     def prepare(self, ctx, pdf_doc, only_verify):
         self.image_key = None
         # set image_key which is used to fetch cached images
         if self.source:
             if Context.is_parameter_name(self.source):
                 # use current parameter value as image key
                 param_ref = ctx.get_parameter(Context.strip_parameter_name(self.source))
@@ -51,30 +56,34 @@
                         self.image_key, _ = ctx.get_parameter_data(param_ref)
                     elif source_parameter.type == ParameterType.image:
                         self.image_key = self.source + '_' +\
                                          str(Context.get_parameter_context_id(param_ref))
             else:
                 # static url
                 self.image_key = self.source
-        else:
+        elif self.image:
             # static image
             if self.image_filename:
                 self.image_key = self.image_filename
             else:
                 self.image_key = 'image_' + str(self.id)
-        self.report.load_image(self.image_key, ctx, self.id, self.source, self.image)
+
+        # only load image if available
+        if self.image_key:
+            self.report.load_image(self.image_key, ctx, self.id, self.source, self.image)
+
         if self.link:
             self.prepared_link = ctx.fill_parameters(self.link, self.id, field='link')
             if not (self.prepared_link.startswith('http://') or self.prepared_link.startswith('https://')):
                 raise ReportBroError(
                     Error('errorMsgInvalidLink', object_id=self.id, field='link'))
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         _, rv = DocElement.get_next_render_element(
-            self, offset_y, container_top, container_height, ctx, pdf_doc)
+            self, offset_y, container_top, container_width, container_height, ctx, pdf_doc)
         if not rv:
             return None, False
         return ImageRenderElement(self.report, offset_y, self), True
 
     def render_spreadsheet(self, row, col, ctx, renderer):
         if self.image_key:
             image = self.report.get_image(self.image_key)
@@ -104,70 +113,153 @@
 
 
 class BarCodeElement(DocElement):
     def __init__(self, report, data):
         DocElement.__init__(self, report, data)
         self.content = get_str_value(data, 'content')
         self.format = get_str_value(data, 'format').lower()
-        assert self.format in ('code128', 'qrcode')
-        self.display_value = bool(data.get('displayValue')) if self.format == 'code128' else False
-        self.bar_width = get_float_value(data, 'barWidth')
+        if self.format not in ('code39', 'code128', 'ean8', 'ean13', 'upc', 'qrcode'):
+            raise ReportBroInternalError(f'invalid format for barcode element {self.id}', log_error=False)
+        self.display_value = bool(data.get('displayValue'))
+        self.guardbar = bool(data.get('guardBar'))
+        if self.format not in ('ean8', 'ean13'):
+            self.guardbar = False
+        # use default for bar_width if setting is not available since setting was introduced in a later version
+        # and could be missing in an older report definition
+        self.bar_width = get_float_value(data, 'barWidth') if 'barWidth' in data else 2.0
+        if self.format != 'qrcode' and (self.bar_width < 0.3 or self.bar_width > 3.0):
+            raise ReportBroInternalError(f'bar width for barcode element {self.id} is out of range', log_error=False)
+        self.rotate = bool(data.get('rotate'))
+        if self.format == 'qrcode':
+            self.display_value = False
+            self.rotate = False
         error_correction_level = get_str_value(data, 'errorCorrectionLevel')
         self.error_correction_level = qrcode.ERROR_CORRECT_M
         if error_correction_level == 'L':
             self.error_correction_level = qrcode.ERROR_CORRECT_L
         elif error_correction_level == 'H':
             self.error_correction_level = qrcode.ERROR_CORRECT_H
         elif error_correction_level == 'Q':
             self.error_correction_level = qrcode.ERROR_CORRECT_Q
         self.print_if = data.get('printIf', '')
         self.remove_empty_element = bool(data.get('removeEmptyElement'))
         self.spreadsheet_hide = bool(data.get('spreadsheet_hide'))
         self.spreadsheet_column = get_int_value(data, 'spreadsheet_column')
         self.spreadsheet_colspan = get_int_value(data, 'spreadsheet_colspan')
         self.spreadsheet_add_empty_row = bool(data.get('spreadsheet_addEmptyRow'))
-        self.image_key = None
-        self.image_height = self.height - 22 if (self.display_value and self.format == 'code128') else self.height
+        self.svg_data = None
+        self.barcode_width = 0
+        self.barcode_height = self.width if self.rotate else self.height
+        if self.display_value:
+            # save space for barcode value as text
+            self.barcode_height -= 22
         self.prepared_content = None
 
     def is_printed(self, ctx):
         if not self.content:
             return False
         return DocElementBase.is_printed(self, ctx)
 
     def prepare(self, ctx, pdf_doc, only_verify):
-        self.image_key = None
         self.prepared_content = ctx.fill_parameters(self.content, self.id, field='content')
         if self.prepared_content:
-            try:
-                if self.format == 'qrcode':
-                    img = qrcode.make(self.prepared_content, border=0, error_correction=self.error_correction_level)
-                elif self.format == 'code128':
-                    img = code128_image(
-                        self.prepared_content, height=self.image_height, thickness=self.bar_width, quiet_zone=False)
-            except:
-                raise ReportBroError(
-                    Error('errorMsgInvalidBarCode', object_id=self.id, field='content'))
-            if not only_verify:
-                with tempfile.NamedTemporaryFile(delete=False, suffix='.png') as f:
-                    img.save(f.name)
-                    self.image_key = f.name
-                    if self.format == 'qrcode':
-                        # QR Code is always quadratic and only height can be set -> use same value for width
-                        self.width = self.height
+            self.svg_data = BytesIO()
+            if self.format == 'qrcode':
+                qr = qrcode.make(
+                    self.prepared_content, error_correction=self.error_correction_level, border=0,
+                    image_factory=qrcode.image.svg.SvgPathImage)
+                # use defined height in layout since qr code is quadratic
+                self.barcode_width = self.barcode_height
+
+                if not only_verify:
+                    qr.save(self.svg_data)
+
+            else:
+                svg_writer = BarcodeSVGWriter()
+                barcode = None
+                checksum_digit = None  # checksum digit in given barcode value
+                checksum = None
+                digits = dict(ean8=EAN8.digits, ean13=EAN13.digits, upc=UPCA.digits).get(self.format, 0)
+                if digits and len(self.prepared_content) > digits:
+                    # barcode assumes certain number of digits + one optional checksum digit
+                    if len(self.prepared_content) > digits + 1:
+                        raise ReportBroError(
+                            Error('errorMsgInvalidBarCode', object_id=self.id, field='content',
+                                  info='barcode value too long'))
                     else:
-                        # for Code128 the width is defined by the image width of the bar code
-                        self.width = img.width
+                        # barcode value contains checksum digit
+                        checksum_digit = self.prepared_content[digits]
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
-        _, rv = DocElement.get_next_render_element(
-            self, offset_y, container_top, container_height, ctx, pdf_doc)
-        if not rv:
-            return None, False
-        return BarCodeRenderElement(self.report, offset_y, self), True
+                try:
+                    if self.format == 'code39':
+                        barcode = Code39(self.prepared_content, writer=svg_writer)
+                        self.prepared_content = barcode.code  # make sure value is upper case and contains checksum
+                    elif self.format == 'code128':
+                        barcode = Code128(self.prepared_content, writer=svg_writer)
+                    elif self.format == 'ean8':
+                        barcode = EAN8(self.prepared_content, writer=svg_writer, guardbar=self.guardbar)
+                        self.prepared_content = barcode.ean  # make sure value contains checksum
+                        checksum = barcode.ean[-1]
+                    elif self.format == 'ean13':
+                        barcode = EAN13(self.prepared_content, writer=svg_writer, guardbar=self.guardbar)
+                        self.prepared_content = barcode.ean  # make sure value contains checksum
+                        checksum = barcode.ean[-1]
+                    elif self.format == 'upc':
+                        barcode = UPCA(self.prepared_content, writer=svg_writer)
+                        self.prepared_content = barcode.upc  # make sure value contains checksum
+                        checksum = barcode.upc[-1]
+
+                    if checksum_digit and checksum_digit != checksum:
+                        # checksum digit is present in bar code value but does not match calculated checksum
+                        raise ReportBroError(
+                            Error('errorMsgInvalidBarCode', object_id=self.id, field='content',
+                                  info='invalid checksum'))
+                except (BarcodeError, KeyError) as ex:
+                    raise ReportBroError(
+                        Error('errorMsgInvalidBarCode', object_id=self.id, field='content', info=str(ex)))
+                assert barcode
+
+                if not only_verify:
+                    barcode_height = self.barcode_height
+                    if self.guardbar:
+                        # guardbars are longer than normal bars, therefor we reduce the height for the
+                        # normal bars so the maximum height is not exceeded
+                        barcode_height -= 7
+                    barcode.write(self.svg_data, options=dict(
+                        module_width=self.bar_width, module_height=barcode_height,
+                        write_text=False, quiet_zone=0)
+                    )
+                    self.barcode_width = svg_writer.barcode_width
+
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
+        content_width = 0
+        if self.display_value:
+            pdf_doc.set_font('courier', 'B', 18)
+            content_width = pdf_doc.get_string_width(self.prepared_content)
+
+        if self.rotate:
+            # if barcode is rotated and value is shown then the rendered height is the larger value of
+            # barcode width and value text width
+            height = self.barcode_width if self.barcode_width > content_width else content_width
+        else:
+            # make sure barcode fits inside available space of container when barcode width depends on barcode value
+            if self.format in ('code39', 'code128'):
+                width = self.barcode_width if self.barcode_width > content_width else content_width
+                if self.x + width > container_width:
+                    raise ReportBroError(
+                        Error('errorMsgInvalidSize', object_id=self.id, field='height'))
+
+            height = self.height
+
+        if offset_y + height <= container_height:
+            self.render_y = offset_y
+            self.render_bottom = offset_y + height
+            self.rendering_complete = True
+            return BarCodeRenderElement(self.report, offset_y, content_width=content_width, barcode=self), True
+        return None, False
 
     def render_spreadsheet(self, row, col, ctx, renderer):
         if self.content:
             cell_format = dict()
             if self.spreadsheet_column:
                 col = self.spreadsheet_column - 1
             renderer.write(row, col, self.spreadsheet_colspan, self.prepared_content, cell_format, self.width)
@@ -209,31 +301,30 @@
         if self.rich_text and not isinstance(self.rich_text_content, dict):
             raise ReportBroInternalError(f'Invalid richTextContent for text element {self.id}')
         self.eval = bool(data.get('eval'))
         if data.get('styleId'):
             style = report.styles.get(get_int_value(data, 'styleId'))
             if style is None:
                 raise ReportBroInternalError(f'Style for text element {self.id} not found')
-            # shallow copy is sufficient in our case
-            self.style = copy.copy(style)
+            self.style = style
         else:
-            self.style = TextStyle(data)
+            self.style = TextStyle(data, id_suffix='_text')
+
         self.print_if = get_str_value(data, 'printIf')
         self.pattern = get_str_value(data, 'pattern')
         self.link = get_str_value(data, 'link')
         self.cs_condition = get_str_value(data, 'cs_condition')
         if self.cs_condition:
             if data.get('cs_styleId'):
                 style = report.styles.get(int(data.get('cs_styleId')))
                 if style is None:
                     raise ReportBroInternalError(f'Conditional style for text element {self.id} not found')
-                # shallow copy is sufficient in our case
-                self.conditional_style = copy.copy(style)
+                self.conditional_style = style
             else:
-                self.conditional_style = TextStyle(data, key_prefix='cs_')
+                self.conditional_style = TextStyle(data, key_prefix='cs_', id_suffix='_text_cs')
         else:
             self.conditional_style = None
         # additional styles are used when text is rendered inside table row and
         # the row has a background color -> a new style is created based on the
         # existing style
         self.additional_styles = dict()
         if isinstance(self, TableTextElement):
@@ -326,14 +417,16 @@
         else:
             # set text_lines so is_printed can check for empty element when rendering spreadsheet
             self.text_lines = [content] if content else []
 
     def get_style(self, style_id, background_color, base_style):
         if style_id in self.additional_styles:
             return self.additional_styles[style_id]
+
+        # copy is needed because the background_color of the style is modified,
         # shallow copy is sufficient in our case
         style = copy.copy(base_style)
         style.id = style_id
         style.background_color = background_color
         self.additional_styles[style_id] = style
         return style
 
@@ -351,15 +444,15 @@
             elif self.used_style.vertical_alignment == VerticalAlignment.middle:
                 self.space_top = remaining_space / 2
                 self.space_bottom = remaining_space / 2
             elif self.used_style.vertical_alignment == VerticalAlignment.bottom:
                 self.space_top = remaining_space
         self.total_height = total_height + self.space_top + self.space_bottom
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         available_height = container_height - offset_y
         if self.always_print_on_same_page and self.first_render_element and\
                 self.total_height > available_height and (offset_y != 0 or container_top != 0):
             return None, False
 
         lines = []
         remaining_height = available_height
@@ -375,15 +468,15 @@
         if self.space_top == 0:
             while self.line_index < self.lines_count:
                 last_line = (self.line_index >= self.lines_count - 1)
                 line_height = self.text_lines[self.line_index].height
                 tmp_height = line_height
                 if self.line_index == 0:
                     tmp_height += self.used_style.padding_top
-                if  last_line:
+                if last_line:
                     tmp_height += self.used_style.padding_bottom
                 if tmp_height > remaining_height:
                     break
                 lines.append(self.text_lines[self.line_index])
                 remaining_height -= tmp_height
                 block_height += tmp_height
                 text_height += line_height
@@ -882,15 +975,15 @@
                 ctx.pop_context()
                 self.row_index += 1
 
         if self.footer:
             self.footer.set_printed_cells(ctx)
             self.footer.prepare(ctx)
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         self.render_y = offset_y
         self.render_bottom = self.render_y
         if self.is_rendering_complete():
             self.rendering_complete = True
             return None, True
         render_element = TableRenderElement(self.report, table=self, render_y=offset_y)
 
@@ -1356,15 +1449,15 @@
 
     def prepare(self, ctx, pdf_doc, only_verify):
         self.container.prepare(ctx, pdf_doc=pdf_doc, only_verify=only_verify)
         self.next_page_rendering_complete = False
         self.prev_page_content_height = 0
         self.render_element_type = RenderElementType.none
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         self.render_y = offset_y
         available_height = container_height - offset_y
         content_height = container_height
         render_element = FrameRenderElement(self.report, self, render_y=offset_y)
 
         if self.border_style.border_top and self.render_element_type == RenderElementType.none:
             content_height -= self.border_style.border_width
@@ -1604,15 +1697,15 @@
                 ctx.push_context(self.row_parameters, self.rows[self.row_index])
                 self.content.prepare(ctx, pdf_doc=None, only_verify=True)
                 ctx.pop_context()
                 self.row_index += 1
             if self.footer:
                 self.footer.prepare(ctx, pdf_doc=None, only_verify=True)
 
-    def get_next_render_element(self, offset_y, container_top, container_height, ctx, pdf_doc):
+    def get_next_render_element(self, offset_y, container_top, container_width, container_height, ctx, pdf_doc):
         self.render_y = offset_y
         self.render_bottom = self.render_y
         render_element = SectionRenderElement(self.report, render_y=offset_y)
 
         if self.print_header:
             self.header.create_render_elements(offset_y, container_top, container_height, ctx, pdf_doc)
             render_element.add_section_band(self.header)
```

### Comparing `reportbro_lib-3.1.0/reportbro/enums.py` & `reportbro_lib-3.2.0/reportbro/enums.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/reportbro/errors.py` & `reportbro_lib-3.2.0/reportbro/errors.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/reportbro/reportbro.py` & `reportbro_lib-3.2.0/reportbro/reportbro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Copyright (C) 2017-2022 jobsta
 #
 # This file is part of ReportBro, a library to generate PDF and Excel reports.
 # Demos can be found at https://www.reportbro.com
 #
 # Dual licensed under AGPLv3 and ReportBro commercial license:
 # https://www.reportbro.com/license
@@ -15,18 +14,20 @@
 #
 
 import base64
 import fpdf
 import importlib.resources
 import re
 import os
+import urllib
 import xlsxwriter
 from copy import deepcopy
 from babel import Locale
 from io import BufferedReader, IOBase
+from datetime import datetime
 
 from .containers import ReportBand
 from .elements import *
 from .enums import *
 from .errors import Error, ReportBroError, ReportBroInternalError
 from .structs import Parameter, TextStyle
 from .utils import get_int_value, parse_datetime_string
@@ -47,14 +48,15 @@
             encode_error_handling=encode_error_handling, core_fonts_encoding=core_fonts_encoding)
         self.pdf_doc.set_margins(0, 0)
         self.pdf_doc.c_margin = 0  # interior cell margin
         self.context = context
         self.filename = filename
         self.add_watermark = add_watermark
         self.page_limit = page_limit
+        self.creation_date = report.creation_date
 
     def add_page(self):
         self.pdf_doc.add_page()
         self.context.inc_page_number()
 
     def is_finished(self):
         return self.content_band.is_finished()
@@ -123,26 +125,31 @@
                 self.footer_band.reset()
 
             self.content_band.render_pdf(
                 self.document_properties.margin_left, content_offset_y, self.pdf_doc, cleanup=True)
 
         self.header_band.cleanup()
         self.footer_band.cleanup()
-        dest = 'F' if self.filename else 'S'
-        return self.pdf_doc.output(name=self.filename, dest=dest)
+
+        if self.creation_date:
+            self.pdf_doc.set_creation_date(self.creation_date)
+
+        return self.pdf_doc.output(name=self.filename)
 
 
 class DocumentXLSXRenderer:
     def __init__(self, header_band, content_band, footer_band, report, context, filename):
         self.header_band = header_band
         self.content_band = content_band
         self.footer_band = footer_band
         self.document_properties = report.document_properties
         self.workbook_mem = BytesIO()
         self.workbook = xlsxwriter.Workbook(filename if filename else self.workbook_mem)
+        if report.creation_date:
+            self.workbook.set_properties({'created': report.creation_date})
         self.worksheet = self.workbook.add_worksheet()
         self.context = context
         self.filename = filename
         self.row = 0
         self.column_widths = []
 
     def render(self):
@@ -288,14 +295,20 @@
         else:
             self.footer_display = BandDisplay.never
             self.footer_size = 0
         if self.content_height == 0:
             self.content_height = self.page_height - self.header_size - self.footer_size -\
                 self.margin_top - self.margin_bottom
 
+        creation_date = data.get('creationDate')
+        if creation_date:
+            self.creation_date = parse_datetime_string(creation_date)
+        else:
+            self.creation_date = None
+
 
 class ImageData:
     def __init__(self, ctx, image_id, source, image_file, is_test_data, headers):
         self.image_data = None
         self.image_type = None
         image_uri = None  # can be either url or file path
         image_url = None
@@ -402,16 +415,15 @@
         self.available_fonts = dict(
             courier=dict(standard_font=True),
             helvetica=dict(standard_font=True),
             times=dict(standard_font=True))
         if additional_fonts:
             for additional_font in additional_fonts:
                 filename = additional_font.get('filename', '')
-                font = dict(
-                    standard_font=False, uni=additional_font.get('uni', True))
+                font = dict(standard_font=False)
 
                 regular_style = dict(
                     font_filename=filename, style='', font_added=False)
                 bold_style = dict(
                     font_filename=additional_font.get('bold_filename', filename),
                     style='B', font_added=False)
                 italic_style = dict(
@@ -442,22 +454,24 @@
 
     def add_image(self, img, image_key):
         self.loaded_images[image_key] = img
 
     def get_image(self, image_key):
         return self.loaded_images.get(image_key)
 
-    def set_font(self, family, style='', size=0, underline=False):
+    def set_font(self, family=None, style='', size=0, underline=False):
         """Set font in underlying pdf renderer.
 
         This font is used for all following text rendering calls until changed again.
 
         :param family: name of the font which must either be one of the standard
         fonts (courier, helvetica, times) or added to ReportBro instance with the
         additional_fonts setting.
+        :param style: empty string (by default) or a combination of one or several
+        letters among B (bold), I (italic) and U (underline).
         :param size: font size, if not set then the standard font size is used.
         :param underline: True if text should be rendered with underlined style.
         :return: True if font exists, False otherwise.
         """
         font = self.available_fonts.get(family)
         if font:
             if not font['standard_font']:
@@ -469,16 +483,15 @@
                     # style could be different in case styles are mapped,
                     # e.g. if bold style has same font file as regular style
                     style = style_font['style']
                 else:
                     style_font = font['style']
 
                 if not style_font['font_added']:
-                    self.add_font(
-                        family, style=style, fname=style_font['font_filename'], uni=font['uni'])
+                    self.add_font(family, style=style, fname=style_font['font_filename'])
                     style_font['font_added'] = True
 
             if underline:
                 style += 'U'
             fpdf.FPDF.set_font(self, family, style, size)
             return True
         else:
@@ -610,14 +623,16 @@
                           is_test_data=is_test_data, parents=[])
         try:
             if not self.errors:
                 self.evaluate_parameters(parameter_list, self.data)
         except ReportBroError as err:
             self.errors.append(err.error)
 
+        self.creation_date = None
+
     def load_image(self, image_key, ctx, image_id, source, image_file):
         # test if image is not already loaded into image cache
         if image_key not in self.images:
             image = ImageData(ctx, image_id, source, image_file, self.is_test_data, headers=self.request_headers)
             self.images[image_key] = image
 
     def get_image(self, image_key):
@@ -898,7 +913,10 @@
                     object_id=parameter.id, field='expression', context=parameter.name))
 
         if valid_value:
             if dest_data is not None:
                 dest_data[parameter.name] = value
             else:
                 data[parameter.name] = value
+
+    def set_creation_date(self, creation_date):
+        self.creation_date = parse_datetime_string(creation_date)
```

### Comparing `reportbro_lib-3.1.0/reportbro/utils.py` & `reportbro_lib-3.2.0/reportbro/utils.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.1.0/PKG-INFO` & `reportbro_lib-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportbro-lib
-Version: 3.1.0
+Version: 3.2.0
 Summary: Generate PDF and Excel reports from visually designed templates
 Home-page: https://www.reportbro.com
 License: AGPL-3.0
 Keywords: pdf,excel,report,generate,create,web,template,layout
 Author: jobsta
 Author-email: alex@reportbro.com
 Requires-Python: >=3.7,<4.0
@@ -22,16 +22,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Babel (>=2.10.2,<3.0.0)
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: XlsxWriter (>=3.0.3,<4.0.0)
-Requires-Dist: qrcode (>=7.3.1,<8.0.0)
-Requires-Dist: reportbro-fpdf2 (>=0.9.1,<0.10.0)
+Requires-Dist: python-barcode (>=0.14.0,<0.15.0)
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
+Requires-Dist: reportbro-fpdf2 (>=2.7.1,<3.0.0)
 Requires-Dist: reportbro-simpleeval (>=0.9.11,<0.10.0)
 Project-URL: Documentation, https://www.reportbro.com/doc/installation
 Project-URL: Repository, https://github.com/jobsta/reportbro-lib
 Description-Content-Type: text/x-rst
 
 ReportBro Lib
 =================
@@ -72,15 +73,17 @@
 For pull requests the same coding styles should be used.
 
 License
 -------
 
 - Commercial license
 
-If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index.
+If you want to use ReportBro to develop commercial applications and projects, the Commercial license is the appropriate license. With this license, your source code is kept proprietary. Purchase a ReportBro Commercial license at https://www.reportbro.com/license/index
+
+This license includes ReportBro PLUS with additional features.
 
 - Open-source license
 
 If you are creating an open-source application under a license compatible with the `GNU AGPL license v3 <https://www.gnu.org/licenses/agpl-3.0.html>`_, you may use ReportBro under the terms of the AGPLv3.
 
 Read more about ReportBro's license options at https://www.reportbro.com/license/index.
```

