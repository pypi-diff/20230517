# Comparing `tmp/dirt_ssg-0.1.0.tar.gz` & `tmp/dirt_ssg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirt_ssg-0.1.0.tar", max compression
+gzip compressed data, was "dirt_ssg-0.2.0.tar", max compression
```

## Comparing `dirt_ssg-0.1.0.tar` & `dirt_ssg-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,34 @@
--rw-r--r--   0        0        0      671 2023-05-15 15:17:50.510767 dirt_ssg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/__init__.py
--rw-r--r--   0        0        0    10543 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/builder.py
--rw-r--r--   0        0        0     6102 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/checker.py
--rw-r--r--   0        0        0     2557 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/common.py
--rw-r--r--   0        0        0     8659 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/composer.py
--rw-r--r--   0        0        0     4472 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/config.py
--rw-r--r--   0        0        0     7477 2023-05-15 15:13:37.952009 dirt_ssg-0.1.0/src/dirt/conversion.py
--rw-r--r--   0        0        0      881 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/dirtcontext.py
--rw-r--r--   0        0        0     6000 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/extras.py
--rw-r--r--   0        0        0     3333 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/feeds.py
--rw-r--r--   0        0        0     3015 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/fx_pico.py
--rw-r--r--   0        0        0     1509 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/fx_tufte.py
--rw-r--r--   0        0        0     5844 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/gdocs.py
--rw-r--r--   0        0        0     5485 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/generate.py
--rw-r--r--   0        0        0     5335 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/htmlify.py
--rw-r--r--   0        0        0     6160 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/localserver.py
--rw-r--r--   0        0        0     2722 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/main.py
--rw-r--r--   0        0        0      745 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/pageinfo.py
--rw-r--r--   0        0        0     4984 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/ssg.py
--rw-r--r--   0        0        0      948 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/urls.py
--rw-r--r--   0        0        0     4958 2023-05-15 15:13:37.953009 dirt_ssg-0.1.0/src/dirt/words.py
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 dirt_ssg-0.1.0/setup.py
--rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 dirt_ssg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      725 2023-05-17 16:36:09.893576 dirt_ssg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/__init__.py
+-rw-r--r--   0        0        0    10543 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/builder.py
+-rw-r--r--   0        0        0     6102 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/checker.py
+-rw-r--r--   0        0        0     2216 2023-05-17 07:53:03.046297 dirt_ssg-0.2.0/src/dirt/common.py
+-rw-r--r--   0        0        0     8633 2023-05-17 08:52:46.624906 dirt_ssg-0.2.0/src/dirt/composer.py
+-rw-r--r--   0        0        0     4472 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/config.py
+-rw-r--r--   0        0        0     7560 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/conversion.py
+-rw-r--r--   0        0        0      881 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/dirtcontext.py
+-rw-r--r--   0        0        0     6000 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/extras.py
+-rw-r--r--   0        0        0     3333 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/feeds.py
+-rw-r--r--   0        0        0     3015 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/fx_pico.py
+-rw-r--r--   0        0        0     1509 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/fx_tufte.py
+-rw-r--r--   0        0        0     5755 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/gdocs.py
+-rw-r--r--   0        0        0     5485 2023-05-17 06:56:46.169278 dirt_ssg-0.2.0/src/dirt/generate.py
+-rw-r--r--   0        0        0     5335 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/htmlify.py
+-rw-r--r--   0        0        0     6160 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/localserver.py
+-rw-r--r--   0        0        0     2697 2023-05-17 08:51:32.920716 dirt_ssg-0.2.0/src/dirt/main.py
+-rw-r--r--   0        0        0       76 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/_config.toml
+-rw-r--r--   0        0        0      570 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/dirt.toml
+-rw-r--r--   0        0        0    72244 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/frameworks/pico/style/pico.min.css
+-rw-r--r--   0        0        0    11212 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/frameworks/tufte/style/tufte.css
+-rw-r--r--   0        0        0      194 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/index.md
+-rw-r--r--   0        0        0     1495 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/local_jscript.html
+-rw-r--r--   0        0        0      395 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/pico_template.html
+-rw-r--r--   0        0        0      375 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/rss_feed_template.xml
+-rw-r--r--   0        0        0      147 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/rss_item_template.xml
+-rw-r--r--   0        0        0      324 2023-04-19 09:21:30.367884 dirt_ssg-0.2.0/src/dirt/meta/tufte_template.html
+-rw-r--r--   0        0        0      745 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/pageinfo.py
+-rw-r--r--   0        0        0     5056 2023-05-17 07:35:25.720383 dirt_ssg-0.2.0/src/dirt/ssg.py
+-rw-r--r--   0        0        0      948 2023-04-19 09:21:30.368884 dirt_ssg-0.2.0/src/dirt/urls.py
+-rw-r--r--   0        0        0     4958 2023-05-17 06:56:46.170278 dirt_ssg-0.2.0/src/dirt/words.py
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 dirt_ssg-0.2.0/setup.py
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 dirt_ssg-0.2.0/PKG-INFO
```

### Comparing `dirt_ssg-0.1.0/pyproject.toml` & `dirt_ssg-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 [tool.poetry]
 name = "dirt-ssg"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Loren Kohnfelder"]
 packages = [
 	{ include = "dirt", from = "src" }
 ]
 
+[tool.pytest.ini_options]
+pythonpath = [
+	"./src/"
+]
+
 [tool.poetry.scripts]
 dirt = 'dirt.main:main'
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
```

### Comparing `dirt_ssg-0.1.0/src/dirt/builder.py` & `dirt_ssg-0.2.0/src/dirt/builder.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/checker.py` & `dirt_ssg-0.2.0/src/dirt/checker.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/common.py` & `dirt_ssg-0.2.0/src/dirt/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,24 +22,14 @@
 
 
 class DirtError(Exception):
     def __init__(self, message):
         self.message = message
 
 
-def dirt_dir(path):
-    """Returns file path for dirt-relative path."""
-    dir_path = os.path.join(os.path.dirname(os.path.abspath(__file__)),
-                            '../..', path)
-    dir_path = os.path.normpath(dir_path)
-    if (os.path.isdir(dir_path)):
-        return dir_path
-    raise DirtError("No such directory: %s" % path)
-
-
 def canonical_rel(path, dot=True):
     """Returns the canonical relative form of path.
     The purpose of this is to canonicalize the forms "./dir" and "dir".
     The dot parameter specifies that "./dir" is canonical, or False
     means that "dir" is. The canonical relative root is always ".".
     """
     relpath = os.path.relpath(path)
```

### Comparing `dirt_ssg-0.1.0/src/dirt/composer.py` & `dirt_ssg-0.2.0/src/dirt/composer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 __author__ = "Loren Kohnfelder"
 __copyright__ = "Copyright 2022 Loren Kohnfelder"
 __version__ = "0"
 __license__ = "CC BY-SA 4.0"
 
 
-from dirt.common import DirtError, dirt_dir, META_DIR, canonical_rel
+from dirt.common import DirtError, META_DIR, canonical_rel
 from dirt.dirtcontext import DirtContext
 from dirt.generate import soft_copyfile
 from dirt.htmlify import htmltag, htmllink
 from dirt.words import curly_expander, excerpt
+from importlib.resources import files
 
 import os
 import re
 
 
 class DirtFramework():
     """Abstract class for rendering HTML for a specific web framework for dirt.
@@ -49,29 +50,27 @@
         """Make a snippet with name and string value.
         String type snippet becomes value or list of one string is a filename,
         files are found in the meta directory.
         """
         if (type(snippet) is str):
             pass
         elif (type(snippet) is list and len(snippet) == 1):
-            metapath = dirt_dir(META_DIR)
-            filepath = os.path.join(metapath, snippet[0])
-            with open(filepath, 'r') as f:
+            with files("dirt").joinpath(META_DIR + "/" + snippet[0]).open('r') as f:
                 snippet = f.read()
         else:
             raise DirtError("Invalid [snippets] entry: " + name)
         self.cxt.snippets[name] = snippet
 
     def add_files(self, realtargetpath):
         """Add files in directory ./meta/frameworks/FXNAME to target directory.
         Returns a dictionary {(relative directory path): [file, name, list]}
         to be used to know what files belong and which should be removed.
         """
-        rootpath = dirt_dir(os.path.join(META_DIR,
-                                         "frameworks/%s" % self.nickname()))
+        framework_name = "%s/frameworks/%s" % (META_DIR, self.nickname())
+        rootpath = files('dirt').joinpath(framework_name)
         added_file_map = dict()
         for dirpath, subdirs, filenames in os.walk(rootpath):
             reldir = canonical_rel(os.path.relpath(dirpath, rootpath),
                                    dot=False)
             generated_filenames = list()
             targetdir = os.path.join(realtargetpath, reldir)
             for filename in filenames:
```

### Comparing `dirt_ssg-0.1.0/src/dirt/config.py` & `dirt_ssg-0.2.0/src/dirt/config.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/conversion.py` & `dirt_ssg-0.2.0/src/dirt/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,20 +111,23 @@
     before the markdown text it applies to, terminated by empty curlies ({}).
     {tag}markdown contents here{}
     Alternatively, write a styling expression enclosed by double quotes. Ex:
     {"styling-expression..."}markdown contents here{}
     The above will be rendered as <span style="styling-expression..."> ...
     """
     def handleMatch(self, m, data):
-        styling = re.match(r'^"(.+)"$', m.group(1))
+        inner = m.group(1)
+        styling = re.match(r'^"(.+)"$', inner)
         if styling:
             el = etree.Element('span')
             el.set('style', styling.group(1))
+        elif inner.isalpha():
+            el = etree.Element(inner)
         else:
-            el = etree.Element(m.group(1))
+            return None, None, None
         el.text = m.group(2)
         return el, m.start(0), m.end(0)
 
 
 class DirtInlineExtension(Extension):
     """Dirt extension for markdown conversion. See processor comments for more.
     {tag}markdown contents here{}
```

### Comparing `dirt_ssg-0.1.0/src/dirt/dirtcontext.py` & `dirt_ssg-0.2.0/src/dirt/dirtcontext.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/extras.py` & `dirt_ssg-0.2.0/src/dirt/extras.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/feeds.py` & `dirt_ssg-0.2.0/src/dirt/feeds.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/fx_pico.py` & `dirt_ssg-0.2.0/src/dirt/fx_pico.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/fx_tufte.py` & `dirt_ssg-0.2.0/src/dirt/fx_tufte.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/gdocs.py` & `dirt_ssg-0.2.0/src/dirt/gdocs.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,18 @@
                 url = params.get('url', None)
                 if (url):
                     basepath = os.path.join(dirpath, basename)
                     docxpath = basepath + ".docx"
                     docxhash = download_doc_file(url, docxpath)
                     if (docxhash is not None):
                         mdpath = basepath + ".md"
-                        pandoc_command = ("pandoc -f docx -t markdown "
-                                          + docxpath)
-                        process = subprocess.Popen(pandoc_command, shell=True,
-                                                   stdout=subprocess.PIPE)
-                        markdown = process.communicate()[0].decode("utf-8")
+                        pandoc_command = ["pandoc", "-f", "docx", "-t",
+                                          "markdown", docxpath]
+                        output = subprocess.check_output(pandoc_command)
+                        markdown = output.decode("utf-8")
                         with open(mdpath, 'w') as f:
                             f.write('\n'.join(meta_attrs))
                             f.write('\n\n\n')
                             f.write(markdown)
             except Exception as e:
                 print("%s: unable to download" % basename)
                 print(str(e))
```

### Comparing `dirt_ssg-0.1.0/src/dirt/generate.py` & `dirt_ssg-0.2.0/src/dirt/generate.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/htmlify.py` & `dirt_ssg-0.2.0/src/dirt/htmlify.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/localserver.py` & `dirt_ssg-0.2.0/src/dirt/localserver.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/main.py` & `dirt_ssg-0.2.0/src/dirt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,31 +11,29 @@
 __author__ = "Loren Kohnfelder"
 __copyright__ = "Copyright 2022 Loren Kohnfelder"
 __version__ = "0"
 __license__ = "CC BY-SA 4.0"
 
 
 from dirt.common import META_DIR, DIRT_TOML
+from importlib.resources import files
 
 import argparse
 from dirt.ssg import cli
-import os
 import sys
 
 
 def main(argv=None):
     """Parse command line arguments and invoke processing.
     Run with --help for full options.
     """
     parser = argparse.ArgumentParser(
         description="A dirt simple static site generator",
         epilog=("Version: %s" % __version__))
-    standard_meta_config = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)),
-        '../..', META_DIR, DIRT_TOML)
+    standard_meta_config = files('dirt').joinpath(META_DIR + "/" + DIRT_TOML)
     parser.add_argument('-c', '--config', help="root config file",
                         action='store',
                         default=standard_meta_config)
     parser.add_argument('-i', '--input', action='store',
                         help="directory of source content files",
                         default='./content/')
     parser.add_argument('-l', '--localhost', help="hostname for local server",
```

### Comparing `dirt_ssg-0.1.0/src/dirt/pageinfo.py` & `dirt_ssg-0.2.0/src/dirt/pageinfo.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/ssg.py` & `dirt_ssg-0.2.0/src/dirt/ssg.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 __license__ = "CC BY-SA 4.0"
 
 
 import dirt.localserver as localserver
 from dirt.builder import regenerate
 from dirt.checker import link_check
 from dirt.common import DirtError, META_DIR, CONFIG_TOML
-from dirt.common import dirt_dir
 from dirt.config import load_config
 from dirt.dirtcontext import DirtContext
 from dirt.extras import make_extras
+from importlib.resources import files
 
 from datetime import datetime, timezone, timedelta
 import os
 import shutil
 from typing import Optional
 
 
@@ -126,11 +126,12 @@
     return None
 
 
 def create_content_file(basepath, filename):
     """Create a content file as part of dirt start command.
     Returns the path of the newly created file.
     """
-    sourcepath = os.path.join(dirt_dir(META_DIR), filename)
+    sourcepath = files('dirt').joinpath(META_DIR + "/" + filename)
+    # todo: maybe open a file-pointer and use that for copy
     destinationpath = os.path.join(basepath, filename)
     shutil.copyfile(sourcepath, destinationpath)
     return destinationpath
```

### Comparing `dirt_ssg-0.1.0/src/dirt/urls.py` & `dirt_ssg-0.2.0/src/dirt/urls.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/src/dirt/words.py` & `dirt_ssg-0.2.0/src/dirt/words.py`

 * *Files identical despite different names*

### Comparing `dirt_ssg-0.1.0/setup.py` & `dirt_ssg-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['dirt']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'dirt': ['meta/*',
+          'meta/frameworks/pico/style/*',
+          'meta/frameworks/tufte/style/*']}
 
 install_requires = \
 ['Markdown>=3.3.7,<4.0.0', 'toml>=0.10.2,<0.11.0', 'watchdog>=2.1.8,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['dirt = dirt.main:main']}
 
 setup_kwargs = {
     'name': 'dirt-ssg',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': '',
     'long_description': 'None',
     'author': 'Loren Kohnfelder',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

