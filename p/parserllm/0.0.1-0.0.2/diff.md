# Comparing `tmp/parserllm-0.0.1.tar.gz` & `tmp/parserllm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parserllm-0.0.1.tar", max compression
+gzip compressed data, was "parserllm-0.0.2.tar", max compression
```

## Comparing `parserllm-0.0.1.tar` & `parserllm-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-05-06 21:53:10.969573 parserllm-0.0.1/LICENSE
--rw-r--r--   0        0        0      248 2023-05-06 22:07:08.764954 parserllm-0.0.1/README.md
--rw-r--r--   0        0        0       43 2023-05-06 22:01:29.809327 parserllm-0.0.1/parserllm/__init__.py
--rw-r--r--   0        0        0     2165 2023-05-06 22:06:52.347430 parserllm-0.0.1/parserllm/parserllm.py
--rw-r--r--   0        0        0      675 2023-05-06 21:55:33.573631 parserllm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 parserllm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-06 21:53:10.969573 parserllm-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2383 2023-05-14 16:12:53.585300 parserllm-0.0.2/README.md
+-rw-r--r--   0        0        0       43 2023-05-06 22:01:29.809327 parserllm-0.0.2/parserllm/__init__.py
+-rw-r--r--   0        0        0     2093 2023-05-17 01:12:13.433437 parserllm-0.0.2/parserllm/parserllm.py
+-rw-r--r--   0        0        0      675 2023-05-17 01:12:39.238753 parserllm-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3143 1970-01-01 00:00:00.000000 parserllm-0.0.2/PKG-INFO
```

### Comparing `parserllm-0.0.1/LICENSE` & `parserllm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parserllm-0.0.1/pyproject.toml` & `parserllm-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parserllm"
-version = "0.0.1"
+version = "0.0.2"
 description = "Force LLMs to use a specific context-free grammar in completions"
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "parserllm"}]
 keywords = [
```

