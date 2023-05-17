# Comparing `tmp/piicli-0.0.5.tar.gz` & `tmp/piicli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piicli-0.0.5.tar", max compression
+gzip compressed data, was "piicli-0.0.6.tar", max compression
```

## Comparing `piicli-0.0.5.tar` & `piicli-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.5/LICENSE
--rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.5/README.md
--rw-r--r--   0        0        0      718 2023-05-17 12:49:58.590200 piicli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.5/src/piicli/__init__.py
--rw-r--r--   0        0        0     4575 2023-05-17 12:49:04.544077 piicli-0.0.5/src/piicli/main.py
--rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.5/src/piicli/utils.py
--rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 09:44:17.758376 piicli-0.0.6/LICENSE
+-rw-r--r--   0        0        0      170 2023-05-16 09:44:41.423465 piicli-0.0.6/README.md
+-rw-r--r--   0        0        0      718 2023-05-17 12:51:05.481390 piicli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 11:11:21.834362 piicli-0.0.6/src/piicli/__init__.py
+-rw-r--r--   0        0        0     4533 2023-05-17 12:51:05.485518 piicli-0.0.6/src/piicli/main.py
+-rw-r--r--   0        0        0      331 2023-05-17 10:39:02.171793 piicli-0.0.6/src/piicli/utils.py
+-rw-r--r--   0        0        0     1254 1970-01-01 00:00:00.000000 piicli-0.0.6/PKG-INFO
```

### Comparing `piicli-0.0.5/LICENSE` & `piicli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `piicli-0.0.5/src/piicli/main.py` & `piicli-0.0.6/src/piicli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,28 @@
     region = 'ap-south-1'
     s3 = boto3.client('s3', aws_access_key_id=access_key, aws_secret_access_key=secret_key, region_name=region)
     return s3
 
 
 def check_for_updates(config_path):
     package_name = "piicli"
-    # try:
-    #     current_version = pkg_resources.get_distribution(package_name).version
-    # except pkg_resources.DistributionNotFound:
-    #     print(f"{package_name} is not installed.")
-    #     return
+    try:
+        current_version = pkg_resources.get_distribution(package_name).version
+    except pkg_resources.DistributionNotFound:
+        print(f"{package_name} is not installed.")
+        return
 
-    current_version = "0.0.2"
     response = requests.get(f'https://pypi.org/pypi/{package_name}/json')
     latest_version = response.json()['info']['version']
 
     conf = read_yaml(config_path)
     if current_version != latest_version:
         print(f"Update available, updating to latest version: {latest_version}")
         conf["version"] = latest_version
-        # subprocess.call(f"pip3 install --upgrade {package_name}", shell=True)
+        subprocess.call(f"pip3 install --upgrade {package_name}", shell=True)
         print("Updated lib to latest version")
         write_yaml(config_path, conf)
     else:
         print("No updates available")
 
 
 def download(s3, bucket_name, folder_name, file_name, download_path):
@@ -106,15 +105,15 @@
 #         os.chmod(binary_path, 0o755)
 #         subprocess.run(binary_path)
 #
 #     except Exception as e:
 #         print(f"Something went wrong, err: {e}")
 
 def print_version():
-    print("running 0.0.5")
+    print("running 0.0.6")
 
 
 def execute_binary():
     try:
         home = os.getenv("HOME")
         metadata_dir = home + "/piicli_metadata"
         config_file = "conf.yaml"
```

### Comparing `piicli-0.0.5/PKG-INFO` & `piicli-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piicli
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author: Shubham Dogra
 Author-email: shubham.dogra@pingsafe.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

