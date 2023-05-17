# Comparing `tmp/ubiquity-student-0.8.2.tar.gz` & `tmp/ubiquity_student-1.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ubiquity-student-0.8.2.tar", last modified: Fri Jan 20 09:18:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

