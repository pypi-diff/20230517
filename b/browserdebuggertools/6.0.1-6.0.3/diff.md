# Comparing `tmp/browserdebuggertools-6.0.1.tar.gz` & `tmp/browserdebuggertools-6.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/browserdebuggertools-6.0.1.tar", last modified: Mon May 17 11:33:43 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

