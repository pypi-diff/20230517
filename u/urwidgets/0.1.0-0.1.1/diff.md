# Comparing `tmp/urwidgets-0.1.0.tar.gz` & `tmp/urwidgets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urwidgets-0.1.0.tar", last modified: Sun May 14 21:58:00 2023, max compression
+gzip compressed data, was "urwidgets-0.1.1.tar", last modified: Wed May 17 21:35:33 2023, max compression
```

## Comparing `urwidgets-0.1.0.tar` & `urwidgets-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-14 21:58:00.765734 urwidgets-0.1.0/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-03 17:30:15.000000 urwidgets-0.1.0/LICENSE
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2825 2023-05-14 21:58:00.765734 urwidgets-0.1.0/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1496 2023-05-14 20:51:57.000000 urwidgets-0.1.0/README.md
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      148 2023-03-03 18:11:46.000000 urwidgets-0.1.0/pyproject.toml
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-05-14 21:58:00.765734 urwidgets-0.1.0/setup.cfg
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1623 2023-05-14 21:51:05.000000 urwidgets-0.1.0/setup.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-14 21:58:00.762400 urwidgets-0.1.0/src/
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-14 21:58:00.765734 urwidgets-0.1.0/src/urwidgets/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      816 2023-05-14 21:51:05.000000 urwidgets-0.1.0/src/urwidgets/__init__.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     5938 2023-04-30 17:11:49.000000 urwidgets-0.1.0/src/urwidgets/hyperlink.py
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    23640 2023-05-14 21:42:42.000000 urwidgets-0.1.0/src/urwidgets/text_embed.py
-drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-14 21:58:00.765734 urwidgets-0.1.0/src/urwidgets.egg-info/
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2825 2023-05-14 21:58:00.000000 urwidgets-0.1.0/src/urwidgets.egg-info/PKG-INFO
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      306 2023-05-14 21:58:00.000000 urwidgets-0.1.0/src/urwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-05-14 21:58:00.000000 urwidgets-0.1.0/src/urwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       16 2023-05-14 21:58:00.000000 urwidgets-0.1.0/src/urwidgets.egg-info/requires.txt
--rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       10 2023-05-14 21:58:00.000000 urwidgets-0.1.0/src/urwidgets.egg-info/top_level.txt
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-17 21:35:33.012691 urwidgets-0.1.1/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1076 2023-03-03 17:30:15.000000 urwidgets-0.1.1/LICENSE
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2868 2023-05-17 21:35:33.012691 urwidgets-0.1.1/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1539 2023-05-17 21:29:22.000000 urwidgets-0.1.1/README.md
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      148 2023-03-03 18:11:46.000000 urwidgets-0.1.1/pyproject.toml
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       38 2023-05-17 21:35:33.012691 urwidgets-0.1.1/setup.cfg
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     1623 2023-05-17 21:25:32.000000 urwidgets-0.1.1/setup.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-17 21:35:33.009357 urwidgets-0.1.1/src/
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-17 21:35:33.009357 urwidgets-0.1.1/src/urwidgets/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      816 2023-05-17 21:25:32.000000 urwidgets-0.1.1/src/urwidgets/__init__.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     6441 2023-05-17 21:19:42.000000 urwidgets-0.1.1/src/urwidgets/hyperlink.py
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)    23646 2023-05-17 21:19:42.000000 urwidgets-0.1.1/src/urwidgets/text_embed.py
+drwxr-xr-x   0 anonymoux47  (1000) anonymoux47  (1001)        0 2023-05-17 21:35:33.012691 urwidgets-0.1.1/src/urwidgets.egg-info/
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)     2868 2023-05-17 21:35:33.000000 urwidgets-0.1.1/src/urwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)      306 2023-05-17 21:35:33.000000 urwidgets-0.1.1/src/urwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)        1 2023-05-17 21:35:33.000000 urwidgets-0.1.1/src/urwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       16 2023-05-17 21:35:33.000000 urwidgets-0.1.1/src/urwidgets.egg-info/requires.txt
+-rw-r--r--   0 anonymoux47  (1000) anonymoux47  (1001)       10 2023-05-17 21:35:33.000000 urwidgets-0.1.1/src/urwidgets.egg-info/top_level.txt
```

### Comparing `urwidgets-0.1.0/LICENSE` & `urwidgets-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urwidgets-0.1.0/PKG-INFO` & `urwidgets-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urwidgets
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of widgets for urwid (https://urwid.org)
 Home-page: https://github.com/AnonymouX47/urwidgets
 Author: AnonymouX47
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/urwidgets/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://urwidgets.readthedocs.io/
@@ -39,14 +39,15 @@
 - [Contribution](#contribution)
 - [Donate](#donate)
 
 
 ## Installation
 
 ### Requirements
+- [Python](https://www.python.org/) >= 3.7
 - [urwid](https://github.com/urwid/urwid/wiki/Installation-instructions) (will be installed automatically)
 
 ### Steps
 The latest **stable** version can be installed from [PyPI](https://pypi.org/project/urwidgets) with:
 
 ```shell
 pip install urwidgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urwidgets Version: 0.1.0 Summary: A collection of
+Metadata-Version: 2.1 Name: urwidgets Version: 0.1.1 Summary: A collection of
 widgets for urwid (https://urwid.org) Home-page: https://github.com/
 AnonymouX47/urwidgets Author: AnonymouX47 Author-email: anonymoux47@gmail.com
 License: MIT Project-URL: Changelog, https://github.com/AnonymouX47/urwidgets/
 blob/main/CHANGELOG.md Project-URL: Documentation, https://
 urwidgets.readthedocs.io/ Project-URL: Source, https://github.com/AnonymouX47/
 urwidgets Project-URL: Tracker, https://github.com/AnonymouX47/urwidgets/issues
 Keywords: terminal,console,xterm,library,tui,urwid,curses Classifier:
@@ -14,20 +14,21 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # urWIDgets A
 collection of widgets for [urwid](https://urwid.org) ## Contents -
 [Installation](#installation) - [Usage](#usage) - [Contribution](#contribution)
-- [Donate](#donate) ## Installation ### Requirements - [urwid](https://
-github.com/urwid/urwid/wiki/Installation-instructions) (will be installed
-automatically) ### Steps The latest **stable** version can be installed from
-[PyPI](https://pypi.org/project/urwidgets) with: ```shell pip install urwidgets
-``` The **development** version can be installed with: ```shell pip install
-git+https://github.com/AnonymouX47/urwidgets.git ``` ## Usage
+- [Donate](#donate) ## Installation ### Requirements - [Python](https://
+www.python.org/) >= 3.7 - [urwid](https://github.com/urwid/urwid/wiki/
+Installation-instructions) (will be installed automatically) ### Steps The
+latest **stable** version can be installed from [PyPI](https://pypi.org/
+project/urwidgets) with: ```shell pip install urwidgets ``` The **development**
+version can be installed with: ```shell pip install git+https://github.com/
+AnonymouX47/urwidgets.git ``` ## Usage
   ð§ There might be incompatible changes between minor versions of version
                                      zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.1,<0.2`.** See the [docs](https://urwidgets.readthedocs.io) for the API
 Reference. ## Contribution Please read through the [guidelines](https://
 github.com/AnonymouX47/urwidgets/blob/main/CONTRIBUTING.md). ## Donate [Buy_Me
```

### Comparing `urwidgets-0.1.0/README.md` & `urwidgets-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 - [Contribution](#contribution)
 - [Donate](#donate)
 
 
 ## Installation
 
 ### Requirements
+- [Python](https://www.python.org/) >= 3.7
 - [urwid](https://github.com/urwid/urwid/wiki/Installation-instructions) (will be installed automatically)
 
 ### Steps
 The latest **stable** version can be installed from [PyPI](https://pypi.org/project/urwidgets) with:
 
 ```shell
 pip install urwidgets
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # urWIDgets A collection of widgets for [urwid](https://urwid.org) ## Contents
 - [Installation](#installation) - [Usage](#usage) - [Contribution]
-(#contribution) - [Donate](#donate) ## Installation ### Requirements - [urwid]
-(https://github.com/urwid/urwid/wiki/Installation-instructions) (will be
-installed automatically) ### Steps The latest **stable** version can be
-installed from [PyPI](https://pypi.org/project/urwidgets) with: ```shell pip
-install urwidgets ``` The **development** version can be installed with:
-```shell pip install git+https://github.com/AnonymouX47/urwidgets.git ``` ##
-Usage
+(#contribution) - [Donate](#donate) ## Installation ### Requirements - [Python]
+(https://www.python.org/) >= 3.7 - [urwid](https://github.com/urwid/urwid/wiki/
+Installation-instructions) (will be installed automatically) ### Steps The
+latest **stable** version can be installed from [PyPI](https://pypi.org/
+project/urwidgets) with: ```shell pip install urwidgets ``` The **development**
+version can be installed with: ```shell pip install git+https://github.com/
+AnonymouX47/urwidgets.git ``` ## Usage
   ð§ There might be incompatible changes between minor versions of version
                                      zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.1,<0.2`.** See the [docs](https://urwidgets.readthedocs.io) for the API
 Reference. ## Contribution Please read through the [guidelines](https://
 github.com/AnonymouX47/urwidgets/blob/main/CONTRIBUTING.md). ## Donate [Buy_Me
```

### Comparing `urwidgets-0.1.0/setup.py` & `urwidgets-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="urwidgets",
-    version="0.1.0",
+    version="0.1.1",
     author="AnonymouX47",
     author_email="anonymoux47@gmail.com",
     url="https://github.com/AnonymouX47/urwidgets",
     description="A collection of widgets for urwid (https://urwid.org)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `urwidgets-0.1.0/src/urwidgets/__init__.py` & `urwidgets-0.1.1/src/urwidgets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     TextEmbed,
     TupleMarkup,
     WidgetListMarkup,
     WidgetTupleMarkup,
     parse_text,
 )
 
-version_info = (0, 1, 0)
+version_info = (0, 1, 1)
 
 # Follows https://semver.org/spec/v2.0.0.html
 __version__ = ".".join(map(str, version_info[:3]))
 if version_info[3:]:
     __version__ += "-" + ".".join(map(str, version_info[3:]))
```

### Comparing `urwidgets-0.1.0/src/urwidgets/hyperlink.py` & `urwidgets-0.1.1/src/urwidgets/hyperlink.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 __all__ = ("Hyperlink",)
 
-from typing import Generator, List, Optional, Tuple, Union
+from typing import Generator, List, Optional, Tuple
 
 import urwid
 
+from .text_embed import DisplayAttribute
+
 # NOTE: Any new "private" attribute of any subclass of an urwid class should be
 # prepended with "_uw" to avoid clashes with names used by urwid itself.
 
 
 ESC = "\033"
 OSC = f"{ESC}]"
 ST = f"{ESC}\\"
@@ -63,49 +65,51 @@
     """
 
     no_cache = ["render"]
 
     def __init__(
         self,
         uri: str,
-        attr: Union[None, str, bytes, urwid.AttrSpec] = None,
+        attr: DisplayAttribute = None,
         text: Optional[str] = None,
     ) -> None:
         self._uw_set_uri(uri)
-        super().__init__(urwid.Text((attr, ""), "left", "ellipsis"))
-        self._uw_set_text(text or uri)
+        super().__init__(urwid.Text((_Attr(attr), ""), "left", "ellipsis"))
+        self._uw_set_text(uri if text is None else text)
 
     def render(self, size: Tuple[int,], focus: bool = False) -> urwid.HyperlinkCanvas:
         return HyperlinkCanvas(self._uw_uri, self._w.render(size, focus))
 
     def _uw_set_text(self, text: str):
         if not isinstance(text, str):
             raise TypeError(f"Invalid type for 'text' (got: {type(text).__name__!r})")
-        if "\n" in text:
+        if not text:
+            raise ValueError("Hyperlink text is empty")
+        if "\n" in text:  # Other multi-line whitespace characters are escaped by urwid
             raise ValueError(f"Multi-line text (got: {text!r})")
-        self._w.set_text(((self._w.attrib or [(None, 0)])[0][0], text))
+        self._w.set_text((self._w.attrib[0][0], text))
 
     def _uw_set_uri(self, uri: str):
         if not isinstance(uri, str):
             raise TypeError(f"Invalid type for 'uri' (got: {type(uri).__name__!r})")
         if not uri:
             raise ValueError("URI is empty")
         invalid_bytes = frozenset(uri.encode()).difference(valid_byte_range)
         if invalid_bytes:
             raise ValueError(
                 f"Invalid byte '\\x{tuple(invalid_bytes)[0]:02x}' found in URI: {uri!r}"
             )
         self._uw_uri = uri
 
     attrib = property(
-        lambda self: (self._w.attrib or [(None, 0)])[0][0],
-        lambda self, attrib: self._w.set_text((attrib, self._w.text)),
+        lambda self: self._w.attrib[0][0].attr,
+        lambda self, attrib: self._w.set_text((_Attr(attrib), self._w.text)),
         doc="""The display attirbute of the hyperlink.
 
-        :type: Union[None, str, bytes, urwid.AttrSpec]
+        :type: DisplayAttribute
 
         GET:
             Returns the display attirbute.
 
         SET:
             Sets the display attirbute.
         """,
@@ -158,31 +162,42 @@
         __class__._uw_free_ids.add(self._uw_id)
 
     def cols(self):
         return self._uw_text_canv.cols()
 
     def content(
         self, *args, **kwargs
-    ) -> Generator[
-        List[Tuple[Union[None, str, bytes, urwid.AttrSpec], Optional[str], bytes]],
-        None,
-        None,
-    ]:
-        yield [
-            (None, "U", START % (self._uw_id, self._uw_uri)),
-            # There can be only one line since wrap="ellipsis" and the text was checked
-            # to not contain "\n".
-            # There can be only one run since there was only one display attribute.
-            next(self._uw_text_canv.content(*args, **kwargs))[0],
-            (None, "U", END),
-        ]
+    ) -> Generator[List[Tuple[DisplayAttribute, Optional[str], bytes]], None, None]:
+        # There can only be one line since wrap="ellipsis" and the text was checked
+        # to not contain "\n".
+        content_line = next(self._uw_text_canv.content(*args, **kwargs))
+
+        if isinstance(content_line[0][0], _Attr):
+            hyperlink_text, *padding = content_line
+            yield [
+                (None, "U", START % (self._uw_id, self._uw_uri)),
+                (hyperlink_text[0].attr, *hyperlink_text[1:]),
+                (None, "U", END),
+                *padding,  # if any
+            ]
+        else:  # A trim containing padding only
+            yield content_line
 
     def rows(self):
         return self._uw_text_canv.rows()
 
     @staticmethod
     def _uw_get_id():
         if __class__._uw_free_ids:
             return __class__._uw_free_ids.pop()
         __class__._uw_next_id += 1
 
         return __class__._uw_next_id - 1
+
+
+class _Attr:
+    """Wraps a text display attribute to ensure it's always distinguished from those of
+    neighbouring text runs.
+    """
+
+    def __init__(self, attr: DisplayAttribute):
+        self.attr = attr
```

### Comparing `urwidgets-0.1.0/src/urwidgets/text_embed.py` & `urwidgets-0.1.1/src/urwidgets/text_embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 
 # I really hope these are correct :D
 Markup = Union["StringMarkup", "ListMarkup", "TupleMarkup"]
 StringMarkup = Union[str, bytes]
 ListMarkup = List["Markup"]
 TupleMarkup = Union["NormalTupleMarkup", "WidgetTupleMarkup"]
 NormalTupleMarkup = Tuple["DisplayAttribute", Union["StringMarkup", "ListMarkup"]]
-DisplayAttribute = Union[None, str, bytes, urwid.AttrSpec]
-WidgetTupleMarkup = Tuple[int, Union[urwid.Widget, "WidgetListMarkup"]]
-WidgetListMarkup = List[Union[urwid.Widget, "Markup", "WidgetListMarkup"]]
+DisplayAttribute = Union[None, str, bytes, "urwid.AttrSpec"]
+WidgetTupleMarkup = Tuple[int, Union["urwid.Widget", "WidgetListMarkup"]]
+WidgetListMarkup = List[Union["urwid.Widget", "Markup", "WidgetListMarkup"]]
 
 
 class TextEmbed(urwid.Text):
     """A text widget within which other widgets may be embedded.
 
     This is an extension of the :py:class:`urwid.Text` widget. Every feature and
     interface of :py:class:`~urwid.Text` is supported and works essentially the same,
```

### Comparing `urwidgets-0.1.0/src/urwidgets.egg-info/PKG-INFO` & `urwidgets-0.1.1/src/urwidgets.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urwidgets
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of widgets for urwid (https://urwid.org)
 Home-page: https://github.com/AnonymouX47/urwidgets
 Author: AnonymouX47
 Author-email: anonymoux47@gmail.com
 License: MIT
 Project-URL: Changelog, https://github.com/AnonymouX47/urwidgets/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://urwidgets.readthedocs.io/
@@ -39,14 +39,15 @@
 - [Contribution](#contribution)
 - [Donate](#donate)
 
 
 ## Installation
 
 ### Requirements
+- [Python](https://www.python.org/) >= 3.7
 - [urwid](https://github.com/urwid/urwid/wiki/Installation-instructions) (will be installed automatically)
 
 ### Steps
 The latest **stable** version can be installed from [PyPI](https://pypi.org/project/urwidgets) with:
 
 ```shell
 pip install urwidgets
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urwidgets Version: 0.1.0 Summary: A collection of
+Metadata-Version: 2.1 Name: urwidgets Version: 0.1.1 Summary: A collection of
 widgets for urwid (https://urwid.org) Home-page: https://github.com/
 AnonymouX47/urwidgets Author: AnonymouX47 Author-email: anonymoux47@gmail.com
 License: MIT Project-URL: Changelog, https://github.com/AnonymouX47/urwidgets/
 blob/main/CHANGELOG.md Project-URL: Documentation, https://
 urwidgets.readthedocs.io/ Project-URL: Source, https://github.com/AnonymouX47/
 urwidgets Project-URL: Tracker, https://github.com/AnonymouX47/urwidgets/issues
 Keywords: terminal,console,xterm,library,tui,urwid,curses Classifier:
@@ -14,20 +14,21 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # urWIDgets A
 collection of widgets for [urwid](https://urwid.org) ## Contents -
 [Installation](#installation) - [Usage](#usage) - [Contribution](#contribution)
-- [Donate](#donate) ## Installation ### Requirements - [urwid](https://
-github.com/urwid/urwid/wiki/Installation-instructions) (will be installed
-automatically) ### Steps The latest **stable** version can be installed from
-[PyPI](https://pypi.org/project/urwidgets) with: ```shell pip install urwidgets
-``` The **development** version can be installed with: ```shell pip install
-git+https://github.com/AnonymouX47/urwidgets.git ``` ## Usage
+- [Donate](#donate) ## Installation ### Requirements - [Python](https://
+www.python.org/) >= 3.7 - [urwid](https://github.com/urwid/urwid/wiki/
+Installation-instructions) (will be installed automatically) ### Steps The
+latest **stable** version can be installed from [PyPI](https://pypi.org/
+project/urwidgets) with: ```shell pip install urwidgets ``` The **development**
+version can be installed with: ```shell pip install git+https://github.com/
+AnonymouX47/urwidgets.git ``` ## Usage
   ð§ There might be incompatible changes between minor versions of version
                                      zero!
 **If you want to use this library in a project while it's still on version
 zero, ensure you pin the dependency to a specific minor version e.g
 `>=0.1,<0.2`.** See the [docs](https://urwidgets.readthedocs.io) for the API
 Reference. ## Contribution Please read through the [guidelines](https://
 github.com/AnonymouX47/urwidgets/blob/main/CONTRIBUTING.md). ## Donate [Buy_Me
```

