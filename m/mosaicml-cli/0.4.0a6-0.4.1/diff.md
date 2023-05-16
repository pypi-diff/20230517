# Comparing `tmp/mosaicml-cli-0.4.0a6.tar.gz` & `tmp/mosaicml_cli-0.4.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.0a6.tar", last modified: Tue May  9 23:14:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

