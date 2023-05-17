# Comparing `tmp/covidillness-0.0.5.tar.gz` & `tmp/covidillness-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covidillness-0.0.5.tar", last modified: Tue Nov  8 17:18:18 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

