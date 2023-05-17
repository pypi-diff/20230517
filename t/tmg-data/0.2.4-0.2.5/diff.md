# Comparing `tmp/tmg-data-0.2.4.tar.gz` & `tmp/tmg_data-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmg-data-0.2.4.tar", last modified: Tue Mar  7 14:28:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

