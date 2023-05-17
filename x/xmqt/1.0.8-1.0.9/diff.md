# Comparing `tmp/xmqt-1.0.8.tar.gz` & `tmp/xmqt-1.0.9-py3.6.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xmqt-1.0.8.tar", last modified: Thu Jan 20 03:51:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

