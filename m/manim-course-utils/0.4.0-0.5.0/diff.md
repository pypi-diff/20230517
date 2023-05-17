# Comparing `tmp/manim_course_utils-0.4.0.tar.gz` & `tmp/manim_course_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_course_utils-0.4.0.tar", max compression
+gzip compressed data, was "manim_course_utils-0.5.0.tar", max compression
```

## Comparing `manim_course_utils-0.4.0.tar` & `manim_course_utils-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.4.0/manim_course_utils/__init__.py
--rw-r--r--   0        0        0     2813 2023-05-11 22:33:05.730047 manim_course_utils-0.4.0/manim_course_utils/animation_description.py
--rw-r--r--   0        0        0      273 2023-05-11 22:31:05.058757 manim_course_utils-0.4.0/manim_course_utils/markdown_tex_template.py
--rw-r--r--   0        0        0     1920 2023-05-11 22:32:31.604716 manim_course_utils-0.4.0/manim_course_utils/mobject_description.py
--rw-r--r--   0        0        0      521 2023-05-11 22:35:40.441599 manim_course_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.4.0/README.md
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 manim_course_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.5.0/manim_course_utils/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-11 22:33:05.730047 manim_course_utils-0.5.0/manim_course_utils/animation_description.py
+-rw-r--r--   0        0        0      273 2023-05-11 22:31:05.058757 manim_course_utils-0.5.0/manim_course_utils/markdown_tex_template.py
+-rw-r--r--   0        0        0     1920 2023-05-11 22:32:31.604716 manim_course_utils-0.5.0/manim_course_utils/mobject_description.py
+-rw-r--r--   0        0        0      520 2023-05-17 16:37:52.153158 manim_course_utils-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.5.0/README.md
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.5.0/PKG-INFO
```

### Comparing `manim_course_utils-0.4.0/manim_course_utils/animation_description.py` & `manim_course_utils-0.5.0/manim_course_utils/animation_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.4.0/manim_course_utils/mobject_description.py` & `manim_course_utils-0.5.0/manim_course_utils/mobject_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.4.0/pyproject.toml` & `manim_course_utils-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "manim-course-utils"
-version = "0.4.0"
+version = "0.5.0"
 description = "Para el curso de ManimCE de MathLike"
 homepage = "https://github.com/MathLike/manim-course-utils"
 repository = "https://github.com/MathLike/manim-course-utils"
 authors = ["MathLike <benjamin.ubilla@uc.cl>"]
 readme = "README.md"
 packages = [{include = "manim_course_utils"}]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.7,<3.12"
 manim = "^0.17.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `manim_course_utils-0.4.0/PKG-INFO` & `manim_course_utils-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: manim-course-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: Para el curso de ManimCE de MathLike
 Home-page: https://github.com/MathLike/manim-course-utils
 Author: MathLike
 Author-email: benjamin.ubilla@uc.cl
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: manim (>=0.17.3,<0.18.0)
 Project-URL: Repository, https://github.com/MathLike/manim-course-utils
 Description-Content-Type: text/markdown
 
 # Utilidades del curso de Manim
```

