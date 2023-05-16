# Comparing `tmp/calysto_scheme-1.4.7.tar.gz` & `tmp/calysto_scheme-1.4.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calysto_scheme-1.4.7.tar", last modified: Thu Nov 25 16:38:00 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

