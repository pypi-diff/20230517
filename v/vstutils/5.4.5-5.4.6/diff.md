# Comparing `tmp/vstutils-5.4.5.tar.gz` & `tmp/vstutils-5.4.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.5.tar", last modified: Mon May 15 04:02:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

