# Comparing `tmp/sphinx_pdf_generate-0.0.2.tar.gz` & `tmp/sphinx_pdf_generate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_pdf_generate-0.0.2.tar", max compression
+gzip compressed data, was "sphinx_pdf_generate-0.0.3.tar", max compression
```

## Comparing `sphinx_pdf_generate-0.0.2.tar` & `sphinx_pdf_generate-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1068 2023-05-07 01:56:49.720092 sphinx_pdf_generate-0.0.2/LICENSE.md
--rw-r--r--   0        0        0     5646 2023-05-07 01:56:49.720092 sphinx_pdf_generate-0.0.2/README.rst
--rw-r--r--   0        0        0     3311 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/__init__.py
--rw-r--r--   0        0        0      115 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/__main__.py
--rw-r--r--   0        0        0     1897 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/build.py
--rw-r--r--   0        0        0     5288 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cli.py
--rw-r--r--   0        0        0     2437 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cover.py
--rw-r--r--   0        0        0     3029 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/generate_txt.py
--rw-r--r--   0        0        0      171 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/logging.py
--rw-r--r--   0        0        0     3860 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/options.py
--rw-r--r--   0        0        0     9834 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/pdf_generate.py
--rw-r--r--   0        0        0       58 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/__init__.py
--rw-r--r--   0        0        0       67 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/__init__.py
--rw-r--r--   0        0        0      837 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/tabbed_block.py
--rw-r--r--   0        0        0       67 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/__init__.py
--rw-r--r--   0        0        0     1970 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/util.py
--rw-r--r--   0        0        0     2482 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/prep.py
--rw-r--r--   0        0        0     6169 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/renderer.py
--rw-r--r--   0        0        0     3135 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/__init__.py
--rw-r--r--   0        0        0     1294 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/_paging.css
--rw-r--r--   0        0        0     1777 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/cover.css
--rw-r--r--   0        0        0     1659 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/toc.css
--rw-r--r--   0        0        0        0 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/__init__.py
--rw-r--r--   0        0        0     1272 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/default_cover.html.j2
--rw-r--r--   0        0        0      437 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/__init__.py
--rw-r--r--   0        0        0      184 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/datetime.py
--rw-r--r--   0        0        0      924 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/url.py
--rw-r--r--   0        0        0     5038 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/template.py
--rw-r--r--   0        0        0        0 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/__init__.py
--rw-r--r--   0        0        0     3689 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/alabaster.py
--rw-r--r--   0        0        0      456 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/generic.py
--rw-r--r--   0        0        0    11433 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/immaterial_styles.css
--rw-r--r--   0        0        0     1852 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/material_styles.css
--rw-r--r--   0        0        0     4270 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_immaterial.py
--rw-r--r--   0        0        0     4273 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_material.py
--rw-r--r--   0        0        0     5841 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/toc.py
--rw-r--r--   0        0        0     3780 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/utils.py
--rw-r--r--   0        0        0       22 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/version.py
--rw-r--r--   0        0        0     7469 1970-01-01 00:00:00.000000 sphinx_pdf_generate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-17 07:35:29.209722 sphinx_pdf_generate-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     5793 2023-05-17 07:35:29.209722 sphinx_pdf_generate-0.0.3/README.rst
+-rw-r--r--   0        0        0     3310 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/__main__.py
+-rw-r--r--   0        0        0     1900 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/build.py
+-rw-r--r--   0        0        0     5288 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/cli.py
+-rw-r--r--   0        0        0     2437 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/cover.py
+-rw-r--r--   0        0        0      171 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/logging.py
+-rw-r--r--   0        0        0     3860 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/options.py
+-rw-r--r--   0        0        0    10080 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/pdf_generate.py
+-rw-r--r--   0        0        0       58 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/content/__init__.py
+-rw-r--r--   0        0        0      837 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/content/tabbed_block.py
+-rw-r--r--   0        0        0       67 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/links/__init__.py
+-rw-r--r--   0        0        0     1983 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/links/util.py
+-rw-r--r--   0        0        0     2482 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/prep.py
+-rw-r--r--   0        0        0     6169 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/renderer.py
+-rw-r--r--   0        0        0     3135 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/_paging.css
+-rw-r--r--   0        0        0     1777 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/cover.css
+-rw-r--r--   0        0        0     1659 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/toc.css
+-rw-r--r--   0        0        0        0 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/__init__.py
+-rw-r--r--   0        0        0     1272 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/default_cover.html.j2
+-rw-r--r--   0        0        0      437 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/filters/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/filters/datetime.py
+-rw-r--r--   0        0        0      924 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/filters/url.py
+-rw-r--r--   0        0        0     5038 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/template.py
+-rw-r--r--   0        0        0        0 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/__init__.py
+-rw-r--r--   0        0        0     3689 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/alabaster.py
+-rw-r--r--   0        0        0      456 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/generic.py
+-rw-r--r--   0        0        0    11433 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/immaterial_styles.css
+-rw-r--r--   0        0        0     1852 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/material_styles.css
+-rw-r--r--   0        0        0     4270 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/sphinx_immaterial.py
+-rw-r--r--   0        0        0     4273 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/sphinx_material.py
+-rw-r--r--   0        0        0     5835 2023-05-17 07:35:29.213722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/toc.py
+-rw-r--r--   0        0        0     3780 2023-05-17 07:35:29.217722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/utils.py
+-rw-r--r--   0        0        0       22 2023-05-17 07:35:29.217722 sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/version.py
+-rw-r--r--   0        0        0     7616 1970-01-01 00:00:00.000000 sphinx_pdf_generate-0.0.3/PKG-INFO
```

### Comparing `sphinx_pdf_generate-0.0.2/LICENSE.md` & `sphinx_pdf_generate-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/README.rst` & `sphinx_pdf_generate-0.0.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 .. |github-issues| replace:: GitHub issues
 
 .. _weasyprint-linux: https://weasyprint.readthedocs.io/en/latest/install.html#linux
 
 .. |weasyprint-linux| replace:: Linux
 
-.. _weasyprint-macos: https://weasyprint.readthedocs.io/en/latest/install.html#os-x
+.. _weasyprint-macos: https://weasyprint.readthedocs.io/en/latest/install.html#macos
 
 .. |weasyprint-macos| replace:: MacOS
 
 .. _weasyprint-windows: https://weasyprint.readthedocs.io/en/latest/install.html#windows
 
 .. |weasyprint-windows| replace:: Windows
 
@@ -31,16 +31,16 @@
    :alt: Downloads
 .. image:: https://img.shields.io/pypi/l/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: License
 .. image:: https://img.shields.io/pypi/pyversions/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: Supported versions
-.. image:: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/workflows/main.yaml/badge.svg
-   :target: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/main.yaml
+.. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/main.yaml
    :alt: GitHub Docs CI Action status
 .. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/ci.yaml/badge.svg
    :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions
    :alt: GitHub CI Action status
 .. image:: https://img.shields.io/pypi/v/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: PyPI Package latest release
@@ -56,14 +56,16 @@
 Sphinx-PDF-Generate extension generates separate PDF files from each HTML page derived from your Sphinx RST files page
 in your Sphinx documentation using `WeasyPrint <http://weasyprint.org/>`_.
 
 The extension supports many advanced features such as table of contents, customisable cover page
 , support for CSS paged media module `CSS paged media module <https://developer.mozilla.org/en-US/docs/Web/CSS/@page>`_
 , and using Sphinx page metadata to generate cover page.
 
+If you find Sphinx-PDF Generate useful, please consider `starring  <https://github.com/iSOLveIT/sphinx-pdf-generate>`_ the project. Thank you!
+
 Requirements
 ------------
 
 1. This package requires Sphinx version 5.0 or higher.
 2. Python 3.8 or higher
 3. WeasyPrint depends on cairo, Pango and GDK-PixBuf which need to be installed separately. Please follow the installation instructions for your platform carefully:
     - |weasyprint-linux|_
```

### Comparing `sphinx_pdf_generate-0.0.2/pyproject.toml` & `sphinx_pdf_generate-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sphinx-pdf-generate"
 
-# !! Don't miss updates in __init__.py, and changelog.rst!!!
-version = "0.0.2"
+# !! Don't miss updates in version.py, and changelog.rst!!!
+version = "0.0.3"
 
 description = "A Sphinx extension to generate individual PDF files for each documentation page."
 authors = ["Duodu Randy <duodurandy19@gmail.com>"]
 license = "MIT"
 maintainers = [
     "Duodu Randy <duodurandy19@gmail.com>",
 ]
```

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/build.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 def show(*, context: Optional[str] = None, command: Union[list, tuple, None] = None, error: Optional[bool] = None):
     """Show context and command-to-be-executed, with nice formatting and colors."""
     if context is not None:
         _log(context, colour=Fore.CYAN)
     if command is not None:
         assert isinstance(command, (list, tuple))
-        _log("> " + " ".join(shlex.quote(s) for s in command), colour=Fore.BLUE)
+        _log("> " + " ".join(shlex.quote(s) for s in command), colour=Fore.MAGENTA)
     if error is not None:
         _log(context, colour=Fore.RED)
 
 
 def get_builder(sphinx_args: List[str]) -> int:
     """Prepare the function that calls sphinx."""
     sphinx_command = [sys.executable, "-m", "sphinx"] + sphinx_args
```

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cli.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cover.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/cover.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/options.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/options.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/pdf_generate.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/pdf_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from timeit import default_timer as timer
 from typing import Any, Dict
 
 from docutils import nodes
 from sphinx.application import Sphinx
 from sphinx.util import docutils
 
+from sphinx_pdf_generate.build import show
 from sphinx_pdf_generate.logging import get_logger
 from sphinx_pdf_generate.options import Options
 from sphinx_pdf_generate.renderer import Renderer
 from sphinx_pdf_generate.templates.filters.url import URLFilter
 from sphinx_pdf_generate.utils import get_pdf_metadata, h1_title_tag, secure_filename
 from sphinx_pdf_generate.version import __version__
 
@@ -104,14 +105,18 @@
         toc_level=app.config.pdfgen_toc_level,
         cover_images=app.config.pdfgen_cover_images,
         theme_name=app.config.html_theme,
         templates_path=app.config.templates_path,
     )
 
     local_options = app.env.sphinx_pdfgen_data
+    if "genindex" in local_options:
+        local_options["genindex"] = {"pdf-build": "False"}
+    if "search" in local_options:
+        local_options["search"] = {"pdf-build": "False"}
     pdf_metadata = {"GLOBAL_OPTIONS": global_options, "LOCAL_OPTIONS": local_options}
 
     path_to_save_metadata = Path(app.outdir).joinpath("pdf_metadata.json")
     with open(path_to_save_metadata, "w") as json_file:
         json.dump(pdf_metadata, json_file, indent=4)
 
 
@@ -184,40 +189,41 @@
 
         if build_pdf_document and Path(self._config["srcdir"]).joinpath(src_path).exists():
             self._options.body_title = h1_title_tag(html_content, pdf_meta.get("title"))
 
             file_name = pdf_meta.get("filename") or pdf_meta.get("title") or self._options.body_title or None
             if file_name is None:
                 file_name = str(pagename).split("/")[-1]
-                self._logger.error(
-                    f"You must set the filename metadata in {pagename}.rst so we can use in the PDF document. "
-                    f"The source filename is used as fallback."
+                show(
+                    context=f"You must set the filename metadata in {pagename}.rst so we can use in the PDF document. "
+                    f"The source filename is used as fallback.",
+                    error=True,
                 )
 
             # Generate a secure filename
             file_name = secure_filename(file_name)
             base_url = dest_path.joinpath(file_name).as_uri()
             pdf_file = file_name + ".pdf"
 
             try:
-                self._logger.info(f"Converting {src_path} to {pdf_file}")
+                show(context=f"Converting {src_path} to {pdf_file}")
                 self.renderer.write_pdf(
                     html_content,
                     base_url,
                     dest_path.joinpath(pdf_file),
                     pdf_metadata=pdf_meta,
                 )
 
                 html_content = self.renderer.add_link(html_content, pdf_file)
                 self.pdf_num_files += 1
             except Exception as e:
                 self.num_errors += 1
                 raise PDFGenerateException(f"Error converting {src_path}. Reason: {e}")
         else:
-            self._logger.info(f"Skipped: PDF conversion for {src_path}")
+            show(context=f"Skipped: PDF conversion for {src_path}")
 
         end = timer()
         self.total_time += end - start
         return html_content
 
 
 class PDFGenerateException(Exception):
```

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/tabbed_block.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/content/tabbed_block.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/util.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/links/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def rel_html_href(base_url: str, href: str, site_url: str, outdir: str):
     new_base_url = os.path.dirname(base_url)
     rel_url = new_base_url.replace("file://", "")
     pattern = r"^(/tmp|tmp)/pages[\w\-]+|^[\w\-:\\]+\\+(temp|Temp)\\+pages[\w\-]+|^{}".format(outdir.rstrip("/"))
     replace_build_dir = re.compile(pattern)
 
     internal = href.startswith("#")
-    web_url = re.search(r"^(https://|http://)", href)
+    web_url = re.search(r"^(https://|http://|mailto:|tel:)", href)
     if web_url or internal or not is_doc(href):
         return href
 
     abs_html_href = Path(rel_url).joinpath(href).resolve()
     abs_html_href = replace_build_dir.sub(site_url.rstrip("/"), str(abs_html_href))
     abs_html_href = abs_html_href.replace("\\", "/")
```

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/prep.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/preprocessor/prep.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/renderer.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/renderer.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/__init__.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/_paging.css` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/_paging.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/cover.css` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/cover.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/toc.css` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/styles/toc.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/default_cover.html.j2` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/default_cover.html.j2`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/url.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/filters/url.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/template.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/templates/template.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/alabaster.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/alabaster.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/immaterial_styles.css` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/immaterial_styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/material_styles.css` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/material_styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_immaterial.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/sphinx_immaterial.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_material.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/themes/sphinx_material.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/toc.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/toc.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # exclude_lv2 = exclude_lv3 = False
 
     def makelink(heading: PageElement) -> PageElement:
         li = soup.new_tag("li")
         ref = heading.get("id", "")
         if ref == "":
             ref = heading.parent.get("id")  # support for all sphinx themes
-        prefix = heading.get("data-numbering", None)
+        prefix = heading.get("data-numbering")
         a = (
             soup.new_tag("a", href=f"#{ref}", attrs={"data-numbering": prefix})
             if prefix is not None
             else soup.new_tag("a", href=f"#{ref}")
         )
         for el in heading.contents:
             if el.name == "a":
```

### Comparing `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/utils.py` & `sphinx_pdf_generate-0.0.3/sphinx_pdf_generate/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.2/PKG-INFO` & `sphinx_pdf_generate-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-pdf-generate
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Sphinx extension to generate individual PDF files for each documentation page.
 Home-page: https://github.com/iSOLveIT/sphinx-pdf-generate
 License: MIT
 Author: Duodu Randy
 Author-email: duodurandy19@gmail.com
 Maintainer: Duodu Randy
 Maintainer-email: duodurandy19@gmail.com
@@ -46,15 +46,15 @@
 
 .. |github-issues| replace:: GitHub issues
 
 .. _weasyprint-linux: https://weasyprint.readthedocs.io/en/latest/install.html#linux
 
 .. |weasyprint-linux| replace:: Linux
 
-.. _weasyprint-macos: https://weasyprint.readthedocs.io/en/latest/install.html#os-x
+.. _weasyprint-macos: https://weasyprint.readthedocs.io/en/latest/install.html#macos
 
 .. |weasyprint-macos| replace:: MacOS
 
 .. _weasyprint-windows: https://weasyprint.readthedocs.io/en/latest/install.html#windows
 
 .. |weasyprint-windows| replace:: Windows
 
@@ -75,16 +75,16 @@
    :alt: Downloads
 .. image:: https://img.shields.io/pypi/l/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: License
 .. image:: https://img.shields.io/pypi/pyversions/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: Supported versions
-.. image:: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/workflows/main.yaml/badge.svg
-   :target: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/main.yaml
+.. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/main.yaml
    :alt: GitHub Docs CI Action status
 .. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/ci.yaml/badge.svg
    :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions
    :alt: GitHub CI Action status
 .. image:: https://img.shields.io/pypi/v/sphinx-pdf-generate.svg
    :target: https://pypi.python.org/pypi/sphinx-pdf-generate
    :alt: PyPI Package latest release
@@ -100,14 +100,16 @@
 Sphinx-PDF-Generate extension generates separate PDF files from each HTML page derived from your Sphinx RST files page
 in your Sphinx documentation using `WeasyPrint <http://weasyprint.org/>`_.
 
 The extension supports many advanced features such as table of contents, customisable cover page
 , support for CSS paged media module `CSS paged media module <https://developer.mozilla.org/en-US/docs/Web/CSS/@page>`_
 , and using Sphinx page metadata to generate cover page.
 
+If you find Sphinx-PDF Generate useful, please consider `starring  <https://github.com/iSOLveIT/sphinx-pdf-generate>`_ the project. Thank you!
+
 Requirements
 ------------
 
 1. This package requires Sphinx version 5.0 or higher.
 2. Python 3.8 or higher
 3. WeasyPrint depends on cairo, Pango and GDK-PixBuf which need to be installed separately. Please follow the installation instructions for your platform carefully:
     - |weasyprint-linux|_
```

