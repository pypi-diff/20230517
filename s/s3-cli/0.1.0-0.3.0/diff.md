# Comparing `tmp/s3-cli-0.1.0.tar.gz` & `tmp/s3_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3-cli-0.1.0.tar", max compression
+gzip compressed data, was "s3_cli-0.3.0.tar", max compression
```

## Comparing `s3-cli-0.1.0.tar` & `s3_cli-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      325 2022-06-28 16:38:31.360378 s3-cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2022-06-28 16:37:25.421830 s3-cli-0.1.0/s3_cli/__init__.py
--rw-r--r--   0        0        0     2536 2022-06-28 16:38:03.072324 s3-cli-0.1.0/s3_cli/main.py
--rw-r--r--   0        0        0      590 2022-06-28 16:39:05.654676 s3-cli-0.1.0/setup.py
--rw-r--r--   0        0        0      289 2022-06-28 16:39:05.655416 s3-cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      369 2023-05-17 09:05:39.258708 s3_cli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-06-28 16:37:25.421830 s3_cli-0.3.0/s3_cli/__init__.py
+-rw-r--r--   0        0        0     2557 2023-05-17 09:00:08.491176 s3_cli-0.3.0/s3_cli/main.py
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 s3_cli-0.3.0/PKG-INFO
```

### Comparing `s3-cli-0.1.0/s3_cli/main.py` & `s3_cli-0.3.0/s3_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def download(self, from_location, to_location):
         self.client.download_file(self.bucket, from_location, to_location)
 
     def stream(self, filename, out_dir, file):
         print("start stream for file: ", f"{out_dir}/{filename}")
         output = BytesIO()
-        file.to_excel(output, index=False)
+        file.to_excel(output, index=False, engine='xlsxwriter')
         self.put(file=output.getvalue(), key=f"{out_dir}/{filename}")
         print("finish stream")
 
 
 class LocalFS:
     class DoesNotExist(Exception):
         pass
```

