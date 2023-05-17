# Comparing `tmp/fairscape_cli-0.1.5a1.tar.gz` & `tmp/fairscape_cli-0.1.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairscape_cli-0.1.5a1.tar", max compression
+gzip compressed data, was "fairscape_cli-0.1.5a2.tar", max compression
```

## Comparing `fairscape_cli-0.1.5a1.tar` & `fairscape_cli-0.1.5a2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a1/LICENSE
--rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/README.md
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/__init__.py
--rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/cache.py
--rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a1/fairscape_cli/apps/describe.py
--rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/fairscape.py
--rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/list.py
--rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/__init__.py
--rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/computation.py
--rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/dataset.py
--rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/models/software.py
--rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/objects.py
--rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/rocrate.py
--rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/utils.py
--rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/apps/validator.py
--rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/main.py
--rw-r--r--   0        0        0      285 2023-05-11 18:22:39.597260 fairscape_cli-0.1.5a1/fairscape_cli/models/__init__.py
--rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/models/computation.py
--rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/models/dataset.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/models/models.py
--rw-r--r--   0        0        0     5033 2023-05-11 18:45:00.117305 fairscape_cli-0.1.5a1/fairscape_cli/models/rocrate.py
--rw-r--r--   0        0        0    13036 2023-05-10 19:09:33.371675 fairscape_cli-0.1.5a1/fairscape_cli/models/schema.py
--rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a1/fairscape_cli/models/software.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/__init__.py
--rw-r--r--   0        0        0    15800 2023-05-11 18:51:57.277320 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/rocrate.py
--rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5a1/fairscape_cli/rocrate/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/validate/__init__.py
--rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a1/fairscape_cli/validate/validate_json.py
--rw-r--r--   0        0        0     1517 2023-05-11 18:52:55.677321 fairscape_cli-0.1.5a1/pyproject.toml
--rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-06 17:27:00.899279 fairscape_cli-0.1.5a2/LICENSE
+-rw-r--r--   0        0        0     4058 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/cache.py
+-rw-r--r--   0        0        0      510 2023-03-27 17:08:49.098247 fairscape_cli-0.1.5a2/fairscape_cli/apps/describe.py
+-rw-r--r--   0        0        0      764 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/fairscape.py
+-rw-r--r--   0        0        0       89 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/list.py
+-rw-r--r--   0        0        0      173 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/__init__.py
+-rw-r--r--   0        0        0      340 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/computation.py
+-rw-r--r--   0        0        0     2559 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/dataset.py
+-rw-r--r--   0        0        0     1890 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/models/software.py
+-rw-r--r--   0        0        0     8135 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/objects.py
+-rw-r--r--   0        0        0     3369 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/rocrate.py
+-rw-r--r--   0        0        0     2276 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/utils.py
+-rw-r--r--   0        0        0     2677 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/apps/validator.py
+-rw-r--r--   0        0        0      397 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/main.py
+-rw-r--r--   0        0        0      285 2023-05-11 18:22:39.597260 fairscape_cli-0.1.5a2/fairscape_cli/models/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/models/computation.py
+-rw-r--r--   0        0        0      205 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/models/dataset.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/models/models.py
+-rw-r--r--   0        0        0     4861 2023-05-17 17:28:34.300407 fairscape_cli-0.1.5a2/fairscape_cli/models/rocrate.py
+-rw-r--r--   0        0        0    13053 2023-05-15 16:54:08.216085 fairscape_cli-0.1.5a2/fairscape_cli/models/schema.py
+-rw-r--r--   0        0        0      128 2023-04-17 19:02:18.829104 fairscape_cli-0.1.5a2/fairscape_cli/models/software.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/__init__.py
+-rw-r--r--   0        0        0    16263 2023-05-17 17:15:12.990546 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/rocrate.py
+-rw-r--r--   0        0        0     1326 2023-04-17 19:02:18.839104 fairscape_cli-0.1.5a2/fairscape_cli/rocrate/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 16:53:18.146083 fairscape_cli-0.1.5a2/fairscape_cli/schema/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-15 16:57:34.786089 fairscape_cli-0.1.5a2/fairscape_cli/schema/schema.py
+-rw-r--r--   0        0        0        0 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/validate/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-27 17:08:49.108247 fairscape_cli-0.1.5a2/fairscape_cli/validate/validate_json.py
+-rw-r--r--   0        0        0     1499 2023-05-17 21:20:04.727973 fairscape_cli-0.1.5a2/pyproject.toml
+-rw-r--r--   0        0        0     4949 1970-01-01 00:00:00.000000 fairscape_cli-0.1.5a2/PKG-INFO
```

### Comparing `fairscape_cli-0.1.5a1/LICENSE` & `fairscape_cli-0.1.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/README.md` & `fairscape_cli-0.1.5a2/README.md`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/fairscape.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/fairscape.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/models/dataset.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/models/dataset.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/models/software.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/models/software.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/objects.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/objects.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/rocrate.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/rocrate.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/utils.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/apps/validator.py` & `fairscape_cli-0.1.5a2/fairscape_cli/apps/validator.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/models/rocrate.py` & `fairscape_cli-0.1.5a2/fairscape_cli/models/rocrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -114,27 +114,21 @@
 
         Marshals a given model into JSON-LD, opens the ro-crate-metadata.json,
         appends the new metadata to the @graph, and overwrites the ro-crate-metadata.json
         '''
 
         metadata_path = self.path
 
-        # open the ro-crate-metadata.json
-        with metadata_path.open("r") as rocrate_metadata_file:
+        with metadata_path.open("r+") as rocrate_metadata_file:
             rocrate_metadata = json.load(rocrate_metadata_file)
-
-            # TODO check if the file is redundant
-     
+            
             # add to the @graph
             rocrate_metadata['@graph'].append(model.dict(by_alias=True))
-        
-        # overwrite the ro-crate-metadata.json file
-        with metadata_path.open("w") as f:
-            json_object = json.dumps(rocrate_metadata, indent=2)
-            f.write(json_object)
+            rocrate_metadata_file.seek(0)
+            json.dump(rocrate_metadata, rocrate_metadata_file, indent=2)
 
 
 
     def registerDataset(self, Dataset):
         self.registerObject(model=Dataset)
```

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/models/schema.py` & `fairscape_cli-0.1.5a2/fairscape_cli/models/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,19 +153,21 @@
             )
 
         if width != self.ImageSchema.width:
             raise ImageValidationException(
                 message=f"Image Width {width} != {self.ImageSchema.width}"
             )
 
+
 class FiletypeEnum(str, Enum):
     """List of supported filetypes with normative naming
     """
     csv = "csv"
     tsv = "tsv"
+    hcx = "hcx"
     
 
 class DatatypeEnum(str, Enum):
     """
     A Datatype Enum for supported types for validation
 
     These Choices are to be expanded until covering the full spec from [CSV on the Web](https://w3c.github.io/csvw/metadata/#datatypes)
```

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/rocrate/rocrate.py` & `fairscape_cli-0.1.5a2/fairscape_cli/rocrate/rocrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 @click.option('--name',    required=True, prompt = "Software Name")
 @click.option('--author',  required=True, prompt = "Author Name")
 @click.option('--version', required=True, prompt = "Software Version")
 @click.option('--description', required = True, prompt = "Software Description")
 @click.option('--file-format', required = True, prompt = "File Format of Software")
 @click.option('--url',     required = False)
 @click.option('--date-modified', required=False)
-@click.option('--filepath', required=True)
+@click.option('--filepath', required=False)
 @click.option('--used-by-computation', required=False, multiple=True)
 @click.option('--associated-publication', required=False)
 @click.option('--additional-documentation', required=False)
 def registerSoftware(
     rocrate_path: pathlib.Path,
     guid: str,
     name: str,
@@ -162,32 +162,41 @@
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate(path=metadata_path)
 
-    try:
-        software_model = Software(   
-            **{
+
+    software_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Software",
             "url": url,
             "name": name,
             "author": author,
             "dateModified": date_modified,
             "description": description,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": file_format,
             "usedByComputation": used_by_computation,
-            "contentUrl": "file://" + filepath
             }
-        )
+
+    if filepath != "" and filepath is not None:
+            software_metadata["contentUrl"] = f"file://{str(filepath)}" 
+    else:
+        # if filepath is null and url is null
+        # raise an error
+        if url == "" or url is None:
+            click.echo("Software Validation Error: url and filepath cannot both be null")
+            click.Abort()
+
+    try:
+        software_model = Software(**software_metadata)
 
     except ValidationError as e:
         click.echo("Software Validation Error")
         click.echo(e)
         click.Abort()
         
     crate.registerSoftware(software_model)
@@ -233,32 +242,36 @@
     # ro-crate-metadata.json should be a local file
     if metadata_path.exists() != True:
         click.echo(f"Cannot Find RO-Crate Metadata: {metadata_path}")
         click.Abort()
 
     crate = ROCrate(path=metadata_path)
 
-    try:
-        dataset_model = Dataset(   
-            **{
+    dataset_metadata = {
             "@id": guid,
             "@type": "https://w3id.org/EVI#Dataset",
             "url": url,
             "author": author,
             "name": name,
             "description": description,
             "datePublished": date_published,
             "version": version,
             "associatedPublication": associated_publication,
             "additionalDocumentation": additional_documentation,
             "format": data_format,
             "derivedFrom": derived_from,
             "usedBy": used_by
             }
-        )
+
+    if filepath != "" and filepath is not None:
+        dataset_metadata["contentUrl"] = f"file://{str(filepath)}" 
+
+
+    try:
+        dataset_model = Dataset(**dataset_metadata)
 
     except ValidationError as e:
         click.echo("Dataset Validation Error")
         click.echo(e)
         click.Abort()
     
     crate.registerDataset(dataset_model)
```

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/rocrate/utils.py` & `fairscape_cli-0.1.5a2/fairscape_cli/rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/fairscape_cli/validate/validate_json.py` & `fairscape_cli-0.1.5a2/fairscape_cli/validate/validate_json.py`

 * *Files identical despite different names*

### Comparing `fairscape_cli-0.1.5a1/pyproject.toml` & `fairscape_cli-0.1.5a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "fairscape-cli"
-version = "0.1.0"
 description = "CLI tool for B2AI metadata validation and ROCrate creation"
 readme = "README.md"
 authors = [
         { name = "Max Levinson",    email = "mal8ch@virginia.edu"},
         { name = "Sadnan Al Manir", email = "sadnanalmanir@gmail.com"},
         { name = "Tim Clark",       email = "twc8q@virginia.edu"}
 ]
@@ -23,15 +22,15 @@
 
 [project.urls]
 Homepage = "https://github.com/fairscape/fairscape-cli"
 
 
 [tool.poetry]
 name = "fairscape-cli"
-version = "0.1.5a1"
+version = "0.1.5a2"
 description = "A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API"
 authors = ["mlev71 <max.adam.levinson@gmail.com>"]
 license = "LICENSE"
 readme = "README.md"
 packages = [{include = "fairscape_cli"}]
```

### Comparing `fairscape_cli-0.1.5a1/PKG-INFO` & `fairscape_cli-0.1.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairscape-cli
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: A cli for validating metadata, packaging ROCrates, and interacting with the FAIRSCAPE API
 License: LICENSE
 Author: mlev71
 Author-email: max.adam.levinson@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

