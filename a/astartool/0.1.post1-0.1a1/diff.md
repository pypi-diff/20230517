# Comparing `tmp/astartool-0.1.post1.tar.gz` & `tmp/astartool-0.1a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\astartool-0.1.post1.tar", last modified: Fri Apr 29 05:09:31 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

